# Comparing `tmp/test_core_package-1.1.2.tar.gz` & `tmp/test_core_package-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_core_package-1.1.2.tar", last modified: Thu May 23 10:59:17 2024, max compression
+gzip compressed data, was "test_core_package-1.2.0.tar", last modified: Mon May 27 10:41:42 2024, max compression
```

## Comparing `test_core_package-1.1.2.tar` & `test_core_package-1.2.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.828848 test_core_package-1.1.2/
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.1.2/LICENCE.txt
--rw-rw-rw-   0        0        0      965 2024-05-23 10:59:17.828848 test_core_package-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.541972 test_core_package-1.1.2/qa_qc_check/
--rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-1.1.2/qa_qc_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.569877 test_core_package-1.1.2/qa_qc_check/controller/
--rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-1.1.2/qa_qc_check/controller/__init__.py
--rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-1.1.2/qa_qc_check/controller/checks.json
--rw-rw-rw-   0        0        0     4274 2024-05-23 07:44:29.000000 test_core_package-1.1.2/qa_qc_check/controller/meta_data.py
--rw-rw-rw-   0        0        0     9310 2024-05-23 09:34:46.000000 test_core_package-1.1.2/qa_qc_check/controller/meta_data_extractor.py
--rw-rw-rw-   0        0        0     1581 2024-05-22 12:18:45.000000 test_core_package-1.1.2/qa_qc_check/controller/qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.574175 test_core_package-1.1.2/qa_qc_check/model/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-1.1.2/qa_qc_check/model/__init__.py
--rw-rw-rw-   0        0        0      932 2024-05-22 12:18:49.000000 test_core_package-1.1.2/qa_qc_check/model/metadata_model.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.582284 test_core_package-1.1.2/qa_qc_check/test/
--rw-rw-rw-   0        0        0        0 2024-05-22 12:18:30.000000 test_core_package-1.1.2/qa_qc_check/test/__init__.py
--rw-rw-rw-   0        0        0    15150 2024-05-23 09:34:42.000000 test_core_package-1.1.2/qa_qc_check/test/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.595127 test_core_package-1.1.2/qa_qc_check/test/controller/
--rw-rw-rw-   0        0        0        0 2024-05-22 12:18:24.000000 test_core_package-1.1.2/qa_qc_check/test/controller/__init__.py
--rw-rw-rw-   0        0        0      434 2024-05-23 09:32:01.000000 test_core_package-1.1.2/qa_qc_check/test/controller/test_meta_data.py
--rw-rw-rw-   0        0        0      496 2024-05-23 09:34:39.000000 test_core_package-1.1.2/qa_qc_check/test/controller/test_meta_data_extractor.py
--rw-rw-rw-   0        0        0      265 2024-05-23 09:34:26.000000 test_core_package-1.1.2/qa_qc_check/test/controller/test_qa_qc.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.613141 test_core_package-1.1.2/qa_qc_check/validator/
--rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-1.1.2/qa_qc_check/validator/__init__.py
--rw-rw-rw-   0        0        0     1955 2024-05-23 09:35:03.000000 test_core_package-1.1.2/qa_qc_check/validator/meta_data_validator.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.659445 test_core_package-1.1.2/satelite/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.2/satelite/__init__.py
--rw-rw-rw-   0        0        0     1011 2024-05-17 11:24:27.000000 test_core_package-1.1.2/satelite/config.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.659445 test_core_package-1.1.2/satelite/core/
--rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/core/__init__.py
--rw-rw-rw-   0        0        0     2552 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/core/downloader.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.659445 test_core_package-1.1.2/satelite/gdal/
--rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/gdal/__init__.py
--rw-rw-rw-   0        0        0     2620 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/gdal/gdal_commands.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.676331 test_core_package-1.1.2/satelite/models/
--rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/models/__init__.py
--rw-rw-rw-   0        0        0      388 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/models/s2_enum.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.695077 test_core_package-1.1.2/satelite/raster/
--rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/raster/__init__.py
--rw-rw-rw-   0        0        0     9161 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/raster/raster.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.734509 test_core_package-1.1.2/satelite/sentinel2/
--rw-rw-rw-   0        0        0      457 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.739137 test_core_package-1.1.2/satelite/sentinel2/band_stack/
--rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/band_stack/__init__.py
--rw-rw-rw-   0        0        0     2903 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-rw-rw-   0        0        0     2488 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-1.1.2/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     3248 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/get_tiles.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.742257 test_core_package-1.1.2/satelite/sentinel2/indices/
--rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/indices/__init__.py
--rw-rw-rw-   0        0        0     4320 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/indices/general_indices.py
--rw-rw-rw-   0        0        0     2534 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/mosaic_same_bands.py
--rw-rw-rw-   0        0        0     1548 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/path_row_from_shp.py
--rw-rw-rw-   0        0        0     3337 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/s2_l1c_urls.py
--rw-rw-rw-   0        0        0     2992 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/sentinel2/s2_l2a_urls.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.749699 test_core_package-1.1.2/satelite/tests/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.2/satelite/tests/__init__.py
--rw-rw-rw-   0        0        0     1038 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.777885 test_core_package-1.1.2/satelite/tests/sentinel2/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.1.2/satelite/tests/sentinel2/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-1.1.2/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-1.1.2/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-rw-rw-   0        0        0     1366 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/tests/sentinel2/test_get_tile.py
--rw-rw-rw-   0        0        0      334 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-rw-rw-   0        0        0      906 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-rw-rw-   0        0        0      931 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-rw-rw-   0        0        0     1594 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/tests/sentinel2/test_validate.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.783281 test_core_package-1.1.2/satelite/validators/
--rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/validators/__init__.py
--rw-rw-rw-   0        0        0     2446 2024-05-14 07:37:16.000000 test_core_package-1.1.2/satelite/validators/check_shape_of_rid.py
--rw-rw-rw-   0        0        0       42 2024-05-23 10:59:17.828848 test_core_package-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1037 2024-05-23 10:59:12.000000 test_core_package-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:59:17.827416 test_core_package-1.1.2/test_core_package.egg-info/
--rw-rw-rw-   0        0        0      965 2024-05-23 10:59:17.000000 test_core_package-1.1.2/test_core_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2086 2024-05-23 10:59:17.000000 test_core_package-1.1.2/test_core_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:59:17.000000 test_core_package-1.1.2/test_core_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      362 2024-05-23 10:59:17.000000 test_core_package-1.1.2/test_core_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-23 10:59:17.000000 test_core_package-1.1.2/test_core_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.690145 test_core_package-1.2.0/
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.2.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      965 2024-05-27 10:41:42.689139 test_core_package-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-29 09:27:23.000000 test_core_package-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.265177 test_core_package-1.2.0/qa_qc_check/
+-rw-rw-rw-   0        0        0        0 2024-05-07 12:52:35.000000 test_core_package-1.2.0/qa_qc_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.285733 test_core_package-1.2.0/qa_qc_check/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-02 09:51:13.000000 test_core_package-1.2.0/qa_qc_check/controller/__init__.py
+-rw-rw-rw-   0        0        0     4161 2024-05-06 12:22:37.000000 test_core_package-1.2.0/qa_qc_check/controller/checks.json
+-rw-rw-rw-   0        0        0     4274 2024-05-23 07:44:29.000000 test_core_package-1.2.0/qa_qc_check/controller/meta_data.py
+-rw-rw-rw-   0        0        0     9310 2024-05-23 09:34:46.000000 test_core_package-1.2.0/qa_qc_check/controller/meta_data_extractor.py
+-rw-rw-rw-   0        0        0     1581 2024-05-22 12:18:45.000000 test_core_package-1.2.0/qa_qc_check/controller/qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.289241 test_core_package-1.2.0/qa_qc_check/model/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:48.000000 test_core_package-1.2.0/qa_qc_check/model/__init__.py
+-rw-rw-rw-   0        0        0      932 2024-05-22 12:18:49.000000 test_core_package-1.2.0/qa_qc_check/model/metadata_model.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.291607 test_core_package-1.2.0/qa_qc_check/test/
+-rw-rw-rw-   0        0        0        0 2024-05-22 12:18:30.000000 test_core_package-1.2.0/qa_qc_check/test/__init__.py
+-rw-rw-rw-   0        0        0    15150 2024-05-23 09:34:42.000000 test_core_package-1.2.0/qa_qc_check/test/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.300556 test_core_package-1.2.0/qa_qc_check/test/controller/
+-rw-rw-rw-   0        0        0        0 2024-05-22 12:18:24.000000 test_core_package-1.2.0/qa_qc_check/test/controller/__init__.py
+-rw-rw-rw-   0        0        0      434 2024-05-23 09:32:01.000000 test_core_package-1.2.0/qa_qc_check/test/controller/test_meta_data.py
+-rw-rw-rw-   0        0        0      496 2024-05-23 09:34:39.000000 test_core_package-1.2.0/qa_qc_check/test/controller/test_meta_data_extractor.py
+-rw-rw-rw-   0        0        0      265 2024-05-23 09:34:26.000000 test_core_package-1.2.0/qa_qc_check/test/controller/test_qa_qc.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.303703 test_core_package-1.2.0/qa_qc_check/validator/
+-rw-rw-rw-   0        0        0        0 2024-05-13 08:52:55.000000 test_core_package-1.2.0/qa_qc_check/validator/__init__.py
+-rw-rw-rw-   0        0        0     1955 2024-05-23 09:35:03.000000 test_core_package-1.2.0/qa_qc_check/validator/meta_data_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.317862 test_core_package-1.2.0/satelite/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.2.0/satelite/__init__.py
+-rw-rw-rw-   0        0        0     1011 2024-05-17 11:24:27.000000 test_core_package-1.2.0/satelite/config.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.332920 test_core_package-1.2.0/satelite/core/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/core/__init__.py
+-rw-rw-rw-   0        0        0     2552 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/core/downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.349285 test_core_package-1.2.0/satelite/gdal/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/gdal/__init__.py
+-rw-rw-rw-   0        0        0     2620 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/gdal/gdal_commands.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.361112 test_core_package-1.2.0/satelite/models/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/models/__init__.py
+-rw-rw-rw-   0        0        0      388 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/models/s2_enum.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.400957 test_core_package-1.2.0/satelite/raster/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/raster/__init__.py
+-rw-rw-rw-   0        0        0     9161 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/raster/raster.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.498295 test_core_package-1.2.0/satelite/sentinel2/
+-rw-rw-rw-   0        0        0      457 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.508266 test_core_package-1.2.0/satelite/sentinel2/band_stack/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/band_stack/__init__.py
+-rw-rw-rw-   0        0        0     2903 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-rw-rw-   0        0        0     2488 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0     1679 2024-05-07 11:29:36.000000 test_core_package-1.2.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     3248 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/get_tiles.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.523837 test_core_package-1.2.0/satelite/sentinel2/indices/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/indices/__init__.py
+-rw-rw-rw-   0        0        0     4320 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/indices/general_indices.py
+-rw-rw-rw-   0        0        0     2534 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/mosaic_same_bands.py
+-rw-rw-rw-   0        0        0     1548 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/path_row_from_shp.py
+-rw-rw-rw-   0        0        0     3337 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/s2_l1c_urls.py
+-rw-rw-rw-   0        0        0     2992 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/sentinel2/s2_l2a_urls.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.535412 test_core_package-1.2.0/satelite/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.2.0/satelite/tests/__init__.py
+-rw-rw-rw-   0        0        0     1038 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.623152 test_core_package-1.2.0/satelite/tests/sentinel2/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:29:36.000000 test_core_package-1.2.0/satelite/tests/sentinel2/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-07 11:29:36.000000 test_core_package-1.2.0/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-rw-rw-   0        0        0      443 2024-05-07 11:29:36.000000 test_core_package-1.2.0/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-rw-rw-   0        0        0     1366 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/tests/sentinel2/test_get_tile.py
+-rw-rw-rw-   0        0        0      334 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-rw-rw-   0        0        0      906 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-rw-rw-   0        0        0      931 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-rw-rw-   0        0        0     1594 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/tests/sentinel2/test_validate.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.647594 test_core_package-1.2.0/satelite/validators/
+-rw-rw-rw-   0        0        0        0 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/validators/__init__.py
+-rw-rw-rw-   0        0        0     2446 2024-05-14 07:37:16.000000 test_core_package-1.2.0/satelite/validators/check_shape_of_rid.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:41:42.690145 test_core_package-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2024-05-27 10:39:47.000000 test_core_package-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:42.679671 test_core_package-1.2.0/test_core_package.egg-info/
+-rw-rw-rw-   0        0        0      965 2024-05-27 10:41:41.000000 test_core_package-1.2.0/test_core_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2086 2024-05-27 10:41:42.000000 test_core_package-1.2.0/test_core_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:41:41.000000 test_core_package-1.2.0/test_core_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      362 2024-05-27 10:41:41.000000 test_core_package-1.2.0/test_core_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-27 10:41:41.000000 test_core_package-1.2.0/test_core_package.egg-info/top_level.txt
```

### Comparing `test_core_package-1.1.2/PKG-INFO` & `test_core_package-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-core-package
-Version: 1.1.2
+Version: 1.2.0
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: requests
 Requires-Dist: fiona
 Requires-Dist: pandas
```

### Comparing `test_core_package-1.1.2/qa_qc_check/controller/checks.json` & `test_core_package-1.2.0/qa_qc_check/controller/checks.json`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/qa_qc_check/controller/meta_data.py` & `test_core_package-1.2.0/qa_qc_check/controller/meta_data.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/qa_qc_check/controller/meta_data_extractor.py` & `test_core_package-1.2.0/qa_qc_check/controller/meta_data_extractor.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/qa_qc_check/controller/qa_qc.py` & `test_core_package-1.2.0/qa_qc_check/controller/qa_qc.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/qa_qc_check/model/metadata_model.py` & `test_core_package-1.2.0/qa_qc_check/model/metadata_model.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/qa_qc_check/test/conftest.py` & `test_core_package-1.2.0/qa_qc_check/test/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/qa_qc_check/validator/meta_data_validator.py` & `test_core_package-1.2.0/qa_qc_check/validator/meta_data_validator.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/config.py` & `test_core_package-1.2.0/satelite/config.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/core/downloader.py` & `test_core_package-1.2.0/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/gdal/gdal_commands.py` & `test_core_package-1.2.0/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/raster/raster.py` & `test_core_package-1.2.0/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/band_stack/generate_band_stack.py` & `test_core_package-1.2.0/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/fetch_unique_tile_date.py` & `test_core_package-1.2.0/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `test_core_package-1.2.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/get_tiles.py` & `test_core_package-1.2.0/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/indices/general_indices.py` & `test_core_package-1.2.0/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/mosaic_same_bands.py` & `test_core_package-1.2.0/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/path_row_from_shp.py` & `test_core_package-1.2.0/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/s2_l1c_urls.py` & `test_core_package-1.2.0/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/sentinel2/s2_l2a_urls.py` & `test_core_package-1.2.0/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/tests/conftest.py` & `test_core_package-1.2.0/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/tests/sentinel2/test_get_tile.py` & `test_core_package-1.2.0/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `test_core_package-1.2.0/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `test_core_package-1.2.0/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/tests/sentinel2/test_validate.py` & `test_core_package-1.2.0/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/satelite/validators/check_shape_of_rid.py` & `test_core_package-1.2.0/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `test_core_package-1.1.2/setup.py` & `test_core_package-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="test-core-package",
-    version="1.1.2",
+    version="1.2.0",
     description="satsure core package",
     author="Satsure",
     author_email="kmstpm@email.com",
     packages=find_packages(),
     install_requires=[
         "requests",
         "fiona",
```

### Comparing `test_core_package-1.1.2/test_core_package.egg-info/PKG-INFO` & `test_core_package-1.2.0/test_core_package.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-core-package
-Version: 1.1.2
+Version: 1.2.0
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: requests
 Requires-Dist: fiona
 Requires-Dist: pandas
```

### Comparing `test_core_package-1.1.2/test_core_package.egg-info/SOURCES.txt` & `test_core_package-1.2.0/test_core_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

