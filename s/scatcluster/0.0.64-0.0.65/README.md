# Comparing `tmp/scatcluster-0.0.64.tar.gz` & `tmp/scatcluster-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.64.tar", last modified: Sun May 26 19:57:22 2024, max compression
+gzip compressed data, was "scatcluster-0.0.65.tar", last modified: Mon May 27 17:53:32 2024, max compression
```

## Comparing `scatcluster-0.0.64.tar` & `scatcluster-0.0.65.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:57:22.644570 scatcluster-0.0.64/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-26 19:57:17.000000 scatcluster-0.0.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 19:57:17.000000 scatcluster-0.0.64/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 19:57:22.644570 scatcluster-0.0.64/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:57:22.640570 scatcluster-0.0.64/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:57:22.640570 scatcluster-0.0.64/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:57:22.644570 scatcluster-0.0.64/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    24715 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-26 19:57:17.000000 scatcluster-0.0.64/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:57:22.644570 scatcluster-0.0.64/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 19:57:22.000000 scatcluster-0.0.64/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-26 19:57:22.000000 scatcluster-0.0.64/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:57:22.000000 scatcluster-0.0.64/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-26 19:57:22.000000 scatcluster-0.0.64/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 19:57:22.000000 scatcluster-0.0.64/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:57:22.644570 scatcluster-0.0.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-26 19:57:17.000000 scatcluster-0.0.64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 17:53:29.000000 scatcluster-0.0.65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 17:53:29.000000 scatcluster-0.0.65/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 17:53:32.587445 scatcluster-0.0.65/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.583445 scatcluster-0.0.65/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24705 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:53:32.587445 scatcluster-0.0.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 17:53:29.000000 scatcluster-0.0.65/setup.py
```

### Comparing `scatcluster-0.0.64/LICENSE` & `scatcluster-0.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/PKG-INFO` & `scatcluster-0.0.65/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.64
+Version: 0.0.65
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.64/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.65/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.65/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.65/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/analysis/predictions.py` & `scatcluster-0.0.65/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/analysis/processing.py` & `scatcluster-0.0.65/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.65/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.65/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/helper.py` & `scatcluster-0.0.65/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/processing/ica.py` & `scatcluster-0.0.65/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/processing/scattering.py` & `scatcluster-0.0.65/scatcluster/processing/scattering.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
                 if len(stream.traces) == 0:
                     print(f'>> Skipping {day_start} as there is no traces')
                 elif len(stream.traces) < 3:
                     print(f'>> Skipping {day_start} as there is not all 3 channels')
                 else:
                     # Numpyification
                     times = stream[0].times('matplotlib')
-                    data = np.array([trace.data for trace in stream])
+                    data = [trace.data for trace in stream]
 
                     # Segmentization
                     data_segments = segmentize(data, self.network_samples_per_segment, self.network_samples_per_step)
                     times_scat = segmentize(times, self.network_samples_per_segment, self.network_samples_per_step)[:,
                                                                                                                     0]
 
                     # Scattering transform
```

### Comparing `scatcluster-0.0.64/scatcluster/scatcluster.py` & `scatcluster-0.0.65/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster/structure.py` & `scatcluster-0.0.65/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.65/scatcluster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.64
+Version: 0.0.65
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.64/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.65/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.64/setup.py` & `scatcluster-0.0.65/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.64',
+    version='0.0.65',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

