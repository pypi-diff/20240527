# Comparing `tmp/opsramp-analytics-utils-3.5.4.tar.gz` & `tmp/opsramp-analytics-utils-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.5.4.tar", last modified: Fri May 10 07:39:55 2024, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.5.5.tar", last modified: Mon May 27 10:14:34 2024, max compression
```

## Comparing `opsramp-analytics-utils-3.5.4.tar` & `opsramp-analytics-utils-3.5.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.104915 opsramp-analytics-utils-3.5.4/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/LICENSE
--rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/MANIFEST.in
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-10 07:39:55.104766 opsramp-analytics-utils-3.5.4/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/README.md
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.086693 opsramp-analytics-utils-3.5.4/analytics_sdk/
--rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/__init__.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.090607 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/main.js
--rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.099238 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.101908 opsramp-analytics-utils-3.5.4/analytics_sdk/api/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/api/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17480 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/api/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/api/api_task.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/api/thread_process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17467 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/components.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/constants.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-05-08 11:52:29.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/oap_dash.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.102469 opsramp-analytics-utils-3.5.4/analytics_sdk/process/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/process/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/process/process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/process/querybuilder.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.103853 opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    35159 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/excel.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17745 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/excel_writer.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/pdf.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    45767 2024-05-10 07:37:13.000000 opsramp-analytics-utils-3.5.4/analytics_sdk/utilities.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-10 07:39:55.104550 opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-10 07:39:55.000000 opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1737 2024-05-10 07:39:55.000000 opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-05-10 07:39:55.000000 opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      148 2024-05-10 07:39:55.000000 opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/requires.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-05-10 07:39:55.000000 opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/top_level.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      162 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.4/requires-install.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-05-10 07:39:55.104972 opsramp-analytics-utils-3.5.4/setup.cfg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-05-10 07:38:26.000000 opsramp-analytics-utils-3.5.4/setup.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.737266 opsramp-analytics-utils-3.5.5/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/LICENSE
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/MANIFEST.in
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-27 10:14:34.737098 opsramp-analytics-utils-3.5.5/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/README.md
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.721233 opsramp-analytics-utils-3.5.5/analytics_sdk/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/__init__.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.724729 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/main.js
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.732782 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.733681 opsramp-analytics-utils-3.5.5/analytics_sdk/api/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/api/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17387 2024-05-27 10:13:13.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/api/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/api/api_task.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/api/thread_process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17374 2024-05-27 10:13:13.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/components.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/constants.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-05-08 11:52:29.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/oap_dash.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.734284 opsramp-analytics-utils-3.5.5/analytics_sdk/process/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/process/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/process/process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/process/querybuilder.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.735835 opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    35159 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/excel.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17460 2024-05-27 10:13:13.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/excel_writer.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/pdf.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    45767 2024-05-10 07:37:13.000000 opsramp-analytics-utils-3.5.5/analytics_sdk/utilities.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-05-27 10:14:34.736820 opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-05-27 10:14:34.000000 opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1737 2024-05-27 10:14:34.000000 opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-05-27 10:14:34.000000 opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      148 2024-05-27 10:14:34.000000 opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/requires.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-05-27 10:14:34.000000 opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      162 2024-05-08 08:32:16.000000 opsramp-analytics-utils-3.5.5/requires-install.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-05-27 10:14:34.737329 opsramp-analytics-utils-3.5.5/setup.cfg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-05-27 10:13:13.000000 opsramp-analytics-utils-3.5.5/setup.py
```

### Comparing `opsramp-analytics-utils-3.5.4/LICENSE` & `opsramp-analytics-utils-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/PKG-INFO` & `opsramp-analytics-utils-3.5.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.4
+Version: 3.5.5
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.4/README.md` & `opsramp-analytics-utils-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.5.5/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/api/api_client.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,14 @@
                         else:
                             uri = self.add_page_no_page_size_for_url(add_pageNo, url, page_no, page_size)
                             res = self.get_response(uri, type)
                         if res == None or not res.ok:
                             error_message = f'Get {type} API is failed, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}'
                             logger.error('Get %s API is failed, run_id ::: %s, url ::: %s, response ::: %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
-                            if res.status_code == 410:
-                                break
                             if retry_count > 3:
                                 raise Exception(error_message)
                         elif res.json() is not None and "results" not in res.json():
                             error_message = f"Get {type} results keyword is missing in API response, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}"
                             logger.error('Get %s results keyword is missing in API response, run_id ::: %s, url ::: %s, response : %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
                             if retry_count > 3:
```

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/api/api_task.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/api/api_task.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/api/thread_process.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/api/thread_process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/api_client.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,14 @@
                         else:
                             uri = self.add_page_no_page_size_for_url(add_pageNo, url, page_no, page_size)
                             res = self.get_response(uri, type)
                         if res == None or not res.ok:
                             error_message = f'Get {type} API is failed, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}'
                             logger.error('Get %s API is failed, run_id ::: %s, url ::: %s, response ::: %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
-                            if res.status_code == 410:
-                                break
                             if retry_count > 3:
                                 raise Exception(error_message)
                         elif res.json() is not None and "results" not in res.json():
                             error_message = f"Get {type} results keyword is missing in API response, run_id ::: {self.run_id}, url ::: {url}, response ::: {res}, response_json ::: {res.json()}, API_Retry_Count ::: {retry_count}"
                             logger.error('Get %s results keyword is missing in API response, run_id ::: %s, url ::: %s, response : %s, response_json ::: %s, API_Retry_Count ::: %s ', type, self.run_id, url, res, res.json(), retry_count)
                             res = None
                             if retry_count > 3:
```

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/components.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/excel.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/excel_writer.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/excel_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import xlsxwriter
-from openpyxl.cell.cell import ILLEGAL_CHARACTERS_RE
 from analytics_sdk.utilities import (
     APP_ID,
     APP_DISPLAY_NAME,
     upload_file
 )
 
 class ExcelWriter:
@@ -11,15 +10,15 @@
     DATA_PER_SHEET_LIMIT = 1000001
     ROW_START = 3
     CONTENT_ROW_START = 0
     def __init__(self, run_id, file_name, app_id):
         self.run_id = run_id
         self.file_name = file_name
         self.app_id = app_id
-        self.wb = xlsxwriter.Workbook(self.file_name, {'constant_memory':True})
+        self.wb = xlsxwriter.Workbook(self.file_name, {'constant_memory':True, 'nan_inf_to_errors': True})
         self.total_sheet_row_counts = {}
         self.active_sheet_title = ''
         self.sheet_refs = {}
         self.run_params = None
 
 
     def create_sheet(self, sheet_title):
@@ -97,14 +96,16 @@
     def get_value(self, value):
         if value:
             try:
                 value = float(value)
                 return value
             except ValueError:
                 return value
+            except Exception as e:
+                return value
         return value
 
     def render_table(self, title, headers, data, row_start=1, col_start=1):
         column_widths = {}
         if data:
             sheet_count = 1
             ws = self.create_sheet(title)
@@ -125,15 +126,15 @@
                     ws = self.create_sheet(new_title)
                     self.add_headers(ws)
                     if self.active_sheet_title not in self.total_sheet_row_counts:
                         self.total_sheet_row_counts[self.active_sheet_title] = 0
                 if row_no == ExcelWriter.CONTENT_ROW_START:
                     # Adding table title here
                     # ws.write_row(row_no-1, 0, [title], self.wb.add_format({'font_color': '00598B', 'bold':True}))
-                    ws.write_row(row_no, 0, headers[0], self.wb.add_format({'bold': True, 'border': 1, 'bg_color': '#4F81BD', 'font_color':'#FFFFFF', 'border': 2, 'border_color': '#FFFFFF'}))
+                    ws.write_row(row_no, 0, headers[0], self.wb.add_format({'bold': True, 'bg_color': '#7D92AF', 'font_color':'#FFFFFF', 'border': 2, 'border_color': '#FFFFFF'}))
                     row_no += 1
                 for col_delta, val in enumerate(_row):
                     cell_position = xlsxwriter.utility.xl_rowcol_to_cell(row_no, col_delta)
                     bg_color = '#DCE6F1'
                     try:
                         if APP_ID == 'AVAILABILITY-DETAILS':
                             if isinstance(val, str) and 'COLOR-CODE_' in val:
@@ -141,19 +142,18 @@
                                 if len(vals) == 3:
                                     val = vals[2]
                                     if vals[1] is not None and len(vals[1]):
                                         bg_color = vals[1]
                         val = self.get_value(val)
                     except Exception as e:
                         print('ExcelWriter: found exception... value is :: ', val)
-                        print('ExcelWriter: with open xl illegal char : ', ILLEGAL_CHARACTERS_RE.sub(r'', val))
-                        if isinstance(val, str):
-                            val = ILLEGAL_CHARACTERS_RE.sub(r'', val)
-                        else:
-                            val = self.get_value(val)
+                        try:
+                            val = str(val)
+                        except Exception as ex:
+                            val = ''
                     ws.write(cell_position, val, self.wb.add_format({'bg_color': bg_color, 'border': 1, 'border_color': '#FFFFFF'}))
                     if col_delta in column_widths:
                         column_widths[col_delta] = max(len(str(val)), column_widths[col_delta])
                     else:
                         column_widths[col_delta] = max(len(str(val)), 8)
                 row_no += 1
                 self.total_sheet_row_counts[new_title] = row_no
@@ -290,32 +290,31 @@
                         self.total_sheet_row_counts[self.active_sheet_title] = 0
                 if row_no == ExcelWriter.CONTENT_ROW_START:
                     # Adding table title here
                     # ws.write_row(row_no, 0, headers[0], self.wb.add_format({'bold': True, 'border': 1, 'bg_color': '#4F81BD', 'font_color':'#FFFFFF', 'border': 2, 'border_color': '#FFFFFF'}))
                     for header in headers:
                         for col_delta, val in enumerate(header):
                             cell_position = xlsxwriter.utility.xl_rowcol_to_cell(row_no, col_delta)
-                            ws.write(cell_position, self.get_value(val), self.wb.add_format({'bold': True, 'border': 1, 'bg_color': '#4F81BD', 'font_color':'#FFFFFF', 'border': 2, 'border_color': '#FFFFFF'}))
+                            ws.write(cell_position, self.get_value(val), self.wb.add_format({'align': 'center', 'bold': True, 'bg_color': '#7D92AF', 'font_color':'#FFFFFF', 'border': 0, 'border_color': '#FFFFFF'}))
                             if col_delta in column_widths:
                                 column_widths[col_delta] = max(len(str(val)), column_widths[col_delta])
                             else:
                                 column_widths[col_delta] = max(len(str(val)), 8)
                         row_no += 1
                 for col_delta, val in enumerate(_row):
                     cell_position = xlsxwriter.utility.xl_rowcol_to_cell(row_no, col_delta)
                     bg_color = '#DCE6F1'
                     try:
                         val = self.get_value(val)
                     except Exception as e:
                         print('ExcelWriter: found exception... value is :: ', val)
-                        print('ExcelWriter: with open xl illegal char : ', ILLEGAL_CHARACTERS_RE.sub(r'', val))
-                        if isinstance(val, str):
-                            val = ILLEGAL_CHARACTERS_RE.sub(r'', val)
-                        else:
-                            val = self.get_value(val)
+                        try:
+                            val = str(val)
+                        except Exception as ex:
+                            val = ''
                     ws.write(cell_position, val, self.wb.add_format({'bg_color': bg_color, 'border': 1, 'border_color': '#FFFFFF'}))
                     if col_delta in column_widths:
                         column_widths[col_delta] = max(len(str(val)), column_widths[col_delta])
                     else:
                         column_widths[col_delta] = max(len(str(val)), 8)
                 row_no += 1
                 self.total_sheet_row_counts[new_title] = row_no
```

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.5.5/analytics_sdk/utilities.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.4
+Version: 3.5.5
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.4/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.5.5/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.4/setup.py` & `opsramp-analytics-utils-3.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.5.4",
+    version="3.5.5",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     # url="https://github.com/opsramp/analytics-sdk",
```

