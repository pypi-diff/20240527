# Comparing `tmp/torchoutil-0.3.1.tar.gz` & `tmp/torchoutil-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchoutil-0.3.1.tar", last modified: Thu Apr 25 15:01:15 2024, max compression
+gzip compressed data, was "torchoutil-0.4.0.tar", last modified: Mon May 27 15:36:56 2024, max compression
```

## Comparing `torchoutil-0.3.1.tar` & `torchoutil-0.4.0.tar`

### file list

```diff
@@ -1,103 +1,106 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.452894 torchoutil-0.3.1/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1064 2024-03-01 09:46:35.000000 torchoutil-0.3.1/LICENSE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7441 2024-04-25 15:01:15.448894 torchoutil-0.3.1/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4865 2024-04-25 14:46:40.000000 torchoutil-0.3.1/README.md
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1959 2024-03-07 15:01:16.000000 torchoutil-0.3.1/pyproject.toml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-04-25 14:46:40.000000 torchoutil-0.3.1/requirements-dev.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-04-25 14:46:40.000000 torchoutil-0.3.1/requirements-extras.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       57 2024-03-04 17:33:08.000000 torchoutil-0.3.1/requirements.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-04-25 15:01:15.452894 torchoutil-0.3.1/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2024-03-04 17:33:08.000000 torchoutil-0.3.1/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      376 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/__main__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil/hub/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       96 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/hub/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      996 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/hub/download.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6856 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/hub/registry.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1032 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil/nn/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       70 2024-04-17 12:32:36.000000 torchoutil-0.3.1/src/torchoutil/nn/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/nn/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      329 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      404 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/activation.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2566 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      460 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/get.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4475 2024-03-08 10:17:47.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/indices.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12723 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4805 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/multiclass.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6945 2024-03-08 10:17:47.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1231 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/numpy.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4534 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/others.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8564 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2877 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/functional/transform.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/nn/modules/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      297 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      810 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/activation.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2064 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1643 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/layer.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1381 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5870 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/multiclass.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6125 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1244 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/numpy.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3740 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9618 2024-04-25 12:28:31.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/tensor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2833 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/transform.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6170 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/nn/modules/typed.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/optim/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       68 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/optim/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1805 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/optim/utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-04-25 13:24:09.000000 torchoutil-0.3.1/src/torchoutil/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10196 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/collections.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.444894 torchoutil-0.3.1/src/torchoutil/utils/data/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      141 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/utils/data/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2370 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/utils/data/collate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      523 2024-04-17 14:04:29.000000 torchoutil-0.3.1/src/torchoutil/utils/data/dataloader.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1508 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/data/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4099 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/utils/data/split.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/src/torchoutil/utils/hdf/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      394 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      875 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16619 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16706 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/hdf/pack.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2797 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/log_utils.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      730 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/packaging.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      177 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      473 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3842 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6055 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/pack.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      528 2024-03-04 17:33:08.000000 torchoutil-0.3.1/src/torchoutil/utils/return_types.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/src/torchoutil/utils/saving/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      195 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      945 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1598 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/csv_io.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2389 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/saving/yaml_io.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5297 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/tensorboard.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2658 2024-04-25 14:46:40.000000 torchoutil-0.3.1/src/torchoutil/utils/type_checks.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.440894 torchoutil-0.3.1/src/torchoutil.egg-info/
--rw-r--r--   0 labbeti   (1000) labbeti   (1000)     7441 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2924 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      206 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       11 2024-04-25 15:01:15.000000 torchoutil-0.3.1/src/torchoutil.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-25 15:01:15.448894 torchoutil-0.3.1/tests/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1176 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_hub.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      472 2024-03-04 17:33:08.000000 torchoutil-0.3.1/tests/test_nn_functional_crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      620 2024-03-07 15:01:16.000000 torchoutil-0.3.1/tests/test_nn_functional_indices.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10920 2024-03-07 12:43:25.000000 torchoutil-0.3.1/tests/test_nn_functional_mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1659 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_functional_multiclass.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3836 2024-03-07 15:01:16.000000 torchoutil-0.3.1/tests/test_nn_functional_multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2478 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_functional_others.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7010 2024-03-07 12:42:21.000000 torchoutil-0.3.1/tests/test_nn_functional_pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1750 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_functional_transform.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      674 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_modules.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1240 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_nn_modules_multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2239 2024-03-01 09:46:35.000000 torchoutil-0.3.1/tests/test_readme.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3484 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_utils_collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1967 2024-03-07 15:01:16.000000 torchoutil-0.3.1/tests/test_utils_hdf.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5279 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_utils_pickle.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      755 2024-04-25 14:46:40.000000 torchoutil-0.3.1/tests/test_utils_type_checks.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.451690 torchoutil-0.4.0/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1064 2024-03-01 09:46:35.000000 torchoutil-0.4.0/LICENSE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7477 2024-05-27 15:36:56.451690 torchoutil-0.4.0/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4901 2024-05-27 15:17:34.000000 torchoutil-0.4.0/README.md
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1959 2024-03-07 15:01:16.000000 torchoutil-0.4.0/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-04-25 14:46:40.000000 torchoutil-0.4.0/requirements-dev.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       79 2024-05-27 15:17:34.000000 torchoutil-0.4.0/requirements-extras.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       57 2024-03-04 17:33:08.000000 torchoutil-0.4.0/requirements.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-05-27 15:36:56.451690 torchoutil-0.4.0/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2024-03-04 17:33:08.000000 torchoutil-0.4.0/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.439689 torchoutil-0.4.0/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.443690 torchoutil-0.4.0/src/torchoutil/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      650 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-03-04 17:33:08.000000 torchoutil-0.4.0/src/torchoutil/__main__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.443690 torchoutil-0.4.0/src/torchoutil/hub/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       96 2024-04-17 14:04:29.000000 torchoutil-0.4.0/src/torchoutil/hub/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1453 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/hub/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6931 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/hub/registry.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1032 2024-03-04 17:33:08.000000 torchoutil-0.4.0/src/torchoutil/info.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.443690 torchoutil-0.4.0/src/torchoutil/nn/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       70 2024-05-14 12:52:06.000000 torchoutil-0.4.0/src/torchoutil/nn/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.443690 torchoutil-0.4.0/src/torchoutil/nn/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1561 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      447 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/activation.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2566 2024-05-10 13:46:50.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      513 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/get.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4459 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/indices.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12760 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5995 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10031 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1459 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/numpy.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6918 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/others.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8588 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4203 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/functional/transform.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.443690 torchoutil-0.4.0/src/torchoutil/nn/modules/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1253 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      810 2024-05-14 12:56:45.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/activation.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2059 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1601 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/layer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1393 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    14780 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/mixins.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6561 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7092 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1656 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/numpy.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3724 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    11393 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/tensor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4052 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/nn/modules/transform.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.447690 torchoutil-0.4.0/src/torchoutil/optim/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       68 2024-04-25 14:46:40.000000 torchoutil-0.4.0/src/torchoutil/optim/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1253 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/optim/schedulers.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1826 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/optim/utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.447690 torchoutil-0.4.0/src/torchoutil/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-04-25 13:24:09.000000 torchoutil-0.4.0/src/torchoutil/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10787 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/collections.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.447690 torchoutil-0.4.0/src/torchoutil/utils/data/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      272 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/data/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2370 2024-05-13 11:41:49.000000 torchoutil-0.4.0/src/torchoutil/utils/data/collate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      523 2024-04-17 14:04:29.000000 torchoutil-0.4.0/src/torchoutil/utils/data/dataloader.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1508 2024-05-13 11:47:02.000000 torchoutil-0.4.0/src/torchoutil/utils/data/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4115 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/data/split.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.447690 torchoutil-0.4.0/src/torchoutil/utils/hdf/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      394 2024-03-04 17:33:08.000000 torchoutil-0.4.0/src/torchoutil/utils/hdf/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      882 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/hdf/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16633 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/hdf/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16664 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/hdf/pack.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4880 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/log_utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.447690 torchoutil-0.4.0/src/torchoutil/utils/pack/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      155 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/pack/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      528 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/pack/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4612 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/pack/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6928 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/pack/pack.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      886 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/packaging.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      528 2024-03-04 17:33:08.000000 torchoutil-0.4.0/src/torchoutil/utils/return_types.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.447690 torchoutil-0.4.0/src/torchoutil/utils/saving/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      236 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/saving/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3458 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/saving/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2440 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/saving/csv_io.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2821 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/saving/yaml_io.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5297 2024-04-25 14:46:40.000000 torchoutil-0.4.0/src/torchoutil/utils/tensorboard.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6462 2024-05-27 15:17:34.000000 torchoutil-0.4.0/src/torchoutil/utils/type_checks.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.443690 torchoutil-0.4.0/src/torchoutil.egg-info/
+-rw-r--r--   0 labbeti   (1000) labbeti   (1000)     7477 2024-05-27 15:36:56.000000 torchoutil-0.4.0/src/torchoutil.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2986 2024-05-27 15:36:56.000000 torchoutil-0.4.0/src/torchoutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-05-27 15:36:56.000000 torchoutil-0.4.0/src/torchoutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-05-27 15:36:56.000000 torchoutil-0.4.0/src/torchoutil.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      215 2024-05-27 15:36:56.000000 torchoutil-0.4.0/src/torchoutil.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       11 2024-05-27 15:36:56.000000 torchoutil-0.4.0/src/torchoutil.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-05-27 15:36:56.451690 torchoutil-0.4.0/tests/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1176 2024-05-07 09:14:26.000000 torchoutil-0.4.0/tests/test_hub.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      472 2024-03-04 17:33:08.000000 torchoutil-0.4.0/tests/test_nn_functional_crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      620 2024-03-07 15:01:16.000000 torchoutil-0.4.0/tests/test_nn_functional_indices.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10920 2024-03-07 12:43:25.000000 torchoutil-0.4.0/tests/test_nn_functional_mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1639 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_functional_multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5064 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_functional_multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4667 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_functional_others.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7010 2024-03-07 12:42:21.000000 torchoutil-0.4.0/tests/test_nn_functional_pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1787 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_functional_transform.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      690 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_modules.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1683 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_modules_mixins.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1323 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_modules_multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1375 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_nn_modules_multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2442 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_readme.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3516 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_utils_collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1984 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_utils_hdf.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6309 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_utils_pack.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2971 2024-05-27 15:17:34.000000 torchoutil-0.4.0/tests/test_utils_type_checks.py
```

### Comparing `torchoutil-0.3.1/LICENSE` & `torchoutil-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/PKG-INFO` & `torchoutil-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchoutil
-Version: 0.3.1
+Version: 0.4.0
 Summary: Collection of functions and modules to help development in PyTorch.
 Author-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Labbeti
         
@@ -83,96 +83,98 @@
 
 To check if the package is installed and show the package version, you can use the following command:
 ```bash
 torchoutil-info
 ```
 
 
-## Usage
+## Examples
 
-### Batch of padded sequences
+### Multilabel conversions
 ```python
 import torch
-from torchoutil import masked_mean
+from torchoutil import probs_to_name
 
-x = torch.as_tensor([1, 2, 3, 4])
-mask = torch.as_tensor([True, True, False, False])
-result = masked_mean(x, mask)
-# result contains the mean of the values marked as True: 1.5
+probs = torch.as_tensor([[0.9, 0.1], [0.4, 0.6]])
+names = probs_to_name(probs, idx_to_name={0: "Cat", 1: "Dog"})
+# ["Cat", "Dog"]
+```
+
+```python
+import torch
+from torchoutil import multihot_to_indices
+
+multihot = torch.as_tensor([[1, 0, 0], [0, 1, 1], [0, 0, 0]])
+indices = multihot_to_indices(multihot)
+# [[0], [1, 2], []]
 ```
 
+### Masked operations
+
 ```python
 import torch
 from torchoutil import lengths_to_non_pad_mask
 
 x = torch.as_tensor([3, 1, 2])
 mask = lengths_to_non_pad_mask(x, max_len=4)
 # Each row i contains x[i] True values for non-padding mask
 # tensor([[True, True, True, False],
 #         [True, False, False, False],
 #         [True, True, False, False]])
 ```
 
-### Multilabel conversions
-```python
-import torch
-from torchoutil import probs_to_names
-
-probs = torch.as_tensor([[0.9, 0.1], [0.6, 0.9]])
-names = probs_to_names(probs, threshold=0.5, idx_to_name={0: "Cat", 1: "Dog"})
-# [["Cat"], ["Cat", "Dog"]]
-```
-
 ```python
 import torch
-from torchoutil import multihot_to_indices
+from torchoutil import masked_mean
 
-multihot = torch.as_tensor([[1, 0, 0], [0, 1, 1], [0, 0, 0]])
-indices = multihot_to_indices(multihot)
-# [[0], [1, 2], []]
+x = torch.as_tensor([1, 2, 3, 4])
+mask = torch.as_tensor([True, True, False, False])
+result = masked_mean(x, mask)
+# result contains the mean of the values marked as True: 1.5
 ```
 
-### Easely pre-compute transforms
+### Pre-compute datasets to pickle or HDF files
 
-Here is an example of pre-computing spectrograms of torchaudio `SPEECHCOMMANDS` dataset, using `pack_to_pickle` function:
+Here is an example of pre-computing spectrograms of torchaudio `SPEECHCOMMANDS` dataset, using `pack_to_custom` function:
 
 ```python
 from torch import nn
 from torchaudio.datasets import SPEECHCOMMANDS
 from torchaudio.transforms import Spectrogram
-from torchoutil.utils.pickle_dataset import pack_to_pickle
+from torchoutil.utils.pack import pack_to_custom
 
 speech_commands_root = "path/to/speech_commands"
-pickle_root = "path/to/pickle_dataset"
+packed_root = "path/to/packed_dataset"
 
 dataset = SPEECHCOMMANDS(speech_commands_root, download=True, subset="validation")
+# dataset[0] is a tuple, contains waveform and other metadata
 
 class MyTransform(nn.Module):
     def __init__(self) -> None:
         super().__init__()
         self.spectrogram_extractor = Spectrogram()
 
     def forward(self, item):
         waveform = item[0]
         spectrogram = self.spectrogram_extractor(waveform)
         return (spectrogram,) + item[1:]
 
-pack_to_pickle(dataset, pickle_root, MyTransform())
+pack_to_custom(dataset, packed_root, MyTransform())
 ```
 
-Then you can load the pre-computed dataset using `PickleDataset`:
+Then you can load the pre-computed dataset using `PackedDataset`:
 ```python
-from torchoutil.utils.pickle_dataset import PickleDataset
+from torchoutil.utils.pack import PackedDataset
 
-pickle_root = "path/to/pickle_dataset"
-pickle_dataset = PickleDataset(pickle_root)
-pickle_dataset[0]  # == first transformed item, i.e. transform(dataset[0])
+packed_root = "path/to/packed_dataset"
+packed_dataset = PackedDataset(packed_root)
+packed_dataset[0]  # == first transformed item, i.e. transform(dataset[0])
 ```
 
-### ...and more tensor manipulations!
+### Other tensors manipulations!
 
 ```python
 import torch
 from torchoutil import insert_at_indices
 
 x = torch.as_tensor([1, 2, 3, 4])
 result = insert_at_indices(x, indices=[0, 2], values=5)
@@ -188,19 +190,19 @@
 
 x1 = torch.rand(10)
 x2 = x1[perm]
 x3 = x2[inv_perm]
 # inv_perm are indices that allow us to get x3 from x2, i.e. x1 == x3 here
 ```
 
-## Extras
+## Extras requirements
 `torchoutil` also provides additional modules when some specific package are already installed in your environment.
 All extras can be installed with `pip install torchoutil[extras]`
 
 - If `tensorboard` is installed, the function `load_event_file` can be used. It is useful to load manually all data contained in an tensorboard event file.
-- If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
+- If `numpy` is installed, the classes `NumpyToTensor` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
 - If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF files, and supports variable-length sequences of data.
 
 
 ## Contact
 Maintainer:
 - [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `torchoutil-0.3.1/README.md` & `torchoutil-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,96 +32,98 @@
 
 To check if the package is installed and show the package version, you can use the following command:
 ```bash
 torchoutil-info
 ```
 
 
-## Usage
+## Examples
 
-### Batch of padded sequences
+### Multilabel conversions
 ```python
 import torch
-from torchoutil import masked_mean
+from torchoutil import probs_to_name
 
-x = torch.as_tensor([1, 2, 3, 4])
-mask = torch.as_tensor([True, True, False, False])
-result = masked_mean(x, mask)
-# result contains the mean of the values marked as True: 1.5
+probs = torch.as_tensor([[0.9, 0.1], [0.4, 0.6]])
+names = probs_to_name(probs, idx_to_name={0: "Cat", 1: "Dog"})
+# ["Cat", "Dog"]
+```
+
+```python
+import torch
+from torchoutil import multihot_to_indices
+
+multihot = torch.as_tensor([[1, 0, 0], [0, 1, 1], [0, 0, 0]])
+indices = multihot_to_indices(multihot)
+# [[0], [1, 2], []]
 ```
 
+### Masked operations
+
 ```python
 import torch
 from torchoutil import lengths_to_non_pad_mask
 
 x = torch.as_tensor([3, 1, 2])
 mask = lengths_to_non_pad_mask(x, max_len=4)
 # Each row i contains x[i] True values for non-padding mask
 # tensor([[True, True, True, False],
 #         [True, False, False, False],
 #         [True, True, False, False]])
 ```
 
-### Multilabel conversions
-```python
-import torch
-from torchoutil import probs_to_names
-
-probs = torch.as_tensor([[0.9, 0.1], [0.6, 0.9]])
-names = probs_to_names(probs, threshold=0.5, idx_to_name={0: "Cat", 1: "Dog"})
-# [["Cat"], ["Cat", "Dog"]]
-```
-
 ```python
 import torch
-from torchoutil import multihot_to_indices
+from torchoutil import masked_mean
 
-multihot = torch.as_tensor([[1, 0, 0], [0, 1, 1], [0, 0, 0]])
-indices = multihot_to_indices(multihot)
-# [[0], [1, 2], []]
+x = torch.as_tensor([1, 2, 3, 4])
+mask = torch.as_tensor([True, True, False, False])
+result = masked_mean(x, mask)
+# result contains the mean of the values marked as True: 1.5
 ```
 
-### Easely pre-compute transforms
+### Pre-compute datasets to pickle or HDF files
 
-Here is an example of pre-computing spectrograms of torchaudio `SPEECHCOMMANDS` dataset, using `pack_to_pickle` function:
+Here is an example of pre-computing spectrograms of torchaudio `SPEECHCOMMANDS` dataset, using `pack_to_custom` function:
 
 ```python
 from torch import nn
 from torchaudio.datasets import SPEECHCOMMANDS
 from torchaudio.transforms import Spectrogram
-from torchoutil.utils.pickle_dataset import pack_to_pickle
+from torchoutil.utils.pack import pack_to_custom
 
 speech_commands_root = "path/to/speech_commands"
-pickle_root = "path/to/pickle_dataset"
+packed_root = "path/to/packed_dataset"
 
 dataset = SPEECHCOMMANDS(speech_commands_root, download=True, subset="validation")
+# dataset[0] is a tuple, contains waveform and other metadata
 
 class MyTransform(nn.Module):
     def __init__(self) -> None:
         super().__init__()
         self.spectrogram_extractor = Spectrogram()
 
     def forward(self, item):
         waveform = item[0]
         spectrogram = self.spectrogram_extractor(waveform)
         return (spectrogram,) + item[1:]
 
-pack_to_pickle(dataset, pickle_root, MyTransform())
+pack_to_custom(dataset, packed_root, MyTransform())
 ```
 
-Then you can load the pre-computed dataset using `PickleDataset`:
+Then you can load the pre-computed dataset using `PackedDataset`:
 ```python
-from torchoutil.utils.pickle_dataset import PickleDataset
+from torchoutil.utils.pack import PackedDataset
 
-pickle_root = "path/to/pickle_dataset"
-pickle_dataset = PickleDataset(pickle_root)
-pickle_dataset[0]  # == first transformed item, i.e. transform(dataset[0])
+packed_root = "path/to/packed_dataset"
+packed_dataset = PackedDataset(packed_root)
+packed_dataset[0]  # == first transformed item, i.e. transform(dataset[0])
 ```
 
-### ...and more tensor manipulations!
+### Other tensors manipulations!
 
 ```python
 import torch
 from torchoutil import insert_at_indices
 
 x = torch.as_tensor([1, 2, 3, 4])
 result = insert_at_indices(x, indices=[0, 2], values=5)
@@ -137,19 +139,19 @@
 
 x1 = torch.rand(10)
 x2 = x1[perm]
 x3 = x2[inv_perm]
 # inv_perm are indices that allow us to get x3 from x2, i.e. x1 == x3 here
 ```
 
-## Extras
+## Extras requirements
 `torchoutil` also provides additional modules when some specific package are already installed in your environment.
 All extras can be installed with `pip install torchoutil[extras]`
 
 - If `tensorboard` is installed, the function `load_event_file` can be used. It is useful to load manually all data contained in an tensorboard event file.
-- If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
+- If `numpy` is installed, the classes `NumpyToTensor` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
 - If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF files, and supports variable-length sequences of data.
 
 
 ## Contact
 Maintainer:
 - [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `torchoutil-0.3.1/pyproject.toml` & `torchoutil-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/hub/registry.py` & `torchoutil-0.4.0/src/torchoutil/hub/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,54 @@
 # -*- coding: utf-8 -*-
 
 import json
 import logging
 import os
 import os.path as osp
 from pathlib import Path
-from typing import Callable, Dict, List, Mapping, Optional, Tuple, TypedDict, Union
+from typing import (
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Mapping,
+    Optional,
+    Tuple,
+    TypedDict,
+    TypeVar,
+    Union,
+)
 
 import torch
 from torch import Tensor
+from torch.types import Device
 from typing_extensions import NotRequired
 
 from torchoutil.hub.download import HashType, hash_file
 from torchoutil.nn.functional.get import get_device
 
 pylog = logging.getLogger(__name__)
 
 
+T = TypeVar("T")
+
+
 class RegistryEntry(TypedDict):
     url: str
     fname: str
     hash_value: NotRequired[str]
     hash_type: NotRequired[HashType]
     state_dict_key: NotRequired[str]
     architecture: NotRequired[str]
 
 
-class RegistryHub:
+class RegistryHub(Generic[T]):
     def __init__(
         self,
-        infos: Mapping[str, RegistryEntry],
+        infos: Mapping[T, RegistryEntry],
         register_root: Union[str, Path, None] = None,
     ) -> None:
         """
         Args:
             infos: Maps model_name to their checkpoint information, with download url, filename, hash value, hash type and state_dict key.
             register_root: Directory where checkpoints are saved. If None, defaults to `~/.cache/torch/hub/checkpoints`.
         """
@@ -45,44 +60,44 @@
             register_root = Path(register_root)
 
         super().__init__()
         self._infos = infos
         self._ckpt_parent_path = register_root
 
     @property
-    def infos(self) -> Dict[str, RegistryEntry]:
+    def infos(self) -> Dict[T, RegistryEntry]:
         return self._infos
 
     @property
     def register_root(self) -> Path:
         return self._ckpt_parent_path.resolve()
 
     @property
-    def names(self) -> List[str]:
+    def names(self) -> List[T]:
         return list(self._infos.keys())
 
     @property
     def paths(self) -> List[Path]:
         return [self.get_path(model_name) for model_name in self.names]
 
-    def get_path(self, name: str) -> Path:
+    def get_path(self, name: T) -> Path:
         if name not in self.names:
             raise ValueError(
                 f"Invalid argument {name=}. (expected one of {self.names})"
             )
 
         fname = self._infos[name]["fname"]
         fpath = self.register_root.joinpath(fname)
         return fpath
 
     def load_state_dict(
         self,
-        name_or_path: Union[str, Path],
+        name_or_path: Union[T, str, Path],
         *,
-        device: Union[str, torch.device, None] = None,
+        device: Device = None,
         offline: bool = False,
         load_fn: Callable = torch.load,
         verbose: int = 0,
     ) -> Dict[str, Tensor]:
         """Load state_dict weights.
 
         Args:
@@ -92,15 +107,14 @@
             load_fn: Load function backend. defaults to torch.load.
             verbose: Verbose level. defaults to 0.
 
         Returns:
             Loaded file content.
         """
         device = get_device(device)
-        name_or_path = str(name_or_path)
 
         if osp.isfile(name_or_path):
             path = name_or_path
             name = self._get_name(path)
         else:
             name = name_or_path
             try:
@@ -136,15 +150,15 @@
                 f"Loading encoder weights from '{path}'... (with test_mAP={test_map})"
             )
 
         return state_dict
 
     def download_file(
         self,
-        name: str,
+        name: T,
         force: bool = False,
         check_hash: bool = True,
         verbose: int = 0,
     ) -> Tuple[Path, bool]:
         """Download checkpoint file."""
         model_path = self.get_path(name)
         exists = model_path.exists()
@@ -168,15 +182,15 @@
         if valid:
             return model_path, True
         else:
             raise ValueError(f"Invalid hash for file '{model_path}'.")
 
     def is_valid_hash(
         self,
-        name: str,
+        name: T,
     ) -> bool:
         info = self.infos[name]
         if "hash_type" not in info or "hash_value" not in info:
             pylog.warning(
                 f"Cannot check hash for {name}. (cannot find any expected hash value or type)"
             )
             return True
@@ -201,26 +215,26 @@
     @classmethod
     def from_file(cls, path: Union[str, Path]) -> "RegistryHub":
         """Load register info from JSON file."""
         with open(path, "r") as file:
             args = json.load(file)
         return RegistryHub(**args)
 
-    def _get_name(self, path: Union[str, Path]) -> Optional[str]:
+    def _get_name(self, path: Union[str, Path]) -> Optional[T]:
         path_to_name = {
             path_i.resolve().expanduser(): name_i
             for path_i, name_i in zip(self.paths, self.names)
         }
         path = Path(path).resolve().expanduser()
         if path in path_to_name:
-            model_name = path_to_name[path]
+            name = path_to_name[path]
         else:
-            model_name = None
-        return model_name
+            name = None
+        return name
 
 
 def get_default_register_root() -> Path:
-    """Default checkpoint path: `~/.cache/torch/hub/checkpoints`."""
+    """Default register root path is `~/.cache/torch/hub/checkpoints`, which is based on `torch.hub.get_dir`."""
     path = torch.hub.get_dir()
     path = Path(path)
     path = path.joinpath("checkpoints")
     return path
```

### Comparing `torchoutil-0.3.1/src/torchoutil/info.py` & `torchoutil-0.4.0/src/torchoutil/info.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/functional/crop.py` & `torchoutil-0.4.0/src/torchoutil/nn/functional/crop.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/functional/indices.py` & `torchoutil-0.4.0/src/torchoutil/nn/functional/indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Any, Dict, List, Union
 
 import torch
 from torch import Tensor
-from torch.types import Number
+from torch.types import Device, Number
 
 from torchoutil.nn.functional.get import _DEVICE_CUDA_IF_AVAILABLE, get_device
 
 
 def get_inverse_perm(indices: Tensor, dim: int = -1) -> Tensor:
     """Return inverse permutation indices.
     The output will be a tensor of shape (..., N).
@@ -28,15 +28,15 @@
     indices_inv = indices_inv.scatter(dim, indices, arange)
     return indices_inv
 
 
 def randperm_diff(
     size: int,
     generator: Union[None, int, torch.Generator] = None,
-    device: Union[str, torch.device, None] = _DEVICE_CUDA_IF_AVAILABLE,
+    device: Device = _DEVICE_CUDA_IF_AVAILABLE,
 ) -> Tensor:
     """This function ensure that every value i cannot be the element at index i.
     The output will be a tensor of shape (size,).
 
     Args:
         size: The number of indices. Cannot be < 2.
         seed: The seed or torch.Generator used to generate permutation.
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/functional/mask.py` & `torchoutil-0.4.0/src/torchoutil/nn/functional/mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Iterable, List, Optional, Union
 
 import torch
 from torch import Tensor
+from torch.types import Device
 
 from torchoutil.nn.functional.get import get_device
 
 
 def masked_mean(
     x: Tensor,
     non_pad_mask: Tensor,
+    *,
     dim: Union[None, int, Iterable[int]] = None,
 ) -> Tensor:
     """Average a tensor along the specified dim(s).
 
     Args:
         tensor: (N, ...)
         non_pad_mask: Non-padding mask, should be broadcastable with argument tensor and reduced with argument dim.
@@ -33,14 +35,15 @@
     reduced = masked.sum(dim=dim) / non_pad_mask.sum(dim=dim).clamp(min=1.0)
     return reduced
 
 
 def masked_sum(
     x: Tensor,
     non_pad_mask: Tensor,
+    *,
     dim: Union[None, int, Iterable[int]] = None,
 ) -> Tensor:
     """Sum a tensor along the specified dim(s).
 
     Args:
         x: (N, ...)
         non_pad_mask: Non-padding mask, should be broadcastable with argument tensor and reduced with argument dim.
@@ -71,22 +74,22 @@
         x2: Second tensor of shape S.
         mask: Boolean tensor of shape S. Position marked as False are ignored by the equality.
     """
     if x1.shape != x2.shape:
         return False
     mask = mask.bool().logical_not().logical_or(x1.eq(x2))
     equal = mask.all().item()
-    return equal
+    return equal  # type: ignore
 
 
 def generate_square_subsequent_mask(
     size: int,
     diagonal: int = 0,
     *,
-    device: Union[str, torch.device, None] = None,
+    device: Device = None,
     dtype: Optional[torch.dtype] = None,
 ) -> Tensor:
     device = get_device(device)
     mask = torch.ones((size, size), device=device, dtype=torch.bool)
     mask = torch.tril(mask, diagonal=diagonal)
     mask = torch.where(mask, 0.0, -torch.inf)
     mask = mask.to(dtype=dtype)
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/functional/multiclass.py` & `torchoutil-0.4.0/src/torchoutil/nn/functional/multiclass.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,170 +1,211 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """Helper functions for conversion between classes indices, onehot, names and probabilities for multiclass classification.
 """
 
-from typing import List, Mapping, Optional, Sequence, TypeVar, Union
+from typing import Hashable, Iterable, List, Mapping, Optional, Sequence, TypeVar, Union
 
 import torch
 from torch import Tensor
 from torch.nn import functional as F
+from torch.types import Device
 
 from torchoutil.nn.functional.get import get_device
+from torchoutil.utils.type_checks import is_scalar
 
 T = TypeVar("T")
 
 
-def indices_to_onehot(
-    indices: Union[Sequence[int], Tensor, Sequence],
+def index_to_onehot(
+    index: Union[Sequence[int], Tensor, Sequence],
     num_classes: int,
     *,
     padding_idx: Optional[int] = None,
-    device: Union[str, torch.device, None] = None,
+    device: Device = None,
     dtype: Union[torch.dtype, None] = torch.bool,
 ) -> Tensor:
     """Convert indices of labels to onehot boolean encoding.
 
     Args:
         indices: List label indices.
             Can be a nested list of indices, but it should be convertible to Tensor.
         num_classes: Number maximal of unique classes.
         padding_idx: Class index to ignore. Output will contains only zeroes for this value. defaults to None.
         device: PyTorch device of the output tensor.
         dtype: PyTorch DType of the output tensor.
     """
     device = get_device(device)
-    indices = torch.as_tensor(indices, device=device, dtype=torch.long)
+    index = torch.as_tensor(index, device=device, dtype=torch.long)
 
     if padding_idx is not None:
-        mask = indices == padding_idx
-        indices = torch.where(mask, num_classes, indices)
+        mask = index == padding_idx
+        index = torch.where(mask, num_classes, index)
         num_classes += 1
 
-    onehot: Tensor = F.one_hot(indices, num_classes)
+    onehot: Tensor = F.one_hot(index, num_classes)
     onehot = onehot.to(dtype=dtype)
 
     if padding_idx is not None:
-        onehot = onehot[..., :-1].contiguous()
+        onehot = onehot[..., :-1]
 
     return onehot
 
 
-def indices_to_names(
-    indices: Union[Sequence[int], Tensor],
-    idx_to_name: Mapping[int, T],
+def index_to_name(
+    index: Union[Sequence[int], Tensor, Sequence],
+    idx_to_name: Union[Mapping[int, T], Sequence[T]],
 ) -> List[T]:
     """Convert indices of labels to names using a mapping.
 
     Args:
         indices: List of list of label indices.
         idx_to_name: Mapping to convert a class index to its name.
     """
-    return [idx_to_name[indices_i] for indices_i in indices]  # type: ignore
 
+    def index_to_name_impl(x) -> Union[T, list]:
+        if is_scalar(x):
+            return idx_to_name[x]  # type: ignore
+        elif isinstance(x, Iterable):
+            return [index_to_name_impl(xi) for xi in x]
+        else:
+            raise ValueError(
+                f"Invalid argument {x=}. (not present in idx_to_name and not an iterable type)"
+            )
 
-def onehot_to_indices(
+    name = index_to_name_impl(index)
+    return name  # type: ignore
+
+
+def onehot_to_index(
     onehot: Tensor,
+    *,
+    dim: int = -1,
 ) -> List[int]:
     """Convert onehot boolean encoding to indices of labels.
 
     Args:
-        onehot: OneHot labels encoded as 2D matrix.
+        onehot: Onehot labels encoded as 2D matrix.
     """
-    return onehot.int().argmax(dim=-1).tolist()
+    onehot = onehot.int()
+    index = onehot.argmax(dim=dim)
+    index = index.tolist()
+    return index
 
 
-def onehot_to_names(
+def onehot_to_name(
     onehot: Tensor,
-    idx_to_name: Mapping[int, T],
+    idx_to_name: Union[Mapping[int, T], Sequence[T]],
+    *,
+    dim: int = -1,
 ) -> List[T]:
     """Convert onehot boolean encoding to names using a mapping.
 
     Args:
-        onehot: OneHot labels encoded as 2D matrix.
+        onehot: Onehot labels encoded as 2D matrix.
         idx_to_name: Mapping to convert a class index to its name.
     """
-    indices = onehot_to_indices(onehot)
-    names = indices_to_names(indices, idx_to_name)
+    indices = onehot_to_index(onehot, dim=dim)
+    names = index_to_name(indices, idx_to_name)
     return names
 
 
-def names_to_indices(
-    names: List[T],
-    idx_to_name: Mapping[int, T],
+def name_to_index(
+    name: List[T],
+    idx_to_name: Union[Mapping[int, T], Sequence[T]],
 ) -> List[int]:
     """Convert names to indices of labels.
 
     Args:
         names: List of list of label names.
         idx_to_name: Mapping to convert a class index to its name.
     """
-    name_to_idx = {name: idx for idx, name in idx_to_name.items()}
-    indices = [name_to_idx[name] for name in names]
-    return indices
-
-
-def names_to_onehot(
-    names: List[T],
-    idx_to_name: Mapping[int, T],
+    if isinstance(idx_to_name, Mapping):
+        name_to_idx = {name: idx for idx, name in idx_to_name.items()}
+    else:
+        name_to_idx = {name: idx for idx, name in enumerate(idx_to_name)}
+    del idx_to_name
+
+    def name_to_index_impl(x) -> Union[T, list]:
+        if isinstance(x, Hashable) and x in name_to_idx:
+            return name_to_idx[x]  # type: ignore
+        elif isinstance(x, Iterable):
+            return [name_to_index_impl(xi) for xi in x]
+        else:
+            raise ValueError(
+                f"Invalid argument {x=}. (not present in name_to_idx and not an iterable type)"
+            )
+
+    index = name_to_index_impl(name)
+    return index  # type: ignore
+
+
+def name_to_onehot(
+    name: List[T],
+    idx_to_name: Union[Mapping[int, T], Sequence[T]],
     *,
-    device: Union[str, torch.device, None] = None,
+    device: Device = None,
     dtype: Union[torch.dtype, None] = torch.bool,
 ) -> Tensor:
     """Convert names to onehot boolean encoding.
 
     Args:
         names: List of list of label names.
         idx_to_name: Mapping to convert a class index to its name.
         device: PyTorch device of the output tensor.
         dtype: PyTorch DType of the output tensor.
     """
-    indices = names_to_indices(names, idx_to_name)
-    onehot = indices_to_onehot(indices, len(idx_to_name), device=device, dtype=dtype)
+    index = name_to_index(name, idx_to_name)
+    onehot = index_to_onehot(index, len(idx_to_name), device=device, dtype=dtype)
     return onehot
 
 
-def probs_to_indices(
+def probs_to_index(
     probs: Tensor,
+    *,
+    dim: int = -1,
 ) -> List[int]:
     """Convert matrix of probabilities to indices of labels.
 
     Args:
         probs: Output probabilities for each classes.
     """
-    indices = probs.argmax(dim=-1)
-    indices = indices.tolist()
-    return indices
+    index = probs.argmax(dim=dim)
+    index = index.tolist()
+    return index
 
 
 def probs_to_onehot(
     probs: Tensor,
     *,
-    device: Union[str, torch.device, None] = None,
+    dim: int = -1,
+    device: Device = None,
     dtype: Union[torch.dtype, None] = torch.bool,
 ) -> Tensor:
     """Convert matrix of probabilities to onehot boolean encoding.
 
     Args:
         probs: Output probabilities for each classes.
     """
     if device is None:
         device = probs.device
-    indices = probs_to_indices(probs)
-    onehot = indices_to_onehot(indices, probs.shape[-1], device=device, dtype=dtype)
+    indices = probs_to_index(probs, dim=dim)
+    onehot = index_to_onehot(indices, probs.shape[-1], device=device, dtype=dtype)
     return onehot
 
 
-def probs_to_names(
+def probs_to_name(
     probs: Tensor,
-    idx_to_name: Mapping[int, T],
+    idx_to_name: Union[Mapping[int, T], Sequence[T]],
+    *,
+    dim: int = -1,
 ) -> List[T]:
     """Convert matrix of probabilities to labels names.
 
     Args:
         probs: Output probabilities for each classes.
         idx_to_name: Mapping to convert a class index to its name.
     """
-    indices = probs_to_indices(probs)
-    names = indices_to_names(indices, idx_to_name)
+    indices = probs_to_index(probs, dim=dim)
+    names = index_to_name(indices, idx_to_name)
     return names
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/functional/numpy.py` & `torchoutil-0.4.0/src/torchoutil/nn/functional/numpy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Any, Literal, Union
+from typing import Union
 
 import torch
 from torch import Tensor
-from typing_extensions import TypeGuard
+from torch.types import Device
 
 from torchoutil.nn.functional.get import get_device
 from torchoutil.utils.packaging import _NUMPY_AVAILABLE
 
 if not _NUMPY_AVAILABLE:
-
-    def is_numpy_scalar(x: Any) -> Literal[False]:
-        return False
+    ACCEPTED_NUMPY_DTYPES = ()
 
 else:
     import numpy as np
 
+    ACCEPTED_NUMPY_DTYPES = (
+        np.float64,
+        np.float32,
+        np.float16,
+        np.complex64,
+        np.complex128,
+        np.int64,
+        np.int32,
+        np.int16,
+        np.int8,
+        np.uint8,
+        bool,
+    )
+
     def to_numpy(
         x: Union[Tensor, np.ndarray, list],
         *,
         dtype: Union[str, np.dtype, None] = None,
     ) -> np.ndarray:
+        """Convert input to numpy array."""
         if isinstance(x, Tensor):
-            return x.cpu().numpy().astype(dtype=dtype)
+            return tensor_to_numpy(x, dtype=dtype)
         else:
             return np.asarray(x, dtype=dtype)
 
-    def from_numpy(
+    def tensor_to_numpy(
+        x: Tensor,
+        *,
+        dtype: Union[str, np.dtype, None] = None,
+    ) -> np.ndarray:
+        """Convert PyTorch tensor to numpy array."""
+        return x.cpu().numpy().astype(dtype=dtype)
+
+    def numpy_to_tensor(
         x: np.ndarray,
         *,
-        device: Union[str, torch.device, None] = None,
+        device: Device = None,
         dtype: Union[torch.dtype, None] = None,
     ) -> Tensor:
+        """Convert numpy array to PyTorch tensor."""
         device = get_device(device)
         return torch.from_numpy(x).to(dtype=dtype, device=device)
-
-    def is_numpy_scalar(x: Any) -> TypeGuard[Union[np.generic, np.ndarray]]:
-        """Returns True if x is a numpy generic type or a zero-dimensional numpy array."""
-        return isinstance(x, np.generic) or (isinstance(x, np.ndarray) and x.ndim == 0)
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/functional/pad.py` & `torchoutil-0.4.0/src/torchoutil/nn/functional/pad.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # -*- coding: utf-8 -*-
 
 from typing import Any, Callable, Dict, Iterable, List, Literal, Sized, Tuple, Union
 
 import torch
 from torch import Generator, Size, Tensor
 from torch.nn import functional as F
-from torch.types import Number
+from torch.types import Device, Number
 
 from torchoutil.nn.functional.get import get_device
-from torchoutil.nn.functional.others import can_be_stacked, is_scalar
+from torchoutil.nn.functional.others import can_be_stacked
+from torchoutil.utils.type_checks import is_scalar
 
 PAD_ALIGNS = ("left", "right", "center", "random")
 PadAlign = Literal["left", "right", "center", "random"]
 PadValue = Union[Number, Callable[[Tensor], Number]]
 
 
 def pad_dim(
@@ -69,15 +70,15 @@
     return x
 
 
 def pad_and_stack_rec(
     sequence: Union[Tensor, int, float, tuple, list],
     pad_value: Number,
     *,
-    device: Union[str, torch.device, None] = None,
+    device: Device = None,
     dtype: Union[None, torch.dtype] = None,
 ) -> Tensor:
     """Recursive version of torch.nn.utils.rnn.pad_sequence, with padding of Tensors.
 
     Args:
         sequence: The sequence to pad. Must be convertable to tensor by having the correct number of dims in all sublists.
         pad_value: The pad value used.
@@ -137,55 +138,14 @@
 
     else:
         raise TypeError(
             f"Invalid type {type(sequence)}. (expected Tensor, int, float, list or tuple)"
         )
 
 
-def __generate_pad_seq(
-    x_shape: Size,
-    target_lengths: List[int],
-    dims: List[int],
-    aligns: List[PadAlign],
-    generator: Union[None, Generator],
-) -> List[int]:
-    pad_seq = [0 for _ in range(len(x_shape) * 2)]
-    for target_length, dim, align in zip(target_lengths, dims, aligns):
-        missing = max(target_length - x_shape[dim], 0)
-
-        if align == "left":
-            missing_left = 0
-            missing_right = missing
-        elif align == "right":
-            missing_left = missing
-            missing_right = 0
-        elif align == "center":
-            missing_left = missing // 2 + missing % 2
-            missing_right = missing // 2
-        elif align == "random":
-            missing_left = int(
-                torch.randint(
-                    low=0, high=missing + 1, size=(), generator=generator
-                ).item()
-            )
-            missing_right = missing - missing_left
-        else:
-            raise ValueError(
-                f"Invalid argument {align=}. (expected one of {PAD_ALIGNS})"
-            )
-
-        # Note: pad_seq : [pad_left_dim_-1, pad_right_dim_-1, pad_left_dim_-2, pad_right_dim_-2, ...)
-        idx = len(x_shape) - (dim % len(x_shape)) - 1
-        assert pad_seq[idx * 2] == 0 and pad_seq[idx * 2 + 1] == 0
-        pad_seq[idx * 2] = missing_left
-        pad_seq[idx * 2 + 1] = missing_right
-
-    return pad_seq
-
-
 def cat_padded_batch(
     x1: Tensor,
     x1_lens: Tensor,
     x2: Tensor,
     x2_lens: Tensor,
     seq_dim: int = -1,
     batch_dim: int = 0,
@@ -228,14 +188,55 @@
         slices = [slice(None) for _ in range(ndim)]
         slices[seq_dim] = slice(max_size_12)
         x12 = x12[slices]
 
     return x12, x12_lens
 
 
+def __generate_pad_seq(
+    x_shape: Size,
+    target_lengths: List[int],
+    dims: List[int],
+    aligns: List[PadAlign],
+    generator: Union[None, Generator],
+) -> List[int]:
+    pad_seq = [0 for _ in range(len(x_shape) * 2)]
+    for target_length, dim, align in zip(target_lengths, dims, aligns):
+        missing = max(target_length - x_shape[dim], 0)
+
+        if align == "left":
+            missing_left = 0
+            missing_right = missing
+        elif align == "right":
+            missing_left = missing
+            missing_right = 0
+        elif align == "center":
+            missing_left = missing // 2 + missing % 2
+            missing_right = missing // 2
+        elif align == "random":
+            missing_left = int(
+                torch.randint(
+                    low=0, high=missing + 1, size=(), generator=generator
+                ).item()
+            )
+            missing_right = missing - missing_left
+        else:
+            raise ValueError(
+                f"Invalid argument {align=}. (expected one of {PAD_ALIGNS})"
+            )
+
+        # Note: pad_seq : [pad_left_dim_-1, pad_right_dim_-1, pad_left_dim_-2, pad_right_dim_-2, ...)
+        idx = len(x_shape) - (dim % len(x_shape)) - 1
+        assert pad_seq[idx * 2] == 0 and pad_seq[idx * 2 + 1] == 0
+        pad_seq[idx * 2] = missing_left
+        pad_seq[idx * 2 + 1] = missing_right
+
+    return pad_seq
+
+
 def _check_cat_padded_batch(
     x1: Tensor,
     x1_lens: Tensor,
     x2: Tensor,
     x2_lens: Tensor,
     seq_dim: int,
     batch_dim: int,
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/activation.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/crop.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
         target_length: int,
         align: CropAlign = "left",
         dim: int = -1,
         generator: Union[int, Generator, None] = None,
     ) -> None:
         super().__init__()
         self.target_length = target_length
-        self.align = align
+        self.align: CropAlign = align
         self.dim = dim
         self.generator = generator
 
     def forward(
         self,
         x: Tensor,
     ) -> Tensor:
         return crop_dim(
             x,
             self.target_length,
-            self.align,  # type: ignore
+            self.align,
             self.dim,
             self.generator,
         )
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/layer.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import math
-from typing import Union
 
 import torch
 from torch import Tensor, nn
+from torch.types import Device
 
 from torchoutil.nn.functional.get import get_device
 
 
 class PositionalEncoding(nn.Module):
     def __init__(
         self,
         emb_size: int,
         dropout_p: float,
         maxlen: int = 5000,
-        device: Union[str, torch.device, None] = None,
+        device: Device = None,
     ) -> None:
         """Vanilla Positional Encoding for transformers networks.
 
         Based on PyTorch tutorial from: https://pytorch.org/tutorials/beginner/transformer_tutorial.html
         """
         pos_embedding = init_pos_emb(emb_size, maxlen, device)
 
@@ -34,15 +34,15 @@
         output = self.dropout(token_emb + pos_emb)
         return output
 
 
 def init_pos_emb(
     emb_size: int,
     maxlen: int = 5000,
-    device: Union[str, torch.device, None] = None,
+    device: Device = None,
 ) -> Tensor:
     """Returns positional embedding tensor of shape (1, maxlen, emb_size)."""
     device = get_device(device)
 
     den = torch.exp(
         -torch.arange(0, emb_size, 2, device=device) * math.log(10000) / emb_size
     )
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/mask.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/mask.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,39 +15,39 @@
     """
 
     def __init__(self, dim: Union[None, int, Iterable[int]] = None) -> None:
         super().__init__()
         self.dim = dim
 
     def forward(self, tensor: Tensor, non_pad_mask: Tensor) -> Tensor:
-        reduced = masked_mean(tensor, non_pad_mask, self.dim)
+        reduced = masked_mean(tensor, non_pad_mask, dim=self.dim)
         return reduced
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 dim=self.dim,
             ),
-            ignore_none=True,
+            ignore_lst=(None,),
         )
 
 
 class MaskedSum(nn.Module):
     """
     For more information, see :func:`~torchoutil.nn.functional.mask.masked_sum`.
     """
 
     def __init__(self, dim: Union[None, int, Iterable[int]] = None) -> None:
         super().__init__()
         self.dim = dim
 
     def forward(self, tensor: Tensor, non_pad_mask: Tensor) -> Tensor:
-        reduced = masked_sum(tensor, non_pad_mask, self.dim)
+        reduced = masked_sum(tensor, non_pad_mask, dim=self.dim)
         return reduced
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 dim=self.dim,
             ),
-            ignore_none=True,
+            ignore_lst=(None,),
         )
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/multiclass.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/multiclass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Generic, List, Mapping, Optional, TypeVar, Union
+from typing import Generic, List, Mapping, Optional, Sequence, TypeVar, Union
 
 import torch
 from torch import Tensor, nn
+from torch.types import Device
 
 from torchoutil.nn.functional.multiclass import (
-    indices_to_names,
-    indices_to_onehot,
-    names_to_indices,
-    names_to_onehot,
-    onehot_to_indices,
-    onehot_to_names,
-    probs_to_indices,
-    probs_to_names,
+    index_to_name,
+    index_to_onehot,
+    name_to_index,
+    name_to_onehot,
+    onehot_to_index,
+    onehot_to_name,
+    probs_to_index,
+    probs_to_name,
     probs_to_onehot,
 )
 from torchoutil.utils.collections import dump_dict
 
 T = TypeVar("T")
 
 
-class IndicesToOneHot(nn.Module):
+class IndexToOnehot(nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.indices_to_onehot`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.index_to_onehot`.
     """
 
     def __init__(
         self,
         num_classes: int,
         *,
         padding_idx: Optional[int] = None,
-        device: Union[str, torch.device, None] = None,
+        device: Device = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.padding_idx = padding_idx
         self.device = device
         self.dtype = dtype
 
     def forward(
         self,
-        indices: Union[List[int], Tensor],
+        index: Union[List[int], Tensor],
     ) -> Tensor:
-        onehot = indices_to_onehot(
-            indices,
+        onehot = index_to_onehot(
+            index,
             self.num_classes,
             padding_idx=self.padding_idx,
             device=self.device,
             dtype=self.dtype,
         )
         return onehot
 
@@ -58,193 +59,218 @@
         return dump_dict(
             dict(
                 num_classes=self.num_classes,
                 padding_idx=self.padding_idx,
                 device=self.device,
                 dtype=self.dtype,
             ),
-            ignore_none=True,
+            ignore_lst=(None,),
         )
 
 
-class IndicesToNames(nn.Module, Generic[T]):
+class IndexToName(Generic[T], nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.indices_to_names`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.index_to_name`.
     """
 
     def __init__(
         self,
-        idx_to_name: Mapping[int, T],
+        idx_to_name: Union[Mapping[int, T], Sequence[T]],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
     def forward(
         self,
-        indices: Union[List[int], Tensor],
+        index: Union[List[int], Tensor],
     ) -> List[T]:
-        names = indices_to_names(indices, self.idx_to_name)
-        return names
+        name = index_to_name(index, self.idx_to_name)
+        return name
 
 
-class OneHotToIndices(nn.Module):
+class OnehotToIndex(nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.onehot_to_indices`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.onehot_to_index`.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, dim: int = -1) -> None:
         super().__init__()
+        self.dim = dim
 
     def forward(
         self,
         onehot: Tensor,
     ) -> List[int]:
-        names = onehot_to_indices(onehot)
-        return names
+        index = onehot_to_index(onehot, dim=self.dim)
+        return index
+
+    def extra_repr(self) -> str:
+        return dump_dict(dict(dim=self.dim))
 
 
-class OneHotToNames(nn.Module, Generic[T]):
+class OnehotToName(Generic[T], nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.onehot_to_names`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.onehot_to_name`.
     """
 
     def __init__(
         self,
-        idx_to_name: Mapping[int, T],
+        idx_to_name: Union[Mapping[int, T], Sequence[T]],
+        dim: int = -1,
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
+        self.dim = dim
 
     def forward(
         self,
         onehot: Tensor,
     ) -> List[T]:
-        names = onehot_to_names(onehot, self.idx_to_name)
-        return names
+        name = onehot_to_name(onehot, self.idx_to_name, dim=self.dim)
+        return name
 
+    def extra_repr(self) -> str:
+        return dump_dict(dict(dim=self.dim))
 
-class NamesToIndices(nn.Module, Generic[T]):
+
+class NameToIndex(Generic[T], nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.names_to_indices`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.name_to_index`.
     """
 
     def __init__(
         self,
-        idx_to_name: Mapping[int, T],
+        idx_to_name: Union[Mapping[int, T], Sequence[T]],
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
 
     def forward(
         self,
-        names: List[T],
+        name: List[T],
     ) -> List[int]:
-        indices = names_to_indices(names, self.idx_to_name)
-        return indices
+        index = name_to_index(name, self.idx_to_name)
+        return index
 
 
-class NamesToOneHot(nn.Module, Generic[T]):
+class NameToOnehot(Generic[T], nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.names_to_onehot`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.name_to_onehot`.
     """
 
     def __init__(
         self,
-        idx_to_name: Mapping[int, T],
+        idx_to_name: Union[Mapping[int, T], Sequence[T]],
         *,
-        device: Union[str, torch.device, None] = None,
+        device: Device = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
         self.device = device
         self.dtype = dtype
 
     def forward(
         self,
-        names: List[T],
+        name: List[T],
     ) -> Tensor:
-        onehot = names_to_onehot(
-            names,
+        onehot = name_to_onehot(
+            name,
             self.idx_to_name,
             device=self.device,
             dtype=self.dtype,
         )
         return onehot
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 device=self.device,
                 dtype=self.dtype,
             ),
-            ignore_none=True,
+            ignore_lst=(None,),
         )
 
 
-class ProbsToIndices(nn.Module):
+class ProbsToIndex(nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_indices`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_index`.
     """
 
+    def __init__(self, dim: int = -1) -> None:
+        super().__init__()
+        self.dim = dim
+
     def forward(
         self,
         probs: Tensor,
     ) -> List[int]:
-        indices = probs_to_indices(probs)
-        return indices
+        index = probs_to_index(probs, dim=self.dim)
+        return index
+
+    def extra_repr(self) -> str:
+        return dump_dict(dict(dim=self.dim))
 
 
-class ProbsToOneHot(nn.Module):
+class ProbsToOnehot(nn.Module):
     """
     For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_onehot`.
     """
 
     def __init__(
         self,
         *,
-        device: Union[str, torch.device, None] = None,
+        dim: int = -1,
+        device: Device = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
+        self.dim = dim
         self.device = device
         self.dtype = dtype
 
     def forward(
         self,
         probs: Tensor,
     ) -> Tensor:
         onehot = probs_to_onehot(
             probs,
+            dim=self.dim,
             device=self.device,
             dtype=self.dtype,
         )
         return onehot
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
+                dim=self.dim,
                 device=self.device,
                 dtype=self.dtype,
             ),
-            ignore_none=True,
+            ignore_lst=(None,),
         )
 
 
-class ProbsToNames(nn.Module, Generic[T]):
+class ProbsToName(Generic[T], nn.Module):
     """
-    For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_names`.
+    For more information, see :func:`~torchoutil.nn.functional.multiclass.probs_to_name`.
     """
 
     def __init__(
         self,
-        idx_to_name: Mapping[int, T],
+        idx_to_name: Union[Mapping[int, T], Sequence[T]],
+        dim: int = -1,
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
+        self.dim = dim
 
     def forward(
         self,
         probs: Tensor,
     ) -> List[T]:
-        names = probs_to_names(probs, self.idx_to_name)
-        return names
+        name = probs_to_name(probs, self.idx_to_name, dim=self.dim)
+        return name
+
+    def extra_repr(self) -> str:
+        return dump_dict(dict(dim=self.dim))
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/numpy.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/numpy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,65 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Union
+from typing import Any, Union
 
 import torch
 from torch import Tensor, nn
+from torch.types import Device
 
+from torchoutil.nn.functional.numpy import numpy_to_tensor, tensor_to_numpy, to_numpy
 from torchoutil.utils.packaging import _NUMPY_AVAILABLE
 
-if _NUMPY_AVAILABLE:
+if not _NUMPY_AVAILABLE:
+
+    class np:
+        dtype = Any
+        ndarray = Any
+
+else:
     import numpy as np
 
-    from torchoutil.nn.functional.numpy import from_numpy, to_numpy
 
-    class ToNumpy(nn.Module):
-        """
-        For more information, see :func:`~torchoutil.nn.functional.numpy.to_numpy`.
-        """
-
-        def __init__(self, *, dtype: Union[str, np.dtype, None] = None) -> None:
-            super().__init__()
-            self.dtype = dtype
-
-        def forward(self, x: Union[Tensor, np.ndarray, list]) -> np.ndarray:
-            return to_numpy(x, dtype=self.dtype)
-
-    class FromNumpy(nn.Module):
-        """
-        For more information, see :func:`~torchoutil.nn.functional.numpy.from_numpy`.
-        """
-
-        def __init__(
-            self,
-            *,
-            device: Union[str, torch.device, None] = None,
-            dtype: Union[torch.dtype, None] = None,
-        ) -> None:
-            super().__init__()
-            self.device = device
-            self.dtype = dtype
+class ToNumpy(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.numpy.to_numpy`.
+    """
+
+    def __init__(self, *, dtype: Union[str, np.dtype, None] = None) -> None:
+        super().__init__()
+        self.dtype = dtype
+
+    def forward(self, x: Union[Tensor, np.ndarray, list]) -> np.ndarray:
+        return to_numpy(x, dtype=self.dtype)
+
+
+class TensorToNumpy(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.numpy.tensor_to_numpy`.
+    """
+
+    def __init__(self, *, dtype: Union[str, np.dtype, None] = None) -> None:
+        super().__init__()
+        self.dtype = dtype
+
+    def forward(self, x: Union[Tensor, np.ndarray, list]) -> np.ndarray:
+        return tensor_to_numpy(x, dtype=self.dtype)
+
+
+class NumpyToTensor(nn.Module):
+    """
+    For more information, see :func:`~torchoutil.nn.functional.numpy.numpy_to_tensor`.
+    """
+
+    def __init__(
+        self,
+        *,
+        device: Device = None,
+        dtype: Union[torch.dtype, None] = None,
+    ) -> None:
+        super().__init__()
+        self.device = device
+        self.dtype = dtype
 
-        def forward(self, x: np.ndarray) -> Tensor:
-            return from_numpy(x, dtype=self.dtype, device=self.device)
+    def forward(self, x: np.ndarray) -> Tensor:
+        return numpy_to_tensor(x, dtype=self.dtype, device=self.device)
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/pad.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/pad.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Iterable, Union
 
 import torch
 from torch import Generator, Tensor, nn
-from torch.types import Number
+from torch.types import Device, Number
 
 from torchoutil.nn.functional.pad import (
     PadAlign,
     PadValue,
     pad_and_stack_rec,
     pad_dim,
     pad_dims,
@@ -118,15 +118,15 @@
     For more information, see :func:`~torchoutil.nn.functional.pad.pad_and_stack_rec`.
     """
 
     def __init__(
         self,
         pad_value: Number,
         *,
-        device: Union[str, torch.device, None] = None,
+        device: Device = None,
         dtype: Union[None, torch.dtype] = None,
     ) -> None:
         super().__init__()
         self.pad_value = pad_value
         self.device = device
         self.dtype = dtype
```

### Comparing `torchoutil-0.3.1/src/torchoutil/nn/modules/tensor.py` & `torchoutil-0.4.0/src/torchoutil/nn/modules/tensor.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """Module versions of tensor functions that do not already exists in PyTorch."""
 
 from typing import List, Optional, Union
 
 import torch
 from torch import Tensor, nn
 from torch.nn import functional as F
-from torch.types import Number
+from torch.types import Device, Number
 
 from torchoutil.nn.functional.get import get_device
 from torchoutil.utils import return_types
 from torchoutil.utils.collections import dump_dict
 
 
 class Reshape(nn.Module):
@@ -44,15 +44,15 @@
             return x.mean(dim=self.dim, keepdim=self.keepdim)
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 dim=self.dim,
             ),
-            ignore_none=True,
+            ignore_lst=(None,),
         )
 
 
 class Max(nn.Module):
     def __init__(
         self,
         dim: Optional[int],
@@ -291,15 +291,15 @@
         return x.item()
 
 
 class AsTensor(nn.Module):
     def __init__(
         self,
         *,
-        device: Union[str, torch.device, None] = None,
+        device: Device = None,
         dtype: Union[torch.dtype, None] = None,
     ) -> None:
         device = get_device(device)
         super().__init__()
         self.device = device
         self.dtype = dtype
 
@@ -308,15 +308,15 @@
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 device=self.device,
                 dtype=self.dtype,
             ),
-            ignore_none=True,
+            ignore_lst=(None,),
         )
 
 
 class Abs(nn.Module):
     def forward(self, x: Tensor) -> Tensor:
         return x.abs()
 
@@ -342,7 +342,82 @@
         self.return_zeros = return_zeros
 
     def forward(self, x: Tensor) -> Tensor:
         if self.return_zeros and not x.is_complex():
             return torch.zeros_like(x)
         else:
             return x.imag
+
+
+class Pow(nn.Module):
+    def __init__(self, exponent: Union[Number, Tensor]) -> None:
+        super().__init__()
+        self.exponent = exponent
+
+    def forward(self, x: Tensor) -> Tensor:
+        return x.pow(self.exponent)
+
+    def extra_repr(self) -> str:
+        return dump_dict(dict(exponent=self.exponent))
+
+
+class FFT(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        return torch.fft.fft(x)
+
+
+class IFFT(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        return torch.fft.ifft(x)
+
+
+class Log(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        return x.log()
+
+
+class Log10(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        return x.log10()
+
+
+class Log2(nn.Module):
+    def forward(self, x: Tensor) -> Tensor:
+        return x.log2()
+
+
+class Repeat(nn.Module):
+    def __init__(self, *repeats: int) -> None:
+        super().__init__()
+        self.repeats = repeats
+
+    def forward(self, x: Tensor) -> Tensor:
+        return x.repeat(self.repeats)
+
+    def extra_repr(self) -> str:
+        return dump_dict(dict(repeats=self.repeats))
+
+
+class RepeatInterleave(nn.Module):
+    def __init__(
+        self,
+        repeats: Union[int, Tensor],
+        dim: int,
+        output_size: Optional[int] = None,
+    ) -> None:
+        super().__init__()
+        self.repeats = repeats
+        self.dim = dim
+        self.output_size = output_size
+
+    def forward(self, x: Tensor) -> Tensor:
+        return x.repeat_interleave(self.repeats, self.dim, output_size=self.output_size)
+
+    def extra_repr(self) -> str:
+        return dump_dict(
+            dict(
+                repeats=self.repeats,
+                dim=self.dim,
+                output_size=self.output_size,
+            ),
+            ignore_lst=(None,),
+        )
```

### Comparing `torchoutil-0.3.1/src/torchoutil/optim/utils.py` & `torchoutil-0.4.0/src/torchoutil/optim/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 from torch import nn
 from torch.nn.parameter import Parameter
 from torch.optim.optimizer import Optimizer
 
 pylog = logging.getLogger(__name__)
 
@@ -33,15 +33,15 @@
 
 
 def create_params_groups_bias(
     model: Union[nn.Module, Iterable[Tuple[str, Parameter]]],
     weight_decay: float,
     skip_list: Optional[Iterable[str]] = (),
     verbose: int = 2,
-) -> List[Dict[str, Any]]:
+) -> List[Dict[str, Union[List[Parameter], float]]]:
     if isinstance(model, nn.Module):
         params = model.named_parameters()
     else:
         params = model
     del model
 
     decay: List[Parameter] = []
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/collections.py` & `torchoutil-0.4.0/src/torchoutil/utils/collections.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import copy
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
@@ -25,14 +26,24 @@
 V = TypeVar("V")
 W = TypeVar("W")
 
 KEY_MODES = ("same", "intersect", "union")
 KeyMode = Literal["intersect", "same", "union"]
 
 
+def sorted_dict(
+    x: Mapping[K, V],
+    /,
+    *,
+    key: Optional[Callable[[K], Any]] = None,
+    reverse: bool = False,
+) -> Dict[K, V]:
+    return {k: x[k] for k in sorted(x.keys(), key=key, reverse=reverse)}
+
+
 @overload
 def list_dict_to_dict_list(
     lst: Sequence[Mapping[K, V]],
     key_mode: Literal["intersect", "same"],
     default_val: Any = None,
 ) -> Dict[K, List[V]]:
     ...
@@ -63,16 +74,19 @@
         default_val: Default value of an element when key_mode is "union". defaults to None.
     """
     if len(lst) <= 0:
         return {}
 
     keys = set(lst[0].keys())
     if key_mode == "same":
-        if not all(keys == set(item.keys()) for item in lst[1:]):
-            raise ValueError(f"Invalid keys with {key_mode=}.")
+        invalids = [list(item.keys()) for item in lst[1:] if keys != set(item.keys())]
+        if len(invalids):
+            raise ValueError(
+                f"Invalid keys with {key_mode=}. (with {keys=} and {invalids=})"
+            )
     elif key_mode == "intersect":
         keys = intersect_lists([item.keys() for item in lst])
     elif key_mode == "union":
         keys = union_lists([item.keys() for item in lst])
     else:
         raise ValueError(
             f"Invalid argument key_mode={key_mode}. (expected one of {KEY_MODES})"
@@ -156,41 +170,42 @@
     for lst_i in lst_of_lst:
         out.update(dict.fromkeys(lst_i))
     out = list(out)
     return out
 
 
 def dump_dict(
-    dic: Mapping[str, Any],
+    dic: Mapping[str, T],
     /,
     join: str = ", ",
     fmt: str = "{key}={value}",
-    ignore_none: bool = False,
+    ignore_lst: Iterable[T] = (),
 ) -> str:
     """Dump dictionary to string."""
+    ignore_lst = dict.fromkeys(ignore_lst)
     result = join.join(
         fmt.format(key=key, value=value)
         for key, value in dic.items()
-        if not (value is None and ignore_none)
+        if value not in ignore_lst
     )
     return result
 
 
 def pass_filter(
-    name: T,
+    x: T,
     include: Optional[Iterable[T]] = None,
     exclude: Optional[Iterable[T]] = None,
 ) -> bool:
     """Returns True if name in include set and not in exclude set."""
     if include is not None and exclude is not None:
-        return (name in include) and (name not in exclude)
+        return (x in include) and (x not in exclude)
     if include is not None:
-        return name in include
+        return x in include
     elif exclude is not None:
-        return name not in exclude
+        return x not in exclude
     else:
         return True
 
 
 def filter_iterable(
     it: Iterable[T],
     include: Optional[Iterable[T]] = None,
@@ -237,23 +252,23 @@
     >>> dic = {
     ...     "a": 1,
     ...     "b": {
     ...         "a": 2,
     ...         "b": 10,
     ...     },
     ... }
-    >>> flat_dict(dic)
+    >>> flat_dict_of_dict(dic)
     ... {"a": 1, "b.a": 2, "b.b": 10}
     ```
 
     Example 2
     ---------
     ```
     >>> dic = {"a": ["hello", "world"], "b": 3}
-    >>> flat_dict(dic, flat_iterables=True)
+    >>> flat_dict_of_dict(dic, flat_iterables=True)
     ... {"a.0": "hello", "a.1": "world", "b": 3}
     ```
 
     Args:
         nested_dict: Nested mapping containing sub-mappings or iterables.
         sep: Separators between keys.
         flat_iterables: If True, flat iterable and use index as key.
@@ -274,15 +289,17 @@
                 v = {f"{k}{sep}{kv}": vv for kv, vv in v.items()}
                 output.update(v)
 
             elif overwrite or k not in output:
                 output[k] = v
 
             else:
-                raise ValueError(f"Ambiguous flatten dict with key '{k}'.")
+                raise ValueError(
+                    f"Ambiguous flatten dict with key '{k}'. (with value '{v}')"
+                )
         return output
 
     return _flat_dict_of_dict_impl(nested_dic)
 
 
 def unflat_dict_of_dict(dic: Mapping[str, Any], sep: str = ".") -> Dict[str, Any]:
     """Unflat a dictionary.
@@ -319,22 +336,25 @@
     output = {
         k: (unflat_dict_of_dict(v) if isinstance(v, Mapping) else v)
         for k, v in output.items()
     }
     return output
 
 
-def flat_list(lst: Iterable[Sequence[T]]) -> Tuple[List[T], List[int]]:
+def flat_list_of_list(lst: Iterable[Sequence[T]]) -> Tuple[List[T], List[int]]:
     """Return a flat version of the input list of sublists with each sublist size."""
-    flatten_lst = [element for sublst in lst for element in sublst]
+    flatten_lst = [elt for sublst in lst for elt in sublst]
     sizes = [len(sents) for sents in lst]
     return flatten_lst, sizes
 
 
-def unflat_list(flatten_lst: Sequence[T], sizes: Iterable[int]) -> List[List[T]]:
+def unflat_list_of_list(
+    flatten_lst: Sequence[T],
+    sizes: Iterable[int],
+) -> List[List[T]]:
     """Unflat a list to a list of sublists of given sizes."""
     lst = []
     start = 0
     stop = 0
     for count in sizes:
         stop += count
         lst.append(flatten_lst[start:stop])
@@ -375,7 +395,14 @@
         >>> lst_zipped = list(zip(lst1, lst2))
         >>> lst_zipped
         ... [(1, 5), (2, 6), (3, 7), (4, 8)]
         >>> unzip(lst_zipped)
         ... ([1, 2, 3, 4], [5, 6, 7, 8])
     """
     return tuple(map(list, zip(*lst)))
+
+
+def prod(x: Iterable[T], /, start: T = 1) -> T:
+    result = copy.copy(start)
+    for xi in x:
+        result = result * xi
+    return result
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/data/collate.py` & `torchoutil-0.4.0/src/torchoutil/utils/data/collate.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/data/dataloader.py` & `torchoutil-0.4.0/src/torchoutil/utils/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/data/dataset.py` & `torchoutil-0.4.0/src/torchoutil/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/data/split.py` & `torchoutil-0.4.0/src/torchoutil/utils/data/split.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import math
 from typing import Callable, Iterable, List, Optional, Union
 
 import torch
 from torch import Generator, Tensor
 
-from torchoutil.utils.collections import flat_list
+from torchoutil.utils.collections import flat_list_of_list
 
 
 def random_split(
     num_samples: int,
     lengths: Iterable[float],
     generator: Union[int, Generator, None] = None,
 ) -> List[List[int]]:
@@ -58,15 +58,15 @@
     for class_idx in range(num_classes):
         indices = torch.where(targets_indices.eq(class_idx))[0]
         indices = indices.tolist()
         indices_per_class.append(indices)
 
     indices_per_class = _shuffle_indices_per_class(indices_per_class, generator)
     splits = _split_indices_per_class(indices_per_class, lengths, math.floor)
-    flatten = [flat_list(split)[0] for split in splits]
+    flatten = [flat_list_of_list(split)[0] for split in splits]
     return flatten
 
 
 def _round_lengths(
     n: int,
     lengths: Iterable[Union[int, float]],
     round_fn: Callable[[float], int],
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/hdf/common.py` & `torchoutil-0.4.0/src/torchoutil/utils/hdf/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     return dict(zip(map(str, range(len(x))), x))
 
 
 def _dict_to_tuple(x: Dict[str, T]) -> Tuple[T, ...]:
     return tuple(x.values())
 
 
-class HDFAttributes(TypedDict):
+class HDFDatasetAttributes(TypedDict):
     creation_date: str
     source_dataset: str
     length: int
     metadata: str
     encoding: str
     info: str
     global_hash_value: int
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/hdf/dataset.py` & `torchoutil-0.4.0/src/torchoutil/utils/hdf/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from torchoutil.nn.functional.indices import get_inverse_perm
 from torchoutil.utils.collections import all_eq
 from torchoutil.utils.hdf.common import (
     HDF_ENCODING,
     HDF_STRING_DTYPE,
     HDF_VOID_DTYPE,
     SHAPE_SUFFIX,
-    HDFAttributes,
+    HDFDatasetAttributes,
     _dict_to_tuple,
 )
 from torchoutil.utils.type_checks import (
     is_iterable_bytes_list,
     is_iterable_int,
     is_iterable_str,
 )
@@ -132,15 +132,15 @@
 
     @property
     def all_columns(self) -> List[str]:
         """The name of all columns of the dataset."""
         return list(self.get_hdf_keys())
 
     @property
-    def attrs(self) -> HDFAttributes:
+    def attrs(self) -> HDFDatasetAttributes:
         return dict(self._hdf_file.attrs)  # type: ignore
 
     @property
     def metadata(self) -> str:
         return self.attrs.get("metadata", "")
 
     @property
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/hdf/pack.py` & `torchoutil-0.4.0/src/torchoutil/utils/hdf/pack.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,27 +23,26 @@
 import numpy as np
 import torch
 import tqdm
 from h5py import Dataset as HDFRawDataset
 from torch import Tensor, nn
 from torch.utils.data.dataloader import DataLoader
 
-from torchoutil.nn.functional.numpy import is_numpy_scalar
 from torchoutil.utils.collections import all_eq, unzip
 from torchoutil.utils.data.dataloader import get_auto_num_cpus
 from torchoutil.utils.data.dataset import SizedDatasetLike, TransformWrapper
 from torchoutil.utils.hdf.common import (
     HDF_ENCODING,
     HDF_STRING_DTYPE,
     HDF_VOID_DTYPE,
     SHAPE_SUFFIX,
     _tuple_to_dict,
 )
 from torchoutil.utils.hdf.dataset import HDFDataset
-from torchoutil.utils.type_checks import is_dict_str
+from torchoutil.utils.type_checks import is_dict_str, is_numpy_scalar
 
 pylog = logging.getLogger(__name__)
 
 T = TypeVar("T")
 U = TypeVar("U", bound=Union[int, float, str, Tensor, list])
 
 _HDF_SUPPORTED_DTYPES = (
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/dataset.py` & `torchoutil-0.4.0/src/torchoutil/utils/pack/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import json
 import logging
+import sys
 from pathlib import Path
 from typing import Any, Callable, Dict, Generic, List, Optional, TypeVar, Union
 
 import torch
 from torch.utils.data.dataset import Dataset
 
-from torchoutil.utils.pickle_dataset.common import (
+from torchoutil.utils.pack.common import (
     ATTRS_FNAME,
     ContentMode,
-    PickleAttributes,
+    PackedDatasetAttributes,
 )
 
 pylog = logging.getLogger(__name__)
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-class PickleDataset(Generic[T, U], Dataset[U]):
+class PackedDataset(Generic[T, U], Dataset[U]):
     def __init__(
         self,
         root: Union[str, Path],
         transform: Optional[Callable[[T], U]] = None,
         *,
         load_fn: Callable[..., Union[T, List[T]]] = torch.load,
         load_kwds: Optional[Dict[str, Any]] = None,
@@ -54,15 +55,15 @@
         self._attrs = {}
         self._fpaths = []
         self._cache = None
         self._cache_idx = None
         self._reload_data()
 
     @property
-    def attrs(self) -> PickleAttributes:
+    def attrs(self) -> PackedDatasetAttributes:
         return self._attrs  # type: ignore
 
     @property
     def content_mode(self) -> Optional[ContentMode]:
         return self._attrs.get("content_mode")
 
     @property
@@ -108,21 +109,44 @@
             item = batch[local_idx]
 
         return item
 
     def _reload_data(self) -> None:
         attrs_fpath = self._root.joinpath(ATTRS_FNAME)
 
-        if attrs_fpath.is_file():
-            with open(attrs_fpath, "r") as file:
-                attrs = json.load(file)
-        else:
+        if not attrs_fpath.is_file():
             raise FileNotFoundError(f"Cannot find attribute file '{str(attrs_fpath)}'.")
 
+        with open(attrs_fpath, "r") as file:
+            attrs = json.load(file)
+
+        # Disable check for python <= 3.8 because __required_keys__ does not exists in this version
+        if sys.version_info.major < 3 or (
+            sys.version_info.major == 3 and sys.version_info.minor <= 8
+        ):
+            missing = []
+        else:
+            missing = list(
+                set(PackedDatasetAttributes.__required_keys__).difference(attrs)
+            )
+
+        if len(missing) > 0:
+            raise RuntimeError(
+                f"Missing {len(missing)} keys in attribute file. (with {missing=})"
+            )
+
         content_dname = attrs["content_dname"]
         content_dpath = self._root.joinpath(content_dname)
 
         fnames = attrs["files"]
         fpaths = [content_dpath.joinpath(fname) for fname in fnames]
 
         self._attrs = attrs
         self._fpaths = fpaths
+
+    @classmethod
+    def is_pickle_root(cls, root: Union[str, Path]) -> bool:
+        try:
+            PackedDataset(root)
+            return True
+        except (FileNotFoundError, RuntimeError):
+            return False
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/pickle_dataset/pack.py` & `torchoutil-0.4.0/src/torchoutil/utils/pack/pack.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,67 +2,90 @@
 # -*- coding: utf-8 -*-
 
 import datetime
 import json
 import logging
 import math
 import shutil
-from dataclasses import asdict, is_dataclass
 from pathlib import Path
 from typing import Callable, List, Literal, Optional, TypeVar, Union
 
 import torch
 from torch import nn
 from torch.utils.data.dataloader import DataLoader
 
 from torchoutil.utils.data.dataloader import get_auto_num_cpus
 from torchoutil.utils.data.dataset import SizedDatasetLike, TransformWrapper
-from torchoutil.utils.pickle_dataset.common import (
-    ATTRS_FNAME,
-    CONTENT_DNAME,
-    ContentMode,
-)
-from torchoutil.utils.pickle_dataset.dataset import PickleDataset
-from torchoutil.utils.type_checks import is_mapping_str
+from torchoutil.utils.pack.common import ATTRS_FNAME, CONTENT_DNAME, ContentMode
+from torchoutil.utils.pack.dataset import PackedDataset
+from torchoutil.utils.packaging import _TQDM_AVAILABLE
+from torchoutil.utils.saving.common import to_builtin
+
+if _TQDM_AVAILABLE:
+    import tqdm
+
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 pylog = logging.getLogger(__name__)
 
 
 @torch.inference_mode()
-def pack_to_pickle(
+def pack_dataset(
     dataset: SizedDatasetLike[T],
     root: Union[str, Path],
     pre_transform: Optional[Callable[[T], U]] = None,
     batch_size: int = 32,
     num_workers: Union[int, Literal["auto"]] = "auto",
     overwrite: bool = False,
     content_mode: ContentMode = "item",
     custom_file_fmt: Union[None, str, Callable[[int], str]] = None,
     save_fn: Callable[[Union[U, List[U]], Path], None] = torch.save,
-) -> PickleDataset[U, U]:
+    subdir_size: Optional[int] = 100,
+    verbose: int = 0,
+) -> PackedDataset[U, U]:
     """Pack a dataset to pickle files.
 
+    Here is an example how files are stored on disk for a dataset containing 1000 items:
+
+    .. code-block:: text
+        :caption:  Dataset folder tree example
+
+        {root}
+        ├── attributes.json
+        └── data
+            ├── 0
+            |   └── 100 pt files
+            ├── 1
+            |   └── 100 pt files
+            ├── ...
+            |   └── ...
+            └── 9
+                └── 100 pt files
+
     Args:
         dataset: Dataset-like to pack.
         root: Directory to store pickled data.
         pre_transform: Transform to apply to each item before saving. defaults to None.
         batch_size: Batch size used by the dataloader. defaults to 32.
         num_workers: Number of workers used by the dataloader. defaults to "auto".
         overwrite: If True, overwrite all data in root directory. defaults to False.
         content_mode: Specify how the data should be stored.
             If "item", each dataset item will be stored in a separate file.
             If "batch", each dataset item will be stored in a batch file of size batch_size.
         custom_file_fmt: Custom file format.
             If None, defaults to "{{i:0{num_digits}d}}.pt".
             defaults to None.
         save_fn: Custom save function to save an item or a batch. defaults to torch.save.
+        subdir_size: Optional number of files per folder.
+            Using None will disable subdir an put all files in data/ folder.
+            defaults to 100.
+        verbose: Verbose level during packing. Higher value means more messages. defaults to 0.
     """
 
     # Check inputs
     if not isinstance(dataset, SizedDatasetLike):
         raise TypeError(
             f"Cannot pack to hdf a non-sized-dataset '{dataset.__class__.__name__}'."
         )
@@ -115,71 +138,75 @@
     elif isinstance(custom_file_fmt, str):
         file_fmt = custom_file_fmt.format
     else:
         file_fmt = custom_file_fmt
 
     fnames = [file_fmt(i) for i in range(num_files)]
 
+    if subdir_size is not None and len(fnames) > subdir_size:
+        num_subdirs = math.ceil(len(fnames) / subdir_size)
+        num_digits = math.ceil(math.log10(num_subdirs))
+        dir_fmt = f"{{:0{num_digits}d}}".format
+        sub_dnames = [dir_fmt(i) for i in range(num_subdirs)]
+        fnames = [
+            str(Path(sub_dnames[i // subdir_size]).joinpath(fname))
+            for i, fname in enumerate(fnames)
+        ]
+
+    fpaths = [content_dpath.joinpath(fname) for fname in fnames]
+
+    if custom_file_fmt is not None or subdir_size is not None:
+        unique_parents = dict.fromkeys(fpath.parent for fpath in fpaths)
+        for parent in unique_parents:
+            parent.mkdir(parents=True, exist_ok=True)
+
+    if _TQDM_AVAILABLE and verbose >= 1:
+        loader = tqdm.tqdm(loader)
+
     i = 0
     for batch_lst in loader:
         if content_mode == "item":
             for item in batch_lst:
-                fname = fnames[i]
-                fpath = content_dpath.joinpath(fname)
-                if custom_file_fmt is not None:
-                    fpath.parent.mkdir(parents=True, exist_ok=True)
+                fpath = fpaths[i]
                 save_fn(item, fpath)
                 i += 1
 
         elif content_mode == "batch":
-            fname = fnames[i]
-            fpath = content_dpath.joinpath(fname)
-            if custom_file_fmt is not None:
-                fpath.parent.mkdir(parents=True, exist_ok=True)
+            fpath = fpaths[i]
             save_fn(batch_lst, fpath)
             i += 1
 
         else:
             raise ValueError(f"Invalid argument {content_mode=}.")
 
     if hasattr(dataset, "info"):
         info = dataset.info  # type: ignore
-        if is_dataclass(info):
-            info = asdict(info)
-        elif is_mapping_str(info):
-            info = dict(info.items())  # type: ignore
-        else:
-            info = {}
+        info = to_builtin(info)
     else:
         info = {}
 
     if hasattr(dataset, "attrs"):
         source_attrs = dataset.attrs  # type: ignore
-        if is_dataclass(source_attrs):
-            info = asdict(source_attrs)
-        elif is_mapping_str(source_attrs):
-            source_attrs = dict(source_attrs.items())  # type: ignore
-        else:
-            pylog.warning(f"Ignore source attributes type {type(source_attrs)}.")
-            source_attrs = {}
+        source_attrs = to_builtin(source_attrs)
     else:
         source_attrs = {}
 
     attributes = {
         "source_dataset": wrapped.unwrap().__class__.__name__,
         "length": len(wrapped),
         "creation_date": creation_date,
         "batch_size": batch_size,
         "content_mode": content_mode,
         "content_dname": CONTENT_DNAME,
+        "subdir_size": subdir_size,
         "info": info,
         "source_attrs": source_attrs,
         "num_files": len(fnames),
         "files": fnames,
     }
 
     attrs_fpath = root.joinpath(ATTRS_FNAME)
     with open(attrs_fpath, "w") as file:
         json.dump(attributes, file, indent="\t")
 
-    pickle_dataset = PickleDataset(root)
-    return pickle_dataset
+    pack = PackedDataset(root)
+    return pack
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/return_types.py` & `torchoutil-0.4.0/src/torchoutil/utils/return_types.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/saving/yaml_io.py` & `torchoutil-0.4.0/src/torchoutil/utils/saving/csv_io.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,96 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import os
-from argparse import Namespace
-from dataclasses import asdict
+import csv
+import io
 from pathlib import Path
-from typing import Any, Mapping, Union
+from typing import Any, Dict, List, Literal, Mapping, Sequence, Union, overload
 
-from torchoutil.utils.packaging import _OMEGACONF_AVAILABLE, _YAML_AVAILABLE
+from torchoutil.utils.collections import dict_list_to_list_dict, list_dict_to_dict_list
 from torchoutil.utils.saving.common import to_builtin
-from torchoutil.utils.type_checks import DataclassInstance, NamedTupleInstance
 
-if _YAML_AVAILABLE:
-    import yaml
-else:
-    raise ImportError(
-        "Cannot use to_yaml python module since pyyaml package is not installed."
-    )
 
-if _OMEGACONF_AVAILABLE:
-    from omegaconf import DictConfig, OmegaConf
-
-
-def save_to_yaml(
-    data: Mapping[str, Any] | Namespace | DataclassInstance | NamedTupleInstance,
+def to_csv(
+    data: Union[Sequence[Mapping[str, Any]], Mapping[str, Sequence[Any]]],
     fpath: Union[str, Path, None],
     *,
     overwrite: bool = True,
     to_builtins: bool = False,
     make_parents: bool = True,
-    resolve: bool = False,
-    sort_keys: bool = False,
-    indent: int | None = None,
-    **kwargs,
+    **csv_writer_kwargs,
 ) -> str:
-    if resolve and not _OMEGACONF_AVAILABLE:
-        raise ValueError(
-            "Cannot resolve config for yaml without omegaconf package."
-            "Please use resolve=False or install omegaconf with 'pip install torchoutil[extras]'."
-        )
+    if isinstance(data, Mapping):
+        data = dict_list_to_list_dict(data)
+    else:
+        data = [dict(data_i.items()) for data_i in data]
+
+    if len(data) <= 0:
+        raise ValueError(f"Invalid argument {data=}. (found empty iterable)")
 
     if fpath is not None:
         fpath = Path(fpath).resolve().expanduser()
         if not overwrite and fpath.exists():
             raise FileExistsError(f"File {fpath} already exists.")
         elif make_parents:
-            os.makedirs(fpath.parent, exist_ok=True)
-
-    if isinstance(data, Namespace):
-        data = data.__dict__
-
-    elif isinstance(data, DataclassInstance):
-        data = asdict(data)
-
-    elif isinstance(data, NamedTupleInstance):
-        data = data._asdict()
-
-    elif _OMEGACONF_AVAILABLE and isinstance(data, DictConfig):
-        data = OmegaConf.to_container(data, resolve=False)  # type: ignore
+            fpath.parent.mkdir(parents=True, exist_ok=True)
 
     if to_builtins:
         data = to_builtin(data)
 
-    if _OMEGACONF_AVAILABLE and resolve:
-        data_cfg = OmegaConf.create(data)  # type: ignore
-        data = OmegaConf.to_container(data_cfg, resolve=True)  # type: ignore
+    fieldnames = list(data[0].keys())  # type: ignore
+    file = io.StringIO()
+    writer = csv.DictWriter(file, fieldnames, **csv_writer_kwargs)
+    writer.writeheader()
+    writer.writerows(data)  # type: ignore
+    content = file.getvalue()
+    file.close()
 
-    content = yaml.dump(data, sort_keys=sort_keys, indent=indent, **kwargs)
     if fpath is not None:
-        fpath.write_text(content, encoding="utf-8")
+        fpath.write_text(content)
     return content
 
 
-def load_yaml(fpath: Union[str, Path]) -> Any:
+@overload
+def load_csv(
+    fpath: Union[str, Path],
+    /,
+    *,
+    orient: Literal["dict"],
+    **csv_reader_kwargs,
+) -> Dict[str, List[Any]]:
+    ...
+
+
+@overload
+def load_csv(
+    fpath: Union[str, Path],
+    /,
+    *,
+    orient: Literal["list", "dict"] = "list",
+    **csv_reader_kwargs,
+) -> List[Dict[str, Any]]:
+    ...
+
+
+def load_csv(
+    fpath: Union[str, Path],
+    /,
+    *,
+    orient: Literal["list", "dict"] = "list",
+    **csv_reader_kwargs,
+) -> Union[List[Dict[str, Any]], Dict[str, List[Any]]]:
     with open(fpath, "r") as file:
-        data = yaml.safe_load(file)
+        reader = csv.DictReader(file, **csv_reader_kwargs)
+        data = list(reader)
+
+    if orient == "dict":
+        data = list_dict_to_dict_list(data, key_mode="same")
+    elif orient == "list":
+        pass
+    else:
+        ORIENT_VALUES = ("list", "dict")
+        raise ValueError(
+            f"Invalid argument {orient=}. (expected one of {ORIENT_VALUES})"
+        )
+
     return data
```

### Comparing `torchoutil-0.3.1/src/torchoutil/utils/tensorboard.py` & `torchoutil-0.4.0/src/torchoutil/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/src/torchoutil.egg-info/PKG-INFO` & `torchoutil-0.4.0/src/torchoutil.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchoutil
-Version: 0.3.1
+Version: 0.4.0
 Summary: Collection of functions and modules to help development in PyTorch.
 Author-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Labbeti
         
@@ -83,96 +83,98 @@
 
 To check if the package is installed and show the package version, you can use the following command:
 ```bash
 torchoutil-info
 ```
 
 
-## Usage
+## Examples
 
-### Batch of padded sequences
+### Multilabel conversions
 ```python
 import torch
-from torchoutil import masked_mean
+from torchoutil import probs_to_name
 
-x = torch.as_tensor([1, 2, 3, 4])
-mask = torch.as_tensor([True, True, False, False])
-result = masked_mean(x, mask)
-# result contains the mean of the values marked as True: 1.5
+probs = torch.as_tensor([[0.9, 0.1], [0.4, 0.6]])
+names = probs_to_name(probs, idx_to_name={0: "Cat", 1: "Dog"})
+# ["Cat", "Dog"]
+```
+
+```python
+import torch
+from torchoutil import multihot_to_indices
+
+multihot = torch.as_tensor([[1, 0, 0], [0, 1, 1], [0, 0, 0]])
+indices = multihot_to_indices(multihot)
+# [[0], [1, 2], []]
 ```
 
+### Masked operations
+
 ```python
 import torch
 from torchoutil import lengths_to_non_pad_mask
 
 x = torch.as_tensor([3, 1, 2])
 mask = lengths_to_non_pad_mask(x, max_len=4)
 # Each row i contains x[i] True values for non-padding mask
 # tensor([[True, True, True, False],
 #         [True, False, False, False],
 #         [True, True, False, False]])
 ```
 
-### Multilabel conversions
-```python
-import torch
-from torchoutil import probs_to_names
-
-probs = torch.as_tensor([[0.9, 0.1], [0.6, 0.9]])
-names = probs_to_names(probs, threshold=0.5, idx_to_name={0: "Cat", 1: "Dog"})
-# [["Cat"], ["Cat", "Dog"]]
-```
-
 ```python
 import torch
-from torchoutil import multihot_to_indices
+from torchoutil import masked_mean
 
-multihot = torch.as_tensor([[1, 0, 0], [0, 1, 1], [0, 0, 0]])
-indices = multihot_to_indices(multihot)
-# [[0], [1, 2], []]
+x = torch.as_tensor([1, 2, 3, 4])
+mask = torch.as_tensor([True, True, False, False])
+result = masked_mean(x, mask)
+# result contains the mean of the values marked as True: 1.5
 ```
 
-### Easely pre-compute transforms
+### Pre-compute datasets to pickle or HDF files
 
-Here is an example of pre-computing spectrograms of torchaudio `SPEECHCOMMANDS` dataset, using `pack_to_pickle` function:
+Here is an example of pre-computing spectrograms of torchaudio `SPEECHCOMMANDS` dataset, using `pack_to_custom` function:
 
 ```python
 from torch import nn
 from torchaudio.datasets import SPEECHCOMMANDS
 from torchaudio.transforms import Spectrogram
-from torchoutil.utils.pickle_dataset import pack_to_pickle
+from torchoutil.utils.pack import pack_to_custom
 
 speech_commands_root = "path/to/speech_commands"
-pickle_root = "path/to/pickle_dataset"
+packed_root = "path/to/packed_dataset"
 
 dataset = SPEECHCOMMANDS(speech_commands_root, download=True, subset="validation")
+# dataset[0] is a tuple, contains waveform and other metadata
 
 class MyTransform(nn.Module):
     def __init__(self) -> None:
         super().__init__()
         self.spectrogram_extractor = Spectrogram()
 
     def forward(self, item):
         waveform = item[0]
         spectrogram = self.spectrogram_extractor(waveform)
         return (spectrogram,) + item[1:]
 
-pack_to_pickle(dataset, pickle_root, MyTransform())
+pack_to_custom(dataset, packed_root, MyTransform())
 ```
 
-Then you can load the pre-computed dataset using `PickleDataset`:
+Then you can load the pre-computed dataset using `PackedDataset`:
 ```python
-from torchoutil.utils.pickle_dataset import PickleDataset
+from torchoutil.utils.pack import PackedDataset
 
-pickle_root = "path/to/pickle_dataset"
-pickle_dataset = PickleDataset(pickle_root)
-pickle_dataset[0]  # == first transformed item, i.e. transform(dataset[0])
+packed_root = "path/to/packed_dataset"
+packed_dataset = PackedDataset(packed_root)
+packed_dataset[0]  # == first transformed item, i.e. transform(dataset[0])
 ```
 
-### ...and more tensor manipulations!
+### Other tensors manipulations!
 
 ```python
 import torch
 from torchoutil import insert_at_indices
 
 x = torch.as_tensor([1, 2, 3, 4])
 result = insert_at_indices(x, indices=[0, 2], values=5)
@@ -188,19 +190,19 @@
 
 x1 = torch.rand(10)
 x2 = x1[perm]
 x3 = x2[inv_perm]
 # inv_perm are indices that allow us to get x3 from x2, i.e. x1 == x3 here
 ```
 
-## Extras
+## Extras requirements
 `torchoutil` also provides additional modules when some specific package are already installed in your environment.
 All extras can be installed with `pip install torchoutil[extras]`
 
 - If `tensorboard` is installed, the function `load_event_file` can be used. It is useful to load manually all data contained in an tensorboard event file.
-- If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
+- If `numpy` is installed, the classes `NumpyToTensor` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
 - If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF files, and supports variable-length sequences of data.
 
 
 ## Contact
 Maintainer:
 - [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `torchoutil-0.3.1/src/torchoutil.egg-info/SOURCES.txt` & `torchoutil-0.4.0/src/torchoutil.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,23 @@
 src/torchoutil/nn/functional/pad.py
 src/torchoutil/nn/functional/transform.py
 src/torchoutil/nn/modules/__init__.py
 src/torchoutil/nn/modules/activation.py
 src/torchoutil/nn/modules/crop.py
 src/torchoutil/nn/modules/layer.py
 src/torchoutil/nn/modules/mask.py
+src/torchoutil/nn/modules/mixins.py
 src/torchoutil/nn/modules/multiclass.py
 src/torchoutil/nn/modules/multilabel.py
 src/torchoutil/nn/modules/numpy.py
 src/torchoutil/nn/modules/pad.py
 src/torchoutil/nn/modules/tensor.py
 src/torchoutil/nn/modules/transform.py
-src/torchoutil/nn/modules/typed.py
 src/torchoutil/optim/__init__.py
+src/torchoutil/optim/schedulers.py
 src/torchoutil/optim/utils.py
 src/torchoutil/utils/__init__.py
 src/torchoutil/utils/collections.py
 src/torchoutil/utils/log_utils.py
 src/torchoutil/utils/packaging.py
 src/torchoutil/utils/return_types.py
 src/torchoutil/utils/tensorboard.py
@@ -56,31 +57,33 @@
 src/torchoutil/utils/data/dataloader.py
 src/torchoutil/utils/data/dataset.py
 src/torchoutil/utils/data/split.py
 src/torchoutil/utils/hdf/__init__.py
 src/torchoutil/utils/hdf/common.py
 src/torchoutil/utils/hdf/dataset.py
 src/torchoutil/utils/hdf/pack.py
-src/torchoutil/utils/pickle_dataset/__init__.py
-src/torchoutil/utils/pickle_dataset/common.py
-src/torchoutil/utils/pickle_dataset/dataset.py
-src/torchoutil/utils/pickle_dataset/pack.py
+src/torchoutil/utils/pack/__init__.py
+src/torchoutil/utils/pack/common.py
+src/torchoutil/utils/pack/dataset.py
+src/torchoutil/utils/pack/pack.py
 src/torchoutil/utils/saving/__init__.py
 src/torchoutil/utils/saving/common.py
 src/torchoutil/utils/saving/csv_io.py
 src/torchoutil/utils/saving/yaml_io.py
 tests/test_hub.py
 tests/test_nn_functional_crop.py
 tests/test_nn_functional_indices.py
 tests/test_nn_functional_mask.py
 tests/test_nn_functional_multiclass.py
 tests/test_nn_functional_multilabel.py
 tests/test_nn_functional_others.py
 tests/test_nn_functional_pad.py
 tests/test_nn_functional_transform.py
 tests/test_nn_modules.py
+tests/test_nn_modules_mixins.py
+tests/test_nn_modules_multiclass.py
 tests/test_nn_modules_multilabel.py
 tests/test_readme.py
 tests/test_utils_collections.py
 tests/test_utils_hdf.py
-tests/test_utils_pickle.py
+tests/test_utils_pack.py
 tests/test_utils_type_checks.py
```

### Comparing `torchoutil-0.3.1/tests/test_hub.py` & `torchoutil-0.4.0/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/tests/test_nn_functional_indices.py` & `torchoutil-0.4.0/tests/test_nn_functional_indices.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/tests/test_nn_functional_mask.py` & `torchoutil-0.4.0/tests/test_nn_functional_mask.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/tests/test_nn_functional_multiclass.py` & `torchoutil-0.4.0/tests/test_nn_functional_multiclass.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 # -*- coding: utf-8 -*-
 
 import unittest
 from unittest import TestCase
 
 import torch
 
-from torchoutil.nn.functional.multiclass import indices_to_onehot, onehot_to_indices
+from torchoutil.nn.functional.multiclass import index_to_onehot, onehot_to_index
 
 
 class TestMulticlass(TestCase):
-    def test_indices_to_onehot_1(self) -> None:
+    def test_index_to_onehot_1(self) -> None:
         indices = torch.as_tensor([[0, 2, 1], [0, 0, 2]])
         expected = torch.as_tensor(
             [[[1, 0, 0], [0, 0, 1], [0, 1, 0]], [[1, 0, 0], [1, 0, 0], [0, 0, 1]]],
             dtype=torch.bool,
         )
-        result = indices_to_onehot(indices, 3)
+        result = index_to_onehot(indices, 3)
         assert torch.equal(result, expected)
 
-    def test_indices_to_onehot_2(self) -> None:
+    def test_index_to_onehot_2(self) -> None:
         indices = torch.as_tensor([[0, -1, 1], [0, 0, 2], [-1, -1, -1]])
         expected = torch.as_tensor(
             [
                 [[1, 0, 0], [0, 0, 0], [0, 1, 0]],
                 [[1, 0, 0], [1, 0, 0], [0, 0, 1]],
                 [[0, 0, 0], [0, 0, 0], [0, 0, 0]],
             ],
             dtype=torch.bool,
         )
-        result = indices_to_onehot(indices, 3, padding_idx=-1)
+        result = index_to_onehot(indices, 3, padding_idx=-1)
         assert torch.equal(result, expected)
 
-    def test_onehot_to_indices_3d(self) -> None:
+    def test_onehot_to_index_3d(self) -> None:
         onehot = torch.as_tensor([[[0, 1, 0], [1, 0, 0]], [[0, 0, 1], [0, 0, 1]]])
         expected = [[1, 0], [2, 2]]
-        result = onehot_to_indices(onehot)
+        result = onehot_to_index(onehot)
         assert result == expected
 
-    def test_indices_to_onehot_3d(self) -> None:
+    def test_index_to_onehot_3d(self) -> None:
         indices = [[1, 0], [2, 2]]
         expected = torch.as_tensor(
             [[[0, 1, 0], [1, 0, 0]], [[0, 0, 1], [0, 0, 1]]]
         ).bool()
-        result = indices_to_onehot(indices, 3)
+        result = index_to_onehot(indices, 3)
         assert torch.equal(result, expected)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.3.1/tests/test_nn_functional_multilabel.py` & `torchoutil-0.4.0/tests/test_nn_functional_multilabel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import unittest
-
 from unittest import TestCase
 
 import torch
 
 from torchoutil.nn.functional.get import get_device
 from torchoutil.nn.functional.multilabel import (
     indices_to_multihot,
@@ -56,30 +55,30 @@
         num_classes = probs.shape[-1]
         idx_to_name = dict(zip(range(num_classes), map(str, range(num_classes))))
         result = probs_to_names(probs, threshold=0.5, idx_to_name=idx_to_name)
 
         self.assertListEqual(result, expected_names)
 
     def test_convert_multihot(self) -> None:
-        num_samples = int(torch.randint(0, 20, ()).item())
+        num_samples = int(torch.randint(1, 20, ()).item())
         num_classes = int(torch.randint(1, 20, ()).item())
         threshold = torch.rand(())
         idx_to_name = dict(zip(range(num_classes), map(str, range(num_classes))))
 
         probs_1 = torch.rand(num_samples, num_classes)
         multihot_1 = probs_1.ge(threshold)
 
         indices_1 = multihot_to_indices(multihot_1)
         names_1 = indices_to_names(indices_1, idx_to_name)
         multihot_2 = names_to_multihot(names_1, idx_to_name)
 
         names_2 = multihot_to_names(multihot_2, idx_to_name)
         indices_2 = names_to_indices(names_2, idx_to_name)
 
-        self.assertTrue(torch.equal(multihot_1, multihot_2))
+        assert torch.equal(multihot_1, multihot_2), f"{multihot_1=} ; {multihot_2=}"
         self.assertListEqual(names_1, names_2)
         self.assertListEqual(indices_1, indices_2)
 
     def test_ints_to_multihots(self) -> None:
         device = get_device()
         ints = torch.as_tensor([[0, 1, 1]], device=device)
         num_classes = 5
@@ -108,10 +107,49 @@
             ints, num_classes, dtype=torch.int, device=device
         )
 
         self.assertListEqual(ints, expected_ints)
         self.assertEqual(multihots.shape, new_multihots.shape)
         self.assertTrue(multihots.eq(new_multihots).all())
 
+    def test_empty_case_1(self) -> None:
+        num_samples = 0
+        num_classes = 5
+
+        multihot = torch.rand(num_samples, num_classes).ge(0.5)
+        with self.assertRaises(ValueError):
+            multihot_to_indices(multihot)
+
+        indices = torch.empty(0, 5)
+        with self.assertRaises(ValueError):
+            indices_to_multihot(indices, num_classes)
+
+    def test_empty_case_2(self) -> None:
+        num_samples = 5
+        num_classes = 0
+        expected = [[], [], [], [], []]
+
+        multihot = torch.rand(num_samples, num_classes).ge(0.5)
+
+        result_1 = multihot_to_indices(multihot)
+        assert result_1 == expected
+
+        result_2 = indices_to_multihot(expected, num_classes)
+        assert torch.equal(result_2, multihot)
+
+    def test_empty_case_3(self) -> None:
+        num_steps = 3
+        num_samples = 0
+        num_classes = 5
+
+        multihot = torch.rand(num_steps, num_samples, num_classes).ge(0.5)
+
+        with self.assertRaises(ValueError):
+            multihot_to_indices(multihot)
+
+        indices = [torch.empty(0, 5) for _ in range(num_steps)]
+        with self.assertRaises(ValueError):
+            indices_to_multihot(indices, num_classes)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.3.1/tests/test_nn_functional_pad.py` & `torchoutil-0.4.0/tests/test_nn_functional_pad.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.3.1/tests/test_nn_functional_transform.py` & `torchoutil-0.4.0/tests/test_nn_functional_transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # -*- coding: utf-8 -*-
 
 import unittest
 from unittest import TestCase
 
 import torch
 
-from torchoutil.nn.functional.transform import repeat_interleave_nd, resample_nearest
+from torchoutil.nn.functional.transform import (
+    repeat_interleave_nd,
+    resample_nearest_rates,
+)
 
 
 class TestRepeat(TestCase):
     def test_example_1(self) -> None:
         x = torch.as_tensor([[0, 1, 2, 3], [4, 5, 6, 7]])
         result = repeat_interleave_nd(x, repeats=2, dim=0)
         expected = torch.as_tensor(
@@ -18,21 +21,21 @@
         )
         assert torch.equal(result, expected)
 
 
 class TestResampleNearest(TestCase):
     def test_example_1(self) -> None:
         x = torch.arange(10, 20)
-        result = resample_nearest(x, 0.5)
+        result = resample_nearest_rates(x, 0.5)
         expected = torch.as_tensor([10, 12, 14, 16, 18])
         assert torch.equal(result, expected)
 
     def test_example_2(self) -> None:
         x = torch.arange(10, 20)
-        result = resample_nearest(x, 2)
+        result = resample_nearest_rates(x, 2)
         expected = torch.as_tensor(
             [
                 10,
                 10,
                 11,
                 11,
                 12,
@@ -53,14 +56,14 @@
                 19,
             ]
         )
         assert torch.equal(result, expected)
 
     def test_example_3(self) -> None:
         x = torch.stack([torch.arange(10, 20), torch.arange(20, 30)])
-        result = resample_nearest(x, 0.5)
+        result = resample_nearest_rates(x, 0.5)
         expected = torch.as_tensor([[10, 12, 14, 16, 18], [20, 22, 24, 26, 28]])
         assert torch.equal(result, expected)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.3.1/tests/test_nn_modules_multilabel.py` & `torchoutil-0.4.0/tests/test_nn_modules_multilabel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import unittest
 from unittest import TestCase
 
 import torch
-from torch import Tensor
 
+from torchoutil.nn.modules.mixins import ESequential
 from torchoutil.nn.modules.multilabel import (
     IndicesToMultihot,
     IndicesToNames,
     MultihotToIndices,
     MultihotToNames,
     NamesToIndices,
     NamesToMultihot,
 )
-from torchoutil.nn.modules.typed import TSequential
 
 
 class TestMultilabel(TestCase):
     def test_example_1(self) -> None:
-        num_samples = int(torch.randint(0, 20, ()).item())
-        num_classes = int(torch.randint(1, 20, ()).item())
-        threshold = torch.rand(())
-        idx_to_name = dict(zip(range(num_classes), map(str, range(num_classes))))
-
-        multihot = torch.rand(num_samples, num_classes).ge(threshold)
-
-        # dummy pipeline to convert labels multiple times
-        pipeline = TSequential[Tensor, Tensor](
-            MultihotToIndices(),
-            IndicesToNames(idx_to_name),
-            NamesToMultihot(idx_to_name),
-            MultihotToNames(idx_to_name),
-            NamesToIndices(idx_to_name),
-            IndicesToMultihot(num_classes),
-        )
-        result = pipeline(multihot)
-        self.assertTrue(torch.equal(multihot, result))
+        for _ in range(10):
+            num_steps = int(torch.randint(1, 2, ()).item())
+            num_samples = int(torch.randint(1, 2, ()).item())
+            num_classes = int(torch.randint(1, 20, ()).item())
+            threshold = torch.rand(())
+            idx_to_name = dict(zip(range(num_classes), map(str, range(num_classes))))
+
+            multihot = torch.rand(num_steps, num_samples, num_classes).ge(threshold)
+
+            # dummy pipeline to convert labels multiple times
+            pipeline = ESequential(
+                MultihotToIndices(),
+                IndicesToNames(idx_to_name),
+                NamesToMultihot(idx_to_name),
+                MultihotToNames(idx_to_name),
+                NamesToIndices(idx_to_name),
+                IndicesToMultihot(num_classes),
+            )
+            result = pipeline(multihot)
+
+            assert torch.equal(multihot, result), f"{multihot.shape=}"
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.3.1/tests/test_readme.py` & `torchoutil-0.4.0/tests/test_readme.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,68 +8,77 @@
 
 from torchoutil import (
     get_inverse_perm,
     insert_at_indices,
     lengths_to_non_pad_mask,
     masked_mean,
     multihot_to_indices,
+    probs_to_name,
     probs_to_names,
 )
 
 
 class TestReadme(TestCase):
     def test_masked_mean_example(self) -> None:
         x = torch.as_tensor([1, 2, 3, 4])
         mask = torch.as_tensor([True, True, False, False])
         result = masked_mean(x, mask)
         # result contains the mean of the values marked as True: 1.5
-
         result = result.item()
-        self.assertEqual(result, 1.5)
+
+        assert result == 1.5
 
     def test_lengths_to_non_pad_mask_example(self) -> None:
         x = torch.as_tensor([3, 1, 2])
         pad_mask = lengths_to_non_pad_mask(x, max_len=4)
         expected = torch.as_tensor(
             [
                 [True, True, True, False],
                 [True, False, False, False],
                 [True, True, False, False],
             ]
         )
 
-        self.assertTrue(torch.equal(pad_mask, expected))
+        assert torch.equal(pad_mask, expected)
+
+    def test_probs_to_name_example(self) -> None:
+        probs = torch.as_tensor([[0.9, 0.1], [0.4, 0.6]])
+        names = probs_to_name(probs, idx_to_name={0: "Cat", 1: "Dog"})
+        expected = ["Cat", "Dog"]
+
+        assert names == expected
 
     def test_probs_to_names_example(self) -> None:
         probs = torch.as_tensor([[0.9, 0.1], [0.6, 0.9]])
         names = probs_to_names(probs, threshold=0.5, idx_to_name={0: "Cat", 1: "Dog"})
         expected = [["Cat"], ["Cat", "Dog"]]
 
-        self.assertListEqual(names, expected)
+        assert names == expected
 
     def test_multihot_to_indices_example(self) -> None:
         multihot = torch.as_tensor([[1, 0, 0], [0, 1, 1], [0, 0, 0]])
         indices = multihot_to_indices(multihot)
         expected = [[0], [1, 2], []]
 
-        self.assertListEqual(indices, expected)
+        assert indices == expected
 
     def test_insert_at_indices_example(self) -> None:
         x = torch.as_tensor([1, 2, 3, 4])
         result = insert_at_indices(x, [0, 2], 5)
         expected = torch.as_tensor([5, 1, 2, 5, 3, 4])
-        self.assertTrue(torch.equal(result, expected))
+
+        assert torch.equal(result, expected)
 
     def test_get_inverse_perm_example(self) -> None:
         perm = torch.randperm(10)
         inv_perm = get_inverse_perm(perm)
 
         x1 = torch.rand(10)
         x2 = x1[perm]
         x3 = x2[inv_perm]
         # inv_perm are indices that allow us to get x1 from x3, i.e. x1 == x3 here
 
-        self.assertTrue(torch.equal(x1, x3))
+        assert torch.equal(x1, x3)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.3.1/tests/test_utils_collections.py` & `torchoutil-0.4.0/tests/test_utils_collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 import random
 import unittest
 from unittest import TestCase
 
 from torchoutil.utils.collections import (
     flat_dict_of_dict,
-    flat_list,
+    flat_list_of_list,
     intersect_lists,
     list_dict_to_dict_list,
     unflat_dict_of_dict,
-    unflat_list,
+    unflat_list_of_list,
 )
 from torchoutil.utils.type_checks import is_list_list_str, is_list_str
 
 
 class TestFlatDict(TestCase):
     def test_example_1(self) -> None:
         x = {
@@ -104,21 +104,21 @@
         ]
         for sublst in lst:
             random.shuffle(sublst)
         random.shuffle(lst)
 
         self.assertTrue(is_list_list_str(lst))
 
-        flatten, sizes = flat_list(lst)
+        flatten, sizes = flat_list_of_list(lst)
 
         self.assertTrue(is_list_str(flatten))
         self.assertEqual(len(lst), len(sizes))
         self.assertEqual(len(flatten), sum(sizes))
 
-        unflat = unflat_list(flatten, sizes)
+        unflat = unflat_list_of_list(flatten, sizes)
 
         self.assertTrue(is_list_list_str(unflat))
         self.assertEqual(len(lst), len(unflat))
         self.assertListEqual(lst, unflat)
 
 
 if __name__ == "__main__":
```

### Comparing `torchoutil-0.3.1/tests/test_utils_hdf.py` & `torchoutil-0.4.0/tests/test_utils_hdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 import numpy as np
 import torch
 from torch import Tensor
 from torch.utils.data.dataset import Subset
 from torchvision.datasets import CIFAR10
 
-from torchoutil.nn import IndicesToOneHot, ToList, ToNumpy, TSequential
+from torchoutil.nn import ESequential, IndexToOnehot, ToList, ToNumpy
 from torchoutil.utils.hdf import pack_to_hdf
 
 
 class TestHDF(TestCase):
     def test_cifar10_pack_to_hdf(self) -> None:
         dataset = CIFAR10(
             "/tmp",
             train=False,
             transform=ToNumpy(),
-            target_transform=TSequential(IndicesToOneHot(10), ToList()),
+            target_transform=ESequential(IndexToOnehot(10), ToList()),
             download=True,
         )
         dataset = Subset(
             dataset,
             torch.randint(0, len(dataset), (max(len(dataset) // 10, 1),)).tolist(),
         )
 
@@ -34,15 +34,15 @@
 
         idx = 0
         image0, label0 = dataset[idx]
         image1, label1 = hdf_dataset[idx]
 
         assert len(dataset) == len(hdf_dataset)
         assert np.equal(image0, image1).bool().all()
-        assert label0 == label1
+        assert np.equal(label0, label1).bool().all()
 
         hdf_dataset.close()
         os.remove(path)
 
     def test_shape_column(self) -> None:
         data = [torch.rand(10, 2), torch.rand(10, 5), torch.rand(10, 3)]
         data_shape = [(10, 1), (10, 2), (10, 1)]
```

### Comparing `torchoutil-0.3.1/tests/test_utils_pickle.py` & `torchoutil-0.4.0/tests/test_utils_pack.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 import numpy as np
 import torch
 from torch import Generator
 from torch.utils.data.dataset import Subset
 from torchvision.datasets import CIFAR10
 
-from torchoutil.nn import IndicesToOneHot, ToList, ToNumpy, TSequential
-from torchoutil.utils.pickle_dataset import pack_to_pickle
+from torchoutil.nn import ESequential, IndexToOnehot, ToList, ToNumpy
+from torchoutil.utils.pack import pack_dataset
 
 
-class TestCIFAR10ToPickle(TestCase):
-    def test_cifar10_pack_to_pickle(self) -> None:
+class TestPackCIFAR10(TestCase):
+    def test_cifar10_pack_per_item(self) -> None:
         dataset = CIFAR10(
             "/tmp",
             train=False,
             transform=ToNumpy(),
-            target_transform=TSequential(IndicesToOneHot(10), ToList()),
+            target_transform=ESequential(IndexToOnehot(10), ToList()),
             download=True,
         )
 
         seed = int(torch.randint(0, 10000, ()).item())
         generator = Generator().manual_seed(seed)
         dataset = Subset(
             dataset,
@@ -35,32 +35,32 @@
                 len(dataset),
                 (max(len(dataset) // 10, 1),),
                 generator=generator,
             ).tolist(),
         )
 
         path = "/tmp/test_cifar10"
-        pkl_dataset = pack_to_pickle(dataset, path, overwrite=True)
+        pkl_dataset = pack_dataset(dataset, path, overwrite=True)
 
         assert len(dataset) == len(pkl_dataset)
 
         idx = 0
         image0, label0 = dataset[idx]
         image1, label1 = pkl_dataset[idx]
 
         assert len(dataset) == len(pkl_dataset)
         assert label0 == label1, f"{label0=}, {label1=}"
         assert np.equal(image0, image1).all()
 
-    def test_cifar10_pack_to_pickle_batch(self) -> None:
+    def test_cifar10_pack_per_batch(self) -> None:
         dataset = CIFAR10(
             "/tmp",
             train=False,
             transform=ToNumpy(),
-            target_transform=TSequential(IndicesToOneHot(10), ToList()),
+            target_transform=ESequential(IndexToOnehot(10), ToList()),
             download=True,
         )
 
         seed = int(torch.randint(0, 10000, ()).item())
         generator = Generator().manual_seed(seed)
         dataset = Subset(
             dataset,
@@ -68,44 +68,86 @@
                 0,
                 len(dataset),
                 (max(len(dataset) // 10, 1),),
                 generator=generator,
             ).tolist(),
         )
 
-        path = "/tmp/test_cifar10"
-        pkl_dataset = pack_to_pickle(
-            dataset, path, overwrite=True, content_mode="batch"
+        path = "/tmp/test_cifar10_batch"
+        pkl_dataset = pack_dataset(
+            dataset,
+            path,
+            overwrite=True,
+            content_mode="batch",
+        )
+
+        assert len(dataset) == len(pkl_dataset)
+
+        idx = 0
+        image0, label0 = dataset[idx]
+        image1, label1 = pkl_dataset[idx]
+
+        assert len(dataset) == len(pkl_dataset)
+        assert label0 == label1, f"{label0=}, {label1=}"
+        assert np.equal(image0, image1).all()
+
+    def test_cifar10_pack_subdir(self) -> None:
+        dataset = CIFAR10(
+            "/tmp",
+            train=False,
+            transform=ToNumpy(),
+            target_transform=ESequential(IndexToOnehot(10), ToList()),
+            download=True,
+        )
+
+        seed = int(torch.randint(0, 10000, ()).item())
+        generator = Generator().manual_seed(seed)
+        dataset = Subset(
+            dataset,
+            torch.randint(
+                0,
+                len(dataset),
+                (max(len(dataset) // 50, 1),),
+                generator=generator,
+            ).tolist(),
+        )
+
+        path = "/tmp/test_cifar10_subdir"
+        pkl_dataset = pack_dataset(
+            dataset,
+            path,
+            overwrite=True,
+            content_mode="item",
+            subdir_size=100,
         )
 
         assert len(dataset) == len(pkl_dataset)
 
         idx = 0
         image0, label0 = dataset[idx]
         image1, label1 = pkl_dataset[idx]
 
         assert len(dataset) == len(pkl_dataset)
         assert label0 == label1, f"{label0=}, {label1=}"
         assert np.equal(image0, image1).all()
 
 
-class TestSpeechCommandsToPickle(TestCase):
+class TestPackSpeechCommands(TestCase):
     def test_example_1(self) -> None:
-        # Pack to pickle
         from torch import nn
         from torchaudio.datasets import SPEECHCOMMANDS
         from torchaudio.transforms import Spectrogram
 
-        from torchoutil.utils.pickle_dataset import pack_to_pickle
+        from torchoutil.utils.pack import pack_dataset
 
         speech_commands_root = "/tmp/speech_commands"
-        pickle_root = "/tmp/pickled_speech_commands"
+        packed_root = "/tmp/packed_speech_commands"
 
         os.makedirs(speech_commands_root, exist_ok=True)
-        os.makedirs(pickle_root, exist_ok=True)
+        os.makedirs(packed_root, exist_ok=True)
 
         dataset = SPEECHCOMMANDS(
             speech_commands_root,
             download=True,
             subset="validation",
         )
         indices = torch.randperm(len(dataset))[: len(dataset) // 10].tolist()
@@ -118,31 +160,31 @@
 
             def forward(self, item):
                 waveform = item[0]
                 spectrogram = self.spectrogram_extractor(waveform)
                 return (spectrogram,) + item[1:]
 
         transform = MyTransform()
-        pack_to_pickle(dataset, pickle_root, transform, overwrite=True, num_workers=0)
+        pack_dataset(dataset, packed_root, transform, overwrite=True, num_workers=0)
 
         # Read from pickle
-        from torchoutil.utils.pickle_dataset import PickleDataset
+        from torchoutil.utils.pack import PackedDataset
 
-        pickle_root = "/tmp/pickled_speech_commands"
-        pickle_dataset = PickleDataset(pickle_root)
-        pickle_dataset[0]  # first transformed item
+        packed_root = "/tmp/packed_speech_commands"
+        pack = PackedDataset(packed_root)
+        pack[0]  # first transformed item
 
         # Tests
         indices = torch.randperm(len(dataset))[:10].tolist()
 
-        assert len(dataset) == len(pickle_dataset)
+        assert len(dataset) == len(pack)
 
         for idx in indices:
             item_1 = transform(dataset[idx])
-            item_2 = pickle_dataset[idx]
+            item_2 = pack[idx]
 
             assert isinstance(item_1, tuple)
             assert isinstance(item_2, tuple)
             assert len(item_1) == len(item_2)
             assert torch.equal(item_1[0], item_2[0])
 
             for i in range(1, len(item_1)):
@@ -156,15 +198,15 @@
             start_1 = time.perf_counter()
             for idx in indices:
                 transform(dataset[idx])
             end_1 = time.perf_counter()
 
             start_2 = time.perf_counter()
             for idx in indices:
-                pickle_dataset[idx]
+                pack[idx]
             end_2 = time.perf_counter()
 
             durations_1.append(end_1 - start_1)
             durations_2.append(end_2 - start_2)
 
         duration_1 = sum(durations_1)
         duration_2 = sum(durations_2)
```

