# Comparing `tmp/geofileops-0.9.0.post0.tar.gz` & `tmp/geofileops-0.9.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofileops-0.9.0.post0.tar", last modified: Sun May 26 23:17:23 2024, max compression
+gzip compressed data, was "geofileops-0.9.0.post2.tar", last modified: Sun May 26 23:33:53 2024, max compression
```

## Comparing `geofileops-0.9.0.post0.tar` & `geofileops-0.9.0.post2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.220236 geofileops-0.9.0.post0/geofileops/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    99739 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)   143535 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/geoops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.220236 geofileops-0.9.0.post0/geofileops/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/_configoptions_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.224236 geofileops-0.9.0.post0/geofileops/util/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_general_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geofileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    89942 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoops_ogr.py
--rw-r--r--   0 runner    (1001) docker     (127)   149339 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_io_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    27258 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_sqlite_userdefined.py
--rw-r--r--   0 runner    (1001) docker     (127)    27682 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/geodataframe_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/geofiletypes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    98304 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/test.gpkg
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/geofileops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_configoptions_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_general_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    65667 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    39967 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    46887 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_gpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_ogr.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    81890 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_twolayers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoops_dissolve_within_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_io_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_spatialite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_sqlite_userdefined.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:33:53.876884 geofileops-0.9.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-26 23:33:53.876884 geofileops-0.9.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:33:53.868884 geofileops-0.9.0.post2/geofileops/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99739 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143535 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/geoops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:33:53.868884 geofileops-0.9.0.post2/geofileops/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/helpers/_configoptions_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/helpers/_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/helpers/layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:33:53.872884 geofileops-0.9.0.post2/geofileops/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_geofileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89942 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_geoops_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149339 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27258 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_sqlite_userdefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27682 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/geodataframe_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/geofiletypes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    98304 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/util/test.gpkg
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/geofileops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:33:53.876884 geofileops-0.9.0.post2/geofileops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-26 23:33:53.000000 geofileops-0.9.0.post2/geofileops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-26 23:33:53.000000 geofileops-0.9.0.post2/geofileops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:33:53.000000 geofileops-0.9.0.post2/geofileops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-26 23:33:53.000000 geofileops-0.9.0.post2/geofileops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 23:33:53.000000 geofileops-0.9.0.post2/geofileops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:33:53.876884 geofileops-0.9.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:33:53.876884 geofileops-0.9.0.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_configoptions_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65667 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geofileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39967 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geofileops_singlelayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46887 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geofileops_singlelayer_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geofileops_singlelayer_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geofileops_singlelayer_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81890 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geofileops_twolayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geoops_dissolve_within_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_spatialite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_sqlite_userdefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 23:33:49.000000 geofileops-0.9.0.post2/tests/test_version.py
```

### Comparing `geofileops-0.9.0.post0/LICENSE.txt` & `geofileops-0.9.0.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/PKG-INFO` & `geofileops-0.9.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.9.0.post0
+Version: 0.9.0.post2
 Summary: Python toolbox to process large vector files faster.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `geofileops-0.9.0.post0/README.md` & `geofileops-0.9.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/__init__.py` & `geofileops-0.9.0.post2/geofileops/__init__.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/_compat.py` & `geofileops-0.9.0.post2/geofileops/_compat.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/fileops.py` & `geofileops-0.9.0.post2/geofileops/fileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/geoops.py` & `geofileops-0.9.0.post2/geofileops/geoops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/helpers/_configoptions_helper.py` & `geofileops-0.9.0.post2/geofileops/helpers/_configoptions_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/helpers/_parameter_helper.py` & `geofileops-0.9.0.post2/geofileops/helpers/_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/helpers/layerstyles.py` & `geofileops-0.9.0.post2/geofileops/helpers/layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_general_util.py` & `geofileops-0.9.0.post2/geofileops/util/_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_geofileinfo.py` & `geofileops-0.9.0.post2/geofileops/util/_geofileinfo.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_geometry_util.py` & `geofileops-0.9.0.post2/geofileops/util/_geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_geoops_gpd.py` & `geofileops-0.9.0.post2/geofileops/util/_geoops_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_geoops_ogr.py` & `geofileops-0.9.0.post2/geofileops/util/_geoops_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_geoops_sql.py` & `geofileops-0.9.0.post2/geofileops/util/_geoops_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_geoseries_util.py` & `geofileops-0.9.0.post2/geofileops/util/_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_io_util.py` & `geofileops-0.9.0.post2/geofileops/util/_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_ogr_sql_util.py` & `geofileops-0.9.0.post2/geofileops/util/_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_ogr_util.py` & `geofileops-0.9.0.post2/geofileops/util/_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_processing_util.py` & `geofileops-0.9.0.post2/geofileops/util/_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_sqlite_userdefined.py` & `geofileops-0.9.0.post2/geofileops/util/_sqlite_userdefined.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/_sqlite_util.py` & `geofileops-0.9.0.post2/geofileops/util/_sqlite_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/geodataframe_util.py` & `geofileops-0.9.0.post2/geofileops/util/geodataframe_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/geofiletypes.csv` & `geofileops-0.9.0.post2/geofileops/util/geofiletypes.csv`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops/util/test.gpkg` & `geofileops-0.9.0.post2/geofileops/util/test.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/geofileops.egg-info/PKG-INFO` & `geofileops-0.9.0.post2/geofileops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.9.0.post0
+Version: 0.9.0.post2
 Summary: Python toolbox to process large vector files faster.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `geofileops-0.9.0.post0/geofileops.egg-info/SOURCES.txt` & `geofileops-0.9.0.post2/geofileops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/pyproject.toml` & `geofileops-0.9.0.post2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -140,16 +140,14 @@
     "D200",
     # Multi-line docstring summary should start at the first line
     "D212",
 ]
 exclude = [
     "docs/*",
     "local_ignore/*",
-    "versioneer.py",
-    "geopandas/_version.py",
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = ["D"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
```

### Comparing `geofileops-0.9.0.post0/setup.py` & `geofileops-0.9.0.post2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     author="Pieter Roggemans",
     author_email="pieter.roggemans@gmail.com",
     description="Python toolbox to process large vector files faster.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geofileops/geofileops",
     include_package_data=True,
-    packages=setuptools.find_packages(include=["geofileops", "geofileops.*"]),
+    packages=setuptools.find_packages(
+        exclude=("tests", "benchmark", "benchmark.*"),
+        include=("geofileops", "geofileops.*"),
+    ),
     install_requires=[
         "cloudpickle",
         "gdal>=3.6,<3.10",
         "geopandas>=0.12,<1",
         "numpy",
         "packaging",
         "pandas",
```

### Comparing `geofileops-0.9.0.post0/tests/test_configoptions_helper.py` & `geofileops-0.9.0.post2/tests/test_configoptions_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_general_util.py` & `geofileops-0.9.0.post2/tests/test_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geofile.py` & `geofileops-0.9.0.post2/tests/test_geofile.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geofileinfo.py` & `geofileops-0.9.0.post2/tests/test_geofileinfo.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer.py` & `geofileops-0.9.0.post2/tests/test_geofileops_singlelayer.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_gpd.py` & `geofileops-0.9.0.post2/tests/test_geofileops_singlelayer_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_ogr.py` & `geofileops-0.9.0.post2/tests/test_geofileops_singlelayer_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_sql.py` & `geofileops-0.9.0.post2/tests/test_geofileops_singlelayer_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geofileops_twolayers.py` & `geofileops-0.9.0.post2/tests/test_geofileops_twolayers.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geoops_dissolve_within_distance.py` & `geofileops-0.9.0.post2/tests/test_geoops_dissolve_within_distance.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geoops_gpd.py` & `geofileops-0.9.0.post2/tests/test_geoops_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geoops_sql.py` & `geofileops-0.9.0.post2/tests/test_geoops_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_geoseries_util.py` & `geofileops-0.9.0.post2/tests/test_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_helper.py` & `geofileops-0.9.0.post2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_io_util.py` & `geofileops-0.9.0.post2/tests/test_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_layerstyles.py` & `geofileops-0.9.0.post2/tests/test_layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_ogr_sql_util.py` & `geofileops-0.9.0.post2/tests/test_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_ogr_util.py` & `geofileops-0.9.0.post2/tests/test_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_parameter_helper.py` & `geofileops-0.9.0.post2/tests/test_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_processing_util.py` & `geofileops-0.9.0.post2/tests/test_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_spatialite.py` & `geofileops-0.9.0.post2/tests/test_spatialite.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_sqlite_userdefined.py` & `geofileops-0.9.0.post2/tests/test_sqlite_userdefined.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0.post0/tests/test_sqlite_util.py` & `geofileops-0.9.0.post2/tests/test_sqlite_util.py`

 * *Files identical despite different names*

