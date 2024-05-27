# Comparing `tmp/scatcluster-0.0.73.tar.gz` & `tmp/scatcluster-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.73.tar", last modified: Mon May 27 20:51:21 2024, max compression
+gzip compressed data, was "scatcluster-0.0.74.tar", last modified: Mon May 27 21:00:26 2024, max compression
```

## Comparing `scatcluster-0.0.73.tar` & `scatcluster-0.0.74.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:51:21.729417 scatcluster-0.0.73/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 20:51:18.000000 scatcluster-0.0.73/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:51:18.000000 scatcluster-0.0.73/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:51:21.729417 scatcluster-0.0.73/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:51:21.725417 scatcluster-0.0.73/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:51:21.729417 scatcluster-0.0.73/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:51:21.729417 scatcluster-0.0.73/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    26829 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 20:51:18.000000 scatcluster-0.0.73/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:51:21.729417 scatcluster-0.0.73/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:51:21.000000 scatcluster-0.0.73/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 20:51:21.000000 scatcluster-0.0.73/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:51:21.000000 scatcluster-0.0.73/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 20:51:21.000000 scatcluster-0.0.73/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 20:51:21.000000 scatcluster-0.0.73/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:51:21.729417 scatcluster-0.0.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 20:51:18.000000 scatcluster-0.0.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 21:00:23.000000 scatcluster-0.0.74/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 21:00:23.000000 scatcluster-0.0.74/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:00:26.587015 scatcluster-0.0.74/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.583016 scatcluster-0.0.74/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26855 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:00:26.587015 scatcluster-0.0.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 21:00:23.000000 scatcluster-0.0.74/setup.py
```

### Comparing `scatcluster-0.0.73/LICENSE` & `scatcluster-0.0.74/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/PKG-INFO` & `scatcluster-0.0.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.73
+Version: 0.0.74
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.73/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.74/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.74/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.74/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/analysis/predictions.py` & `scatcluster-0.0.74/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/analysis/processing.py` & `scatcluster-0.0.74/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.74/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.74/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/helper.py` & `scatcluster-0.0.74/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/processing/ica.py` & `scatcluster-0.0.74/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/processing/scattering.py` & `scatcluster-0.0.74/scatcluster/processing/scattering.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,15 +490,15 @@
         del SC1
 
         
         
         n_samples = len(times)
         n_channels = len(self.channel_list)
         
-        attributes = {**self.__dict__}
+        attributes = {k:str(v) for k,v in self.__dict__.items()}
 
         # The coordinates of the xarray dataset are the center frequencies of the
         # scattering network, the starttime of the waveforms, and the channel names.
         center_frequencies = [bank.centers for bank in self.net.banks]
         coordinates = {
                 "time": ("time", times),
                 "channel": ("channel", self.channel_list),
```

### Comparing `scatcluster-0.0.73/scatcluster/scatcluster.py` & `scatcluster-0.0.74/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster/structure.py` & `scatcluster-0.0.74/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.74/scatcluster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.73
+Version: 0.0.74
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.73/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.74/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.73/setup.py` & `scatcluster-0.0.74/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.73',
+    version='0.0.74',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

