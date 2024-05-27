# Comparing `tmp/dcnum-0.19.1.tar.gz` & `tmp/dcnum-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.19.1.tar", last modified: Mon May 20 22:19:07 2024, max compression
+gzip compressed data, was "dcnum-0.20.0.tar", last modified: Mon May 27 12:51:47 2024, max compression
```

## Comparing `dcnum-0.19.1.tar` & `dcnum-0.20.0.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.297881 dcnum-0.19.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.273881 dcnum-0.19.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.277881 dcnum-0.19.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-20 22:19:04.000000 dcnum-0.19.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-20 22:19:04.000000 dcnum-0.19.1/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-20 22:19:04.000000 dcnum-0.19.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-20 22:19:04.000000 dcnum-0.19.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-05-20 22:19:04.000000 dcnum-0.19.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 22:19:04.000000 dcnum-0.19.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-20 22:19:07.297881 dcnum-0.19.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-20 22:19:04.000000 dcnum-0.19.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.277881 dcnum-0.19.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-20 22:19:04.000000 dcnum-0.19.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.277881 dcnum-0.19.1/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-20 22:19:04.000000 dcnum-0.19.1/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-20 22:19:04.000000 dcnum-0.19.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 22:19:04.000000 dcnum-0.19.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-20 22:19:04.000000 dcnum-0.19.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:19:07.297881 dcnum-0.19.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.273881 dcnum-0.19.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.277881 dcnum-0.19.1/src/dcnum/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 22:19:07.000000 dcnum-0.19.1/src/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.281881 dcnum-0.19.1/src/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.281881 dcnum-0.19.1/src/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_background/bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13173 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)    20705 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.281881 dcnum-0.19.1/src/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.281881 dcnum-0.19.1/src/dcnum/feat/feat_contour/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_contour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_contour/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_contour/moments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_contour/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.281881 dcnum-0.19.1/src/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.285881 dcnum-0.19.1/src/dcnum/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27956 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/logic/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/logic/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/logic/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.285881 dcnum-0.19.1/src/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/meta/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.285881 dcnum-0.19.1/src/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/read/hdf5_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/read/mapped.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.285881 dcnum-0.19.1/src/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.285881 dcnum-0.19.1/src/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-20 22:19:04.000000 dcnum-0.19.1/src/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.293881 dcnum-0.19.1/src/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-20 22:19:07.000000 dcnum-0.19.1/src/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-20 22:19:07.000000 dcnum-0.19.1/src/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:19:07.000000 dcnum-0.19.1/src/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 22:19:07.000000 dcnum-0.19.1/src/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 22:19:07.000000 dcnum-0.19.1/src/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.293881 dcnum-0.19.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:19:07.293881 dcnum-0.19.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
--rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/data/fmt-hdf5_shapein_empty.zip
--rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_background_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_background_bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_background_bg_sparsemed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_event_extractor_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_moments_based_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_feat_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_logic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_logic_join.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_logic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    33551 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_logic_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_meta_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_meta_ppid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_meta_ppid_bg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_meta_ppid_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_meta_ppid_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_meta_ppid_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_meta_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_read_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_read_hdf5_index_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_segm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_segm_no_mask_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_write_queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-20 22:19:04.000000 dcnum-0.19.1/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.634594 dcnum-0.20.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.614594 dcnum-0.20.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.614594 dcnum-0.20.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-27 12:51:42.000000 dcnum-0.20.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-27 12:51:42.000000 dcnum-0.20.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-27 12:51:42.000000 dcnum-0.20.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-27 12:51:42.000000 dcnum-0.20.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-27 12:51:42.000000 dcnum-0.20.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-27 12:51:42.000000 dcnum-0.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-27 12:51:47.634594 dcnum-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-27 12:51:42.000000 dcnum-0.20.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-27 12:51:42.000000 dcnum-0.20.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:51:47.634594 dcnum-0.20.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.614594 dcnum-0.20.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/feat/feat_contour/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34405 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/meta/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/mapped.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.626594 dcnum-0.20.0/src/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.634594 dcnum-0.20.0/src/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.630594 dcnum-0.20.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.634594 dcnum-0.20.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_shapein_empty.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_bg_sparsemed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_event_extractor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_moments_based_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35480 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_hdf5_basins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_hdf5_index_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_segm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_segm_no_mask_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_write_queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_write_writer.py
```

### Comparing `dcnum-0.19.1/.github/workflows/check.yml` & `dcnum-0.20.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/.github/workflows/deploy_pypi.yml` & `dcnum-0.20.0/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/.gitignore` & `dcnum-0.20.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/CHANGELOG` & `dcnum-0.20.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.20.0
+ - feat: support reading mapped basins
+ - feat: support writing mapped-basin-based output files
+ - fix: copy "bg_off" data to output file when copying background data
+ - enh: allow to slice BaseImageChunkCache
+ - enh: sort logs, tables and basins for reproducible access
+ - enh: add more timing information in logs
+ - ref: background progress value is now a double between 0 and 1
 0.19.1
  - enh: support steps when specifying data slices in `index_mapping`
 0.19.0
  - enh: elevate `HDF5Data`s `index_mapping` to pipeline identifier status
    (this changes the pipeline identifier)
  - enh: improve sanity checks for `BackgroundRollMed`
 0.18.0
```

### Comparing `dcnum-0.19.1/LICENSE` & `dcnum-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/PKG-INFO` & `dcnum-0.20.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.19.1
+Version: 0.20.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.19.1/README.rst` & `dcnum-0.20.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/docs/conf.py` & `dcnum-0.20.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/docs/extensions/github_changelog.py` & `dcnum-0.20.0/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/pyproject.toml` & `dcnum-0.20.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.20.0/src/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_background/base.py` & `dcnum-0.20.0/src/dcnum/feat/feat_background/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         if num_cpus is None:
             num_cpus = mp_spawn.cpu_count()
         #: number of CPUs used
         self.num_cpus = num_cpus
 
         #: number of images in the input data
         self.image_count = None
-        #: number of images that have been processed
-        self.image_proc = mp_spawn.Value("L", 0)
+        #: fraction images that have been processed
+        self.image_proc = mp_spawn.Value("d", 0)
 
         #: HDF5Data instance for input data
         self.hdin = None
         #: input h5py.File
         self.h5in = None
         #: output h5py.File
         self.h5out = None
@@ -181,15 +181,15 @@
         return kwargs
 
     def get_progress(self):
         """Return progress of background computation, float in [0,1]"""
         if self.image_count == 0:
             return 0.
         else:
-            return self.image_proc.value / self.image_count
+            return self.image_proc.value
 
     def process(self):
         # Delete any old background data
         for key in ["image_bg", "bg_off"]:
             if key in self.h5out["events"]:
                 del self.h5out["events"][key]
         # Perform the actual background computation
```

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_background/bg_copy.py` & `dcnum-0.20.0/src/dcnum/feat/feat_background/bg_copy.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 class BackgroundCopy(Background):
     @staticmethod
     def check_user_kwargs():
         pass
 
     def process(self):
-        """Perform median computation on entire input data"""
+        """Copy input data to output dataset"""
         if self.h5in != self.h5out:
-            hin = self.hdin.image_bg.h5ds
-            h5py.h5o.copy(src_loc=hin.parent.id,
-                          src_name=b"image_bg",
-                          dst_loc=self.h5out["events"].id,
-                          dst_name=b"image_bg",
-                          )
+            hin = self.hdin.h5
+            for feat in ["image_bg", "bg_off"]:
+                if feat in hin["events"]:
+                    h5py.h5o.copy(src_loc=hin["events"].id,
+                                  src_name=feat.encode("utf-8"),
+                                  dst_loc=self.h5out["events"].id,
+                                  dst_name=feat.encode("utf-8"),
+                                  )
 
         # set progress to 100%
-        self.image_proc.value = self.image_count
+        self.image_proc.value = 1
 
     def process_approach(self):
         # We do the copying in `process`, because we do not want to modify
         # any metadata or delete datasets as is done in the base class.
         # But we still have to implement this method, because it is an
         # abstractmethod in the base class.
         pass
```

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.20.0/src/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         if num_remaining:
             last_image = self.h5out["events/image_bg"][-1]
             last_chunk = np.repeat(
                 last_image[np.newaxis],
                 num_remaining,
                 axis=0)
             self.writer.store_feature_chunk("image_bg", last_chunk)
-            self.image_proc.value += num_remaining
+        self.image_proc.value = 1
 
     def process_next_batch(self):
         """Process one batch of input data"""
         cur_slice_in, cur_slice_out, output_size = \
             self.get_slices_for_batch(self.current_batch)
 
         if output_size:
@@ -219,15 +219,15 @@
             self.writer.store_feature_chunk(
                 "image_bg",
                 self.shared_output[:output_size].reshape(output_size,
                                                          *self.image_shape),
             )
 
         self.current_batch += 1
-        self.image_proc.value += self.batch_size
+        self.image_proc.value += self.batch_size / self.image_count
 
 
 class WorkerRollMed(mp_spawn.Process):
     def __init__(self, job_queue, counter, shared_input, shared_output,
                  batch_size, kernel_size, *args, **kwargs):
         """Worker process for median computation"""
         super(WorkerRollMed, self).__init__(*args, **kwargs)
```

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.20.0/src/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
             idx1 = np.argmin(np.abs(self.time - t1 + self.split_time/2))
             bg_idx[idx0:idx1] = ii
             idx0 = idx1
         if idx1 is not None:
             # Fill up remainder of index array with last entry
             bg_idx[idx1:] = ii
 
-        self.image_proc.value = self.image_count
+        self.image_proc.value = 1
 
         # Write background data
         pos = 0
         step = 1000
         while pos < self.image_count:
             stop = min(pos + step, self.image_count)
             cur_slice = slice(pos, stop)
@@ -389,15 +389,15 @@
         while True:
             time.sleep(.01)
             if self.worker_counter.value == num_jobs:
                 break
 
         self.bg_images[ii] = self.shared_output.reshape(self.image_shape)
 
-        self.image_proc.value = idx_stop
+        self.image_proc.value = idx_stop / self.image_count
 
 
 class WorkerSparseMed(mp_spawn.Process):
     def __init__(self, job_queue, counter, shared_input, shared_output,
                  kernel_size, *args, **kwargs):
         """Worker process for median computation"""
         super(WorkerSparseMed, self).__init__(*args, **kwargs)
```

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.20.0/src/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_contour/moments.py` & `dcnum-0.20.0/src/dcnum/feat/feat_contour/moments.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_contour/volume.py` & `dcnum-0.20.0/src/dcnum/feat/feat_contour/volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.20.0/src/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/feat/gate.py` & `dcnum-0.20.0/src/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/feat/queue_event_extractor.py` & `dcnum-0.20.0/src/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/logic/ctrl.py` & `dcnum-0.20.0/src/dcnum/logic/ctrl.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 import socket
 import threading
 import time
 import traceback
 import uuid
 
 import h5py
+import numpy as np
 
 from ..feat.feat_background.base import get_available_background_methods
 from ..feat.queue_event_extractor import QueueEventExtractor
 from ..feat import gate
 from ..feat import EventExtractorManagerThread
 from ..segm import SegmenterManagerThread, get_available_segmenters
 from ..meta import ppid
-from ..read import HDF5Data
-from .._version import version_tuple
+from ..read import HDF5Data, get_mapping_indices
+from .._version import version, version_tuple
 from ..write import (
-    DequeWriterThread, HDF5Writer, QueueCollectorThread,
+    DequeWriterThread, HDF5Writer, QueueCollectorThread, copy_features,
     copy_metadata, create_with_basins, set_default_filter_kwargs
 )
 
 from .job import DCNumPipelineJob
 from .json_encoder import ExtendedJSONEncoder
 
 # Force using "spawn" method for multiprocessing, because we are using
@@ -39,14 +40,15 @@
 #: not in alphabetical order.
 valid_states = [
     "created",
     "init",
     "setup",
     "background",
     "segmentation",
+    "plumbing",
     "cleanup",
     "done",
     "error",
 ]
 
 
 class DCNumJobRunner(threading.Thread):
@@ -75,16 +77,17 @@
         self.event_count = 0
 
         self._data_raw = None
         self._data_temp_in = None
         # current job state
         self._state = "init"
         # overall progress [0, 1]
-        self._progress_bg = None
-        self._progress_ex = None
+        self._progress_bg = None  # background
+        self._progress_ex = None  # segmentation
+        self._progress_bn = None  # creating basins
         # segmentation frame rate
         self._segm_rate = 0
 
         # Set up logging
         # General logger for this job
         self.main_logger = logging.getLogger("dcnum")
         self.main_logger.setLevel(
@@ -233,33 +236,44 @@
         self.close(delete_temporary_files=delete_temporary_files)
 
     def get_status(self):
         # Compute the total progress. The following weights indicate
         # how much fractional time each processing step takes.
         bgw = 4  # fraction of background
         exw = 27  # fraction of segmentation and feature extraction
+        if self.job["basin_strategy"] == "drain":
+            drw = 15  # because data need to be copied
+        else:
+            drw = 1  # just creating the basins in output file
         clw = 1  # fraction of cleanup operations
-        tot = bgw + exw + clw
+        tot = bgw + exw + drw + clw
         progress = 0
         st = self.state
 
         # background
         if valid_states.index(st) > valid_states.index("background"):
             # background already computed
             progress += bgw / tot
         elif self._progress_bg is not None:
-            # This is the image count of the input dataset
-            progress += bgw / tot * (self._progress_bg.value / len(self.draw))
+            # This is the image count of the input dataset.
+            progress += self._progress_bg.value * bgw / tot
 
         # segmentation
         if valid_states.index(st) > valid_states.index("segmentation"):
             # segmentation already done
             progress += exw / tot
         elif self._progress_ex is not None:
-            progress += exw / tot * self._progress_ex
+            progress += self._progress_ex * exw / tot
+
+        # draining basins
+        if valid_states.index(st) > valid_states.index("plumbing"):
+            # plumbing already done
+            progress += drw / tot
+        if self._progress_bn is not None:
+            progress += self._progress_bn * drw / tot
 
         if self.state == "done":
             progress = 1
 
         return {
             "progress": progress,
             "segm rate": self._segm_rate,
@@ -367,24 +381,28 @@
             # Access the temporary input HDF5Data so that the underlying
             # basin file is created and close it immediately afterward.
             self.dtin.close()
             self._data_temp_in = None
             # Note any new actions that work on `self.path_temp_in` are not
             # reflected in `self.path_temp_out`.
             self.path_temp_in.rename(self.path_temp_out)
-
-        self.state = "cleanup"
-
-        # The user would normally expect the output file to be something
-        # that is self-contained (copying the file wildly across file
-        # systems and network shares should not impair feature availability).
-        # Therefore, we copy any remaining basin-based features to the
-        # temporary output file.
-        if self.job["no_basins_in_output"]:
-            self.task_transfer_basin_data()
+            # Since no segmentation was done, the output file now does not
+            # contain any events. This is not really what we wanted, but we
+            # can still store all features in the output file if required.
+            if self.job["basin_strategy"] == "drain":
+                orig_feats = []
+                for feat in self.draw.h5["events"].keys():
+                    if isinstance(self.draw.h5["events"][feat], h5py.Dataset):
+                        # copy_features does not support Groups
+                        orig_feats.append(feat)
+                with h5py.File(self.path_temp_out, "a") as h5_dst:
+                    copy_features(h5_src=self.draw.h5,
+                                  h5_dst=h5_dst,
+                                  features=orig_feats,
+                                  mapping=None)
 
         with HDF5Writer(self.path_temp_out) as hw:
             # pipeline metadata
             hw.h5.attrs["pipeline:dcnum generation"] = self.ppdict["gen_id"]
             hw.h5.attrs["pipeline:dcnum data"] = self.ppdict["dat_id"]
             hw.h5.attrs["pipeline:dcnum background"] = self.ppdict["bg_id"]
             hw.h5.attrs["pipeline:dcnum segmenter"] = self.ppdict["seg_id"]
@@ -429,15 +447,16 @@
                              cls=ExtendedJSONEncoder,
                          ).split("\n"))
 
             # copy metadata/logs/tables from original file
             with h5py.File(self.job["path_in"]) as h5_src:
                 copy_metadata(h5_src=h5_src,
                               h5_dst=hw.h5,
-                              # don't copy basins
+                              # Don't copy basins, we would have to index-map
+                              # them first.
                               copy_basins=False)
             if redo_seg:
                 # Store the correct measurement identifier. This is used to
                 # identify this file as a correct basin in subsequent pipeline
                 # steps, and it also makes sure that the original file cannot
                 # become a basin by accident (we have different indexing).
                 # This is the identifier appendix that we use to identify this
@@ -446,14 +465,20 @@
                 mid_ap = "dcn-" + self.pphash[:7]
                 # This is the current measurement identifier (may be empty).
                 mid_cur = hw.h5.attrs.get("experiment:run identifier", "")
                 # The new measurement identifier is a combination of both.
                 mid_new = f"{mid_cur}_{mid_ap}" if mid_cur else mid_ap
                 hw.h5.attrs["experiment:run identifier"] = mid_new
 
+        # Handle basin data according to the user's request
+        self.state = "plumbing"
+        self.task_enforce_basin_strategy()
+
+        self.state = "cleanup"
+
         trun = datetime.timedelta(seconds=round(time.monotonic() - time_start))
         self.logger.info(f"Run duration: {str(trun)}")
         self.logger.info(time.strftime("Run stop: %Y-%m-%d-%H.%M.%S",
                                        time.gmtime()))
         # Add the log file to the resulting .rtdc file
         if self.path_log.exists():
             with HDF5Writer(self.path_temp_out) as hw:
@@ -487,14 +512,123 @@
                 num_cpus=self.job["num_procs"],
                 # custom kwargs
                 **self.job["background_kwargs"]) as bic:
             self._progress_bg = bic.image_proc
             bic.process()
         self.logger.info("Finished background computation")
 
+    def task_enforce_basin_strategy(self):
+        """Transfer basin data from input files to output if requested
+
+        The user specified the "basin_strategy" keyword argument in
+        `self.job`. If this is set to "drain", then copy all basin
+        information from the input file to the output file. If it
+        is set to "tap", then only create basins in the output file.
+        """
+        self._progress_bn = 0
+        t0 = time.perf_counter()
+        # We need to make sure that the features are correctly attributed
+        # from the input files. E.g. if the input file already has
+        # background images, but we recompute the background images, then
+        # we have to use the data from the recomputed background file.
+        # We achieve this by keeping a specific order and only copying those
+        # features that we don't already have in the output file.
+        feats_raw = [
+            # 1. background data from the temporary input image
+            # (this must come before draw [sic!])
+            [self.dtin.h5, ["image_bg", "bg_off"], "critical"],
+            # 2. frame-based scalar features from the raw input file
+            # (e.g. "temp" or "frame")
+            [self.draw.h5, self.draw.features_scalar_frame, "optional"],
+            # 3. image features from the input file
+            [self.draw.h5, ["image", "image_bg", "bg_off"], "optional"],
+        ]
+        with h5py.File(self.path_temp_out, "a") as hout:
+            hw = HDF5Writer(hout)
+            # First, we have to determine the basin mapping from input to
+            # output. This information is stored by the QueueCollectorThread
+            # in the "basinmap0" feature, ready to be used by us.
+            if "index_unmapped" in hout["events"]:
+                # The unmapped indices enumerate the events in the output file
+                # with indices from the mapped input file. E.g. if for the
+                # first image in the input file, two events are found and for
+                # the second image in the input file, three events are found,
+                # then this would contain [0, 0, 1, 1, 1, ...]. If the index
+                # mapping of the input file was set to slice(1, 100), then the
+                # first image would not be there, and we would have
+                # [1, 1, 1, ...].
+                idx_um = hout["events/index_unmapped"]
+
+                # If we want to convert this to an actual basinmap feature,
+                # then we have to convert those indices to indices that map
+                # to the original input HDF5 file.
+                raw_im = self.draw.index_mapping
+                if raw_im is None:
+                    self.logger.info("Input file mapped with basinmap0")
+                    # Create a hard link to save time and space
+                    hout["events/basinmap0"] = hout["events/index_unmapped"]
+                    basinmap = idx_um
+                else:
+                    basinmap = get_mapping_indices(raw_im)[idx_um]
+                    # Store the mapped basin data in the output file.
+                    hw.store_feature_chunk("basinmap0", basinmap)
+                # We don't need them anymore.
+                del hout["events/index_unmapped"]
+
+                # Note that `size_raw != (len(self.draw))` [sic!]. The former
+                # is the size of the raw dataset and the latter is its mapped
+                # size!
+                size_raw = self.draw.h5.attrs["experiment:event count"]
+                if (len(basinmap) == size_raw
+                        and np.all(basinmap == np.arange(size_raw))):
+                    # This means that the images in the input overlap perfectly
+                    # with the images in the output, i.e. a "copy" segmenter
+                    # was used or something is very reproducible.
+                    # We set basinmap to None to be more efficient.
+                    basinmap = None
+
+            else:
+                # The input is identical to the output, because we are using
+                # the same pipeline identifier.
+                basinmap = None
+
+            for hin, feats, importance in feats_raw:
+                # Only consider features that are available in the input
+                # and that are not already in the output.
+                feats = [f for f in feats
+                         if (f in hin["events"] and f not in hout["events"])]
+                if not feats:
+                    continue
+                elif (self.job["basin_strategy"] == "drain"
+                      or importance == "critical"):
+                    # DRAIN: Copy all features over to the output file.
+                    self.logger.debug(f"Transferring {feats} to output file")
+                    copy_features(h5_src=hin,
+                                  h5_dst=hout,
+                                  features=feats,
+                                  mapping=basinmap)
+                else:
+                    # TAP: Create basins for the "optional" features in the
+                    # output file. Note that the "critical" features never
+                    # reach this case.
+                    self.logger.debug(f"Creating basin for {feats}")
+                    # Relative and absolute paths.
+                    pin = pathlib.Path(hin.filename).resolve()
+                    pout = pathlib.Path(hout.filename).resolve()
+                    paths = [pin, os.path.relpath(pin, pout)]
+                    hw.store_basin(name="dcnum basin",
+                                   features=feats,
+                                   mapping=basinmap,
+                                   paths=paths,
+                                   description=f"Created with dcnum {version}",
+                                   )
+                self._progress_bn += 1 / len(feats_raw)
+        t_tot = time.perf_counter() - t0
+        self.logger.info(f"Enforcing basin strategy time: {t_tot:.1f}s")
+
     def task_segment_extract(self):
         self.logger.info("Starting segmentation and feature extraction")
         # Start writer thread
         writer_dq = collections.deque()
         ds_kwds = set_default_filter_kwargs()
         thr_write = DequeWriterThread(
             path_out=self.path_temp_out,
@@ -625,29 +759,14 @@
         if self.event_count == 0:
             self.logger.error(
                 f"No events found in {self.draw.path}! Please check the "
                 f"input file or revise your pipeline")
 
         self.logger.info("Finished segmentation and feature extraction")
 
-    def task_transfer_basin_data(self):
-        with h5py.File(self.path_temp_out, "a") as hout:
-            hd = HDF5Data(hout)
-            for ii, _ in enumerate(hd.basins):
-                hindat, features = hd.get_basin_data(ii)
-                for feat in features:
-                    if feat not in hout["events"]:
-                        self.logger.debug(
-                            f"Transferring {feat} to output file")
-                        h5py.h5o.copy(src_loc=hindat.h5["events"].id,
-                                      src_name=feat.encode(),
-                                      dst_loc=hout["events"].id,
-                                      dst_name=feat.encode(),
-                                      )
-
 
 def join_thread_helper(thr, timeout, retries, logger, name):
     for _ in range(retries):
         thr.join(timeout=timeout)
         if thr.is_alive():
             logger.info(f"Waiting for '{name}' ({thr}")
         else:
```

### Comparing `dcnum-0.19.1/src/dcnum/logic/json_encoder.py` & `dcnum-0.20.0/src/dcnum/logic/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/meta/paths.py` & `dcnum-0.20.0/src/dcnum/meta/paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/meta/ppid.py` & `dcnum-0.20.0/src/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/read/cache.py` & `dcnum-0.20.0/src/dcnum/read/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,42 +18,64 @@
 class BaseImageChunkCache(abc.ABC):
     def __init__(self,
                  shape: Tuple[int],
                  chunk_size: int = 1000,
                  cache_size: int = 2,
                  ):
         self.shape = shape
+        self._dtype = None
         chunk_size = min(shape[0], chunk_size)
         self._len = self.shape[0]
         #: This is a FILO cache for the chunks
         self.cache = collections.OrderedDict()
         self.image_shape = self.shape[1:]
         self.chunk_shape = (chunk_size,) + self.shape[1:]
         self.chunk_size = chunk_size
         self.cache_size = cache_size
         self.num_chunks = int(np.ceil(self._len / (self.chunk_size or 1)))
 
     def __getitem__(self, index):
-        chunk_index, sub_index = self._get_chunk_index_for_index(index)
-        return self.get_chunk(chunk_index)[sub_index]
+        if isinstance(index, (slice, list, np.ndarray)):
+            if isinstance(index, slice):
+                indices = np.arange(index.start or 0,
+                                    index.stop or len(self),
+                                    index.step)
+            else:
+                indices = index
+            array_out = np.empty((len(indices),) + self.image_shape,
+                                 dtype=self.dtype)
+            for ii, idx in enumerate(indices):
+                array_out[ii] = self[idx]
+            return array_out
+        else:
+            chunk_index, sub_index = self._get_chunk_index_for_index(index)
+            return self.get_chunk(chunk_index)[sub_index]
 
     def __len__(self):
         return self._len
 
+    @property
+    def dtype(self):
+        """data type of the image data"""
+        if self._dtype is None:
+            self._dtype = self[0].dtype
+        return self._dtype
+
     @abc.abstractmethod
     def _get_chunk_data(self, chunk_slice):
         """Implemented in subclass to obtain actual data"""
 
     def _get_chunk_index_for_index(self, index):
         if index < 0:
             index = self._len + index
         elif index >= self._len:
             raise IndexError(
                 f"Index {index} out of bounds for HDF5ImageCache "
                 f"of size {self._len}")
+        index = int(index)  # convert np.uint64 to int, so we get ints below
         chunk_index = index // self.chunk_size
         sub_index = index % self.chunk_size
         return chunk_index, sub_index
 
     def get_chunk(self, chunk_index):
         """Return one chunk of images"""
         if chunk_index not in self.cache:
```

### Comparing `dcnum-0.19.1/src/dcnum/read/hdf5_data.py` & `dcnum-0.20.0/src/dcnum/read/hdf5_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -182,33 +182,35 @@
                            ) as h5:
                 # meta
                 self.meta = dict(h5.attrs)
                 for key in self.meta:
                     if isinstance(self.meta[key], bytes):
                         self.meta[key] = self.meta[key].decode("utf-8")
                 # logs
-                for key in h5.get("logs", []):
+                for key in sorted(h5.get("logs", {}).keys()):
                     alog = list(h5["logs"][key])
                     if alog:
                         if isinstance(alog[0], bytes):
                             alog = [ll.decode("utf") for ll in alog]
                         self.logs[key] = alog
                 # tables
-                for tab in h5.get("tables", []):
+                for tab in sorted(h5.get("tables", {}).keys()):
                     tabdict = {}
                     for tkey in h5["tables"][tab].dtype.fields.keys():
                         tabdict[tkey] = \
                             np.array(h5["tables"][tab][tkey]).reshape(-1)
                     self.tables[tab] = tabdict
                 # basins
-                for bnkey in h5.get("basins", []):
+                basins = []
+                for bnkey in h5.get("basins", {}).keys():
                     bn_data = "\n".join(
                         [s.decode() for s in h5["basins"][bnkey][:].tolist()])
                     bn_dict = json.loads(bn_data)
-                    self.basins.append(bn_dict)
+                    basins.append(bn_dict)
+                self.basins = sorted(basins, key=lambda x: x["name"])
 
         if state["pixel_size"] is not None:
             self.pixel_size = state["pixel_size"]
 
         self.image_cache_size = state["image_cache_size"]
 
         self.index_mapping = state["index_mapping"]
@@ -391,15 +393,30 @@
                         path = prel
                         break
             else:
                 path = None
             if path is None:
                 self._basin_data[index] = (None, None)
             else:
-                h5dat = HDF5Data(path, index_mapping=self.index_mapping)
+                feat_basinmap = bn_dict.get("mapping", None)
+                if feat_basinmap is None:
+                    # This is NOT a mapped basin.
+                    index_mapping = self.index_mapping
+                else:
+                    # This is a mapped basin. Create an indexing list.
+                    if self.index_mapping is None:
+                        # The current dataset is not mapped.
+                        basinmap_idx = slice(None)
+                    else:
+                        # The current dataset is also mapped.
+                        basinmap_idx = get_mapping_indices(self.index_mapping)
+                    basinmap = self.h5[f"events/{feat_basinmap}"]
+                    index_mapping = basinmap[basinmap_idx]
+
+                h5dat = HDF5Data(path, index_mapping=index_mapping)
                 features = bn_dict.get("features")
                 if features is None:
                     # Only get the features from the actual HDF5 file.
                     # If this file has basins as well, the basin metadata
                     # should have been copied over to the parent file. This
                     # makes things a little cleaner, because basins are not
                     # nested, but all basins are available in the top file.
@@ -416,29 +433,35 @@
         """Create an HDF5ImageCache object for the current dataset
 
         This method also tries to find image data in `self.basins`.
         """
         if feat not in self._image_cache:
             if f"events/{feat}" in self.h5:
                 ds = self.h5[f"events/{feat}"]
+                idx_map = self.index_mapping
             else:
+                idx_map = None
                 # search all basins
                 for idx in range(len(self.basins)):
-                    bndat, features = self.get_basin_data(idx)
+                    bn_dat, features = self.get_basin_data(idx)
                     if features is not None:
                         if feat in features:
-                            ds = bndat.h5[f"events/{feat}"]
+                            # HDF5 dataset
+                            ds = bn_dat.h5[f"events/{feat}"]
+                            # Index mapping (taken from the basins which
+                            # already includes the mapping from the current
+                            # instance).
+                            idx_map = bn_dat.index_mapping
                             break
                 else:
                     ds = None
 
             if ds is not None:
                 image = HDF5ImageCache(
-                    h5ds=get_mapped_object(obj=ds,
-                                           index_mapping=self.index_mapping),
+                    h5ds=get_mapped_object(obj=ds, index_mapping=idx_map),
                     cache_size=self.image_cache_size,
                     boolean=feat == "mask")
             else:
                 image = None
             self._image_cache[feat] = image
 
         return self._image_cache[feat]
```

### Comparing `dcnum-0.19.1/src/dcnum/read/mapped.py` & `dcnum-0.20.0/src/dcnum/read/mapped.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,24 @@
             idx_mapped = self.mapping_indices[idx]
             return self.h5ds[idx_mapped]
 
 
 def get_mapping_indices(
         index_mapping: numbers.Integral | slice | list | np.ndarray
         ):
+    """Return integer numpy array with mapping indices for a range
+
+    Parameters
+    ----------
+    index_mapping: numbers.Integral | slice | list | np.ndarray
+        Several options you have here:
+        - integer: results in np.arrange(integer)
+        - slice: results in np.arrange(slice.start, slice.stop, slice.step)
+        - list or np.ndarray: returns the input as  unit32 array
+    """
     if isinstance(index_mapping, numbers.Integral):
         return _get_mapping_indices_cached(index_mapping)
     elif isinstance(index_mapping, slice):
         return _get_mapping_indices_cached(
             (index_mapping.start, index_mapping.stop, index_mapping.step))
     elif isinstance(index_mapping, (np.ndarray, list)):
         return np.array(index_mapping, dtype=np.uint32)
```

### Comparing `dcnum-0.19.1/src/dcnum/segm/segm_thresh.py` & `dcnum-0.20.0/src/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/segm/segmenter.py` & `dcnum-0.20.0/src/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/segm/segmenter_cpu.py` & `dcnum-0.20.0/src/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/segm/segmenter_gpu.py` & `dcnum-0.20.0/src/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.20.0/src/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/src/dcnum/write/deque_writer_thread.py` & `dcnum-0.20.0/src/dcnum/write/deque_writer_thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import collections
+import logging
 import pathlib
 import threading
 import time
 
+import h5py
+
 from .writer import HDF5Writer
 
 
 class DequeWriterThread(threading.Thread):
     def __init__(self,
-                 path_out: pathlib.Path,
+                 path_out: pathlib.Path | h5py.File,
                  dq: collections.deque,
                  ds_kwds: dict = None,
                  mode: str = "a",
                  *args, **kwargs):
         """Convenience class for writing to data outside the main loop
 
         Parameters
@@ -20,14 +23,15 @@
         path_out:
             Path to the output HDF5 file
         dq: collections.deque
             `collections.deque` object from which data are taken
             using `popleft()`.
         """
         super(DequeWriterThread, self).__init__(*args, **kwargs)
+        self.logger = logging.getLogger("dcnum.write.DequeWriterThread")
         if mode == "w":
             path_out.unlink(missing_ok=True)
         self.writer = HDF5Writer(path_out, mode=mode, ds_kwds=ds_kwds)
         self.dq = dq
         self.may_stop_loop = False
         self.must_stop_loop = False
 
@@ -36,21 +40,25 @@
         self.must_stop_loop = True
 
     def finished_when_queue_empty(self):
         """Stop the loop as soon as `self.dq` is empty"""
         self.may_stop_loop = True
 
     def run(self):
+        time_tot = 0
         while True:
             ldq = len(self.dq)
             if self.must_stop_loop:
                 break
             elif ldq:
+                t0 = time.perf_counter()
                 for _ in range(ldq):
                     feat, data = self.dq.popleft()
                     self.writer.store_feature_chunk(feat=feat, data=data)
+                time_tot += time.perf_counter() - t0
             elif self.may_stop_loop:
                 break
             else:
                 # wait for the next item to arrive
                 time.sleep(.1)
+        self.logger.info(f"Disk time: {time_tot:.1f}s")
         self.writer.close()
```

### Comparing `dcnum-0.19.1/src/dcnum/write/queue_collector_thread.py` & `dcnum-0.20.0/src/dcnum/write/queue_collector_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -241,28 +241,22 @@
             # Now we also would like to add all the other information
             # that were not in the events dictionaries.
 
             # This array contains indices for `data` corresponding to
             # the events that we just saved.
             indices = stash.indices_for_data
 
-            # Write all the scalar features.
-            for feat in self.data.features_scalar_frame:
-                self.writer_dq.append((feat, self.data[feat][indices]))
-
-            # Write the image and background data.
-            imdat = np.zeros((stash.size,) + self.data.image.image_shape,
-                             dtype=np.uint8)
-            bgdat = np.zeros((stash.size,) + self.data.image.image_shape,
-                             dtype=np.uint8)
-            for ii, idx in enumerate(indices):
-                imdat[ii] = self.data.image[idx]
-                bgdat[ii] = self.data.image_bg[idx]
-            self.writer_dq.append(("image", imdat))
-            self.writer_dq.append(("image_bg", bgdat))
+            # This is the unmapped index from the input HDF5Data instance.
+            # Unmapped means that this only enumerates HDF5Data, but since
+            # HDF5Data can be mapped, the index does not necessarily enumerate
+            # the underlying HDF5 file. Later on, we will have to convert this
+            # to the correct "basinmap0" feature
+            # (see `DCNumJobRunner.task_enforce_basin_strategy`)
+            self.writer_dq.append(("index_unmapped",
+                                   np.array(indices, dtype=np.uint32)))
 
             # Write the number of events.
             self.writer_dq.append(("nevents",
                                    # Get nevents for each event from the
                                    # frame-based cur_nevents array.
                                    np.array(stash.feat_nevents)[
                                        indices - stash.index_offset]
```

### Comparing `dcnum-0.19.1/src/dcnum/write/writer.py` & `dcnum-0.20.0/src/dcnum/write/writer.py`

 * *Files 21% similar despite different names*

```diff
@@ -111,37 +111,71 @@
         return dset, offset
 
     def store_basin(self,
                     name: str,
                     paths: List[str | pathlib.Path],
                     features: List[str] = None,
                     description: str | None = None,
+                    mapping: np.ndarray = None
                     ):
         """Write an HDF5-based file basin
 
         Parameters
         ----------
         name: str
             basin name; Names do not have to be unique.
         paths: list of str or pathlib.Path
             location(s) of the basin
         features: list of str
             list of features provided by `paths`
         description: str
             optional string describing the basin
+        mapping: 1D array
+            integer array with indices that map the basin dataset
+            to this dataset
         """
         bdat = {
             "description": description,
             "format": "hdf5",
             "name": name,
             "paths": [str(pp) for pp in paths],
             "type": "file",
         }
+        # Explicit features stored in basin file
         if features is not None and len(features):
             bdat["features"] = features
+        # Mapped basin information
+        if mapping is not None:
+            events = self.h5.require_group("events")
+            # Reserve a mapping feature for this dataset
+            for ii in range(10):  # basinmap0 to basinmap9
+                bm_cand = f"basinmap{ii}"
+                if bm_cand in events:
+                    # There is a basin mapping defined in the file. Check
+                    # whether it is identical to ours.
+                    if np.all(events[bm_cand] == mapping):
+                        # Great, we are done here.
+                        feat_basinmap = bm_cand
+                        break
+                    else:
+                        # This mapping belongs to a different basin,
+                        # try the next mapping.
+                        continue
+                else:
+                    # The mapping is not defined in the dataset, and we may
+                    # write it to a new feature.
+                    feat_basinmap = bm_cand
+                    self.store_feature_chunk(feat=feat_basinmap, data=mapping)
+                    break
+            else:
+                raise ValueError(
+                    "You have exhausted the usage of mapped basins for "
+                    "the current dataset. Please revise your analysis "
+                    "pipeline.")
+            bdat["mapping"] = feat_basinmap
         bstring = json.dumps(bdat, indent=2)
         # basin key is its hash
         key = hashlib.md5(bstring.encode("utf-8",
                                          errors="ignore")).hexdigest()
         # write json-encoded basin to "basins" group
         basins = self.h5.require_group("basins")
         if key not in basins:
@@ -262,14 +296,71 @@
             hw.store_basin(name=name,
                            paths=bps,
                            features=features,
                            description=f"Created by dcnum {version}",
                            )
 
 
+def copy_features(h5_src: h5py.File,
+                  h5_dst: h5py.File,
+                  features: List[str],
+                  mapping: np.ndarray = None,
+                  ):
+    """Copy feature data from one HDF5 file to another
+
+    The feature must not exist in the destination file.
+
+    Parameters
+    ----------
+    h5_src: h5py.File
+        Input HDF5File containing `features` in the "events" group
+    h5_dst: h5py.File
+        Output HDF5File opened in write mode not containing `features`
+    features: List[str]
+        List of features to copy from source to destination
+    mapping: 1D array
+        If given, contains indices in the input file that should be
+        written to the output file. If set to None, all features are written.
+    """
+    ei = h5_src["events"]
+    eo = h5_dst.require_group("events")
+    # This is the size of the output dataset
+    size = h5_dst.attrs["experiment:event count"]
+    hw = HDF5Writer(h5_dst)
+    for feat in features:
+        if feat in eo:
+            raise ValueError(f"Output file {h5_dst.filename} already contains "
+                             f"the feature {feat}.")
+        if not isinstance(ei[feat], h5py.Dataset):
+            raise NotImplementedError(
+                f"Only dataset-based features are supported here, not {feat}")
+        if mapping is None:
+            # Just copy the data as-is.
+            h5py.h5o.copy(src_loc=ei.id,
+                          src_name=feat.encode(),
+                          dst_loc=eo.id,
+                          dst_name=feat.encode(),
+                          )
+        else:
+            # Perform mapping and store the features in chunks to keep
+            # memory usage down.
+            dsi = ei[feat]
+            chunk_size = hw.get_best_nd_chunks(dsi[0].shape, dsi.dtype)[0]
+            start = 0
+            while start < size:
+                chunk_idx = mapping[start:start + chunk_size]
+                # h5py only supports indexing in increasing order
+                chunk_unique, order = np.unique(chunk_idx, return_inverse=True)
+                data_unique = dsi[chunk_unique]
+                data = data_unique[order]
+                hw.store_feature_chunk(feat, data)
+                # increment start
+                start += chunk_size
+
+
 def copy_metadata(h5_src: h5py.File,
                   h5_dst: h5py.File,
                   copy_basins=True):
     """Copy attributes, tables, logs, and basins from one H5File to another
 
     Notes
     -----
```

### Comparing `dcnum-0.19.1/src/dcnum.egg-info/PKG-INFO` & `dcnum-0.20.0/src/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.19.1
+Version: 0.20.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.19.1/src/dcnum.egg-info/SOURCES.txt` & `dcnum-0.20.0/src/dcnum.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 tests/test_meta_ppid_data.py
 tests/test_meta_ppid_feat.py
 tests/test_meta_ppid_gate.py
 tests/test_meta_ppid_segm.py
 tests/test_read_basin.py
 tests/test_read_concat_hdf5.py
 tests/test_read_hdf5.py
+tests/test_read_hdf5_basins.py
 tests/test_read_hdf5_index_mapping.py
 tests/test_segm_base.py
 tests/test_segm_no_mask_proc.py
 tests/test_segm_thresh.py
 tests/test_write_deque_writer_thread.py
 tests/test_write_queue_collector_thread.py
 tests/test_write_writer.py
```

### Comparing `dcnum-0.19.1/tests/conftest.py` & `dcnum-0.20.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip` & `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip` & `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/data/fmt-hdf5_shapein_empty.zip` & `dcnum-0.20.0/tests/data/fmt-hdf5_shapein_empty.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip` & `dcnum-0.20.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/helper_methods.py` & `dcnum-0.20.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_background_base.py` & `dcnum-0.20.0/tests/test_feat_background_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_background_bg_copy.py` & `dcnum-0.20.0/tests/test_feat_background_bg_copy.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,14 +26,41 @@
     assert path_out.exists()
 
     with h5py.File(path_out) as h5:
         assert "image_bg" in h5["events"]
         assert np.median(h5["events/image_bg"][0]) == 186.0
 
 
+def test_copy_simple_with_bg_off():
+    path = retrieve_data(
+        "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    path_out = path.with_name("output.rtdc")
+
+    with h5py.File(path, "a") as h5:
+        assert "image_bg" in h5["events"], "sanity check"
+        bg_off = np.linspace(-1, 1, len(h5["events/deform"]))
+        h5["events/bg_off"] = bg_off
+
+    assert not path_out.exists(), "sanity check"
+
+    with bg_copy.BackgroundCopy(input_data=path,
+                                output_path=path_out) as bic:
+        assert bic.get_ppid() == "copy:"
+        # process the data
+        assert bic.get_progress() == 0
+        bic.process()
+        assert bic.get_progress() == 1
+    assert path_out.exists()
+
+    with h5py.File(path_out) as h5:
+        assert "image_bg" in h5["events"]
+        assert np.allclose(h5["events/bg_off"], bg_off)
+        assert np.median(h5["events/image_bg"][0]) == 186.0
+
+
 def test_copy_simple_same_path():
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
     path_out = path  # [sic!]
 
     with h5py.File(path) as h5:
         assert "image_bg" in h5["events"], "sanity check"
```

### Comparing `dcnum-0.19.1/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.20.0/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_background_bg_sparsemed.py` & `dcnum-0.20.0/tests/test_feat_background_bg_sparsemed.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_brightness.py` & `dcnum-0.20.0/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_event_extractor_manager.py` & `dcnum-0.20.0/tests/test_feat_event_extractor_manager.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_gate.py` & `dcnum-0.20.0/tests/test_feat_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_haralick.py` & `dcnum-0.20.0/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_moments_based.py` & `dcnum-0.20.0/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_moments_based_extended.py` & `dcnum-0.20.0/tests/test_feat_moments_based_extended.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_feat_volume.py` & `dcnum-0.20.0/tests/test_feat_volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_logic_job.py` & `dcnum-0.20.0/tests/test_logic_job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_logic_join.py` & `dcnum-0.20.0/tests/test_logic_join.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_logic_pipeline.py` & `dcnum-0.20.0/tests/test_logic_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,81 @@
     for key in hd.logs:
         if key.startswith(startswith):
             return hd.logs[key]
     else:
         raise KeyError(f"Log starting with {startswith} not found!")
 
 
+def test_basin_strategy_drain_mapped_input():
+    """When basin strategy is "drain", features are mapped from the input
+
+    This test also makes sure that basin index mapping works for input files
+    that are opened with the "index_mapping" keyword argument ot HDF5Data.
+    """
+    path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
+    path = path_orig.with_name("input.rtdc")
+    path_out = path_orig.with_name("out.rtdc")
+    with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
+        pass
+
+    job = logic.DCNumPipelineJob(path_in=path,
+                                 path_out=path_out,
+                                 data_kwargs={"index_mapping": slice(2, 5)},
+                                 basin_strategy="drain",
+                                 debug=True)
+    with logic.DCNumJobRunner(job=job) as runner:
+        runner.run()
+
+    with h5py.File(path_out) as ho, h5py.File(path) as hi:
+        assert "image_bg" in ho["events"]
+        assert "image" in ho["events"]
+        assert "bg_off" in ho["events"]
+        assert "deform" in ho["events"]
+        assert "basinmap0" in ho["events"]
+        basinmap0 = np.array([2, 2, 3, 3, 4, 4, 4])
+        assert np.all(ho["events/basinmap0"][:] == basinmap0)
+        assert np.all(hi["events/frame"][:][basinmap0]
+                      == ho["events/frame"][:])
+
+        for feat in ho["events"]:
+            assert len(ho["events"][feat]) == 7
+
+
+def test_basin_strategy_tap():
+    """When basin strategy is "tap", features are mapped from the input"""
+    path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
+    path = path_orig.with_name("input.rtdc")
+    path_out = path_orig.with_name("out.rtdc")
+    with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
+        pass
+
+    job = logic.DCNumPipelineJob(path_in=path,
+                                 path_out=path_out,
+                                 background_kwargs={"kernel_size": 150},
+                                 basin_strategy="tap",
+                                 debug=True)
+    with logic.DCNumJobRunner(job=job) as runner:
+        runner.run()
+
+    with h5py.File(path_out) as h5:
+        assert h5.attrs["pipeline:dcnum background"] \
+               == "sparsemed:k=150^s=1^t=0^f=0.8^o=1"
+        assert "image_bg" in h5["events"]
+        assert "bg_off" in h5["events"]
+        assert "deform" in h5["events"]
+        # the rest of the original features are basins!
+        assert "time" not in h5["events"]
+        assert "image" not in h5["events"]
+        for feat in h5["events"]:
+            assert len(h5["events"][feat]) == 275
+        # The other features are accessed via basins
+        hd = read.HDF5Data(h5)
+        assert "image" in hd
+
+
 def test_chained_pipeline():
     """Test running two pipelines consecutively"""
     path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path = path_orig.with_name("input.rtdc")
     path2 = path.with_name("path_intermediate.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
@@ -37,30 +104,37 @@
     # perform the initial pipeline
     with logic.DCNumJobRunner(job=job) as runner:
         runner.run()
 
     with h5py.File(path2) as h5:
         assert h5.attrs["pipeline:dcnum background"] \
                == "sparsemed:k=150^s=1^t=0^f=0.8^o=1"
+        assert "image" in h5["events"]
+        assert "image_bg" in h5["events"]
+        for feat in h5["events"]:
+            assert len(h5["events"][feat]) == 275
 
-    # now when we do everything again, not a things should be done
+    # now when we do everything again, the pipeline changes
     job2 = logic.DCNumPipelineJob(path_in=path2,
                                   path_out=path2.with_name("final_out.rtdc"),
                                   background_kwargs={"kernel_size": 250},
                                   debug=True)
+
     with logic.DCNumJobRunner(job=job2) as runner2:
         runner2.run()
 
     with h5py.File(job2["path_out"]) as h5:
         assert "deform" in h5["events"]
         assert "image" in h5["events"]
         assert "image_bg" in h5["events"]
         assert len(h5["events/deform"]) == 285
         assert h5.attrs["pipeline:dcnum background"] \
                == "sparsemed:k=250^s=1^t=0^f=0.8^o=1"
+        for feat in h5["events"]:
+            assert len(h5["events"][feat]) == 285
 
 
 def test_duplicate_pipeline():
     """Test running the same pipeline twice
 
     When the pipeline is run on a file that has been run with the same
     pipeline identifier, then we do not run the pipeline. Instead, we
@@ -104,15 +178,14 @@
         assert len(h5["events/deform"]) == 395
         del h5["logs"]
 
     # now when we do everything again, not a thing should be done
     job2 = logic.DCNumPipelineJob(
         path_in=path2,
         path_out=path2.with_name("final_out.rtdc"),
-        no_basins_in_output=True,
         background_code="copy",
         segmenter_code="thresh",
         segmenter_kwargs={"thresh": -6,
                           "kwargs_mask": {"closing_disk": 0}},
         debug=True)
     with logic.DCNumJobRunner(job=job2) as runner2:
         runner2.run()
@@ -185,15 +258,15 @@
         # Modify the yield, triggering a new pipeline run
         h5.attrs["pipeline:dcnum yield"] = 111111
 
     # now when we do everything again, not a thing should be done
     job2 = logic.DCNumPipelineJob(
         path_in=path2,
         path_out=path2.with_name("final_out.rtdc"),
-        no_basins_in_output=True,
+
         data_kwargs={"index_mapping": 10},
         background_code="copy",
         segmenter_code="thresh",
         segmenter_kwargs={"thresh": -6,
                           "kwargs_mask": {"closing_disk": 0}},
         debug=True)
     with logic.DCNumJobRunner(job=job2) as runner2:
@@ -270,15 +343,14 @@
         # Modify the yield, triggering a new pipeline run
         h5.attrs["pipeline:dcnum yield"] = 111111
 
     # now when we do everything again, not a thing should be done
     job2 = logic.DCNumPipelineJob(
         path_in=path2,
         path_out=path2.with_name("final_out.rtdc"),
-        no_basins_in_output=True,
         background_code="copy",
         segmenter_code="thresh",
         segmenter_kwargs={"thresh": -6,
                           "kwargs_mask": {"closing_disk": 0}},
         debug=True)
     with logic.DCNumJobRunner(job=job2) as runner2:
         runner2.run()
@@ -371,40 +443,19 @@
 
     # perform the initial pipeline
     with logic.DCNumJobRunner(job=job) as runner:
         runner.run()
 
     with h5py.File(path2) as h5:
         # The feature comes from the input file and will *not* be copied.
+        # The "peter" feature is also not part of the PROTECTED_FEATURES,
+        # so there should never be a "peter" feature from any input file
+        # in any output file.
         assert "peter" not in h5["events"]
 
-    # Now we change things. The input file now contains basins that should
-    # also be present in the output file. Using the `no_basins_in_output`
-    # option, the feature data from the input should actually be stored
-    # in the output file.
-    with write.HDF5Writer(path2) as hw2:
-        del hw2.h5["logs"]  # remove logs
-        path_basin2 = path2.with_name("data_basin_2.rtdc")
-        # store the basin in the original file
-        hw2.store_basin(name="test", paths=[path_basin2], features=["peter2"])
-        # store the peter data in the basin
-        with h5py.File(path_basin2, "a") as hb2:
-            hb2["events/peter2"] = 3.15 * hw2.h5["events/deform"][:]
-
-    job2 = logic.DCNumPipelineJob(path_in=path2,
-                                  path_out=path2.with_name("final_out.rtdc"),
-                                  no_basins_in_output=True,
-                                  debug=True)
-    with logic.DCNumJobRunner(job=job2) as runner2:
-        runner2.run()
-
-    with h5py.File(job2["path_out"]) as h52:
-        # The feature comes from the input file and *will* be copied.
-        assert "peter2" in h52["events"]
-
 
 def test_error_file_exists():
     path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path = path_orig.with_name("input.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
     path_out = path.with_name("test_out.rtdc")
```

### Comparing `dcnum-0.19.1/tests/test_meta_paths.py` & `dcnum-0.20.0/tests/test_meta_paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_meta_ppid_base.py` & `dcnum-0.20.0/tests/test_meta_ppid_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_meta_ppid_bg.py` & `dcnum-0.20.0/tests/test_meta_ppid_bg.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_meta_ppid_data.py` & `dcnum-0.20.0/tests/test_meta_ppid_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_meta_ppid_feat.py` & `dcnum-0.20.0/tests/test_meta_ppid_feat.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_meta_ppid_gate.py` & `dcnum-0.20.0/tests/test_meta_ppid_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_meta_ppid_segm.py` & `dcnum-0.20.0/tests/test_meta_ppid_segm.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_read_basin.py` & `dcnum-0.20.0/tests/test_read_basin.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_read_concat_hdf5.py` & `dcnum-0.20.0/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_read_hdf5.py` & `dcnum-0.20.0/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_read_hdf5_index_mapping.py` & `dcnum-0.20.0/tests/test_read_hdf5_index_mapping.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_segm_base.py` & `dcnum-0.20.0/tests/test_segm_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_segm_no_mask_proc.py` & `dcnum-0.20.0/tests/test_segm_no_mask_proc.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_segm_thresh.py` & `dcnum-0.20.0/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_write_deque_writer_thread.py` & `dcnum-0.20.0/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.19.1/tests/test_write_queue_collector_thread.py` & `dcnum-0.20.0/tests/test_write_queue_collector_thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,25 +76,25 @@
 
     # BATCH 1
     feat, deform1 = writer_dq.popleft()
     assert feat == "deform"
     assert np.all(deform1 == [.1, .1, .2, .3])
     feat, _ = writer_dq.popleft()
     assert feat == "area_um"
-    for fexp in data.features_scalar_frame + ["image", "image_bg", "nevents"]:
+    for fexp in ["index_unmapped", "nevents"]:
         fact, _ = writer_dq.popleft()
         assert fexp == fact
 
     # BATCH 2
     feat, deform1 = writer_dq.popleft()
     assert feat == "deform"
     assert np.all(deform1 == [.1, .1, .2, .3, .4, .5])
     feat, _ = writer_dq.popleft()
     assert feat == "area_um"
-    for fexp in data.features_scalar_frame + ["image", "image_bg", "nevents"]:
+    for fexp in ["index_unmapped", "nevents"]:
         fact, _ = writer_dq.popleft()
         assert fexp == fact
 
     assert len(writer_dq) == 0
 
 
 def test_queue_collector_thread_with_full_stash():
@@ -143,22 +143,22 @@
 
     # BATCH 1
     feat, deform1 = writer_dq.popleft()
     assert feat == "deform"
     assert np.all(deform1 == [.1, .1, .2, .3])
     feat, _ = writer_dq.popleft()
     assert feat == "area_um"
-    for fexp in data.features_scalar_frame + ["image", "image_bg", "nevents"]:
+    for fexp in ["index_unmapped", "nevents"]:
         fact, _ = writer_dq.popleft()
         assert fexp == fact
 
     # BATCH 2
     feat, deform1 = writer_dq.popleft()
     assert feat == "deform"
     assert np.all(deform1 == [.1, .1, .2, .3, .4, .5])
     feat, _ = writer_dq.popleft()
     assert feat == "area_um"
-    for fexp in data.features_scalar_frame + ["image", "image_bg", "nevents"]:
+    for fexp in ["index_unmapped", "nevents"]:
         fact, _ = writer_dq.popleft()
         assert fexp == fact
 
     assert len(writer_dq) == 0
```

### Comparing `dcnum-0.19.1/tests/test_write_writer.py` & `dcnum-0.20.0/tests/test_write_writer.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,87 @@
 
 from dcnum import read, write
 from dcnum import __version__ as version
 
 from helper_methods import retrieve_data
 
 
+@pytest.mark.parametrize("mapping,mslice", [
+    [None, slice(None)],
+    [np.arange(3), slice(0, 3)],
+    [np.arange(2, 4), slice(2, 4)],
+])
+def test_copy_features(mapping, mslice):
+    path = retrieve_data(
+        "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    path_wrt = path.with_name("written.hdf5")
+
+    with h5py.File(path, "r") as h5_src, h5py.File(path_wrt, "w") as h5_dst:
+        write.copy_metadata(h5_src=h5_src, h5_dst=h5_dst, copy_basins=False)
+        write.copy_features(h5_src=h5_src,
+                            h5_dst=h5_dst,
+                            features=["deform", "image", "aspect"],
+                            mapping=mapping,
+                            )
+        assert np.all(h5_src["events/deform"][mslice]
+                      == h5_dst["events/deform"][:])
+        assert np.all(h5_src["events/image"][mslice]
+                      == h5_dst["events/image"][:])
+        assert np.all(h5_src["events/aspect"][mslice]
+                      == h5_dst["events/aspect"][:])
+
+
+def test_copy_features_error_exists():
+    path = retrieve_data(
+        "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    path_wrt = path.with_name("written.hdf5")
+
+    with h5py.File(path, "r") as h5_src, h5py.File(path_wrt, "w") as h5_dst:
+        write.copy_metadata(h5_src=h5_src, h5_dst=h5_dst, copy_basins=False)
+        write.copy_features(h5_src=h5_src,
+                            h5_dst=h5_dst,
+                            features=["deform"],
+                            )
+        with pytest.raises(ValueError, match="already contains the feature"):
+            write.copy_features(h5_src=h5_src,
+                                h5_dst=h5_dst,
+                                features=["deform"],
+                                )
+
+
+def test_copy_features_error_missing():
+    path = retrieve_data(
+        "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    path_wrt = path.with_name("written.hdf5")
+
+    with h5py.File(path, "r") as h5_src, h5py.File(path_wrt, "w") as h5_dst:
+        write.copy_metadata(h5_src=h5_src, h5_dst=h5_dst, copy_basins=False)
+        with pytest.raises(KeyError, match="object 'peter' doesn't exist"):
+            write.copy_features(h5_src=h5_src,
+                                h5_dst=h5_dst,
+                                features=["peter"],
+                                )
+
+
+def test_copy_features_error_type_group():
+    path = retrieve_data(
+        "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
+    path_wrt = path.with_name("written.hdf5")
+
+    with h5py.File(path, "a") as h5_src, h5py.File(path_wrt, "w") as h5_dst:
+        write.copy_metadata(h5_src=h5_src, h5_dst=h5_dst, copy_basins=False)
+        h5_src["events"].require_group("peter")
+        with pytest.raises(NotImplementedError,
+                           match="dataset-based features are supported"):
+            write.copy_features(h5_src=h5_src,
+                                h5_dst=h5_dst,
+                                features=["peter"],
+                                )
+
+
 def test_copy_metadata_empty_log_variable_length_string():
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
 
     # Add an empty log file
     with h5py.File(path, "a") as h5:
         data = np.asarray([], dtype=h5py.string_dtype(length=None))
```

