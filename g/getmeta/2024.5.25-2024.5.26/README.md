# Comparing `tmp/getmeta-2024.5.25.tar.gz` & `tmp/getmeta-2024.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getmeta-2024.5.25.tar", last modified: Sun May 26 01:53:49 2024, max compression
+gzip compressed data, was "getmeta-2024.5.26.tar", last modified: Mon May 27 13:18:09 2024, max compression
```

## Comparing `getmeta-2024.5.25.tar` & `getmeta-2024.5.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:53:49.498929 getmeta-2024.5.25/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 01:53:41.000000 getmeta-2024.5.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-26 01:53:49.498929 getmeta-2024.5.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-26 01:53:41.000000 getmeta-2024.5.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:53:49.498929 getmeta-2024.5.25/getmeta/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-26 01:53:41.000000 getmeta-2024.5.25/getmeta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-26 01:53:41.000000 getmeta-2024.5.25/getmeta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-26 01:53:41.000000 getmeta-2024.5.25/getmeta/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:53:49.498929 getmeta-2024.5.25/getmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 01:53:49.498929 getmeta-2024.5.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-26 01:53:41.000000 getmeta-2024.5.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:09.502251 getmeta-2024.5.26/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 13:18:03.000000 getmeta-2024.5.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-27 13:18:09.502251 getmeta-2024.5.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-27 13:18:03.000000 getmeta-2024.5.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:09.498251 getmeta-2024.5.26/getmeta/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-27 13:18:03.000000 getmeta-2024.5.26/getmeta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 13:18:03.000000 getmeta-2024.5.26/getmeta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-27 13:18:03.000000 getmeta-2024.5.26/getmeta/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:09.502251 getmeta-2024.5.26/getmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-27 13:18:09.000000 getmeta-2024.5.26/getmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-27 13:18:09.000000 getmeta-2024.5.26/getmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:18:09.000000 getmeta-2024.5.26/getmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 13:18:09.000000 getmeta-2024.5.26/getmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:18:09.000000 getmeta-2024.5.26/getmeta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 13:18:09.000000 getmeta-2024.5.26/getmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 13:18:09.000000 getmeta-2024.5.26/getmeta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:18:09.502251 getmeta-2024.5.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-27 13:18:03.000000 getmeta-2024.5.26/setup.py
```

### Comparing `getmeta-2024.5.25/LICENSE` & `getmeta-2024.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `getmeta-2024.5.25/PKG-INFO` & `getmeta-2024.5.26/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getmeta
-Version: 2024.5.25
+Version: 2024.5.26
 Summary: Not just gold builds anymore!
 Home-page: https://github.com/4n6ir/getmeta
 Author: John Lukach
 Author-email: hello@4n6ir.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -64,26 +64,30 @@
 10. md5dir
 11. sha256dir
 12. sha3dir
 13. md5name
 14. sha256name
 15. sha3name
 16. type
-17. entropy
-18. block
-19. location
 
 ### INSTALLATION
 
 ```
 pip install getmeta
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
 ```
 
+### EXECUTABLE
+
+```
+pip install pyinstaller
+pyinstaller getmeta.py --onefile
+```
+
 ### META INFORMATION
 
 ![Meta Information](images/metainfo.png)
```

### Comparing `getmeta-2024.5.25/README.md` & `getmeta-2024.5.26/getmeta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: getmeta
+Version: 2024.5.26
+Summary: Not just gold builds anymore!
+Home-page: https://github.com/4n6ir/getmeta
+Author: John Lukach
+Author-email: hello@4n6ir.com
+License: Apache-2.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
 # getmeta
 
 ### NORMALIZATION
 
 Clean data is mission-critical for collecting operating system artifacts, especially with user home directories.
 
 ### APPLE, LINUX, & UNIX
@@ -51,26 +64,30 @@
 10. md5dir
 11. sha256dir
 12. sha3dir
 13. md5name
 14. sha256name
 15. sha3name
 16. type
-17. entropy
-18. block
-19. location
 
 ### INSTALLATION
 
 ```
 pip install getmeta
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
 ```
 
+### EXECUTABLE
+
+```
+pip install pyinstaller
+pyinstaller getmeta.py --onefile
+```
+
 ### META INFORMATION
 
-![Meta Information](images/metainfo.png)
+![Meta Information](images/metainfo.png)
```

### Comparing `getmeta-2024.5.25/getmeta.egg-info/PKG-INFO` & `getmeta-2024.5.26/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: getmeta
-Version: 2024.5.25
-Summary: Not just gold builds anymore!
-Home-page: https://github.com/4n6ir/getmeta
-Author: John Lukach
-Author-email: hello@4n6ir.com
-License: Apache-2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
 # getmeta
 
 ### NORMALIZATION
 
 Clean data is mission-critical for collecting operating system artifacts, especially with user home directories.
 
 ### APPLE, LINUX, & UNIX
@@ -64,26 +51,30 @@
 10. md5dir
 11. sha256dir
 12. sha3dir
 13. md5name
 14. sha256name
 15. sha3name
 16. type
-17. entropy
-18. block
-19. location
 
 ### INSTALLATION
 
 ```
 pip install getmeta
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
 ```
 
+### EXECUTABLE
+
+```
+pip install pyinstaller
+pyinstaller getmeta.py --onefile
+```
+
 ### META INFORMATION
 
-![Meta Information](images/metainfo.png)
+![Meta Information](images/metainfo.png)
```

### Comparing `getmeta-2024.5.25/setup.py` & `getmeta-2024.5.26/setup.py`

 * *Files identical despite different names*

