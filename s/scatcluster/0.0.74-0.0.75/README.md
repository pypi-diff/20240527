# Comparing `tmp/scatcluster-0.0.74.tar.gz` & `tmp/scatcluster-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.74.tar", last modified: Mon May 27 21:00:26 2024, max compression
+gzip compressed data, was "scatcluster-0.0.75.tar", last modified: Mon May 27 21:28:18 2024, max compression
```

## Comparing `scatcluster-0.0.74.tar` & `scatcluster-0.0.75.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 21:00:23.000000 scatcluster-0.0.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 21:00:23.000000 scatcluster-0.0.74/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:00:26.587015 scatcluster-0.0.74/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.583016 scatcluster-0.0.74/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    26855 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 21:00:23.000000 scatcluster-0.0.74/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:00:26.587015 scatcluster-0.0.74/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 21:00:26.000000 scatcluster-0.0.74/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:00:26.587015 scatcluster-0.0.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 21:00:23.000000 scatcluster-0.0.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:28:18.978503 scatcluster-0.0.75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 21:28:15.000000 scatcluster-0.0.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 21:28:15.000000 scatcluster-0.0.75/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:28:18.974503 scatcluster-0.0.75/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:28:18.970503 scatcluster-0.0.75/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:28:18.974503 scatcluster-0.0.75/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:28:18.974503 scatcluster-0.0.75/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26950 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-27 21:28:15.000000 scatcluster-0.0.75/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:28:18.974503 scatcluster-0.0.75/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 21:28:18.000000 scatcluster-0.0.75/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 21:28:18.000000 scatcluster-0.0.75/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:28:18.000000 scatcluster-0.0.75/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 21:28:18.000000 scatcluster-0.0.75/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 21:28:18.000000 scatcluster-0.0.75/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:28:18.978503 scatcluster-0.0.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 21:28:15.000000 scatcluster-0.0.75/setup.py
```

### Comparing `scatcluster-0.0.74/LICENSE` & `scatcluster-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.74/PKG-INFO` & `scatcluster-0.0.75/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.74
+Version: 0.0.75
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.74/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.75/scatcluster/analysis/crosstab.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             ct_data = pd.crosstab(df_preds.predictions_1, df_preds.predictions_2)
         elif normalization in normalization_options:
             ct_data = pd.crosstab(df_preds.predictions_1, df_preds.predictions_2, normalize=normalization)
             ct_data = ct_data * 100
         else:
             raise ValueError(
                 f"Provided Normalization is not valid. This can be 'None' or [{normalization_options}]. Kindly see "
-                f"https://pandas.pydata.org/docs/reference/api/pandas.crosstab.html for more info.")
+                f'https://pandas.pydata.org/docs/reference/api/pandas.crosstab.html for more info.')
         ct_data = ct_data.sort_index(ascending=False)
         return ct_data, factor_difference, fowlkes_mallows_score(df_preds.predictions_1, df_preds.predictions_2)
 
     def plot_clustering_crosstab(self,
                                  cluster_1=3600,
                                  num_clusters_1=10,
                                  cluster_2=60,
```

### Comparing `scatcluster-0.0.74/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.75/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.74/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.75/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.74/scatcluster/analysis/predictions.py` & `scatcluster-0.0.75/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.74/scatcluster/analysis/processing.py` & `scatcluster-0.0.75/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.74/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.75/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.74/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.75/scatcluster/analysis/waveforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             waveforms_n_samples (int, optional): Number of waveforms to plot. Defaults to None.
             **kwargs: Additional keyword arguments to pass to plt.subplots().
         """
         # get channel list from plotting
         stream = self.load_data(starttime=UTCDateTime(self.data_sample_starttime),
                                 endtime=UTCDateTime(self.data_sample_endtime),
                                 channel=self.data_channel)
-        channel_list = sorted(list(set([trace.stats.channel for trace in stream])))
+        channel_list = sorted(trace.stats.channel for trace in stream)
 
         if clusters is not None:
             classes = clusters
         else:
             # Calculate centroid
             classes = np.unique(self.dendrogram_predictions)
```

### Comparing `scatcluster-0.0.74/scatcluster/helper.py` & `scatcluster-0.0.75/scatcluster/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return False
 
 
 def tqdm_importer():
     """
     A function that imports the tqdm module based on the current environment.
     """
-    if is_notebook:
+    if is_notebook():
         pass
     else:
         pass
 
 
 def demad(x, factor=10.0):
     """Normalize signal with median absolute deviation.
```

### Comparing `scatcluster-0.0.74/scatcluster/processing/ica.py` & `scatcluster-0.0.75/scatcluster/processing/ica.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import numpy as np
 import pandas as pd
 from matplotlib import dates as mdates
 from obspy.core import UTCDateTime
 from scipy.signal import medfilt
 from sklearn.decomposition import FastICA
 from sklearn.metrics import explained_variance_score, mean_squared_error
-from sklearn.preprocessing import RobustScaler
 
 from scatcluster.helper import demad, list_of_strings
 
 
 def round_nearest(x, a):
     """
     Rounds a number `x` to the nearest multiple of `a`.
@@ -82,15 +81,16 @@
         """
         print(f'Performing ICA for {num_ICA} ICAs')
         ica_model_path = (f'{self.data_savepath}ICA/{self.data_network}_{self.data_station}_{self.data_location}_'
                           f'{self.network_name}_dimension_{num_ICA}.pickle')
         # check if reduction exists already
         if os.path.exists(ica_model_path) and self.ica_overwrite_previous_models is False:
             print('  Using pre-calculated model')
-            model = pickle.load(open(ica_model_path, 'rb'))
+            with open(ica_model_path, 'rb') as f:
+                model = pickle.load(f)
         else:
             # else fit
             kwargs['max_iter'] = 1000 if kwargs.get('max_iter') is None else kwargs.get('max_iter')
             kwargs['whiten'] = 'unit-variance' if kwargs.get('whiten') is None else kwargs.get('whiten')
             model = FastICA(n_components=num_ICA, random_state=42, **kwargs)
 
         # Exclude any timestamps
@@ -176,22 +176,21 @@
 
         Args:
             num_ICA (int): Desired number of ICAs
         """
         if not os.path.exists(f'{self.data_savepath}ICA/{self.data_network}_{self.data_station}_{self.data_location}_'
                               f'{self.network_name}_dimension_{num_ICA}.pickle'):
             raise ValueError(
-                f"The supplied number of ICAs {num_ICA} has not been computed. Choose another number for the ICAs or "
+                f'The supplied number of ICAs {num_ICA} has not been computed. Choose another number for the ICAs or '
                 f"calcate using 'process_ICA_single'")
 
-        self.ica = pickle.load(
-            open(
-                f'{self.data_savepath}ICA/{self.data_network}_{self.data_station}_{self.data_location}_'
-                f'{self.network_name}_dimension_{num_ICA}.pickle', 'rb'))
-
+        ica_file = f'{self.data_savepath}ICA/{self.data_network}_{self.data_station}_{self.data_location}_' + \
+                    f'{self.network_name}_dimension_{num_ICA}.pickle'
+        with open(ica_file, 'rb') as f:
+            self.ica = pickle.load(f)
         ica_results = np.load(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
                               f'{self.network_name}_features_{num_ICA}.npz')
         self.ica_features = ica_results['features']
         self.ica_features_inverse = ica_results['features_inverse']
         self.ica_explained_variance_score = ica_results['score_explained_variance']
         self.ica_mse = ica_results['score_mse']
```

### Comparing `scatcluster-0.0.74/scatcluster/processing/scattering.py` & `scatcluster-0.0.75/scatcluster/processing/scattering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import pickle
 
+import cupy as cp
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scipy as sp
+import xarray as xr
 from matplotlib import dates as mdates
 from obspy.clients.filesystem.sds import Client
 from obspy.core import UTCDateTime
 from obspy.core.stream import Stream
 from scatseisnet.network import ScatteringNetwork
 from scatseisnet.operation import segmentize
-import cupy as cp
-import xarray as xr
 from tqdm import tqdm
 
 
 class Scattering:
 
     def reduce_type(self):
         """
@@ -61,16 +61,15 @@
             day_start for day_start in pd.date_range(
                 UTCDateTime(self.data_starttime).strftime('%Y%m%d'), (
                     UTCDateTime(self.data_endtime) - (60 * 60 * 24)).strftime('%Y%m%d')).strftime('%Y-%m-%d').tolist()
             if day_start not in [UTCDateTime(day_exc).strftime('%Y-%m-%d') for day_exc in self.data_exclude_days]
         ]
 
         self.data_day_list = day_list
-        
-        
+
     def build_channel_list(self) -> None:
         if self.sample_stream is None:
             self.process_sample_data()
         self.channel_list = [trace.stats.channel for trace in self.sample_stream]
 
     def stream_process(self, stream: Stream) -> Stream:
         """PreProcessing of obspy stream before calculating scattering coefficients
@@ -78,19 +77,19 @@
         Args:
             stream (Stream): Obspy Stream
 
         Returns:
             Stream: processed obspy Stream
         """
         # Remove trend
-        stream.detrend(type="demean")
+        stream.detrend(type='demean')
         # High-pass filter
-        stream.filter(type="highpass", freq=0.5)
+        stream.filter(type='highpass', freq=0.5)
         # Remove residual trend
-        stream.detrend(type="constant")
+        stream.detrend(type='constant')
         # Remove edge effects
         stream.taper(0.05)
         return stream
 
     def load_data(self, starttime: UTCDateTime, endtime: UTCDateTime, channel: str) -> Stream:
         """Load the seismic and trim according to data_starttime and data_endtime
 
@@ -138,77 +137,79 @@
         """
         Plot the filter banks
         """
         NROWS = len(self.net.banks)
         # Crete axes
         octaves = [bank.octaves for bank in self.net.banks]
         height_ratios = 2, (octaves[1] + 2) / (octaves[0] + 2)
-        grid = dict(height_ratios=height_ratios, wspace=0.1, hspace=0.1)
-        _, axes = plt.subplots(NROWS, 2, figsize=(10, 10), gridspec_kw=grid, sharey="row"
-        )
+        grid = {'height_ratios': height_ratios, 'wspace': 0.1, 'hspace': 0.1}
+        _, axes = plt.subplots(NROWS, 2, figsize=(10, 10), gridspec_kw=grid, sharey='row')
         # Loop over network layers
         for ax_enum, (ax, bank) in enumerate(zip(axes, self.net.banks)):
             # Limit view to three times the temporal width of largest wavelet
             width_max = min(2 * bank.widths.max(), bank.times.max())
-            if type(bank.wavelets) == cp.ndarray:
+            if isinstance(bank.wavelets, cp.ndarray):
                 bank.wavelets = bank.wavelets.get()
-            if type(bank.spectra) == cp.ndarray:
+            if isinstance(bank.spectra, cp.ndarray):
                 bank.spectra = bank.spectra.get()
-            if type(bank.widths) == cp.ndarray:
+            if isinstance(bank.widths, cp.ndarray):
                 bank.widths = bank.widths.get()
-            if type(bank.centers) == cp.ndarray:
-                bank.centers = bank.centers.get()        
+            if isinstance(bank.centers, cp.ndarray):
+                bank.centers = bank.centers.get()
+            if isinstance(bank.frequencies, cp.ndarray):
+                bank.centers = bank.frequencies.get()
 
             # Temporal
             for octave_enum, (wavelet, octave, width) in enumerate(zip(bank.wavelets, bank.ratios, bank.widths)):
                 # Truncate time for small-duration wavelets
                 inner = np.abs(bank.times) < width_max
                 t = bank.times[inner]
                 y = wavelet[inner] / np.abs(wavelet[inner].max()) / 3
-                ax[0].plot(t, y.real + octave, color="C0", zorder=1)
-                ax[0].plot(t, y.imag + octave, color="C0", zorder=0, alpha=0.4)
-                ax[0].text(-1*width_max*(1 if octave_enum%2==0 else 1.1), octave, f'{width*4:.2f}', fontsize='small')
+                ax[0].plot(t, y.real + octave, color='C0', zorder=1)
+                ax[0].plot(t, y.imag + octave, color='C0', zorder=0, alpha=0.4)
+                ax[0].text(-1 * width_max * (1 if octave_enum % 2 == 0 else 1.1),
+                           octave,
+                           f'{width*4:.2f}',
+                           fontsize='small')
 
             # Spectral
-            sepctra = bank.spectra
             frequencies = bank.frequencies
             for octave_enum, (spectrum, octave, center) in enumerate(zip(bank.spectra, bank.ratios, bank.centers)):
                 inner = frequencies > frequencies[1]
                 f = frequencies[inner]
                 y = spectrum[inner]
                 y /= np.abs(y.max())
-                ax[1].plot(f, np.abs(y) + octave, color="C0")
-                ax[1].text((10**-2)*(1 if octave_enum%2==0 else 1.1), octave, f'{center:.2f}', fontsize='small')
-            
+                ax[1].plot(f, np.abs(y) + octave, color='C0')
+                ax[1].text((10**-2) * (1 if octave_enum % 2 == 0 else 1.1), octave, f'{center:.2f}', fontsize='small')
+
             # Labels
-            ax[0].grid(axis="x")
-            ax[0].set_xlabel("Time (seconds)")
+            ax[0].grid(axis='x')
+            ax[0].set_xlabel('Time (seconds)')
             axes[ax_enum, 0].set_ylabel(f'Order {ax_enum+1}\nOctaves (base 2 log)')
-            ax[1].grid(axis="x")
-            ax[1].set_xlabel("Frequency (Hz)")
-            ax[1].set_xscale("log")
-            axes[ax_enum, 0].text(-1*width_max, 0.2, 'Temporal\nWidth (s)', fontsize='small')
+            ax[1].grid(axis='x')
+            ax[1].set_xlabel('Frequency (Hz)')
+            ax[1].set_xscale('log')
+            axes[ax_enum, 0].text(-1 * width_max, 0.2, 'Temporal\nWidth (s)', fontsize='small')
             axes[ax_enum, 1].text(10**-2, 0.2, 'Centre\nFreq. (Hz)', fontsize='small')
 
             # Axes
             ax[1].set_ylim(-bank.octaves - 1, 1)
             ax[0].set_yticks(-np.arange(bank.octaves + 1))
             ax[0].set_yticklabels(np.arange(bank.octaves + 1))
             ax[0].set_yticks(-np.arange(bank.octaves + 1))
             ax[0].set_yticklabels(np.arange(bank.octaves + 1))
-            ax[1].tick_params(axis="y", left=False, labelleft=False)
-
+            ax[1].tick_params(axis='y', left=False, labelleft=False)
 
         # Legend
-        axes[1][0].legend([r"Re $\varphi(t)$", r"Im $\varphi(t)$"], loc=1)
-        axes[1][1].legend([r"$\hat\varphi(\omega)$"], loc=1)
+        axes[1][0].legend([r'Re $\varphi(t)$', r'Im $\varphi(t)$'], loc=1)
+        axes[1][1].legend([r'$\hat\varphi(\omega)$'], loc=1)
 
         plt.suptitle('ScatCluster Parametrization'
-                    f'\nSegment:{self.network_segment}s  Step: {self.network_step}\n Banks: {self.network_banks_name}')
-        plt.subplots_adjust(top=0.9) 
+                     f'\nSegment:{self.network_segment}s  Step: {self.network_step}\n Banks: {self.network_banks_name}')
+        plt.subplots_adjust(top=0.9)
         if savefig:
             plt.savefig(f'{self.data_savepath}figures/{self.data_network}_{self.data_station}_{self.data_location}_'
                         f'{self.network_name}_filter_banks.png')
 
     def load_sample_data(self) -> Stream:
         """Load sample
         """
@@ -282,15 +283,15 @@
                 self.sample_data = np.array([trace.data for trace in self.sample_stream])
                 self.channel_list = [trace.stats.channel for trace in self.sample_stream]
 
             times = self.sample_times
             data = self.sample_data
             channel_list = self.channel_list
         else:
-            if self.data_all is None:
+            if self.data_all is None:  # pylint: disable=access-member-before-definition
                 self.data_stream = self.load_data(starttime=UTCDateTime(self.data_starttime),
                                                   endtime=UTCDateTime(self.data_endtime),
                                                   channel=self.data_channel)
                 self.data_times = self.data_stream[0].times('matplotlib')
                 self.data_all = np.array([trace.data for trace in self.data_stream])
                 self.channel_list = [trace.stats.channel for trace in self.data_stream]
             times = self.data_times
@@ -347,17 +348,17 @@
                     scattering_coefficients = self.net.transform(data_segments, self.reduce_type())
 
                     # SAVE SCATTERING COEFFICIENTS IN NPZ FILE
                     np.savez(scatterings_path,
                              scat_coef_0=scattering_coefficients[0],
                              scat_coef_1=scattering_coefficients[1],
                              times=times_scat)
-                    
+
                     # print stats
-                    print(f">>> min {data.min()} : max {data.max()} : mean {data.mean()}")
+                    print(f'>>> min {data.min()} : max {data.max()} : mean {data.mean()}')
 
     def process_scatcluster_for_range(self) -> None:
         """Process scatcluster_yyyy_mm_dd for range of YYYY-MM-DDs
         """
         self.build_day_list()
         if len(self.data_day_list) > 0:
             print(f'The following days will be excluded from the analysis: {self.data_exclude_days}')
@@ -365,24 +366,22 @@
         for day_start, day_end in zip(
                 pd.date_range(
                     UTCDateTime(self.data_starttime).strftime('%Y%m%d'),
                     (UTCDateTime(self.data_endtime) - (60 * 60 * 24)).strftime('%Y%m%d')).strftime('%Y-%m-%d').tolist(),
                 pd.date_range((UTCDateTime(self.data_starttime) + (60 * 60 * 24)).strftime('%Y%m%d'),
                               UTCDateTime(self.data_endtime).strftime('%Y%m%d')).strftime('%Y-%m-%d').tolist()):
             self.process_scatcluster_yyyy_mm_dd(day_start, day_end)
-            
-            
+
     def filters_per_layer(self, model):
         """Get the number of filters per layer."""
         center_frequencies = [bank.centers for bank in model.banks]
         return [len(centers) for centers in center_frequencies]
 
-
     def layer_shape(self, model, order):
-        return self.filters_per_layer(model)[: order + 1]
+        return self.filters_per_layer(model)[:order + 1]
 
     def log(self, dataset, waterlevel=1e-10):
         """Get the log of the scattering coefficients.
 
         Parameters
         ----------
         dataset : xarray.Dataset
@@ -392,24 +391,23 @@
 
         Returns
         -------
         xarray.Dataset
             The scattering coefficients in the xarray.Dataset format.
         """
         # Select where order 1 is non-zero for all channels and frequencies
-        select = (dataset.order_1 > waterlevel).all(dim=["channel", "f1"])
+        select = (dataset.order_1 > waterlevel).all(dim=['channel', 'f1'])
         dataset = dataset.sel(time=select)
 
         # Get the log
         dataset.order_1.values = np.log10(dataset.order_1.values + waterlevel)
         dataset.order_2.values = np.log10(dataset.order_2.values + waterlevel)
 
         return dataset
 
-
     def nyquist_mask(self, dataset):
         """Mask the scattering coefficients with a Nyquist frequency.
 
         The scattering coefficients of order 2 are masked when the frequency
         f2 is greater than the frequency f1 to avoid aliasing.
 
         Parameters
@@ -419,49 +417,46 @@
 
         Returns
         -------
         xarray.Dataset
             The scattering coefficients in the xarray.Dataset format.
         """
         # Mask order 2 when f2 > f1
-        dataset.order_2.data = dataset.order_2.where(
-            dataset.f1 >= dataset.f2, np.nan
-        )
+        dataset.order_2.data = dataset.order_2.where(dataset.f1 >= dataset.f2, np.nan)
 
         # Drop NaN values
-        dataset = dataset.dropna(dim="time", how="all")
+        dataset = dataset.dropna(dim='time', how='all')
 
         return dataset
 
-
     def normalize(self, dataset):
         """Normalize the scattering coefficients.
 
         Parameters
         ----------
         dataset : xarray.Dataset
             The scattering coefficients in the xarray.Dataset format.
 
         Returns
         -------
         xarray.Dataset
             The scattering coefficients in the xarray.Dataset format.
         """
         # Working dimensions for normalization
-        order_1_dim = ["time", "f1", "channel"]
-        order_2_dim = ["time", "f1", "f2", "channel"]
+        order_1_dim = ['time', 'f1', 'channel']
+        order_2_dim = ['time', 'f1', 'f2', 'channel']
 
         # Normalize
         dataset.order_1.data -= dataset.order_1.mean(dim=order_1_dim).data
         dataset.order_1.data /= dataset.order_1.std(dim=order_1_dim).data
         dataset.order_2.data -= dataset.order_2.mean(dim=order_2_dim).data
         dataset.order_2.data /= dataset.order_2.std(dim=order_2_dim).data
 
-        return dataset            
-            
+        return dataset
+
     def process_vectorized_scattering_coefficients(self) -> None:
         """
         Process the vectorized scattering coefficients by loading data from files, reshaping the coefficients,
         standardizing in log space, and vectorizing them. Display statistics from the vectorization and store the
         processed data.
 
         Parameters:
@@ -485,76 +480,74 @@
         times = np.hstack(TIMES)
         del TIMES
         scat_coef_0 = np.vstack(SC0)
         del SC0
         scat_coef_1 = np.vstack(SC1)
         del SC1
 
-        
-        
         n_samples = len(times)
+        if self.channel_list is None:
+            self.build_channel_list()
         n_channels = len(self.channel_list)
-        
-        attributes = {k:str(v) for k,v in self.__dict__.items()}
+
+        attributes = {k: str(v) for k, v in self.__dict__.items()}
 
         # The coordinates of the xarray dataset are the center frequencies of the
         # scattering network, the starttime of the waveforms, and the channel names.
         center_frequencies = [bank.centers for bank in self.net.banks]
         coordinates = {
-                "time": ("time", times),
-                "channel": ("channel", self.channel_list),
-                **{
-                    f"f{i + 1}": (f"f{i + 1}", centers)
-                    for i, centers in enumerate(center_frequencies)
-                },
-            }
+            'time': ('time', times),
+            'channel': ('channel', self.channel_list),
+            **{
+                f'f{i + 1}': (f'f{i + 1}', centers)
+                for i, centers in enumerate(center_frequencies)
+            },
+        }
         # We now fill the data variables of the xarray dataset. The data variables
         # are the scattering coefficients for each order.
-        variables = dict()
+        variables = {}
         for order in range(len(self.net)):
             # Variable dimensions
             dimension = (
-                "time",
-                "channel",
-                *[f"f{j + 1}" for j in range(order + 1)],
+                'time',
+                'channel',
+                *[f'f{j + 1}' for j in range(order + 1)],
             )
 
             # Initialize and fill scattering matrix with scattering coefficients
-            variable = np.zeros(
-                (n_samples, n_channels, *self.layer_shape(self.net, order))
-            )
+            variable = np.zeros((n_samples, n_channels, *self.layer_shape(self.net, order)))
 
-            for time_stamp in tqdm(range(n_samples), desc=f"Xarray order {order + 1}"):
+            for time_stamp in tqdm(range(n_samples), desc=f'Xarray order {order + 1}'):
                 if order == 0:
                     x = np.abs(scat_coef_0[time_stamp])
                 elif order == 1:
                     x = np.abs(scat_coef_1[time_stamp])
                 for channel in range(n_channels):
                     variable[time_stamp, channel] = x[order][channel]
 
             # Assign scattering matrix to data variable
-            variables[f"order_{order + 1}"] = (dimension, variable)
+            variables[f'order_{order + 1}'] = (dimension, variable)
 
         # Assign attributes and data variables to dataset
         coefficients = xr.Dataset(
             coords=coordinates,
             data_vars=variables,
             attrs=attributes,
         )
 
         # Drop empty channels (where transform_waveform returned None)
         coefficients = coefficients.where(
-            coefficients.order_1.sum(dim=("f1", "channel")) > 0,
+            coefficients.order_1.sum(dim=('f1', 'channel')) > 0,
             drop=True,
         )
         coefficients = self.log(coefficients, waterlevel=1e-20)
         coefficients = self.nyquist_mask(coefficients)
         coefficients = self.normalize(coefficients)
         print(coefficients)
-        
+
         # Extract design matrix
         n_samples = coefficients.time.shape[0]
         x1 = coefficients.order_1.data.reshape(n_samples, -1)
         x2 = coefficients.order_2.data.reshape(n_samples, -1)
         x = np.hstack((x1, x2))
 
         # Remove NaNs
@@ -572,30 +565,32 @@
         # Store Data
         np.save(
             f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
             f'{self.network_name}_times.npy', self.data_times)
         np.save(
             f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
             f'{self.network_name}_scat_coef_vectorized.npy', self.data_scat_coef_vectorized)
-        coefficients.to_netcdf(
-            f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
-            f'{self.network_name}_scat_coef_xarray.nc')
-        
+        coefficients.to_netcdf(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
+                               f'{self.network_name}_scat_coef_xarray.nc')
+
+        return coefficients
+
     def load_scattering_coefficients_xarray(self):
         """
-        Load the scattering coefficients from an xarray dataset file and store them in the `scattering_coefficients_xarray` attribute.
+        Load the scattering coefficients from an xarray dataset file and store them in the
+        `scattering_coefficients_xarray` attribute.
 
         Returns:
             xr.Dataset: The loaded scattering coefficients dataset.
         """
-        scat_coeff_xr = xr.open_dataset(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
-                                        f'{self.network_name}_scat_coef_xarray.nc')
+        scat_coeff_xr = xr.open_dataset(
+            f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
+            f'{self.network_name}_scat_coef_xarray.nc')
         self.scattering_coefficients_xarray = scat_coeff_xr
-        return scat_coeff_xr 
-        
+        return scat_coeff_xr
 
     def preload_times(self):
         """
         Preloads the times data from a numpy file and assigns it to the `data_times` attribute of the class.
 
         """
         data_times = np.load(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
```

### Comparing `scatcluster-0.0.74/scatcluster/scatcluster.py` & `scatcluster-0.0.75/scatcluster/scatcluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 class ScatCluster(Structure, Scattering, ICA, Dendrogram, Waveforms, Predictions, ExternalCorrelation,
                   WaveformCorrelations, AnalysisProcessing):
     """
     INGV ScatCluster class workflow for clustering continuous time series with a deep scattering network.
     """
 
-    def __init__(
+    def __init__(  # pylint: disable=dangerous-default-value
             self,
             data_savepath: str,
             data_client_path: str,
             data_network: str,
             data_station: str,
             data_location: str,
             data_channel: str,
@@ -70,15 +70,15 @@
             ica_max_ICAs: int = 10,
             ica_overwrite_previous_models: bool = False,
             ica_explained_variance_score: float = None,  # pylint: disable=unused-argument
             dendrogram_method: str = 'ward',
             dendrogram_time_zone: str = None,  # pylint: disable=unused-argument
             waveforms_n_samples: int = 5,
             waveforms=None,  # pylint: disable=unused-argument
-            spectrograms=None, # pylint: disable=unused-argument
+            spectrograms=None,  # pylint: disable=unused-argument
             scattering_coefficients_xarray=None):  # pylint: disable=unused-argument
         """
         Initializes a ScatCluster instance.
 
         Args:
             data_savepath (str): The path to save data.
             data_client_path (str): The path to the client data.
```

### Comparing `scatcluster-0.0.74/scatcluster/structure.py` & `scatcluster-0.0.75/scatcluster/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # scatcluster/structure.py
 import json
 import os
 from glob import glob
 from typing import List, Optional
-from glob import glob
+
 
 class Structure:
 
     def prepare_directory_structure(self, directories: Optional[List[str]] = None) -> None:
         """Build directory structure required for workflow processing
 
         Args:
@@ -126,23 +126,19 @@
          are the instance variables of the object.
 
         Parameters:
             self (object): The object whose attributes are to be printed.
 
         """
         print(self.__dict__)
-        
+
     def list_available_configurations(self):
         """
         Lists all the available configurations in the config directory.
 
         This function uses the `glob` function to find all the JSON files in the config directory.
         It prints the list of JSON files found.
 
         Parameters:
             self (object): The instance of the class.
-
-        Returns:
-            None
         """
         print(glob(f'{self.data_savepath}config/*json'))
-
```

### Comparing `scatcluster-0.0.74/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.75/scatcluster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.74
+Version: 0.0.75
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.74/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.75/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.74/setup.py` & `scatcluster-0.0.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.74',
+    version='0.0.75',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

