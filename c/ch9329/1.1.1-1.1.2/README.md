# Comparing `tmp/ch9329-1.1.1.tar.gz` & `tmp/ch9329-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.1.1.tar", last modified: Fri May 24 18:40:32 2024, max compression
+gzip compressed data, was "ch9329-1.1.2.tar", last modified: Mon May 27 09:21:29 2024, max compression
```

## Comparing `ch9329-1.1.1.tar` & `ch9329-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:40:32.482196 ch9329-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 18:40:28.000000 ch9329-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 18:40:28.000000 ch9329-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 18:40:32.482196 ch9329-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-24 18:40:28.000000 ch9329-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:40:32.482196 ch9329-1.1.1/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-24 18:40:28.000000 ch9329-1.1.1/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:40:32.482196 ch9329-1.1.1/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 18:40:32.000000 ch9329-1.1.1/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-24 18:40:32.000000 ch9329-1.1.1/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:40:32.000000 ch9329-1.1.1/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 18:40:32.000000 ch9329-1.1.1/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 18:40:32.000000 ch9329-1.1.1/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 18:40:28.000000 ch9329-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:40:32.482196 ch9329-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:28.999347 ch9329-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 09:21:24.000000 ch9329-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 09:21:24.000000 ch9329-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-27 09:21:28.999347 ch9329-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-27 09:21:24.000000 ch9329-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:28.999347 ch9329-1.1.2/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:28.999347 ch9329-1.1.2/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-27 09:21:24.000000 ch9329-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:21:28.999347 ch9329-1.1.2/setup.cfg
```

### Comparing `ch9329-1.1.1/LICENSE` & `ch9329-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.1/PKG-INFO` & `ch9329-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.1.1/README.md` & `ch9329-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.1/ch9329/config.py` & `ch9329-1.1.2/ch9329/config.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.1/ch9329/hid.py` & `ch9329-1.1.2/ch9329/hid.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.1/ch9329/keyboard.py` & `ch9329-1.1.2/ch9329/keyboard.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.1/ch9329/mouse.py` & `ch9329-1.1.2/ch9329/mouse.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,25 +25,42 @@
 def send_data_absolute(
     ser: Serial,
     x: int,
     y: int,
     ctrl: str = "null",
     x_max: int = 1920,
     y_max: int = 1080,
+    wheel_delta: int = 0,
 ) -> None:
+    # CMD_SEND_MS_ABS_DATA has exactly 7 bytes
+
+    # first byte is alwasys 0x02
     data = b"\x02"
+
+    # second byte is mouse button value
     data += ctrl_to_hex_mapping[ctrl]
+
+    # third and fourth bytes are x-coordinates
     x_cur = (4096 * x) // x_max
-    y_cur = (4096 * y) // y_max
     data += x_cur.to_bytes(2, byteorder="little")
+
+    # fifth and sixth bytes are y-coordinates
+    y_cur = (4096 * y) // y_max
     data += y_cur.to_bytes(2, byteorder="little")
-    if len(data) < 7:
-        data += b"\x00" * (7 - len(data))
-    else:
-        data = data[:7]
+
+    # seventh byte contains wheel data
+    # If it is 0x00, it means there is no scrolling action
+    # 0x01-0x7F, means scrolling upward
+    # 0x81-0xFF, means scroll down
+    if abs(wheel_delta) > 127:
+        raise RuntimeError("Maximum wheel delta allowed is 127.")
+    if wheel_delta >= 0:
+        data += (0x00 + wheel_delta).to_bytes(1)
+    elif wheel_delta < 0:
+        data += (0x100 + wheel_delta).to_bytes(1)
     packet = get_packet(HEAD, ADDR, CMD_ABS, LEN_ABS, data)
     ser.write(packet)
 
 
 def send_data_relative(
     ser: Serial, x: int, y: int, ctrl: str = "null"
 ) -> None:
@@ -88,7 +105,11 @@
 
 
 def click(ser: Serial, button: str = "left") -> None:
     press(ser, button)
     # 100 to 450 milliseconds delay for simulating natural behavior
     time.sleep(random.uniform(0.1, 0.45))
     release(ser)
+
+
+def wheel(ser: Serial, wheel: int = 1) -> None:
+    send_data_absolute(ser, 0, 0, wheel_delta=wheel)
```

### Comparing `ch9329-1.1.1/ch9329/utils.py` & `ch9329-1.1.2/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.1/ch9329.egg-info/PKG-INFO` & `ch9329-1.1.2/ch9329.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.1.1/pyproject.toml` & `ch9329-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.1.1"
+version = "1.1.2"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

