# Comparing `tmp/geofileops-0.9.0.tar.gz` & `tmp/geofileops-0.9.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofileops-0.9.0.tar", last modified: Sun May 26 21:21:57 2024, max compression
+gzip compressed data, was "geofileops-0.9.0.post0.tar", last modified: Sun May 26 23:17:23 2024, max compression
```

## Comparing `geofileops-0.9.0.tar` & `geofileops-0.9.0.post0.tar`

### file list

```diff
@@ -1,80 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.801408 geofileops-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-26 21:21:53.000000 geofileops-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-26 21:21:53.000000 geofileops-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-26 21:21:57.801408 geofileops-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-26 21:21:53.000000 geofileops-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.789408 geofileops-0.9.0/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/benchmark_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/benchmark_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/benchmarker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.789408 geofileops-0.9.0/benchmark/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18284 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/benchmarks/benchmarks_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/benchmarks/testdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-05-26 21:21:53.000000 geofileops-0.9.0/benchmark/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.789408 geofileops-0.9.0/geofileops/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    99739 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)   143535 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/geoops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.793408 geofileops-0.9.0/geofileops/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/helpers/_configoptions_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/helpers/_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/helpers/layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.797408 geofileops-0.9.0/geofileops/util/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_general_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_geofileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    89942 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_geoops_ogr.py
--rw-r--r--   0 runner    (1001) docker     (127)   149339 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_io_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    27258 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_sqlite_userdefined.py
--rw-r--r--   0 runner    (1001) docker     (127)    27682 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/geodataframe_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/geofiletypes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    98304 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/util/test.gpkg
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 21:21:53.000000 geofileops-0.9.0/geofileops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.801408 geofileops-0.9.0/geofileops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-26 21:21:57.000000 geofileops-0.9.0/geofileops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-26 21:21:57.000000 geofileops-0.9.0/geofileops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:21:57.000000 geofileops-0.9.0/geofileops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-26 21:21:57.000000 geofileops-0.9.0/geofileops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 21:21:57.000000 geofileops-0.9.0/geofileops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-26 21:21:53.000000 geofileops-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:21:57.801408 geofileops-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-26 21:21:53.000000 geofileops-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:57.801408 geofileops-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_configoptions_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_general_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    65667 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geofile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geofileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    39967 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geofileops_singlelayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    46887 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geofileops_singlelayer_gpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geofileops_singlelayer_ogr.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geofileops_singlelayer_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    81890 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geofileops_twolayers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geoops_dissolve_within_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_io_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_spatialite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_sqlite_userdefined.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 21:21:53.000000 geofileops-0.9.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.220236 geofileops-0.9.0.post0/geofileops/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99739 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143535 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/geoops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.220236 geofileops-0.9.0.post0/geofileops/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/_configoptions_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/helpers/layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.224236 geofileops-0.9.0.post0/geofileops/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geofileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89942 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoops_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149339 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27258 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_sqlite_userdefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27682 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/geodataframe_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/geofiletypes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    98304 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/util/test.gpkg
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/geofileops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/geofileops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 23:17:23.000000 geofileops-0.9.0.post0/geofileops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:17:23.228236 geofileops-0.9.0.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_configoptions_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65667 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39967 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46887 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81890 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geofileops_twolayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoops_dissolve_within_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_spatialite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_sqlite_userdefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 23:17:17.000000 geofileops-0.9.0.post0/tests/test_version.py
```

### Comparing `geofileops-0.9.0/LICENSE.txt` & `geofileops-0.9.0.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/PKG-INFO` & `geofileops-0.9.0.post0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.9.0
+Version: 0.9.0.post0
 Summary: Python toolbox to process large vector files faster.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: cloudpickle
 Requires-Dist: gdal<3.10,>=3.6
 Requires-Dist: geopandas<1,>=0.12
 Requires-Dist: numpy
```

### Comparing `geofileops-0.9.0/README.md` & `geofileops-0.9.0.post0/README.md`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/__init__.py` & `geofileops-0.9.0.post0/geofileops/__init__.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/_compat.py` & `geofileops-0.9.0.post0/geofileops/_compat.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/fileops.py` & `geofileops-0.9.0.post0/geofileops/fileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/geoops.py` & `geofileops-0.9.0.post0/geofileops/geoops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/helpers/_configoptions_helper.py` & `geofileops-0.9.0.post0/geofileops/helpers/_configoptions_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/helpers/_parameter_helper.py` & `geofileops-0.9.0.post0/geofileops/helpers/_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/helpers/layerstyles.py` & `geofileops-0.9.0.post0/geofileops/helpers/layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_general_util.py` & `geofileops-0.9.0.post0/geofileops/util/_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_geofileinfo.py` & `geofileops-0.9.0.post0/geofileops/util/_geofileinfo.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_geometry_util.py` & `geofileops-0.9.0.post0/geofileops/util/_geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_geoops_gpd.py` & `geofileops-0.9.0.post0/geofileops/util/_geoops_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_geoops_ogr.py` & `geofileops-0.9.0.post0/geofileops/util/_geoops_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_geoops_sql.py` & `geofileops-0.9.0.post0/geofileops/util/_geoops_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_geoseries_util.py` & `geofileops-0.9.0.post0/geofileops/util/_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_io_util.py` & `geofileops-0.9.0.post0/geofileops/util/_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_ogr_sql_util.py` & `geofileops-0.9.0.post0/geofileops/util/_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_ogr_util.py` & `geofileops-0.9.0.post0/geofileops/util/_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_processing_util.py` & `geofileops-0.9.0.post0/geofileops/util/_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_sqlite_userdefined.py` & `geofileops-0.9.0.post0/geofileops/util/_sqlite_userdefined.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/_sqlite_util.py` & `geofileops-0.9.0.post0/geofileops/util/_sqlite_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/geodataframe_util.py` & `geofileops-0.9.0.post0/geofileops/util/geodataframe_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/geofiletypes.csv` & `geofileops-0.9.0.post0/geofileops/util/geofiletypes.csv`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops/util/test.gpkg` & `geofileops-0.9.0.post0/geofileops/util/test.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/geofileops.egg-info/PKG-INFO` & `geofileops-0.9.0.post0/geofileops.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.9.0
+Version: 0.9.0.post0
 Summary: Python toolbox to process large vector files faster.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: cloudpickle
 Requires-Dist: gdal<3.10,>=3.6
 Requires-Dist: geopandas<1,>=0.12
 Requires-Dist: numpy
```

### Comparing `geofileops-0.9.0/geofileops.egg-info/SOURCES.txt` & `geofileops-0.9.0.post0/geofileops.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-benchmark/__init__.py
-benchmark/benchmark_all.py
-benchmark/benchmark_geofileops.py
-benchmark/benchmarker.py
-benchmark/reporter.py
-benchmark/benchmarks/__init__.py
-benchmark/benchmarks/benchmarks_geofileops.py
-benchmark/benchmarks/testdata.py
 geofileops/__init__.py
 geofileops/_compat.py
 geofileops/fileops.py
 geofileops/geoops.py
 geofileops/py.typed
 geofileops/version.txt
 geofileops.egg-info/PKG-INFO
@@ -39,15 +31,14 @@
 geofileops/util/_ogr_util.py
 geofileops/util/_processing_util.py
 geofileops/util/_sqlite_userdefined.py
 geofileops/util/_sqlite_util.py
 geofileops/util/geodataframe_util.py
 geofileops/util/geofiletypes.csv
 geofileops/util/test.gpkg
-tests/__init__.py
 tests/test_configoptions_helper.py
 tests/test_general_util.py
 tests/test_geofile.py
 tests/test_geofileinfo.py
 tests/test_geofileops_singlelayer.py
 tests/test_geofileops_singlelayer_gpd.py
 tests/test_geofileops_singlelayer_ogr.py
```

### Comparing `geofileops-0.9.0/pyproject.toml` & `geofileops-0.9.0.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/setup.py` & `geofileops-0.9.0.post0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     author="Pieter Roggemans",
     author_email="pieter.roggemans@gmail.com",
     description="Python toolbox to process large vector files faster.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geofileops/geofileops",
     include_package_data=True,
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(include=["geofileops", "geofileops.*"]),
     install_requires=[
         "cloudpickle",
         "gdal>=3.6,<3.10",
         "geopandas>=0.12,<1",
         "numpy",
         "packaging",
         "pandas",
@@ -32,12 +32,16 @@
         "pygeoops>=0.4,<0.5",
         "pyogrio",
         "pyproj",
         "shapely>=2,<2.1",
     ],
     extras_require={"full": ["simplification"]},
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Scientific/Engineering :: GIS",
     ],
     python_requires=">=3.9",
 )
```

### Comparing `geofileops-0.9.0/tests/test_configoptions_helper.py` & `geofileops-0.9.0.post0/tests/test_configoptions_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_general_util.py` & `geofileops-0.9.0.post0/tests/test_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geofile.py` & `geofileops-0.9.0.post0/tests/test_geofile.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geofileinfo.py` & `geofileops-0.9.0.post0/tests/test_geofileinfo.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geofileops_singlelayer.py` & `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geofileops_singlelayer_gpd.py` & `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geofileops_singlelayer_ogr.py` & `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geofileops_singlelayer_sql.py` & `geofileops-0.9.0.post0/tests/test_geofileops_singlelayer_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geofileops_twolayers.py` & `geofileops-0.9.0.post0/tests/test_geofileops_twolayers.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geoops_dissolve_within_distance.py` & `geofileops-0.9.0.post0/tests/test_geoops_dissolve_within_distance.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geoops_gpd.py` & `geofileops-0.9.0.post0/tests/test_geoops_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geoops_sql.py` & `geofileops-0.9.0.post0/tests/test_geoops_sql.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_geoseries_util.py` & `geofileops-0.9.0.post0/tests/test_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_helper.py` & `geofileops-0.9.0.post0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_io_util.py` & `geofileops-0.9.0.post0/tests/test_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_layerstyles.py` & `geofileops-0.9.0.post0/tests/test_layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_ogr_sql_util.py` & `geofileops-0.9.0.post0/tests/test_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_ogr_util.py` & `geofileops-0.9.0.post0/tests/test_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_parameter_helper.py` & `geofileops-0.9.0.post0/tests/test_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_processing_util.py` & `geofileops-0.9.0.post0/tests/test_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_spatialite.py` & `geofileops-0.9.0.post0/tests/test_spatialite.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_sqlite_userdefined.py` & `geofileops-0.9.0.post0/tests/test_sqlite_userdefined.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.9.0/tests/test_sqlite_util.py` & `geofileops-0.9.0.post0/tests/test_sqlite_util.py`

 * *Files identical despite different names*

