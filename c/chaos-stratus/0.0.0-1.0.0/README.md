# Comparing `tmp/chaos_stratus-0.0.0.tar.gz` & `tmp/chaos_stratus-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaos_stratus-0.0.0.tar", last modified: Mon May 27 10:33:42 2024, max compression
+gzip compressed data, was "chaos_stratus-1.0.0.tar", last modified: Mon May 27 12:03:09 2024, max compression
```

## Comparing `chaos_stratus-0.0.0.tar` & `chaos_stratus-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 10:33:42.394674 chaos_stratus-0.0.0/
--rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3444 2024-05-27 10:33:42.394674 chaos_stratus-0.0.0/PKG-INFO
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)     2975 2024-05-27 10:27:03.000000 chaos_stratus-0.0.0/README.md
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      635 2024-05-27 10:09:11.000000 chaos_stratus-0.0.0/pyproject.toml
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       38 2024-05-27 10:33:42.394674 chaos_stratus-0.0.0/setup.cfg
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 10:33:42.394674 chaos_stratus-0.0.0/src/
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 10:33:42.394674 chaos_stratus-0.0.0/src/chaos_stratus/
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      234 2024-05-27 09:28:34.000000 chaos_stratus-0.0.0/src/chaos_stratus/__init__.py
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      426 2024-05-27 07:43:44.000000 chaos_stratus-0.0.0/src/chaos_stratus/__main__.py
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)    11668 2024-05-27 09:03:17.000000 chaos_stratus-0.0.0/src/chaos_stratus/stratus.py
-drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 10:33:42.394674 chaos_stratus-0.0.0/src/chaos_stratus.egg-info/
--rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3444 2024-05-27 10:33:42.000000 chaos_stratus-0.0.0/src/chaos_stratus.egg-info/PKG-INFO
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      277 2024-05-27 10:33:42.000000 chaos_stratus-0.0.0/src/chaos_stratus.egg-info/SOURCES.txt
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)        1 2024-05-27 10:33:42.000000 chaos_stratus-0.0.0/src/chaos_stratus.egg-info/dependency_links.txt
--rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       14 2024-05-27 10:33:42.000000 chaos_stratus-0.0.0/src/chaos_stratus.egg-info/top_level.txt
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:03:09.694220 chaos_stratus-1.0.0/
+-rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3444 2024-05-27 12:03:09.694220 chaos_stratus-1.0.0/PKG-INFO
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)     2975 2024-05-27 10:27:03.000000 chaos_stratus-1.0.0/README.md
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      631 2024-05-27 12:03:05.000000 chaos_stratus-1.0.0/pyproject.toml
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       38 2024-05-27 12:03:09.694220 chaos_stratus-1.0.0/setup.cfg
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:03:09.694220 chaos_stratus-1.0.0/src/
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:03:09.694220 chaos_stratus-1.0.0/src/chaos_stratus/
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      234 2024-05-27 09:28:34.000000 chaos_stratus-1.0.0/src/chaos_stratus/__init__.py
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      426 2024-05-27 07:43:44.000000 chaos_stratus-1.0.0/src/chaos_stratus/__main__.py
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)    11668 2024-05-27 09:03:17.000000 chaos_stratus-1.0.0/src/chaos_stratus/stratus.py
+drwxrwxr-x   0 jbartle9  (1000) jbartle9  (1000)        0 2024-05-27 12:03:09.694220 chaos_stratus-1.0.0/src/chaos_stratus.egg-info/
+-rw-r--r--   0 jbartle9  (1000) jbartle9  (1000)     3444 2024-05-27 12:03:09.000000 chaos_stratus-1.0.0/src/chaos_stratus.egg-info/PKG-INFO
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)      277 2024-05-27 12:03:09.000000 chaos_stratus-1.0.0/src/chaos_stratus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)        1 2024-05-27 12:03:09.000000 chaos_stratus-1.0.0/src/chaos_stratus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbartle9  (1000) jbartle9  (1000)       14 2024-05-27 12:03:09.000000 chaos_stratus-1.0.0/src/chaos_stratus.egg-info/top_level.txt
```

### Comparing `chaos_stratus-0.0.0/PKG-INFO` & `chaos_stratus-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaos-stratus
-Version: 0.0.0
+Version: 1.0.0
 Summary: Python tools used to interact with (appropriately compiled) Chaos Stratus effect libraries
 Author-email: Martin Bartlett <martin.j.bartlett@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/bassmanitram/chaos-stratus-python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
```

### Comparing `chaos_stratus-0.0.0/README.md` & `chaos_stratus-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `chaos_stratus-0.0.0/pyproject.toml` & `chaos_stratus-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chaos-stratus"
-dynamic = ["version"]
+version = "1.0.0"
 description = 'Python tools used to interact with (appropriately compiled) Chaos Stratus effect libraries'
 readme = "README.md"
 authors = [{ name = "Martin Bartlett", email = "martin.j.bartlett@gmail.com" }]
 license = {text = "MIT License"}
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `chaos_stratus-0.0.0/src/chaos_stratus/stratus.py` & `chaos_stratus-1.0.0/src/chaos_stratus/stratus.py`

 * *Files identical despite different names*

### Comparing `chaos_stratus-0.0.0/src/chaos_stratus.egg-info/PKG-INFO` & `chaos_stratus-1.0.0/src/chaos_stratus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaos-stratus
-Version: 0.0.0
+Version: 1.0.0
 Summary: Python tools used to interact with (appropriately compiled) Chaos Stratus effect libraries
 Author-email: Martin Bartlett <martin.j.bartlett@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/bassmanitram/chaos-stratus-python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
```

