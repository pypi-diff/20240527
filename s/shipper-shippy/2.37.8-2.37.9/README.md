# Comparing `tmp/shipper_shippy-2.37.8.tar.gz` & `tmp/shipper_shippy-2.37.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper_shippy-2.37.8.tar", last modified: Thu May 23 23:44:20 2024, max compression
+gzip compressed data, was "shipper_shippy-2.37.9.tar", last modified: Mon May 27 06:02:17 2024, max compression
```

## Comparing `shipper_shippy-2.37.8.tar` & `shipper_shippy-2.37.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:44:20.819246 shipper_shippy-2.37.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-23 23:44:20.819246 shipper_shippy-2.37.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 23:44:20.819246 shipper_shippy-2.37.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:44:20.819246 shipper_shippy-2.37.8/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-23 23:44:20.000000 shipper_shippy-2.37.8/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 23:44:20.000000 shipper_shippy-2.37.8/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:44:20.000000 shipper_shippy-2.37.8/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 23:44:20.000000 shipper_shippy-2.37.8/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 23:44:20.000000 shipper_shippy-2.37.8/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 23:44:20.000000 shipper_shippy-2.37.8/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:44:20.819246 shipper_shippy-2.37.8/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 23:44:12.000000 shipper_shippy-2.37.8/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:02:17.279873 shipper_shippy-2.37.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-27 06:02:17.279873 shipper_shippy-2.37.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:02:17.279873 shipper_shippy-2.37.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:02:17.279873 shipper_shippy-2.37.9/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-27 06:02:17.000000 shipper_shippy-2.37.9/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-27 06:02:17.000000 shipper_shippy-2.37.9/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:02:17.000000 shipper_shippy-2.37.9/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 06:02:17.000000 shipper_shippy-2.37.9/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 06:02:17.000000 shipper_shippy-2.37.9/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 06:02:17.000000 shipper_shippy-2.37.9/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:02:17.279873 shipper_shippy-2.37.9/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 06:02:09.000000 shipper_shippy-2.37.9/shippy/version.py
```

### Comparing `shipper_shippy-2.37.8/PKG-INFO` & `shipper_shippy-2.37.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.37.8
+Version: 2.37.9
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.32.2
 Requires-Dist: rich==13.7.1
 Requires-Dist: semver==3.0.2
-Requires-Dist: sentry-sdk==2.2.1
+Requires-Dist: sentry-sdk==2.3.1
 Requires-Dist: setuptools==70.0.0
 
 # shippy
 
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
```

### Comparing `shipper_shippy-2.37.8/README.md` & `shipper_shippy-2.37.9/README.md`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.8/setup.py` & `shipper_shippy-2.37.9/setup.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.8/shipper_shippy.egg-info/PKG-INFO` & `shipper_shippy-2.37.9/shipper_shippy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.37.8
+Version: 2.37.9
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.32.2
 Requires-Dist: rich==13.7.1
 Requires-Dist: semver==3.0.2
-Requires-Dist: sentry-sdk==2.2.1
+Requires-Dist: sentry-sdk==2.3.1
 Requires-Dist: setuptools==70.0.0
 
 # shippy
 
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
```

### Comparing `shipper_shippy-2.37.8/shippy/__main__.py` & `shipper_shippy-2.37.9/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.8/shippy/client.py` & `shipper_shippy-2.37.9/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.8/shippy/config.py` & `shipper_shippy-2.37.9/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.8/shippy/constants.py` & `shipper_shippy-2.37.9/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.37.8/shippy/helper.py` & `shipper_shippy-2.37.9/shippy/helper.py`

 * *Files identical despite different names*

