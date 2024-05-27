# Comparing `tmp/xingpyc-0.2.0.tar.gz` & `tmp/xingpyc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.2.0.tar", last modified: Sun May 26 06:59:51 2024, max compression
+gzip compressed data, was "xingpyc-0.2.1.tar", last modified: Mon May 27 16:18:30 2024, max compression
```

## Comparing `xingpyc-0.2.0.tar` & `xingpyc-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.289636 xingpyc-0.2.0/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:59:51.289446 xingpyc-0.2.0/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.0/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-26 06:59:47.000000 xingpyc-0.2.0/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:59:51.289674 xingpyc-0.2.0/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.287797 xingpyc-0.2.0/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.288354 xingpyc-0.2.0/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     8765 2024-05-26 06:59:27.000000 xingpyc-0.2.0/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.0/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.289247 xingpyc-0.2.0/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.289081 xingpyc-0.2.0/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.0/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 16:18:30.569545 xingpyc-0.2.1/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 16:18:30.569336 xingpyc-0.2.1/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.1/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-27 16:18:21.000000 xingpyc-0.2.1/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-27 16:18:30.569592 xingpyc-0.2.1/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 16:18:30.567308 xingpyc-0.2.1/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 16:18:30.568102 xingpyc-0.2.1/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8814 2024-05-27 16:18:14.000000 xingpyc-0.2.1/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.1/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 16:18:30.569126 xingpyc-0.2.1/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 16:18:30.000000 xingpyc-0.2.1/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-27 16:18:30.000000 xingpyc-0.2.1/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-27 16:18:30.000000 xingpyc-0.2.1/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-27 16:18:30.000000 xingpyc-0.2.1/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-27 16:18:30.000000 xingpyc-0.2.1/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 16:18:30.568985 xingpyc-0.2.1/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.1/tests/test1.py
```

### Comparing `xingpyc-0.2.0/PKG-INFO` & `xingpyc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.2.0/pyproject.toml` & `xingpyc-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.2.0/src/xingpyc/__init__.py` & `xingpyc-0.2.1/src/xingpyc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,15 @@
                             content = content.encode("utf-8")
                         if client_id == -1:
                             print("start sending to cloud")
                             count = 0
                             totalblocks = len(content) // blocksize
                             while len(content) > blocksize:
                                 Thread(target=self.cloudClient.send_bytes, args=(b"block     " + task_id + content[0:blocksize],)).start()
+                                time.sleep(0.01)
                                 #self.cloudClient.send_bytes(b"block     " + task_id + content[0:blocksize])
                                 content = content[blocksize:]
                                 print(f"sent block {count}/{totalblocks}")
                                 count += 1
 
                             self.cloudClient.send_bytes(header + task_id + content)
                             print("sent to cloud")
```

### Comparing `xingpyc-0.2.0/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.2.1/src/xingpyc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

