# Comparing `tmp/strax-1.6.3.tar.gz` & `tmp/strax-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strax-1.6.3.tar", last modified: Tue Apr 30 23:08:24 2024, max compression
+gzip compressed data, was "strax-1.6.4.tar", last modified: Mon May 27 16:01:15 2024, max compression
```

## Comparing `strax-1.6.3.tar` & `strax-1.6.4.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.442614 strax-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-30 23:08:22.000000 strax-1.6.3/CODE-OF-CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-30 23:08:22.000000 strax-1.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    26918 2024-04-30 23:08:22.000000 strax-1.6.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 23:08:22.000000 strax-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 23:08:22.000000 strax-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    29721 2024-04-30 23:08:24.442614 strax-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-30 23:08:22.000000 strax-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.430614 strax-1.6.3/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-30 23:08:22.000000 strax-1.6.3/bin/rechunker
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.430614 strax-1.6.3/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 23:08:22.000000 strax-1.6.3/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 23:08:22.000000 strax-1.6.3/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-30 23:08:22.000000 strax-1.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-30 23:08:24.442614 strax-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-30 23:08:22.000000 strax-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.434614 strax-1.6.3/strax/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-30 23:08:22.000000 strax-1.6.3/strax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 23:08:22.000000 strax-1.6.3/strax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-30 23:08:22.000000 strax-1.6.3/strax/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-30 23:08:22.000000 strax-1.6.3/strax/config.py
--rw-r--r--   0 runner    (1001) docker     (127)   100198 2024-04-30 23:08:22.000000 strax-1.6.3/strax/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-04-30 23:08:22.000000 strax-1.6.3/strax/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-30 23:08:22.000000 strax-1.6.3/strax/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-30 23:08:22.000000 strax-1.6.3/strax/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-04-30 23:08:22.000000 strax-1.6.3/strax/mailbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.434614 strax-1.6.3/strax/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/down_chunking_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/exhaust_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/loop_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/merge_only_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/overlap_window_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/parrallel_source_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-04-30 23:08:22.000000 strax-1.6.3/strax/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.438614 strax-1.6.3/strax/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/general.py
--rw-r--r--   0 runner    (1001) docker     (127)    22690 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/hitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_building.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-04-30 23:08:22.000000 strax-1.6.3/strax/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20586 2024-04-30 23:08:22.000000 strax-1.6.3/strax/run_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.438614 strax-1.6.3/strax/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/file_rechunker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-30 23:08:22.000000 strax-1.6.3/strax/storage/zipfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-04-30 23:08:22.000000 strax-1.6.3/strax/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27398 2024-04-30 23:08:22.000000 strax-1.6.3/strax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.434614 strax-1.6.3/strax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29721 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 23:08:24.000000 strax-1.6.3/strax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:24.442614 strax-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:08:22.000000 strax-1.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_child_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_down_chunk_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_exhaust_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_fixed_plugin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_general_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_get_zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_hitlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_inline_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_lone_hit_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_loop_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_mongo_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_multi_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_overlap_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15818 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_superruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-30 23:08:22.000000 strax-1.6.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.213220 strax-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-27 16:01:13.000000 strax-1.6.4/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-27 16:01:13.000000 strax-1.6.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27459 2024-05-27 16:01:13.000000 strax-1.6.4/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-27 16:01:13.000000 strax-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 16:01:13.000000 strax-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30262 2024-05-27 16:01:15.213220 strax-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-27 16:01:13.000000 strax-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.201220 strax-1.6.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-27 16:01:13.000000 strax-1.6.4/bin/rechunker
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.201220 strax-1.6.4/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 16:01:13.000000 strax-1.6.4/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 16:01:13.000000 strax-1.6.4/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 16:01:13.000000 strax-1.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 16:01:15.213220 strax-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-27 16:01:13.000000 strax-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.205220 strax-1.6.4/strax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-27 16:01:13.000000 strax-1.6.4/strax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-27 16:01:13.000000 strax-1.6.4/strax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-27 16:01:13.000000 strax-1.6.4/strax/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-05-27 16:01:13.000000 strax-1.6.4/strax/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104957 2024-05-27 16:01:13.000000 strax-1.6.4/strax/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-05-27 16:01:13.000000 strax-1.6.4/strax/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-05-27 16:01:13.000000 strax-1.6.4/strax/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-27 16:01:13.000000 strax-1.6.4/strax/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-05-27 16:01:13.000000 strax-1.6.4/strax/mailbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.205220 strax-1.6.4/strax/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/down_chunking_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/exhaust_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/loop_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/merge_only_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/overlap_window_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/parrallel_source_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-05-27 16:01:13.000000 strax-1.6.4/strax/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.209220 strax-1.6.4/strax/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18567 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22690 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/hitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/peak_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-05-27 16:01:13.000000 strax-1.6.4/strax/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-05-27 16:01:13.000000 strax-1.6.4/strax/run_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.209220 strax-1.6.4/strax/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:13.000000 strax-1.6.4/strax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27595 2024-05-27 16:01:13.000000 strax-1.6.4/strax/storage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-27 16:01:13.000000 strax-1.6.4/strax/storage/file_rechunker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-05-27 16:01:13.000000 strax-1.6.4/strax/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13716 2024-05-27 16:01:13.000000 strax-1.6.4/strax/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-27 16:01:13.000000 strax-1.6.4/strax/storage/zipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-05-27 16:01:13.000000 strax-1.6.4/strax/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27398 2024-05-27 16:01:13.000000 strax-1.6.4/strax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.205220 strax-1.6.4/strax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30262 2024-05-27 16:01:15.000000 strax-1.6.4/strax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-27 16:01:15.000000 strax-1.6.4/strax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:01:15.000000 strax-1.6.4/strax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:01:15.000000 strax-1.6.4/strax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-27 16:01:15.000000 strax-1.6.4/strax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 16:01:15.000000 strax-1.6.4/strax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:15.213220 strax-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:01:13.000000 strax-1.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_child_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_down_chunk_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_exhaust_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_fixed_plugin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_general_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_get_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_hitlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_hyperruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_inline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_lone_hit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_loop_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_mongo_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_multi_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_overlap_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_peak_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15818 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_superruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-27 16:01:13.000000 strax-1.6.4/tests/test_utils.py
```

### Comparing `strax-1.6.3/CODE-OF-CONDUCT.md` & `strax-1.6.4/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/CONTRIBUTING.md` & `strax-1.6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/HISTORY.md` & `strax-1.6.4/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+1.6.4 / 2024-05-27
+---------------------
+* Minor fix on `_is_superrun` variable  names by @dachengx in https://github.com/AxFoundation/strax/pull/837
+* Implement Hyperrun by @dachengx in https://github.com/AxFoundation/strax/pull/838
+* Add function to collect `data_type` and `data_kind` by @dachengx in https://github.com/AxFoundation/strax/pull/839
+* Check `include_tags` and `exclude_tags` by @dachengx in https://github.com/AxFoundation/strax/pull/841
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.3...v1.6.4
+
+
 1.6.3 / 2024-04-30
 ---------------------
 * Install `graphviz` for the pytests by @dachengx in https://github.com/AxFoundation/strax/pull/817
 * Increase the timing precision of progress bar by @dachengx in https://github.com/AxFoundation/strax/pull/819
 * Initialize plugin because `depends_on` can be property by @dachengx in https://github.com/AxFoundation/strax/pull/820
 * Update context.py by @WenzDaniel in https://github.com/AxFoundation/strax/pull/821
 * Disable tqdm progress bar when `check_available` is empty by @dachengx in https://github.com/AxFoundation/strax/pull/822
```

### Comparing `strax-1.6.3/LICENSE` & `strax-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/PKG-INFO` & `strax-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.6.3
+Version: 1.6.4
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: strax developers
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -36,14 +36,24 @@
 
 
 Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
 
 Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
 
 
+1.6.4 / 2024-05-27
+---------------------
+* Minor fix on `_is_superrun` variable  names by @dachengx in https://github.com/AxFoundation/strax/pull/837
+* Implement Hyperrun by @dachengx in https://github.com/AxFoundation/strax/pull/838
+* Add function to collect `data_type` and `data_kind` by @dachengx in https://github.com/AxFoundation/strax/pull/839
+* Check `include_tags` and `exclude_tags` by @dachengx in https://github.com/AxFoundation/strax/pull/841
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.3...v1.6.4
+
+
 1.6.3 / 2024-04-30
 ---------------------
 * Install `graphviz` for the pytests by @dachengx in https://github.com/AxFoundation/strax/pull/817
 * Increase the timing precision of progress bar by @dachengx in https://github.com/AxFoundation/strax/pull/819
 * Initialize plugin because `depends_on` can be property by @dachengx in https://github.com/AxFoundation/strax/pull/820
 * Update context.py by @WenzDaniel in https://github.com/AxFoundation/strax/pull/821
 * Disable tqdm progress bar when `check_available` is empty by @dachengx in https://github.com/AxFoundation/strax/pull/822
```

### Comparing `strax-1.6.3/README.md` & `strax-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/bin/rechunker` & `strax-1.6.4/bin/rechunker`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/setup.cfg` & `strax-1.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/setup.py` & `strax-1.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     readme = file.read()
 
 with open("HISTORY.md") as file:
     history = file.read()
 
 setuptools.setup(
     name="strax",
-    version="1.6.3",
+    version="1.6.4",
     description="Streaming analysis for xenon TPCs",
     author="strax developers",
     url="https://github.com/AxFoundation/strax",
     setup_requires=["pytest-runner"],
     install_requires=requires,
     tests_require=requires + tests_requires,
     long_description=readme + "\n\n" + history,
```

### Comparing `strax-1.6.3/strax/__init__.py` & `strax-1.6.4/strax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-__version__ = "1.6.3"
+__version__ = "1.6.4"
 
 # Glue the package together
 # See https://www.youtube.com/watch?v=0oTh1CXRaQ0 if this confuses you
 # The order of subpackes is not invariant, since we use strax.xxx inside strax
 from .utils import *
 from .chunk import *
 from .dtypes import *
```

### Comparing `strax-1.6.3/strax/chunk.py` & `strax-1.6.4/strax/chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             data_kind=data_kind,
             run_id=run_id,
             data=data,
             target_size_mb=max([c.target_size_mb for c in chunks]),
         )
 
     @classmethod
-    def concatenate(cls, chunks):
+    def concatenate(cls, chunks, allow_hyperrun=False):
         """Create chunk by concatenating chunks of same data type You can pass None's, they will be
         ignored."""
         chunks = [c for c in chunks if c is not None]
         if not chunks:
             raise ValueError("Need at least one chunk to concatenate")
         if len(chunks) == 1:
             return chunks[0]
@@ -257,15 +257,15 @@
         data_types = [c.data_type for c in chunks]
         if len(set(data_types)) != 1:
             raise ValueError(f"Cannot concatenate chunks of different data types: {data_types}")
         data_type = data_types[0]
 
         run_ids = [c.run_id for c in chunks]
 
-        if len(set(run_ids)) != 1:
+        if len(set(run_ids)) != 1 and not allow_hyperrun:
             raise ValueError(
                 f"Cannot concatenate {data_type} chunks with different run ids: {run_ids}"
             )
 
         run_id = run_ids[0]
         subruns = _update_subruns_in_chunk(chunks)
```

### Comparing `strax-1.6.3/strax/config.py` & `strax-1.6.4/strax/config.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/context.py` & `strax-1.6.4/strax/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -425,14 +425,32 @@
             for p_key in plugins_to_deregister:
                 self.log.info(f"Deregister {p_key}")
                 del self._plugin_class_registry[p_key]
 
             if not len(plugins_to_deregister):
                 registry_changed = False
 
+    def get_data_kinds(self) -> ty.Tuple:
+        """Return two dictionaries:
+        1. one with all available data_kind as key and their data_types(list) as values
+        2. one with all available data_type as key and their data_kind(str) as values
+        """
+        data_kind_collection: ty.Dict[str, ty.List] = dict()
+        data_type_collection: ty.Dict[str, str] = dict()
+        for data_type in self._plugin_class_registry.keys():
+            plugin = self.__get_plugin("0", data_type)
+            if isinstance(plugin.data_kind, (dict, immutabledict)):
+                data_kind = plugin.data_kind[data_type]
+            else:
+                data_kind = plugin.data_kind
+            data_kind_collection.setdefault(data_kind, [])
+            data_kind_collection[data_kind].append(data_type)
+            data_type_collection[data_type] = data_kind
+        return data_kind_collection, data_type_collection
+
     def search_field(
         self,
         pattern: str,
         include_code_usage: bool = True,
         return_matches: bool = False,
     ):
         """Find and print which plugin(s) provides a field that matches pattern (fnmatch).
@@ -622,22 +640,31 @@
 
         """
         plugin = self._get_plugins((data_name,), run_id)[data_name]
         self._set_plugin_config(plugin, run_id, tolerant=False)
         plugin.setup()
         return plugin
 
+    @staticmethod
+    def hyperrun_id(run_id):
+        if run_id.startswith("__"):
+            _run_id = run_id[2:]
+        else:
+            _run_id = run_id
+        return _run_id
+
     def _set_plugin_config(self, p, run_id, tolerant=True):
         # Explicit type check, since if someone calls this with
         # plugin CLASSES, funny business might ensue
+        _run_id = self.hyperrun_id(run_id)
         assert isinstance(p, strax.Plugin)
         config = self.config.copy()
         for opt in p.takes_config.values():
             try:
-                opt.validate(config, run_id=run_id, run_defaults=self.run_defaults(run_id))
+                opt.validate(config, run_id=_run_id, run_defaults=self.run_defaults(_run_id))
             except strax.InvalidConfiguration:
                 if not tolerant:
                     raise
 
         p.config = {k: v for k, v in config.items() if k in p.takes_config}
 
         if p.child_plugin:
@@ -727,15 +754,15 @@
         for target, plugin in cached_plugins.items():
             if target in requested_plugins:
                 # If e.g. target is already seen because the plugin is
                 # multi output
                 continue
 
             requested_p = plugin.__copy__()
-            requested_p.run_id = run_id
+            requested_p.run_id = self.hyperrun_id(run_id)
 
             # Re-use only one instance if the plugin is multi output
             for provides in strax.to_str_tuple(requested_p.provides):
                 requested_plugins[provides] = requested_p
 
         # Finally, fix the dtype.
         for plugin in requested_plugins.values():
@@ -797,15 +824,15 @@
             return target_plugin
 
         if data_type not in self._plugin_class_registry:
             raise KeyError(f"No plugin class registered that provides {data_type}")
 
         plugin = self._plugin_class_registry[data_type]()
 
-        plugin.run_id = run_id
+        plugin.run_id = self.hyperrun_id(run_id)
 
         # The plugin may not get all the required options here
         # but we don't know if we need the plugin yet
         self._set_plugin_config(plugin, run_id, tolerant=True)
 
         plugin.deps = {
             d_depends: self.__get_plugin(run_id, d_depends) for d_depends in plugin.depends_on
@@ -963,14 +990,15 @@
     def get_components(
         self,
         run_id: str,
         targets=tuple(),
         save=tuple(),
         time_range=None,
         chunk_number=None,
+        multi_run_progress_bar=False,
     ) -> strax.ProcessorComponents:
         """Return components for setting up a processor.
 
         {get_docs}
 
         """
         save = strax.to_str_tuple(save)
@@ -978,14 +1006,18 @@
 
         for t in targets:
             if len(t) == 1:
                 raise ValueError(f"Plugin names must be more than one letter, not {t}")
 
         plugins = self._get_plugins(targets, run_id)
 
+        allow_hyperruns = [plugins[target_i].allow_hyperrun for target_i in targets]
+        if sum(allow_hyperruns) != 0 and sum(allow_hyperruns) != len(targets):
+            raise ValueError("Cannot mix plugins that allow hyperruns with those that do not.")
+
         # Get savers/loaders, and meanwhile filter out plugins that do not
         # have to do computation. (their instances will stick around
         # though the .deps attribute of plugins that do)
         loaders = dict()
         loader_plugins = dict()
         savers: ty.Dict[str, strax.Saver] = dict()
         seen = set()
@@ -1003,25 +1035,34 @@
             loading_this_data = False
             key = self.key_for(run_id, target_i)
 
             loader = self._get_partial_loader_for(
                 key, chunk_number=chunk_number, time_range=time_range
             )
 
-            _is_superrun = run_id.startswith("_") and not target_plugin.provides[0].startswith(
-                "_temp"
-            )
-            if not loader and _is_superrun:
+            _is_temp = not target_plugin.provides[0].startswith("_temp")
+            _is_superrun = run_id.startswith("_") and _is_temp
+            _is_hyperrun = run_id.startswith("__") and _is_temp
+            # hyperrun is always superrun
+            allow_hyperrun = plugins[target_i].allow_hyperrun
+            if not loader and (
+                (_is_superrun and not _is_hyperrun) or (_is_hyperrun and not allow_hyperrun)
+            ):
                 if time_range is not None:
                     raise NotImplementedError("time range loading not yet supported for superruns")
 
                 sub_run_spec = self.run_metadata(run_id, "sub_run_spec")["sub_run_spec"]
 
                 # Make subruns if they do not exist.
-                self.make(list(sub_run_spec.keys()), target_i, save=(target_i,))
+                self.make(
+                    list(sub_run_spec.keys()),
+                    target_i,
+                    save=(target_i,),
+                    multi_run_progress_bar=multi_run_progress_bar,
+                )
 
                 ldrs = []
                 for subrun in sub_run_spec:
                     sub_key = self.key_for(subrun, target_i)
 
                     if sub_run_spec[subrun] == "all":
                         _subrun_time_range = None
@@ -1106,20 +1147,25 @@
 
             # Now we should check whether we meet the saving requirements (Explicit, Target etc.)
             # In case of the storage converter mode we copy already existing data. So we do not
             # have to check for the saving requirements here.
             current_plugin_to_savers = [target_i]
             if (
                 not self._target_should_be_saved(
-                    target_plugin, target_i, targets, save, loader, _is_superrun
+                    target_plugin,
+                    target_i,
+                    targets,
+                    save,
+                    loader,
+                    _is_superrun and not _is_hyperrun,
                 )
                 and not self.context_config["storage_converter"]
             ):
                 if len(target_plugin.provides) > 1:
-                    # In case the plugin has more then a single provides we also have to check
+                    # In case the plugin has more than a single provides we also have to check
                     # whether any of the other data_types should be stored. Hence only remove
                     # the current traget from the list of plugins_to_savers.
                     current_plugin_to_savers = []
                 else:
                     # In case of a single-provide plugin we can return now.
                     return
 
@@ -1138,40 +1184,48 @@
                 self.log.warning(f"Not saving {target_i} while fuzzy matching is turned on.")
                 return
             if self.context_config["allow_incomplete"]:
                 self.log.warning(f"Not saving {target_i} while loading incomplete data is allowed.")
                 return
 
             # Save the target and any other outputs of the plugin.
-            if _is_superrun:
+            if _is_superrun and not _is_hyperrun:
                 # In case of a superrun we are only interested in the specified targets
                 # and not any other stuff provided by the corresponding plugin.
                 savers = self._add_saver(
-                    savers, target_i, target_plugin, _is_superrun, loading_this_data
+                    savers, target_i, run_id, target_plugin, _is_superrun, loading_this_data
                 )
-            else:
+            elif not _is_hyperrun or allow_hyperrun:
+                # only save if we are not in a hyperrun or the plugin allows hyperruns
+                # otherwise we will see error at Chunk.concatenate
+                # but anyway the data is should already been made
                 for d_to_save in set(current_plugin_to_savers + list(target_plugin.provides)):
                     key = self.key_for(run_id, d_to_save)
                     loader = self._get_partial_loader_for(
                         key, time_range=time_range, chunk_number=chunk_number
                     )
 
                     if (
                         not self._target_should_be_saved(
-                            target_plugin, d_to_save, targets, save, loader, _is_superrun
+                            target_plugin,
+                            d_to_save,
+                            targets,
+                            save,
+                            loader,
+                            _is_superrun and not _is_hyperrun,
                         )
                         and not self.context_config["storage_converter"]
                     ) or savers.get(d_to_save):
                         # This multi-output plugin was scanned before
                         # let's not create doubled savers or store data_types we do not want to.
                         assert target_plugin.multi_output
                         continue
 
                     savers = self._add_saver(
-                        savers, d_to_save, target_plugin, _is_superrun, loading_this_data
+                        savers, d_to_save, run_id, target_plugin, _is_superrun, loading_this_data
                     )
 
         for target_i in targets:
             check_cache(target_i)
         plugins = to_compute
 
         intersec = list(plugins.keys() & loaders.keys())
@@ -1200,14 +1254,15 @@
             targets=strax.to_str_tuple(final_plugin),
         )
 
     def _add_saver(
         self,
         savers: dict,
         d_to_save: str,
+        run_id,
         target_plugin: strax.Plugin,
         _is_superrun: bool,
         loading_this_data: bool,
     ):
         """Adds savers to already existing savers. Checks if data_type can be stored in any storage
         frontend.
 
@@ -1216,15 +1271,15 @@
         :param target_plugin: Plugin which produces the data_type
         :param _is_superrun: Boolean if run is a superrun
         :param loading_this_data: Boolean if data can be loaded. Required for storing during
             storage_converter mode and writing of superruns.
         :return: Updated savers dictionary.
 
         """
-        key = strax.DataKey(target_plugin.run_id, d_to_save, target_plugin.lineage)
+        key = strax.DataKey(run_id, d_to_save, target_plugin.lineage)
         for sf in self._sorted_storage:
             if sf.readonly:
                 continue
             if loading_this_data:
                 # Usually, we don't save if we're loading
                 if not self.context_config["storage_converter"] and (
                     not self.context_config["write_superruns"] and _is_superrun
@@ -1240,15 +1295,15 @@
                 except strax.DataNotAvailable:
                     # Don't have it, so let's save it!
                     pass
             # If we get here, we must try to save
             try:
                 saver = sf.saver(
                     key,
-                    metadata=target_plugin.metadata(target_plugin.run_id, d_to_save),
+                    metadata=target_plugin.metadata(run_id, d_to_save),
                     saver_timeout=self.context_config["saver_timeout"],
                 )
                 # Now that we are surely saving, make an entry in savers
                 savers.setdefault(d_to_save, [])
                 savers[d_to_save].append(saver)
             except strax.DataNotAvailable:
                 # This frontend cannot save. Too bad.
@@ -1388,14 +1443,15 @@
         time_selection="fully_contained",
         selection=None,
         selection_str=None,
         keep_columns=None,
         drop_columns=None,
         allow_multiple=False,
         progress_bar=True,
+        multi_run_progress_bar=True,
         _chunk_number=None,
         **kwargs,
     ) -> ty.Iterator[strax.Chunk]:
         """Compute target for run_id and iterate over results.
 
         Do NOT interrupt the iterator (i.e. break): it will keep running stuff
         in background threads...
@@ -1443,15 +1499,20 @@
             ):
                 # For allow_multiple we don't want allow this when in lazy mode
                 # with long timeouts (lazy-mode is disabled if multiprocessing
                 # so if that is activated, we can also continue)
                 raise RuntimeError(f"Cannot allow_multiple in lazy mode or with long timeouts.")
 
         components = self.get_components(
-            run_id, targets=targets, save=save, time_range=time_range, chunk_number=_chunk_number
+            run_id,
+            targets=targets,
+            save=save,
+            time_range=time_range,
+            chunk_number=_chunk_number,
+            multi_run_progress_bar=multi_run_progress_bar,
         )
 
         # Cleanup the temp plugins
         for k in list(self._plugin_class_registry.keys()):
             if k.startswith("_temp"):
                 del self._plugin_class_registry[k]
 
@@ -1606,15 +1667,15 @@
                 throw_away_result=True,
                 log=self.log,
                 save=save,
                 max_workers=max_workers,
                 **kwargs,
             )
 
-        if _skip_if_built and self.is_stored(run_id, targets):
+        if _skip_if_built and self.is_stored(run_ids[0], targets):
             return
 
         for _ in self.get_iter(run_ids[0], targets, save=save, max_workers=max_workers, **kwargs):
             pass
 
     def get_array(
         self, run_id: ty.Union[str, tuple, list], targets, save=tuple(), max_workers=None, **kwargs
@@ -2396,14 +2457,65 @@
         )
 
         return {
             data_type: dict(hash=_hash, save_when=save_when.name, version=version)
             for data_type, _hash, save_when, version in hashes
         }
 
+    @property
+    def root_data_types(self):
+        """Root data_type that does not depend on anything."""
+        _root_data_types = set()
+        for k, v in self._plugin_class_registry.items():
+            if not v.depends_on:
+                _root_data_types |= set((k,))
+        return _root_data_types
+
+    @property
+    def inverse_tree(self):
+        """Inverse tree whose key is depends_on and value is provides."""
+        _inverse_tree = dict()
+        for k, v in self._plugin_class_registry.items():
+            for d in v().depends_on:
+                _inverse_tree.setdefault(d, [])
+                _inverse_tree[d] += v().provides
+        return _inverse_tree
+
+    def check_hyperrun(self):
+        """Raise if non-hyperrun plugins depends on hyperrun plugins."""
+        inverse_tree = self.inverse_tree
+
+        # define a recursive function to check if all the dependencies support hyperruns
+        def check_support_hyperrun(data_type, checked=set(), seen_allow=None):
+            if data_type in checked:
+                return checked
+            if self._plugin_class_registry[data_type].allow_hyperrun:
+                seen_allow = data_type
+            if seen_allow and not self._plugin_class_registry[data_type].allow_hyperrun:
+                raise ValueError(
+                    f"Already support hyperruns in {seen_allow}, "
+                    f"but it's dependency {data_type} does not support hyperruns."
+                )
+            checked |= set((data_type,))
+            if data_type not in inverse_tree:
+                return checked
+            for d in inverse_tree[data_type]:
+                checked |= check_support_hyperrun(d, checked, seen_allow)
+            return checked
+
+        # use checked set to record the data_type that has been checked
+        # to shorten the time of checking
+        checked = set()
+        for data_type in self.root_data_types:
+            if self._plugin_class_registry[data_type].allow_hyperrun:
+                seen_allow = data_type
+            else:
+                seen_allow = None
+            checked |= check_support_hyperrun(data_type, checked, seen_allow)
+
     @classmethod
     def add_method(cls, f):
         """Add f as a new Context method."""
         setattr(cls, f.__name__, f)
 
 
 select_docs = """
```

### Comparing `strax-1.6.3/strax/corrections.py` & `strax-1.6.4/strax/corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/dtypes.py` & `strax-1.6.4/strax/dtypes.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/io.py` & `strax-1.6.4/strax/io.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/mailbox.py` & `strax-1.6.4/strax/mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/plugins/cut_plugin.py` & `strax-1.6.4/strax/plugins/cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/plugins/down_chunking_plugin.py` & `strax-1.6.4/strax/plugins/down_chunking_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/plugins/exhaust_plugin.py` & `strax-1.6.4/strax/plugins/exhaust_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/plugins/loop_plugin.py` & `strax-1.6.4/strax/plugins/loop_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/plugins/merge_only_plugin.py` & `strax-1.6.4/strax/plugins/merge_only_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/plugins/overlap_window_plugin.py` & `strax-1.6.4/strax/plugins/overlap_window_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
     def do_compute(self, chunk_i=None, **kwargs):
         if not len(kwargs):
             raise RuntimeError("OverlapWindowPlugin must have a dependency")
 
         # Add cached inputs to compute arguments
         for data_kind, chunk in kwargs.items():
             if len(self.cached_input):
-                kwargs[data_kind] = strax.Chunk.concatenate([self.cached_input[data_kind], chunk])
+                kwargs[data_kind] = strax.Chunk.concatenate(
+                    [self.cached_input[data_kind], chunk], self.allow_hyperrun
+                )
 
         # Compute new results
         result = super().do_compute(chunk_i=chunk_i, **kwargs)
 
         # Throw away results we already sent out
         _, result = result.split(t=self.sent_until, allow_early_split=False)
```

### Comparing `strax-1.6.3/strax/plugins/parrallel_source_plugin.py` & `strax-1.6.4/strax/plugins/parrallel_source_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/plugins/plugin.py` & `strax-1.6.4/strax/plugins/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,16 @@
     run_i: int
     config: typing.Dict
     deps: typing.Dict  # Dictionary of dependency plugin instances
 
     compute_takes_chunk_i = False  # Autoinferred, no need to set yourself
     compute_takes_start_end = False
 
+    allow_hyperrun = False
+
     def __init__(self):
         if not hasattr(self, "depends_on"):
             raise ValueError(f"depends_on not provided for {self.__class__.__name__}")
 
         self.depends_on = strax.to_str_tuple(self.depends_on)
 
         # Store compute parameter names, see if we take chunk_i too
@@ -372,15 +374,17 @@
         :param iters: iterators that produce data
         :param check_end_not_before: Raise a runtimeError if the source is exhausted, but the input
             buffer ends before this time.
 
         """
         try:
             # print(f"Fetching {d} in {self}, hope to see {hope_to_see}")
-            self.input_buffer[d] = strax.Chunk.concatenate([self.input_buffer[d], next(iters[d])])
+            self.input_buffer[d] = strax.Chunk.concatenate(
+                [self.input_buffer[d], next(iters[d])], self.allow_hyperrun
+            )
             # print(f"Fetched {d} in {self}, "
             #      f"now have {self.input_buffer[d]}")
             return True
         except StopIteration:
             # print(f"Got StopIteration while fetching for {d} in {self}")
             if check_end_not_before is not None and self.input_buffer[d].end < check_end_not_before:
                 raise RuntimeError(
@@ -473,15 +477,16 @@
                         if len(set([x.end for x in inputs.values()])) <= 1:
                             break
                         for d in self.depends_on:
                             inputs[d], back_to_buffer = inputs[d].split(
                                 t=this_chunk_end, allow_early_split=True
                             )
                             self.input_buffer[d] = strax.Chunk.concatenate(
-                                [back_to_buffer, self.input_buffer[d]]
+                                [back_to_buffer, self.input_buffer[d]],
+                                self.allow_hyperrun,
                             )
                         max_passes_left -= 1
                     else:
                         raise RuntimeError(
                             f"{self} was unable to get time-consistent "
                             f"inputs after ten passess. Inputs: \n{inputs}\n"
                             f"Input buffer:\n{self.input_buffer}"
```

### Comparing `strax-1.6.3/strax/processing/data_reduction.py` & `strax-1.6.4/strax/processing/data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/general.py` & `strax-1.6.4/strax/processing/general.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/hitlets.py` & `strax-1.6.4/strax/processing/hitlets.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/peak_building.py` & `strax-1.6.4/strax/processing/peak_building.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/peak_merging.py` & `strax-1.6.4/strax/processing/peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/peak_properties.py` & `strax-1.6.4/strax/processing/peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/peak_splitting.py` & `strax-1.6.4/strax/processing/peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/pulse_processing.py` & `strax-1.6.4/strax/processing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processing/statistics.py` & `strax-1.6.4/strax/processing/statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/processor.py` & `strax-1.6.4/strax/processor.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/run_selection.py` & `strax-1.6.4/strax/run_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -520,17 +520,21 @@
     dsets,
     include_tags,
     exclude_tags,
     pattern_type,
     ignore_underscore,
 ):
     if include_tags is not None:
+        if not isinstance(include_tags, (str, list, tuple)):
+            raise ValueError("include_tags must be a str, list or tuple")
         dsets = dsets[_tags_match(dsets, include_tags, pattern_type, ignore_underscore)]
 
     if exclude_tags is not None:
+        if not isinstance(exclude_tags, (str, list, tuple)):
+            raise ValueError("exclude_tags must be a str, list or tuple")
         dsets = dsets[True ^ _tags_match(dsets, exclude_tags, pattern_type, ignore_underscore)]
     return dsets
 
 
 def _tags_match(dsets, patterns, pattern_type, ignore_underscore):
     result = np.zeros(len(dsets), dtype=np.bool_)
```

### Comparing `strax-1.6.3/strax/storage/common.py` & `strax-1.6.4/strax/storage/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,17 @@
             fuzzy_for=fuzzy_for,
             fuzzy_for_options=fuzzy_for_options,
         )
         return self._get_backend(backend).get_metadata(backend_key)
 
     def _we_take(self, data_type):
         """Return if data_type can be provided by this frontend."""
-        return not (data_type in self.exclude or self.take_only and data_type not in self.take_only)
+        return not (
+            data_type in self.exclude or (self.take_only and data_type not in self.take_only)
+        )
 
     def _support_superruns(self, run_id):
         """Checks if run is a superrun and if superruns are provided by frontend."""
         is_superrun = run_id.startswith("_")
         if is_superrun:
             return self.provide_superruns
         else:
@@ -630,34 +632,34 @@
     def save_from(self, source: typing.Generator, rechunk=True, executor=None):
         """Iterate over source and save the results under key along with metadata."""
         pending: List = []
         exhausted = False
         chunk_i = 0
 
         run_id = self.md["run_id"]
-        _is_super_run = run_id.startswith("_")
+        _is_superrun = run_id.startswith("_") and not run_id.startswith("__")
         try:
             while not exhausted:
                 chunk = None
 
                 try:
                     if rechunk and self.allow_rechunk:
                         while chunk is None or chunk.data.nbytes < chunk.target_size_mb * 1e6:
                             next_chunk = next(source)
 
-                            if _is_super_run:
+                            if _is_superrun:
                                 # If we are creating a superrun, we load data from subruns
                                 # and the loaded subrun chunk becomes a superun chunk:
                                 next_chunk = strax.transform_chunk_to_superrun_chunk(
                                     run_id, next_chunk
                                 )
                             chunk = strax.Chunk.concatenate([chunk, next_chunk])
                     else:
                         chunk = next(source)
-                        if _is_super_run:
+                        if _is_superrun:
                             # If we are creating a superrun, we load data from subruns
                             # and the loaded subrun chunk becomes a superun chunk:
                             chunk = strax.transform_chunk_to_superrun_chunk(run_id, chunk)
 
                 except StopIteration:
                     exhausted = True
```

### Comparing `strax-1.6.3/strax/storage/file_rechunker.py` & `strax-1.6.4/strax/storage/file_rechunker.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/storage/files.py` & `strax-1.6.4/strax/storage/files.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/storage/mongo.py` & `strax-1.6.4/strax/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/storage/zipfiles.py` & `strax-1.6.4/strax/storage/zipfiles.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/testutils.py` & `strax-1.6.4/strax/testutils.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax/utils.py` & `strax-1.6.4/strax/utils.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/strax.egg-info/PKG-INFO` & `strax-1.6.4/strax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.6.3
+Version: 1.6.4
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: strax developers
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -36,14 +36,24 @@
 
 
 Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
 
 Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
 
 
+1.6.4 / 2024-05-27
+---------------------
+* Minor fix on `_is_superrun` variable  names by @dachengx in https://github.com/AxFoundation/strax/pull/837
+* Implement Hyperrun by @dachengx in https://github.com/AxFoundation/strax/pull/838
+* Add function to collect `data_type` and `data_kind` by @dachengx in https://github.com/AxFoundation/strax/pull/839
+* Check `include_tags` and `exclude_tags` by @dachengx in https://github.com/AxFoundation/strax/pull/841
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.6.3...v1.6.4
+
+
 1.6.3 / 2024-04-30
 ---------------------
 * Install `graphviz` for the pytests by @dachengx in https://github.com/AxFoundation/strax/pull/817
 * Increase the timing precision of progress bar by @dachengx in https://github.com/AxFoundation/strax/pull/819
 * Initialize plugin because `depends_on` can be property by @dachengx in https://github.com/AxFoundation/strax/pull/820
 * Update context.py by @WenzDaniel in https://github.com/AxFoundation/strax/pull/821
 * Disable tqdm progress bar when `check_available` is empty by @dachengx in https://github.com/AxFoundation/strax/pull/822
```

### Comparing `strax-1.6.3/strax.egg-info/SOURCES.txt` & `strax-1.6.4/strax.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 tests/test_down_chunk_plugin.py
 tests/test_exhaust_plugin.py
 tests/test_fixed_plugin_cache.py
 tests/test_general_processing.py
 tests/test_get_zarr.py
 tests/test_helpers.py
 tests/test_hitlet.py
+tests/test_hyperruns.py
 tests/test_inline_plugin.py
 tests/test_lone_hit_integration.py
 tests/test_loop_plugins.py
 tests/test_mailbox.py
 tests/test_mongo_frontend.py
 tests/test_multi_output.py
 tests/test_overlap_plugin.py
```

### Comparing `strax-1.6.3/tests/test_child_plugins.py` & `strax-1.6.4/tests/test_child_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_config.py` & `strax-1.6.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_context.py` & `strax-1.6.4/tests/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -495,7 +495,24 @@
         st.make(run_id, "records")
         old_metadata = st.get_metadata(run_id, "records")
         comparison_dict = st.compare_metadata(
             (run_id, "records"), old_metadata, return_results=True
         )
         comparison_dict["metadata2"].pop("strax_version")
         assert comparison_dict["metadata2"] == old_metadata, "metadata comparison failed"
+
+    def test_get_data_kinds(self):
+        st = self.get_context(True)
+        st.register(Records)
+        st.register(Peaks)
+        st.register(self.get_dummy_peaks_dependency())
+        data_kind_collection, data_type_collection = st.get_data_kinds()
+        # Assert the expected data kinds and their corresponding data types
+        expected_data_kind_collection = {"records": ["records"], "peaks": ["peaks", "cut_peaks"]}
+        assert data_kind_collection == expected_data_kind_collection
+        # Assert the expected data types and their corresponding data kinds
+        expected_data_type_collection = {
+            "records": "records",
+            "peaks": "peaks",
+            "cut_peaks": "peaks",
+        }
+        assert data_type_collection == expected_data_type_collection
```

### Comparing `strax-1.6.3/tests/test_core.py` & `strax-1.6.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_corrections.py` & `strax-1.6.4/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_cut_plugin.py` & `strax-1.6.4/tests/test_cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_data_reduction.py` & `strax-1.6.4/tests/test_data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_down_chunk_plugin.py` & `strax-1.6.4/tests/test_down_chunk_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_exhaust_plugin.py` & `strax-1.6.4/tests/test_exhaust_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_fixed_plugin_cache.py` & `strax-1.6.4/tests/test_fixed_plugin_cache.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_general_processing.py` & `strax-1.6.4/tests/test_general_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_get_zarr.py` & `strax-1.6.4/tests/test_get_zarr.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_helpers.py` & `strax-1.6.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_hitlet.py` & `strax-1.6.4/tests/test_hitlet.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_inline_plugin.py` & `strax-1.6.4/tests/test_inline_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_lone_hit_integration.py` & `strax-1.6.4/tests/test_lone_hit_integration.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_loop_plugins.py` & `strax-1.6.4/tests/test_loop_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_mailbox.py` & `strax-1.6.4/tests/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_mongo_frontend.py` & `strax-1.6.4/tests/test_mongo_frontend.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_multi_output.py` & `strax-1.6.4/tests/test_multi_output.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_overlap_plugin.py` & `strax-1.6.4/tests/test_overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_peak_merging.py` & `strax-1.6.4/tests/test_peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_peak_processing.py` & `strax-1.6.4/tests/test_peak_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_peak_properties.py` & `strax-1.6.4/tests/test_peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_peak_splitting.py` & `strax-1.6.4/tests/test_peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_pulse_processing.py` & `strax-1.6.4/tests/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_saving.py` & `strax-1.6.4/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_statistics.py` & `strax-1.6.4/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_storage.py` & `strax-1.6.4/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_superruns.py` & `strax-1.6.4/tests/test_superruns.py`

 * *Files identical despite different names*

### Comparing `strax-1.6.3/tests/test_utils.py` & `strax-1.6.4/tests/test_utils.py`

 * *Files identical despite different names*

