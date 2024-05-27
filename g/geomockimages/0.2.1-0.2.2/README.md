# Comparing `tmp/geomockimages-0.2.1.tar.gz` & `tmp/geomockimages-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomockimages-0.2.1.tar", max compression
+gzip compressed data, was "geomockimages-0.2.2.tar", max compression
```

## Comparing `geomockimages-0.2.1.tar` & `geomockimages-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-04-19 06:06:31.014821 geomockimages-0.2.1/LICENSE
--rw-r--r--   0        0        0     1893 2024-05-24 04:21:06.692977 geomockimages-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 07:17:28.778191 geomockimages-0.2.1/geomockimages/__init__.py
--rw-r--r--   0        0        0    14041 2024-05-22 10:13:58.233715 geomockimages-0.2.1/geomockimages/imagecreator.py
--rw-r--r--   0        0        0      923 2024-04-19 07:17:28.779244 geomockimages-0.2.1/geomockimages/logging.py
--rw-r--r--   0        0        0     1511 2024-05-20 08:53:13.724556 geomockimages-0.2.1/geomockimages/raster.py
--rw-r--r--   0        0        0        0 2024-04-19 07:17:28.779518 geomockimages-0.2.1/geomockimages/test/__init__.py
--rw-r--r--   0        0        0     5462 2024-05-22 10:13:58.234271 geomockimages-0.2.1/geomockimages/test/test_geomockimages.py
--rw-r--r--   0        0        0      689 2024-05-24 04:23:16.899744 geomockimages-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 geomockimages-0.2.1/setup.py
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 geomockimages-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-19 06:06:31.014821 geomockimages-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1893 2024-05-27 04:15:14.100791 geomockimages-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 07:17:28.778191 geomockimages-0.2.2/geomockimages/__init__.py
+-rw-r--r--   0        0        0    14049 2024-05-27 07:19:14.666358 geomockimages-0.2.2/geomockimages/imagecreator.py
+-rw-r--r--   0        0        0      923 2024-04-19 07:17:28.779244 geomockimages-0.2.2/geomockimages/logging.py
+-rw-r--r--   0        0        0     1511 2024-05-20 08:53:13.724556 geomockimages-0.2.2/geomockimages/raster.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:17:28.779518 geomockimages-0.2.2/geomockimages/test/__init__.py
+-rw-r--r--   0        0        0     5462 2024-05-27 07:19:14.668804 geomockimages-0.2.2/geomockimages/test/test_geomockimages.py
+-rw-r--r--   0        0        0      819 2024-05-27 10:41:50.884573 geomockimages-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 geomockimages-0.2.2/setup.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 geomockimages-0.2.2/PKG-INFO
```

### Comparing `geomockimages-0.2.1/LICENSE` & `geomockimages-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.1/README.md` & `geomockimages-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.1/geomockimages/imagecreator.py` & `geomockimages-0.2.2/geomockimages/imagecreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             ```
         """
 
         self.xsize = xsize
         self.ysize = ysize
         self.num_bands = num_bands
         self.data_type = data_type
-        self.image_type = image_type
+        self.image_type = image_type.lower()
         self.out_dir = out_dir
         self.crs = crs
         self.nodata_fill = nodata_fill
         if nodata == -1:
             self.nodata = None
         else:
             self.nodata = nodata
@@ -209,15 +209,15 @@
         bands = []
         band_idx = 0
         while band_idx < self.num_bands:
             data_ar = np.zeros_like(image, dtype=self.data_type)
 
             if self.image_type == "optical":
                 lc_values = enumerate(LC_CLASSES_OPTICAL.values(), 1)
-            elif self.image_type == "SAR":
+            elif self.image_type == "sar":
                 lc_values = enumerate(LC_CLASSES_SAR.values(), 1)
             else:
                 raise Exception("Only optical and SAR images are supported")
 
             for class_idx, lc_class in lc_values:
                 # Add Gaussian noise
                 try:
```

### Comparing `geomockimages-0.2.1/geomockimages/logging.py` & `geomockimages-0.2.2/geomockimages/logging.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.1/geomockimages/raster.py` & `geomockimages-0.2.2/geomockimages/raster.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.1/geomockimages/test/test_geomockimages.py` & `geomockimages-0.2.2/geomockimages/test/test_geomockimages.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     with tempfile.TemporaryDirectory() as td:
         test_img1, data1 = GeoMockImage(
             10, 5, 1, "uint16", "SAR", out_dir=Path(td)
         ).create(seed=4, noise_seed=5, noise_intensity=2.0)
 
     with tempfile.TemporaryDirectory() as td:
         test_img2, data2 = GeoMockImage(
-            10, 5, 1, "uint16", "SAR", out_dir=Path(td)
+            10, 5, 1, "uint16", "sar", out_dir=Path(td)
         ).create(seed=4, noise_seed=3, noise_intensity=2.0)
 
     # The two images should appear like they were taken at different dates from the same area
     diff = data1.astype(int) - data2.astype(int)
     assert (np.abs(diff)).max() < 150
     assert np.abs(np.sum(diff)) < 1000
```

### Comparing `geomockimages-0.2.1/pyproject.toml` & `geomockimages-0.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geomockimages"
-version = "0.2.1"
+version = "0.2.2"
 description = "A module to programmatically create geotiff images which can be used for unit tests."
 authors = ["Markus Müller <markus.u.mueller@zoho.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -23,7 +23,11 @@
 pytest-ruff = "^0.3.2"
 pre-commit = "^3.7.1"
 ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[project.urls]
+"Homepage" = "https://github.com/markusuwe/geomockimages"
+"Source" = "https://github.com/markusuwe/geomockimages"
```

### Comparing `geomockimages-0.2.1/setup.py` & `geomockimages-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'rasterio>=1.3.10,<2.0.0',
  'rio-cogeo>=5.3.0,<6.0.0',
  'scikit-image>=0.23.2,<0.24.0',
  'scipy>=1.13.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'geomockimages',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'A module to programmatically create geotiff images which can be used for unit tests.',
     'long_description': '# geomockimages\n\nA module to programmatically create geotiff images which can be used for unit tests.\n\nThe underlying idea is that in order to write unit tests for geospatial image processsing algorithms,\nit is necessary to have an actual input image file or array. Organising these test images becomes a chore over time,\nthey should not be stored in git as they are large binary data and when stored outside, there always\nis the danger that they are not updated according to changes in the code repo.\n\n**geomockimages** provides a solution to the problem by providing simple code that allows to create\ngeospatial images (so far geotiffs) in a parameterised way.\n\n## Install package\n```bash\npip install geomockimages\n```\n\n## Run tests\n```bash\npytest\n```\n\n## Usage\n\nIn the following an example unit test for a hypothetical NDVI function.\n\n```python\nimport numpy as np\nimport rasterio as rio\nfrom pathlib import Path\n\nfrom rasterio.transform import from_origin\nfrom my_image_processing import ndvi\nfrom geomockimages.imagecreator import GeoMockImage\n\ndef test_ndvi():\n    """\n    A unit test if an NDVI method works in general\n    """\n    # Create 4-band image simulating RGBN as needed for NDVI\n    test_image, _ = GeoMockImage(\n        300,\n        150,\n        4,\n        "uint16",\n        out_dir=Path("/tmp"),\n        crs=4326,\n        nodata=0,\n        nodata_fill=3,\n        cog=False,\n    ).create(seed=42, transform=from_origin(13.428596, 52.494384, 0.000006, 0.000006))\n\n    ndvi_image = ndvi(test_image)\n\n    with rio.open(str(ndvi_image)) as src:\n        ndvi_array = src.read()\n        # NDVI only has one band of same size as input bands\n        assert ndvi_array.shape == (1, 150, 300)\n        # NDVI has float values between -1 and 1\n        assert ndvi_array.dtype == np.dtype(\'float32\')\n        assert np.nanmin(ndvi_array) >= -1\n        assert np.nanmax(ndvi_array) <= 1\n\n```\n',
     'author': 'Markus Müller',
     'author_email': 'markus.u.mueller@zoho.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `geomockimages-0.2.1/PKG-INFO` & `geomockimages-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomockimages
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module to programmatically create geotiff images which can be used for unit tests.
 License: MIT
 Author: Markus Müller
 Author-email: markus.u.mueller@zoho.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

