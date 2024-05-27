# Comparing `tmp/ricklib-0.0.3.tar.gz` & `tmp/ricklib-0.0.4.tar.gz`

## Comparing `ricklib-0.0.3.tar` & `ricklib-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ricklib-0.0.3/src/ricklib/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 ricklib-0.0.3/src/ricklib/audio.py
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 ricklib-0.0.3/src/ricklib/pngenerator.py
--rw-r--r--   0        0        0   352844 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/audio.wav
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/graphic_test.py
--rw-r--r--   0        0        0   125130 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/testc.png
--rw-r--r--   0        0        0    65865 2020-02-02 00:00:00.000000 ricklib-0.0.3/tests/testg.png
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ricklib-0.0.3/LICENSE
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ricklib-0.0.3/README.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ricklib-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 ricklib-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0   352844 2020-02-02 00:00:00.000000 ricklib-0.0.4/audio.wav
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ricklib-0.0.4/src/ricklib/__init__.py
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 ricklib-0.0.4/src/ricklib/audio.py
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 ricklib-0.0.4/src/ricklib/pngenerator.py
+-rw-r--r--   0        0        0   352844 2020-02-02 00:00:00.000000 ricklib-0.0.4/tests/audio.wav
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ricklib-0.0.4/tests/graphic_test.py
+-rw-r--r--   0        0        0   125130 2020-02-02 00:00:00.000000 ricklib-0.0.4/tests/testc.png
+-rw-r--r--   0        0        0    65865 2020-02-02 00:00:00.000000 ricklib-0.0.4/tests/testg.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ricklib-0.0.4/LICENSE
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 ricklib-0.0.4/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ricklib-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 ricklib-0.0.4/PKG-INFO
```

### Comparing `ricklib-0.0.3/src/ricklib/audio.py` & `ricklib-0.0.4/src/ricklib/audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,20 @@
 
 
 def test_data() -> list:
     data = []
     length = sec2smp(seconds=2)
     hz = 400
     for i in range(0, length):
-        data.append(math.sin(2 * math.pi * hz * i / DEFAULT_SAMPLE_RATE))
+        f = math.sin(2 * math.pi * hz * i / DEFAULT_SAMPLE_RATE)
+        if f < -1:
+            f = -1
+        elif f > 1:
+            f = 1
+        data.append(f)
     
     return data
 
 
 def hard_clip(data: list, threshold: float) -> list:
     # Hard clip the audio data
     # data: list of floats
@@ -81,20 +86,23 @@
     for i in range(1, len(data)):
         filtered_data.append(data[i] - data[i - 1] + a * filtered_data[i - 1])
 
     return filtered_data
 
 
 def floats2bytes(data: list, bit_depth: int = DEFAULT_BIT_DEPTH) -> bytes:
-    # Convert a list of floats to a list of bytes
+    # Convert a list of floats in [-1, 1] to a list of bytes
     # data: list of floats
     # bit_depth: int, bit depth of the audio data
 
-    # The maximum value of the audio data
-    max_val = 2 ** (bit_depth - 3) - 1
+    # Make sure the floats are in the correct range
+    data = hard_clip(data, 1.0)
+
+    # The maximum value of the audio data with one bit reserved for the sign
+    max_val = 2 ** (bit_depth - 1) - 1
 
     # Convert the floats to ints
     data = [int(d * max_val) for d in data]
 
     # Convert the integers to bytes
     data = [d.to_bytes(bit_depth // 8, 'little', signed=True) for d in data]
```

### Comparing `ricklib-0.0.3/src/ricklib/pngenerator.py` & `ricklib-0.0.4/src/ricklib/pngenerator.py`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.3/tests/audio.wav` & `ricklib-0.0.4/tests/audio.wav`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.3/tests/testc.png` & `ricklib-0.0.4/tests/testc.png`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.3/tests/testg.png` & `ricklib-0.0.4/tests/testg.png`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.3/LICENSE` & `ricklib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.3/pyproject.toml` & `ricklib-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ricklib"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   {name="Richard (Rick) Howell", email="rick.howell.arts@gmail.com"},
 ]
 description = "A small package for personal use including useful operations."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ricklib-0.0.3/PKG-INFO` & `ricklib-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ricklib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package for personal use including useful operations.
 Project-URL: Homepage, https://github.com/rick-howell/ricklib
 Project-URL: Issues, https://github.com/rick-howell/ricklib/issues
 Author-email: "Richard (Rick) Howell" <rick.howell.arts@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 rick-howell
```

