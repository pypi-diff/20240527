# Comparing `tmp/glassestools-0.5.1.tar.gz` & `tmp/glassestools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassestools-0.5.1.tar", last modified: Fri May 24 18:46:52 2024, max compression
+gzip compressed data, was "glassestools-1.0.0.tar", last modified: Sun May 26 22:42:34 2024, max compression
```

## Comparing `glassestools-0.5.1.tar` & `glassestools-1.0.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:46:52.771605 glassestools-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-24 18:46:48.000000 glassestools-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 18:46:48.000000 glassestools-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-24 18:46:52.767605 glassestools-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-24 18:46:48.000000 glassestools-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-24 18:46:48.000000 glassestools-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 18:46:48.000000 glassestools-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:46:52.771605 glassestools-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-24 18:46:48.000000 glassestools-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:46:52.763605 glassestools-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:46:52.767605 glassestools-0.5.1/src/glassesTools/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/data_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/eyetracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/gaze_headref.py
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/gaze_worldref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:46:52.767605 glassestools-0.5.1/src/glassesTools/importing/
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/importing/SMI_ETG.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/importing/SeeTrue_STONE.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/importing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/importing/adhawk_mindlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/importing/pupilLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/importing/tobii_G2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/importing/tobii_G3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:46:52.767605 glassestools-0.5.1/src/glassesTools/mp4analyser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/mp4analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/mp4analyser/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    60401 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/mp4analyser/iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/mp4analyser/mpeglookups.py
--rw-r--r--   0 runner    (1001) docker     (127)    29359 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/mp4analyser/non_iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/mp4analyser/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/mp4analyser/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/ocv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-24 18:46:48.000000 glassestools-0.5.1/src/glassesTools/video_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:46:52.767605 glassestools-0.5.1/src/glassesTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-24 18:46:52.000000 glassestools-0.5.1/src/glassesTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-24 18:46:52.000000 glassestools-0.5.1/src/glassesTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:46:52.000000 glassestools-0.5.1/src/glassesTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 18:46:52.000000 glassestools-0.5.1/src/glassesTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 18:46:52.000000 glassestools-0.5.1/src/glassesTools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:42:34.669979 glassestools-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-26 22:42:30.000000 glassestools-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-26 22:42:30.000000 glassestools-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-26 22:42:34.669979 glassestools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-26 22:42:30.000000 glassestools-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-26 22:42:30.000000 glassestools-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-26 22:42:30.000000 glassestools-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 22:42:34.669979 glassestools-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-26 22:42:30.000000 glassestools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:42:34.657979 glassestools-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:42:34.661979 glassestools-1.0.0/src/glassesTools/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/aruco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/data_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/eyetracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/gaze_headref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/gaze_worldref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:42:34.665979 glassestools-1.0.0/src/glassesTools/importing/
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/importing/SMI_ETG.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/importing/SeeTrue_STONE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/importing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/importing/adhawk_mindlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/importing/pupilLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/importing/tobii_G2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/importing/tobii_G3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:42:34.669979 glassestools-1.0.0/src/glassesTools/mp4analyser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/mp4analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/mp4analyser/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60401 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/mp4analyser/iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/mp4analyser/mpeglookups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29359 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/mp4analyser/non_iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/mp4analyser/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/mp4analyser/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/ocv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-26 22:42:30.000000 glassestools-1.0.0/src/glassesTools/video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:42:34.669979 glassestools-1.0.0/src/glassesTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-26 22:42:34.000000 glassestools-1.0.0/src/glassesTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 22:42:34.000000 glassestools-1.0.0/src/glassesTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:42:34.000000 glassestools-1.0.0/src/glassesTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-26 22:42:34.000000 glassestools-1.0.0/src/glassesTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 22:42:34.000000 glassestools-1.0.0/src/glassesTools.egg-info/top_level.txt
```

### Comparing `glassestools-0.5.1/LICENSE` & `glassestools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/PKG-INFO` & `glassestools-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassesTools
-Version: 0.5.1
+Version: 1.0.0
 Summary: Tools for processing wearable eye tracker recordings.
 Home-page: https://github.com/dcnieho/glassesTools
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2022-2023 Diederick Niehorster
@@ -42,13 +42,13 @@
 Requires-Dist: ffpyplayer
 Requires-Dist: scipy==1.11.3
 
 [![Downloads](https://static.pepy.tech/badge/glassestools)](https://pepy.tech/project/glassestools)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/glassesTools.svg)](https://pypi.org/project/glassesTools/)
 [![image](https://img.shields.io/pypi/pyversions/glassesTools.svg)](https://pypi.org/project/glassesTools/)
 
-# GlassesTools v0.5.1
+# GlassesTools v1.0.0
 Tools for processing wearable eye tracker recordings.
 
 If you use this package or any of the code in this repository, please cite:<br>
 [Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2023). GlassesValidator:
 A data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5](https://doi.org/10.3758/s13428-023-02105-5)
```

### Comparing `glassestools-0.5.1/README.md` & `glassestools-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Downloads](https://static.pepy.tech/badge/glassestools)](https://pepy.tech/project/glassestools)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/glassesTools.svg)](https://pypi.org/project/glassesTools/)
 [![image](https://img.shields.io/pypi/pyversions/glassesTools.svg)](https://pypi.org/project/glassesTools/)
 
-# GlassesTools v0.5.1
+# GlassesTools v1.0.0
 Tools for processing wearable eye tracker recordings.
 
 If you use this package or any of the code in this repository, please cite:<br>
 [Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2023). GlassesValidator:
 A data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5](https://doi.org/10.3758/s13428-023-02105-5)
```

### Comparing `glassestools-0.5.1/setup.py` & `glassestools-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/drawing.py` & `glassestools-1.0.0/src/glassesTools/drawing.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/eyetracker.py` & `glassestools-1.0.0/src/glassesTools/eyetracker.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/importing/SMI_ETG.py` & `glassestools-1.0.0/src/glassesTools/importing/SMI_ETG.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/importing/SeeTrue_STONE.py` & `glassestools-1.0.0/src/glassesTools/importing/SeeTrue_STONE.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/importing/__init__.py` & `glassestools-1.0.0/src/glassesTools/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/importing/adhawk_mindlink.py` & `glassestools-1.0.0/src/glassesTools/importing/adhawk_mindlink.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/importing/pupilLabs.py` & `glassestools-1.0.0/src/glassesTools/importing/pupilLabs.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/importing/tobii_G2.py` & `glassestools-1.0.0/src/glassesTools/importing/tobii_G2.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/importing/tobii_G3.py` & `glassestools-1.0.0/src/glassesTools/importing/tobii_G3.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,19 +229,19 @@
     df = pd.DataFrame([],index=dfR.index)
     expander = lambda a,n: [[math.nan]*n if not isinstance(x,list) else x for x in a]
     # monocular gaze data
     for eye in ('left','right'):
         if 'data.eye'+eye+'.gazeorigin' not in dfR.columns:
             continue    # no data at all for this eye
         which_eye = eye[:1]
-        df[data_files.getXYZLabels('gaze_ori_'+which_eye,3)] = pd.DataFrame(expander(dfR['data.eye'+eye+'.gazeorigin'   ].tolist(),3), index=dfR.index)
-        df[data_files.getXYZLabels('gaze_dir_'+which_eye,3)] = pd.DataFrame(expander(dfR['data.eye'+eye+'.gazedirection'].tolist(),3), index=dfR.index)
+        df[data_files.getColumnLabels('gaze_ori_'+which_eye,3)] = pd.DataFrame(expander(dfR['data.eye'+eye+'.gazeorigin'   ].tolist(),3), index=dfR.index)
+        df[data_files.getColumnLabels('gaze_dir_'+which_eye,3)] = pd.DataFrame(expander(dfR['data.eye'+eye+'.gazedirection'].tolist(),3), index=dfR.index)
         df['pup_diam_'+which_eye] = dfR['data.eye'+eye+'.pupildiameter']
 
     # binocular gaze data
-    df[data_files.getXYZLabels('gaze_pos_3d',3) ] = pd.DataFrame(expander(dfR['data.gaze3d'].tolist(),3), index=dfR.index)
-    df[data_files.getXYZLabels('gaze_pos_vid',2)] = pd.DataFrame(expander(dfR['data.gaze2d'].tolist(),2), index=dfR.index)
+    df[data_files.getColumnLabels('gaze_pos_3d',3) ] = pd.DataFrame(expander(dfR['data.gaze3d'].tolist(),3), index=dfR.index)
+    df[data_files.getColumnLabels('gaze_pos_vid',2)] = pd.DataFrame(expander(dfR['data.gaze2d'].tolist(),2), index=dfR.index)
     df.loc[:,'gaze_pos_vid_x'] *= sceneVideoDimensions[0]
     df.loc[:,'gaze_pos_vid_y'] *= sceneVideoDimensions[1]
 
     # return the dataframe
     return df
```

### Comparing `glassestools-0.5.1/src/glassesTools/marker.py` & `glassestools-1.0.0/src/glassesTools/marker.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/mp4analyser/core.py` & `glassestools-1.0.0/src/glassesTools/mp4analyser/core.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/mp4analyser/iso.py` & `glassestools-1.0.0/src/glassesTools/mp4analyser/iso.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/mp4analyser/mpeglookups.py` & `glassestools-1.0.0/src/glassesTools/mp4analyser/mpeglookups.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/mp4analyser/non_iso.py` & `glassestools-1.0.0/src/glassesTools/mp4analyser/non_iso.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/mp4analyser/summary.py` & `glassestools-1.0.0/src/glassesTools/mp4analyser/summary.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/mp4analyser/util.py` & `glassestools-1.0.0/src/glassesTools/mp4analyser/util.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/ocv.py` & `glassestools-1.0.0/src/glassesTools/ocv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import numpy as np
 import pandas as pd
 import cv2
 import pathlib
 import bisect
 
 
-def arucoRefineDetectedMarkers(detector, image, arucoBoard, detectedCorners, detectedIds, rejectedCorners, cameraMatrix = None, distCoeffs= None):
-    corners, ids, rejectedImgPoints, recoveredIds = detector.refineDetectedMarkers(
-                            image = image, board = arucoBoard,
-                            detectedCorners = detectedCorners, detectedIds = detectedIds, rejectedCorners = rejectedCorners,
-                            cameraMatrix = cameraMatrix, distCoeffs = distCoeffs)
-    if corners and corners[0].shape[0]==4:
-        # there are versions out there where there is a bug in output shape of each set of corners, fix up
-        corners = [np.reshape(c,(1,4,2)) for c in corners]
-    if rejectedImgPoints and rejectedImgPoints[0].shape[0]==4:
-        # same as for corners
-        rejectedImgPoints = [np.reshape(c,(1,4,2)) for c in rejectedImgPoints]
-
-    return corners, ids, rejectedImgPoints, recoveredIds
-
-
-def readCameraCalibrationFile(fileName):
-    fs = cv2.FileStorage(str(fileName), cv2.FILE_STORAGE_READ)
-    cameraMatrix    = fs.getNode("cameraMatrix").mat()
-    distCoeff       = fs.getNode("distCoeff").mat()
-    # camera extrinsics for 3D gaze
-    cameraRotation  = fs.getNode("rotation").mat()
-    if cameraRotation is not None:
-        cameraRotation  = cv2.Rodrigues(cameraRotation)[0]  # need rotation vector, not rotation matrix
-    cameraPosition  = fs.getNode("position").mat()
-    fs.release()
+class CameraParams:
+    def __init__(self,
+                 # camera info
+                 resolution: np.ndarray,
+                 # intrinsics
+                 camera_mtx: np.ndarray, distort_coeffs: np.ndarray = None,
+                 # extrinsics
+                 rotation_vec: np.ndarray = None, position: np.ndarray = None):
+
+        self.resolution     : np.ndarray = resolution
+        self.camera_mtx     : np.ndarray = camera_mtx
+        self.distort_coeffs : np.ndarray = distort_coeffs
+        self.rotation_vec   : np.ndarray = rotation_vec
+        self.position       : np.ndarray = position
+
+    @staticmethod
+    def readFromFile(fileName: str|pathlib.Path) -> 'CameraParams':
+        fs = cv2.FileStorage(str(fileName), cv2.FILE_STORAGE_READ)
+        resolution      = fs.getNode("resolution").mat()
+        cameraMatrix    = fs.getNode("cameraMatrix").mat()
+        distCoeff       = fs.getNode("distCoeff").mat()
+        # camera extrinsics for 3D gaze
+        cameraRotation  = fs.getNode("rotation").mat()
+        if cameraRotation is not None:
+            cameraRotation  = cv2.Rodrigues(cameraRotation)[0]  # need rotation vector, not rotation matrix
+        cameraPosition  = fs.getNode("position").mat()
+        fs.release()
 
-    return (cameraMatrix,distCoeff,cameraRotation,cameraPosition)
+        return CameraParams(resolution,cameraMatrix,distCoeff,cameraRotation,cameraPosition)
+
+    def has_intrinsics(self):
+        return (self.camera_mtx is not None) and (self.distort_coeffs is not None)
 
 
 class CV2VideoReader:
     def __init__(self, file: str|pathlib.Path, timestamps: list|np.ndarray|pd.DataFrame):
         self.file = pathlib.Path(file)
         if isinstance(timestamps,list):
             self.ts = np.array(timestamps)
@@ -57,15 +62,15 @@
 
     def get_prop(self, cv2_prop):
         return self.cap.get(cv2_prop)
 
     def set_prop(self, cv2_prop, val):
         return self.cap.set(cv2_prop, val)
 
-    def read_frame(self):
+    def read_frame(self, report_gap=False):
         ts0 = self.cap.get(cv2.CAP_PROP_POS_MSEC)
         ret, frame = self.cap.read()
         ts1 = self.cap.get(cv2.CAP_PROP_POS_MSEC)
         self.frame_idx += 1
 
         # check if this is a stream for which opencv returns timestamps that are one frame off
         if self.frame_idx==0 and ts0==ts1:
@@ -86,14 +91,20 @@
                 tss = self.ts-self._last_good_ts[2]
                 # find best matching frame idx so we catch up with the jump
                 idx = bisect.bisect(tss, t_jump)
                 if abs(tss[idx-1]-t_jump)<abs(tss[idx]-t_jump):
                     idx -= 1
                 self.frame_idx = idx
                 ts_from_list = self.ts[self.frame_idx]
+                if report_gap and self.frame_idx-self._last_good_ts[0]>1:
+                    print(f'Frame discontinuity detected (jumped from {self._last_good_ts[0]} to {self.frame_idx}), there are probably corrupt frames in your video')
             self._last_good_ts = (self.frame_idx, ts1, ts_from_list)
 
         # we might not have a valid frame, but we're not done yet
         if not ret or frame is None:
             return False, None,  self.frame_idx, ts_from_list
         else:
-            return False, frame, self.frame_idx, ts_from_list
+            return False, frame, self.frame_idx, ts_from_list
+
+    def report_frame(self, interval=100):
+        if self.frame_idx%interval==0:
+            print('  frame {}'.format(self.frame_idx))
```

### Comparing `glassestools-0.5.1/src/glassesTools/plane.py` & `glassestools-1.0.0/src/glassesTools/plane.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,119 @@
 import numpy as np
-import pandas as pd
 import cv2
-import math
-from collections import defaultdict
+import pathlib
 
-from . import data_files, transforms, utils
+from . import data_files, ocv
 
 
 class Pose:
+    # description of tsv file used for storage
     _columns_compressed = {'frame_idx':1,
-                           'pose_ok': 1, 'pose_N_markers': 1, 'pose_R_vec': 3, 'pose_T_vec': 3,
+                           'pose_N_markers': 1, 'pose_R_vec': 3, 'pose_T_vec': 3,
                            'homography_N_markers': 1, 'homography_mat': 9}
     _non_float          = {'frame_idx': int, 'pose_ok': bool, 'pose_N_markers': int, 'homography_N_markers': int}
 
     def __init__(self,
-                 frame_idx:int,
-                 pose_ok=False,
-                 pose_N_markers=0,
-                 pose_R_vec:np.ndarray=None,
-                 pose_T_vec:np.ndarray=None,
-                 homography_N_markers=0,
-                 homography_mat:np.ndarray=None):
+                 frame_idx              : int,
+                 pose_N_markers         : int       = 0,
+                 pose_R_vec             : np.ndarray= None,
+                 pose_T_vec             : np.ndarray= None,
+                 homography_N_markers   : int       = 0,
+                 homography_mat         : np.ndarray= None):
         self.frame_idx            : int         = frame_idx
         # pose
-        self.pose_ok              : bool        = pose_ok               # Output of cv2.SolvePnP(), whether successful or not
-        self.pose_N_markers       : int         = pose_N_markers        # number of ArUco markers this pose estimate is based on
+        self.pose_N_markers       : int         = pose_N_markers        # number of ArUco markers this pose estimate is based on. 0 if failed
         self.pose_R_vec           : np.ndarray  = pose_R_vec
         self.pose_T_vec           : np.ndarray  = pose_T_vec
         # homography
-        self.homography_N_markers : int         = homography_N_markers  # number of ArUco markers this homongraphy estimate is based on
+        self.homography_N_markers : int         = homography_N_markers  # number of ArUco markers this homongraphy estimate is based on. 0 if failed
         self.homography_mat       : np.ndarray  = homography_mat.reshape(3,3) if homography_mat is not None else homography_mat
 
         # internals
         self._RMat        = None
         self._RtMat       = None
         self._planeNormal = None
         self._planePoint  = None
         self._RMatInv     = None
         self._RtMatInv    = None
+        self._iH          = None
 
     @staticmethod
-    def readFromFile(fileName,start=None,end=None) -> dict[int,'Pose']:
-        readSubset  = start is not None and end is not None
-        df          = pd.read_csv(str(fileName), delimiter='\t', index_col=False, dtype=defaultdict(lambda: float, **Pose._non_float))
-        if readSubset:
-            df = df[(df['frame_idx'] >= start) & (df['frame_idx'] <= end)]
-
-        # figure out what the data columns are
-        # group columns into numpy arrays, insert None if missing
-        cols = [col for col in Pose._columns_compressed if Pose._columns_compressed[col]>1]
-        allCols = tuple([c for c in df.columns if col in c] for col in cols)
-
-        # drop rows where are all data columns are nan
-        df = df.dropna(how='all',subset=[c for cs in allCols for c in cs])
-
-        # group columns into numpy arrays, insert None if missing
-        for c,ac in zip(cols,allCols):
-            if ac:
-                df[c] = [data_files.noneIfAnyNan(x) for x in df[ac].values]  # make list of numpy arrays, or None if there are any NaNs in the array
-            else:
-                df[c] = None
-
-        # keep only the columns we want (this also puts them in the right order even if that doesn't matter since we use kwargs to construct objects)
-        df = df[Pose._columns_compressed.keys()]
-
-        poses = {idx:Pose(**kwargs) for idx,kwargs in zip(df['frame_idx'].values,df.to_dict(orient='records'))}
-        return poses
+    def readFromFile(fileName:str|pathlib.Path, start:int=None, end:int=None) -> dict[int,'Pose']:
+        return data_files.read_file(fileName,
+                                    Pose, True, True, False,
+                                    start=start, end=end)[0]
 
     @staticmethod
-    def writeToFile(poses: list['Pose'], fileName, skip_failed=False):
-        records = [{k:getattr(p,k) for k in vars(p) if not k.startswith('_')} for p in poses]
-        df = pd.DataFrame.from_records(records)
-
-        # unpack array columns
-        allCols = []
-        for c in Pose._columns_compressed:
-            N = Pose._columns_compressed[c]
-            if N==1:
-                allCols.append([c])
-            elif N==3:
-                allCols.append(data_files.getXYZLabels(c))
-            else:
-                allCols.append(['homography[%d,%d]' % (r,c) for r in range(3) for c in range(3)])
-        for c,ac in zip(Pose._columns_compressed,allCols):
-            if len(ac)>1:
-                df[ac] = np.vstack([data_files.allNanIfNone(v,len(ac)).flatten() for v in df[c].values])
-
-        # keep only columns to be written out and order them correctly
-        df = df[[c for cs in allCols for c in cs]]
-
-        # drop rows where are all data columns are nan
-        if skip_failed:
-            df = df.dropna(how='all', subset=[c for cs in allCols if len(cs)>1 for c in cs])
-
-        df.to_csv(str(fileName), index=False, sep='\t', na_rep='nan', float_format="%.8f")
+    def writeToFile(poses: list['Pose'], fileName:str|pathlib.Path, skip_failed=False):
+        data_files.write_array_to_file(poses, fileName,
+                                       Pose._columns_compressed,
+                                       skip_all_nan=skip_failed)
 
-    def camToWorld(self, point):
+    def camToWorld(self, point: np.ndarray):
         if (self.pose_R_vec is None) or (self.pose_T_vec is None) or np.any(np.isnan(point)):
-            return np.array([np.nan, np.nan, np.nan])
+            return np.full((3,), np.nan)
 
         if self._RtMatInv is None:
             if self._RMatInv is None:
                 if self._RMat is None:
                     self._RMat = cv2.Rodrigues(self.pose_R_vec)[0]
                 self._RMatInv = self._RMat.T
             self._RtMatInv = np.hstack((self._RMatInv,np.matmul(-self._RMatInv,self.pose_T_vec.reshape(3,1))))
 
         return np.matmul(self._RtMatInv,np.append(np.array(point),1.).reshape((4,1))).flatten()
 
-    def worldToCam(self, point):
+    def worldToCam(self, point: np.ndarray):
         if (self.pose_R_vec is None) or (self.pose_T_vec is None) or np.any(np.isnan(point)):
-            return np.array([np.nan, np.nan, np.nan])
+            return np.full((3,), np.nan)
 
         if self._RtMat is None:
             if self._RMat is None:
                 self._RMat = cv2.Rodrigues(self.pose_R_vec)[0]
             self._RtMat = np.hstack((self._RMat, self.pose_T_vec.reshape(3,1)))
 
         return np.matmul(self._RtMat,np.append(np.array(point),1.).reshape((4,1))).flatten()
 
-    def vectorIntersect(self, vector, origin = np.array([0.,0.,0.])):
+    def planeToCamHomography(self, point: np.ndarray, camera_params: ocv.CameraParams) -> np.ndarray:
+        # from location on plane (2D) to location on camera image (2D)
+        from . import transforms
+        if self.homography_mat is None:
+            return np.full((2,), np.nan)
+
+        if self._iH is None:
+            self._iH = np.linalg.inv(self.homography_mat)
+        out = transforms.applyHomography(self._iH, *point)
+        if camera_params.has_intrinsics():
+            out = transforms.distortPoint(*out, camera_params.camera_mtx, camera_params.distort_coeffs)
+        return out
+
+    def camToPlaneHomography(self, point: np.ndarray, camera_params: ocv.CameraParams) -> np.ndarray:
+        # from location on camera image (2D) to location on plane (2D)
+        from . import transforms
+        if self.homography_mat is None:
+            return np.full((2,), np.nan)
+
+        if camera_params.has_intrinsics():
+            point = transforms.undistortPoint(*point, camera_params.camera_mtx, camera_params.distort_coeffs)
+        return transforms.applyHomography(self.homography_mat, *point)
+
+    def getOriginOnImage(self, camera_params: ocv.CameraParams) -> np.ndarray:
+        if self.pose_N_markers>0 and camera_params.has_intrinsics():
+            a = cv2.projectPoints(np.zeros((1,3)), self.pose_R_vec,self.pose_T_vec, camera_params.camera_mtx,camera_params.distort_coeffs)[0].flatten()
+        elif self.homography_N_markers>0:
+            a = self.planeToCamHomography([0., 0.], camera_params.camera_mtx, camera_params.distort_coeffs)
+        else:
+            a = np.full((2,), np.nan)
+        return a
+
+    def vectorIntersect(self, vector: np.ndarray, origin = np.array([0.,0.,0.])):
+        from . import transforms
+
         if (self.pose_R_vec is None) or (self.pose_T_vec is None) or np.any(np.isnan(vector)):
-            return np.array([np.nan, np.nan, np.nan])
+            return np.full((3,), np.nan)
 
         if self._planeNormal is None:
             if self._RtMat is None:
                 if self._RMat is None:
                     self._RMat = cv2.Rodrigues(self.pose_R_vec)[0]
                 self._RtMat = np.hstack((self._RMat, self.pose_T_vec.reshape(3,1)))
```

### Comparing `glassestools-0.5.1/src/glassesTools/recording.py` & `glassestools-1.0.0/src/glassesTools/recording.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/timestamps.py` & `glassestools-1.0.0/src/glassesTools/timestamps.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/transforms.py` & `glassestools-1.0.0/src/glassesTools/transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import math
 import cv2
 
-from . import gaze_headref, gaze_worldref, plane
+from . import gaze_headref, gaze_worldref, marker, ocv, plane
 
 def toNormPos(x,y,bbox):
     # transforms input (x,y) which is on a plane in world units
     # (e.g. mm on an aruco poster) to a normalized position
     # in an image of the plane, given the image's bounding box in
     # world units
     # for input (0,0) is bottom left, for output (0,0) is top left
@@ -25,112 +25,116 @@
     # fractional position between bounding box edges, (0,0) in bottom left
     pos = toNormPos(x,y, bbox)
     # turn into int, add margin
     pos = [p*s+m for p,s,m in zip(pos,imSize,margin)]
     return pos
 
 
-def estimateHomography(known, detectedCorners, detectedIDs):
+def estimateHomographyKnownMarker(known: list[marker.Marker], detectedCorners, detectedIDs):
     # collect matching corners in image and in world
-    pts_src = []
-    pts_dst = []
+    imgP = []
+    objP = []
     detectedIDs = detectedIDs.flatten()
     if len(detectedIDs) != len(detectedCorners):
         raise ValueError('unexpected number of IDs (%d) given number of corner arrays (%d)' % (len(detectedIDs),len(detectedCorners)))
     for i in range(0, len(detectedIDs)):
         if detectedIDs[i] in known:
             dc = detectedCorners[i]
             if dc.shape[0]==1 and dc.shape[1]==4:
                 dc = np.reshape(dc,(4,1,2))
-            pts_src.extend( [x.flatten() for x in dc] )
-            pts_dst.extend( known[detectedIDs[i]].corners )
+            imgP.extend( [x.flatten() for x in dc] )
+            objP.extend( known[detectedIDs[i]].corners )
 
-    if len(pts_src) < 4:
+    if len(imgP) < 4:
         return None, False
 
     # compute Homography
-    pts_src = np.float32(pts_src)
-    pts_dst = np.float32(pts_dst)
-    h, _ = cv2.findHomography(pts_src, pts_dst)
+    return estimateHomography(objP, imgP)
+
+def estimateHomography(objP, imgP):
+    imgP = np.float32(imgP)
+    objP = np.float32(objP)
+    h, _ = cv2.findHomography(imgP, objP)
     return h, True
 
-def applyHomography(h, x, y):
+def applyHomography(H, x, y):
     if math.isnan(x) or math.isnan(y):
-        return np.array([np.nan, np.nan])
+        return np.full((2,), np.nan)
 
     src = np.asarray([x, y], dtype='float32').reshape((1, -1, 2))
-    dst = cv2.perspectiveTransform(src,h)
+    dst = cv2.perspectiveTransform(src,H)
     return dst.flatten()
 
 
 def distortPoint(x, y, cameraMatrix, distCoeff):
     if math.isnan(x) or math.isnan(y):
-        return np.array([np.nan, np.nan])
+        return np.full((2,), np.nan)
 
     # unproject, ignoring distortion as this is an undistored point
     points_2d = np.asarray([x, y], dtype='float32').reshape((1, -1, 2))
     points_2d = cv2.undistortPoints(points_2d, cameraMatrix, np.asarray([[0.0, 0.0, 0.0, 0.0, 0.0]]))
     points_3d = cv2.convertPointsToHomogeneous(points_2d)
     points_3d.shape = -1, 3
 
     # reproject, applying distortion
     points_2d, _ = cv2.projectPoints(points_3d, np.zeros((1, 1, 3)), np.zeros((1, 1, 3)), cameraMatrix, distCoeff)
     return points_2d.flatten()
 
 def undistortPoint(x, y, cameraMatrix, distCoeff):
     if math.isnan(x) or math.isnan(y):
-        return np.array([np.nan, np.nan])
+        return np.full((2,), np.nan)
 
     points_2d = np.asarray([x, y], dtype='float32').reshape((1, -1, 2))
     points_2d = cv2.undistortPoints(points_2d, cameraMatrix, distCoeff, P=cameraMatrix) # P=cameraMatrix to reproject to camera
     return points_2d.flatten()
 
 def unprojectPoint(x, y, cameraMatrix, distCoeff):
     if math.isnan(x) or math.isnan(y):
-        return np.array([np.nan, np.nan, np.nan])
+        return np.full((3,), np.nan)
 
     points_2d = np.asarray([x, y], dtype='float32').reshape((1, -1, 2))
     points_2d = cv2.undistortPoints(points_2d, cameraMatrix, distCoeff)
     points_3d = cv2.convertPointsToHomogeneous(points_2d)
     points_3d.shape = -1, 3
     return points_3d.flatten()
 
 
 def intersect_plane_ray(planeNormal, planePoint, rayDirection, rayPoint, epsilon=1e-6):
     # from https://rosettacode.org/wiki/Find_the_intersection_of_a_line_with_a_plane#Python
 
     ndotu = planeNormal.dot(rayDirection)
     if abs(ndotu) < epsilon:
         # raise RuntimeError("no intersection or line is within plane")
-        np.array([np.nan, np.nan, np.nan])
+        return np.full((3,), np.nan)
 
     w = rayPoint - planePoint
     si = -planeNormal.dot(w) / ndotu
     return w + si * rayDirection + planePoint
 
 
 def angle_between(v1, v2):
     return (180.0 / math.pi) * math.atan2(np.linalg.norm(np.cross(v1,v2)), np.dot(v1,v2))
 
 
-def gazeToPlane(gaze: gaze_headref.Gaze, pose: plane.Pose, cameraRotation,cameraPosition, cameraMatrix=None, distCoeffs=None) -> gaze_worldref.Gaze:
-    hasCameraPose = (pose.pose_R_vec is not None) and (pose.pose_T_vec is not None)
+def gazeToPlane(gaze: gaze_headref.Gaze, pose: plane.Pose, cameraParams: ocv.CameraParams) -> gaze_worldref.Gaze:
     gazeWorld     = gaze_worldref.Gaze(gaze.timestamp, gaze.frame_idx)
-    if hasCameraPose:
+    if pose.pose_N_markers>0:
         # get transform from ET data's coordinate frame to camera's coordinate frame
+        cameraRotation = cameraParams.rotation_vec
+        cameraPosition = cameraParams.position
         if cameraRotation is None:
             cameraRotation = np.zeros((3,1))
         RCam  = cv2.Rodrigues(cameraRotation)[0]
         if cameraPosition is None:
             cameraPosition = np.zeros((3,1))
         RtCam = np.hstack((RCam, cameraPosition))
 
         # project gaze on video to reference poster using camera pose
         # turn observed gaze position on video into position on tangent plane
-        g3D = unprojectPoint(gaze.gaze_pos_vid[0],gaze.gaze_pos_vid[1], cameraMatrix, distCoeffs)
+        g3D = unprojectPoint(*gaze.gaze_pos_vid, cameraParams.camera_mtx, cameraParams.distort_coeffs)
 
         # find intersection of 3D gaze with poster
         gazeWorld.gazePosCam_vidPos_ray = pose.vectorIntersect(g3D)  # default vec origin (0,0,0) because we use g3D from camera's view point
 
         # above intersection is in camera space, turn into poster space to get position on poster
         (x,y,z) = pose.camToWorld(gazeWorld.gazePosCam_vidPos_ray) # z should be very close to zero
         gazeWorld.gazePosPlane2D_vidPos_ray = np.asarray([x, y])
@@ -147,27 +151,23 @@
             (x,y,z) = pose.camToWorld(gazeWorld.gazePosCamWorld)   # z should be very close to zero
             gazeWorld.gazePosPlane2DWorld = np.asarray([x, y])
 
     # unproject 2D gaze point on video to point on poster (should yield values very close to
     # the above method of intersecting video gaze point ray with poster, and usually also very
     # close to binocular gaze point (though for at least one tracker the latter is not the case;
     # the AdHawk has an optional parallax correction using a vergence signal))
-    if pose.homography_mat is not None:
-        ux, uy = gaze.gaze_pos_vid
-        if (cameraMatrix is not None) and (distCoeffs is not None):
-            ux, uy = undistortPoint( ux, uy, cameraMatrix, distCoeffs)
-        (xW, yW) = applyHomography(pose.homography_mat, ux, uy)
-        gazeWorld.gazePosPlane2D_vidPos_homography = np.asarray([xW, yW])
+    if pose.homography_N_markers>0:
+        gazeWorld.gazePosPlane2D_vidPos_homography = pose.camToPlaneHomography(gaze.gaze_pos_vid, cameraParams)
 
         # get this point in camera space
-        if hasCameraPose:
-            gazeWorld.gazePosCam_vidPos_homography = pose.worldToCam(np.array([xW,yW,0.]))
+        if pose.pose_N_markers>0:
+            gazeWorld.gazePosCam_vidPos_homography = pose.worldToCam(np.append(gazeWorld.gazePosPlane2D_vidPos_homography, 0))
 
     # project gaze vectors to reference poster (and draw on video)
-    if not hasCameraPose:
+    if not pose.pose_N_markers>0:
         # nothing to do anymore
         return gazeWorld
 
     gazeVecs    = [gaze.gaze_dir_l, gaze.gaze_dir_r]
     gazeOrigins = [gaze.gaze_ori_l, gaze.gaze_ori_r]
     attrs       = [['gazeOriCamLeft','gazePosCamLeft','gazePosPlane2DLeft'],['gazeOriCamRight','gazePosCamRight','gazePosPlane2DRight']]
     for gVec,gOri,attr in zip(gazeVecs,gazeOrigins,attrs):
```

### Comparing `glassestools-0.5.1/src/glassesTools/utils.py` & `glassestools-1.0.0/src/glassesTools/utils.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools/video_utils.py` & `glassestools-1.0.0/src/glassesTools/video_utils.py`

 * *Files identical despite different names*

### Comparing `glassestools-0.5.1/src/glassesTools.egg-info/PKG-INFO` & `glassestools-1.0.0/src/glassesTools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassesTools
-Version: 0.5.1
+Version: 1.0.0
 Summary: Tools for processing wearable eye tracker recordings.
 Home-page: https://github.com/dcnieho/glassesTools
 Author: Diederick Niehorster
 Author-email: diederick_c.niehorster@humlab.lu.se
 License: MIT License
         
         Copyright (c) 2022-2023 Diederick Niehorster
@@ -42,13 +42,13 @@
 Requires-Dist: ffpyplayer
 Requires-Dist: scipy==1.11.3
 
 [![Downloads](https://static.pepy.tech/badge/glassestools)](https://pepy.tech/project/glassestools)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/glassesTools.svg)](https://pypi.org/project/glassesTools/)
 [![image](https://img.shields.io/pypi/pyversions/glassesTools.svg)](https://pypi.org/project/glassesTools/)
 
-# GlassesTools v0.5.1
+# GlassesTools v1.0.0
 Tools for processing wearable eye tracker recordings.
 
 If you use this package or any of the code in this repository, please cite:<br>
 [Niehorster, D.C., Hessels, R.S., Benjamins, J.S., Nyström, M. and Hooge, I.T.C. (2023). GlassesValidator:
 A data quality tool for eye tracking glasses. Behavior Research Methods. doi: 10.3758/s13428-023-02105-5](https://doi.org/10.3758/s13428-023-02105-5)
```

### Comparing `glassestools-0.5.1/src/glassesTools.egg-info/SOURCES.txt` & `glassestools-1.0.0/src/glassesTools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 src/glassesTools/__init__.py
+src/glassesTools/aruco.py
 src/glassesTools/data_files.py
 src/glassesTools/drawing.py
 src/glassesTools/eyetracker.py
 src/glassesTools/gaze_headref.py
 src/glassesTools/gaze_worldref.py
+src/glassesTools/intervals.py
 src/glassesTools/marker.py
 src/glassesTools/ocv.py
 src/glassesTools/plane.py
 src/glassesTools/recording.py
 src/glassesTools/timestamps.py
 src/glassesTools/transforms.py
 src/glassesTools/utils.py
```

