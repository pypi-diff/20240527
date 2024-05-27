# Comparing `tmp/pygrl-0.0.1.tar.gz` & `tmp/pygrl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrl-0.0.1.tar", last modified: Mon May 27 10:36:30 2024, max compression
+gzip compressed data, was "pygrl-0.0.2.tar", last modified: Mon May 27 10:38:14 2024, max compression
```

## Comparing `pygrl-0.0.1.tar` & `pygrl-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:36:30.780146 pygrl-0.0.1/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-27 07:20:34.000000 pygrl-0.0.1/LICENSE
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2550 2024-05-27 10:36:30.780146 pygrl-0.0.1/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1989 2024-05-27 10:35:53.000000 pygrl-0.0.1/README.md
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:36:30.776146 pygrl-0.0.1/pygrl/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     1497 2024-05-27 10:34:31.000000 pygrl-0.0.1/pygrl/__init__.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      133 2024-05-27 09:32:59.000000 pygrl-0.0.1/pygrl/custom_exception.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)    11703 2024-05-27 10:17:36.000000 pygrl-0.0.1/pygrl/main.py
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2139 2024-05-27 10:13:10.000000 pygrl-0.0.1/pygrl/storage.py
-drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:36:30.780146 pygrl-0.0.1/pygrl.egg-info/
--rw-rw-r--   0 jonah     (1000) jonah     (1000)     2550 2024-05-27 10:36:30.000000 pygrl-0.0.1/pygrl.egg-info/PKG-INFO
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      217 2024-05-27 10:36:30.000000 pygrl-0.0.1/pygrl.egg-info/SOURCES.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-27 10:36:30.000000 pygrl-0.0.1/pygrl.egg-info/dependency_links.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)        6 2024-05-27 10:36:30.000000 pygrl-0.0.1/pygrl.egg-info/top_level.txt
--rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-27 10:36:30.780146 pygrl-0.0.1/setup.cfg
--rw-rw-r--   0 jonah     (1000) jonah     (1000)      860 2024-05-27 10:34:12.000000 pygrl-0.0.1/setup.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:38:14.924838 pygrl-0.0.2/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1067 2024-05-27 07:20:34.000000 pygrl-0.0.2/LICENSE
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2559 2024-05-27 10:38:14.924838 pygrl-0.0.2/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1989 2024-05-27 10:35:53.000000 pygrl-0.0.2/README.md
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:38:14.924838 pygrl-0.0.2/pygrl/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     1497 2024-05-27 10:34:31.000000 pygrl-0.0.2/pygrl/__init__.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      133 2024-05-27 09:32:59.000000 pygrl-0.0.2/pygrl/custom_exception.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)    11703 2024-05-27 10:17:36.000000 pygrl-0.0.2/pygrl/main.py
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2139 2024-05-27 10:13:10.000000 pygrl-0.0.2/pygrl/storage.py
+drwxrwxr-x   0 jonah     (1000) jonah     (1000)        0 2024-05-27 10:38:14.924838 pygrl-0.0.2/pygrl.egg-info/
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)     2559 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/PKG-INFO
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      217 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        1 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)        6 2024-05-27 10:38:14.000000 pygrl-0.0.2/pygrl.egg-info/top_level.txt
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)       38 2024-05-27 10:38:14.924838 pygrl-0.0.2/setup.cfg
+-rw-rw-r--   0 jonah     (1000) jonah     (1000)      869 2024-05-27 10:38:10.000000 pygrl-0.0.2/setup.py
```

### Comparing `pygrl-0.0.1/LICENSE` & `pygrl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrl-0.0.1/PKG-INFO` & `pygrl-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygrl
-Version: 0.0.1
-Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
+Version: 0.0.2
+Summary: Another Python package aim to offer "Rate Limiting" functionality for general use cases.
 Home-page: UNKNOWN
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,rate,limiter,rate limiter,rate limiting
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pygrl-0.0.1/README.md` & `pygrl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pygrl-0.0.1/pygrl/__init__.py` & `pygrl-0.0.2/pygrl/__init__.py`

 * *Files identical despite different names*

### Comparing `pygrl-0.0.1/pygrl/main.py` & `pygrl-0.0.2/pygrl/main.py`

 * *Files identical despite different names*

### Comparing `pygrl-0.0.1/pygrl/storage.py` & `pygrl-0.0.2/pygrl/storage.py`

 * *Files identical despite different names*

### Comparing `pygrl-0.0.1/pygrl.egg-info/PKG-INFO` & `pygrl-0.0.2/pygrl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygrl
-Version: 0.0.1
-Summary: Package that wraps the python-telegram-bot library to make broadcasting easier.
+Version: 0.0.2
+Summary: Another Python package aim to offer "Rate Limiting" functionality for general use cases.
 Home-page: UNKNOWN
 Author: jonah_whaler_2348
 Author-email: jk_saga@proton.me
 License: MIT
 Keywords: python,rate,limiter,rate limiter,rate limiting
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

