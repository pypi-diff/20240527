# Comparing `tmp/xdbutils-0.0.1.post1.tar.gz` & `tmp/xdbutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdbutils-0.0.1.post1.tar", last modified: Mon May 27 07:24:40 2024, max compression
+gzip compressed data, was "xdbutils-0.0.2.tar", last modified: Mon May 27 07:25:37 2024, max compression
```

## Comparing `xdbutils-0.0.1.post1.tar` & `xdbutils-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:24:40.240969 xdbutils-0.0.1.post1/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1235 2023-08-30 13:36:11.000000 xdbutils-0.0.1.post1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32832 2024-05-27 07:24:40.236105 xdbutils-0.0.1.post1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32936 2024-05-01 12:43:29.000000 xdbutils-0.0.1.post1/README.md
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      651 2024-05-27 07:24:40.246967 xdbutils-0.0.1.post1/setup.cfg
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)       77 2023-08-30 13:36:11.000000 xdbutils-0.0.1.post1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:24:39.276761 xdbutils-0.0.1.post1/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:24:39.555917 xdbutils-0.0.1.post1/src/test/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-08-30 13:36:11.000000 xdbutils-0.0.1.post1/src/test/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1783 2024-05-01 12:07:25.000000 xdbutils-0.0.1.post1/src/test/test_pipelines_data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1709 2024-05-01 11:40:09.000000 xdbutils-0.0.1.post1/src/test/test_pipelines_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2248 2024-05-01 12:10:45.000000 xdbutils-0.0.1.post1/src/test/test_pipelines_source.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2442 2023-08-30 13:39:15.000000 xdbutils-0.0.1.post1/src/test/test_transforms_scd2.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:24:39.695309 xdbutils-0.0.1.post1/src/xdbutils/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6990 2024-05-01 12:42:50.000000 xdbutils-0.0.1.post1/src/xdbutils/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17183 2023-08-30 13:39:35.000000 xdbutils-0.0.1.post1/src/xdbutils/datalakehouse.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      679 2023-10-06 09:10:44.000000 xdbutils-0.0.1.post1/src/xdbutils/deprecation.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:24:40.099140 xdbutils-0.0.1.post1/src/xdbutils/pipelines/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-04-10 13:12:39.000000 xdbutils-0.0.1.post1/src/xdbutils/pipelines/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8549 2024-05-01 13:11:36.000000 xdbutils-0.0.1.post1/src/xdbutils/pipelines/data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      697 2024-04-24 09:00:35.000000 xdbutils-0.0.1.post1/src/xdbutils/pipelines/deprecation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11125 2024-05-01 11:50:23.000000 xdbutils-0.0.1.post1/src/xdbutils/pipelines/management.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17814 2024-05-27 07:10:52.000000 xdbutils-0.0.1.post1/src/xdbutils/pipelines/source.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    28199 2024-04-10 14:41:08.000000 xdbutils-0.0.1.post1/src/xdbutils/pipelines_pre_14_3_lts.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:24:40.172526 xdbutils-0.0.1.post1/src/xdbutils/transforms/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-08-30 13:36:11.000000 xdbutils-0.0.1.post1/src/xdbutils/transforms/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3979 2023-08-30 13:39:15.000000 xdbutils-0.0.1.post1/src/xdbutils/transforms/scd2.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:24:40.213674 xdbutils-0.0.1.post1/src/xdbutils.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32832 2024-05-27 07:24:38.000000 xdbutils-0.0.1.post1/src/xdbutils.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      734 2024-05-27 07:24:39.000000 xdbutils-0.0.1.post1/src/xdbutils.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-27 07:24:38.000000 xdbutils-0.0.1.post1/src/xdbutils.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2024-05-27 07:24:38.000000 xdbutils-0.0.1.post1/src/xdbutils.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2024-05-27 07:24:38.000000 xdbutils-0.0.1.post1/src/xdbutils.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:25:37.301624 xdbutils-0.0.2/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1235 2023-08-30 13:36:11.000000 xdbutils-0.0.2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32826 2024-05-27 07:25:37.295116 xdbutils-0.0.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32936 2024-05-01 12:43:29.000000 xdbutils-0.0.2/README.md
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      649 2024-05-27 07:25:37.313630 xdbutils-0.0.2/setup.cfg
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)       77 2023-08-30 13:36:11.000000 xdbutils-0.0.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:25:36.217558 xdbutils-0.0.2/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:25:36.542759 xdbutils-0.0.2/src/test/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-08-30 13:36:11.000000 xdbutils-0.0.2/src/test/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1783 2024-05-01 12:07:25.000000 xdbutils-0.0.2/src/test/test_pipelines_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1709 2024-05-01 11:40:09.000000 xdbutils-0.0.2/src/test/test_pipelines_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2248 2024-05-01 12:10:45.000000 xdbutils-0.0.2/src/test/test_pipelines_source.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2442 2023-08-30 13:39:15.000000 xdbutils-0.0.2/src/test/test_transforms_scd2.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:25:36.675509 xdbutils-0.0.2/src/xdbutils/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6990 2024-05-01 12:42:50.000000 xdbutils-0.0.2/src/xdbutils/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17183 2023-08-30 13:39:35.000000 xdbutils-0.0.2/src/xdbutils/datalakehouse.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      679 2023-10-06 09:10:44.000000 xdbutils-0.0.2/src/xdbutils/deprecation.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:25:37.149205 xdbutils-0.0.2/src/xdbutils/pipelines/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-04-10 13:12:39.000000 xdbutils-0.0.2/src/xdbutils/pipelines/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8549 2024-05-01 13:11:36.000000 xdbutils-0.0.2/src/xdbutils/pipelines/data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      697 2024-04-24 09:00:35.000000 xdbutils-0.0.2/src/xdbutils/pipelines/deprecation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11125 2024-05-01 11:50:23.000000 xdbutils-0.0.2/src/xdbutils/pipelines/management.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17814 2024-05-27 07:10:52.000000 xdbutils-0.0.2/src/xdbutils/pipelines/source.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    28199 2024-04-10 14:41:08.000000 xdbutils-0.0.2/src/xdbutils/pipelines_pre_14_3_lts.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:25:37.228290 xdbutils-0.0.2/src/xdbutils/transforms/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2023-08-30 13:36:11.000000 xdbutils-0.0.2/src/xdbutils/transforms/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3979 2023-08-30 13:39:15.000000 xdbutils-0.0.2/src/xdbutils/transforms/scd2.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-27 07:25:37.282798 xdbutils-0.0.2/src/xdbutils.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32826 2024-05-27 07:25:35.000000 xdbutils-0.0.2/src/xdbutils.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      734 2024-05-27 07:25:36.000000 xdbutils-0.0.2/src/xdbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-27 07:25:35.000000 xdbutils-0.0.2/src/xdbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2024-05-27 07:25:35.000000 xdbutils-0.0.2/src/xdbutils.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2024-05-27 07:25:35.000000 xdbutils-0.0.2/src/xdbutils.egg-info/top_level.txt
```

### Comparing `xdbutils-0.0.1.post1/LICENSE` & `xdbutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/PKG-INFO` & `xdbutils-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdbutils
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: Utilities for Databricks
 Home-page: https://github.com/henrikbulldog/xdbutils
 Author: Henrik Thomsen
 Author-email: henrik.thomsen.dk@gmail.dk
 Project-URL: Bug Tracker, https://github.com/henrikbulldog/xdbutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `xdbutils-0.0.1.post1/README.md` & `xdbutils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/setup.cfg` & `xdbutils-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xdbutils
-version = 0.0.1-1
+version = 0.0.2
 author = Henrik Thomsen
 author_email = henrik.thomsen.dk@gmail.dk
 description = Utilities for Databricks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/henrikbulldog/xdbutils
 project_urls =
```

### Comparing `xdbutils-0.0.1.post1/src/test/test_pipelines_data.py` & `xdbutils-0.0.2/src/test/test_pipelines_data.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/test/test_pipelines_manager.py` & `xdbutils-0.0.2/src/test/test_pipelines_manager.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/test/test_pipelines_source.py` & `xdbutils-0.0.2/src/test/test_pipelines_source.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/test/test_transforms_scd2.py` & `xdbutils-0.0.2/src/test/test_transforms_scd2.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/__init__.py` & `xdbutils-0.0.2/src/xdbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/datalakehouse.py` & `xdbutils-0.0.2/src/xdbutils/datalakehouse.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/deprecation.py` & `xdbutils-0.0.2/src/xdbutils/deprecation.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/pipelines/data.py` & `xdbutils-0.0.2/src/xdbutils/pipelines/data.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/pipelines/deprecation.py` & `xdbutils-0.0.2/src/xdbutils/pipelines/deprecation.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/pipelines/management.py` & `xdbutils-0.0.2/src/xdbutils/pipelines/management.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/pipelines/source.py` & `xdbutils-0.0.2/src/xdbutils/pipelines/source.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/pipelines_pre_14_3_lts.py` & `xdbutils-0.0.2/src/xdbutils/pipelines_pre_14_3_lts.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils/transforms/scd2.py` & `xdbutils-0.0.2/src/xdbutils/transforms/scd2.py`

 * *Files identical despite different names*

### Comparing `xdbutils-0.0.1.post1/src/xdbutils.egg-info/PKG-INFO` & `xdbutils-0.0.2/src/xdbutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdbutils
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: Utilities for Databricks
 Home-page: https://github.com/henrikbulldog/xdbutils
 Author: Henrik Thomsen
 Author-email: henrik.thomsen.dk@gmail.dk
 Project-URL: Bug Tracker, https://github.com/henrikbulldog/xdbutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `xdbutils-0.0.1.post1/src/xdbutils.egg-info/SOURCES.txt` & `xdbutils-0.0.2/src/xdbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

