# Comparing `tmp/geefcc-0.1.tar.gz` & `tmp/geefcc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geefcc-0.1.tar", last modified: Thu May 23 05:06:29 2024, max compression
+gzip compressed data, was "geefcc-0.1.1.tar", last modified: Mon May 27 02:24:05 2024, max compression
```

## Comparing `geefcc-0.1.tar` & `geefcc-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:06:29.873624 geefcc-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 05:06:27.000000 geefcc-0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 05:06:27.000000 geefcc-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 05:06:27.000000 geefcc-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-23 05:06:29.869624 geefcc-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-23 05:06:27.000000 geefcc-0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:06:29.869624 geefcc-0.1/geefcc/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/download_gadm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/ee_gfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/ee_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/ee_tmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/geefcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/geeic2geotiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/geotiff_from_tiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/get_extent_from_aoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/get_fcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/get_vector_extent.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/make_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-23 05:06:27.000000 geefcc-0.1/geefcc/make_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:06:29.869624 geefcc-0.1/geefcc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-23 05:06:29.000000 geefcc-0.1/geefcc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-23 05:06:29.000000 geefcc-0.1/geefcc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:06:29.000000 geefcc-0.1/geefcc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 05:06:29.000000 geefcc-0.1/geefcc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:06:29.000000 geefcc-0.1/geefcc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 05:06:29.000000 geefcc-0.1/geefcc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 05:06:29.000000 geefcc-0.1/geefcc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 05:06:29.873624 geefcc-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-23 05:06:27.000000 geefcc-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:06:29.869624 geefcc-0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 05:06:27.000000 geefcc-0.1/test/test_get_fcc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-27 02:24:03.000000 geefcc-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 02:24:03.000000 geefcc-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 02:24:03.000000 geefcc-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-27 02:24:05.443144 geefcc-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-27 02:24:03.000000 geefcc-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/geefcc/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/download_gadm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/ee_gfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/ee_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/ee_tmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/geefcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/geeic2geotiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/geotiff_from_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/get_extent_from_aoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/get_fcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/get_vector_extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/make_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/sum_raster_bands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/geefcc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 02:24:05.447144 geefcc-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-27 02:24:03.000000 geefcc-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-27 02:24:03.000000 geefcc-0.1.1/test/test_get_fcc.py
```

### Comparing `geefcc-0.1/LICENSE` & `geefcc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/PKG-INFO` & `geefcc-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geefcc
-Version: 0.1
+Version: 0.1.1
 Summary: Forest cover change from Google Earth Engine
 Home-page: https://ecology.ghislainv.fr/geefcc
 Author: Ghislain Vieilledent
 Author-email: ghislain.vieilledent@cirad.fr
 License: GPLv3
 Project-URL: Documentation, https://ecology.ghislainv.fr/geefcc
 Project-URL: Source, https://github.com/ghislainv/geefcc/
@@ -176,11 +176,11 @@
    :target: https://github.com/ghislainv/geefcc/actions
    :alt: GitHub Actions
 	 
 .. |License| image:: https://img.shields.io/badge/licence-GPLv3-8f10cb.svg
    :target: https://www.gnu.org/licenses/gpl-3.0.html
    :alt: License GPLv3
 
-.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4275513.svg
-   :target: https://doi.org/10.5281/zenodo.4275513
+.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.11258039.svg
+   :target: https://doi.org/10.5281/zenodo.11258039
    :alt: Zenodo
```

### Comparing `geefcc-0.1/README.rst` & `geefcc-0.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -146,11 +146,11 @@
    :target: https://github.com/ghislainv/geefcc/actions
    :alt: GitHub Actions
 	 
 .. |License| image:: https://img.shields.io/badge/licence-GPLv3-8f10cb.svg
    :target: https://www.gnu.org/licenses/gpl-3.0.html
    :alt: License GPLv3
 
-.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4275513.svg
-   :target: https://doi.org/10.5281/zenodo.4275513
+.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.11258039.svg
+   :target: https://doi.org/10.5281/zenodo.11258039
    :alt: Zenodo
```

### Comparing `geefcc-0.1/geefcc/download_gadm.py` & `geefcc-0.1.1/geefcc/download_gadm.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/geefcc/ee_gfc.py` & `geefcc-0.1.1/geefcc/ee_gfc.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/geefcc/ee_initialize.py` & `geefcc-0.1.1/geefcc/ee_initialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,9 +43,11 @@
             credential = (
                 '{"refresh_token":"%s"}' % ee_token
             )  # deals with token generated by old auth method.
             with open(credential_file_path, "w", encoding="utf-8") as f:
                 f.write(credential)
 
     # Initialize
-    ee.Initialize(project=project,
-                  **kwargs)
+    ee.Initialize(project=project, **kwargs)
+
+
+# End
```

### Comparing `geefcc-0.1/geefcc/ee_tmf.py` & `geefcc-0.1.1/geefcc/ee_tmf.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/geefcc/geefcc.py` & `geefcc-0.1.1/geefcc/geefcc.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/geefcc/geeic2geotiff.py` & `geefcc-0.1.1/geefcc/geeic2geotiff.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,29 +175,31 @@
     :param forest: Forest image collection from GEE.
     :param proj: Projection.
     :param scale: Scale.
     :param output_dir: Output directory.
 
     """
 
-    # Open dataset
-    ds = (
-        xr.open_dataset(
-            forest,
-            engine="ee",
-            crs=proj,
-            scale=scale,
-            geometry=extent,
-            chunks={"time": -1},
+    ofile = os.path.join(out_dir, f"forest_{index}.tif")
+    if not os.path.isfile(ofile):
+        # Open dataset
+        ds = (
+            xr.open_dataset(
+                forest,
+                engine="ee",
+                crs=proj,
+                scale=scale,
+                geometry=extent,
+                chunks={"time": -1},
+            )
+            .astype("b")
+            .rename({"lon": "longitude", "lat": "latitude"})
         )
-        .astype("b")
-        .rename({"lon": "longitude", "lat": "latitude"})
-    )
-    ds = ds.load()
+        ds = ds.load()
 
-    # Load and write data to geotiff
-    xarray2geotiff(ds, "forest_cover", out_dir, index)
+        # Load and write data to geotiff
+        xarray2geotiff(ds, "forest_cover", out_dir, index)
 
-    # Progress bar
-    progress_bar_async(index, ntiles)
+        # Progress bar
+        progress_bar_async(index, ntiles)
 
 # End Of File
```

### Comparing `geefcc-0.1/geefcc/get_extent_from_aoi.py` & `geefcc-0.1.1/geefcc/get_extent_from_aoi.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/geefcc/get_fcc.py` & `geefcc-0.1.1/geefcc/get_fcc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Get forest cover change data."""
 
 import os
 import multiprocessing as mp
 
 from .get_extent_from_aoi import get_extent_from_aoi
-from .make_dir import make_dir
+from .misc import make_dir
 from .make_grid import make_grid, grid_intersection
 from .geeic2geotiff import geeic2geotiff
 from .geotiff_from_tiles import geotiff_from_tiles
 from .ee_tmf import ee_tmf
 from .ee_gfc import ee_gfc
 
 opj = os.path.join
@@ -17,14 +17,16 @@
 
 def get_fcc(aoi,
             buff=0,
             years=[2000, 2010, 2020],
             source="tmf",
             perc=75,
             tile_size=1,
+            # crop_to_aoi=False,
+            ncpu=None,
             output_file="fcc.tif"):
     """Get forest cover change data.
 
      Produce a forest cover change raster file. One band for each
      year. Value 1 for forest and 0 for non-forest.
 
     :param aoi: Area of interest defined either by a country iso code
@@ -45,14 +47,19 @@
         defining the forest must be specified with parameter ``perc``.
 
     :param perc: Tree cover threshold defining the forest for GFC
         product.
 
     :param tile_size: Tile size for parallel computing.
 
+    :param ncpu: Number of CPU to use for parallel computing.
+
+    :param crop_to_aoi: Crop the raster GeoTIFF file to aoi. If False,
+        the output file will match the grid covering the aoi with buffer.
+
     :param output_file: Path to output GeoTIFF file. If directories in path
         do not exist they will be created.
 
     """
 
     # Output dir
     out_dir = opd(output_file)
@@ -92,26 +99,27 @@
 
     # Create dir for forest tiles
     out_dir_tiles = opj(out_dir, "forest_tiles")
     make_dir(out_dir_tiles)
 
     # Write tiles in parallel
     # https://superfastpython.com/multiprocessing-pool-starmap_async/
-    ncpu = os.cpu_count() - 1
     # Message
     print(f"get_fcc running, {ntiles} tiles .", end="", flush=True)
     # create and configure the process pool
+    if ncpu is None:
+        ncpu = os.cpu_count() - 1
     with mp.Pool(processes=ncpu) as pool:
         # prepare arguments
         args = [(i, ext, ntiles, forest, proj, scale, out_dir_tiles)
                 for (i, ext) in enumerate(grid)]
         # issue many tasks asynchronously to the process pool
         _ = pool.starmap_async(geeic2geotiff, args)
         # close the pool
         pool.close()
         # wait for all issued tasks to complete
         pool.join()
 
     # Geotiff from tiles
-    geotiff_from_tiles(extent_latlong, scale, output_file)
+    geotiff_from_tiles(output_file)
 
 # End
```

### Comparing `geefcc-0.1/geefcc/get_vector_extent.py` & `geefcc-0.1.1/geefcc/get_vector_extent.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/geefcc/make_grid.py` & `geefcc-0.1.1/geefcc/make_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 
     :param input_file: Input filename.
     :param output_file: Output filename (`.gpkg`).
     :param buffer_dist: Buffer distance (in unit of CRS).
 
     """
     input_ds = ogr.Open(input_file)
-    input_lyr = input_ds.GetLayer()
+    # Get first layer
+    input_lyr = input_ds.GetLayer(0)
 
     driver = ogr.GetDriverByName("GPKG")
     if os.path.exists(output_file):
         driver.DeleteDataSource(output_file)
     ds = driver.CreateDataSource(output_file)
+    # Must be MultiPolygon here
     lyr = ds.CreateLayer(
         "buffer",
-        geom_type=ogr.wkbPolygon)
+        geom_type=ogr.wkbMultiPolygon)
     feature_defn = lyr.GetLayerDefn()
 
     for feature in input_lyr:
         in_geom = feature.GetGeometryRef()
         geom_buffer = in_geom.Buffer(buffer_dist)
 
         out_feature = ogr.Feature(feature_defn)
```

### Comparing `geefcc-0.1/geefcc.egg-info/PKG-INFO` & `geefcc-0.1.1/geefcc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geefcc
-Version: 0.1
+Version: 0.1.1
 Summary: Forest cover change from Google Earth Engine
 Home-page: https://ecology.ghislainv.fr/geefcc
 Author: Ghislain Vieilledent
 Author-email: ghislain.vieilledent@cirad.fr
 License: GPLv3
 Project-URL: Documentation, https://ecology.ghislainv.fr/geefcc
 Project-URL: Source, https://github.com/ghislainv/geefcc/
@@ -176,11 +176,11 @@
    :target: https://github.com/ghislainv/geefcc/actions
    :alt: GitHub Actions
 	 
 .. |License| image:: https://img.shields.io/badge/licence-GPLv3-8f10cb.svg
    :target: https://www.gnu.org/licenses/gpl-3.0.html
    :alt: License GPLv3
 
-.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4275513.svg
-   :target: https://doi.org/10.5281/zenodo.4275513
+.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.11258039.svg
+   :target: https://doi.org/10.5281/zenodo.11258039
    :alt: Zenodo
```

### Comparing `geefcc-0.1/geefcc.egg-info/SOURCES.txt` & `geefcc-0.1.1/geefcc.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 geefcc/ee_tmf.py
 geefcc/geefcc.py
 geefcc/geeic2geotiff.py
 geefcc/geotiff_from_tiles.py
 geefcc/get_extent_from_aoi.py
 geefcc/get_fcc.py
 geefcc/get_vector_extent.py
-geefcc/make_dir.py
 geefcc/make_grid.py
+geefcc/sum_raster_bands.py
 geefcc.egg-info/PKG-INFO
 geefcc.egg-info/SOURCES.txt
 geefcc.egg-info/dependency_links.txt
 geefcc.egg-info/entry_points.txt
 geefcc.egg-info/not-zip-safe
 geefcc.egg-info/requires.txt
 geefcc.egg-info/top_level.txt
```

### Comparing `geefcc-0.1/setup.py` & `geefcc-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1/test/test_get_fcc.py` & `geefcc-0.1.1/test/test_get_fcc.py`

 * *Files identical despite different names*

