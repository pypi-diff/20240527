# Comparing `tmp/dicio_py-1.5.tar.gz` & `tmp/dicio_py-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-1.5.tar", last modified: Mon May 27 12:26:02 2024, max compression
+gzip compressed data, was "dicio_py-1.6.tar", last modified: Mon May 27 13:13:51 2024, max compression
```

## Comparing `dicio_py-1.5.tar` & `dicio_py-1.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:26:02.297423 dicio_py-1.5/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.5/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 12:26:02.297423 dicio_py-1.5/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.5/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:26:02.289424 dicio_py-1.5/dicio_my/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.5/dicio_my/__init__.py
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3317 2024-05-27 12:24:23.000000 dicio_py-1.5/dicio_my/__main__.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 12:26:02.297423 dicio_py-1.5/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      231 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       52 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/entry_points.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        9 2024-05-27 12:26:02.000000 dicio_py-1.5/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 12:26:02.297423 dicio_py-1.5/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      760 2024-05-27 12:23:42.000000 dicio_py-1.5/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:13:51.112713 dicio_py-1.6/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.6/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:13:51.112713 dicio_py-1.6/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.6/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:13:51.108713 dicio_py-1.6/dicio_my/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.6/dicio_my/__init__.py
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3940 2024-05-27 13:12:54.000000 dicio_py-1.6/dicio_my/__main__.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 13:13:51.112713 dicio_py-1.6/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 13:13:51.000000 dicio_py-1.6/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      196 2024-05-27 13:13:51.000000 dicio_py-1.6/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 13:13:51.000000 dicio_py-1.6/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        9 2024-05-27 13:13:51.000000 dicio_py-1.6/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 13:13:51.112713 dicio_py-1.6/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      647 2024-05-27 13:13:22.000000 dicio_py-1.6/setup.py
```

### Comparing `dicio_py-1.5/LICENSE` & `dicio_py-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-1.5/PKG-INFO` & `dicio_py-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.5
+Version: 1.6
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-1.5/README.md` & `dicio_py-1.6/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-1.5/dicio_py.egg-info/PKG-INFO` & `dicio_py-1.6/dicio_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.5
+Version: 1.6
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-1.5/setup.py` & `dicio_py-1.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dicio-py",
-    version="1.5",
+    version="1.6",
     author="Jetrom17",
     author_email="Jeiel@duck.com",
     description="Dicionário via CLI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Jetrom17/dicio-py",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
-    entry_points={
-        'console_scripts': [
-            'dicio-py=dicio_py.__main__:main',
-        ],
-    },
     python_requires='>=3.0',
 )
```

