# Comparing `tmp/scatcluster-0.0.71.tar.gz` & `tmp/scatcluster-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.71.tar", last modified: Mon May 27 20:35:04 2024, max compression
+gzip compressed data, was "scatcluster-0.0.72.tar", last modified: Mon May 27 20:46:50 2024, max compression
```

## Comparing `scatcluster-0.0.71.tar` & `scatcluster-0.0.72.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:04.749250 scatcluster-0.0.71/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 20:35:01.000000 scatcluster-0.0.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:35:01.000000 scatcluster-0.0.71/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:35:04.749250 scatcluster-0.0.71/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:04.745250 scatcluster-0.0.71/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:04.749250 scatcluster-0.0.71/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:04.749250 scatcluster-0.0.71/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    25943 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 20:35:01.000000 scatcluster-0.0.71/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:04.749250 scatcluster-0.0.71/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:35:04.000000 scatcluster-0.0.71/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 20:35:04.000000 scatcluster-0.0.71/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:35:04.000000 scatcluster-0.0.71/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 20:35:04.000000 scatcluster-0.0.71/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 20:35:04.000000 scatcluster-0.0.71/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:35:04.749250 scatcluster-0.0.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 20:35:01.000000 scatcluster-0.0.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:50.536387 scatcluster-0.0.72/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 20:46:47.000000 scatcluster-0.0.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:46:47.000000 scatcluster-0.0.72/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:46:50.536387 scatcluster-0.0.72/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:50.528387 scatcluster-0.0.72/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:50.532387 scatcluster-0.0.72/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:50.532387 scatcluster-0.0.72/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26829 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 20:46:47.000000 scatcluster-0.0.72/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:50.532387 scatcluster-0.0.72/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 20:46:50.000000 scatcluster-0.0.72/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 20:46:50.000000 scatcluster-0.0.72/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:46:50.000000 scatcluster-0.0.72/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 20:46:50.000000 scatcluster-0.0.72/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 20:46:50.000000 scatcluster-0.0.72/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:46:50.536387 scatcluster-0.0.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 20:46:47.000000 scatcluster-0.0.72/setup.py
```

### Comparing `scatcluster-0.0.71/LICENSE` & `scatcluster-0.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/PKG-INFO` & `scatcluster-0.0.72/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.71
+Version: 0.0.72
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.71/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.72/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.72/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.72/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/analysis/predictions.py` & `scatcluster-0.0.72/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/analysis/processing.py` & `scatcluster-0.0.72/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.72/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.72/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/helper.py` & `scatcluster-0.0.72/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/processing/ica.py` & `scatcluster-0.0.72/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster/processing/scattering.py` & `scatcluster-0.0.72/scatcluster/processing/scattering.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
             if day_start not in [UTCDateTime(day_exc).strftime('%Y-%m-%d') for day_exc in self.data_exclude_days]
         ]
 
         self.data_day_list = day_list
         
         
     def build_channel_list(self) -> None:
+        if self.sample_stream is None:
+            self.process_sample_data()
         self.channel_list = [trace.stats.channel for trace in self.sample_stream]
 
     def stream_process(self, stream: Stream) -> Stream:
         """PreProcessing of obspy stream before calculating scattering coefficients
 
         Args:
             stream (Stream): Obspy Stream
@@ -570,14 +572,30 @@
         # Store Data
         np.save(
             f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
             f'{self.network_name}_times.npy', self.data_times)
         np.save(
             f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
             f'{self.network_name}_scat_coef_vectorized.npy', self.data_scat_coef_vectorized)
+        coefficients.to_netcdf(
+            f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
+            f'{self.network_name}_scat_coef_xarray.nc')
+        
+    def load_scattering_coefficients_xarray(self):
+        """
+        Load the scattering coefficients from an xarray dataset file and store them in the `scattering_coefficients_xarray` attribute.
+
+        Returns:
+            xr.Dataset: The loaded scattering coefficients dataset.
+        """
+        scat_coeff_xr = xr.open_dataset(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
+                                        f'{self.network_name}_scat_coef_xarray.nc')
+        self.scattering_coefficients_xarray = scat_coeff_xr
+        return scat_coeff_xr 
+        
 
     def preload_times(self):
         """
         Preloads the times data from a numpy file and assigns it to the `data_times` attribute of the class.
 
         """
         data_times = np.load(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
```

### Comparing `scatcluster-0.0.71/scatcluster/scatcluster.py` & `scatcluster-0.0.72/scatcluster/scatcluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,16 @@
             ica_max_ICAs: int = 10,
             ica_overwrite_previous_models: bool = False,
             ica_explained_variance_score: float = None,  # pylint: disable=unused-argument
             dendrogram_method: str = 'ward',
             dendrogram_time_zone: str = None,  # pylint: disable=unused-argument
             waveforms_n_samples: int = 5,
             waveforms=None,  # pylint: disable=unused-argument
-            spectrograms=None):  # pylint: disable=unused-argument
+            spectrograms=None, # pylint: disable=unused-argument
+            scattering_coefficients_xarray=None):  # pylint: disable=unused-argument
         """
         Initializes a ScatCluster instance.
 
         Args:
             data_savepath (str): The path to save data.
             data_client_path (str): The path to the client data.
             data_network (str): The network name.
@@ -110,14 +111,15 @@
             ica_overwrite_previous_models (bool, optional): Whether to overwrite previous models. Defaults to False.
             ica_explained_variance_score (float, optional): The explained variance score. Defaults to None.
             dendrogram_method (str, optional): The dendrogram method. Defaults to 'ward'.
             dendrogram_time_zone (str, optional): The dendrogram time zone. Defaults to None.
             waveforms_n_samples (int, optional): The number of samples for waveforms. Defaults to 5.
             waveforms (Optional): The waveforms. Defaults to None.
             spectrograms (Optional): The spectrograms. Defaults to None.
+            scattering_coefficients_xarray (Optional): Xarray containing the scattering coefficients. Defaults to None.
         """
 
         self.sc_config = sc_config
         self.data_savepath = data_savepath
         self.data_client_path = data_client_path
         self.data_network = data_network
         self.data_station = data_station
@@ -164,14 +166,15 @@
         self.dendrogram_time_zone = None
         self.waveforms_n_samples = waveforms_n_samples
         self.network_banks_name = '_'.join([str(order[vals]) for order in self.network_banks for vals in order.keys()])
         self.network_name = (f'{self.network_segment}_{self.network_step}_{self.network_sampling_rate}_'
                              f'{self.network_banks_name}_{self.network_pooling}')
         self.waveforms = None
         self.spectrograms = None
+        self.scattering_coefficients_xarray = None
 
     def __setitem__(self, key, value):
         """
         Set the value of an item in the object.
 
         Parameters:
             key (str): The key of the item.
```

### Comparing `scatcluster-0.0.71/scatcluster/structure.py` & `scatcluster-0.0.72/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.72/scatcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.71
+Version: 0.0.72
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.71/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.72/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.71/setup.py` & `scatcluster-0.0.72/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.71',
+    version='0.0.72',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

