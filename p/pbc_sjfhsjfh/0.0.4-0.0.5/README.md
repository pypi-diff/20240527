# Comparing `tmp/pbc_sjfhsjfh-0.0.4.tar.gz` & `tmp/pbc_sjfhsjfh-0.0.5.tar.gz`

## Comparing `pbc_sjfhsjfh-0.0.4.tar` & `pbc_sjfhsjfh-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/requirements.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/__init__.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/bin.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/phira_chart.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/utils/__init__.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/src/pbc/utils/fraction.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/src/pbc/__init__.py
+-rw-r--r--   0        0        0    13182 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/src/pbc/bin.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/src/pbc/phira_chart.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/src/pbc/utils/__init__.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/src/pbc/utils/fraction.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pbc_sjfhsjfh-0.0.5/PKG-INFO
```

### Comparing `pbc_sjfhsjfh-0.0.4/src/pbc/bin.py` & `pbc_sjfhsjfh-0.0.5/src/pbc/bin.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,16 @@
                     res = PhiraAnim()
                 else:
                     reader.reset_time()
                     PhiraAnim(keyframes=reader.array(f"KeyFrame:{newT}"))
                 if res.next:
                     res.next = read_opt(reader)
                 return res
+            return read_opt(reader)
+
         raise ValueError(f"Invalid type {T}")
 
     @staticmethod
     def write_binary(value: Any, writer: BinaryWriter, T: SupportBinName):
         match T:
             case "Byte":
                 return writer.io.write(bytes([value]))
@@ -314,14 +316,16 @@
                     for kf in cur.keyframes:
                         writer.write(kf, f"KeyFrame:{newT}")
                 if cur.next:
                     cur = cur.next
                 else:
                     writer.write_val(0, "Byte")
                     break
+            return
+
         raise ValueError(f"Invalid type {T}")
 
 
 def test():
     test = BytesIO()
     writer = BinaryWriter(test)
     writer.write(True, "Bool")
```

### Comparing `pbc_sjfhsjfh-0.0.4/src/pbc/phira_chart.py` & `pbc_sjfhsjfh-0.0.5/src/pbc/phira_chart.py`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.4/src/pbc/utils/fraction.py` & `pbc_sjfhsjfh-0.0.5/src/pbc/utils/fraction.py`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.4/LICENSE` & `pbc_sjfhsjfh-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pbc_sjfhsjfh-0.0.4/pyproject.toml` & `pbc_sjfhsjfh-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pbc_sjfhsjfh"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "sjfhsjfh", email = "sjfhsjfh@qq.com" }]
 description = "Phira chart structure package"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

