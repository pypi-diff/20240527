# Comparing `tmp/scatcluster-0.0.65.tar.gz` & `tmp/scatcluster-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.65.tar", last modified: Mon May 27 17:53:32 2024, max compression
+gzip compressed data, was "scatcluster-0.0.66.tar", last modified: Mon May 27 19:51:37 2024, max compression
```

## Comparing `scatcluster-0.0.65.tar` & `scatcluster-0.0.66.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 17:53:29.000000 scatcluster-0.0.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 17:53:29.000000 scatcluster-0.0.65/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 17:53:32.587445 scatcluster-0.0.65/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.583445 scatcluster-0.0.65/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    24705 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 17:53:29.000000 scatcluster-0.0.65/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:53:32.587445 scatcluster-0.0.65/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 17:53:32.000000 scatcluster-0.0.65/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:53:32.587445 scatcluster-0.0.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 17:53:29.000000 scatcluster-0.0.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-27 19:51:34.000000 scatcluster-0.0.66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 19:51:34.000000 scatcluster-0.0.66/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 19:51:37.793326 scatcluster-0.0.66/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.789326 scatcluster-0.0.66/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-27 19:51:34.000000 scatcluster-0.0.66/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:51:37.793326 scatcluster-0.0.66/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 19:51:37.000000 scatcluster-0.0.66/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:51:37.793326 scatcluster-0.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 19:51:34.000000 scatcluster-0.0.66/setup.py
```

### Comparing `scatcluster-0.0.65/LICENSE` & `scatcluster-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/PKG-INFO` & `scatcluster-0.0.66/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.65
+Version: 0.0.66
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.65/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.66/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.66/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.66/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/analysis/predictions.py` & `scatcluster-0.0.66/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/analysis/processing.py` & `scatcluster-0.0.66/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.66/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.66/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/helper.py` & `scatcluster-0.0.66/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/processing/ica.py` & `scatcluster-0.0.66/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/processing/scattering.py` & `scatcluster-0.0.66/scatcluster/processing/scattering.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import scipy as sp
 from matplotlib import dates as mdates
 from obspy.clients.filesystem.sds import Client
 from obspy.core import UTCDateTime
 from obspy.core.stream import Stream
 from scatseisnet.network import ScatteringNetwork
 from scatseisnet.operation import segmentize
-
-from scatcluster.helper import is_gpu_available
+import cupy as cp
 import xarray as xr
 from tqdm import tqdm
 
 
 class Scattering:
 
     def reduce_type(self):
@@ -135,57 +134,79 @@
 
     def plot_network_filter_banks(self) -> None:
         """
         Plot the filter banks
         """
         NROWS = len(self.net.banks)
         # Crete axes
-        _, ax = plt.subplots(NROWS, 2, sharey='row', figsize=(10, 8))
+        octaves = [bank.octaves for bank in self.net.banks]
+        height_ratios = 2, (octaves[1] + 2) / (octaves[0] + 2)
+        grid = dict(height_ratios=height_ratios, wspace=0.1, hspace=0.1)
+        _, axes = plt.subplots(NROWS, 2, figsize=(10, 12), gridspec_kw=grid, sharey="row"
+        )
         # Loop over network layers
-        for bank_enum, bank in enumerate(self.net.banks):
-            if is_gpu_available():
+        for ax_enum, (ax, bank) in enumerate(zip(axes, self.net.banks)):
+            # Limit view to three times the temporal width of largest wavelet
+            width_max = min(2 * bank.widths.max(), bank.times.max())
+            if type(bank.wavelets) == cp.ndarray:
                 bank.wavelets = bank.wavelets.get()
+            if type(bank.spectra) == cp.ndarray:
                 bank.spectra = bank.spectra.get()
-                # bank.ratios = bank.ratios.get()
-                # bank.widths = bank.widths.get()
-                # bank.centers = bank.centers.get()
-                # bank.times = bank.times.get()
-                # bank.frequencies = bank.frequencies.get()
-
-            # Limit view to three times the temporal width of largest wavelet
-            width_max_label = -1 * min(2.5 * bank.widths.max(), bank.times.max())
-
-            # Show each wavelet
-
-            iterable = zip(bank.wavelets, bank.spectra, bank.ratios, bank.widths, bank.centers)
-            for wavelet, spectrum, ratio, width, center in iterable:
-
-                # Time domain
-                ax[bank_enum, 0].plot(bank.times, wavelet.real + ratio, 'C0')
-                ax[bank_enum, 0].text(width_max_label, ratio, f'{width*4:.2f}', fontsize='small')
-
-                # Spectral domain
-                ax[bank_enum, 1].plot(bank.frequencies, np.log(np.abs(spectrum) + 1) + ratio, 'C0')
-                ax[bank_enum, 1].text(0.001, ratio, f'{center:.2f}', fontsize='small')
-
-            # Limit view to three times the temporal width of largest wavelet
-            width_max = min(3 * bank.widths.max(), bank.times.max())
-
+            if type(bank.widths) == cp.ndarray:
+                bank.widths = bank.widths.get()
+            if type(bank.centers) == cp.ndarray:
+                bank.centers = bank.centers.get()        
+
+            # Temporal
+            for octave_enum, (wavelet, octave, width) in enumerate(zip(bank.wavelets, bank.ratios, bank.widths)):
+                # Truncate time for small-duration wavelets
+                inner = np.abs(bank.times) < width_max
+                t = bank.times[inner]
+                y = wavelet[inner] / np.abs(wavelet[inner].max()) / 3
+                ax[0].plot(t, y.real + octave, color="C0", zorder=1)
+                ax[0].plot(t, y.imag + octave, color="C0", zorder=0, alpha=0.4)
+                ax[0].text(-1*width_max*(1 if octave_enum%2==0 else 1.1), octave, f'{width*4:.2f}', fontsize='small')
+
+            # Spectral
+            sepctra = bank.spectra
+            frequencies = bank.frequencies
+            for octave_enum, (spectrum, octave, center) in enumerate(zip(bank.spectra, bank.ratios, bank.centers)):
+                inner = frequencies > frequencies[1]
+                f = frequencies[inner]
+                y = spectrum[inner]
+                y /= np.abs(y.max())
+                ax[1].plot(f, np.abs(y) + octave, color="C0")
+                ax[1].text((10**-2)*(1 if octave_enum%2==0 else 1.1), octave, f'{center:.2f}', fontsize='small')
+            
             # Labels
-            ax[bank_enum, 0].set_ylabel(f'Order {bank_enum+1}\nOctaves (base 2 log)')
-            ax[bank_enum, 0].set_xlabel('Time (seconds)')
-            ax[bank_enum, 0].set_xlim(-width_max, width_max)
-            ax[bank_enum, 1].set_xscale('log')
-            ax[bank_enum, 1].set_xlabel('Frequency (Hz)')
-
-            ax[bank_enum, 0].text(width_max_label, 0, 'Temporal Width (s)', fontsize='small')
-            ax[bank_enum, 1].text(0.001, 0, 'Centre Freq. (Hz)', fontsize='small')
-        plt.suptitle(f'scatcluster parametrization for Segment {self.network_segment}: Step {self.network_step}: Banks '
-                     f'{self.network_banks_name}')
-
+            ax[0].grid(axis="x")
+            ax[0].set_xlabel("Time (seconds)")
+            axes[ax_enum, 0].set_ylabel(f'Order {ax_enum+1}\nOctaves (base 2 log)')
+            ax[1].grid(axis="x")
+            ax[1].set_xlabel("Frequency (Hz)")
+            ax[1].set_xscale("log")
+            axes[ax_enum, 0].text(-1*width_max, 0.2, 'Temporal\nWidth (s)', fontsize='small')
+            axes[ax_enum, 1].text(10**-2, 0.2, 'Centre\nFreq. (Hz)', fontsize='small')
+
+            # Axes
+            ax[1].set_ylim(-bank.octaves - 1, 1)
+            ax[0].set_yticks(-np.arange(bank.octaves + 1))
+            ax[0].set_yticklabels(np.arange(bank.octaves + 1))
+            ax[0].set_yticks(-np.arange(bank.octaves + 1))
+            ax[0].set_yticklabels(np.arange(bank.octaves + 1))
+            ax[1].tick_params(axis="y", left=False, labelleft=False)
+
+
+        # Legend
+        axes[1][0].legend([r"Re $\varphi(t)$", r"Im $\varphi(t)$"], loc=1)
+        axes[1][1].legend([r"$\hat\varphi(\omega)$"], loc=1)
+
+        plt.suptitle('ScatCluster Parametrization'
+                    f'\nSegment:{self.network_segment}s  Step: {self.network_step}\n Banks: {self.network_banks_name}')
+        plt.subplots_adjust(top=0.9) 
         plt.savefig(f'{self.data_savepath}figures/{self.data_network}_{self.data_station}_{self.data_location}_'
                     f'{self.network_name}_filter_banks.png')
 
     def load_sample_data(self) -> Stream:
         """Load sample
         """
         return self.load_data(starttime=UTCDateTime(self.data_sample_starttime),
@@ -564,10 +585,10 @@
 
     def load_scat_coef_vectorized(self):
         if not hasattr(self, 'scat_coef_vectorized'):
             self.scat_coef_vectorized = np.load(
                 f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
                 f'{self.network_name}_scat_coef_vectorized.npy')
         else:
-            print('SC.scat_coef_vectorized already exist')
+            print('self.scat_coef_vectorized already exist')
 
         return self.scat_coef_vectorized
```

### Comparing `scatcluster-0.0.65/scatcluster/scatcluster.py` & `scatcluster-0.0.66/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster/structure.py` & `scatcluster-0.0.66/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.66/scatcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.65
+Version: 0.0.66
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.65/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.66/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.65/setup.py` & `scatcluster-0.0.66/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.65',
+    version='0.0.66',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

