# Comparing `tmp/skysurvey-0.9.2.tar.gz` & `tmp/skysurvey-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.9.2.tar", last modified: Wed Sep 20 07:23:39 2023, max compression
+gzip compressed data, was "skysurvey-0.9.3.tar", last modified: Wed Sep 20 13:14:19 2023, max compression
```

## Comparing `skysurvey-0.9.2.tar` & `skysurvey-0.9.3.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.898731 skysurvey-0.9.2/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.9.2/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)     1199 2023-09-20 07:23:39.898655 skysurvey-0.9.2/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2064 2023-09-17 16:45:52.000000 skysurvey-0.9.2/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1205 2023-09-20 07:23:39.899076 skysurvey-0.9.2/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.9.2/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.889158 skysurvey-0.9.2/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       90 2023-09-20 07:23:21.000000 skysurvey-0.9.2/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      524 2023-06-27 13:24:20.000000 skysurvey-0.9.2/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)    28021 2023-09-14 11:24:51.000000 skysurvey-0.9.2/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.890396 skysurvey-0.9.2/skysurvey/effects/
--rw-r--r--   0 rigault   (2358) staff       (20)     2975 2023-09-14 21:01:45.000000 skysurvey-0.9.2/skysurvey/effects/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     6104 2023-09-14 15:16:44.000000 skysurvey-0.9.2/skysurvey/effects/dust.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.890858 skysurvey-0.9.2/skysurvey/examples/
--rw-r--r--   0 rigault   (2358) staff       (20)       26 2023-06-29 14:59:14.000000 skysurvey-0.9.2/skysurvey/examples/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2233 2023-06-29 14:59:29.000000 skysurvey-0.9.2/skysurvey/examples/mocksurvey.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.893414 skysurvey-0.9.2/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      125 2023-06-28 15:34:39.000000 skysurvey-0.9.2/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     9812 2023-08-17 15:28:29.000000 skysurvey-0.9.2/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2849 2023-06-29 07:52:19.000000 skysurvey-0.9.2/skysurvey/survey/des.py
--rw-r--r--   0 rigault   (2358) staff       (20)    17200 2023-09-13 18:49:07.000000 skysurvey-0.9.2/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)      976 2023-06-30 08:20:21.000000 skysurvey-0.9.2/skysurvey/survey/lsst.py
--rw-r--r--   0 rigault   (2358) staff       (20)    13296 2023-09-13 18:49:07.000000 skysurvey-0.9.2/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8945 2023-09-13 18:49:07.000000 skysurvey-0.9.2/skysurvey/survey/survey.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1938 2023-07-19 09:47:02.000000 skysurvey-0.9.2/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.896576 skysurvey-0.9.2/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.9.2/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    12064 2023-06-30 12:09:56.000000 skysurvey-0.9.2/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    38150 2023-09-19 19:37:36.000000 skysurvey-0.9.2/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.9.2/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)     3394 2023-07-20 21:35:56.000000 skysurvey-0.9.2/skysurvey/target/host.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.9.2/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.9.2/skysurvey/target/sncc.py
--rw-r--r--   0 rigault   (2358) staff       (20)    17887 2023-09-14 11:51:08.000000 skysurvey-0.9.2/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.9.2/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     4569 2023-08-17 10:39:43.000000 skysurvey-0.9.2/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    16795 2023-09-14 15:24:36.000000 skysurvey-0.9.2/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.897902 skysurvey-0.9.2/skysurvey/tools/
--rw-r--r--   0 rigault   (2358) staff       (20)       64 2023-06-29 10:12:11.000000 skysurvey-0.9.2/skysurvey/tools/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5602 2023-09-14 08:06:42.000000 skysurvey-0.9.2/skysurvey/tools/blackbody.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2301 2023-06-27 14:26:14.000000 skysurvey-0.9.2/skysurvey/tools/snana.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2762 2023-06-27 08:23:39.000000 skysurvey-0.9.2/skysurvey/tools/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 07:23:39.890170 skysurvey-0.9.2/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)     1199 2023-09-20 07:23:39.000000 skysurvey-0.9.2/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     1032 2023-09-20 07:23:39.000000 skysurvey-0.9.2/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-09-20 07:23:39.000000 skysurvey-0.9.2/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.9.2/skysurvey.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      194 2023-09-20 07:23:39.000000 skysurvey-0.9.2/skysurvey.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-09-20 07:23:39.000000 skysurvey-0.9.2/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.444043 skysurvey-0.9.3/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.9.3/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)     1199 2023-09-20 13:14:19.443977 skysurvey-0.9.3/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2064 2023-09-17 16:45:52.000000 skysurvey-0.9.3/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1205 2023-09-20 13:14:19.444349 skysurvey-0.9.3/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-06-12 09:49:45.000000 skysurvey-0.9.3/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.439608 skysurvey-0.9.3/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       90 2023-09-20 13:13:47.000000 skysurvey-0.9.3/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      524 2023-06-27 13:24:20.000000 skysurvey-0.9.3/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    28021 2023-09-14 11:24:51.000000 skysurvey-0.9.3/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.440706 skysurvey-0.9.3/skysurvey/effects/
+-rw-r--r--   0 rigault   (2358) staff       (20)     2975 2023-09-14 21:01:45.000000 skysurvey-0.9.3/skysurvey/effects/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     6104 2023-09-14 15:16:44.000000 skysurvey-0.9.3/skysurvey/effects/dust.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.440926 skysurvey-0.9.3/skysurvey/examples/
+-rw-r--r--   0 rigault   (2358) staff       (20)       26 2023-06-29 14:59:14.000000 skysurvey-0.9.3/skysurvey/examples/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2233 2023-06-29 14:59:29.000000 skysurvey-0.9.3/skysurvey/examples/mocksurvey.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.441853 skysurvey-0.9.3/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      125 2023-06-28 15:34:39.000000 skysurvey-0.9.3/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     9812 2023-08-17 15:28:29.000000 skysurvey-0.9.3/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2849 2023-06-29 07:52:19.000000 skysurvey-0.9.3/skysurvey/survey/des.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    17200 2023-09-13 18:49:07.000000 skysurvey-0.9.3/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      976 2023-06-30 08:20:21.000000 skysurvey-0.9.3/skysurvey/survey/lsst.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    13296 2023-09-13 18:49:07.000000 skysurvey-0.9.3/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8945 2023-09-13 18:49:07.000000 skysurvey-0.9.3/skysurvey/survey/survey.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1938 2023-07-19 09:47:02.000000 skysurvey-0.9.3/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.443112 skysurvey-0.9.3/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.9.3/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1823 2023-09-20 13:13:19.000000 skysurvey-0.9.3/skysurvey/target/afterglow.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    12064 2023-06-30 12:09:56.000000 skysurvey-0.9.3/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    38150 2023-09-19 19:37:36.000000 skysurvey-0.9.3/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.9.3/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3394 2023-07-20 21:35:56.000000 skysurvey-0.9.3/skysurvey/target/host.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.9.3/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2341 2023-06-09 12:22:54.000000 skysurvey-0.9.3/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    17887 2023-09-14 11:51:08.000000 skysurvey-0.9.3/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-06-02 09:01:21.000000 skysurvey-0.9.3/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     4569 2023-08-17 10:39:43.000000 skysurvey-0.9.3/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16795 2023-09-14 15:24:36.000000 skysurvey-0.9.3/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.443518 skysurvey-0.9.3/skysurvey/tools/
+-rw-r--r--   0 rigault   (2358) staff       (20)       64 2023-06-29 10:12:11.000000 skysurvey-0.9.3/skysurvey/tools/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5602 2023-09-14 08:06:42.000000 skysurvey-0.9.3/skysurvey/tools/blackbody.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2301 2023-06-27 14:26:14.000000 skysurvey-0.9.3/skysurvey/tools/snana.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2762 2023-06-27 08:23:39.000000 skysurvey-0.9.3/skysurvey/tools/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-09-20 13:14:19.440485 skysurvey-0.9.3/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)     1199 2023-09-20 13:14:19.000000 skysurvey-0.9.3/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     1062 2023-09-20 13:14:19.000000 skysurvey-0.9.3/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-09-20 13:14:19.000000 skysurvey-0.9.3/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-12 09:47:03.000000 skysurvey-0.9.3/skysurvey.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      194 2023-09-20 13:14:19.000000 skysurvey-0.9.3/skysurvey.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-09-20 13:14:19.000000 skysurvey-0.9.3/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.9.2/LICENSE` & `skysurvey-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/PKG-INFO` & `skysurvey-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.9.2
+Version: 0.9.3
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.9.2/README.md` & `skysurvey-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/setup.cfg` & `skysurvey-0.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/config.py` & `skysurvey-0.9.3/skysurvey/config.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/dataset.py` & `skysurvey-0.9.3/skysurvey/dataset.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/effects/__init__.py` & `skysurvey-0.9.3/skysurvey/effects/__init__.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/effects/dust.py` & `skysurvey-0.9.3/skysurvey/effects/dust.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/examples/mocksurvey.py` & `skysurvey-0.9.3/skysurvey/examples/mocksurvey.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/survey/core.py` & `skysurvey-0.9.3/skysurvey/survey/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/survey/des.py` & `skysurvey-0.9.3/skysurvey/survey/des.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/survey/healpix.py` & `skysurvey-0.9.3/skysurvey/survey/healpix.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/survey/lsst.py` & `skysurvey-0.9.3/skysurvey/survey/lsst.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/survey/polygon.py` & `skysurvey-0.9.3/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/survey/survey.py` & `skysurvey-0.9.3/skysurvey/survey/survey.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/survey/ztf.py` & `skysurvey-0.9.3/skysurvey/survey/ztf.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/target/collection.py` & `skysurvey-0.9.3/skysurvey/target/collection.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/target/core.py` & `skysurvey-0.9.3/skysurvey/target/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/target/host.py` & `skysurvey-0.9.3/skysurvey/target/host.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/target/sncc.py` & `skysurvey-0.9.3/skysurvey/target/sncc.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/target/snia.py` & `skysurvey-0.9.3/skysurvey/target/snia.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/target/stars.py` & `skysurvey-0.9.3/skysurvey/target/stars.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/target/timeserie.py` & `skysurvey-0.9.3/skysurvey/target/timeserie.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/template.py` & `skysurvey-0.9.3/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/tools/blackbody.py` & `skysurvey-0.9.3/skysurvey/tools/blackbody.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/tools/snana.py` & `skysurvey-0.9.3/skysurvey/tools/snana.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey/tools/utils.py` & `skysurvey-0.9.3/skysurvey/tools/utils.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.9.2/skysurvey.egg-info/PKG-INFO` & `skysurvey-0.9.3/skysurvey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skysurvey
-Version: 0.9.2
+Version: 0.9.3
 Summary: Simulating Transient in the sky and how to observe them
 Home-page: https://github.com/MickaelRigault/skysurvey
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `skysurvey-0.9.2/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.9.3/skysurvey.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 skysurvey/survey/des.py
 skysurvey/survey/healpix.py
 skysurvey/survey/lsst.py
 skysurvey/survey/polygon.py
 skysurvey/survey/survey.py
 skysurvey/survey/ztf.py
 skysurvey/target/__init__.py
+skysurvey/target/afterglow.py
 skysurvey/target/collection.py
 skysurvey/target/core.py
 skysurvey/target/environments.py
 skysurvey/target/host.py
 skysurvey/target/kilonova.py
 skysurvey/target/sncc.py
 skysurvey/target/snia.py
```

