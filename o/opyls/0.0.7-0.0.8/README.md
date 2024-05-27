# Comparing `tmp/opyls-0.0.7.tar.gz` & `tmp/opyls-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opyls-0.0.7.tar", last modified: Mon Apr 29 06:49:59 2024, max compression
+gzip compressed data, was "opyls-0.0.8.tar", last modified: Mon May 27 01:02:32 2024, max compression
```

## Comparing `opyls-0.0.7.tar` & `opyls-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:49:59.150560 opyls-0.0.7/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.7/LICENSE
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:49:59.150327 opyls-0.0.7/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.7/README.md
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:49:59.149630 opyls-0.0.7/opyls/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      128 2024-04-29 06:47:35.000000 opyls-0.0.7/opyls/__init__.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      628 2024-04-29 06:49:17.000000 opyls-0.0.7/opyls/collections.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      879 2024-04-29 06:16:46.000000 opyls-0.0.7/opyls/json.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)     1320 2024-04-29 06:15:12.000000 opyls-0.0.7/opyls/load.py
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      644 2024-04-29 06:15:06.000000 opyls-0.0.7/opyls/paths.py
-drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-04-29 06:49:59.150091 opyls-0.0.7/opyls.egg-info/
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-04-29 06:49:59.000000 opyls-0.0.7/opyls.egg-info/PKG-INFO
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      224 2024-04-29 06:49:59.000000 opyls-0.0.7/opyls.egg-info/SOURCES.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-04-29 06:49:59.000000 opyls-0.0.7/opyls.egg-info/dependency_links.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-04-29 06:49:59.000000 opyls-0.0.7/opyls.egg-info/top_level.txt
--rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-04-29 06:49:59.150603 opyls-0.0.7/setup.cfg
--rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-04-29 06:49:56.000000 opyls-0.0.7/setup.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-05-27 01:02:32.620200 opyls-0.0.8/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)     1071 2024-04-29 04:55:51.000000 opyls-0.0.8/LICENSE
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-05-27 01:02:32.619963 opyls-0.0.8/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       30 2024-04-29 04:55:51.000000 opyls-0.0.8/README.md
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-05-27 01:02:32.618354 opyls-0.0.8/opyls/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      128 2024-04-29 06:47:35.000000 opyls-0.0.8/opyls/__init__.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      628 2024-04-29 06:49:17.000000 opyls-0.0.8/opyls/collections.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      155 2024-05-27 00:59:36.000000 opyls-0.0.8/opyls/dates.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      879 2024-04-29 06:16:46.000000 opyls-0.0.8/opyls/json.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)     1333 2024-04-29 07:04:07.000000 opyls-0.0.8/opyls/load.py
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      644 2024-04-29 06:15:06.000000 opyls-0.0.8/opyls/paths.py
+drwxr-xr-x   0 vladimirlevin   (501) staff       (20)        0 2024-05-27 01:02:32.619685 opyls-0.0.8/opyls.egg-info/
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      516 2024-05-27 01:02:32.000000 opyls-0.0.8/opyls.egg-info/PKG-INFO
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      239 2024-05-27 01:02:32.000000 opyls-0.0.8/opyls.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        1 2024-05-27 01:02:32.000000 opyls-0.0.8/opyls.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)        6 2024-05-27 01:02:32.000000 opyls-0.0.8/opyls.egg-info/top_level.txt
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)       38 2024-05-27 01:02:32.620244 opyls-0.0.8/setup.cfg
+-rw-r--r--   0 vladimirlevin   (501) staff       (20)      748 2024-05-27 01:01:47.000000 opyls-0.0.8/setup.py
```

### Comparing `opyls-0.0.7/LICENSE` & `opyls-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opyls-0.0.7/PKG-INFO` & `opyls-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.7
+Version: 0.0.8
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.7/opyls/collections.py` & `opyls-0.0.8/opyls/collections.py`

 * *Files identical despite different names*

### Comparing `opyls-0.0.7/opyls/json.py` & `opyls-0.0.8/opyls/json.py`

 * *Files identical despite different names*

### Comparing `opyls-0.0.7/opyls/load.py` & `opyls-0.0.8/opyls/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Union, Any
 
 import json
 
 
 # https://www.postgresqltutorial.com/postgresql-python/connect/
-def load_ini(filename: str, section: str) -> dict[str, str]:
+def load_ini(filename: Union[str, Path], section: str) -> dict[str, str]:
     """
     Load configuration from an INI file.
 
     Args:
         filename (str): The path to the INI file.
         section (str): The name of the section to load.
```

### Comparing `opyls-0.0.7/opyls/paths.py` & `opyls-0.0.8/opyls/paths.py`

 * *Files identical despite different names*

### Comparing `opyls-0.0.7/opyls.egg-info/PKG-INFO` & `opyls-0.0.8/opyls.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opyls
-Version: 0.0.7
+Version: 0.0.8
 Summary: opa_oz's python utils
 Author: Vladimir Levin
 Author-email: opaozhub@gmail.com
 Keywords: python,utils
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `opyls-0.0.7/setup.py` & `opyls-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = "opa_oz's python utils"
 LONG_DESCRIPTION = "Python package with stuff that I'm interested in"
 
 setup(
     name="opyls",
     version=VERSION,
     author="Vladimir Levin",
```

