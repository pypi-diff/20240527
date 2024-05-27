# Comparing `tmp/distnet2d-0.1.7.tar.gz` & `tmp/distnet2d-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distnet2d-0.1.7.tar", last modified: Wed May 22 20:38:15 2024, max compression
+gzip compressed data, was "distnet2d-0.1.8.tar", last modified: Mon May 27 20:35:19 2024, max compression
```

## Comparing `distnet2d-0.1.7.tar` & `distnet2d-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.671552 distnet2d-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.671552 distnet2d-0.1.7/DiSTNet2D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 20:38:15.000000 distnet2d-0.1.7/DiSTNet2D.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 20:38:12.000000 distnet2d-0.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-22 20:38:15.671552 distnet2d-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-22 20:38:12.000000 distnet2d-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.667552 distnet2d-0.1.7/distnet_2d/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.667552 distnet2d-0.1.7/distnet_2d/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34930 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/dydx_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/medoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/data/swim1d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.667552 distnet2d-0.1.7/distnet_2d/model/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/distnet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/distnet_2d_seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/gradient_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/model/spatial_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:38:15.671552 distnet2d-0.1.7/distnet_2d/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/agc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/metrics_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-05-22 20:38:12.000000 distnet2d-0.1.7/distnet_2d/utils/objectwise_computation_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:38:15.671552 distnet2d-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-22 20:38:12.000000 distnet2d-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:19.496310 distnet2d-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:19.492310 distnet2d-0.1.8/DiSTNet2D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-27 20:35:19.000000 distnet2d-0.1.8/DiSTNet2D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-27 20:35:19.000000 distnet2d-0.1.8/DiSTNet2D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:35:19.000000 distnet2d-0.1.8/DiSTNet2D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 20:35:19.000000 distnet2d-0.1.8/DiSTNet2D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 20:35:19.000000 distnet2d-0.1.8/DiSTNet2D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 20:35:15.000000 distnet2d-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-27 20:35:19.492310 distnet2d-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 20:35:15.000000 distnet2d-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:19.488310 distnet2d-0.1.8/distnet_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:19.492310 distnet2d-0.1.8/distnet_2d/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37579 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/data/dydx_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/data/medoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/data/swim1d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:19.492310 distnet2d-0.1.8/distnet_2d/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/model/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41274 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/model/distnet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/model/distnet_2d_seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/model/gradient_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/model/spatial_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:35:19.492310 distnet2d-0.1.8/distnet_2d/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/agc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/image_derivatives_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/image_derivatives_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/metrics_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-05-27 20:35:15.000000 distnet2d-0.1.8/distnet_2d/utils/objectwise_computation_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:35:19.496310 distnet2d-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-27 20:35:15.000000 distnet2d-0.1.8/setup.py
```

### Comparing `distnet2d-0.1.7/DiSTNet2D.egg-info/PKG-INFO` & `distnet2d-0.1.8/DiSTNet2D.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.7
+Version: 0.1.8
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.7/distnet2d-0.1.7.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.8/distnet2d-0.1.8.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `distnet2d-0.1.7/DiSTNet2D.egg-info/SOURCES.txt` & `distnet2d-0.1.8/DiSTNet2D.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,11 +17,13 @@
 distnet_2d/model/distnet_2d_seg.py
 distnet_2d/model/gradient_accumulator.py
 distnet_2d/model/layers.py
 distnet_2d/model/spatial_attention.py
 distnet_2d/utils/__init__.py
 distnet_2d/utils/agc.py
 distnet_2d/utils/helpers.py
+distnet_2d/utils/image_derivatives_np.py
+distnet_2d/utils/image_derivatives_tf.py
 distnet_2d/utils/losses.py
 distnet_2d/utils/lovasz_loss.py
 distnet_2d/utils/metrics_tf.py
 distnet_2d/utils/objectwise_computation_tf.py
```

### Comparing `distnet2d-0.1.7/LICENSE.txt` & `distnet2d-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/PKG-INFO` & `distnet2d-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.7
+Version: 0.1.8
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.7/distnet2d-0.1.7.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.8/distnet2d-0.1.8.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `distnet2d-0.1.7/README.md` & `distnet2d-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/data/dydx_iterator.py` & `distnet2d-0.1.8/distnet_2d/data/dydx_iterator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 from dataset_iterator import TrackingIterator
 from dataset_iterator.tile_utils import extract_tile_random_zoom_function
 import numpy as np
 import numpy.ma as ma
-from scipy.ndimage import center_of_mass, find_objects, maximum_filter, map_coordinates
+from scipy.ndimage import center_of_mass, find_objects, maximum_filter, map_coordinates, gaussian_filter, convolve
 from skimage.transform import rescale
 from skimage.feature import peak_local_max
 import skfmm
 from math import copysign, isnan
 import sys
 import itertools
 import edt
 from random import random
 from .medoid import get_medoid
+from ..utils import image_derivatives_np as der
+import time
+
+CENTER_MODE = ["GEOMETRICAL", "EDM_MAX", "EDM_MEAN", "SKELETON", "MEDOID"]
+
 
 class DyDxIterator(TrackingIterator):
     def __init__(self,
                  dataset,
                  extract_tile_function,  # = extract_tile_random_zoom_function(tile_shape=(128, 128), n_tiles=8, zoom_range=[0.6, 1.6], aspect_ratio_range=[0.75, 1.5], random_channel_jitter_shape=[50, 50] ),
                  frame_window:int,
                  aug_frame_subsampling,  # either int: frame number interval will be drawn uniformly in [frame_window,aug_frame_subsampling] or callable that generate an frame number interval (int)
                  erase_edge_cell_size:int,
                  next:bool = True,
                  allow_frame_subsampling_direct_neigh:bool = False,
-                 aug_remove_prob: float = 0.01,
+                 aug_remove_prob: float = 0.005,
                  return_link_multiplicity:bool = True,
                  channel_keywords:list=['/raw', '/regionLabels'],  # channel @1 must be label
                  array_keywords:list=['/linksPrev'],
                  elasticdeform_parameters:dict = None,
                  downscale_displacement_and_link_multiplicity=1,
-                 return_center = True,
-                 center_mode = "MEDOID",  # GEOMETRICAL, "EDM_MAX", "EDM_MEAN", "SKELETON", "MEDOID"
+                 return_edm_derivatives: bool = False,
+                 return_center:bool = True,
+                 center_mode:str = "MEDOID",  # GEOMETRICAL, "EDM_MAX", "EDM_MEAN", "SKELETON", "MEDOID"
                  return_label_rank = False,
                  long_term:bool = True,
                  return_next_displacement:bool = True,
                  output_float16=False,
                  **kwargs):
         assert len(channel_keywords)==2, 'keyword should contain 2 elements in this order: grayscale input images, object labels'
         assert len(array_keywords) == 1, 'array keyword should contain 1 element: links to previous objects'
+        assert center_mode.upper() in CENTER_MODE, f"invalid center mode: {center_mode} should be in {CENTER_MODE}"
         self.return_link_multiplicity=return_link_multiplicity
         self.downscale=downscale_displacement_and_link_multiplicity
         self.erase_edge_cell_size=erase_edge_cell_size
         self.aug_frame_subsampling=aug_frame_subsampling
         self.allow_frame_subsampling_direct_neigh=allow_frame_subsampling_direct_neigh
         self.output_float16=output_float16
+        self.return_edm_derivatives=return_edm_derivatives
         self.return_center=return_center
-        self.center_mode=center_mode
+        self.center_mode=center_mode.upper()
         self.return_label_rank=return_label_rank
         assert frame_window>=1, "frame_window must be >=1"
         self.frame_window = frame_window
         self.return_next_displacement=return_next_displacement
         self.n_label_max = kwargs.pop("n_label_max", 2000)
         self.long_term=long_term if self.frame_window>1 else False
         self.return_central_only = False
@@ -213,30 +221,34 @@
             self._erase_small_objects_at_edges(labelIms[i,...,frame_window], i, mask_to_erase_cur, mask_to_erase_chan_cur, batch_by_channel)
             # prev timepoints
             for j in range(0, frame_window):
                 self._erase_small_objects_at_edges(labelIms[i,...,j], i, mask_to_erase_prev, [m+j for m in mask_to_erase_chan_prev], batch_by_channel)
             if return_next:
                 for j in range(0, frame_window):
                     self._erase_small_objects_at_edges(labelIms[i,...,frame_window+1+j], i, mask_to_erase_next, [m+j for m in mask_to_erase_chan_next], batch_by_channel)
+        object_slices = {}
+        for b, c in itertools.product(range(labelIms.shape[0]), range(labelIms.shape[-1])):
+            object_slices[(b, c)] = find_objects(labelIms[b,...,c])
         edm = np.zeros(shape=labelIms.shape, dtype=np.float32)
         for b,c in itertools.product(range(edm.shape[0]), range(edm.shape[-1])):
-            edm[b,...,c] = edt.edt(labelIms[b,...,c], black_border=False)
+            edm[b,...,c] = edt_smooth(labelIms[b,...,c], object_slices[(b, c)])
+            #edm[b,...,c] = edt.edt(labelIms[b,...,c], black_border=False)
         n_motion = 2 * frame_window if return_next else frame_window
         if long_term:
             n_motion = n_motion + (2 * ( frame_window - 1 ) if return_next else frame_window -1)
         dyIm = np.zeros(labelIms.shape[:-1]+(n_motion,), dtype=self.dtype)
         dxIm = np.zeros(labelIms.shape[:-1]+(n_motion,), dtype=self.dtype)
         if ndisp:
             dyImNext = np.zeros(labelIms.shape[:-1]+(n_motion,), dtype=self.dtype)
             dxImNext = np.zeros(labelIms.shape[:-1]+(n_motion,), dtype=self.dtype)
             if self.return_link_multiplicity:
                 linkMultiplicityImNext = np.zeros(labelIms.shape[:-1]+(n_motion,), dtype=self.dtype)
         centerIm = np.zeros(labelIms.shape, dtype=self.dtype) if self.return_center else None
         if self.return_label_rank:
-            labelIm = np.zeros(labelIms.shape, dtype=np.int32)
+            rankIm = np.zeros(labelIms.shape, dtype=np.int32)
             prevLabelArr = np.zeros(labelIms.shape[:1]+(n_motion, self.n_label_max), dtype=np.int32)
             nextLabelArr = np.zeros(labelIms.shape[:1] + (n_motion, self.n_label_max), dtype=np.int32)
             centerArr = np.zeros(labelIms.shape[:1]+labelIms.shape[-1:]+(self.n_label_max,2), dtype=np.float32)
             centerArr.fill(np.nan)
         if self.return_link_multiplicity:
             linkMultiplicityIm = np.zeros(labelIms.shape[:-1]+(n_motion,), dtype=self.dtype)
 
@@ -251,54 +263,67 @@
         for b,c in itertools.product(range(labelIms.shape[0]), range(labelIms.shape[-1])):
             labels_and_centers[(b, c)] = _get_labels_and_centers(labelIms[b][...,c], edm[b][...,c], self.center_mode)
         for i in range(labelIms.shape[0]):
             bidx = get_idx(i)
             for c in range(0, frame_window):
                 sel = [c, c+1]
                 l_c = [labels_and_centers[(i,s)] for s in sel]
-                _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c], dyIm[i,...,c], dxIm[i,...,c], dyImNext=dyImNext[i,...,c] if ndisp else None, dxImNext=dxImNext[i,...,c] if ndisp else None, gdcmIm=centerIm[i,...,frame_window] if self.return_center and sel[1] == frame_window else None, gdcmImPrev=centerIm[i,...,c] if self.return_center else None, linkMultiplicityIm=linkMultiplicityIm[i,...,c] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,...,c] if self.return_link_multiplicity and ndisp else None, rankIm=labelIm[i,...,frame_window] if self.return_label_rank and sel[1] == frame_window else None, rankImPrev=labelIm[i,...,c] if self.return_label_rank else None, prevLabelArr=prevLabelArr[i,c] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i,c] if self.return_label_rank and ndisp else None, centerArr=centerArr[i,frame_window] if self.return_label_rank and sel[1] == frame_window else None, centerArrPrev=centerArr[i,c] if self.return_label_rank else None, center_mode=self.center_mode)
+                o_s = [object_slices[(i, s)] for s in sel]
+                _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c], o_s, dyIm[i,...,c], dxIm[i,...,c], dyImNext=dyImNext[i,...,c] if ndisp else None, dxImNext=dxImNext[i,...,c] if ndisp else None, gdcmIm=centerIm[i,...,frame_window] if self.return_center and sel[1] == frame_window else None, gdcmImPrev=centerIm[i,...,c] if self.return_center else None, linkMultiplicityIm=linkMultiplicityIm[i,...,c] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,...,c] if self.return_link_multiplicity and ndisp else None, rankIm=rankIm[i,...,frame_window] if self.return_label_rank and sel[1] == frame_window else None, rankImPrev=rankIm[i,...,c] if self.return_label_rank else None, prevLabelArr=prevLabelArr[i,c] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i,c] if self.return_label_rank and ndisp else None, centerArr=centerArr[i,frame_window] if self.return_label_rank and sel[1] == frame_window else None, centerArrPrev=centerArr[i,c] if self.return_label_rank else None, center_mode=self.center_mode)
             if return_next:
                 for c in range(frame_window, 2*frame_window):
                     sel = [c, c+1]
                     l_c = [labels_and_centers[(i, s)] for s in sel]
-                    _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c], dyIm[i,...,c], dxIm[i,...,c], dyImNext=dyImNext[i,...,c] if ndisp else None, dxImNext=dxImNext[i,...,c] if ndisp else None, gdcmIm=centerIm[i,..., c + 1] if self.return_center else None, gdcmImPrev=None, linkMultiplicityIm=linkMultiplicityIm[i,...,c] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,...,c] if self.return_link_multiplicity and ndisp else None, rankIm=labelIm[i,..., c + 1] if self.return_label_rank else None, rankImPrev=None, prevLabelArr=prevLabelArr[i,c] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i,c] if self.return_label_rank and ndisp else None, centerArr=centerArr[i, c + 1] if self.return_label_rank else None, center_mode=self.center_mode)
+                    o_s = [object_slices[(i, s)] for s in sel]
+                    _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c], o_s, dyIm[i,...,c], dxIm[i,...,c], dyImNext=dyImNext[i,...,c] if ndisp else None, dxImNext=dxImNext[i,...,c] if ndisp else None, gdcmIm=centerIm[i,..., c + 1] if self.return_center else None, gdcmImPrev=None, linkMultiplicityIm=linkMultiplicityIm[i,...,c] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,...,c] if self.return_link_multiplicity and ndisp else None, rankIm=rankIm[i,..., c + 1] if self.return_label_rank else None, rankImPrev=None, prevLabelArr=prevLabelArr[i,c] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i,c] if self.return_label_rank and ndisp else None, centerArr=centerArr[i, c + 1] if self.return_label_rank else None, center_mode=self.center_mode)
             if long_term:
                 off = 2*frame_window if return_next else frame_window
                 for c in range(0, frame_window-1):
                     sel = [c, frame_window]
                     l_c = [labels_and_centers[(i, s)] for s in sel]
-                    _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c+off], dyIm[i,...,c+off], dxIm[i,...,c+off], dyImNext=dyImNext[i,...,c+off] if ndisp else None, dxImNext=dxImNext[i,...,c+off] if ndisp else None, gdcmIm=None, gdcmImPrev=None, linkMultiplicityIm=linkMultiplicityIm[i,..., c + off] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,..., c + off] if self.return_link_multiplicity and ndisp else None, rankIm=None, rankImPrev=None, prevLabelArr=prevLabelArr[i, c + off] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i, c + off] if self.return_label_rank and ndisp else None, center_mode=self.center_mode)
+                    o_s = [object_slices[(i, s)] for s in sel]
+                    _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c+off], o_s, dyIm[i,...,c+off], dxIm[i,...,c+off], dyImNext=dyImNext[i,...,c+off] if ndisp else None, dxImNext=dxImNext[i,...,c+off] if ndisp else None, gdcmIm=None, gdcmImPrev=None, linkMultiplicityIm=linkMultiplicityIm[i,..., c + off] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,..., c + off] if self.return_link_multiplicity and ndisp else None, rankIm=None, rankImPrev=None, prevLabelArr=prevLabelArr[i, c + off] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i, c + off] if self.return_label_rank and ndisp else None, center_mode=self.center_mode)
                 if return_next:
                     for c in range(frame_window-1, 2*(frame_window-1)):
                         sel = [frame_window, c+3]
                         l_c = [labels_and_centers[(i, s)] for s in sel]
-                        _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c+off], dyIm[i,...,c+off], dxIm[i,...,c+off], dyImNext=dyImNext[i,...,c+off] if ndisp else None, dxImNext=dxImNext[i,...,c+off] if ndisp else None, gdcmIm=None, gdcmImPrev=None, linkMultiplicityIm=linkMultiplicityIm[i,..., c + off] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,..., c + off] if self.return_link_multiplicity and ndisp else None, rankIm=None, rankImPrev=None, prevLabelArr=prevLabelArr[i, c + off] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i, c + off] if self.return_label_rank and ndisp else None, center_mode=self.center_mode)
-        other_output_channels = [chan_idx for chan_idx in self.output_channels if chan_idx!=1 and chan_idx!=2]
-        all_channels = [batch_by_channel[chan_idx] for chan_idx in other_output_channels]
-        channel_inc = 0
+                        o_s = [object_slices[(i, s)] for s in sel]
+                        _compute_displacement(l_c, labelIms[i][...,sel], labels_map_prev[bidx][c+off], o_s, dyIm[i,...,c+off], dxIm[i,...,c+off], dyImNext=dyImNext[i,...,c+off] if ndisp else None, dxImNext=dxImNext[i,...,c+off] if ndisp else None, gdcmIm=None, gdcmImPrev=None, linkMultiplicityIm=linkMultiplicityIm[i,..., c + off] if self.return_link_multiplicity else None, linkMultiplicityImNext=linkMultiplicityImNext[i,..., c + off] if self.return_link_multiplicity and ndisp else None, rankIm=None, rankImPrev=None, prevLabelArr=prevLabelArr[i, c + off] if self.return_label_rank else None, nextLabelArr=nextLabelArr[i, c + off] if self.return_label_rank and ndisp else None, center_mode=self.center_mode)
+
+        edm[edm == 0] = -1
+        if self.return_edm_derivatives:
+            der_y, der_x = np.zeros_like(edm), np.zeros_like(edm)
+            for b, c in itertools.product(range(edm.shape[0]), range(edm.shape[-1])):
+                derivatives_labelwise(edm[b, ..., c], -1, der_y[b, ..., c], der_x[b, ..., c], labelIms[b, ..., c],  object_slices[(b, c)])
+            if self.return_central_only:
+                der_y = der_y[..., 1:2]
+                der_x = der_x[..., 1:2]
         if self.return_central_only: # select only central frame for edm / center and only displacement / link multiplicity related to central frame
             edm = edm[..., 1:2]
             centerIm = centerIm[..., 1:2]
             dyIm = dyIm[..., :1]
             dxIm = dxIm[..., :1]
             if self.return_link_multiplicity:
                 linkMultiplicityIm = linkMultiplicityIm[..., :1]
             if ndisp:
                 dyImNext = dyImNext[..., 1:]
                 dxImNext = dxImNext[..., 1:]
                 if self.return_link_multiplicity:
                     linkMultiplicityImNext = linkMultiplicityImNext[..., 1:]
             if self.return_label_rank:
-                labelIm = labelIm[..., 1:2]
+                rankIm = rankIm[..., 1:2]
                 centerArr = centerArr[: , 1:2]
                 prevLabelArr = prevLabelArr[:, :1]
                 if ndisp:
                     nextLabelArr = nextLabelArr[:, 1:]
-
-        edm[edm==0] = -1
+        if self.return_edm_derivatives:
+            edm = np.concatenate([edm, der_y, der_x], -1)
+        other_output_channels = [chan_idx for chan_idx in self.output_channels if chan_idx != 1 and chan_idx != 2]
+        all_channels = [batch_by_channel[chan_idx] for chan_idx in other_output_channels]
+        channel_inc = 0
         all_channels.insert(channel_inc, edm)
         if self.return_center:
             channel_inc+=1
             all_channels.insert(channel_inc, centerIm)
         downscale_factor = 1./self.downscale if self.downscale>1 else 0
         scale = [1, downscale_factor, downscale_factor, 1]
         if self.downscale>1:
@@ -325,15 +350,15 @@
         if self.output_float16:
             for i, c in enumerate(all_channels):
                 if not (self.return_link_multiplicity and i == 3 + channel_inc or self.return_label_rank and (i == channel_inc or i == channel_inc + 1)): # softmax / sigmoid activation -> float32
                     all_channels[i] = c.astype('float16', copy=False)
         if self.return_label_rank:
             if ndisp:
                 prevLabelArr = np.concatenate([prevLabelArr, nextLabelArr], 1)
-            all_channels.append(labelIm)
+            all_channels.append(rankIm)
             all_channels.append(prevLabelArr)
             all_channels.append(centerArr)
         return all_channels
 
     def _erase_small_objects_at_edges(self, labelImage, batch_idx, channel_idxs, channel_idxs_chan, batch_by_channel):
         objects_to_erase = _get_small_objects_at_edges_to_erase(labelImage, self.erase_edge_cell_size)
         if len(objects_to_erase)>0:
@@ -367,39 +392,25 @@
         return dict()
     if center_mode == "GEOMETRICAL":
         centers = center_of_mass(labelIm, labelIm, labels)
     elif center_mode == "EDM_MAX":
         assert edm is not None and edm.shape == labelIm.shape
         centers = []
         for label in labels:
-            edm_label = ma.array(edm, mask = labelIm != label)
+            edm_label = ma.array(edm, mask=labelIm != label)
             center = ma.argmax(edm_label, fill_value=0)
             center = np.unravel_index(center, edm_label.shape)
             centers.append(center)
     elif center_mode == "EDM_MEAN":
         assert edm is not None and edm.shape == labelIm.shape
         centers = center_of_mass(edm, labelIm, labels)
     elif center_mode == "SKELETON":
-        assert edm is not None and edm.shape == labelIm.shape
-        mass_centers = np.array(center_of_mass(labelIm, labelIm, labels))[np.newaxis] # 1, N_ob, 2
-        lm_coords = peak_local_max(edm, labels = labelIm) # N_lm, 2
-        lm_coords_l = labelIm[lm_coords[:,0], lm_coords[:,1]] # N_lm
-        # labels in labelIm are not necessarily continuous -> replace by rank
-        label_rank = np.zeros(shape=(max(labels)+1,), dtype=np.int32)
-        for l in labels:
-            label_rank[l] = labels.index(l)
-        lm_coords_l = label_rank[lm_coords_l]
-        lm_coords_l = np.eye(len(labels))[lm_coords_l] # N_lm, N_ob
-        lm_coords_ob = lm_coords[:,np.newaxis] * lm_coords_l[...,np.newaxis] # N_lm, N_ob, 1 # TODO medoid of local maxima, weighted by edm?
-        lm_coords_dist = np.sum(np.square(mass_centers - lm_coords_ob), 2, keepdims=True) # N_lm, N_ob, 1
-        lm_coords_dinv= 1./(lm_coords_dist + 0.1) # N_lm, N_ob, 1
-        lm_coords_dinv = lm_coords_dinv * lm_coords_ob # erase weights that are outside object
-        wsum=np.sum(lm_coords_ob * lm_coords_dinv, 0, keepdims=False) # N_ob, 2
-        sum=np.sum(lm_coords_dinv, 0, keepdims=False) # N_ob, 1
-        centers = wsum / sum # N_ob, 2
+        edm_lap = der.laplacian_2d(gaussian_filter(edm, sigma=1.5))
+        skeleton = edm_lap<0.25
+        centers = [get_medoid(*np.asarray( (labelIm == l) & skeleton).nonzero()) for l in labels]
     elif center_mode == "MEDOID":
         centers = [get_medoid(*np.asarray(labelIm == l).nonzero()) for l in labels]
     else:
         raise ValueError(f"Invalid center mode: {center_mode}")
     return dict(zip(labels, centers))
 
 # channel dimension = frames
@@ -476,15 +487,15 @@
     if n_neigh == 0:
         return 3
     elif n_neigh == 1:
         return 1
     else:
         return 2
 
-def _compute_displacement(labels_map_centers, labelIm, labels_map_prev, dyIm, dxIm, dyImNext=None, dxImNext=None, gdcmIm=None, gdcmImPrev=None, linkMultiplicityIm=None, linkMultiplicityImNext=None, rankIm=None, rankImPrev=None, prevLabelArr=None, nextLabelArr=None, centerArr=None, centerArrPrev=None, center_mode:str= "MEDOID"):
+def _compute_displacement(labels_map_centers, labelIm, labels_map_prev, object_slices, dyIm, dxIm, dyImNext=None, dxImNext=None, gdcmIm=None, gdcmImPrev=None, linkMultiplicityIm=None, linkMultiplicityImNext=None, rankIm=None, rankImPrev=None, prevLabelArr=None, nextLabelArr=None, centerArr=None, centerArrPrev=None, center_mode:str= "MEDOID"):
     assert labelIm.shape[-1] == 2, f"invalid labelIm : {labelIm.shape[-1]} channels instead of 2"
     assert (dxImNext is None) == (dyImNext is None)
     if len(labels_map_centers[-1])==0: # no cells
         return
     curLabelIm = labelIm[...,-1]
     labels_prev = labels_map_centers[0].keys()
     labels_prev_rank = {l:r for r, l in enumerate(labels_prev)}
@@ -522,46 +533,85 @@
                     nextLabelArr[rank] = labels_next_rank[label_next]+1
             if linkMultiplicityImNext is not None:
                 linkMultiplicityImNext[mask] = _get_category(len(label_nexts))
             if rankImPrev is not None:
                 rankImPrev[mask] = rank + 1
     if gdcmIm is not None:
         assert gdcmIm.shape == dyIm.shape, "invalid shape for center image"
-        _draw_centers(gdcmIm, labels_map_centers[-1], labelIm[...,1], geometrical_distance=center_mode == "GEOMETRICAL")
+        _draw_centers(gdcmIm, labels_map_centers[-1], labelIm[...,1], object_slices[1], geometrical_distance=center_mode == "GEOMETRICAL")
     if gdcmImPrev is not None:
         assert gdcmImPrev.shape == dyIm.shape, "invalid shape for center image prev"
-        _draw_centers(gdcmImPrev, labels_map_centers[0], labelIm[...,0], geometrical_distance=center_mode == "GEOMETRICAL")
+        _draw_centers(gdcmImPrev, labels_map_centers[0], labelIm[...,0], object_slices[0], geometrical_distance=center_mode == "GEOMETRICAL")
     if centerArr is not None:
         for rank, (label, center) in enumerate(labels_map_centers[-1].items()):
             centerArr[rank,0] = center[0]
             centerArr[rank,1] = center[1]
     if centerArrPrev is not None:
         for rank, (label, center) in enumerate(labels_map_centers[0].items()):
             centerArrPrev[rank,0] = center[0]
             centerArrPrev[rank,1] = center[1]
 
-def _draw_centers(centerIm, labels_map_centers, labelIm, geometrical_distance:bool=False):
+def _draw_centers(centerIm, labels_map_centers, labelIm, object_slices, geometrical_distance:bool=False):
     if len(labels_map_centers)==0:
         return
     # geodesic distance to center
     if not geometrical_distance:
-        count = 0
-        m = np.ones_like(labelIm)
-        for center in labels_map_centers.values():
-            if not (isnan(center[0]) or isnan(center[1])):
-                m[int(round(center[0])), int(round(center[1]))] = 0
-                count+=1
-        if count>0:
-            m = ma.masked_array(m, ~labelIm.astype(bool))
-            centerIm[:] = skfmm.distance(m)
+        shape = centerIm.shape
+        labelIm_dil = maximum_filter(labelIm, size=5)
+        non_zero = labelIm>0
+        labelIm_dil[non_zero] = labelIm[non_zero]
+        for (i, sl) in enumerate(object_slices):
+            if sl is not None:
+                center = labels_map_centers.get(i+1)
+                if not (isnan(center[0]) or isnan(center[1])):
+                    sl = tuple( [slice(max(0, s.start - 2), min(s.stop + 2, ax), s.step) for s, ax in zip(sl, shape)])
+                    mask = labelIm_dil[sl] == i + 1
+                    m = np.ones_like(mask)
+                    #print(f"label: {i+1} slice: {sl}, center: {center}, sub_m {sub_m.shape}, coord: {(int(round(center[0]))-sl[0].start, int(round(center[1]))-sl[1].start)}", flush=True)
+                    m[int(round(center[0]))-sl[0].start, int(round(center[1]))-sl[1].start] = 0
+                    m = ma.masked_array(m, ~mask)
+                    centerIm[sl][mask] = skfmm.distance(m)[mask]
     else:
         Y, X = centerIm.shape
         Y, X = np.meshgrid(np.arange(Y, dtype = np.float32), np.arange(X, dtype = np.float32), indexing = 'ij')
         for i, (label, center) in enumerate(labels_map_centers.items()): # in case center prediction is a classification
             if isnan(center[0]) or isnan(center[1]):
                 pass
             else:
                 # distance to center
                 mask = labelIm==label
                 if mask.sum()>0:
                     d = np.sqrt(np.square(Y-center[0])+np.square(X-center[1]))
                     centerIm[mask] = d[mask]
+
+
+def edt_smooth(labelIm, object_slices):
+    shape = labelIm.shape
+    upsampled = np.kron(labelIm, np.ones((2, 2))) # upsample by factor 2
+    w=np.ones(shape=(3, 3), dtype=np.int8)
+    for (i, sl) in enumerate(object_slices):
+        if sl is not None:
+            sl = tuple([slice(max(s.start*2 - 1, 0), min(s.stop*2 + 1, ax*2), s.step) for s, ax in zip(sl, shape)])
+            sub_labelIm = upsampled[sl]
+            mask = sub_labelIm == i + 1
+            new_mask = convolve(mask.astype(np.int8), weights=w, mode="nearest") > 4 # smooth borders
+            sub_labelIm[mask] = 0  # replace mask by smoothed
+            sub_labelIm[new_mask] = i + 1
+    edm = edt.edt(upsampled)
+    edm = edm.reshape((shape[0], 2, shape[1], 2)).mean(-1).mean(1) # downsample (bin) by factor 2
+    edm = np.divide(edm + 0.5, 2)  #convert to pixel unit
+    edm[edm <= 0.5] = 0
+    return edm
+
+
+def derivatives_labelwise(image, bck_value, der_y, der_x, labelIm, object_slices):
+    shape = labelIm.shape
+    for (i, sl) in enumerate(object_slices):
+        if sl is not None:
+            sl = tuple([slice(max(s.start - 1, 0), min(s.stop + 1, ax), s.step) for s, ax in zip(sl, shape)])
+            mask = labelIm[sl] == i + 1
+            sub_im = np.copy(image[sl])
+            sub_im[np.logical_not(mask)] = bck_value # erase neighboring cells
+            sub_der_y, sub_der_x = der.der_2d(sub_im, 0, 1)
+            der_y[sl][mask] = sub_der_y[mask]
+            der_x[sl][mask] = sub_der_x[mask]
+    return der_y, der_x
```

### Comparing `distnet2d-0.1.7/distnet_2d/data/swim1d.py` & `distnet2d-0.1.8/distnet_2d/data/swim1d.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/model/architectures.py` & `distnet2d-0.1.8/distnet_2d/model/architectures.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/model/distnet_2d.py` & `distnet2d-0.1.8/distnet_2d/model/distnet_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import tensorflow as tf
 from .layers import ker_size_to_string, Combine, ResConv2D, Conv2DBNDrop, Conv2DTransposeBNDrop, WSConv2D, BatchToChannel, SplitBatch, ChannelToBatch, NConvToBatch2D, SelectFeature
 import numpy as np
 from .spatial_attention import SpatialAttention2D
 from ..utils.helpers import ensure_multiplicity, flatten_list
-from ..utils.losses import weighted_loss_by_category, balanced_category_loss, PseudoHuber
+from ..utils.losses import weighted_loss_by_category, balanced_category_loss, PseudoHuber, compute_loss_derivatives
 from ..utils.agc import adaptive_clip_grad
 from .gradient_accumulator import GradientAccumulator
+
 import time
 
 class DiSTNetModel(tf.keras.Model):
     def __init__(self, *args, spatial_dims,
                  edm_loss_weight:float=1,
                  center_loss_weight:float=1,
                  displacement_loss_weight:float=1,
                  category_loss_weight:float=1,
-                 edm_loss=PseudoHuber(1),
-                 gcdm_loss=PseudoHuber(1), gcdm_gradients:bool=False,
+                 edm_loss=PseudoHuber(1), edm_derivative_loss:bool=False,
+                 gcdm_loss=PseudoHuber(1), gcdm_derivative_loss:bool=False,
                  displacement_loss=PseudoHuber(1),
                  category_weights=None,  # array of weights: [normal, division, no previous cell] or None = auto
                  category_class_frequency_range=[1/50, 50],
                  next=True,
                  frame_window=3,
                  long_term:bool=True,
                  predict_next_displacement:bool=True,
+                 predict_gcdm_derivatives:bool=False, predict_edm_derivatives:bool=False,
                  print_gradients:bool=False,  # for optimization, available in eager mode only
                  accum_steps=1, use_agc=False, agc_clip_factor=0.1, agc_eps=1e-3, agc_exclude_output=False,  # lower clip factor clips more
                  **kwargs):
         super().__init__(*args, **kwargs)
         self.edm_weight = edm_loss_weight
         self.center_weight = center_loss_weight
         self.displacement_weight = displacement_loss_weight
         self.category_weight = category_loss_weight
         self.spatial_dims = spatial_dims
         self.next = next
         self.predict_next_displacement=predict_next_displacement
         self.frame_window = frame_window
         self.edm_loss = edm_loss
-        self.gdcm_loss=gcdm_loss
-        self.gcdm_gradients=gcdm_gradients
+        self.edm_derivative_loss = edm_derivative_loss
+        self.gcdm_loss = gcdm_loss
+        self.gcdm_derivative_loss = gcdm_derivative_loss
         self.displacement_loss = displacement_loss
-
+        self.predict_gcdm_derivatives = predict_gcdm_derivatives
+        self.predict_edm_derivatives = predict_edm_derivatives
         min_class_frequency=category_class_frequency_range[0]
         max_class_frequency=category_class_frequency_range[1]
         if category_weights is not None:
             assert len(category_weights)==3, "3 category weights should be provided: normal cell, dividing cell, cell with no previous cell"
             self.category_loss=weighted_loss_by_category(tf.keras.losses.CategoricalCrossentropy(), category_weights, remove_background=True)
         else:
             self.category_loss = balanced_category_loss(tf.keras.losses.CategoricalCrossentropy(),3, min_class_frequency=min_class_frequency, max_class_frequency=max_class_frequency, remove_background=True)
@@ -52,15 +56,15 @@
         self.use_grad_acc = accum_steps>1
         self.accum_steps = float(accum_steps)
         if self.use_grad_acc or use_agc:
             self.gradient_accumulator = GradientAccumulator(accum_steps, self)
         self.use_agc = use_agc
         self.agc_clip_factor = agc_clip_factor
         self.agc_eps = agc_eps
-        self.agc_exclude_keywords=["DecoderTrackY0/, DecoderTrackX0/", "DecoderCat0/", "DecoderCenter0/", "DecoderSegEDM0"] if agc_exclude_output else None
+        self.agc_exclude_keywords=["DecoderTrackY0/, DecoderTrackX0/", "DecoderCat0/", "DecoderCenterGCDM0/", "DecoderCenterGCDMdY0/", "DecoderCenterGCDMdX0/", "DecoderSegEDM0/", "DecoderSegEDMdY0/", "DecoderSegEDMdX0/"] if agc_exclude_output else None
         self.print_gradients=print_gradients
 
     def train_step(self, data):
         if self.use_grad_acc:
             self.gradient_accumulator.init_train_step()
 
         fw = self.frame_window
@@ -74,39 +78,51 @@
         displacement_weight = self.displacement_weight / (2. * n_fp_mul) # y & x
         category_weight = self.category_weight / (n_fp_mul * float(n_frame_pairs))
         edm_weight = self.edm_weight / float(n_frames) # divide by channel number ?
         center_weight = self.center_weight / float(n_frames)# divide by channel number ?
         if category_weight>0:
             assert len(y) == 5 , f"invalid number of output. Expected: >=4 actual {len(y)}" # 0 = edm, 1 = center, 2 = dY, 3 = dX, 4 = cat
         else:
-            assert len(y) >= 4, f"invalid number of output. Expected: >=4 actual {len(y)}"  # 0 = edm, 1 = center, 2 = dY, 3 = dX, 4 = cat
+            assert len(y) >= 4, f"invalid number of output. Expected: >=4 actual {len(y)}"  # 0 = edm, 1 = center, 2 = dY, 3 = dX
 
         with tf.GradientTape(persistent=self.print_gradients) as tape:
             y_pred = self(x, training=True)  # Forward pass
+            if self.predict_edm_derivatives:
+                edm, edm_dy, edm_dx = tf.split(y_pred[0], num_or_size_splits=3, axis=-1)
+            else:
+                edm, edm_dy, edm_dx = y_pred[0], None, None
+            if self.predict_gcdm_derivatives:
+                gcdm, gcdm_dy, gcdm_dx = tf.split(y_pred[1], num_or_size_splits=3, axis=-1)
+            else:
+                gcdm, gcdm_dy, gcdm_dx = y_pred[1], None, None
+            if self.predict_edm_derivatives or self.edm_derivative_loss:
+                true_edm, true_edm_dy, true_edm_dx = tf.split(y[0], num_or_size_splits=3, axis=-1)
+            else:
+                true_edm, true_edm_dy, true_edm_dx = y[0], None, None
             # compute loss
             losses = dict()
             loss_weights = dict()
 
-            cell_mask = tf.math.greater(y[0], 0)
+            cell_mask = tf.math.greater(true_edm, 0.5)
+            cell_mask_interior = tf.math.greater(true_edm, 1.5) if self.gcdm_derivative_loss or self.predict_gcdm_derivatives else None
             # edm
             if edm_weight>0:
-                edm_loss = self.edm_loss(y[0], y_pred[0]) #, sample_weight = weight_map)
+                edm_loss = compute_loss_derivatives(true_edm, edm, self.edm_loss, true_dy=true_edm_dy, true_dx=true_edm_dx, pred_dy=edm_dy, pred_dx=edm_dx, derivative_loss=self.edm_derivative_loss, laplacian_loss=self.edm_derivative_loss)
                 losses["edm"] = edm_loss
                 loss_weights["edm"] = edm_weight
 
             # center
             if center_weight>0:
-                center_pred_inside=tf.where(cell_mask, y_pred[1], 0) # do not predict anything outside
-                center_loss = self.gdcm_loss(y[1], center_pred_inside)
+                center_loss = compute_loss_derivatives(y[1], gcdm, self.gcdm_loss, pred_dy=gcdm_dy, pred_dx=gcdm_dx, mask=cell_mask, mask_interior=cell_mask_interior, derivative_loss=self.gcdm_derivative_loss)
                 losses["center"] = center_loss
                 loss_weights["center"] = center_weight
 
             #regression displacement loss
             if displacement_weight>0:
-                loss_dY, loss_dX = self._compute_displacement_loss(y, y_pred, cell_mask, spatial_gradients=self.gcdm_gradients)
+                loss_dY, loss_dX = self._compute_displacement_loss(y, y_pred, cell_mask)
                 losses["dY"] = loss_dY
                 loss_weights["dY"] = displacement_weight
                 losses["dX"] = loss_dX
                 loss_weights["dX"] = displacement_weight
 
             # category loss
             if category_weight>0:
@@ -121,15 +137,15 @@
 
             # print(f"reg loss: {len(self.losses)} values: {self.losses}")
             if len(self.losses)>0:
                 loss += tf.add_n(self.losses) # regularizers
             losses["loss"] = loss
 
         if self.print_gradients:
-            trainable_vars_tape = [t for t in self.trainable_variables if (t.name.startswith("DecoderSegEDM") or t.name.startswith("DecoderCenter0") or t.name.startswith("DecoderTrackY0") or t.name.startswith("DecoderTrackX0") or t.name.startswith("DecoderCat0") or t.name.startswith("FeatureSequence/Op4") or t.name.startswith("Attention")) and ("/kernel" in t.name or "/wv" in t.name) ]
+            trainable_vars_tape = [t for t in self.trainable_variables if (t.name.startswith("DecoderSegEDM") or t.name.startswith("DecoderCenterGCDM") or t.name.startswith("DecoderTrackY0") or t.name.startswith("DecoderTrackX0") or t.name.startswith("DecoderCat0") or t.name.startswith("FeatureSequence/Op4") or t.name.startswith("Attention")) and ("/kernel" in t.name or "/wv" in t.name) ]
             for loss_name, loss_value in losses.items():
                 if loss_name != "loss" :
                     w = loss_weights[loss_name] # outside tape: cannot modify loss_value -> need to apply w to gradient itself
                     if mixed_precision:
                         loss_value = self.optimizer.get_scaled_loss(loss_value)
                     gradients = tape.gradient(loss_value, trainable_vars_tape)
                     if mixed_precision:
@@ -153,45 +169,42 @@
         if not self.use_grad_acc:
             self.optimizer.apply_gradients(zip(gradients, self.trainable_variables)) #Update weights
         else:
             self.gradient_accumulator.accumulate_gradients(gradients)
             self.gradient_accumulator.apply_gradients()
         return losses
 
-    def _compute_displacement_loss(self, y, y_pred, cell_mask, spatial_gradients:bool=False):
+    def _compute_displacement_loss(self, y, y_pred, cell_mask):
+        mask = self._to_pair_mask(cell_mask)
+        dy = tf.where(mask, y_pred[2], 0)  # do not predict anything outside
+        dx = tf.where(mask, y_pred[3], 0)  # do not predict anything outside
+        return self.displacement_loss(y[2], dy), self.displacement_loss(y[3], dx)
+
+    def _to_pair_mask(self, cell_mask):
         fw = self.frame_window
         mask = cell_mask[..., 1:]
         if self.predict_next_displacement:
             mask_next = cell_mask[..., :-1]
         if self.long_term and fw > 1:
             mask_center = tf.tile(mask[..., fw - 1:fw], [1, 1, 1, fw - 1])
             if self.predict_next_displacement:
                 if self.next:
-                    mask = tf.concat( [mask, mask_center, cell_mask[..., -fw + 1:], mask_next, cell_mask[..., :fw - 1], mask_center], -1)
+                    mask = tf.concat(
+                        [mask, mask_center, cell_mask[..., -fw + 1:], mask_next, cell_mask[..., :fw - 1], mask_center],
+                        -1)
                 else:
                     mask = tf.concat([mask, mask_center, mask_next, cell_mask[..., :fw - 1]], -1)
             else:
                 if self.next:
                     mask = tf.concat([mask, mask_center, cell_mask[..., -fw + 1:]], -1)
                 else:
                     mask = tf.concat([mask, mask_center], -1)
         elif self.predict_next_displacement:
             mask = tf.concat([mask, mask_next], -1)
-
-        dy_inside = tf.where(mask, y_pred[2], 0)  # do not predict anything outside
-        dx_inside = tf.where(mask, y_pred[3], 0)  # do not predict anything outside
-        if spatial_gradients:
-            dy_dy, dx_dy = tf.image.image_gradients(y[2])
-            dy_dx, dx_dx = tf.image.image_gradients(y[3])
-            dy_dy_pred, dx_dy_pred = tf.image.image_gradients(y[2])
-            dy_dy_pred, dx_dy_pred = tf.where(mask, dy_dy_pred, 0), tf.where(mask, dx_dy_pred, 0)
-            dy_dx_pred, dx_dx_pred = tf.image.image_gradients(y[3])
-            dy_dx_pred, dx_dx_pred = tf.where(mask, dy_dx_pred, 0), tf.where(mask, dx_dx_pred, 0)
-            return 1./3 * (self.displacement_loss(y[2], dy_inside) + self.displacement_loss(dy_dy, dy_dy_pred) + self.displacement_loss(dx_dy, dx_dy_pred)), 1./3 * (self.displacement_loss(y[3], dx_inside) + self.displacement_loss(dy_dx, dy_dx_pred) + self.displacement_loss(dx_dx, dx_dx_pred))
-        return self.displacement_loss(y[2], dy_inside), self.displacement_loss(y[3], dx_inside)
+        return mask
 
     def _compute_category_loss(self, y, y_pred, n_frame_pairs, n_fp_mul):
         cat_loss = 0.
         for i in range(n_frame_pairs * n_fp_mul):
             inside_mask = tf.math.greater(y[4][..., i:i + 1], 0)
             cat_pred_inside = tf.where(inside_mask, y_pred[4][..., 3 * i:3 * i + 3], 1)
             cat_loss = cat_loss + self.category_loss(y[4][..., i:i + 1], cat_pred_inside)
@@ -209,22 +222,23 @@
             self.compile()
         super().save(*args, **kwargs)
         if inference:
             self.set_inference(False)
             self.trainable=True
             self.compile()
 
+
 def get_distnet_2d(input_shape,
             frame_window:int,
             next:bool,
             config,
             name: str="DiSTNet2D",
             **kwargs):
 
-    return get_distnet_2d_model(input_shape, upsampling_mode = config.upsampling_mode, downsampling_mode=config.downsampling_mode, skip_stop_gradient=False, skip_connections=config.skip_connections, encoder_settings=config.encoder_settings, feature_settings=config.feature_settings, feature_blending_settings=config.feature_blending_settings, decoder_settings=config.decoder_settings, feature_decoder_settings=config.feature_decoder_settings, attention=config.attention, attention_dropout=config.dropout, self_attention=config.self_attention, combine_kernel_size=config.combine_kernel_size, pair_combine_kernel_size=config.pair_combine_kernel_size, blending_filter_factor=config.blending_filter_factor, frame_window=frame_window, next=next, name=name, **kwargs)
+    return get_distnet_2d_model(input_shape, upsampling_mode=config.upsampling_mode, downsampling_mode=config.downsampling_mode, skip_stop_gradient=False, skip_connections=config.skip_connections, encoder_settings=config.encoder_settings, feature_settings=config.feature_settings, feature_blending_settings=config.feature_blending_settings, decoder_settings=config.decoder_settings, feature_decoder_settings=config.feature_decoder_settings, attention=config.attention, attention_dropout=config.dropout, self_attention=config.self_attention, combine_kernel_size=config.combine_kernel_size, pair_combine_kernel_size=config.pair_combine_kernel_size, blending_filter_factor=config.blending_filter_factor, frame_window=frame_window, next=next, name=name, **kwargs)
 
 def get_distnet_2d_model(input_shape,  # Y, X
                          encoder_settings:list,
                          feature_settings: list,
                          feature_blending_settings: list,
                          feature_decoder_settings:list,
                          decoder_settings: list,
@@ -239,15 +253,16 @@
                          attention : int = 0,
                          attention_dropout:float = 0.1,
                          self_attention: int = 0,
                          frame_window:int = 1,
                          next:bool=True,
                          long_term:bool = True,
                          predict_next_displacement:bool = True,
-                         gcdm_gradients:bool=False,
+                         predict_edm_derivatives:bool = False,
+                         predict_gcdm_derivatives:bool = False,
                          l2_reg:float = 0,
                          name: str="DiSTNet2D",
                          **kwargs,
                          ):
         total_contraction = np.prod([np.prod([params.get("downscale", 1) for params in param_list]) for param_list in encoder_settings])
         assert len(encoder_settings)==len(decoder_settings), "decoder should have same length as encoder"
         if attention>0 or self_attention>0:
@@ -298,39 +313,47 @@
             feature_pair_skip_op = Combine(filters=feature_filters, l2_reg=l2_reg, name="FeaturePairSkip")
 
         # define decoder operations
         decoder_layers={"Seg":[], "Center":[], "Track":[], "Cat":[]}
         get_seq_and_filters = lambda l : [l[i] for i in [0, 3]]
         decoder_feature_op={n: get_seq_and_filters(parse_param_list(feature_decoder_settings, f"Features{n}", l2_reg=l2_reg, last_input_filters=feature_filters)) for n in decoder_layers.keys()}
         decoder_out={"Seg":{}, "Center":{}, "Track":{}, "Cat":{}}
-        output_per_decoder = {"Seg": ["EDM"], "Center": ["Center"], "Track": ["dY", "dX"] if not predict_next_displacement else ["dY", "dX", "dYNext", "dXNext"], "Cat": ["Cat"] if not predict_next_displacement else ["Cat", "CatNext"]}
+        output_per_decoder = {"Seg": ["EDM"], "Center": ["GCDM"], "Track": ["dY", "dX"] if not predict_next_displacement else ["dY", "dX", "dYNext", "dXNext"], "Cat": ["Cat"] if not predict_next_displacement else ["Cat", "CatNext"]}
+        if predict_edm_derivatives:
+            output_per_decoder["Seg"].append("EDMdY")
+            output_per_decoder["Seg"].append("EDMdX")
+        if predict_gcdm_derivatives:
+            output_per_decoder["Center"].append("GCDMdY")
+            output_per_decoder["Center"].append("GCDMdX")
         n_frame_pairs = n_chan -1
         if long_term:
             n_frame_pairs = n_frame_pairs + (frame_window-1) * (2 if next else 1)
         decoder_is_segmentation = {"Seg": True, "Center": True, "Track": False, "Cat": False}
         skip_per_decoder = {"Seg": skip_connections, "Center": [], "Track": [], "Cat": []}
 
 
         for l_idx, param_list in enumerate(decoder_settings):
             if l_idx==0:
-                decoder_out["Seg"]["EDM"] = decoder_op(**param_list, size_factor=contraction_per_layer[l_idx], mode=upsampling_mode, skip_combine_mode=skip_combine_mode, combine_kernel_size=combine_kernel_size, activation_out="linear", filters_out=1, l2_reg=l2_reg, layer_idx=l_idx, name=f"DecoderSegEDM")
-                decoder_out["Center"]["Center"] = decoder_op(**param_list, size_factor=contraction_per_layer[l_idx], mode=upsampling_mode, skip_combine_mode=skip_combine_mode, combine_kernel_size=combine_kernel_size, activation_out="linear", filters_out=1, l2_reg=l2_reg, layer_idx=l_idx, name=f"DecoderCenter")
+                for dSegName in output_per_decoder["Seg"]:
+                    decoder_out["Seg"][dSegName] = decoder_op(**param_list, size_factor=contraction_per_layer[l_idx], mode=upsampling_mode, skip_combine_mode=skip_combine_mode, combine_kernel_size=combine_kernel_size, activation_out="linear", filters_out=1, l2_reg=l2_reg, layer_idx=l_idx, name=f"DecoderSeg{dSegName}")
+                for dCenterName in output_per_decoder["Center"]:
+                    decoder_out["Center"][dCenterName] = decoder_op(**param_list, size_factor=contraction_per_layer[l_idx], mode=upsampling_mode, skip_combine_mode=skip_combine_mode, combine_kernel_size=combine_kernel_size, activation_out="linear", filters_out=1, l2_reg=l2_reg, layer_idx=l_idx, name=f"DecoderCenter{dCenterName}")
                 for dTrackName in output_per_decoder["Track"]:
                     decoder_out["Track"][dTrackName] = decoder_op(**param_list, size_factor=contraction_per_layer[l_idx], mode=upsampling_mode, skip_combine_mode=skip_combine_mode, combine_kernel_size=combine_kernel_size, activation_out="linear", filters_out=1, l2_reg=l2_reg, layer_idx=l_idx, name=f"DecoderTrack{dTrackName}")
                 for dCatName in output_per_decoder["Cat"]:
                     decoder_out["Cat"][dCatName] = decoder_op(**param_list, size_factor=contraction_per_layer[l_idx], mode=upsampling_mode, skip_combine_mode=skip_combine_mode, combine_kernel_size=combine_kernel_size, activation_out="softmax", filters_out=3, l2_reg=l2_reg, layer_idx=l_idx, name=f"Decoder{dCatName}")
             else:
                 for decoder_name, d_layers in decoder_layers.items():
                     d_layers.append( decoder_op(**param_list, size_factor=contraction_per_layer[l_idx], mode=upsampling_mode, skip_combine_mode=skip_combine_mode, combine_kernel_size=combine_kernel_size, activation="relu", l2_reg=l2_reg, layer_idx=l_idx, name=f"Decoder{decoder_name}") )
         decoder_output_names = dict()
         oi = 0
         for n, o_ns in output_per_decoder.items():
             decoder_output_names[n] = dict()
             for o_n in o_ns:
-                decoder_output_names[n][o_n] = f"Output{oi}_{o_n}"
+                decoder_output_names[n][o_n] = f"Output{oi:02}_{o_n}"
                 oi += 1
         # Create GRAPH
         input = tf.keras.layers.Input(shape=spatial_dims+[n_chan], name="Input")
         print(f"input dims: {input.shape}")
         input_merged = ChannelToBatch(compensate_gradient = False, name = "MergeInputs")(input)
         downsampled = [input_merged]
         residuals = []
@@ -397,26 +420,33 @@
                 for i, (l, res) in enumerate(zip(d_layers[::-1], residuals[:-1])):
                     up = l([up, res if len(d_layers)-1-i in skip else None])
                 output_per_dec = dict()
                 for output_name in output_per_decoder[decoder_name]:
                     if output_name in decoder_out[decoder_name]:
                         d_out = decoder_out[decoder_name][output_name]
                         layer_output_name = decoder_output_names[decoder_name][output_name]
-                        if not is_segmentation and predict_next_displacement:
+                        if not is_segmentation and predict_next_displacement or decoder_name=="Seg" and predict_edm_derivatives or decoder_name== "Center" and predict_gcdm_derivatives:
                             layer_output_name += "_" # will be concatenated -> output name is used @ concat
                         up_out = d_out([up, residuals[-1] if 0 in skip else None]) # (N_OUT x B, Y, X, F)
                         up_out = BatchToChannel(n_splits = n_chan if is_segmentation else n_frame_pairs, compensate_gradient = False, name = layer_output_name)(up_out)
                         output_per_dec[output_name] = up_out
                 if predict_next_displacement: # merge outputs ending by Next
                     for k in list(output_per_dec.keys()):
                         if k.endswith("Next"):
                             output_name = k.replace("Next", "")
                             output_per_dec[output_name] = tf.keras.layers.Concatenate(axis = -1, name = decoder_output_names[decoder_name][output_name])([output_per_dec[output_name], output_per_dec.pop(k)])
+                if decoder_name=="Seg" and predict_edm_derivatives:
+                    output_name = "EDM"
+                    output_per_dec[output_name] = tf.keras.layers.Concatenate(axis=-1,  name=decoder_output_names[decoder_name][output_name])([output_per_dec[output_name], output_per_dec.pop("EDMdY"), output_per_dec.pop("EDMdX")])
+                if decoder_name=="Center" and predict_gcdm_derivatives:
+                    output_name = "GCDM"
+                    output_per_dec[output_name] = tf.keras.layers.Concatenate(axis=-1,  name=decoder_output_names[decoder_name][output_name])([output_per_dec[output_name], output_per_dec.pop("GCDMdY"), output_per_dec.pop("GCDMdX")])
                 outputs.extend(output_per_dec.values())
-        return DiSTNetModel([input], outputs, name=name, frame_window=frame_window, next = next, spatial_dims=spatial_dims if attention > 0 or self_attention > 0 else None, long_term=long_term, predict_next_displacement=predict_next_displacement, gcdm_gradients=gcdm_gradients, **kwargs)
+        return DiSTNetModel([input], outputs, name=name, frame_window=frame_window, next=next, spatial_dims=spatial_dims if attention > 0 or self_attention > 0 else None, long_term=long_term, predict_next_displacement=predict_next_displacement, predict_gcdm_derivatives=predict_gcdm_derivatives, predict_edm_derivatives=predict_edm_derivatives, **kwargs)
+
 
 def encoder_op(param_list, downsampling_mode, skip_stop_gradient:bool = False, l2_reg:float=0, last_input_filters:int=0, name: str="EncoderLayer", layer_idx:int=1):
     name=f"{name}{layer_idx}"
     maxpool = downsampling_mode=="maxpool"
     maxpool_and_stride = downsampling_mode == "maxpool_and_stride"
     sequence, down_sequence, total_contraction, residual_filters, out_filters = parse_param_list(param_list, name, ignore_stride=maxpool, l2_reg=l2_reg, last_input_filters = last_input_filters if maxpool_and_stride else 0)
     assert total_contraction>1, "invalid parameters: no contraction specified"
```

### Comparing `distnet2d-0.1.7/distnet_2d/model/distnet_2d_seg.py` & `distnet2d-0.1.8/distnet_2d/model/distnet_2d_seg.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/model/gradient_accumulator.py` & `distnet2d-0.1.8/distnet_2d/model/gradient_accumulator.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/model/layers.py` & `distnet2d-0.1.8/distnet_2d/model/layers.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/model/spatial_attention.py` & `distnet2d-0.1.8/distnet_2d/model/spatial_attention.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/utils/agc.py` & `distnet2d-0.1.8/distnet_2d/utils/agc.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/utils/helpers.py` & `distnet2d-0.1.8/distnet_2d/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/utils/lovasz_loss.py` & `distnet2d-0.1.8/distnet_2d/utils/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/utils/metrics_tf.py` & `distnet2d-0.1.8/distnet_2d/utils/metrics_tf.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/distnet_2d/utils/objectwise_computation_tf.py` & `distnet2d-0.1.8/distnet_2d/utils/objectwise_computation_tf.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.7/setup.py` & `distnet2d-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DiSTNet2D",
-    version="0.1.7",
+    version="0.1.8",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="tensorflow/keras implementation of DiSTNet 2D",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/distnet2d",
-    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.7/distnet2d-0.1.7.tar.gz',
+    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.8/distnet2d-0.1.8.tar.gz',
     packages=setuptools.find_packages(),
     keywords=['Segmentation', 'Tracking', 'Cell', 'Tensorflow', 'Keras'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

