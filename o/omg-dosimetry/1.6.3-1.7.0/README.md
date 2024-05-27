# Comparing `tmp/omg_dosimetry-1.6.3.tar.gz` & `tmp/omg_dosimetry-1.7.0.tar.gz`

## Comparing `omg_dosimetry-1.6.3.tar` & `omg_dosimetry-1.7.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/.readthedocs.yml
--rw-r--r--   0        0        0     7672 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/OMG.yaml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/requirements_pip.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/requirements_read_the_docs.txt
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/make.bat
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/source/analysis.rst
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/source/calibration.rst
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/source/conf.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/source/index.rst
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/source/installation.rst
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/docs/source/tiff2dose.rst
--rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/src/omg_dosimetry/OMG_Logo.png
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/src/omg_dosimetry/__init__.py
--rw-r--r--   0        0        0    60332 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/src/omg_dosimetry/analysis.py
--rw-r--r--   0        0        0    41301 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/src/omg_dosimetry/calibration.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/src/omg_dosimetry/i_o.py
--rw-r--r--   0        0        0    40888 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/src/omg_dosimetry/imageRGB.py
--rw-r--r--   0        0        0    24784 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/src/omg_dosimetry/tiff2dose.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/LICENSE
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/README.rst
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 omg_dosimetry-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0     7672 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/OMG.yaml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/requirements_pip.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/requirements_read_the_docs.txt
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/make.bat
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/source/analysis.rst
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/source/calibration.rst
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/docs/source/tiff2dose.rst
+-rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/OMG_Logo.png
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/__init__.py
+-rw-r--r--   0        0        0    71379 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/analysis.py
+-rw-r--r--   0        0        0    41310 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/calibration.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/i_o.py
+-rw-r--r--   0        0        0    43666 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/imageRGB.py
+-rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/tiff2dose.py
+-rw-r--r--   0        0        0    19022 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/src/omg_dosimetry/tools.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/LICENSE
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/README.rst
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 omg_dosimetry-1.7.0/PKG-INFO
```

### Comparing `omg_dosimetry-1.6.3/.readthedocs.yml` & `omg_dosimetry-1.7.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/OMG.yaml` & `omg_dosimetry-1.7.0/OMG.yaml`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/.github/workflows/publish-to-test-pypi.yml` & `omg_dosimetry-1.7.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/docs/Makefile` & `omg_dosimetry-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/docs/make.bat` & `omg_dosimetry-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/docs/source/calibration.rst` & `omg_dosimetry-1.7.0/docs/source/calibration.rst`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/docs/source/conf.py` & `omg_dosimetry-1.7.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'OMG dosimetry'
 copyright = '2023, Jean-François Cabana and Luis Alfonso Olivares Jiménez'
 author = 'Jean-François Cabana, Luis Alfonso Olivares Jiménez and Peter Truong'
 
 # The short X.Y version.
-version = "1.6"
+version = "1.7"
 # The full version, including alpha/beta/rc tags.
-release = "1.6.3"
+release = "1.7.0"
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx_contributors',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
```

### Comparing `omg_dosimetry-1.6.3/docs/source/installation.rst` & `omg_dosimetry-1.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/docs/source/tiff2dose.rst` & `omg_dosimetry-1.7.0/docs/source/tiff2dose.rst`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/src/omg_dosimetry/OMG_Logo.png` & `omg_dosimetry-1.7.0/src/omg_dosimetry/OMG_Logo.png`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/src/omg_dosimetry/analysis.py` & `omg_dosimetry-1.7.0/src/omg_dosimetry/analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     - Gamma analysis: display gamma map, pass rate, histogram, pass rate vs dose bar graph,
       pass rate vs distance to agreement (fixed dose to agreement),
       pass rate vs dose to agreement (fixed distance to agreement)
     - Publish PDF report
     
 Written by Jean-Francois Cabana, copyright 2018
 Modified by Peter Truong (CISSSO)
-Version: 2023-12-15
+Version: 2024-05-21
 """
 
 import numpy as np
 import scipy.ndimage.filters as spf
 import copy
 import matplotlib.pyplot as plt
 import os
@@ -31,14 +31,15 @@
 from pathlib import Path
 import pymedphys
 from matplotlib.widgets  import RectangleSelector, MultiCursor, Cursor
 import webbrowser
 from .imageRGB import load, ArrayImage, equate_images
 import bz2
 import time
+from .tools import Ruler
 
 class DoseAnalysis(): 
     """Base class for analysis film dose vs reference dose.
 
     Usage : film = analysis.DoseAnalysis(film_dose=file_doseFilm, ref_dose=ref_dose)
 
     Attributes
@@ -134,15 +135,15 @@
         print("Computing normalisation factor from doses > {} cGy.".format(norm_isodose))
         self.norm_dose = norm_isodose        
         indices = np.where(self.ref_dose.array > self.norm_dose)
         mean_ref = np.mean(self.ref_dose.array[indices])
         mean_film = np.mean(self.film_dose.array[indices])          
         self.apply_film_factor(film_dose_factor = mean_ref / mean_film )
         
-    def apply_factor_from_roi(self, norm_dose = None):
+    def apply_factor_from_roi(self, norm_dose=None, apply=True):
         """ Apply film normalisation factor from a rectangle ROI.
             Brings up an interactive plot, where the user must define a rectangle ROI
             that will be used to compute a film normalisation factor.
             Median dose inside this rectangle will be used to scale the film dose to match
             that of the reference.
         """
         
@@ -151,39 +152,48 @@
         self.roi_xmin, self.roi_xmax = [], []
         self.roi_ymin, self.roi_ymax = [], []
 
         self.fig = plt.figure()
         ax = plt.gca()  
         if self.norm_film_dose:
             self.norm_film_dose.plot(ax=ax)  
-            ax.plot((0,self.norm_film_dose.shape[1]),(self.norm_film_dose.center.y,self.norm_film_dose.center.y),'k--')
-            ax.set_xlim(0, self.norm_film_dose.shape[1])
-            ax.set_ylim(self.norm_film_dose.shape[0],0)
         else:
             self.film_dose.plot(ax=ax)  
-            ax.plot((0,self.film_dose.shape[1]),(self.film_dose.center.y,self.film_dose.center.y),'k--')
-            ax.set_xlim(0, self.film_dose.shape[1])
-            ax.set_ylim(self.film_dose.shape[0],0)
         ax.set_title(msg)
         print(msg)
         
         def select_box(eclick, erelease):
             x1, y1 = int(eclick.xdata), int(eclick.ydata)
             x2, y2 = int(erelease.xdata), int(erelease.ydata)
             self.roi_xmin, self.roi_xmax = min(x1,x2), max(x1,x2)
             self.roi_ymin, self.roi_ymax = min(y1,y2), max(y1,y2)
         
         self.rs = RectangleSelector(ax, select_box, useblit=True, button=[1], minspanx=5, minspany=5, spancoords='pixels', interactive=True)  
-        self.cid = self.fig.canvas.mpl_connect('key_press_event', self.apply_factor_from_roi_press_enter)
+        if apply: self.cid = self.fig.canvas.mpl_connect('key_press_event', self.apply_factor_from_roi_press_enter)
+        else: self.cid = self.fig.canvas.mpl_connect('key_press_event', self.get_factor_from_roi_press_enter)
         
         self.wait = True
         while self.wait: plt.pause(1)
         plt.close(self.fig)
         return
 
+    def get_factor_from_roi_press_enter(self, event):
+        """ Function called from apply_factor_from_roi() when ''enter'' is pressed. """      
+        if event.key == 'enter':
+            roi_film = np.median(self.film_dose.array[self.roi_ymin:self.roi_ymax, self.roi_xmin:self.roi_xmax])
+            roi_ref = np.median(self.ref_dose.array[self.roi_ymin:self.roi_ymax, self.roi_xmin:self.roi_xmax])
+            relative_diff = (roi_film-roi_ref)/roi_ref * 100
+            print("Median film dose = {} cGy; median ref dose = {} cGy; Relative diff = {}%".format(roi_film, roi_ref, relative_diff))
+            
+            if hasattr(self, "rs"): del self.rs                
+            self.fig.canvas.mpl_disconnect(self.cid)
+            self.wait = False
+            self.roi_relative_diff = relative_diff
+            return
+
     def apply_factor_from_roi_press_enter(self, event):
         """ Function called from apply_factor_from_roi() when ''enter'' is pressed. """      
         if event.key == 'enter':
             if self.norm_film_dose: roi_film = np.median(self.norm_film_dose.array[self.roi_ymin:self.roi_ymax, self.roi_xmin:self.roi_xmax])
             else: roi_film = np.median(self.film_dose.array[self.roi_ymin:self.roi_ymax, self.roi_xmin:self.roi_xmax])
             
             if self.norm_dose is None:  # If no normalisation dose is given, assume we normalisation on ref_dose
@@ -556,15 +566,15 @@
         
         ax.bar(bins[:-1], dose_pass_rel, width=bin_size,  align='edge', linewidth=1, edgecolor='k')
         ax.set_xlabel('Doses (cGy)')
         ax.set_ylabel('Pass rate (%)')
         ax.set_title("Gamma pass rate vs dose")
         ax.set_xticks(bins)
         
-    def plot_gamma_stats(self, figsize=(10, 10), show_hist=True, show_pass_hist=True, show_varDistTA=True, show_varDoseTA=True):
+    def show_gamma_stats(self, figsize=(10, 10), show_hist=True, show_pass_hist=True, show_varDistTA=False, show_varDoseTA=False):
         """ Displays a figure with 4 subplots showing gamma analysis statistics:
             1- Gamma map histogram, 
             2- Gamma pass rate vs dose histogram
             3- Gamma pass rate vs variable distance to agreement threshold
             4- Gamma pass rate vs variable dose to agreement threshold
         """
 
@@ -581,15 +591,15 @@
             i=i+1
         if show_varDistTA:
             self.plot_gamma_varDistTA(ax=axes[i])
             i=i+1
         if show_varDoseTA:
             self.plot_gamma_varDoseTA(ax=axes[i])
         
-    def plot_profile(self, ax=None, profile='x', position=None, title=None, diff=False, offset=0):
+    def plot_profile(self, ax=None, profile='x', position=None, title=None, diff=False, offset=0, vertical_line=None, xlim=None, ylim='auto'):
         """ Plot a line profile of reference dose and film dose at a given position.
 
             Parameters
             ----------
             ax : matplotlib.pyplot axe object, optional
                 Axis in which to plot the graph.
                 If None, a new plot is made.
@@ -615,50 +625,84 @@
                 Default is False
 
             offset : int, optional
                 If a known offset exists between the film and the reference dose, the plotted profile can be shifted
                 to account for this offset. For example, a film exposed at a fixed gantry angle coud have a known 
                 offset due to gantry sag, and you could want to correct for it on the profile.
                 Default is 0 mm
+                
+            vertical_line : int, optional
+                If set to True, a dashed vertical line is plotted on the profile at this position
+                
+            xlim : tuple, optional
+                If given, xlim will be passed to ax.set_xlim(xlim) to set the x axis limits
+                
+            ylim : tuple, 'max' or 'auto' (default), optional
+                If given a tuple, ylim will be passed to ax.set_ylim(ylim) to set the y axis limits
+                If 'max', ylim goes from 0 to 105% of maximum reference dose
+                If 'auto', ylim goes from 0 to 105% of maximum of either the current reference or film dose profile.
         """        
 
         film, ref = self.film_dose.array, self.ref_dose.array
-        v_ligne = None
-        if position is None: position = [np.floor(self.ref_dose.shape[1] / 2).astype(int), 
-                                         np.floor(self.ref_dose.shape[0] / 2).astype(int)]
+
         if profile == 'x':
-            film_prof, ref_prof = film[position[1],:], ref[position[1],:] 
-            v_ligne = position[0] / self.film_dose.dpmm
+            if position is None: position = int(self.film_dose.center.y)
+            film_prof, ref_prof = film[position,:], ref[position,:] 
         elif profile == 'y':
-            film_prof, ref_prof = film[:,position[0]], ref[:,position[0]]
-            v_ligne = position[1] / self.film_dose.dpmm        
+            if position is None: position = int(self.film_dose.center.x)
+            film_prof, ref_prof = film[:,position], ref[:,position]
         
         x_axis = (np.array(range(0, len(film_prof))) / self.film_dose.dpmm).tolist()
-        y_max = max(np.concatenate((film_prof, ref_prof)))
         
         if ax is None: fig, ax = plt.subplots()    
         ax.clear()
         ax.plot([i+offset for i in x_axis], film_prof,'r-', linewidth=2)
         ax.plot(x_axis, ref_prof,'b--', linewidth=2)
-        if v_ligne: ax.plot((v_ligne, v_ligne), (0, y_max * 1.10), 'k:', linewidth = 1)
         
         if title is None:
-            if profile == 'x': title='Horizontal Profile (y = {} mm)'.format(int(position[1] / self.film_dose.dpmm))
-            if profile == 'y': title='Vertical Profile (x = {} mm)'.format(int(position[0] / self.film_dose.dpmm))
+            if profile == 'x': title='Horizontal Profile (y = {} mm)'.format(int(position / self.film_dose.dpmm))
+            if profile == 'y': title='Vertical Profile (x = {} mm)'.format(int(position / self.film_dose.dpmm))
         ax.set_title(title)
         ax.set_xlabel('Position (mm)')
         ax.set_ylabel('Dose (cGy)')
         
         if diff:
             ax_diff = ax.twinx()
             diff_prof = film_prof - ref_prof
             ax_diff.set_ylabel("Difference (cGy)")
             ax_diff.plot(x_axis, diff_prof,'g-', linewidth=0.25)
+            
+        if xlim: ax.set_xlim(xlim)
+        if ylim == 'max': ax.set_ylim((0, self.ref_dose.array.max() * 1.05))
+        elif ylim == 'auto': ax.set_ylim((0, max(np.concatenate((film_prof, ref_prof))) * 1.05))
+        else: ax.set_ylim(ylim)
+            
+        if vertical_line:
+            ax.plot((vertical_line / self.film_dose.dpmm, vertical_line / self.film_dose.dpmm), 
+                    ax.get_ylim(), 'k:', linewidth = 1)
     
-    def show_results(self, fig=None, x=None, y=None, show = True):
+    def show_isodoses(self, ax=None, levels=None, colors=None, show_ruler=True, figsize=(15,15)):
+        if ax is None:
+            fig, ax = plt.subplots(figsize=figsize)
+        if levels is None:
+            d_max = self.ref_dose.array.max()
+            levels = [d_max * l for l in np.arange(0.2, 1.0, 0.2)]
+        if colors is None:
+            colors = plt.cm.tab10(np.linspace(0, 1, 10))
+        extent = [0, self.ref_dose.physical_shape[1], self.ref_dose.physical_shape[0], 0]
+        self.film_dose.plot_isodoses(ax=ax, levels=levels, colors=colors, linestyles='dashdot', linewidths=0.5, extent=extent, inline=False)
+        self.ref_dose.plot_isodoses(ax=ax, levels=levels, colors=colors, linestyles='solid', linewidths=0.5, labels=False, extent=extent)
+        legend_lines = [plt.Line2D([0], [0], linestyle='dotted', color='black', label='Film Dose'),
+                        plt.Line2D([0], [0], linestyle='solid', color='black', label='Reference Dose')]
+        plt.legend(handles=legend_lines)
+        ax.invert_yaxis()
+        if show_ruler:
+            self.ruler = add_ruler(ax)
+
+    def show_results(self, fig=None, x=None, y=None, show=True):
         """ Display an interactive figure showing the results of a gamma analysis.
             The figure contains 6 axis, which are, from left to right and top to bottom:
             Film dose, reference dose, gamma map, relative error, x profile and y profile.
             
             Parameters
             ----------
             fig : matplotlib.pyplot figure object, optional
@@ -673,48 +717,57 @@
         """
         a = None
         
         if x is None: self.prof_x = np.floor(self.ref_dose.shape[1] / 2).astype(int)
         elif x == 'max':
             a = np.unravel_index(self.ref_dose.array.argmax(), self.ref_dose.array.shape)
             self.prof_x = a[1]
+        else: self.prof_x = x
         if y is None: self.prof_y = np.floor(self.ref_dose.shape[0] / 2).astype(int)
         elif y == 'max':
             if a is None: a = np.unravel_index(self.ref_dose.array.argmax(), self.ref_dose.array.shape)
             self.prof_y = a[0]
+        else: self.prof_y = y
          
         fig, ((ax1,ax2),(ax3,ax4),(ax5,ax6)) = plt.subplots(3,2, figsize=(10, 8))
         fig.tight_layout()
         axes = [ax1,ax2,ax3,ax4,ax5,ax6]
         fig.canvas.manager.set_window_title("Facteur{:.2f}_Filtre{}_Gamma{}%-{}mm".format(self.film_dose_factor, self.film_filt, self.doseTA, self.distTA))
         
         max_dose_comp = np.percentile(self.ref_dose.array,[98])[0].round(decimals=-1)
         clim = [0, max_dose_comp]
 
-        self.film_dose.plotCB(ax1, clim=clim, title='Film Dose ({})'.format(os.path.basename(self.film_dose.path)))
-        self.ref_dose.plotCB(ax2, clim=clim, title='Reference Dose ({})'.format(os.path.basename(self.ref_dose.path)))
-        self.GammaMap.plotCB(ax3, clim=[0,2], cmap='bwr', title='Gamma Map ({:.2f}% Pass; {:.2f} Mean)'.format(self.GammaMap.passRate, self.GammaMap.mean))
+        self.film_dose.plot(ax1, clim=clim, title='Film Dose ({})'.format(os.path.basename(self.film_dose.path)), colorbar=True)
+        self.ref_dose.plot(ax2, clim=clim, title='Reference Dose ({})'.format(os.path.basename(self.ref_dose.path)), colorbar=True)
+        self.GammaMap.plot(ax3, clim=[0,2], cmap='bwr', title='Gamma Map ({:.2f}% Pass; {:.2f} Mean)'.format(self.GammaMap.passRate, self.GammaMap.mean), colorbar=True)
         ax3.set_facecolor('k')
         min_value = max(-20, np.percentile(self.DiffMap.array,[1])[0].round(decimals=0))
         max_value = min(20, np.percentile(self.DiffMap.array,[99])[0].round(decimals=0))
         clim = [min_value, max_value]    
-        self.RelError.plotCB(ax4, cmap='jet', clim=clim, title='Relative Error (%) (RMSE = {:.2f})'.format(self.DiffMap.RMSE))
+        self.RelError.plot(ax4, cmap='jet', clim=clim, title='Relative Error (%) (RMSE = {:.2f})'.format(self.DiffMap.RMSE), colorbar=True)
         self.show_profiles(axes, x=self.prof_x, y=self.prof_y)
         plt.multi = MultiCursor(None, (axes[0],axes[1],axes[2],axes[3]), color='r', lw=1, horizOn=True)
         
         fig.canvas.mpl_connect('button_press_event', lambda event: self.set_profile(event, axes))
+        fig.canvas.mpl_connect('key_press_event', self.show_results_ontype)
         if show: plt.show()
         
-    def show_profiles(self, axes, x, y):
+    def show_results_ontype(self, event):
+        if event.key == 'enter':
+            self.get_profile_offsets(x=self.prof_x, y=self.prof_y)
+        
+    def show_profiles(self, axes, x, y, figsize=(10,10)):
         """ This function is called by show_results and set_profile to draw dose profiles
             at a given x/y coordinates, and draw lines on the dose distribution maps
             to show where the profile is taken.
         """
-        self.plot_profile(ax=axes[-2], profile='x', position=[x, y])
-        self.plot_profile(ax=axes[-1], profile='y', position=[x, y])
+        ax_x = axes[-2]
+        ax_y = axes[-1]
+        self.plot_profile(ax=ax_x, profile='x', position=y, vertical_line=x)
+        self.plot_profile(ax=ax_y, profile='y', position=x, vertical_line=y)
         
         for i in range(0,4):
             ax = axes[i]
             while len(ax.lines) > 0: ax.lines[-1].remove()       # Remove prior crosshairs (if any)
             
             ### Plot crosshairs
             ax.plot((x,x),(0,self.ref_dose.shape[0]),'w--', linewidth=1)
@@ -731,14 +784,16 @@
             elif event.inaxes == axes[4]: self.prof_x = int(event.xdata * self.film_dose.dpmm)
             elif event.inaxes == axes[5]: self.prof_y = int(event.xdata * self.film_dose.dpmm)
             
             self.show_profiles(axes,x=self.prof_x, y=self.prof_y)    
             plt.gcf().canvas.draw_idle()
         else: print('\nZoom/pan is currently selected.\nNote: Unable to set profile when this tool is active.')
         
+        
+    #=================== Registration functions ======================
     def register(self, shift_x=0, shift_y=0, threshold=10, register_using_gradient=False, markers_center=None, rot=0):
         """ Starts the registration procedure between film and reference dose.
             
             Parameters
             ----------
             shift_x / shift_y : float, optional
             Apply a known shift [mm] in the x/y direction between reference dose and film dose. 
@@ -1077,45 +1132,62 @@
             self.show_registration(ax=ax)
             fig.canvas.draw_idle()
         if event.key == 'enter':
             self.fig.canvas.mpl_disconnect(self.cid)
             self.wait = False
             return
             
-    def save_analyzed_image(self, filename,  x=None, y=None, **kwargs):
+    def save_current_figure(self, filename, **kwargs):
         """Save the analyzed image to a file.
 
         Parameters
         ----------
         filename : str
             The location and filename to save to.
         kwargs
             Keyword arguments are passed to plt.savefig().
         """
-        self.show_results(x=x, y=y, **kwargs)
         fig = plt.gcf()
-        fig.savefig(filename)
+        fig.savefig(filename, **kwargs)
         plt.close(fig)
         
-    def save_analyzed_gamma(self, filename, **kwargs):
-        """Save the analyzed image to a file.
+    def show_cluster_analysis(self, cluster_id=0, xlim_margin_mm=10, figsize=(10,10), levels=None):
+        # Get coordinates of slected cluster
+        x = self.clusters_analysis[cluster_id]['x_px']
+        y = self.clusters_analysis[cluster_id]['y_px']
+        x_mm = self.clusters_analysis[cluster_id]['x_mm']
+        y_mm = self.clusters_analysis[cluster_id]['y_mm']
+    
+        coords = self.ref_dose.clusters[cluster_id]['coords']
+        coords_mm = coords / self.ref_dose.dpmm
+        x_xlim = (min(coords_mm[:,1])-xlim_margin_mm, max(coords_mm[:,1])+xlim_margin_mm)
+        y_xlim = (min(coords_mm[:,0])-xlim_margin_mm, max(coords_mm[:,0])+xlim_margin_mm)
+        
+        # Show full dose distribution and location of selected cluster
+        fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2,2, figsize=figsize)
+        extent = [0, self.ref_dose.physical_shape[1], self.ref_dose.physical_shape[0], 0]
+        self.ref_dose.plot(ax=ax1, extent=extent)
+        ax1.plot((x_mm, x_mm),(0,self.ref_dose.shape[0]),'w--', linewidth=1)
+        ax1.plot((0, self.ref_dose.shape[1]),(y_mm, y_mm),'w--', linewidth=1)
+        
+        rect = plt.Rectangle((min(x_xlim[0], x_xlim[1]), min(y_xlim[0], y_xlim[1])), abs(x_xlim[0]-x_xlim[1]), abs(y_xlim[0]-y_xlim[1]), linewidth=1, edgecolor='w', linestyle='--', fill=False)
+        ax1.add_patch(rect)
+        
+        # Plot the isodoses
+        self.show_isodoses(ax=ax2, levels=levels)
+        ax2.set_xlim(x_xlim)
+        ax2.set_ylim(y_xlim[1], y_xlim[0])
+        
+        # Plot profiles
+        self.plot_profile(ax=ax3, profile='x', position=y, diff=True, xlim=x_xlim, vertical_line=x)
+        self.plot_profile(ax=ax4, profile='y', position=x, diff=True, xlim=y_xlim, vertical_line=y)
+        
 
-        Parameters
-        ----------
-        filename : str
-            The location and filename to save to.
-        kwargs
-            Keyword arguments are passed to plt.savefig().
-        """
-        self.plot_gamma_stats(**kwargs)
-        fig = plt.gcf()
-        fig.savefig(filename)
-        plt.close(fig)
             
-    def publish_pdf(self, filename=None, author=None, unit=None, notes=None, open_file=False, x=None, y=None, **kwargs):
+    def publish_pdf(self, filename=None, author=None, unit=None, notes=None, open_file=False, x=None, y=None, plot_clusters_analysis=False, iso_levels=None, xlim_margin_mm=10, **kwargs):
         """Publish a PDF report of the calibration. The report includes basic
         file information, the image and determined ROIs, and the calibration curves
 
         Parameters
         ----------
         filename : str
             The path and/or filename to save the PDF report as; must end in ".pdf".
@@ -1128,14 +1200,15 @@
         
         notes : str, list of strings, optional
             If a string, adds it as a line of text in the PDf report.
             If a list of strings, each string item is printed on its own line. Useful for writing multiple sentences.
         """
         if filename is None:
             filename = os.path.join(self.path, 'Report.pdf')
+        
         title='Film Analysis Report'
         canvas = pdf.PylinacCanvas(filename, page_title=title, logo=Path(__file__).parent / 'OMG_Logo.png')
         canvas.add_text(text='Film infos:', location=(1, 25.5), font_size=12)
         text = ['Film dose: {}'.format(os.path.basename(self.film_dose.path)),
                 'Film dose factor: {}'.format(self.film_dose_factor),
                 'Reference dose: {}'.format(os.path.basename(self.ref_dose.path)),
                 'Reference dose factor: {}'.format(self.ref_dose_factor),
@@ -1143,44 +1216,147 @@
                 'Gamma threshold: {}'.format(self.threshold),
                 'Gamma dose-to-agreement: {}'.format(self.doseTA),
                 'Gamma distance-to-agreement: {}'.format(self.distTA),
                 'Gamma normalization: {}'.format(self.norm_val)
                ]
         canvas.add_text(text=text, location=(1, 25), font_size=10)
         data = io.BytesIO()
-        self.save_analyzed_image(data, x=x, y=y, show = False)
+        self.show_results(x=x, y=y, show = False)
+        self.save_current_figure(data)
         canvas.add_image(image_data=data, location=(0.5, 3), dimensions=(19, 19))
+
+        if plot_clusters_analysis:   
+            canvas.add_new_page()
+            text = ['Detected dose clusters']
+            canvas.add_text(text=text, location=(1, 25), font_size=10)
+            data = io.BytesIO()
+            self.ref_dose.plot_clusters()
+            self.save_current_figure(data)
+            canvas.add_image(image_data=data, location=(0.5, 0), dimensions=(20, 24))
+            
+            for i, cluster in enumerate(self.clusters_analysis):      
+                canvas.add_new_page()
+                canvas.add_text(text='Cluster analysis', location=(1, 25.5), font_size=12)
+                text = ['Cluster center: X = {:.1f} mm, Y = {:.1f} mm'.format(cluster['x_mm'], cluster['y_mm']),
+                        'Median dose difference: {:.2f} %'.format(cluster['Dose diff']),
+                        'Profile offset: X = {:.2f} mm, Y = {:.2f} mm'.format(cluster['Offset x'], cluster['Offset y']),
+                        'Profile width difference: X = {:.2f} mm, Y = {:.2f} mm'.format(cluster['Diff width x'], cluster['Diff width y'])
+                       ]
+                
+                data = io.BytesIO()
+                self.show_cluster_analysis(cluster_id=i, levels=iso_levels)
+                self.save_current_figure(data)
+                canvas.add_image(image_data=data, location=(0.5, 5), dimensions=(20, 20))
+                canvas.add_text(text=text, location=(1, 25), font_size=10)
+
+        canvas.add_new_page()
+        canvas.add_text(text='Isodoses plot', location=(1, 25), font_size=10)
+        data = io.BytesIO()
+        self.show_isodoses(figsize=(10, 10), levels=iso_levels, show_ruler=False)
+        self.save_current_figure(data)
+        canvas.add_image(image_data=data, location=(0.5, 3), dimensions=(20, 20))
         
         canvas.add_new_page()
-        canvas.add_text(text='Analysis infos:', location=(1, 25.5), font_size=12)
-        canvas.add_text(text=text, location=(1, 25), font_size=10)
         data = io.BytesIO()
-        self.save_analyzed_gamma(data, figsize=(10, 10), **kwargs)
+        self.show_gamma_stats(figsize=(10, 10))
+        self.save_current_figure(data)
         canvas.add_image(image_data=data, location=(0.5, 2), dimensions=(20, 20))
-
+        
         canvas.finish()
         if open_file: webbrowser.open(filename)       
 
-    def get_profile_offsets(self):
+
+    #=================== Clusters analysis ======================
+    def analyse_clusters(self, clusters_threshold=0.6, xlim_margin_mm=10):
+        self.clusters_analysis = []
+        clusters = self.ref_dose.detect_clusters(threshold=clusters_threshold) 
+        self.ref_dose.plot_clusters()
+        fig = plt.gcf()
+        self.ax = plt.gca()
+        for cluster in clusters:
+            com = cluster['center_of_mass']
+            mask = cluster['region_mask']
+            coords = cluster['coords']
+            coords_mm = coords / self.ref_dose.dpmm
+            x = int(com[1])
+            y = int(com[0])
+            x_mm = x / self.ref_dose.dpmm
+            y_mm = y / self.ref_dose.dpmm
+            
+            # self.ref_dose.plot()
+            # fig = plt.gcf()
+            # ax = plt.gca()
+            # contours = plt.contour(mask, levels=[0.5], colors='red', linestyles='dashed')
+            while len(self.ax.lines) > 0: self.ax.lines[-1].remove() 
+            self.ax.plot((x,x),(0,self.ref_dose.shape[0]),'w--', linewidth=1)
+            self.ax.plot((0,self.ref_dose.shape[1]),(y,y),'w--', linewidth=1)
+            fig.canvas.draw_idle()
+            plt.pause(0.01)
+                        
+            median_film_dose = np.median(self.film_dose.array[mask.astype(bool)])
+            median_ref_dose = np.median(self.ref_dose.array[mask.astype(bool)])
+            relative_diff = (median_film_dose-median_ref_dose)/median_ref_dose * 100
+            print("Median film dose = {} cGy; median ref dose = {} cGy; Relative diff = {}%".format(median_film_dose, median_ref_dose, relative_diff))
+            
+            x_xlim = (min(coords_mm[:,1])-xlim_margin_mm, max(coords_mm[:,1])+xlim_margin_mm)
+            y_xlim = (min(coords_mm[:,0])-xlim_margin_mm, max(coords_mm[:,0])+xlim_margin_mm)
+            
+            self.get_profile_offsets(x=x, y=y, x_xlim=x_xlim, y_xlim=y_xlim)
+            self.clusters_analysis.append({'x_px': x, 'y_px': y, 'x_mm': x_mm, 'y_mm': y_mm,
+                                           'Dose diff': relative_diff,
+                                           'Offset x': self.offset_x, 'Offset y': self.offset_y,
+                                           'Diff width x': self.diff_grandeur_x, 'Diff width y': self.diff_grandeur_y })
+        plt.close(fig)
+                
+    
+    #=================== Profile analysis ======================
+    def get_profile_offsets(self, x=None, y=None, x_xlim=None, y_xlim=None):
         """ Starts an interactive process where the user can move
             the measured profile with respect to the reference profile
             in order to compute the spatial offset between the two.
             The process is repeated four times to get offsets on both
             sides in the x and y directions.
+            
+            Parameters
+            ----------
+            x : int, optional
+                The x position of the profile to plot, in pixels.
+                If None, position is set to the center of the reference dose.
+                Default is None
+                
+            y : int, optional
+                The y position of the profile to plot, in pixels.
+                If None, position is set to the center of the reference dose.
+                Default is None
+                
+            xlim : tuple, optional
+                
         """
-        self.get_profile_offset(direction='x', side='left')
+        if x is None: x = np.floor(self.ref_dose.shape[1] / 2).astype(int)
+        if y is None: y = np.floor(self.ref_dose.shape[0] / 2).astype(int)
+        
+        self.get_profile_offset(x=x, y=y, direction='x', side='left', xlim=x_xlim)
         self.offset_x_gauche = self.offset
-        self.get_profile_offset(direction='x', side='right')
+        self.get_profile_offset(x=x, y=y, direction='x', side='right', xlim=x_xlim)
         self.offset_x_droite = self.offset
-        self.get_profile_offset(direction='y', side='left')
+        self.get_profile_offset(x=x, y=y, direction='y', side='left', xlim=y_xlim)
         self.offset_y_gauche = self.offset
-        self.get_profile_offset(direction='y', side='right')
+        self.get_profile_offset(x=x, y=y, direction='y', side='right', xlim=y_xlim)
         self.offset_y_droite = self.offset
+        
+        self.offset_x = -1.0*((self.offset_x_gauche + self.offset_x_droite) / 2.0)
+        self.offset_y = -1.0*((self.offset_y_gauche + self.offset_y_droite) / 2.0)
+        self.diff_grandeur_x = self.offset_x_gauche - self.offset_x_droite
+        self.diff_grandeur_y = self.offset_y_gauche - self.offset_y_droite
+        
+        print("X: Décalage = {:.2f} mm; Diff grandeur = {:.2f} mm".format(self.offset_x, self.diff_grandeur_x))
+        print("Y: Décalage = {:.2f} mm; Diff grandeur = {:.2f} mm".format(self.offset_y, self.diff_grandeur_y))
+        
 
-    def get_profile_offset(self, direction='x', side='left'):
+    def get_profile_offset(self, x, y, direction, side='left', xlim=None):
         """ Opens an interactive plot where the user can move
             the measured profile with respect to the reference profile
             in order to compute the spatial offset between the two.
 
         Parameters
         ----------
         direction : str, optional
@@ -1188,54 +1364,70 @@
             Either 'x' (horizontal) or 'y' (vertical).
             Default is 'x'.
         
         side : str, optional
             The side on the profile that will be matched.
             Either 'left' or 'right'.
             Default is left. 
+            
+        position : int, optional
+            The position of the profile to plot, in pixels, in the direction perpendicular to the profile.
+            eg. if profile='x' and position=400, a profile in the x direction is showed, at position y=400.
+            If None, position is set to the center of the reference dose.
+            Default is None
         """
         msg = '\nUse left/right keyboard arrows to move profile and fit on ' + side + ' side. Press Enter when done.'
         print(msg)
         self.offset = 0
         self.direction = direction
-        self.plot_profile(profile=direction, diff=True, offset=0, title='Fit profiles on ' + side + ' side')
+        self.xlim = xlim
+        
+        if direction == 'x':
+            self.position = y
+            self.line = x
+            self.plot_profile(profile='x', position=y, vertical_line=x, title=direction + ': Fit profiles on ' + side + ' side', xlim=xlim)
+        elif direction == 'y':
+            self.position = x
+            self.line = y
+            self.plot_profile(profile='y', position=x, vertical_line=y, title=direction + ': Fit profiles on ' + side + ' side', xlim=xlim)
+
         self.fig = plt.gcf()
+        fig_manager = plt.get_current_fig_manager()
+        fig_manager.window.showMaximized()
         self.cid = self.fig.canvas.mpl_connect('key_press_event', self.move_profile_ontype)
         self.wait = True
         while self.wait: plt.pause(1)
         plt.close(self.fig)
         return
                 
     def move_profile_ontype(self, event):
         """ This function is called by self.get_profile_offset()
             to either move the profile when left/right keys are pressed,
             or to close the figure when Enter is pressed.
         """
         fig = plt.gcf()
         ax = plt.gca()
+        position = self.position
         
         if event.key == 'left':
             self.offset -= 0.1
-            self.plot_profile(ax=ax, profile=self.direction, position=None, title=None, diff=False, offset=self.offset)
+            self.plot_profile(ax=ax, profile=self.direction, position=position, title='Shift = ' + str(self.offset) + ' mm', diff=False, offset=self.offset, vertical_line=self.line, xlim=self.xlim)
             fig.canvas.draw_idle()
-            ax.set_title('Shift = ' + str(self.offset) + ' mm')
             
         if event.key == 'right':
             self.offset += 0.1
-            self.plot_profile(ax=ax, profile=self.direction, position=None, title=None, diff=False, offset=self.offset)
+            self.plot_profile(ax=ax, profile=self.direction, position=position, title='Shift = ' + str(self.offset) + ' mm', diff=False, offset=self.offset, vertical_line=self.line, xlim=self.xlim)
             fig.canvas.draw_idle()
-            ax.set_title('Shift = ' + str(self.offset) + ' mm')
         
         if event.key == 'enter':
             self.fig.canvas.mpl_disconnect(self.cid)
             self.wait = False
             return self.offset
 
 ########################### End class DoseAnalysis ############################## 
-    
 def line_intersection(line1, line2):
     """ Get the coordinates of the intersection of two lines.
 
         Parameters
         ----------
         line1 : tuple 
             Coordinates of 2 points defining the first line
@@ -1278,13 +1470,21 @@
         file = open(filename, 'rb')
         analysis = pickle.load(file)
     file.close()
     return analysis
 
 def save_analysis(analysis, filename, use_compression=True):
     print("\nSaving analysis file as {}...".format(filename))
+    if hasattr(analysis, "ruler"): del analysis.ruler
     if use_compression:
         file = bz2.open(filename, 'wb')
     else:
         file = open(filename, 'wb')
     pickle.dump(analysis, file, pickle.HIGHEST_PROTOCOL)
     file.close()
+
+def add_ruler(ax=None):
+    if ax is None: ax = plt.gca()
+    markerprops = dict(marker='o', markersize=5, markeredgecolor='red')
+    lineprops = dict(color='red', linewidth=2)
+    ruler = Ruler(ax=ax, useblit=True, markerprops=markerprops, lineprops=lineprops)
+    return ruler
```

### Comparing `omg_dosimetry-1.6.3/src/omg_dosimetry/calibration.py` & `omg_dosimetry-1.7.0/src/omg_dosimetry/calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,20 +132,22 @@
 
     Attributes
     ----------
             
     LUT.lut : numpy array
         When lateral correction is applied:
 
-        3D array of size (nDoses, nPixel, 6), where nDoses is the number of calibration doses used,
-        nPixel is the number of pixels in the lateral scanner direction, and the last dimension contains
-        [doses, output/profile corrected doses, mean channel, R channel, G channel, B channel].
-        Without lateral correct:
+        3D array of size (6, nDoses, nPixel). The first dimension contains 
+        [doses, output/profile corrected doses, mean channel, R channel, G channel, B channel]. 
+        nDoses is the number of calibration doses used, and
+        nPixel is the number of pixels in the lateral scanner direction.
         
-        2D array of size (nDoses, 6), defined as above, except that a single LUT is stored
+        Without lateral correctoin:
+
+        2D array of size (6, nDoses), defined as above, except that a single LUT is stored
         by taking the median values over the ROIs, instead of one LUT for each scanner pixel.
     LUT.channel_mean : 2D array of size (nDoses, nPixel)
         Contains the average RGB value for each dose, at each pixel location.
     LUT.channel_R : 2D array of size (nDoses, nPixel)
         Contains the Red channel value for each dose, at each pixel location.
     LUT.channel_G : 2D array of size (nDoses, nPixel)
         Contains the Gren channel value for each dose, at each pixel location.
```

### Comparing `omg_dosimetry-1.6.3/src/omg_dosimetry/i_o.py` & `omg_dosimetry-1.7.0/src/omg_dosimetry/i_o.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/src/omg_dosimetry/imageRGB.py` & `omg_dosimetry-1.7.0/src/omg_dosimetry/imageRGB.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pydicom
 from pydicom.errors import InvalidDicomError
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image as pImage
 from scipy import ndimage
 from skimage.transform import rotate
+from skimage.measure import regionprops
 import scipy.ndimage.filters as spf
 
 from pylinac.core.utilities import is_close
 # from pylinac.core.decorators import type_accept, value_accept
 from pylinac.core.geometry import Point
 from pylinac.core.io import get_url, TemporaryZipDirectory, retrieve_filenames
 from pylinac.core.profile import stretch as stretcharray
@@ -331,51 +332,118 @@
         if date is None:
             try:
                 date = datetime.fromtimestamp(osp.getctime(self.path)).strftime(format)
             except AttributeError:
                 date = 'Unknown'
         return date
 
-    def plot(self, ax=None, show=True, cmap='inferno', clim=None, title='', **kwargs):
+    def plot(self, ax=None, show=True, cmap='inferno', clim=None, title='', colorbar=False, **kwargs):
         if ax is None:
             fig, ax = plt.subplots()
         if clim is None:
             min_value = np.percentile(self.array,[0.1])[0].round(decimals=-1)
             max_value = np.percentile(self.array,[99.9])[0].round(decimals=-1)
             clim = [min_value, max_value]               
+        fig = plt.gcf()
+        
         if self.array.ndim > 2 and self.array.max() > 255:
-            cax = ax.imshow(self.array / 65535., cmap=cmap, **kwargs) 
+            cax = ax.imshow(self.array / 65535., cmap=cmap, origin='upper', **kwargs) 
         else:
-            cax = ax.imshow(self.array, cmap=cmap, **kwargs)
+            cax = ax.imshow(self.array, cmap=cmap, origin='upper', **kwargs)
         cax.set_clim(clim) 
+        if colorbar: fig.colorbar(cax, ax=ax)
         ax.set_title(title)
         ax.axis('image')      
         if show:
             plt.show()
         return cax
     
-    def plotCB(self, ax=None, show=True, cmap='inferno', clim=None, title='', **kwargs):
+    def plot_isodoses(self, ax=None, levels=None, colors='red', show=True, title='', labels=True, inline=True, **kwargs):
         if ax is None:
-            fig, ax = plt.subplots()
-        if clim is None:
-            min_value = np.percentile(self.array,[0.1])[0].round(decimals=-0)
-            max_value = np.percentile(self.array,[99.9])[0].round(decimals=-0)
-            clim = [min_value, max_value]    
-        fig = plt.gcf()
-            
-        if self.array.ndim > 2 and self.array.max() > 255:
-            cax = ax.imshow(self.array / 65535., cmap=cmap, interpolation='nearest', **kwargs) 
-        else:
-            cax = ax.imshow(self.array, cmap=cmap, interpolation='nearest', **kwargs)
-        cax.set_clim(clim)
-        fig.colorbar(cax, ax=ax)   
+            fig, ax = plt.subplots()    
+        if levels is None:
+            d_max = self.array.max()
+            levels = [d_max * l for l in np.arange(0.2, 1.0, 0.2)]
+        contours = ax.contour(self.array, levels=levels, colors=colors, origin='upper', **kwargs)  # Courbes de contour
+        if labels: ax.clabel(contours, inline=inline, fontsize=10, inline_spacing=1)
         ax.set_title(title)
-        ax.axis('image')      
-        if show: plt.show(block = False)
-        return cax
+        ax.axis('image')   
+        if show:
+            plt.show()
+        return contours
+
+    # The following function is to be removed starting from v2.x
+    def plotCB(self, ax=None, show=True, cmap='inferno', clim=None, title='', **kwargs):
+        self.plot(ax=ax, show=show, cmap=cmap, clim=clim, title=title, colorbar=True, **kwargs)
+
+    def detect_clusters(self, threshold=0.6) -> list:
+        """
+        Detect clusters based on a threshold value.
+
+        Parameters
+        ----------
+        threshold : float, optional
+            Threshold value as a percentage [0 - 1] to be used with respect to the maximum dose. Defaults to 0.6 (60 %).
+
+        Returns
+        -------
+        clusters : list
+            A list containing dictionaries, each representing a detected cluster.
+            Each dictionary contains the following keys:
+            - 'region_mask': A boolean mask indicating the region of the cluster.
+            - 'coords': An array of coordinates of the cluster points.
+            - 'center_of_mass': The center of mass of the cluster.
+        """
+
+        data = self.array
+        mask = data > threshold * self.array.max()
+        labeled_regions, num_features = ndimage.label(mask)
+
+        clusters = []
+        for region_label in range(1, num_features + 1):  # Starts at 1 because the background is labeled 0.
+            cluster = {}    
+            cluster['region_mask'] = labeled_regions == region_label
+            cluster['coords'] = np.argwhere(cluster['region_mask'])
+            cluster['center_of_mass'] = np.mean(cluster['coords'], axis=0)
+            clusters.append(cluster)
+        self.clusters = clusters
+        return clusters
+
+    def discard_small_clusters(self, minimum_length):
+        """
+        Discard cluster with an axis_minor_length less than a given value.
+
+        Parameters
+        ----------
+        minimum_length : float
+            The minimum length in milimeters for retaining clusters.
+        """    
+        new_clusters = []
+        # Calculate the size threshold in pixels
+        size_threshold = minimum_length*self.dpmm
+
+        for region in self.clusters:
+            if region['coords'].shape[0] == 1: # Skip one pixel size clusters.
+                pass
+            region_prop = regionprops(region['region_mask'].astype(int))
+            if region_prop[0]['axis_minor_length'] < size_threshold:
+                pass
+            else:
+                new_clusters.append(region)
+        self.clusters = new_clusters
+
+    def plot_clusters(self):
+        self.plot()
+        for cluster in self.clusters:
+            com = cluster['center_of_mass']
+            mask = cluster['region_mask']
+            fig = plt.gcf()
+            ax = plt.gca()
+            contours = plt.contour(mask, levels=[0.5], colors='red', linestyles='dashed')
+            ax.scatter(com[1], com[0], color='blue', marker='o', label='Center')
 
     # @value_accept(kind=('median', 'gaussian'))
     def filter(self, size=0.05, kind='median'):
         """Filter the profile.
 
         Parameters
         ----------
```

### Comparing `omg_dosimetry-1.6.3/src/omg_dosimetry/tiff2dose.py` & `omg_dosimetry-1.7.0/src/omg_dosimetry/tiff2dose.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,46 +431,49 @@
 
         max_dose_m = np.percentile(self.dose_m.array, [99.9])[0].round(decimals=-1)
         max_dose_opt = np.percentile(self.dose_opt.array, [99.9])[0].round(decimals=-1)
         clim = [0, max(max_dose_m, max_dose_opt)]
         fig, ((ax1,ax2,ax3), (ax4,ax5,ax6), (ax7,ax8,ax9)) = plt.subplots(3, 3, figsize=(14, 9))
         axes = [ax1, ax2, ax3, ax4, ax5, ax6, ax7, ax8, ax9]
 
-        self.dose_r.plotCB(ax1, clim=clim, title='Red channel dose')
-        self.dose_g.plotCB(ax2, clim=clim, title='Green channel dose')
-        self.dose_b.plotCB(ax3, clim=clim, title='Blue channel dose')
-        self.dose_m.plotCB(ax4, clim=clim, title='Mean channel dose')
-        self.dose_rg.plotCB(ax5, clim=clim, title='Red+Green Average dose')
+        self.dose_r.plot(ax1, clim=clim, title='Red channel dose', colorbar=True)
+        self.dose_g.plot(ax2, clim=clim, title='Green channel dose', colorbar=True)
+        self.dose_b.plot(ax3, clim=clim, title='Blue channel dose', colorbar=True)
+        self.dose_m.plot(ax4, clim=clim, title='Mean channel dose', colorbar=True)
+        self.dose_rg.plot(ax5, clim=clim, title='Red+Green Average dose', colorbar=True)
 
-        self.dose_consistency.plotCB(
-            ax6,
+        self.dose_consistency.plot(ax6,
             clim = [0, np.percentile(self.dose_consistency.array, [99.5])[0]],
             cmap='gray',
-            title='Consistency'
+            title='Consistency', 
+            colorbar=True
         )
 
-        self.dose_opt.plotCB(
+        self.dose_opt.plot(
             ax7,
             clim=clim,
-            title='Multichannel optimized dose'
+            title='Multichannel optimized dose',
+            colorbar=True
         )
 
-        self.dose_opt_delta.plotCB(
+        self.dose_opt_delta.plot(
             ax8,
             clim = [np.percentile(self.dose_opt_delta.array, [0.5])[0],
                     np.percentile(self.dose_opt_delta.array, [99.5])[0]],
             cmap='gray',
-            title='Disturbance'
+            title='Disturbance',
+            colorbar=True
         )
 
-        self.dose_opt_RE.plotCB(
+        self.dose_opt_RE.plot(
             ax9,
             clim = [0, np.percentile(self.dose_opt_RE.array, [99.5])[0]],
             cmap='gray',
-            title='Residuals'
+            title='Residuals',
+            colorbar=True
         )
 
         fig.tight_layout()
 
         if savefile:
             plt.savefig(savefile)
         if show:
```

### Comparing `omg_dosimetry-1.6.3/.gitignore` & `omg_dosimetry-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/LICENSE` & `omg_dosimetry-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/README.rst` & `omg_dosimetry-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.6.3/pyproject.toml` & `omg_dosimetry-1.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "omg_dosimetry"
 
-version = "1.6.3"
+version = "1.7.0"
 
 authors = [
   { name="JF Cabana", email="jean-francois.cabana.cisssca@ssss.gouv.qc.ca" },
 ]
 maintainers = [
   {name = "Luis Alfonso Olivares Jimenez", email = "alfonso.cucei.udg@gmail.com"}
 ]
```

### Comparing `omg_dosimetry-1.6.3/PKG-INFO` & `omg_dosimetry-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: omg_dosimetry
-Version: 1.6.3
+Version: 1.7.0
 Summary: Optimized Multichannel Gafchromic Dosimetry (OMG Dosimetry)
 Project-URL: homepage, https://omg-dosimetry.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/jfcabana/omg_dosimetry
 Project-URL: Bug-Tracker, https://github.com/jfcabana/omg_dosimetry/issues
 Author-email: JF Cabana <jean-francois.cabana.cisssca@ssss.gouv.qc.ca>
 Maintainer-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 License-File: LICENSE
```

