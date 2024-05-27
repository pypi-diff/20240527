# Comparing `tmp/dicio_py-1.9.tar.gz` & `tmp/dicio_py-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-1.9.tar", last modified: Mon May 27 13:57:56 2024, max compression
+gzip compressed data, was "dicio_py-2.0.tar", last modified: Mon May 27 14:10:05 2024, max compression
```

## Comparing `dicio_py-1.9.tar` & `dicio_py-2.0.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:57:56.539017 dicio_py-1.9/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.9/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:57:56.539017 dicio_py-1.9/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.9/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:57:56.531017 dicio_py-1.9/dicio_my/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.9/dicio_my/__init__.py
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3877 2024-05-27 13:57:27.000000 dicio_py-1.9/dicio_my/dicio.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:57:56.539017 dicio_py-1.9/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:57:56.000000 dicio_py-1.9/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      193 2024-05-27 13:57:56.000000 dicio_py-1.9/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 13:57:56.000000 dicio_py-1.9/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        9 2024-05-27 13:57:56.000000 dicio_py-1.9/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 13:57:56.539017 dicio_py-1.9/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      647 2024-05-27 13:56:36.000000 dicio_py-1.9/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:10:05.150871 dicio_py-2.0/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-2.0/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:10:05.146871 dicio_py-2.0/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-2.0/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:10:05.146871 dicio_py-2.0/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      154 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 14:10:05.150871 dicio_py-2.0/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      647 2024-05-27 14:09:53.000000 dicio_py-2.0/setup.py
```

### Comparing `dicio_py-1.9/LICENSE` & `dicio_py-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-1.9/PKG-INFO` & `dicio_py-2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.9
+Version: 2.0
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-1.9/README.md` & `dicio_py-2.0/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-1.9/dicio_py.egg-info/PKG-INFO` & `dicio_py-2.0/dicio_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.9
+Version: 2.0
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-1.9/setup.py` & `dicio_py-2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dicio-py",
-    version="1.9",
+    version="2.0",
     author="Jetrom17",
     author_email="Jeiel@duck.com",
     description="Dicionário via CLI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Jetrom17/dicio-py",
     packages=setuptools.find_packages(),
```

