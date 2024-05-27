# Comparing `tmp/xingpyc-0.2.2.tar.gz` & `tmp/xingpyc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.2.2.tar", last modified: Mon May 27 18:55:26 2024, max compression
+gzip compressed data, was "xingpyc-0.2.3.tar", last modified: Mon May 27 19:30:07 2024, max compression
```

## Comparing `xingpyc-0.2.2.tar` & `xingpyc-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 18:55:26.892299 xingpyc-0.2.2/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 18:55:26.891937 xingpyc-0.2.2/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.2/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-27 18:55:23.000000 xingpyc-0.2.2/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-27 18:55:26.892364 xingpyc-0.2.2/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 18:55:26.889237 xingpyc-0.2.2/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 18:55:26.890252 xingpyc-0.2.2/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     9041 2024-05-27 18:55:03.000000 xingpyc-0.2.2/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.2/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 18:55:26.891394 xingpyc-0.2.2/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 18:55:26.000000 xingpyc-0.2.2/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-27 18:55:26.000000 xingpyc-0.2.2/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-27 18:55:26.000000 xingpyc-0.2.2/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-27 18:55:26.000000 xingpyc-0.2.2/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-27 18:55:26.000000 xingpyc-0.2.2/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 18:55:26.891077 xingpyc-0.2.2/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.2/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 19:30:07.964082 xingpyc-0.2.3/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 19:30:07.963812 xingpyc-0.2.3/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.3/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-27 19:29:39.000000 xingpyc-0.2.3/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-27 19:30:07.964132 xingpyc-0.2.3/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 19:30:07.961468 xingpyc-0.2.3/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 19:30:07.962355 xingpyc-0.2.3/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     9042 2024-05-27 19:30:02.000000 xingpyc-0.2.3/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.3/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 19:30:07.963507 xingpyc-0.2.3/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 19:30:07.000000 xingpyc-0.2.3/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-27 19:30:07.000000 xingpyc-0.2.3/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-27 19:30:07.000000 xingpyc-0.2.3/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-27 19:30:07.000000 xingpyc-0.2.3/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-27 19:30:07.000000 xingpyc-0.2.3/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 19:30:07.963337 xingpyc-0.2.3/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.3/tests/test1.py
```

### Comparing `xingpyc-0.2.2/PKG-INFO` & `xingpyc-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.2.2/pyproject.toml` & `xingpyc-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.2.2/src/xingpyc/__init__.py` & `xingpyc-0.2.3/src/xingpyc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,20 +134,20 @@
                     f.write(content)
                 del self.blockbuffers[client_id] # clean buffer
 
         except Exception as e:
             print(f"Error in websocket communication: {e}")
             return
 
-    async def global_send(self, blocksize=30000):
+    async def global_send(self, blocksize=100000):
         print("start result->sender loop")
         loopCount = 0
         while True:
             loopCount += 1
-            if loopCount % 20 == 0 and self.cloudClient is not None:
+            if loopCount % 50 == 0 and self.cloudClient is not None:
                 self.cloudClient.send_bytes("check     0000000000")
                 print("check to cloud")
 
             if len(os.listdir("results")) > 0:
                 for file in os.listdir("results"):
                     try:
                         with open(f"results/{file}", "rb") as f:
```

### Comparing `xingpyc-0.2.2/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.2.3/src/xingpyc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

