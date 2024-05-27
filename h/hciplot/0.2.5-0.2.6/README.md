# Comparing `tmp/hciplot-0.2.5.tar.gz` & `tmp/hciplot-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hciplot-0.2.5.tar", last modified: Tue Aug  1 16:21:26 2023, max compression
+gzip compressed data, was "hciplot-0.2.6.tar", last modified: Mon May 27 18:53:25 2024, max compression
```

## Comparing `hciplot-0.2.5.tar` & `hciplot-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-08-01 16:21:26.298123 hciplot-0.2.5/
--rw-r--r--   0 valentin   (501) staff       (20)     6148 2022-02-15 18:32:34.000000 hciplot-0.2.5/.DS_Store
--rw-r--r--   0 valentin   (501) staff       (20)     1246 2023-08-01 16:19:06.000000 hciplot-0.2.5/.gitignore
--rw-r--r--   0 valentin   (501) staff       (20)     1086 2021-12-01 15:26:15.000000 hciplot-0.2.5/LICENSE
--rw-r--r--   0 valentin   (501) staff       (20)     2743 2023-08-01 16:21:26.297910 hciplot-0.2.5/PKG-INFO
--rw-r--r--   0 valentin   (501) staff       (20)     1841 2021-12-01 15:26:15.000000 hciplot-0.2.5/README.md
-drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-08-01 16:21:26.296288 hciplot-0.2.5/hciplot/
--rw-r--r--   0 valentin   (501) staff       (20)       68 2023-08-01 16:19:06.000000 hciplot-0.2.5/hciplot/__init__.py
--rw-r--r--   0 valentin   (501) staff       (20)    51163 2023-08-01 16:19:52.000000 hciplot-0.2.5/hciplot/hciplot.py
-drwxr-xr-x   0 valentin   (501) staff       (20)        0 2023-08-01 16:21:26.297686 hciplot-0.2.5/hciplot.egg-info/
--rw-r--r--   0 valentin   (501) staff       (20)     2743 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/PKG-INFO
--rw-r--r--   0 valentin   (501) staff       (20)      257 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/SOURCES.txt
--rw-r--r--   0 valentin   (501) staff       (20)        1 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/dependency_links.txt
--rw-r--r--   0 valentin   (501) staff       (20)       53 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/requires.txt
--rw-r--r--   0 valentin   (501) staff       (20)        8 2023-08-01 16:21:26.000000 hciplot-0.2.5/hciplot.egg-info/top_level.txt
--rw-r--r--   0 valentin   (501) staff       (20)       52 2023-08-01 16:19:24.000000 hciplot-0.2.5/requirements.txt
--rw-r--r--   0 valentin   (501) staff       (20)       38 2023-08-01 16:21:26.298174 hciplot-0.2.5/setup.cfg
--rw-r--r--   0 valentin   (501) staff       (20)     2213 2022-05-16 15:51:24.000000 hciplot-0.2.5/setup.py
+drwxr-xr-x   0 valentin   (501) staff       (20)        0 2024-05-27 18:53:25.631132 hciplot-0.2.6/
+-rw-r--r--   0 valentin   (501) staff       (20)     1246 2023-08-01 16:19:06.000000 hciplot-0.2.6/.gitignore
+-rw-r--r--   0 valentin   (501) staff       (20)     1086 2021-12-01 15:26:15.000000 hciplot-0.2.6/LICENSE
+-rw-r--r--   0 valentin   (501) staff       (20)     2886 2024-05-27 18:53:25.630937 hciplot-0.2.6/PKG-INFO
+-rw-r--r--   0 valentin   (501) staff       (20)     1841 2021-12-01 15:26:15.000000 hciplot-0.2.6/README.md
+drwxr-xr-x   0 valentin   (501) staff       (20)        0 2024-05-27 18:53:25.629649 hciplot-0.2.6/hciplot/
+-rw-r--r--   0 valentin   (501) staff       (20)       68 2024-05-27 18:38:56.000000 hciplot-0.2.6/hciplot/__init__.py
+-rw-r--r--   0 valentin   (501) staff       (20)    53011 2024-05-27 18:37:12.000000 hciplot-0.2.6/hciplot/hciplot.py
+drwxr-xr-x   0 valentin   (501) staff       (20)        0 2024-05-27 18:53:25.630722 hciplot-0.2.6/hciplot.egg-info/
+-rw-r--r--   0 valentin   (501) staff       (20)     2886 2024-05-27 18:53:25.000000 hciplot-0.2.6/hciplot.egg-info/PKG-INFO
+-rw-r--r--   0 valentin   (501) staff       (20)      247 2024-05-27 18:53:25.000000 hciplot-0.2.6/hciplot.egg-info/SOURCES.txt
+-rw-r--r--   0 valentin   (501) staff       (20)        1 2024-05-27 18:53:25.000000 hciplot-0.2.6/hciplot.egg-info/dependency_links.txt
+-rw-r--r--   0 valentin   (501) staff       (20)       53 2024-05-27 18:53:25.000000 hciplot-0.2.6/hciplot.egg-info/requires.txt
+-rw-r--r--   0 valentin   (501) staff       (20)        8 2024-05-27 18:53:25.000000 hciplot-0.2.6/hciplot.egg-info/top_level.txt
+-rw-r--r--   0 valentin   (501) staff       (20)       52 2023-08-01 16:19:24.000000 hciplot-0.2.6/requirements.txt
+-rw-r--r--   0 valentin   (501) staff       (20)       38 2024-05-27 18:53:25.631177 hciplot-0.2.6/setup.cfg
+-rw-r--r--   0 valentin   (501) staff       (20)     2213 2022-05-16 15:51:24.000000 hciplot-0.2.6/setup.py
```

### Comparing `hciplot-0.2.5/.gitignore` & `hciplot-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hciplot-0.2.5/LICENSE` & `hciplot-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hciplot-0.2.5/PKG-INFO` & `hciplot-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hciplot
-Version: 0.2.5
+Version: 0.2.6
 Summary: High-contrast Imaging Plotting library
 Home-page: https://github.com/carlgogo/hciplot
 Download-URL: https://github.com/carlgogo/hciplot/archive/refs/tags/v0.1.8.tar.gz
 Author: Carlos Alberto Gomez Gonzalez, Valentin Christiaens
 Author-email: valentinchrist@hotmail.com
 License: MIT
 Keywords: plotting,hci,package
@@ -16,14 +16,20 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib>=3.7.0
+Requires-Dist: holoviews
+Requires-Dist: bokeh
+Requires-Dist: panel
+Requires-Dist: jinja2
 
 [![PyPI version](https://badge.fury.io/py/hciplot.svg)](https://badge.fury.io/py/hciplot)
 
 # HCIplot
 
 ``HCIplot`` -- High-contrast Imaging Plotting library. The goal of this
 library is to be the "Swiss army" solution for plotting and visualizing
```

### Comparing `hciplot-0.2.5/README.md` & `hciplot-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `hciplot-0.2.5/hciplot/hciplot.py` & `hciplot-0.2.6/hciplot/hciplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,53 +6,56 @@
 from os import mkdir
 from os.path import exists
 from shutil import rmtree
 from subprocess import call
 from warnings import filterwarnings
 
 import numpy as np
-from holoviews import extension, Dataset, Image, Layout, output, opts
-from matplotlib.cm import register_cmap
-from matplotlib.colors import LinearSegmentedColormap, LogNorm, ListedColormap, Normalize
+import matplotlib
+from matplotlib.colors import (LinearSegmentedColormap, LogNorm, ListedColormap,
+                               Normalize)
 from matplotlib.patches import Circle, Ellipse
 from matplotlib.pyplot import colorbar as plt_colorbar
 from matplotlib.pyplot import (figure, subplot, show, savefig, close, hlines,
                                annotate)
 from mpl_toolkits.axes_grid1 import make_axes_locatable
+from holoviews import extension, Dataset, Image, Layout, output, opts
 
 filterwarnings("ignore", module="matplotlib")
 
-# Registering heat and cool colormaps from SaoImage DS9
+# Registering heat and cool colormaps from SAOImage DS9
 # borrowed from: https://gist.github.com/adonath/c9a97d2f2d964ae7b9eb
 ds9cool = {'red': lambda v: 2 * v - 1,
            'green': lambda v: 2 * v - 0.5,
            'blue': lambda v: 2 * v}
 ds9heat = {'red': lambda v: np.interp(v, [0, 0.34, 1], [0, 1, 1]),
            'green': lambda v: np.interp(v, [0, 1], [0, 1]),
            'blue': lambda v: np.interp(v, [0, 0.65, 0.98, 1], [0, 0, 1, 1])}
-register_cmap(cmap=LinearSegmentedColormap('ds9cool', ds9cool))
-register_cmap(cmap=LinearSegmentedColormap('ds9heat', ds9heat))
+matplotlib.colormaps.register(cmap=LinearSegmentedColormap(name='ds9cool', segmentdata=ds9cool))
+matplotlib.colormaps.register(cmap=LinearSegmentedColormap(name='ds9heat', segmentdata=ds9heat))
 cmap_binary = ListedColormap(['black', 'white'])
 default_cmap = 'viridis'
 
 
 def plot_frames(data, backend='matplotlib', mode='mosaic', rows=1, vmax=None,
                 vmin=None, circle=None, circle_alpha=0.8, circle_color='white',
                 circle_linestyle='-', circle_radius=6, circle_label=False,
                 circle_label_color='white', ellipse=None, ellipse_alpha=0.8,
                 ellipse_color='white', ellipse_linestyle='-', ellipse_a=6,
                 ellipse_b=4, ellipse_angle=0, ellipse_label=False,
                 ellipse_label_color='white', arrow=None, arrow_alpha=0.8,
-                arrow_length=10, arrow_shiftx=5, arrow_label=None, label=None,
-                label_pad=5, label_size=12, label_color='white', grid=False,
-                grid_alpha=0.4,  grid_color='#f7f7f7', grid_spacing=None,
-                cross=None, cross_alpha=0.4, lab_fontsize=8, cross_color='white',
-                ang_scale=False, ang_ticksep=50, tick_direction='out',
-                tick_color='black', ndec=1, pxscale=0.01, auscale=1.,
-                ang_legend=False, au_legend=False, axis=True,
+                arrow_length=10, arrow_shiftx=5, arrow_label=None,
+                arrow_color='white', arrow_head_width=6, arrow_head_length=4,
+                arrow_width=2, label=None, label_pad=5, label_size=12,
+                label_color='white', grid=False, grid_alpha=0.4,
+                grid_color='#f7f7f7', grid_spacing=None, cross=None,
+                cross_alpha=0.4, lab_fontsize=8, cross_color='white',
+                ang_scale=False, ang_ticksep=50, ang_ticksep_minor=None,
+                tick_direction='out', tick_color='black', ndec=1, pxscale=0.01,
+                auscale=1., ang_legend=False, au_legend=False, axis=True,
                 show_center=False, cmap=None, log=False, colorbar=True,
                 top_colorbar=False, colorbar_ticks=None, colorbar_ticksize=8,
                 colorbar_label='', colorbar_label_size=8, patch=None, dpi=100,
                 size_factor=6, horsp=0.4, versp=0.2, width=400, height=400,
                 title=None, tit_size=16, sampling=1, save=None,
                 return_fig_ax=False, transparent=False):
     """ Plot a 2d array or a tuple of 2d arrays. Supports the ``matplotlib`` and
@@ -60,15 +63,15 @@
     mosaic. For ``matplotlib``, instead of a mosaic of images, we can create a
     mosaic of surface plots. Also, when using the ``matplotlib`` backend, this
     function allows to annotate and customize the plot and produce publication
     quality figures.
 
     Parameters
     ----------
-    data : numpy.ndarray or tuple
+    data : 2d numpy.ndarray, or tuple/list of 2d numpy.ndarray
         A single 2d array or a tuple of 2d arrays.
     backend : {'matplotlib', 'bokeh'}, str optional
         Selects the backend used to display the plots. ``Matplotlib`` plots
         are static and allow customization (leading to publication quality
         figures). ``Bokeh`` plots are interactive, allowing the used to zoom,
         pan, inspect pixel values, etc.
     mode : {'mosaic', 'surface'}, str optional
@@ -157,17 +160,21 @@
     cross_alpha : float, optional
         [backend='matplotlib'] Alpha transparency of the crosshair.
     cross_color : string, optional
         [backend='matplotlib'] Color of the crosshair.
     ang_scale : bool or tuple of bools, optional
         [backend='matplotlib'] If True, the axes are displayed in angular scale
         (arcsecs).
-    ang_ticksep : int, optional
+    ang_ticksep : float, optional
         [backend='matplotlib'] Separation for the ticks in pixels, when using
         axis in angular scale.
+    ang_ticksep_minor : float, optional
+        [backend='matplotlib'] Separation for the minor ticks in pixels, when
+        using axis in angular scale. If not provided, will be determined
+        automatically by matplotlib.
     tick_direction : str, optional
         [backend='matplotlib'] Outward or inward facing axis ticks.
         'in' for inward, 'out' for outwards.
     tick_color : str, optional
         [backend='matplotlib'] Color of the axis ticks.
     ndec : int, optional
         [backend='matplotlib'] Number of decimals for axes labels.
@@ -222,16 +229,17 @@
         [backend='matplotlib'] Horizontal gap between subplots.
     versp : float, optional
         [backend='matplotlib'] Vertical gap between subplots.
     width : int, optional
         [backend='bokeh'] Controls the width of each subplot.
     height : int, optional
         [backend='bokeh'] Controls the height of each subplot.
-    title : None or str, optional
-        [backend='matplotlib'] Title of the whole figure, None by default.
+    title : None or str or tuple of str, optional
+        [backend='matplotlib'] Title of the whole figure, or of each subfigure.
+        None by default.
     tit_size: int, optional
         Size of the title font.
     sampling : int, optional
         [mode='surface'] Sets the stride used to sample the input data to
         generate the surface graph.
     save : None or str, optional
         If a string is provided the plot is saved using ``save`` as the
@@ -511,18 +519,25 @@
 
     # --------------------------------------------------------------------------
     if backend == 'matplotlib':
         # Creating the figure --------------------------------------------------
         fig = figure(figsize=(cols * size_factor, rows * size_factor), dpi=dpi)
 
         if title is not None:
-            fig.suptitle(title, fontsize=tit_size, va='center', x=0.51,
-                         # y=1-0.08*(28/tit_size)**(0.5))
-                         y=1-0.1*(16/tit_size))
-
+            if not isinstance(title, (tuple, list)):
+                do_subtitle = False
+                fig.suptitle(title, fontsize=tit_size, va='center', x=0.51,
+                             # y=1-0.08*(28/tit_size)**(0.5))
+                             y=1-0.1*(16/tit_size))
+            elif len(title) == num_plots:
+                do_subtitle = True
+            else:
+                raise ValueError("Format of provided title not recognized.")
+        else:
+            do_subtitle = False
         if mode == 'surface':
             plot_mosaic = False
         elif mode == 'mosaic':
             plot_mosaic = True
         else:
             raise ValueError("`mode` value was not recognized")
 
@@ -557,14 +572,16 @@
 
                 else:
                     cucmap = custom_cmap[i]
                     cbticks = cbar_ticks[i]
 
                 im = ax.imshow(image, cmap=cucmap, origin='lower',
                                norm=norm, interpolation='nearest')
+                if do_subtitle:
+                    ax.set_title(title[i])
                 # if colorbar[i]:
                 #     divider = make_axes_locatable(ax)
                 #     # the width of cax is 5% of ax and the padding between cax
                 #     # and ax wis fixed at 0.05 inch
                 #     cax = divider.append_axes("right", size="5%", pad=0.05)
                 #     cb = plt_colorbar(im, ax=ax, cax=cax, drawedges=False,
                 #                       ticks=cbticks)
@@ -584,16 +601,16 @@
                 surf = ax.plot_surface(x, y, image, rstride=sampling,
                                        cstride=sampling, linewidth=2,
                                        cmap=custom_cmap[i], antialiased=True,
                                        vmin=vmin[i], vmax=vmax[i])
                 ax.set_xlabel('x')
                 ax.set_ylabel('y')
                 ax.dist = 10
-                if title is not None:
-                    ax.set_title(title)
+                if do_subtitle:
+                    ax.set_title(title[i])
 
                 if colorbar[i]:
                     fig.colorbar(surf, aspect=10, pad=0.05, fraction=0.04)
 
             if ang_legend[i] and plot_mosaic:
                 scaleng = 1. / pxscale
                 scalab = '1 arcsec'
@@ -700,117 +717,136 @@
                         e_offset_j = min(e_offset, ellipse_a[j])
                         ax.text(x, y + ellipse_a[j] + e_offset_j, elllabel,
                                 fontsize=label_size, color=ellipse_label_color,
                                 family='monospace', ha='center', va='center',
                                 weight='bold', alpha=ellipse_alpha[j])
 
             if show_cross and plot_mosaic:
-                ax.axhline(coor_cross[0], xmin=0, xmax=frame_size, alpha=cross_alpha, lw=0.6,
+                ax.axhline(coor_cross[0], xmin=0, xmax=frame_size,
+                           alpha=cross_alpha, lw=0.6,
                            linestyle='dashed', color='white')
-                ax.axvline(coor_cross[1], ymin=0, ymax=frame_size, alpha=cross_alpha, lw=0.6,
+                ax.axvline(coor_cross[1], ymin=0, ymax=frame_size,
+                           alpha=cross_alpha, lw=0.6,
                            linestyle='dashed', color='white')
 
             if show_center[i] and plot_mosaic:
                 ax.scatter([cy], [cx], marker='+',
                            color=cross_color, alpha=cross_alpha)
 
             if show_arrow and plot_mosaic:
                 ax.arrow(arrow[0] + arrow_length + arrow_shiftx, arrow[1],
-                         -arrow_length, 0, color='white', head_width=6,
-                         head_length=4, width=2, length_includes_head=True,
-                         alpha=arrow_alpha)
+                         -arrow_length, 0, color=arrow_color,
+                         head_width=arrow_head_width,
+                         head_length=arrow_head_length, width=arrow_width,
+                         length_includes_head=True, alpha=arrow_alpha)
                 if arrow_label:
                     x = arrow[0]
                     y = arrow[1]
                     if isinstance(arrow_label, str):
                         arrlabel = arrow_label
                     else:
                         arrlabel = str(int(x))+','+str(int(y))
                     if len(arrlabel) < 5:
                         arr_fontsize = 14
                     else:
                         arr_fontsize = lab_fontsize
 
                     ax.text(x + arrow_length + 1.3*arrow_shiftx, y, arrlabel,
-                            fontsize=arr_fontsize, color='white', family='monospace',
-                            ha='left', va='center', weight='bold',
-                            alpha=arrow_alpha)
+                            fontsize=arr_fontsize, color='white',
+                            family='monospace', ha='left', va='center',
+                            weight='bold', alpha=arrow_alpha)
 
             if label[i] is not None and plot_mosaic:
-                ax.annotate(label[i], xy=(label_pad_x, label_pad_y), color=label_color[i],
-                            xycoords='axes pixels', weight='bold',
-                            size=label_size)
-
-            if grid[i] and plot_mosaic:
-                if grid_spacing[i] is None:
-                    if cy < 10:
-                        gridspa = 1
-                    elif cy >= 10:
-                        if cy % 2 == 0:
-                            gridspa = 4
-                        else:
-                            gridspa = 5
-                else:
-                    gridspa = grid_spacing[i]
-
-                ax.tick_params(axis='both', which='minor')
-                minor_ticks = np.arange(0, data[i].shape[0], gridspa)
-                ax.set_xticks(minor_ticks, minor=True)
-                ax.set_yticks(minor_ticks, minor=True)
-                ax.grid(True, which='minor', color=grid_color[i], linewidth=0.5,
-                        alpha=grid_alpha[i], linestyle='dashed')
-            else:
-                ax.grid(False)
+                ax.annotate(label[i], xy=(label_pad_x, label_pad_y),
+                            color=label_color[i], xycoords='axes pixels',
+                            weight='bold', size=label_size)
 
             if ang_scale[i] and plot_mosaic:
                 # Converting axes from pixels to arcseconds
                 half_num_ticks = int(np.round(cy // ang_ticksep))
 
+                # Corresponding distance in arcseconds, measured from the center
+                labels_y = []
+                labels_x = []
+                for t in range(half_num_ticks, -half_num_ticks-1, -1):
+                    labels_y.append(
+                        round(Decimal(-t * (ang_ticksep * pxscale)), ndec))
+                    labels_x.append(
+                        round(Decimal(t * (ang_ticksep * pxscale)), ndec))
+
                 # Calculate the pixel locations at which to put ticks
                 ticks = []
                 for t in range(half_num_ticks, -half_num_ticks-1, -1):
                     # Avoid ticks not showing on the last pixel
                     if not cy - t * ang_ticksep == frame_size:
                         ticks.append(cy - t * ang_ticksep)
                     else:
                         ticks.append((cy - t * ang_ticksep)-1)
                 ax.set_xticks(ticks)
                 ax.set_yticks(ticks)
-
-                # Corresponding distance in arcseconds, measured from the center
-                labels_y = []
-                labels_x = []
-                for t in range(half_num_ticks, -half_num_ticks-1, -1):
-                    labels_y.append(
-                        round(Decimal(-t * (ang_ticksep * pxscale)), ndec))
-                    labels_x.append(
-                        round(Decimal(t * (ang_ticksep * pxscale)), ndec))
                 ax.set_xticklabels(labels_x)
                 ax.set_yticklabels(labels_y)
                 ax.set_xlabel('\u0394RA ["]', fontsize=label_size)
                 ax.set_ylabel('\u0394Dec ["]', fontsize=label_size)
-                ax.minorticks_on()
+
+                if ang_ticksep_minor is None:
+                    ax.minorticks_on()
+                else:
+                    # minor ticks
+                    half_num_ticks = int(np.round(cy // ang_ticksep_minor))
+                    minor_ticks = []
+                    for t in range(half_num_ticks, -half_num_ticks-1, -1):
+                        # Avoid ticks not showing on the last pixel
+                        if not cy - t * ang_ticksep_minor == frame_size:
+                            minor_ticks.append(cy - t * ang_ticksep_minor)
+                        else:
+                            minor_ticks.append((cy - t * ang_ticksep_minor)-1)
+                    ax.set_xticks(minor_ticks, minor=True)
+                    ax.set_yticks(minor_ticks, minor=True)
                 ax.tick_params(axis='both', which='both', labelsize=label_size,
                                direction=tick_direction, color=tick_color)
 
             else:
                 ax.set_xlabel("x", fontsize=label_size)
                 ax.set_ylabel("y", fontsize=label_size)
 
+            if grid[i] and plot_mosaic:
+                if grid_spacing[i] is None:
+                    if cy < 10:
+                        gridspa = 1
+                    elif cy >= 10:
+                        if cy % 2 == 0:
+                            gridspa = 4
+                        else:
+                            gridspa = 5
+                else:
+                    gridspa = grid_spacing[i]
+
+                ax.tick_params(axis='both', which='minor')
+                if ang_ticksep_minor is None:
+                    minor_ticks = np.arange(0, data[i].shape[0], gridspa)
+                    ax.set_xticks(minor_ticks, minor=True)
+                    ax.set_yticks(minor_ticks, minor=True)
+                ax.grid(True, which='minor', color=grid_color[i], linewidth=0.5,
+                        alpha=grid_alpha[i], linestyle='dashed')
+            else:
+                ax.grid(False)
+
             if not axis[i]:
                 ax.set_axis_off()
 
             if colorbar[i] and plot_mosaic:
                 divider = make_axes_locatable(ax)
                 # the width of cax is 5% of ax and the padding between cax
                 # and ax wis fixed at 0.05 inch
                 if top_colorbar:
                     cax = divider.append_axes("top", size="5%", pad=0.05)
                     cb = plt_colorbar(
-                        im, ax=ax, cax=cax, drawedges=False, ticks=cbticks, orientation='horizontal')
+                        im, ax=ax, cax=cax, drawedges=False, ticks=cbticks,
+                        orientation='horizontal')
                     cb.ax.xaxis.set_ticks_position('top')
                     cb.ax.xaxis.set_label_position('top')
                 else:
                     cax = divider.append_axes("right", size="5%", pad=0.05)
                     cb = plt_colorbar(im, ax=ax, cax=cax,
                                       drawedges=False, ticks=cbticks)
                 cb.outline.set_linewidth(0.1)
```

### Comparing `hciplot-0.2.5/hciplot.egg-info/PKG-INFO` & `hciplot-0.2.6/hciplot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hciplot
-Version: 0.2.5
+Version: 0.2.6
 Summary: High-contrast Imaging Plotting library
 Home-page: https://github.com/carlgogo/hciplot
 Download-URL: https://github.com/carlgogo/hciplot/archive/refs/tags/v0.1.8.tar.gz
 Author: Carlos Alberto Gomez Gonzalez, Valentin Christiaens
 Author-email: valentinchrist@hotmail.com
 License: MIT
 Keywords: plotting,hci,package
@@ -16,14 +16,20 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib>=3.7.0
+Requires-Dist: holoviews
+Requires-Dist: bokeh
+Requires-Dist: panel
+Requires-Dist: jinja2
 
 [![PyPI version](https://badge.fury.io/py/hciplot.svg)](https://badge.fury.io/py/hciplot)
 
 # HCIplot
 
 ``HCIplot`` -- High-contrast Imaging Plotting library. The goal of this
 library is to be the "Swiss army" solution for plotting and visualizing
```

### Comparing `hciplot-0.2.5/setup.py` & `hciplot-0.2.6/setup.py`

 * *Files identical despite different names*

