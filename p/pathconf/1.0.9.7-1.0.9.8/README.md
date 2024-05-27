# Comparing `tmp/pathconf-1.0.9.7.tar.gz` & `tmp/pathconf-1.0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathconf-1.0.9.7.tar", last modified: Sun Jan  7 20:41:20 2024, max compression
+gzip compressed data, was "pathconf-1.0.9.8.tar", last modified: Thu Jan 18 09:29:26 2024, max compression
```

## Comparing `pathconf-1.0.9.7.tar` & `pathconf-1.0.9.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:41:20.599734 pathconf-1.0.9.7/
--rw-r--r--   0 root         (0) root         (0)     5466 2024-01-07 20:41:20.599734 pathconf-1.0.9.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5087 2024-01-07 20:41:12.000000 pathconf-1.0.9.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:41:20.599734 pathconf-1.0.9.7/pathconf/
--rw-r--r--   0 root         (0) root         (0)      227 2024-01-07 20:41:12.000000 pathconf-1.0.9.7/pathconf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16222 2024-01-07 20:41:12.000000 pathconf-1.0.9.7/pathconf/pathconf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:41:20.599734 pathconf-1.0.9.7/pathconf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5466 2024-01-07 20:41:20.000000 pathconf-1.0.9.7/pathconf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      188 2024-01-07 20:41:20.000000 pathconf-1.0.9.7/pathconf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-07 20:41:20.000000 pathconf-1.0.9.7/pathconf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-07 20:41:20.000000 pathconf-1.0.9.7/pathconf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-07 20:41:20.599734 pathconf-1.0.9.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      861 2024-01-07 20:41:12.000000 pathconf-1.0.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 09:29:26.128254 pathconf-1.0.9.8/
+-rw-r--r--   0 root         (0) root         (0)     5466 2024-01-18 09:29:26.128254 pathconf-1.0.9.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5087 2024-01-18 09:29:18.000000 pathconf-1.0.9.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 09:29:26.124254 pathconf-1.0.9.8/pathconf/
+-rw-r--r--   0 root         (0) root         (0)      227 2024-01-18 09:29:18.000000 pathconf-1.0.9.8/pathconf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16239 2024-01-18 09:29:18.000000 pathconf-1.0.9.8/pathconf/pathconf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 09:29:26.128254 pathconf-1.0.9.8/pathconf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5466 2024-01-18 09:29:26.000000 pathconf-1.0.9.8/pathconf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      188 2024-01-18 09:29:26.000000 pathconf-1.0.9.8/pathconf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-18 09:29:26.000000 pathconf-1.0.9.8/pathconf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-01-18 09:29:26.000000 pathconf-1.0.9.8/pathconf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-18 09:29:26.128254 pathconf-1.0.9.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      861 2024-01-18 09:29:18.000000 pathconf-1.0.9.8/setup.py
```

### Comparing `pathconf-1.0.9.7/PKG-INFO` & `pathconf-1.0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathconf
-Version: 1.0.9.7
+Version: 1.0.9.8
 Summary: Uses os.walk to find and catalogue a given file.
 Author: Sam Kirby
 Author-email: sam.kirby@gagamuller.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
```

### Comparing `pathconf-1.0.9.7/README.md` & `pathconf-1.0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pathconf-1.0.9.7/pathconf/pathconf.py` & `pathconf-1.0.9.8/pathconf/pathconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import json
 import queue
+import errno
 import threading
 import logging
 from concurrent.futures import ThreadPoolExecutor, as_completed
 workers = os.cpu_count() * 3
 logging.basicConfig(level=logging.INFO,
                     format='%(asctime)s - %(levelname)s - %(message)s')
 
@@ -40,15 +41,15 @@
 
         if stop_event.is_set():
             break
 
         try:
             for dirpath, dirnames, filenames in os.walk(directory):
                 # Filter dirnames and filenames based on 'deprecated' flag
-                if deprecated:
+                if not deprecated:
                     dirnames[:] = [d for d in dirnames if 'Deprecated'
                                    not in d and 'deprecated' not in d]
 
                 if stop_event.is_set():
                     break
 
                 if search_folder:
@@ -85,15 +86,15 @@
             queue.task_done()
 
     return None
 
 
 def load_json_config(file_path):
     """
-    Load JSON configuration file. If the file does not exist, 
+    Load JSON configuration file. If the file does not exist,
     create a new empty JSON file.
 
     Parameters:
         file_path (str): Path to the JSON file.
 
     Returns:
         dict: Loaded JSON object or empty dictionary if file is invalid or new.
@@ -112,14 +113,15 @@
                 json.dump({}, f)
             logging.info(f"Created new config file: {file_path}")
             return {}
         else:
             logging.error(f"IOError occurred: {e}")
             return {}
 
+
 def remove(target_path):
     config_file_path = os.path.join(os.path.expanduser("~"),
                                     '.config', 'pathconf',
                                     '.file_paths.json')
 
     if os.path.isfile(config_file_path):
         config = load_json_config(config_file_path)
```

### Comparing `pathconf-1.0.9.7/pathconf.egg-info/PKG-INFO` & `pathconf-1.0.9.8/pathconf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathconf
-Version: 1.0.9.7
+Version: 1.0.9.8
 Summary: Uses os.walk to find and catalogue a given file.
 Author: Sam Kirby
 Author-email: sam.kirby@gagamuller.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
```

### Comparing `pathconf-1.0.9.7/setup.py` & `pathconf-1.0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Read the contents of your README file
 with open('README.md') as f:
     long_description = f.read()
 
 
 setup(
     name='pathconf',
-    version='1.0.9.7',  # Back to manual versioning
+    version='1.0.9.8',  # Back to manual versioning
     packages=find_packages(),
     description='Uses os.walk to find and catalogue a given file.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sam Kirby',
     author_email='sam.kirby@gagamuller.com',
     install_requires=[
```

