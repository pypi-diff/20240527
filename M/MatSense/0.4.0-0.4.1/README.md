# Comparing `tmp/MatSense-0.4.0.tar.gz` & `tmp/matsense-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/atomie/Seafile/SYNC/Coding/MatSense/dist/tmp_6aavuuu/MatSense-0.4.0.tar", last modified: Fri Jan 28 11:39:14 2022, max compression
+gzip compressed data, was "matsense-0.4.1.tar", last modified: Mon May 27 13:36:47 2024, max compression
```

## Comparing `MatSense-0.4.0.tar` & `matsense-0.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 atomie     (501) staff       (20)        0 2022-01-28 11:39:14.000000 MatSense-0.4.0/
-drwxr-xr-x   0 atomie     (501) staff       (20)        0 2022-01-28 11:39:14.000000 MatSense-0.4.0/MatSense.egg-info/
--rw-r--r--   0 atomie     (501) staff       (20)     9516 2022-01-28 11:39:14.000000 MatSense-0.4.0/MatSense.egg-info/PKG-INFO
--rw-r--r--   0 atomie     (501) staff       (20)      972 2022-01-28 11:39:14.000000 MatSense-0.4.0/MatSense.egg-info/SOURCES.txt
--rw-r--r--   0 atomie     (501) staff       (20)        1 2022-01-28 11:39:14.000000 MatSense-0.4.0/MatSense.egg-info/dependency_links.txt
--rw-r--r--   0 atomie     (501) staff       (20)      114 2022-01-28 11:39:14.000000 MatSense-0.4.0/MatSense.egg-info/entry_points.txt
--rw-r--r--   0 atomie     (501) staff       (20)      287 2022-01-28 11:39:14.000000 MatSense-0.4.0/MatSense.egg-info/requires.txt
--rw-r--r--   0 atomie     (501) staff       (20)        9 2022-01-28 11:39:14.000000 MatSense-0.4.0/MatSense.egg-info/top_level.txt
--rw-r--r--   0 atomie     (501) staff       (20)     9516 2022-01-28 11:39:14.000000 MatSense-0.4.0/PKG-INFO
--rw-r--r--   0 atomie     (501) staff       (20)     8806 2022-01-28 11:36:50.000000 MatSense-0.4.0/README.md
-drwxr-xr-x   0 atomie     (501) staff       (20)        0 2022-01-28 11:39:14.000000 MatSense-0.4.0/matsense/
--rw-r--r--   0 atomie     (501) staff       (20)        0 2022-01-13 11:31:55.000000 MatSense-0.4.0/matsense/__init__.py
--rw-r--r--   0 atomie     (501) staff       (20)     3669 2022-01-28 11:35:55.000000 MatSense-0.4.0/matsense/blank_template.yaml
--rw-r--r--   0 atomie     (501) staff       (20)    10302 2022-01-13 12:40:12.000000 MatSense-0.4.0/matsense/client.py
--rw-r--r--   0 atomie     (501) staff       (20)      751 2022-01-13 12:40:12.000000 MatSense-0.4.0/matsense/cmd.py
--rw-r--r--   0 atomie     (501) staff       (20)     6225 2022-01-28 11:05:07.000000 MatSense-0.4.0/matsense/data.py
--rw-r--r--   0 atomie     (501) staff       (20)     4381 2022-01-27 20:18:15.000000 MatSense-0.4.0/matsense/datasetter.py
--rw-r--r--   0 atomie     (501) staff       (20)      314 2022-01-27 20:17:20.000000 MatSense-0.4.0/matsense/exception.py
--rw-r--r--   0 atomie     (501) staff       (20)     2895 2022-01-27 19:38:15.000000 MatSense-0.4.0/matsense/filemanager.py
-drwxr-xr-x   0 atomie     (501) staff       (20)        0 2022-01-28 11:39:14.000000 MatSense-0.4.0/matsense/process/
--rw-r--r--   0 atomie     (501) staff       (20)      274 2022-01-27 20:13:36.000000 MatSense-0.4.0/matsense/process/__init__.py
--rw-r--r--   0 atomie     (501) staff       (20)     7766 2021-12-22 08:39:59.000000 MatSense-0.4.0/matsense/process/blob_parser.py
--rw-r--r--   0 atomie     (501) staff       (20)    10571 2022-01-28 04:21:58.000000 MatSense-0.4.0/matsense/process/data_handler.py
--rw-r--r--   0 atomie     (501) staff       (20)     1815 2021-12-22 08:39:59.000000 MatSense-0.4.0/matsense/process/interpolator.py
--rw-r--r--   0 atomie     (501) staff       (20)     5576 2020-10-30 06:18:16.000000 MatSense-0.4.0/matsense/process/point_tool.py
--rw-r--r--   0 atomie     (501) staff       (20)     2381 2020-05-15 05:35:58.000000 MatSense-0.4.0/matsense/process/pressure_selector.py
--rw-r--r--   0 atomie     (501) staff       (20)     3266 2022-01-28 04:12:28.000000 MatSense-0.4.0/matsense/process/processor.py
--rw-r--r--   0 atomie     (501) staff       (20)    12987 2022-01-27 20:21:26.000000 MatSense-0.4.0/matsense/server.py
-drwxr-xr-x   0 atomie     (501) staff       (20)        0 2022-01-28 11:39:14.000000 MatSense-0.4.0/matsense/serverkit/
--rw-r--r--   0 atomie     (501) staff       (20)       75 2022-01-27 20:18:31.000000 MatSense-0.4.0/matsense/serverkit/__init__.py
--rw-r--r--   0 atomie     (501) staff       (20)      275 2022-01-13 12:40:12.000000 MatSense-0.4.0/matsense/serverkit/flag.py
--rw-r--r--   0 atomie     (501) staff       (20)     5313 2022-01-27 20:18:39.000000 MatSense-0.4.0/matsense/serverkit/proc.py
--rw-r--r--   0 atomie     (501) staff       (20)     6723 2022-01-13 12:40:12.000000 MatSense-0.4.0/matsense/serverkit/userver.py
--rw-r--r--   0 atomie     (501) staff       (20)     8373 2022-01-28 09:11:23.000000 MatSense-0.4.0/matsense/tools.py
--rw-r--r--   0 atomie     (501) staff       (20)     9494 2022-01-13 12:40:12.000000 MatSense-0.4.0/matsense/uclient.py
-drwxr-xr-x   0 atomie     (501) staff       (20)        0 2022-01-28 11:39:14.000000 MatSense-0.4.0/matsense/visual/
--rw-r--r--   0 atomie     (501) staff       (20)       45 2020-04-30 04:26:10.000000 MatSense-0.4.0/matsense/visual/__init__.py
--rw-r--r--   0 atomie     (501) staff       (20)     8686 2021-12-22 08:39:59.000000 MatSense-0.4.0/matsense/visual/player.py
--rw-r--r--   0 atomie     (501) staff       (20)     3265 2021-12-22 08:39:59.000000 MatSense-0.4.0/matsense/visual/player1d.py
--rw-r--r--   0 atomie     (501) staff       (20)     6706 2021-12-22 08:39:59.000000 MatSense-0.4.0/matsense/visual/player_matplot.py
--rw-r--r--   0 atomie     (501) staff       (20)    13622 2021-12-22 08:39:59.000000 MatSense-0.4.0/matsense/visual/player_pyqtgraph.py
--rw-r--r--   0 atomie     (501) staff       (20)      534 2021-12-22 08:39:59.000000 MatSense-0.4.0/matsense/visual/util.py
--rw-r--r--   0 atomie     (501) staff       (20)      104 2021-12-27 06:38:37.000000 MatSense-0.4.0/pyproject.toml
--rw-r--r--   0 atomie     (501) staff       (20)       38 2022-01-28 11:39:14.000000 MatSense-0.4.0/setup.cfg
--rw-r--r--   0 atomie     (501) staff       (20)     8959 2022-01-27 20:26:03.000000 MatSense-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:47.573404 matsense-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:47.569404 matsense-0.4.1/MatSense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-27 13:36:47.000000 matsense-0.4.1/MatSense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-27 13:36:47.000000 matsense-0.4.1/MatSense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:36:47.000000 matsense-0.4.1/MatSense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-27 13:36:47.000000 matsense-0.4.1/MatSense.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-27 13:36:47.000000 matsense-0.4.1/MatSense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 13:36:47.000000 matsense-0.4.1/MatSense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-27 13:36:47.573404 matsense-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-27 13:36:43.000000 matsense-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:47.569404 matsense-0.4.1/matsense/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/blank_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/datasetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/filemanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:47.569404 matsense-0.4.1/matsense/process/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/process/blob_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14991 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/process/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/process/interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/process/point_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/process/pressure_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/process/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:47.569404 matsense-0.4.1/matsense/serverkit/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/serverkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/serverkit/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/serverkit/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/serverkit/userver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/uclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:36:47.569404 matsense-0.4.1/matsense/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/visual/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/visual/player1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/visual/player_matplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/visual/player_pyqtgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-27 13:36:43.000000 matsense-0.4.1/matsense/visual/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-27 13:36:43.000000 matsense-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:36:47.573404 matsense-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-05-27 13:36:43.000000 matsense-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MatSense-0.4.0/MatSense.egg-info/PKG-INFO` & `matsense-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: MatSense
-Version: 0.4.0
-Summary: A toolkit for matrix sensor data processing 阵列传感器数据处理工具库
-Home-page: https://github.com/atomiechen/MatSense
-Author: Atomie CHEN
-Author-email: atomic_cwh@163.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/atomiechen/MatSense/issues
-Project-URL: Source Code, https://github.com/atomiechen/MatSense
-Keywords: matrix sensor,signal processing,3D visualization
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-Provides-Extra: pyqtgraph
-
 # MatSense
 
 [![PyPi](https://img.shields.io/pypi/v/matsense.svg)](https://pypi.org/project/MatSense/)
 
 A toolkit that supports both real-time and off-line matrix sensor data processing and 3D visualization. 
 
 ![schematic](https://raw.githubusercontent.com/atomiechen/MatSense/main/img/schematic.drawio.svg)
@@ -292,9 +273,7 @@
 
 
 
 ## Author
 
 Atomie CHEN: atomic_cwh@163.com
 
-
-
```

### Comparing `MatSense-0.4.0/MatSense.egg-info/SOURCES.txt` & `matsense-0.4.1/MatSense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/PKG-INFO` & `matsense-0.4.1/MatSense.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: MatSense
-Version: 0.4.0
+Version: 0.4.1
 Summary: A toolkit for matrix sensor data processing 阵列传感器数据处理工具库
 Home-page: https://github.com/atomiechen/MatSense
 Author: Atomie CHEN
 Author-email: atomic_cwh@163.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/atomiechen/MatSense/issues
 Project-URL: Source Code, https://github.com/atomiechen/MatSense
 Keywords: matrix sensor,signal processing,3D visualization
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.19.2
+Requires-Dist: scipy>=1.5.4
+Requires-Dist: pyserial>=3.5
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: pyparsing>=2.4.7
+Requires-Dist: matplotlib<=3.4,>=3.3
 Provides-Extra: pyqtgraph
+Requires-Dist: pyqtgraph==0.11.*; extra == "pyqtgraph"
+Requires-Dist: PyOpenGL~=3.1.5; extra == "pyqtgraph"
+Requires-Dist: PyQt5==5.12.*; python_version == "3.7" and extra == "pyqtgraph"
+Requires-Dist: PyQt5==5.15.*; python_version == "3.8" and extra == "pyqtgraph"
+Requires-Dist: PyQt6==6.0.*; python_version == "3.9" and extra == "pyqtgraph"
 
 # MatSense
 
 [![PyPi](https://img.shields.io/pypi/v/matsense.svg)](https://pypi.org/project/MatSense/)
 
 A toolkit that supports both real-time and off-line matrix sensor data processing and 3D visualization. 
 
@@ -292,9 +301,7 @@
 
 
 
 ## Author
 
 Atomie CHEN: atomic_cwh@163.com
 
-
-
```

### Comparing `MatSense-0.4.0/README.md` & `matsense-0.4.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: MatSense
+Version: 0.4.1
+Summary: A toolkit for matrix sensor data processing 阵列传感器数据处理工具库
+Home-page: https://github.com/atomiechen/MatSense
+Author: Atomie CHEN
+Author-email: atomic_cwh@163.com
+Project-URL: Bug Tracker, https://github.com/atomiechen/MatSense/issues
+Project-URL: Source Code, https://github.com/atomiechen/MatSense
+Keywords: matrix sensor,signal processing,3D visualization
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.19.2
+Requires-Dist: scipy>=1.5.4
+Requires-Dist: pyserial>=3.5
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: pyparsing>=2.4.7
+Requires-Dist: matplotlib<=3.4,>=3.3
+Provides-Extra: pyqtgraph
+Requires-Dist: pyqtgraph==0.11.*; extra == "pyqtgraph"
+Requires-Dist: PyOpenGL~=3.1.5; extra == "pyqtgraph"
+Requires-Dist: PyQt5==5.12.*; python_version == "3.7" and extra == "pyqtgraph"
+Requires-Dist: PyQt5==5.15.*; python_version == "3.8" and extra == "pyqtgraph"
+Requires-Dist: PyQt6==6.0.*; python_version == "3.9" and extra == "pyqtgraph"
+
 # MatSense
 
 [![PyPi](https://img.shields.io/pypi/v/matsense.svg)](https://pypi.org/project/MatSense/)
 
 A toolkit that supports both real-time and off-line matrix sensor data processing and 3D visualization. 
 
 ![schematic](https://raw.githubusercontent.com/atomiechen/MatSense/main/img/schematic.drawio.svg)
```

### Comparing `MatSense-0.4.0/matsense/blank_template.yaml` & `matsense-0.4.1/matsense/blank_template.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,18 @@
   ### voltage to the reciprocal of resistance
   ## reference voltage: 255, 255/3.6*3.3
   V0: ~
   ## constant factor: 1
   R0_RECI: ~
   ## convert voltage to resistance: true
   convert: ~
-
+  ## convert voltage to resistance's opposite number (otherwise reciprocal): false
+  resi_opposite: ~
+  ## convert voltage to delta_R / R0: true
+  resi_delta: ~
   ### server data processing
   ## no filtering and calibration
   raw: ~
   ## time of warming up in seconds: 1
   warm_up: ~
   ## spatial filter: none, ideal, butterworth, gaussian
   filter_spatial: ~
@@ -95,14 +98,18 @@
   filter_temporal_size: ~
   ## rectangular window filter cut-off frequency: 0.04
   rw_cutoff: ~
   ## calibrative frames, 0 for no calibration: 0, 200
   cali_frames: ~
   ## calibration frame window size, 0 for static and >0 for dynamic: 0, 10000
   cali_win_size: ~
+  ## calibration threshold, max data above it maintain, others add to cali_win
+  cali_threshold: 2
+  ## calibration buffer size: 5
+  cali_win_buffer_size: 5
   ## intermediate result: 0, 1, 2
     ## 0: convert voltage to reciprocal resistance
     ## 1: convert & spatial filter
     ## 2: convert & spatial filter & temporal filter
   intermediate: ~
 
   ### (optional) client data processing
```

### Comparing `MatSense-0.4.0/matsense/client.py` & `matsense-0.4.1/matsense/client.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/cmd.py` & `matsense-0.4.1/matsense/cmd.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/data.py` & `matsense-0.4.1/matsense/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,23 +86,27 @@
 
 		my_handler = DataHandlerPressure(
 			n=config['sensor']['shape'],
 			raw=config['process']['raw'],
 			V0=config['process']['V0'],
 			R0_RECI=config['process']['R0_RECI'],
 			convert=config['process']['convert'],
+			resi_opposite=config['process']['resi_opposite'],
+			resi_delta=config['process']['resi_delta'],
 			mask=config['sensor']['mask'],
 			filter_spatial=config['process']['filter_spatial'],
 			filter_spatial_cutoff=config['process']['filter_spatial_cutoff'],
 			butterworth_order=config['process']['butterworth_order'],
 			filter_temporal=config['process']['filter_temporal'],
 			filter_temporal_size=config['process']['filter_temporal_size'],
 			rw_cutoff=config['process']['rw_cutoff'],
 			cali_frames=config['process']['cali_frames'],
 			cali_win_size=config['process']['cali_win_size'],
+            cali_threshold=config['process']['cali_threshold'],
+            cali_win_buffer_size=config['process']['cali_win_buffer_size'],
 			intermediate=config['process']['intermediate'],
 		)
 		my_processor = Processor(
 			config['process']['interp'], 
 			blob=config['process']['blob'], 
 			threshold=config['process']['threshold'],
 			order=config['process']['interp_order'],
```

### Comparing `MatSense-0.4.0/matsense/datasetter.py` & `matsense-0.4.1/matsense/datasetter.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/filemanager.py` & `matsense-0.4.1/matsense/filemanager.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/process/blob_parser.py` & `matsense-0.4.1/matsense/process/blob_parser.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/process/data_handler.py` & `matsense-0.4.1/matsense/process/data_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from math import exp, hypot, pi, sin
 import numpy as np
-
+from collections import deque
 from ..tools import check_shape
 
 
 class FILTER_SPATIAL(Enum):
 	NONE = "none"  # no spatial filter
 	IDEAL = "ideal"  # ideal kernel
 	BUTTERWORTH = "butterworth"  # butterworth kernel
@@ -40,24 +40,29 @@
 
 	## default filters
 	my_filter_spatial = FILTER_SPATIAL.GAUSSIAN
 	my_filter_temporal = FILTER_TEMPORAL.RW
 
 	## voltage-resistance conversion
 	my_convert = True
+	my_resi_opposite = True
+	my_resi_delta = True # count pressure as delta_R / R0
 	V0 = 255
 	R0_RECI = 1  ## a constant to multiply the value
+	R0_START = 0 ## start resistance
 
 	## process parameters
 	my_SF_D0 = 3.5
 	my_BUTTER_ORDER = 2
 	my_LP_SIZE = 15
 	my_LP_W = 0.04
 	my_INIT_CALI_FRAMES = 200
 	my_WIN_SIZE = 0
+	my_WIN_BUFFER_SIZE = 5
+	my_CALI_THRESHOLD = 3
 
 	def __init__(self, **kwargs):
 		self.mask = None
 
 		## output intermediate result
 		## 0: convert voltage to reciprocal resistance
 		## 1: convert & spatial filter
@@ -68,30 +73,35 @@
 		self.config(**kwargs)
 		self.print_proc()
 
 	def config(self, *, n, raw=None, V0=None, R0_RECI=None, convert=None, 
 		mask=None, filter_spatial=None, filter_spatial_cutoff=None, 
 		butterworth_order=None, filter_temporal=None, 
 		filter_temporal_size=None, rw_cutoff=None, cali_frames=None, 
-		cali_win_size=None, 
-		intermediate=None,
+		cali_win_size=None, cali_win_buffer_size=None,
+		intermediate=None, 
+		resi_opposite=None, resi_delta=None, cali_threshold=None,
 		**kwargs):
 
 		self.n = check_shape(n)
 		self.total = self.n[0] * self.n[1]
 		self.cols = self.n[1]//2 + 1
 
 		if raw is not None:
 			self.my_raw = raw
 		if V0:
 			self.V0 = V0
 		if R0_RECI:
 			self.R0_RECI = R0_RECI
 		if convert is not None:
 			self.my_convert = convert
+		if resi_opposite is not None:
+			self.my_resi_opposite = resi_opposite
+		if resi_delta is not None:
+			self.my_resi_delta = resi_delta
 		if mask is not None:
 			self.mask = mask
 		if filter_spatial is not None:
 			try:
 				self.my_filter_spatial = FILTER_SPATIAL(filter_spatial)
 			except:
 				print(f"Invalid spatial filter: '{filter_spatial}'! Use {self.my_filter_spatial.value} instead.")
@@ -110,71 +120,102 @@
 			self.my_LP_W = rw_cutoff
 		if cali_frames is not None:
 			self.my_INIT_CALI_FRAMES = cali_frames
 		if cali_win_size is not None:
 			self.my_WIN_SIZE = cali_win_size
 		if intermediate is not None:
 			self.intermediate = intermediate
+		if cali_threshold is not None:
+			self.my_CALI_THRESHOLD = cali_threshold
+		if cali_win_buffer_size is not None:
+			self.my_WIN_BUFFER_SIZE = cali_win_buffer_size
 
 	@staticmethod
 	def calReciprocalResistance(voltage, v0, r0_reci):
 		if v0 - voltage <= 0:
 			return 0
 		return r0_reci * voltage / (v0 - voltage)
 
 	@staticmethod
 	def calReci_numpy_array(np_array, v0, r0_reci):
 		np_array[np_array >= v0] = 0
 		np_array /= (v0 - np_array)
 		np_array *= r0_reci
 
 	@staticmethod
+	def calOppo_numpy_array(np_array, v0, r0_reci):
+		np_array[np_array >= v0] = 0
+		np_array /= (v0 - np_array)
+		np_array *= r0_reci
+		np_array[np_array != 0] = -1 / np_array[np_array != 0]
+
+	@staticmethod
 	def getNextIndex(idx, size):
 		return (idx+1) if idx != (size-1) else 0
 
+	def calDelta_numpy_array(self, np_array, v0, r0_reci):
+		np_array[np_array >= v0] = 0
+		np_array /= (v0 - np_array)
+		np_array *= r0_reci
+		np_array[np_array != 0] = 1 / np_array[np_array != 0]
+		# print(np_array)
+		np_array[np_array!=0] = abs(np_array[np_array!=0] - self.R0_START[np_array!=0]) / self.R0_START[np_array!=0]
+		np_array *= 10
+		# print(np_array)
+
 	def handle_raw_frame(self, data):
 		self.data_tmp = data
 		self.data_reshape = self.data_tmp.reshape(self.n[0], self.n[1])
 		if self.mask is not None:
 			self.data_reshape *= self.mask
 		if self.my_convert:
 			# for i in range(self.total):
 			# 	self.data_tmp[i] = self.calReciprocalResistance(self.data_tmp[i], self.V0, self.R0_RECI)
-			self.calReci_numpy_array(self.data_tmp, self.V0, self.R0_RECI)
+			if self.my_resi_opposite:
+				self.calOppo_numpy_array(self.data_tmp, self.V0, self.R0_RECI)
+			elif self.my_resi_delta:
+				self.calDelta_numpy_array(self.data_tmp, self.V0, self.R0_RECI)
+			else:
+				self.calReci_numpy_array(self.data_tmp, self.V0, self.R0_RECI)
 
 	def prepare(self, generator):
 		self.generator = generator
 		if not self.my_raw:
+			self.cal_start_R0() # called if my_resi_delta is True
 			self.prepare_spatial()
 			self.prepare_temporal()
-			self.prepare_cali()
+			self.prepare_cali() # called if my_INIT_CALI_FRAMES > 0 and my_resi_delta is False
 
 	def handle(self, data, data_inter=None):
 		self.handle_raw_frame(data)
 		self.data_inter = data_inter
 
 		## output intermediate result
 		if self.data_inter is not None and self.intermediate == 0:
 			self.data_inter[:] = self.data_tmp[:]
 
 		if not self.my_raw:
 			self.filter()
-			self.calibrate()
+			if not self.my_resi_delta:
+				self.calibrate()
 		elif self.data_inter is not None and self.intermediate != 0:
 			## output intermediate result, making data_inter not blank
 			self.data_inter[:] = self.data_tmp[:]
 
 	def prepare_cali(self):
-		if self.my_INIT_CALI_FRAMES <= 0:
+		if self.my_INIT_CALI_FRAMES <= 0 or self.my_resi_delta:
 			return
 
 		print("Initiating calibration...")
 		self.data_zero = np.zeros(self.total, dtype=float)
 		self.data_win = np.zeros((self.my_WIN_SIZE, self.total), dtype=float)
 		self.win_frame_idx = 0
+		self.data_win_buffer = deque(maxlen=self.my_WIN_BUFFER_SIZE)
+		self.win_buffer_frame_idx = 0
+		self.need_to_clean_buffer = False # if True then clean the buffer at next full time
 		## for preparing calibration
 		frame_cnt = 0
 		# ## accumulate data
 		while frame_cnt < self.my_INIT_CALI_FRAMES:
 			# self.get_raw_frame()
 			data = next(self.generator)
 			self.handle_raw_frame(data)
@@ -182,30 +223,78 @@
 			self.filter()
 			self.data_zero += self.data_tmp
 			frame_cnt += 1
 		## get average
 		self.data_zero /= frame_cnt
 		## calculate data_win
 		self.data_win[:] = self.data_zero
+		for _ in range(self.my_WIN_BUFFER_SIZE):
+			self.data_win_buffer.append(self.data_zero)
+        ## save data_min in last WIN_SIZE frames
+		# self.data_min = deque(maxlen=self.my_WIN_SIZE)
+		# self.data_min.append((self.data_zero.copy(), self.win_frame_idx))
+		self.win_frame_idx = self.getNextIndex(self.win_frame_idx, self.my_WIN_SIZE)
+		self.win_buffer_frame_idx = self.getNextIndex(self.win_buffer_frame_idx, self.my_WIN_BUFFER_SIZE)
 
 	def calibrate(self):
 		if self.my_INIT_CALI_FRAMES <= 0:
 			return
 		stored = self.data_tmp.copy()
 		## calibrate
 		self.data_tmp -= self.data_zero
 		## the value should be positive
 		self.data_tmp[self.data_tmp < 0] = 0
 		## adjust window if using dynamic window
 		if self.my_WIN_SIZE > 0:
 			## update data_zero (zero position) and data_win (history data)
-			self.data_zero += (stored - self.data_win[self.win_frame_idx]) / self.my_WIN_SIZE
-			self.data_win[self.win_frame_idx] = stored
-			## update frame index
-			self.win_frame_idx = self.getNextIndex(self.win_frame_idx, self.my_WIN_SIZE)
+
+			## use average number as data_zero
+			# self.data_zero += (stored - self.data_win[self.win_frame_idx]) / self.my_WIN_SIZE
+
+			## use min number as data_zero
+			# if (self.data_min[0][1] == self.win_frame_idx):
+			# 	self.data_min.popleft()
+			# self.data_zero = self.data_min[0][0]
+			# while (self.data_min[-1][0].sum() > stored.sum()):
+			# 	self.data_min.pop()
+			# 	if (len(self.data_min) == 0):
+			# 		break
+			# self.data_min.append((stored, self.win_frame_idx))
+
+			## use average number as data_zero, but delete the odd ones
+			add_to_data_zero = True
+			for id, stored_data in enumerate(stored):
+				data_at_one_point = stored_data - self.data_zero[id]
+				if (data_at_one_point > self.my_CALI_THRESHOLD):
+					# pressure over data_zero + threshold
+					add_to_data_zero = False
+					self.need_to_clean_buffer = True
+					if len(self.data_win_buffer) == self.my_WIN_BUFFER_SIZE:
+						self.data_win_buffer.clear()
+					break
+			if (add_to_data_zero):
+				if len(self.data_win_buffer) < self.my_WIN_BUFFER_SIZE:
+					self.data_win_buffer.append(stored)
+				else:
+					if self.need_to_clean_buffer:
+						self.data_win_buffer.clear()
+						self.need_to_clean_buffer = False
+						self.data_win_buffer.append(stored)
+					else:
+						cur_data = self.data_win_buffer.popleft()
+						self.data_win_buffer.append(stored)
+						## store in data_win
+						self.data_zero += (cur_data - self.data_win[self.win_frame_idx]) / self.my_WIN_SIZE
+						self.data_win[self.win_frame_idx] = cur_data
+						self.win_frame_idx = self.getNextIndex(self.win_frame_idx, self.my_WIN_SIZE)
+
+			# ## store in data_win
+			# self.data_win[self.win_frame_idx] = stored
+			# ## update frame index
+			# self.win_frame_idx = self.getNextIndex(self.win_frame_idx, self.my_WIN_SIZE)
 
 	def filter(self):
 		self.spatial_filter()
 		## output intermediate result
 		if self.data_inter is not None and self.intermediate == 1:
 			self.data_inter[:] = self.data_tmp[:]
 
@@ -263,14 +352,34 @@
 		for t in range(1, self.my_LP_SIZE):
 			self.data_tmp += self.data_filter[self.filter_frame_idx] * self.kernel_lp[t]
 			self.filter_frame_idx = self.getNextIndex(self.filter_frame_idx, self.my_LP_SIZE-1)
 		self.data_filter[self.filter_frame_idx] = stored
 		## update to next index
 		self.filter_frame_idx = self.getNextIndex(self.filter_frame_idx, self.my_LP_SIZE-1)
 
+	def cal_start_R0(self):
+		if not self.my_resi_delta:
+			return
+		# calcualte average start R0
+		frame_cnt = 0
+		data = next(self.generator)
+		r0 = np.zeros(data.shape)
+		R0_AVE_TIMES = 10
+		# ## accumulate data
+		while frame_cnt < R0_AVE_TIMES: # use 10 frames to calculate
+			data = next(self.generator)
+			data = data.reshape(self.n[0], self.n[1])
+			if self.mask is not None:
+				data *= self.mask
+			self.calOppo_numpy_array(data, self.V0, self.R0_RECI)
+			r0 += -1 * data.flatten()
+			frame_cnt += 1
+		self.R0_START = r0 / R0_AVE_TIMES
+		print("start R0: ", self.R0_START)
+
 	def prepare_spatial(self):
 		def gaussianLP(distance):
 			return exp(-distance**2/(2*(self.my_SF_D0)**2))
 
 		def butterworthLP(distance):
 			return 1 / (1 + (distance / self.my_SF_D0)**(2 * self.my_BUTTER_ORDER))
 
@@ -327,23 +436,24 @@
 			arg_list_t = {}
 			if self.my_filter_temporal == FILTER_TEMPORAL.RW:
 				arg_list_t["cut-off normalized freqency"] = self.my_LP_W
 			if self.my_filter_temporal != FILTER_TEMPORAL.NONE:
 				arg_list_t["kernel size"] = self.my_LP_SIZE
 
 			## output to screen
+			print(f"  - Resistance mode: {'delta_R / R0' if self.my_resi_delta else ('-R' if self.my_resi_opposite else '1/R')}")
 			print(f"  - Spatial filter: {self.my_filter_spatial.value}")
 			for value, key in arg_list_s.items():
 				print(f"    {value}: {key}")
 			print(f"  - Temporal filter: {self.my_filter_temporal.value}")
 			for value, key in arg_list_t.items():
 				print(f"    {value}: {key}")
 
-			print(f"  - Calibration: {'No' if self.my_INIT_CALI_FRAMES == 0 else ''}")
-			if self.my_INIT_CALI_FRAMES != 0:
+			print(f"  - Calibration: {'No' if self.my_INIT_CALI_FRAMES == 0 or self.my_resi_delta else ''}")
+			if self.my_INIT_CALI_FRAMES != 0 and not self.my_resi_delta:
 				print(f"    Initializing frames:     {self.my_INIT_CALI_FRAMES}")
 				if self.my_WIN_SIZE == 0:
 					print("    Static calibration")
 				else:
 					print("    Dynamic calibration")
 					print(f"    Calibration window size: {self.my_WIN_SIZE}")
```

### Comparing `MatSense-0.4.0/matsense/process/interpolator.py` & `matsense-0.4.1/matsense/process/interpolator.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/process/point_tool.py` & `matsense-0.4.1/matsense/process/point_tool.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/process/pressure_selector.py` & `matsense-0.4.1/matsense/process/pressure_selector.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/process/processor.py` & `matsense-0.4.1/matsense/process/processor.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/server.py` & `matsense-0.4.1/matsense/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,23 +73,27 @@
 			paras['data_imu'], 
 			paras['idx_out'],
 			raw=paras['config']['process']['raw'],
 			warm_up=paras['config']['process']['warm_up'],
 			V0=paras['config']['process']['V0'],
 			R0_RECI=paras['config']['process']['R0_RECI'],
 			convert=paras['config']['process']['convert'],
+			resi_opposite=paras['config']['process']['resi_opposite'],
+			resi_delta=paras['config']['process']['resi_delta'],
 			mask=paras['config']['sensor']['mask'],
 			filter_spatial=paras['config']['process']['filter_spatial'],
 			filter_spatial_cutoff=paras['config']['process']['filter_spatial_cutoff'],
 			butterworth_order=paras['config']['process']['butterworth_order'],
 			filter_temporal=paras['config']['process']['filter_temporal'],
 			filter_temporal_size=paras['config']['process']['filter_temporal_size'],
 			rw_cutoff=paras['config']['process']['rw_cutoff'],
 			cali_frames=paras['config']['process']['cali_frames'],
 			cali_win_size=paras['config']['process']['cali_win_size'],
+            cali_threshold=paras['config']['process']['cali_threshold'],
+            cali_win_buffer_size=paras['config']['process']['cali_win_buffer_size'],
 			pipe_conn=paras['pipe_proc'],
 			copy_tags=False,
 			imu=paras['config']['serial']['imu'],
 			intermediate=paras['config']['process']['intermediate']
 		)
 		ret = my_proc.run()
 	except KeyboardInterrupt:
@@ -143,23 +147,27 @@
 		paras['data_raw'], 
 		paras['idx_out'],
 		raw=False,
 		warm_up=0,
 		V0=paras['config']['process']['V0'],
 		R0_RECI=paras['config']['process']['R0_RECI'],
 		convert=paras['config']['process']['convert'],
+		resi_opposite=paras['config']['process']['resi_opposite'],
+		resi_delta=paras['config']['process']['resi_delta'],
 		mask=paras['config']['sensor']['mask'],
 		filter_spatial=paras['config']['process']['filter_spatial'],
 		filter_spatial_cutoff=paras['config']['process']['filter_spatial_cutoff'],
 		butterworth_order=paras['config']['process']['butterworth_order'],
 		filter_temporal=paras['config']['process']['filter_temporal'],
 		filter_temporal_size=paras['config']['process']['filter_temporal_size'],
 		rw_cutoff=paras['config']['process']['rw_cutoff'],
 		cali_frames=paras['config']['process']['cali_frames'],
 		cali_win_size=paras['config']['process']['cali_win_size'],
+        cali_threshold=paras['config']['process']['cali_threshold'],
+        cali_win_buffer_size=paras['config']['process']['cali_win_buffer_size'],
 		pipe_conn=None,
 		output_filename=paras['config']['data']['out_filename'],
 		copy_tags=True,
 	)
 	## clear file content
 	clear_file(paras['config']['data']['out_filename'])
 	my_proc.run()
@@ -181,14 +189,18 @@
 		config['serial']['port'] = args.port
 	if config['connection']['udp'] is None or hasattr(args, 'udp'+DEST_SUFFIX):
 		config['connection']['udp'] = args.udp
 	if config['connection']['server_address'] is None or hasattr(args, 'address'+DEST_SUFFIX):
 		config['connection']['server_address'] = args.address
 	if config['process']['convert'] is None or hasattr(args, 'no_convert'+DEST_SUFFIX):
 		config['process']['convert'] = not args.no_convert
+	if config['process']['resi_opposite'] is None or hasattr(args, 'resi_opposite'+DEST_SUFFIX):
+		config['process']['resi_opposite'] = args.resi_opposite
+	if config['process']['resi_delta'] is None or hasattr(args, 'resi_delta'+DEST_SUFFIX):
+		config['process']['resi_delta'] = args.resi_delta
 	if config['visual']['zlim'] is None or hasattr(args, 'zlim'+DEST_SUFFIX):
 		config['visual']['zlim'] = args.zlim
 	if config['visual']['fps'] is None or hasattr(args, 'fps'+DEST_SUFFIX):
 		config['visual']['fps'] = args.fps
 	if config['visual']['pyqtgraph'] is None or hasattr(args, 'pyqtgraph'+DEST_SUFFIX):
 		config['visual']['pyqtgraph'] = args.pyqtgraph
 	if config['visual']['scatter'] is None or hasattr(args, 'scatter'+DEST_SUFFIX):
@@ -307,14 +319,16 @@
 	parser.add_argument('-t', dest='timeout', action=make_action('store'), default=TIMEOUT, type=float, help="specify timeout in seconds")
 	parser.add_argument('-n', dest='n', action=make_action('store'), default=[N], type=int, nargs='+', help="specify sensor shape")
 	parser.add_argument('--noservice', dest='noservice', action=make_action('store_true'), default=False, help="do not run service (only serial data receiving & processing)")
 	parser.add_argument('-a', '--address', dest='address', action=make_action('store'), help="specify server socket address")
 	parser.add_argument('-u', '--udp', dest='udp', action=make_action('store_true'), default=UDP, help="use UDP protocol")
 	parser.add_argument('-r', '--raw', dest='raw', action=make_action('store_true'), default=False, help="raw data mode")
 	parser.add_argument('-nc', '--no_convert', dest='no_convert', action=make_action('store_true'), default=NO_CONVERT, help="do not apply voltage-resistance conversion")
+	parser.add_argument('-ro', '--resi_opposite', dest='resi_opposite', action=make_action('store_true'), default=False, help="turn voltage to the opposite of resistance")
+	parser.add_argument('-rd', '--resi_delta', dest='resi_delta', action=make_action('store_true'), default=True, help="turn voltage to the delta_R / R0")
 	parser.add_argument('-v', '--visualize', dest='visualize', action=make_action('store_true'), default=False, help="enable visualization")
 	parser.add_argument('-z', '--zlim', dest='zlim', action=make_action('store'), default=ZLIM, type=float, help="z-axis limit")
 	parser.add_argument('-f', dest='fps', action=make_action('store'), default=FPS, type=int, help="frames per second")
 	parser.add_argument('--scatter', dest='scatter', action=make_action('store_true'), default=False, help="show scatter plot")
 	parser.add_argument('--pyqtgraph', dest='pyqtgraph', action=make_action('store_true'), default=False, help="use pyqtgraph to plot")
 	# parser.add_argument('-m', '--matplot', dest='matplot', action=make_action('store_true'), default=False, help="use matplotlib to plot")
 	parser.add_argument('--config', dest='config', action=make_action('store'), default=None, help="specify configuration file")
```

### Comparing `MatSense-0.4.0/matsense/serverkit/proc.py` & `matsense-0.4.1/matsense/serverkit/proc.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 						break
 					if flag == FLAG.FLAG_RESTART:
 						config_new = msg[1]
 						## restart with new config
 						ret = (1, config_new)
 						break
 					if flag in (FLAG.FLAG_REC_DATA, FLAG.FLAG_REC_RAW):
-						self.record_raw = True if flag == FLAG.FLAG_REC_RAW else True
+						self.record_raw = True if flag == FLAG.FLAG_REC_RAW else False
 						filename = msg[1]
 						if filename == "":
 							if flag == FLAG.FLAG_REC_RAW:
 								filename = datetime.now().strftime(self.FILENAME_TEMPLATE_RAW)
 							else:
 								filename = datetime.now().strftime(self.FILENAME_TEMPLATE)
 						try:
```

### Comparing `MatSense-0.4.0/matsense/serverkit/userver.py` & `matsense-0.4.1/matsense/serverkit/userver.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/tools.py` & `matsense-0.4.1/matsense/tools.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/uclient.py` & `matsense-0.4.1/matsense/uclient.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/visual/player.py` & `matsense-0.4.1/matsense/visual/player.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/visual/player1d.py` & `matsense-0.4.1/matsense/visual/player1d.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/visual/player_matplot.py` & `matsense-0.4.1/matsense/visual/player_matplot.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/visual/player_pyqtgraph.py` & `matsense-0.4.1/matsense/visual/player_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/matsense/visual/util.py` & `matsense-0.4.1/matsense/visual/util.py`

 * *Files identical despite different names*

### Comparing `MatSense-0.4.0/setup.py` & `matsense-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.4.0',  # Required
+    version='0.4.1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A toolkit for matrix sensor data processing 阵列传感器数据处理工具库',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -154,15 +154,15 @@
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[  # Optional
         "numpy>=1.19.2",
         "scipy>=1.5.4",
         "pyserial>=3.5",
         "PyYAML>=5.4.1",
         "pyparsing>=2.4.7",
-        "matplotlib>=3.3",
+        "matplotlib>=3.3,<=3.4",
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
```

