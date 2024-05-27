# Comparing `tmp/pygmtsar-2024.4.17.post8.tar.gz` & `tmp/pygmtsar-2024.4.17.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.4.17.post8.tar", last modified: Mon May 20 14:18:12 2024, max compression
+gzip compressed data, was "pygmtsar-2024.4.17.post9.tar", last modified: Tue May 21 08:04:48 2024, max compression
```

## Comparing `pygmtsar-2024.4.17.post8.tar` & `pygmtsar-2024.4.17.post9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-20 14:18:12.627515 pygmtsar-2024.4.17.post8/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post8/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-20 14:18:12.624869 pygmtsar-2024.4.17.post8/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post8/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-20 14:18:12.618288 pygmtsar-2024.4.17.post8/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post8/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post8/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post8/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post8/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post8/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post8/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post8/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post8/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5706 2024-05-19 15:27:12.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44539 2024-05-08 11:23:30.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47608 2024-05-07 07:53:29.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    48188 2024-05-20 08:24:15.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     9599 2024-05-15 06:53:05.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post8/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)    10511 2024-05-18 08:33:45.000000 pygmtsar-2024.4.17.post8/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post8/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-05-20 08:15:48.000000 pygmtsar-2024.4.17.post8/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post8/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post8/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post8/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post8/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-20 14:18:12.624554 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-05-20 14:18:12.000000 pygmtsar-2024.4.17.post8/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-05-20 14:18:12.627570 pygmtsar-2024.4.17.post8/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-05-20 06:11:34.000000 pygmtsar-2024.4.17.post8/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-21 08:04:48.788749 pygmtsar-2024.4.17.post9/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.4.17.post9/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-21 08:04:48.788486 pygmtsar-2024.4.17.post9/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.4.17.post9/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-21 08:04:48.786946 pygmtsar-2024.4.17.post9/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    18153 2024-04-26 09:12:06.000000 pygmtsar-2024.4.17.post9/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.4.17.post9/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.4.17.post9/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.4.17.post9/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.4.17.post9/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.4.17.post9/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.4.17.post9/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19225 2024-04-17 06:56:07.000000 pygmtsar-2024.4.17.post9/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5706 2024-05-19 15:27:12.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44539 2024-05-08 11:23:30.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47608 2024-05-07 07:53:29.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9440 2024-05-21 07:34:41.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    48188 2024-05-20 08:24:15.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9599 2024-05-15 06:53:05.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    27198 2024-04-28 10:15:51.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.4.17.post9/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.4.17.post9/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10511 2024-05-18 08:33:45.000000 pygmtsar-2024.4.17.post9/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.4.17.post9/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1040 2024-05-21 07:03:00.000000 pygmtsar-2024.4.17.post9/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.4.17.post9/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.4.17.post9/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.4.17.post9/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.4.17.post9/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-05-21 08:04:48.788184 pygmtsar-2024.4.17.post9/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-05-21 08:04:48.000000 pygmtsar-2024.4.17.post9/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1116 2024-05-21 08:04:48.000000 pygmtsar-2024.4.17.post9/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-05-21 08:04:48.000000 pygmtsar-2024.4.17.post9/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-05-21 08:04:48.000000 pygmtsar-2024.4.17.post9/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-05-21 08:04:48.000000 pygmtsar-2024.4.17.post9/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-05-21 08:04:48.788798 pygmtsar-2024.4.17.post9/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-05-20 06:11:34.000000 pygmtsar-2024.4.17.post9/setup.py
```

### Comparing `pygmtsar-2024.4.17.post8/LICENSE.txt` & `pygmtsar-2024.4.17.post9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/PKG-INFO` & `pygmtsar-2024.4.17.post9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post8
+Version: 2024.4.17.post9
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post8/README.md` & `pygmtsar-2024.4.17.post9/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/ASF.py` & `pygmtsar-2024.4.17.post9/pygmtsar/ASF.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/AWS.py` & `pygmtsar-2024.4.17.post9/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/GMT.py` & `pygmtsar-2024.4.17.post9/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/IO.py` & `pygmtsar-2024.4.17.post9/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.4.17.post9/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/PRM.py` & `pygmtsar-2024.4.17.post9/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.4.17.post9/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/S1.py` & `pygmtsar-2024.4.17.post9/pygmtsar/S1.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_align.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_base.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_dem.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_export.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_phasediff.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_prm.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_ps.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_reframe.py`

 * *Files 13% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         out['metapath'] = new_filename + '.xml'
         out['datapath'] = new_filename + '.tiff'
         # update approximate location
         out['geometry'] = cascaded_union([geom for multi_polygon in df.geometry for geom in multi_polygon.geoms
                                       if geom.intersects(geometry)])
         return out
 
-    def compute_reframe(self, geometry=None, n_jobs=-1, **kwargs):
+    def compute_reframe(self, geometry=None, n_jobs=-1, queue=16, caption='Reframing', **kwargs):
         """
         Reorder bursts from sequential scenes to cover the full orbit area or some bursts only.
 
         Parameters
         ----------
         geometry: shapely.geometry of geopandas.GeoSeries or geopandas.GeoDataFrame
             Optional geometry covering required bursts to crop the area.
@@ -170,25 +170,50 @@
         TODO: Define a point on a selected burst (this option is not available now):
         stack.reframe(geometry=Point(25.3, 35))
         """
         from tqdm.auto import tqdm
         import joblib
         import pandas as pd
 
+        if n_jobs is None or ('debug' in kwargs and kwargs['debug'] == True):
+            print ('Note: sequential joblib processing is applied when "n_jobs" is None or "debug" is True.')
+            joblib_backend = 'sequential'
+        else:
+            joblib_backend = 'loky'
+            
         dates = self.df.index.unique().values
         subswaths = self.get_subswaths()
         # approximate subswath geometries from GCP
         geometries = {subswath: self.df[self.df.subswath==subswath].geometry.unary_union for subswath in subswaths}
 
-        # process all the scenes
-        if n_jobs is None or ('debug' in kwargs and kwargs['debug'] == True):
-            print ('Note: sequential joblib processing is applied when "n_jobs" is None or "debug" is True.')
-            joblib_backend = 'sequential'
+        records = []
+        # Applying iterative processing to prevent Dask scheduler deadlocks.
+        stacksize = len(dates)
+        counter = 0
+        digits = len(str(stacksize))
+        # Splitting all the dates into chunks, each containing approximately queue dates.
+        #n_chunks = stacksize // queue if stacksize > queue else 1
+        if stacksize > queue:
+            chunks = [dates[i:i + queue] for i in range(0, stacksize, queue)]
+            n_chunks = len(chunks)
         else:
-            joblib_backend = None
-        with self.tqdm_joblib(tqdm(desc='Reframing', total=len(dates)*len(subswaths))) as progress_bar:
-            records = joblib.Parallel(n_jobs=n_jobs, backend=joblib_backend)(joblib.delayed(self._reframe_subswath)\
-                            (subswath, date,
-                            geometry.intersection(geometries[subswath]) if geometry is not None else geometries[subswath],
-                            **kwargs) for date in dates for subswath in subswaths)
+            chunks = [dates]
+            n_chunks = 1
+        for chunk in chunks:
+            if n_chunks > 1:
+                chunk_caption = f'{caption}: {(counter+1):0{digits}}...{(counter+len(chunk)):0{digits}} from {stacksize}'
+            else:
+                chunk_caption = caption
+            
+            if joblib_backend == 'loky':
+                # can be missed on some systems
+                from joblib.externals import loky
+                loky.get_reusable_executor(kill_workers=True).shutdown(wait=True)
+            with self.tqdm_joblib(tqdm(desc=chunk_caption, total=len(chunk)*len(subswaths))) as progress_bar:
+                chunk_records = joblib.Parallel(n_jobs=n_jobs, backend=joblib_backend)(joblib.delayed(self._reframe_subswath)\
+                                (subswath, date,
+                                geometry.intersection(geometries[subswath]) if geometry is not None else geometries[subswath],
+                                **kwargs) for date in chunk for subswath in subswaths)
+                records.extend(chunk_records)
+            counter += len(chunk)
 
         self.df = pd.concat(records)
```

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_sbas.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_stl.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_stl.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_topo.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_unwrap.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/Tiles.py` & `pygmtsar-2024.4.17.post9/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/XYZTiles.py` & `pygmtsar-2024.4.17.post9/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.4.17.post9/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/__init__.py` & `pygmtsar-2024.4.17.post9/pygmtsar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.4.17.post8'
+__version__ = '2024.4.17.post9'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/datagrid.py` & `pygmtsar-2024.4.17.post9/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.4.17.post9/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.4.17.post9/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar/utils.py` & `pygmtsar-2024.4.17.post9/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.4.17.post9/pygmtsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.4.17.post8
+Version: 2024.4.17.post9
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pygmtsar-2024.4.17.post8/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.4.17.post9/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.4.17.post8/setup.py` & `pygmtsar-2024.4.17.post9/setup.py`

 * *Files identical despite different names*

