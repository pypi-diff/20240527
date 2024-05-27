# Comparing `tmp/scatcluster-0.0.66.tar.gz` & `tmp/scatcluster-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.66.tar", last modified: Mon May 27 19:51:37 2024, max compression
+gzip compressed data, was "scatcluster-0.0.67.tar", last modified: Mon May 27 20:00:21 2024, max compression
```

## Comparing `scatcluster-0.0.66.tar` & `scatcluster-0.0.67.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 19:51:34.000000 scatcluster-0.0.66/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 19:51:34.000000 scatcluster-0.0.66/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 19:51:37.793326 scatcluster-0.0.66/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.789326 scatcluster-0.0.66/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:51:37.793326 scatcluster-0.0.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 19:51:34.000000 scatcluster-0.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:21.817982 scatcluster-0.0.67/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 20:00:18.000000 scatcluster-0.0.67/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:00:18.000000 scatcluster-0.0.67/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:00:21.817982 scatcluster-0.0.67/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:21.813982 scatcluster-0.0.67/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:21.817982 scatcluster-0.0.67/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:21.817982 scatcluster-0.0.67/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25929 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 20:00:18.000000 scatcluster-0.0.67/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:21.817982 scatcluster-0.0.67/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:00:21.000000 scatcluster-0.0.67/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 20:00:21.000000 scatcluster-0.0.67/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:00:21.000000 scatcluster-0.0.67/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 20:00:21.000000 scatcluster-0.0.67/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 20:00:21.000000 scatcluster-0.0.67/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:00:21.817982 scatcluster-0.0.67/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 20:00:18.000000 scatcluster-0.0.67/setup.py
```

### Comparing `scatcluster-0.0.66/LICENSE` & `scatcluster-0.0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/PKG-INFO` & `scatcluster-0.0.67/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.66
+Version: 0.0.67
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.66/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.67/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.67/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.67/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/analysis/predictions.py` & `scatcluster-0.0.67/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/analysis/processing.py` & `scatcluster-0.0.67/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.67/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.67/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/helper.py` & `scatcluster-0.0.67/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/processing/ica.py` & `scatcluster-0.0.67/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/processing/scattering.py` & `scatcluster-0.0.67/scatcluster/processing/scattering.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
         # SAVE NETWORK IN PICKLE FILE
         with open(
                 f'{self.data_savepath}networks/{self.data_network}_{self.data_station}_{self.data_location}_'
                 f'{self.network_name}.pickle', 'wb') as handle:
             pickle.dump(self.net, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
-    def plot_network_filter_banks(self) -> None:
+    def plot_network_filter_banks(self, savefig: bool = True) -> None:
         """
         Plot the filter banks
         """
         NROWS = len(self.net.banks)
         # Crete axes
         octaves = [bank.octaves for bank in self.net.banks]
         height_ratios = 2, (octaves[1] + 2) / (octaves[0] + 2)
@@ -199,16 +199,17 @@
         # Legend
         axes[1][0].legend([r"Re $\varphi(t)$", r"Im $\varphi(t)$"], loc=1)
         axes[1][1].legend([r"$\hat\varphi(\omega)$"], loc=1)
 
         plt.suptitle('ScatCluster Parametrization'
                     f'\nSegment:{self.network_segment}s  Step: {self.network_step}\n Banks: {self.network_banks_name}')
         plt.subplots_adjust(top=0.9) 
-        plt.savefig(f'{self.data_savepath}figures/{self.data_network}_{self.data_station}_{self.data_location}_'
-                    f'{self.network_name}_filter_banks.png')
+        if savefig:
+            plt.savefig(f'{self.data_savepath}figures/{self.data_network}_{self.data_station}_{self.data_location}_'
+                        f'{self.network_name}_filter_banks.png')
 
     def load_sample_data(self) -> Stream:
         """Load sample
         """
         return self.load_data(starttime=UTCDateTime(self.data_sample_starttime),
                               endtime=UTCDateTime(self.data_sample_endtime),
                               channel=self.data_channel)
```

### Comparing `scatcluster-0.0.66/scatcluster/scatcluster.py` & `scatcluster-0.0.67/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster/structure.py` & `scatcluster-0.0.67/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.67/scatcluster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.66
+Version: 0.0.67
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.66/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.67/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.66/setup.py` & `scatcluster-0.0.67/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.66',
+    version='0.0.67',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

