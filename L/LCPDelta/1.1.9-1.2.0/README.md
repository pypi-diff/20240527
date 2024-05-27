# Comparing `tmp/LCPDelta-1.1.9.tar.gz` & `tmp/lcpdelta-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LCPDelta-1.1.9.tar", last modified: Fri Apr  5 16:59:29 2024, max compression
+gzip compressed data, was "lcpdelta-1.2.0.tar", last modified: Mon May 27 10:15:03 2024, max compression
```

## Comparing `LCPDelta-1.1.9.tar` & `lcpdelta-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.091615 LCPDelta-1.1.9/
--rw-rw-rw-   0        0        0      132 2023-11-09 09:59:32.000000 LCPDelta-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     3405 2024-04-05 16:59:29.089618 LCPDelta-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2799 2024-04-05 16:56:19.000000 LCPDelta-1.1.9/README.md
--rw-rw-rw-   0        0        0      686 2024-04-05 16:56:45.000000 LCPDelta-1.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 16:59:29.091615 LCPDelta-1.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:28.897045 LCPDelta-1.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.086675 LCPDelta-1.1.9/src/LCPDelta.egg-info/
--rw-rw-rw-   0        0        0     3405 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:28.964763 LCPDelta-1.1.9/src/lcp_delta/
--rw-rw-rw-   0        0        0       21 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:28.988898 LCPDelta-1.1.9/src/lcp_delta/common/
--rw-rw-rw-   0        0        0       39 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/common/__init__.py
--rw-rw-rw-   0        0        0     3462 2024-02-08 15:41:52.000000 LCPDelta-1.1.9/src/lcp_delta/common/api_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.053088 LCPDelta-1.1.9/src/lcp_delta/enact/
--rw-rw-rw-   0        0        0      160 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/enact/__init__.py
--rw-rw-rw-   0        0        0    49069 2024-04-05 16:56:19.000000 LCPDelta-1.1.9/src/lcp_delta/enact/api_helper.py
--rw-rw-rw-   0        0        0     1790 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/enact/chart_helper.py
--rw-rw-rw-   0        0        0     4026 2024-02-01 10:06:56.000000 LCPDelta-1.1.9/src/lcp_delta/enact/credentials_holder.py
--rw-rw-rw-   0        0        0     7938 2024-03-15 17:02:19.000000 LCPDelta-1.1.9/src/lcp_delta/enact/dps_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.063099 LCPDelta-1.1.9/src/lcp_delta/enact/response_objects/
--rw-rw-rw-   0        0        0      363 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/enact/response_objects/usage_info.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.084622 LCPDelta-1.1.9/src/lcp_delta/flextrack/
--rw-rw-rw-   0        0        0       91 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/flextrack/__init__.py
--rw-rw-rw-   0        0        0     3495 2023-11-30 10:40:08.000000 LCPDelta-1.1.9/src/lcp_delta/flextrack/api_helper.py
--rw-rw-rw-   0        0        0      626 2024-02-08 17:40:02.000000 LCPDelta-1.1.9/src/lcp_delta/global_helper_methods.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.544933 lcpdelta-1.2.0/
+-rw-rw-rw-   0        0        0    11556 2024-05-27 10:11:07.000000 lcpdelta-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    16586 2024-05-27 10:15:03.542926 lcpdelta-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2799 2024-05-15 10:50:21.000000 lcpdelta-1.2.0/README.md
+-rw-rw-rw-   0        0        0      732 2024-05-27 10:14:30.000000 lcpdelta-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:15:03.545925 lcpdelta-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.454167 lcpdelta-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.539917 lcpdelta-1.2.0/src/LCPDelta.egg-info/
+-rw-rw-rw-   0        0        0    16586 2024-05-27 10:15:03.000000 lcpdelta-1.2.0/src/LCPDelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2024-05-27 10:15:03.000000 lcpdelta-1.2.0/src/LCPDelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:15:03.000000 lcpdelta-1.2.0/src/LCPDelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-27 10:15:03.000000 lcpdelta-1.2.0/src/LCPDelta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-27 10:15:03.000000 lcpdelta-1.2.0/src/LCPDelta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.507533 lcpdelta-1.2.0/src/lcp_delta/
+-rw-rw-rw-   0        0        0       21 2023-11-20 17:21:16.000000 lcpdelta-1.2.0/src/lcp_delta/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.513126 lcpdelta-1.2.0/src/lcp_delta/common/
+-rw-rw-rw-   0        0        0       39 2023-11-20 17:21:16.000000 lcpdelta-1.2.0/src/lcp_delta/common/__init__.py
+-rw-rw-rw-   0        0        0     3462 2023-11-20 17:21:16.000000 lcpdelta-1.2.0/src/lcp_delta/common/api_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.528268 lcpdelta-1.2.0/src/lcp_delta/enact/
+-rw-rw-rw-   0        0        0      160 2024-02-01 15:42:37.000000 lcpdelta-1.2.0/src/lcp_delta/enact/__init__.py
+-rw-rw-rw-   0        0        0    49069 2024-05-15 10:50:21.000000 lcpdelta-1.2.0/src/lcp_delta/enact/api_helper.py
+-rw-rw-rw-   0        0        0     1790 2024-02-01 15:42:37.000000 lcpdelta-1.2.0/src/lcp_delta/enact/chart_helper.py
+-rw-rw-rw-   0        0        0     4026 2023-11-20 17:21:16.000000 lcpdelta-1.2.0/src/lcp_delta/enact/credentials_holder.py
+-rw-rw-rw-   0        0        0     7938 2024-02-13 10:29:37.000000 lcpdelta-1.2.0/src/lcp_delta/enact/dps_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.530935 lcpdelta-1.2.0/src/lcp_delta/enact/response_objects/
+-rw-rw-rw-   0        0        0      363 2023-11-20 17:21:16.000000 lcpdelta-1.2.0/src/lcp_delta/enact/response_objects/usage_info.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:15:03.536358 lcpdelta-1.2.0/src/lcp_delta/flextrack/
+-rw-rw-rw-   0        0        0       91 2023-11-20 17:21:16.000000 lcpdelta-1.2.0/src/lcp_delta/flextrack/__init__.py
+-rw-rw-rw-   0        0        0     3495 2023-11-23 16:23:55.000000 lcpdelta-1.2.0/src/lcp_delta/flextrack/api_helper.py
+-rw-rw-rw-   0        0        0      626 2024-02-13 10:29:37.000000 lcpdelta-1.2.0/src/lcp_delta/global_helper_methods.py
```

### Comparing `LCPDelta-1.1.9/README.md` & `lcpdelta-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/pyproject.toml` & `lcpdelta-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LCPDelta"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="LCP Delta", email="enact.helpdesk@lcp.uk.com" },
 ]
 description = "LCPDelta Python Package"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["LCPDelta", "Enact", "Flextrack", "Storetrack"]
+license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
-    'License :: Other/Proprietary License',
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
     "pandas",
     "requests",
     "signalrcore",
```

### Comparing `LCPDelta-1.1.9/src/LCPDelta.egg-info/SOURCES.txt` & `lcpdelta-1.2.0/src/LCPDelta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/src/lcp_delta/common/api_helper.py` & `lcpdelta-1.2.0/src/lcp_delta/common/api_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/src/lcp_delta/enact/api_helper.py` & `lcpdelta-1.2.0/src/lcp_delta/enact/api_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/src/lcp_delta/enact/chart_helper.py` & `lcpdelta-1.2.0/src/lcp_delta/enact/chart_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/src/lcp_delta/enact/credentials_holder.py` & `lcpdelta-1.2.0/src/lcp_delta/enact/credentials_holder.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/src/lcp_delta/enact/dps_helper.py` & `lcpdelta-1.2.0/src/lcp_delta/enact/dps_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/src/lcp_delta/flextrack/api_helper.py` & `lcpdelta-1.2.0/src/lcp_delta/flextrack/api_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.9/src/lcp_delta/global_helper_methods.py` & `lcpdelta-1.2.0/src/lcp_delta/global_helper_methods.py`

 * *Files identical despite different names*

