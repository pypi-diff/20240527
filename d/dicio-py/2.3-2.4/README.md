# Comparing `tmp/dicio_py-2.3.tar.gz` & `tmp/dicio_py-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-2.3.tar", last modified: Mon May 27 14:56:45 2024, max compression
+gzip compressed data, was "dicio_py-2.4.tar", last modified: Mon May 27 15:07:00 2024, max compression
```

## Comparing `dicio_py-2.3.tar` & `dicio_py-2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:56:45.654386 dicio_py-2.3/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-2.3/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:56:45.650386 dicio_py-2.3/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-2.3/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:56:45.630386 dicio_py-2.3/dicio/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:18:42.000000 dicio_py-2.3/dicio/__init__.py
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3922 2024-05-27 14:56:06.000000 dicio_py-2.3/dicio/dicio.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:56:45.650386 dicio_py-2.3/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:56:45.000000 dicio_py-2.3/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      222 2024-05-27 14:56:45.000000 dicio_py-2.3/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:56:45.000000 dicio_py-2.3/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       40 2024-05-27 14:56:45.000000 dicio_py-2.3/dicio_py.egg-info/entry_points.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        6 2024-05-27 14:56:45.000000 dicio_py-2.3/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 14:56:45.654386 dicio_py-2.3/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      699 2024-05-27 14:56:25.000000 dicio_py-2.3/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 15:07:00.879776 dicio_py-2.4/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-2.4/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 15:07:00.879776 dicio_py-2.4/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-2.4/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 15:07:00.871776 dicio_py-2.4/dicio/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:18:42.000000 dicio_py-2.4/dicio/__init__.py
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3945 2024-05-27 15:06:26.000000 dicio_py-2.4/dicio/dicio.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 15:07:00.879776 dicio_py-2.4/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 15:07:00.000000 dicio_py-2.4/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      222 2024-05-27 15:07:00.000000 dicio_py-2.4/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 15:07:00.000000 dicio_py-2.4/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       40 2024-05-27 15:07:00.000000 dicio_py-2.4/dicio_py.egg-info/entry_points.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        6 2024-05-27 15:07:00.000000 dicio_py-2.4/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 15:07:00.879776 dicio_py-2.4/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      699 2024-05-27 15:03:59.000000 dicio_py-2.4/setup.py
```

### Comparing `dicio_py-2.3/LICENSE` & `dicio_py-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-2.3/PKG-INFO` & `dicio_py-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 2.3
+Version: 2.4
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-2.3/README.md` & `dicio_py-2.4/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-2.3/dicio/dicio.py` & `dicio_py-2.4/dicio/dicio.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Uso:
 python3 ./dicio-py.py [PALAVRA]
 
 Dependências:
 - Nenhuma dependência externa necessária. O script utiliza apenas bibliotecas padrão do Python 3.
 """
 
+from dicio import main
 import sys
 import re
 import os
 from unicodedata import normalize
 from urllib.request import urlopen
 
 BASE_URL = 'https://www.dicio.com.br/'
```

### Comparing `dicio_py-2.3/dicio_py.egg-info/PKG-INFO` & `dicio_py-2.4/dicio_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 2.3
+Version: 2.4
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-2.3/setup.py` & `dicio_py-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="dicio-py",
-  version="2.3",
+  version="2.4",
   author="Jetrom17",
   author_email="Jeiel@duck.com",
   description="Dicionário via CLI",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Jetrom17/dicio-py",
   packages=setuptools.find_packages(),
```

