# Comparing `tmp/geomockimages-0.2.2.tar.gz` & `tmp/geomockimages-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomockimages-0.2.2.tar", max compression
+gzip compressed data, was "geomockimages-0.2.3.tar", max compression
```

## Comparing `geomockimages-0.2.2.tar` & `geomockimages-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-04-19 06:06:31.014821 geomockimages-0.2.2/LICENSE
--rw-r--r--   0        0        0     1893 2024-05-27 04:15:14.100791 geomockimages-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-04-19 07:17:28.778191 geomockimages-0.2.2/geomockimages/__init__.py
--rw-r--r--   0        0        0    14049 2024-05-27 07:19:14.666358 geomockimages-0.2.2/geomockimages/imagecreator.py
--rw-r--r--   0        0        0      923 2024-04-19 07:17:28.779244 geomockimages-0.2.2/geomockimages/logging.py
--rw-r--r--   0        0        0     1511 2024-05-20 08:53:13.724556 geomockimages-0.2.2/geomockimages/raster.py
--rw-r--r--   0        0        0        0 2024-04-19 07:17:28.779518 geomockimages-0.2.2/geomockimages/test/__init__.py
--rw-r--r--   0        0        0     5462 2024-05-27 07:19:14.668804 geomockimages-0.2.2/geomockimages/test/test_geomockimages.py
--rw-r--r--   0        0        0      819 2024-05-27 10:41:50.884573 geomockimages-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 geomockimages-0.2.2/setup.py
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 geomockimages-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-19 06:06:31.014821 geomockimages-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1893 2024-05-27 04:15:14.100791 geomockimages-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 07:17:28.778191 geomockimages-0.2.3/geomockimages/__init__.py
+-rw-r--r--   0        0        0    14049 2024-05-27 07:19:14.666358 geomockimages-0.2.3/geomockimages/imagecreator.py
+-rw-r--r--   0        0        0      923 2024-04-19 07:17:28.779244 geomockimages-0.2.3/geomockimages/logging.py
+-rw-r--r--   0        0        0     1511 2024-05-20 08:53:13.724556 geomockimages-0.2.3/geomockimages/raster.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:17:28.779518 geomockimages-0.2.3/geomockimages/test/__init__.py
+-rw-r--r--   0        0        0     5462 2024-05-27 07:19:14.668804 geomockimages-0.2.3/geomockimages/test/test_geomockimages.py
+-rw-r--r--   0        0        0      803 2024-05-27 11:03:09.662086 geomockimages-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 geomockimages-0.2.3/setup.py
+-rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 geomockimages-0.2.3/PKG-INFO
```

### Comparing `geomockimages-0.2.2/LICENSE` & `geomockimages-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.2/README.md` & `geomockimages-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.2/geomockimages/imagecreator.py` & `geomockimages-0.2.3/geomockimages/imagecreator.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.2/geomockimages/logging.py` & `geomockimages-0.2.3/geomockimages/logging.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.2/geomockimages/raster.py` & `geomockimages-0.2.3/geomockimages/raster.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.2/geomockimages/test/test_geomockimages.py` & `geomockimages-0.2.3/geomockimages/test/test_geomockimages.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.2/pyproject.toml` & `geomockimages-0.2.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "geomockimages"
-version = "0.2.2"
+version = "0.2.3"
 description = "A module to programmatically create geotiff images which can be used for unit tests."
 authors = ["Markus Müller <markus.u.mueller@zoho.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/markusuwe/geomockimages"
+repository = "https://github.com/markusuwe/geomockimages"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
 rasterio = "^1.3.10"
 rio-cogeo = "^5.3.0"
 scikit-image = "^0.23.2"
@@ -23,11 +25,7 @@
 pytest-ruff = "^0.3.2"
 pre-commit = "^3.7.1"
 ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[project.urls]
-"Homepage" = "https://github.com/markusuwe/geomockimages"
-"Source" = "https://github.com/markusuwe/geomockimages"
```

### Comparing `geomockimages-0.2.2/setup.py` & `geomockimages-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,22 @@
  'rasterio>=1.3.10,<2.0.0',
  'rio-cogeo>=5.3.0,<6.0.0',
  'scikit-image>=0.23.2,<0.24.0',
  'scipy>=1.13.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'geomockimages',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'A module to programmatically create geotiff images which can be used for unit tests.',
     'long_description': '# geomockimages\n\nA module to programmatically create geotiff images which can be used for unit tests.\n\nThe underlying idea is that in order to write unit tests for geospatial image processsing algorithms,\nit is necessary to have an actual input image file or array. Organising these test images becomes a chore over time,\nthey should not be stored in git as they are large binary data and when stored outside, there always\nis the danger that they are not updated according to changes in the code repo.\n\n**geomockimages** provides a solution to the problem by providing simple code that allows to create\ngeospatial images (so far geotiffs) in a parameterised way.\n\n## Install package\n```bash\npip install geomockimages\n```\n\n## Run tests\n```bash\npytest\n```\n\n## Usage\n\nIn the following an example unit test for a hypothetical NDVI function.\n\n```python\nimport numpy as np\nimport rasterio as rio\nfrom pathlib import Path\n\nfrom rasterio.transform import from_origin\nfrom my_image_processing import ndvi\nfrom geomockimages.imagecreator import GeoMockImage\n\ndef test_ndvi():\n    """\n    A unit test if an NDVI method works in general\n    """\n    # Create 4-band image simulating RGBN as needed for NDVI\n    test_image, _ = GeoMockImage(\n        300,\n        150,\n        4,\n        "uint16",\n        out_dir=Path("/tmp"),\n        crs=4326,\n        nodata=0,\n        nodata_fill=3,\n        cog=False,\n    ).create(seed=42, transform=from_origin(13.428596, 52.494384, 0.000006, 0.000006))\n\n    ndvi_image = ndvi(test_image)\n\n    with rio.open(str(ndvi_image)) as src:\n        ndvi_array = src.read()\n        # NDVI only has one band of same size as input bands\n        assert ndvi_array.shape == (1, 150, 300)\n        # NDVI has float values between -1 and 1\n        assert ndvi_array.dtype == np.dtype(\'float32\')\n        assert np.nanmin(ndvi_array) >= -1\n        assert np.nanmax(ndvi_array) <= 1\n\n```\n',
     'author': 'Markus Müller',
     'author_email': 'markus.u.mueller@zoho.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/markusuwe/geomockimages',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `geomockimages-0.2.2/PKG-INFO` & `geomockimages-0.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: geomockimages
-Version: 0.2.2
+Version: 0.2.3
 Summary: A module to programmatically create geotiff images which can be used for unit tests.
+Home-page: https://github.com/markusuwe/geomockimages
 License: MIT
 Author: Markus Müller
 Author-email: markus.u.mueller@zoho.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: rasterio (>=1.3.10,<2.0.0)
 Requires-Dist: rio-cogeo (>=5.3.0,<6.0.0)
 Requires-Dist: scikit-image (>=0.23.2,<0.24.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Project-URL: Repository, https://github.com/markusuwe/geomockimages
 Description-Content-Type: text/markdown
 
 # geomockimages
 
 A module to programmatically create geotiff images which can be used for unit tests.
 
 The underlying idea is that in order to write unit tests for geospatial image processsing algorithms,
```

