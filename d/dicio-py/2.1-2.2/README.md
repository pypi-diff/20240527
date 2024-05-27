# Comparing `tmp/dicio_py-2.1.tar.gz` & `tmp/dicio_py-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-2.1.tar", last modified: Mon May 27 14:26:34 2024, max compression
+gzip compressed data, was "dicio_py-2.2.tar", last modified: Mon May 27 14:43:35 2024, max compression
```

## Comparing `dicio_py-2.1.tar` & `dicio_py-2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:26:34.178108 dicio_py-2.1/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-2.1/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:26:34.178108 dicio_py-2.1/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-2.1/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:26:34.170108 dicio_py-2.1/dicio/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:18:42.000000 dicio_py-2.1/dicio/__init__.py
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3877 2024-05-27 13:57:27.000000 dicio_py-2.1/dicio/dicio.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:26:34.174108 dicio_py-2.1/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      222 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       49 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/entry_points.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        6 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 14:26:34.178108 dicio_py-2.1/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      708 2024-05-27 14:25:33.000000 dicio_py-2.1/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:43:35.098857 dicio_py-2.2/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-2.2/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:43:35.098857 dicio_py-2.2/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-2.2/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:43:35.094857 dicio_py-2.2/dicio/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:18:42.000000 dicio_py-2.2/dicio/__init__.py
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3901 2024-05-27 14:40:34.000000 dicio_py-2.2/dicio/dicio.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:43:35.098857 dicio_py-2.2/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:43:35.000000 dicio_py-2.2/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      222 2024-05-27 14:43:35.000000 dicio_py-2.2/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:43:35.000000 dicio_py-2.2/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       40 2024-05-27 14:43:35.000000 dicio_py-2.2/dicio_py.egg-info/entry_points.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        6 2024-05-27 14:43:35.000000 dicio_py-2.2/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 14:43:35.098857 dicio_py-2.2/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      699 2024-05-27 14:43:06.000000 dicio_py-2.2/setup.py
```

### Comparing `dicio_py-2.1/LICENSE` & `dicio_py-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-2.1/PKG-INFO` & `dicio_py-2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 2.1
+Version: 2.2
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-2.1/README.md` & `dicio_py-2.2/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-2.1/dicio/dicio.py` & `dicio_py-2.2/dicio/dicio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 """
 Dicio-Py: Script para buscar o significado de palavras no dicionário online Dicio.
 Versão: 1.0
 Autor: Jeiel Lima Miranda.
 Data: 26 de maio de 2024
 Fork: https://github.com/ludovici-philippus/dicio-py
```

### Comparing `dicio_py-2.1/dicio_py.egg-info/PKG-INFO` & `dicio_py-2.2/dicio_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 2.1
+Version: 2.2
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-2.1/setup.py` & `dicio_py-2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="dicio-py",
-  version="2.1",
+  version="2.2",
   author="Jetrom17",
   author_email="Jeiel@duck.com",
   description="Dicionário via CLI",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Jetrom17/dicio-py",
   packages=setuptools.find_packages(),
@@ -17,11 +17,11 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
   ],
   python_requires='>=3.0',
   entry_points={
       'console_scripts': [
-          'dicio-py = dicio.dicio_py:main'
+          'dicio.py = dicio:main'
       ]
   }
 )
```

