# Comparing `tmp/sophisticate-1.0.2.tar.gz` & `tmp/sophisticate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sophisticate-1.0.2.tar", last modified: Thu May 23 16:45:56 2024, max compression
+gzip compressed data, was "sophisticate-1.0.3.tar", last modified: Mon May 27 19:12:39 2024, max compression
```

## Comparing `sophisticate-1.0.2.tar` & `sophisticate-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:45:56.651929 sophisticate-1.0.2/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     1141 2024-05-23 16:45:56.651929 sophisticate-1.0.2/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      715 2024-05-21 23:24:20.000000 sophisticate-1.0.2/README.md
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-23 16:45:56.651929 sophisticate-1.0.2/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      741 2024-05-23 16:42:52.000000 sophisticate-1.0.2/setup.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:45:56.651929 sophisticate-1.0.2/sophisticate/
--rw-r--r--   0 khiat     (1000) khiat     (1000)       60 2024-05-21 22:25:02.000000 sophisticate-1.0.2/sophisticate/__init__.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-23 16:45:56.651929 sophisticate-1.0.2/sophisticate.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)     1141 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      222 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       60 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       13 2024-05-23 16:45:56.000000 sophisticate-1.0.2/sophisticate.egg-info/top_level.txt
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-27 19:12:39.752244 sophisticate-1.0.3/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     1190 2024-05-27 19:12:39.752244 sophisticate-1.0.3/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      764 2024-05-27 19:10:43.000000 sophisticate-1.0.3/README.md
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-27 19:12:39.752244 sophisticate-1.0.3/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      767 2024-05-27 19:08:48.000000 sophisticate-1.0.3/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-27 19:12:39.752244 sophisticate-1.0.3/sophisticate/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     1293 2024-05-27 19:12:01.000000 sophisticate-1.0.3/sophisticate/__init__.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-27 19:12:39.752244 sophisticate-1.0.3/sophisticate.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)     1190 2024-05-27 19:12:39.000000 sophisticate-1.0.3/sophisticate.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      222 2024-05-27 19:12:39.000000 sophisticate-1.0.3/sophisticate.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-27 19:12:39.000000 sophisticate-1.0.3/sophisticate.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       75 2024-05-27 19:12:39.000000 sophisticate-1.0.3/sophisticate.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       13 2024-05-27 19:12:39.000000 sophisticate-1.0.3/sophisticate.egg-info/top_level.txt
```

### Comparing `sophisticate-1.0.2/PKG-INFO` & `sophisticate-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophisticate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sophisticate Libraries Collection
 Home-page: https://pypi.org/project/sophisticate/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,15 @@
 ## This library will install the following libraries 
 
 
 ### conf-mat : https://pypi.org/project/conf-mat/
 ### linkedit : https://pypi.org/project/linkedit/
 ### cqueue   : https://pypi.org/project/cqueue/
 ### lstack   : https://pypi.org/project/lstack/
+### hashall  : https://pypi.org/project/hashall/
 
 
 ## Installation
 
 
 You can install `sophisticate` via pip:
```

### Comparing `sophisticate-1.0.2/README.md` & `sophisticate-1.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ## This library will install the following libraries 
 
 
 ### conf-mat : https://pypi.org/project/conf-mat/
 ### linkedit : https://pypi.org/project/linkedit/
 ### cqueue   : https://pypi.org/project/cqueue/
 ### lstack   : https://pypi.org/project/lstack/
+### hashall  : https://pypi.org/project/hashall/
 
 
 ## Installation
 
 
 You can install `sophisticate` via pip:
```

### Comparing `sophisticate-1.0.2/setup.py` & `sophisticate-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sophisticate",
-    version="1.0.2",
+    version="1.0.3",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Libraries Collection",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/sophisticate/",
     packages=find_packages(),
     install_requires=[
         "conf-mat>=1.0.7",
-        "linkedit>=1.0.5",
-        "cqueue>=1.0.1",
-        "lstack>=1.0.3",
+        "linkedit>=1.0.8",
+        "cqueue>=1.0.3",
+        "lstack>=1.0.4",
+        "hashall>=1.0.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

### Comparing `sophisticate-1.0.2/sophisticate.egg-info/PKG-INFO` & `sophisticate-1.0.3/sophisticate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophisticate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sophisticate Libraries Collection
 Home-page: https://pypi.org/project/sophisticate/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,15 @@
 ## This library will install the following libraries 
 
 
 ### conf-mat : https://pypi.org/project/conf-mat/
 ### linkedit : https://pypi.org/project/linkedit/
 ### cqueue   : https://pypi.org/project/cqueue/
 ### lstack   : https://pypi.org/project/lstack/
+### hashall  : https://pypi.org/project/hashall/
 
 
 ## Installation
 
 
 You can install `sophisticate` via pip:
```

