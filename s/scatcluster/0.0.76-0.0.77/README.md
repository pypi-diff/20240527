# Comparing `tmp/scatcluster-0.0.76.tar.gz` & `tmp/scatcluster-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.76.tar", last modified: Mon May 27 21:30:24 2024, max compression
+gzip compressed data, was "scatcluster-0.0.77.tar", last modified: Mon May 27 21:45:37 2024, max compression
```

## Comparing `scatcluster-0.0.76.tar` & `scatcluster-0.0.77.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:30:24.377102 scatcluster-0.0.76/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 21:30:20.000000 scatcluster-0.0.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 21:30:20.000000 scatcluster-0.0.76/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:30:24.377102 scatcluster-0.0.76/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:30:24.373103 scatcluster-0.0.76/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:30:24.377102 scatcluster-0.0.76/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:30:24.377102 scatcluster-0.0.76/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    26950 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-27 21:30:20.000000 scatcluster-0.0.76/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:30:24.377102 scatcluster-0.0.76/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:30:24.000000 scatcluster-0.0.76/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 21:30:24.000000 scatcluster-0.0.76/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:30:24.000000 scatcluster-0.0.76/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 21:30:24.000000 scatcluster-0.0.76/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 21:30:24.000000 scatcluster-0.0.76/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:30:24.377102 scatcluster-0.0.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 21:30:21.000000 scatcluster-0.0.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:45:37.211999 scatcluster-0.0.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 21:45:33.000000 scatcluster-0.0.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 21:45:33.000000 scatcluster-0.0.77/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:45:37.211999 scatcluster-0.0.77/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:45:37.207999 scatcluster-0.0.77/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:45:37.207999 scatcluster-0.0.77/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:45:37.211999 scatcluster-0.0.77/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-27 21:45:33.000000 scatcluster-0.0.77/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:45:37.211999 scatcluster-0.0.77/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:45:37.000000 scatcluster-0.0.77/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 21:45:37.000000 scatcluster-0.0.77/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:45:37.000000 scatcluster-0.0.77/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 21:45:37.000000 scatcluster-0.0.77/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 21:45:37.000000 scatcluster-0.0.77/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:45:37.211999 scatcluster-0.0.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 21:45:34.000000 scatcluster-0.0.77/setup.py
```

### Comparing `scatcluster-0.0.76/LICENSE` & `scatcluster-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/PKG-INFO` & `scatcluster-0.0.77/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.76
+Version: 0.0.77
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.76/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.77/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.77/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.77/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/analysis/predictions.py` & `scatcluster-0.0.77/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/analysis/processing.py` & `scatcluster-0.0.77/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.77/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.77/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/helper.py` & `scatcluster-0.0.77/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/processing/ica.py` & `scatcluster-0.0.77/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/processing/scattering.py` & `scatcluster-0.0.77/scatcluster/processing/scattering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pickle
 
 import cupy as cp
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import scipy as sp
+from scipy import stats as sp_stats
 import xarray as xr
 from matplotlib import dates as mdates
 from obspy.clients.filesystem.sds import Client
 from obspy.core import UTCDateTime
 from obspy.core.stream import Stream
 from scatseisnet.network import ScatteringNetwork
 from scatseisnet.operation import segmentize
@@ -18,57 +18,63 @@
 
 class Scattering:
 
     def reduce_type(self):
         """
         Pooling operation performed on the last axis.
         """
-        pooling_options = [
-            ('avg', np.mean),
-            ('max', np.max),
-            ('median', np.median),
-            ('std', np.std),
-            ('gmean', sp.stats.gmean),
-            ('hmean', sp.stats.hmean),
-            ('pmean', sp.stats.pmean),
-            ('kurtosis', sp.stats.kurtosis),
-            ('skew', sp.stats.skew),
-            ('entropy', sp.stats.entropy),
-            ('sem', sp.stats.sem),
-            ('differential_entropy', sp.stats.differential_entropy),
-            ('median_abs_deviation', sp.stats.median_abs_deviation),
-        ]
-        for po in pooling_options:
-            if self.network_pooling == po[0]:
-                return po[1]
+        pooling_options = {
+            'avg': np.mean,
+            'max': np.max,
+            'median': np.median,
+            'std': np.std,
+            'gmean': sp_stats.gmean,
+            'hmean': sp_stats.hmean,
+            'pmean': sp_stats.hmean,
+            'kurtosis': sp_stats.kurtosis,
+            'skew': sp_stats.skew,
+            'entropy': sp_stats.entropy,
+            'sem': sp_stats.sem,
+            'differential_entropy': sp_stats.differential_entropy,
+            'median_abs_deviation': sp_stats.median_abs_deviation,
+        }
+        return pooling_options.get(self.network_pooling, None)
 
     def load_data_times(self):
         """
         Load the data times from a file and store them in the `data_times` attribute.
 
         This function reads the data times from a file located at
         `{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_`
         `{self.network_name}_times.npy` and stores them in the `data_times` attribute.
 
         """
-        self.data_times = np.load(
-            f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
-            f'{self.network_name}_times.npy')
+        try:
+            file_path = f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_' \
+                        f'{self.network_name}_times.npy'
+            self.data_times = np.load(file_path)
+        except FileNotFoundError:
+            print(f"File not found: {file_path}")
+        except Exception as e:
+            print(f"An error occurred while loading data times: {e}")        
 
     def build_day_list(self) -> None:
         """Build data_day_list object
         """
-        day_list = [
-            day_start for day_start in pd.date_range(
-                UTCDateTime(self.data_starttime).strftime('%Y%m%d'), (
-                    UTCDateTime(self.data_endtime) - (60 * 60 * 24)).strftime('%Y%m%d')).strftime('%Y-%m-%d').tolist()
-            if day_start not in [UTCDateTime(day_exc).strftime('%Y-%m-%d') for day_exc in self.data_exclude_days]
-        ]
-
-        self.data_day_list = day_list
+        try:
+            start_time = UTCDateTime(self.data_starttime)
+            end_time = UTCDateTime(self.data_endtime)
+            exclude_days = [UTCDateTime(day).strftime('%Y-%m-%d') for day in self.data_exclude_days]
+            day_list = [
+                day_start for day_start in pd.date_range(start_time.strftime('%Y%m%d'), end_time.strftime('%Y%m%d')).strftime('%Y-%m-%d').tolist()
+                if day_start not in exclude_days
+            ]
+            self.data_day_list = day_list
+        except Exception as e:
+            print(f"An error occurred while building day list: {e}")
 
     def build_channel_list(self) -> None:
         if self.sample_stream is None:
             self.process_sample_data()
         self.channel_list = [trace.stats.channel for trace in self.sample_stream]
 
     def stream_process(self, stream: Stream) -> Stream:
```

### Comparing `scatcluster-0.0.76/scatcluster/scatcluster.py` & `scatcluster-0.0.77/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster/structure.py` & `scatcluster-0.0.77/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.77/scatcluster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.76
+Version: 0.0.77
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.76/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.77/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.76/setup.py` & `scatcluster-0.0.77/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.76',
+    version='0.0.77',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

