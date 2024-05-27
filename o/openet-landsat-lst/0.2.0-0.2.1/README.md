# Comparing `tmp/openet-landsat-lst-0.2.0.tar.gz` & `tmp/openet_landsat_lst-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openet-landsat-lst-0.2.0.tar", last modified: Thu Mar  7 00:34:33 2024, max compression
+gzip compressed data, was "openet_landsat_lst-0.2.1.tar", last modified: Mon May 27 16:24:24 2024, max compression
```

## Comparing `openet-landsat-lst-0.2.0.tar` & `openet_landsat_lst-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-07 00:34:33.019356 openet-landsat-lst-0.2.0/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2248 2024-03-07 00:34:33.019035 openet-landsat-lst-0.2.0/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1482 2024-03-06 14:03:50.000000 openet-landsat-lst-0.2.0/README.md
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-07 00:34:33.012554 openet-landsat-lst-0.2.0/openet/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2024-03-06 13:57:40.000000 openet-landsat-lst-0.2.0/openet/__init__.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-07 00:34:33.014588 openet-landsat-lst-0.2.0/openet/lst/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       90 2024-03-06 13:57:40.000000 openet-landsat-lst-0.2.0/openet/lst/__init__.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3666 2024-03-06 14:03:22.000000 openet-landsat-lst-0.2.0/openet/lst/landsat.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9846 2024-03-06 14:03:06.000000 openet-landsat-lst-0.2.0/openet/lst/model.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-07 00:34:33.016561 openet-landsat-lst-0.2.0/openet/lst/tests/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-06 14:38:49.000000 openet-landsat-lst-0.2.0/openet/lst/tests/conftest.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2804 2024-03-06 14:01:17.000000 openet-landsat-lst-0.2.0/openet/lst/tests/test_landsat.py
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2019 2024-03-06 14:04:33.000000 openet-landsat-lst-0.2.0/openet/lst/tests/test_model.py
-drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-03-07 00:34:33.018605 openet-landsat-lst-0.2.0/openet_landsat_lst.egg-info/
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2248 2024-03-07 00:34:33.000000 openet-landsat-lst-0.2.0/openet_landsat_lst.egg-info/PKG-INFO
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      410 2024-03-07 00:34:33.000000 openet-landsat-lst-0.2.0/openet_landsat_lst.egg-info/SOURCES.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-03-07 00:34:33.000000 openet-landsat-lst-0.2.0/openet_landsat_lst.egg-info/dependency_links.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       59 2024-03-07 00:34:33.000000 openet-landsat-lst-0.2.0/openet_landsat_lst.egg-info/requires.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2024-03-07 00:34:33.000000 openet-landsat-lst-0.2.0/openet_landsat_lst.egg-info/top_level.txt
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1314 2024-03-06 21:44:08.000000 openet-landsat-lst-0.2.0/pyproject.toml
--rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-03-07 00:34:33.019397 openet-landsat-lst-0.2.0/setup.cfg
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-27 16:24:24.387302 openet_landsat_lst-0.2.1/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2248 2024-05-27 16:24:24.387000 openet_landsat_lst-0.2.1/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1482 2024-03-06 14:03:50.000000 openet_landsat_lst-0.2.1/README.md
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-27 16:24:24.380585 openet_landsat_lst-0.2.1/openet/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       65 2024-03-06 13:57:40.000000 openet_landsat_lst-0.2.1/openet/__init__.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-27 16:24:24.382737 openet_landsat_lst-0.2.1/openet/lst/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       90 2024-03-06 13:57:40.000000 openet_landsat_lst-0.2.1/openet/lst/__init__.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3832 2024-03-09 21:56:11.000000 openet_landsat_lst-0.2.1/openet/lst/landsat.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     9834 2024-03-08 21:48:31.000000 openet_landsat_lst-0.2.1/openet/lst/model.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-27 16:24:24.384710 openet_landsat_lst-0.2.1/openet/lst/tests/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      796 2024-03-06 14:38:49.000000 openet_landsat_lst-0.2.1/openet/lst/tests/conftest.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     3538 2024-03-09 22:57:33.000000 openet_landsat_lst-0.2.1/openet/lst/tests/test_landsat.py
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2049 2024-03-09 22:57:20.000000 openet_landsat_lst-0.2.1/openet/lst/tests/test_model.py
+drwxr-xr-x   0 Charles.Morton@dri.edu   (502) staff       (20)        0 2024-05-27 16:24:24.386615 openet_landsat_lst-0.2.1/openet_landsat_lst.egg-info/
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     2248 2024-05-27 16:24:24.000000 openet_landsat_lst-0.2.1/openet_landsat_lst.egg-info/PKG-INFO
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)      410 2024-05-27 16:24:24.000000 openet_landsat_lst-0.2.1/openet_landsat_lst.egg-info/SOURCES.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        1 2024-05-27 16:24:24.000000 openet_landsat_lst-0.2.1/openet_landsat_lst.egg-info/dependency_links.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       59 2024-05-27 16:24:24.000000 openet_landsat_lst-0.2.1/openet_landsat_lst.egg-info/requires.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)        7 2024-05-27 16:24:24.000000 openet_landsat_lst-0.2.1/openet_landsat_lst.egg-info/top_level.txt
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)     1314 2024-05-27 16:23:55.000000 openet_landsat_lst-0.2.1/pyproject.toml
+-rw-r--r--   0 Charles.Morton@dri.edu   (502) staff       (20)       38 2024-05-27 16:24:24.387353 openet_landsat_lst-0.2.1/setup.cfg
```

### Comparing `openet-landsat-lst-0.2.0/PKG-INFO` & `openet_landsat_lst-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openet-landsat-lst
-Version: 0.2.0
+Version: 0.2.1
 Summary: Earth Engine based Landsat LST sharpening functions
 Author-email: Yanghui Kang <ykang38@wisc.edu>, Yun Yang <yun.yang@msstate.edu>
 Maintainer-email: Charles Morton <charles.morton@dri.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Open-ET/openet-landsat-lst
 Keywords: LST,OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: earthengine-api>=0.1.367
-Requires-Dist: openet-core>=0.2.0
+Requires-Dist: openet-core>=0.4.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # Landsat LST Sharpening Algorithms
 
 The thermal sharpening algorithm is developed for Landsat 5, 7, 8, or 9. The algorithm has three components.
```

### Comparing `openet-landsat-lst-0.2.0/README.md` & `openet_landsat_lst-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openet-landsat-lst-0.2.0/openet/lst/landsat.py` & `openet_landsat_lst-0.2.1/openet/lst/landsat.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,25 +10,25 @@
     # CGM - Using the __new__ to return is discouraged and is probably not
     #   great Python but it was the only way I could find to make the general
     #   Landsat class directly callable like the collection specific ones
     # def __init__(self):
     #     """"""
     #     pass
 
-    def __new__(cls, image_id, c2_lst_correct=False):
+    def __new__(cls, image_id, c2_lst_correct=True):
         if type(image_id) is not str:
             raise ValueError('unsupported input type')
         elif re.match('LANDSAT/L[TEC]0[45789]/C02/T1_L2', image_id):
             return Landsat_C02_L2(image_id, c2_lst_correct=c2_lst_correct)
         else:
             raise ValueError('unsupported image_id')
 
 
 class Landsat_C02_L2(Model):
-    def __init__(self, image_id, c2_lst_correct=False):
+    def __init__(self, image_id, c2_lst_correct=True):
         """"""
         # TODO: Support input being an ee.Image
         # For now assume input is always an image ID
         if type(image_id) is not str:
             raise ValueError('unsupported input type')
         elif (image_id.startswith('LANDSAT/') and
                 not re.match('LANDSAT/L[TEC]0[45789]/C02/T1_L2', image_id)):
@@ -37,52 +37,59 @@
         raw_image = ee.Image(image_id)
 
         # CGM - Testing out not setting any self. parameters and passing inputs
         #   to the super().__init__() call instead
 
         spacecraft_id = ee.String(raw_image.get('SPACECRAFT_ID'))
 
-        # CGM - The QA_PIXEL band could probably be dropped
+        # Select the ST/LST band separately from the SR bands
+        # Not passing the QA band through since it is not used in the model
         input_bands = ee.Dictionary({
-            'LANDSAT_4': ['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7',
-                          'ST_B6', 'QA_PIXEL'],
-            'LANDSAT_5': ['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7',
-                          'ST_B6', 'QA_PIXEL'],
-            'LANDSAT_7': ['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7',
-                          'ST_B6', 'QA_PIXEL'],
-            'LANDSAT_8': ['SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7',
-                          'ST_B10', 'QA_PIXEL'],
-            'LANDSAT_9': ['SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7',
-                          'ST_B10', 'QA_PIXEL'],
+            'LANDSAT_4': ['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7'],
+            'LANDSAT_5': ['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7'],
+            'LANDSAT_7': ['SR_B1', 'SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B7'],
+            'LANDSAT_8': ['SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7'],
+            'LANDSAT_9': ['SR_B2', 'SR_B3', 'SR_B4', 'SR_B5', 'SR_B6', 'SR_B7'],
+        })
+        output_bands = ['blue', 'green', 'red', 'nir', 'swir1', 'swir2']
+
+        lst_band = ee.Dictionary({
+            'LANDSAT_4': 'ST_B6', 'LANDSAT_5': 'ST_B6', 'LANDSAT_7': 'ST_B6',
+            'LANDSAT_8': 'ST_B10', 'LANDSAT_9': 'ST_B10',
         })
-        output_bands = ['blue', 'green', 'red', 'nir', 'swir1', 'swir2', 'lst', 'qa']
 
         # # CGM - We are intentionally not masking for clouds in the LST
         # # Cloud mask function must be passed with raw/unnamed image
         # cloud_mask = openet.core.common.landsat_c2_sr_cloud_mask(
         #     raw_image, **cloudmask_args
         # )
 
         # Prep image to 0-1 surface reflectance values
-        prep_image = (
+        prep_img = (
             raw_image
             .select(input_bands.get(spacecraft_id), output_bands)
-            .multiply([0.0000275, 0.0000275, 0.0000275, 0.0000275,
-                       0.0000275, 0.0000275, 0.00341802, 1])
-            .add([-0.2, -0.2, -0.2, -0.2, -0.2, -0.2, 149.0, 1])
+            .multiply([0.0000275, 0.0000275, 0.0000275, 0.0000275, 0.0000275, 0.0000275])
+            .add([-0.2, -0.2, -0.2, -0.2, -0.2, -0.2])
             .set({'system:time_start': raw_image.get('system:time_start'),
                   'system:index': raw_image.get('system:index'),
                   'SPACECRAFT_ID': spacecraft_id,
                   })
         )
 
         # Compute the emissivity corrected LST and add to the prepped image
+        #   or add the raw LST to the prepped image
         if c2_lst_correct:
-            lst = openet.core.common.landsat_c2_sr_lst_correct(
-                raw_image, prep_image.normalizedDifference(['nir', 'red'])
+            lst_img = openet.core.common.landsat_c2_sr_lst_correct(
+                raw_image, prep_img.normalizedDifference(['nir', 'red'])
             )
-            prep_image = prep_image.addBands([lst.rename(['lst'])], overwrite=True)
+        else:
+            lst_img = (
+                raw_image.select([ee.String(lst_band.get(spacecraft_id))])
+                .multiply(0.00341802).add(149.0)
+            )
+
+        init_img = prep_img.addBands(lst_img.rename(['lst']))
 
         # CGM - super could be called without the init if we set input_image and
         #   spacecraft_id as properties of self
-        super().__init__(prep_image)
+        super().__init__(init_img)
         # super()
```

### Comparing `openet-landsat-lst-0.2.0/openet/lst/model.py` & `openet_landsat_lst-0.2.1/openet/lst/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     def __init__(self, image):
         """
 
         Parameters
         ----------
         image : ee.Image
             "Prepped" Landsat image with standardized bands names
-                (i.e. blue, green, red, nir, swir1, swir2, tir).
-            Thermal band must be named 'tir' and be in units of Kelvin.
+                (i.e. blue, green, red, nir, swir1, swir2, lst).
+            Thermal band must be named 'lst' and be in units of Kelvin.
             Must have property 'SPACECRAFT_ID' with a value of 'LANDSAT_4',
                 'LANDSAT_5', 'LANDSAT_7', 'LANDSAT_8', or 'LANDSAT_9'.
 
         """
         self.image = image
 
     # TODO: Decide if this should be a lazy property since it doesn't have inputs
@@ -97,19 +97,18 @@
             .reproject(crs=crs, crsTransform=tir_transform)
         )
 
         # Compute the coefficient of variation of sub-pixel reflectance
         other_cv = other_std.divide(other_mean).reduce(ee.Reducer.mean())
 
         # Add a bias band (=1) to the image for linear regression reducer
-        image_agg = (
-            other_mean
-            .addBands(other_mean.select([0]).multiply(0).add(1).rename(['bias']))
-            .addBands(tir)
-        )
+        # Add the LST image back in
+        image_agg = other_mean.addBands([
+            other_mean.select([0]).multiply(0).add(1).rename(['bias']), tir
+        ])
 
         # Fit moving-window linear regressions at coarse resolution
         # Y: tir (power 4)
         # X: SR Bands
         kernel = ee.Kernel.square(kernel_size)
         local_fit = image_agg.reduceNeighborhood(
             ee.Reducer.linearRegression(len(bands) + 1, 1), kernel, None, False
@@ -126,18 +125,17 @@
             .reproject(crs, transform)
         )
 
         # CGM - Not used below, commenting out
         # rmse = local_fit.select('residuals').arrayFlatten([['residuals']]).pow(0.25)
 
         # Apply linear fit at high resolution for sharpened TIR
-        inputs = (
-            self.image.select(bands)
-            .addBands(self.image.select([0]).multiply(0).add(1).rename(['bias']))
-        )
+        inputs = self.image.select(bands).addBands([
+            self.image.select([0]).multiply(0).add(1).rename(['bias'])
+        ])
         tir_sp_local = inputs.multiply(coefficients).reduce(ee.Reducer.sum()).pow(0.25)
 
         # Fit a scene-wise random forest model
         # Select homogeneous samples defined by a threshold in c.v.
         samples = (
             image_agg.updateMask(other_cv.lt(cv_threshold))
             .sample(region=bound, scale=tir_res, factor=5e-3)
```

### Comparing `openet-landsat-lst-0.2.0/openet/lst/tests/conftest.py` & `openet_landsat_lst-0.2.1/openet/lst/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openet-landsat-lst-0.2.0/openet/lst/tests/test_landsat.py` & `openet_landsat_lst-0.2.1/openet/lst/tests/test_landsat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
-import pprint
 
 import ee
 import pytest
 
 import openet.lst
 import openet.core.utils as utils
 
 logging.basicConfig(level=logging.DEBUG, format='%(message)s')
 
-DEFAULT_BANDS = ['blue', 'green', 'red', 'nir', 'swir1', 'swir2', 'lst', 'qa']
-
+DEFAULT_BANDS = ['blue', 'green', 'red', 'nir', 'swir1', 'swir2', 'lst']
 
 
 def test_ee_init():
     assert ee.Number(1).getInfo() == 1
 
 
 @pytest.mark.parametrize(
@@ -37,15 +35,16 @@
     output = openet.lst.Landsat_C02_L2(image_id=image_id).image.getInfo()
     assert output['properties']['SPACECRAFT_ID'] == 'LANDSAT_8'
 
 
 def test_Landsat_C02_L2_scaling():
     image_id = 'LANDSAT/LC08/C02/T1_L2/LC08_044033_20170716'
     output = utils.point_image_value(
-        openet.lst.Landsat_C02_L2(image_id).image, xy=(-121.5265, 38.7399))
+        openet.lst.Landsat_C02_L2(image_id, c2_lst_correct=False).image,
+        xy=(-121.5265, 38.7399))
     assert abs(output['nir'] - 0.26) <= 0.01
     assert abs(output['lst'] - 306) <= 1
 
 
 @pytest.mark.parametrize(
     'image_id',
     [
@@ -55,25 +54,35 @@
 )
 def test_Landsat_band_names(image_id):
     output = openet.lst.Landsat(image_id).image.bandNames().getInfo()
     assert set(output) == set(DEFAULT_BANDS)
 
 
 @pytest.mark.parametrize(
-    "image_id, xy, expected",
+    "image_id, xy, flag, expected",
     [
         # First two points are in the same field but the second one is in an
         # area of bad emissivity data and needs correction
-        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.266679, 34.368470], 310],
-        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.266754, 34.367682], 310],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.266679, 34.368470], False, 310],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.266679, 34.368470], True, 310],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.266754, 34.367682], False, 312],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.266754, 34.367682], True, 310],
         # This point is just outside the field and should stay the same
-        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.269769, 34.366115], 318],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.269769, 34.366115], False, 318],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_030036_20210725', [-102.269769, 34.366115], True, 318],
         # These two points are in the ASTER GED hole and have no L2 temperature
         # The first is a high NDVI field, the second is a low NDVI field
-        ['LANDSAT/LC08/C02/T1_L2/LC08_031034_20160702', [-102.08284, 37.81728], 307],
-        ['LANDSAT/LC08/C02/T1_L2/LC08_031034_20160702', [-102.04696, 37.81796], 298],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_031034_20160702', [-102.08284, 37.81728], False, None],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_031034_20160702', [-102.08284, 37.81728], True, 307],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_031034_20160702', [-102.04696, 37.81796], False, None],
+        ['LANDSAT/LC08/C02/T1_L2/LC08_031034_20160702', [-102.04696, 37.81796], True, 298],
     ]
 )
-def test_Landsat_c2_lst_correction_flag(image_id, xy, expected, tol=1):
-    output_img = openet.lst.Landsat(image_id, c2_lst_correct=True).image
+def test_Landsat_c2_lst_correction_flag(image_id, xy, flag, expected, tol=1):
+    # Check if the LST correction is being applied and working
+    # These are the same test scenes/points that are in openet-core
+    output_img = openet.lst.Landsat(image_id, c2_lst_correct=flag).image
     corrected = utils.point_image_value(output_img, xy, scale=30)
-    assert abs(corrected['lst'] - expected) <= tol
+    if expected is None:
+        assert corrected['lst'] is None
+    else:
+        assert abs(corrected['lst'] - expected) <= tol
```

### Comparing `openet-landsat-lst-0.2.0/openet/lst/tests/test_model.py` & `openet_landsat_lst-0.2.1/openet/lst/tests/test_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import pprint
 
 import ee
 import pytest
 
 import openet.lst
 import openet.core.utils as utils
 
@@ -21,15 +20,15 @@
 def test_Model_init():
     input_img = ee.Image.constant(DEFAULT_VALUES).rename(DEFAULT_BANDS)
     image_obj = openet.lst.Model(image=input_img)
     assert set(image_obj.image.bandNames().getInfo()) == set(DEFAULT_BANDS)
 
 
 def test_Model_thermal_band_name():
-    input_img = openet.lst.Landsat(TEST_IMAGE_ID).image
+    input_img = openet.lst.Landsat(TEST_IMAGE_ID, c2_lst_correct=False).image
     output = openet.lst.Model(input_img).sharpen().bandNames().getInfo()
     assert output == ['lst_sharpened']
 
 
 @pytest.mark.parametrize(
     "image_id, xy, expected",
     [
@@ -45,11 +44,11 @@
         # ['LANDSAT/LC08/C01/T1_SR/LC08_042034_20180705',
         #  [-120.10237, 36.946608], 304.13262575660264],
         # ['LANDSAT/LC08/C01/T1_TOA/LC08_042034_20180705',
         #  [-120.10237, 36.946608], 303.75037059315696],
     ]
 )
 def test_Model_thermal_point_values(image_id, xy, expected, tol=0.01):
-    input_img = openet.lst.Landsat(image_id).image
+    input_img = openet.lst.Landsat(image_id, c2_lst_correct=False).image
     output_img = openet.lst.Model(input_img).sharpen()
     output = utils.point_image_value(output_img, xy, scale=30)
     assert abs(output['lst_sharpened'] - expected) < tol
```

### Comparing `openet-landsat-lst-0.2.0/openet_landsat_lst.egg-info/PKG-INFO` & `openet_landsat_lst-0.2.1/openet_landsat_lst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openet-landsat-lst
-Version: 0.2.0
+Version: 0.2.1
 Summary: Earth Engine based Landsat LST sharpening functions
 Author-email: Yanghui Kang <ykang38@wisc.edu>, Yun Yang <yun.yang@msstate.edu>
 Maintainer-email: Charles Morton <charles.morton@dri.edu>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Open-ET/openet-landsat-lst
 Keywords: LST,OpenET,Earth Engine,Evapotranspiration,Landsat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: earthengine-api>=0.1.367
-Requires-Dist: openet-core>=0.2.0
+Requires-Dist: openet-core>=0.4.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # Landsat LST Sharpening Algorithms
 
 The thermal sharpening algorithm is developed for Landsat 5, 7, 8, or 9. The algorithm has three components.
```

### Comparing `openet-landsat-lst-0.2.0/pyproject.toml` & `openet_landsat_lst-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openet-landsat-lst"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Yanghui Kang", email = "ykang38@wisc.edu" },
     { name = "Yun Yang", email = "yun.yang@msstate.edu" },
 ]
 maintainers = [
     { name = "Charles Morton", email = "charles.morton@dri.edu" },
 ]
@@ -16,15 +16,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "earthengine-api >= 0.1.367",
-    "openet-core >= 0.2.0",
+    "openet-core >= 0.4.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Open-ET/openet-landsat-lst"
 # "Repository" = "https://github.com/Open-ET/openet-landsat-lst.git"
 # "Documentation" = "https://github.com/Open-ET/openet-landsat-lst"
 # "Bug Tracker" = "https://github.com/Open-ET/openet-landsat-lst"
```

