# Comparing `tmp/optima_ml-0.3.4a1.tar.gz` & `tmp/optima_ml-0.3.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optima_ml-0.3.4a1.tar", last modified: Wed May 22 16:24:14 2024, max compression
+gzip compressed data, was "optima_ml-0.3.4a2.tar", last modified: Mon May 27 15:20:11 2024, max compression
```

## Comparing `optima_ml-0.3.4a1.tar` & `optima_ml-0.3.4a2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/
--rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.4a1/LICENSE
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.716290 optima_ml-0.3.4a1/OPTIMA/
--rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.4a1/OPTIMA/__main__.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/builtin/
--rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.4a1/OPTIMA/builtin/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    35432 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/builtin/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.4a1/OPTIMA/builtin/figures_of_merit.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    66758 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/builtin/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/builtin/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/builtin/search_space.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/core/
--rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/core/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    90299 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/evaluation.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/core/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    12282 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    41918 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/core/search_space.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/core/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    78638 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/training.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    80431 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/core/variable_optimization.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    17991 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/defaults.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/hardware_configs/
--rw-rw-r--   0 erik     (30000) erik     (30003)     2809 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/Dresden_Taurus.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    16754 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/common.py
--rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/hardware_configs/helpers.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/helpers/
--rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/helpers/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/helpers/extract_data_from_NTuples.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/helpers/manage_ray_nodes.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/keras/
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/keras/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    28658 2024-05-08 11:48:13.000000 optima_ml-0.3.4a1/OPTIMA/keras/model.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/OPTIMA/keras/tools.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-05-14 12:20:45.000000 optima_ml-0.3.4a1/OPTIMA/keras/training.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.720290 optima_ml-0.3.4a1/OPTIMA/lightning/
--rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.4a1/OPTIMA/lightning/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/lightning/inputs.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.4a1/OPTIMA/lightning/training.py
--rwxrwxr-x   0 erik     (30000) erik     (30003)   109000 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/OPTIMA/optima.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/OPTIMA/resources/
--rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.4a1/OPTIMA/resources/__init__.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.4a1/OPTIMA/resources/config_verification.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/OPTIMA/resources/pbt_with_seed.py
--rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)   120177 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/README.md
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/optima_ml.egg-info/
--rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/PKG-INFO
--rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/entry_points.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)      175 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/requires.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-05-22 16:24:14.000000 optima_ml-0.3.4a1/optima_ml.egg-info/top_level.txt
--rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/setup.cfg
--rw-rw-r--   0 erik     (30000) erik     (30003)     4231 2024-05-07 17:59:26.000000 optima_ml-0.3.4a1/setup.py
-drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-22 16:24:14.724290 optima_ml-0.3.4a1/tests/
--rw-rw-r--   0 erik     (30000) erik     (30003)    34780 2024-05-07 18:10:46.000000 optima_ml-0.3.4a1/tests/test_builtin.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    25661 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/tests/test_core.py
--rw-rw-r--   0 erik     (30000) erik     (30003)     9011 2024-05-22 16:24:02.000000 optima_ml-0.3.4a1/tests/test_integration.py
--rw-rw-rw-   0 erik     (30000) erik     (30003)     6579 2024-05-14 09:15:25.000000 optima_ml-0.3.4a1/tests/test_integration_sameMachine.py
--rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-04-23 18:38:54.000000 optima_ml-0.3.4a1/tests/test_preprocessing.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.657184 optima_ml-0.3.4a2/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35150 2023-08-12 13:57:40.000000 optima_ml-0.3.4a2/LICENSE
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.649184 optima_ml-0.3.4a2/OPTIMA/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      382 2024-01-30 16:21:26.000000 optima_ml-0.3.4a2/OPTIMA/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      132 2023-08-12 13:57:39.000000 optima_ml-0.3.4a2/OPTIMA/__main__.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.649184 optima_ml-0.3.4a2/OPTIMA/builtin/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      137 2024-02-07 21:12:40.000000 optima_ml-0.3.4a2/OPTIMA/builtin/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    35432 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/OPTIMA/builtin/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    32098 2024-02-07 21:12:40.000000 optima_ml-0.3.4a2/OPTIMA/builtin/figures_of_merit.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    66758 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/OPTIMA/builtin/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      423 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/builtin/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2858 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/OPTIMA/builtin/search_space.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/OPTIMA/core/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      114 2024-01-30 16:21:26.000000 optima_ml-0.3.4a2/OPTIMA/core/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    90299 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/core/evaluation.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    19104 2024-04-23 18:38:54.000000 optima_ml-0.3.4a2/OPTIMA/core/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    12282 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/core/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    41918 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/OPTIMA/core/search_space.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3469 2024-04-23 18:38:54.000000 optima_ml-0.3.4a2/OPTIMA/core/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    78638 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/core/training.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    80431 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/core/variable_optimization.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    17991 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/defaults.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/OPTIMA/hardware_configs/
+-rw-rw-r--   0 erik     (30000) erik     (30003)     2809 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/OPTIMA/hardware_configs/Dresden_Taurus.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      111 2024-01-30 16:21:26.000000 optima_ml-0.3.4a2/OPTIMA/hardware_configs/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    16754 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/OPTIMA/hardware_configs/common.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)      505 2024-04-23 18:38:54.000000 optima_ml-0.3.4a2/OPTIMA/hardware_configs/helpers.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/OPTIMA/helpers/
+-rw-rw-r--   0 erik     (30000) erik     (30003)       35 2024-01-30 16:21:26.000000 optima_ml-0.3.4a2/OPTIMA/helpers/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4853 2024-01-30 16:21:26.000000 optima_ml-0.3.4a2/OPTIMA/helpers/extract_data_from_NTuples.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     8670 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/helpers/manage_ray_nodes.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/OPTIMA/keras/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-01-30 16:21:26.000000 optima_ml-0.3.4a2/OPTIMA/keras/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    28926 2024-05-27 15:17:01.000000 optima_ml-0.3.4a2/OPTIMA/keras/model.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    53862 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/keras/tools.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     3912 2024-05-27 13:11:42.000000 optima_ml-0.3.4a2/OPTIMA/keras/training.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/OPTIMA/lightning/
+-rw-rw-r--   0 erik     (30000) erik     (30003)      106 2024-01-30 16:23:00.000000 optima_ml-0.3.4a2/OPTIMA/lightning/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    10100 2024-04-23 18:38:54.000000 optima_ml-0.3.4a2/OPTIMA/lightning/inputs.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     6301 2024-01-30 16:21:26.000000 optima_ml-0.3.4a2/OPTIMA/lightning/training.py
+-rwxrwxr-x   0 erik     (30000) erik     (30003)   109097 2024-05-27 15:19:08.000000 optima_ml-0.3.4a2/OPTIMA/optima.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/OPTIMA/resources/
+-rw-rw-r--   0 erik     (30000) erik     (30003)        0 2023-08-12 13:57:39.000000 optima_ml-0.3.4a2/OPTIMA/resources/__init__.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4772 2024-03-20 17:10:29.000000 optima_ml-0.3.4a2/OPTIMA/resources/config_verification.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    48922 2024-04-23 18:38:54.000000 optima_ml-0.3.4a2/OPTIMA/resources/pbt_with_seed.py
+-rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-05-27 15:20:11.657184 optima_ml-0.3.4a2/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)   120177 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/README.md
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/optima_ml.egg-info/
+-rw-r--r--   0 erik     (30000) erik     (30003)   121575 2024-05-27 15:20:11.000000 optima_ml-0.3.4a2/optima_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 erik     (30000) erik     (30003)     1342 2024-05-27 15:20:11.000000 optima_ml-0.3.4a2/optima_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        1 2024-05-27 15:20:11.000000 optima_ml-0.3.4a2/optima_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      102 2024-05-27 15:20:11.000000 optima_ml-0.3.4a2/optima_ml.egg-info/entry_points.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)      175 2024-05-27 15:20:11.000000 optima_ml-0.3.4a2/optima_ml.egg-info/requires.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)        7 2024-05-27 15:20:11.000000 optima_ml-0.3.4a2/optima_ml.egg-info/top_level.txt
+-rw-rw-r--   0 erik     (30000) erik     (30003)       38 2024-05-27 15:20:11.657184 optima_ml-0.3.4a2/setup.cfg
+-rw-rw-r--   0 erik     (30000) erik     (30003)     4231 2024-05-07 17:59:26.000000 optima_ml-0.3.4a2/setup.py
+drwxrwxr-x   0 erik     (30000) erik     (30003)        0 2024-05-27 15:20:11.653184 optima_ml-0.3.4a2/tests/
+-rw-rw-r--   0 erik     (30000) erik     (30003)    34779 2024-05-27 13:22:31.000000 optima_ml-0.3.4a2/tests/test_builtin.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    25661 2024-05-23 15:57:15.000000 optima_ml-0.3.4a2/tests/test_core.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)     9011 2024-05-23 15:57:15.000000 optima_ml-0.3.4a2/tests/test_integration.py
+-rw-rw-rw-   0 erik     (30000) erik     (30003)     6655 2024-05-27 15:16:31.000000 optima_ml-0.3.4a2/tests/test_integration_sameMachine.py
+-rw-rw-r--   0 erik     (30000) erik     (30003)    56852 2024-04-23 18:38:54.000000 optima_ml-0.3.4a2/tests/test_preprocessing.py
```

### Comparing `optima_ml-0.3.4a1/LICENSE` & `optima_ml-0.3.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/builtin/evaluation.py` & `optima_ml-0.3.4a2/OPTIMA/builtin/evaluation.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/builtin/figures_of_merit.py` & `optima_ml-0.3.4a2/OPTIMA/builtin/figures_of_merit.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/builtin/inputs.py` & `optima_ml-0.3.4a2/OPTIMA/builtin/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/builtin/search_space.py` & `optima_ml-0.3.4a2/OPTIMA/builtin/search_space.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/core/evaluation.py` & `optima_ml-0.3.4a2/OPTIMA/core/evaluation.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/core/inputs.py` & `optima_ml-0.3.4a2/OPTIMA/core/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/core/model.py` & `optima_ml-0.3.4a2/OPTIMA/core/model.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/core/search_space.py` & `optima_ml-0.3.4a2/OPTIMA/core/search_space.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/core/tools.py` & `optima_ml-0.3.4a2/OPTIMA/core/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/core/training.py` & `optima_ml-0.3.4a2/OPTIMA/core/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/core/variable_optimization.py` & `optima_ml-0.3.4a2/OPTIMA/core/variable_optimization.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/defaults.py` & `optima_ml-0.3.4a2/OPTIMA/defaults.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/hardware_configs/Dresden_Taurus.py` & `optima_ml-0.3.4a2/OPTIMA/hardware_configs/Dresden_Taurus.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/hardware_configs/common.py` & `optima_ml-0.3.4a2/OPTIMA/hardware_configs/common.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/helpers/extract_data_from_NTuples.py` & `optima_ml-0.3.4a2/OPTIMA/helpers/extract_data_from_NTuples.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/helpers/manage_ray_nodes.py` & `optima_ml-0.3.4a2/OPTIMA/helpers/manage_ray_nodes.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/keras/model.py` & `optima_ml-0.3.4a2/OPTIMA/keras/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,17 +280,22 @@
         )
         x = tf.keras.layers.Dense(
             units=units_i,
             kernel_initializer=kernel_initializer_layer,
             bias_initializer=bias_initializer_layer,
             kernel_regularizer=tf.keras.regularizers.L1L2(l1=model_config["l1_lambda"], l2=model_config["l2_lambda"]),
             bias_regularizer=tf.keras.regularizers.L1L2(l1=model_config["l1_lambda"], l2=model_config["l2_lambda"]),
+            use_bias=model_config["activation"] != "selu",
         )(x)
         if not model_config["activation"] == "selu":
-            x = tf.keras.layers.BatchNormalization(axis=1)(x)
+            x = tf.keras.layers.BatchNormalization(
+                axis=1,
+                beta_initializer=bias_initializer_layer,
+                beta_regularizer=tf.keras.regularizers.L1L2(l1=model_config["l1_lambda"], l2=model_config["l2_lambda"]),
+            )(x)
         x = activation_layer[0](**activation_layer[1])(x)
         if model_config["dropout"] > 0:
             if not model_config["activation"] == "selu":
                 x = tf.keras.layers.Dropout(model_config["dropout"])(x)
             else:
                 x = tf.keras.layers.AlphaDropout(model_config["dropout"])(x)
     if targets_train.shape[1] == 1:
```

### Comparing `optima_ml-0.3.4a1/OPTIMA/keras/tools.py` & `optima_ml-0.3.4a2/OPTIMA/keras/tools.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/keras/training.py` & `optima_ml-0.3.4a2/OPTIMA/keras/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/lightning/inputs.py` & `optima_ml-0.3.4a2/OPTIMA/lightning/inputs.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/lightning/training.py` & `optima_ml-0.3.4a2/OPTIMA/lightning/training.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/optima.py` & `optima_ml-0.3.4a2/OPTIMA/optima.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main steering script of OPTIMA."""
 
 __author__ = "E. Bachmann"
 __licence__ = "GPL3"
-__version__ = "0.3.4alpha1"
+__version__ = "0.3.4alpha2"
 __maintainer__ = "E. Bachmann"
 
 import os
 import sys
 import shutil
 import logging
 import argparse
@@ -1742,14 +1742,16 @@
     parser.add_argument('--max_pending_trials', type=int, default=None, help="Set how many trials are allowed to be 'pending'. If not set, will set to cpus / cpus_per_trail.")
 
     parser.add_argument('--is_worker', default=False, action="store_true", help="Is used to differentiate between the initialization step (create and execute batch script) and the working step (where the optimization is done).")
     parser.add_argument('--address', default=None, help="IP-address and port of the head node. This is set automatically for the working step.")
     parser.add_argument('--local_source', default=False, action="store_true", help="If set, will use the local source code even if OPTIMA is installed in the python environment.")
     parser.add_argument('--temp_dir', type=str, default=None, help="Overwrite Ray's default root temporary directory when running locally (i.e. --cluster 'local'). This must be an absolute path.")
 
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
+
     args = parser.parse_args(sys.argv[1:])
 
     # logging config
     DFormat = '%(asctime)s - %(levelname)s - %(message)s'
     logging.basicConfig(format=DFormat, level=logging.INFO)
 
     # load and check the config
```

### Comparing `optima_ml-0.3.4a1/OPTIMA/resources/config_verification.py` & `optima_ml-0.3.4a2/OPTIMA/resources/config_verification.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/OPTIMA/resources/pbt_with_seed.py` & `optima_ml-0.3.4a2/OPTIMA/resources/pbt_with_seed.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/PKG-INFO` & `optima_ml-0.3.4a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.4a1
+Version: 0.3.4a2
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
```

### Comparing `optima_ml-0.3.4a1/README.md` & `optima_ml-0.3.4a2/README.md`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/optima_ml.egg-info/PKG-INFO` & `optima_ml-0.3.4a2/optima_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optima-ml
-Version: 0.3.4a1
+Version: 0.3.4a2
 Summary: Distributed hyperparameter optimization and input variable selection for artificial neural networks.
 Home-page: https://gitlab.cern.ch/atlas-germany-dresden-vbs-group/optima
 Author: E. Bachmann
 Author-email: erik.bachmann@tu-dresden.de
 License: GPL
 Platform: linux
 Platform: darwin
```

### Comparing `optima_ml-0.3.4a1/optima_ml.egg-info/SOURCES.txt` & `optima_ml-0.3.4a2/optima_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/setup.py` & `optima_ml-0.3.4a2/setup.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/tests/test_builtin.py` & `optima_ml-0.3.4a2/tests/test_builtin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Collection of unit tests related to the built-in functionality of multilayer perceptrons for classification."""
 import os
 import sys
 import random as python_random
 import shutil
+import json
 
 if sys.platform == "darwin":
     import multiprocess as mp
 else:
     import multiprocessing as mp
 
 
@@ -110,123 +111,123 @@
             0.6111191
         ],
         "units": [
             0.6111191
         ],
         "activation": [
             [
-                0.11199405789375305,
-                0.11199405789375305,
-                0.13122156262397766,
-                0.24728567898273468,
-                0.24728567898273468,
-                0.2562752664089203,
+                0.11199413985013962,
+                0.11199413985013962,
+                0.15319252014160156,
+                0.24728573858737946,
+                0.24728573858737946,
+                0.26548105478286743,
                 0.49981728196144104,
                 0.49981728196144104,
-                0.48765021562576294
+                0.47525754570961
             ],
             [
-                0.48769962787628174,
-                0.4389059841632843,
-                0.45763760805130005,
-                0.8322291374206543,
-                0.4011659026145935,
-                0.38794681429862976,
-                0.6021961569786072,
+                0.3200555145740509,
+                0.4389059543609619,
+                0.4784073531627655,
+                0.8511413931846619,
+                0.4011658728122711,
+                0.37636175751686096,
+                0.6870542168617249,
                 0.49995288252830505,
-                0.49950286746025085
+                0.4989134669303894
             ],
             [
                 0.24593836069107056,
                 0.24593836069107056,
-                0.2433507740497589,
+                0.24073722958564758,
                 0.2390574812889099,
                 0.2390574812889099,
-                0.2366105318069458,
-                0.16493849456310272,
-                0.16493849456310272,
-                0.16492164134979248
+                0.23415543138980865,
+                0.16493847966194153,
+                0.16493847966194153,
+                0.16489720344543457
             ],
             [
-                0.12047722935676575,
-                0.12047722935676575,
-                0.14015184342861176,
+                0.1204773336648941,
+                0.1204773336648941,
+                0.1565568894147873,
                 0.25132814049720764,
                 0.25132814049720764,
-                0.25459209084510803,
+                0.2544344663619995,
                 0.49986428022384644,
                 0.49986428022384644,
-                0.48883968591690063
+                0.47762367129325867
             ],
             [
-                0.9287115335464478,
-                0.16108368337154388,
-                0.17931674420833588,
-                0.8247283697128296,
+                0.8292364478111267,
+                0.1610838770866394,
+                0.1973705142736435,
+                0.9208518862724304,
                 0.38233426213264465,
-                0.38340455293655396,
-                0.5336682200431824,
+                0.38480424880981445,
+                0.563783586025238,
                 0.49999698996543884,
-                0.4995178282260895
+                0.4983012080192566
             ],
             [
-                0.23903368413448334,
-                0.23903368413448334,
-                0.25384485721588135,
-                0.290642648935318,
-                0.290642648935318,
-                0.29449498653411865,
+                0.2390337437391281,
+                0.2390337437391281,
+                0.2675885260105133,
+                0.2906426787376404,
+                0.2906426787376404,
+                0.29933372139930725,
                 0.49999508261680603,
                 0.49999508261680603,
-                0.49936702847480774
+                0.4977942407131195
             ],
             [
                 0.5326128005981445,
                 0.5326128005981445,
-                0.5336645245552063,
+                0.5326128005981445,
+                0.21461912989616394,
                 0.21461912989616394,
                 0.21461912989616394,
-                0.21455450356006622,
                 0.4999467432498932,
                 0.4999467432498932,
-                0.50677889585495
+                0.4999467432498932
             ],
             [
-                0.11199405789375305,
-                0.11199405789375305,
-                0.13122156262397766,
-                0.24728567898273468,
-                0.24728567898273468,
-                0.2562752664089203,
+                0.11199413985013962,
+                0.11199413985013962,
+                0.15319252014160156,
+                0.24728573858737946,
+                0.24728573858737946,
+                0.26548105478286743,
                 0.49981728196144104,
                 0.49981728196144104,
-                0.48765021562576294
+                0.47525754570961
             ]
         ],
         "kernel_initializer": [
             0.6111191,
             0.025,
             0.49984
         ],
         "bias_initializer": [
             0.6111191,
             0.6111191,
             0.301061
         ],
         "l1_lambda": [
-            0.11199405789375305,
-            0.11199405789375305
+            0.11199413985013962,
+            0.11199413985013962
         ],
         "l2_lambda": [
-            0.11199405789375305,
-            0.11199405789375305
+            0.11199413985013962,
+            0.11199413985013962
         ],
         "dropout": [
-            0.11199405789375305,
-            0.11199405789375305
+            0.11199413985013962,
+            0.11199413985013962
         ],
         "batch_size": [
             0.6111191
         ],
         "learning_rate": [
             0.6111191
         ],
@@ -318,31 +319,31 @@
             0.66367704
         ],
         "units_3": [
             0.66367704
         ],
         "activation": [
             0.5740598440170288,
-            0.22188419103622437,
+            0.3394704759120941,
             0.4631745517253876,
-            0.5869430303573608,
-            0.5426632761955261,
-            0.5887803435325623,
+            0.5869429707527161,
+            0.5978847146034241,
+            0.5887802839279175,
             0.6611102223396301,
             0.5740598440170288
         ],
         "kernel_initializer": [
             0.5740598440170288,
-            0.6003352403640747,
+            0.6003351807594299,
             0.4999960660934448
         ],
         "bias_initializer": [
             0.5740598440170288,
             0.5740598440170288,
-            0.5549465417861938
+            0.5356596112251282
         ],
         "l1_lambda": [
             0.5740598440170288,
             0.5740598440170288
         ],
         "l2_lambda": [
             0.5740598440170288,
```

### Comparing `optima_ml-0.3.4a1/tests/test_core.py` & `optima_ml-0.3.4a2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/tests/test_integration.py` & `optima_ml-0.3.4a2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `optima_ml-0.3.4a1/tests/test_integration_sameMachine.py` & `optima_ml-0.3.4a2/tests/test_integration_sameMachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,16 @@
             _,
             _,
             _,
             _,
             evaluation_string_reference,
             raw_metric_values_reference
         ) = pickle.load(evaluation_file)
-    assert (2 * (best_trials.drop(columns="trial") - best_trials_reference.drop(columns="trial")) / (best_trials.drop(columns="trial") + best_trials_reference.drop(columns="trial"))).abs().max().max() < 1e-8
+    assert (2 * (best_trials.drop(columns=["trial", "best index"]) - best_trials_reference.drop(columns=["trial", "best index"]))
+            / (best_trials.drop(columns=["trial", "best index"]) + best_trials_reference.drop(columns=["trial", "best index"]))).abs().max().max() < 1e-8
     assert configs_df.equals(configs_df_reference)
     for raw, raw_test in zip(raw_metric_values, raw_metric_values_reference):
         if raw != 0 or raw_test != 0:
             assert abs(2 * (raw - raw_test) / (raw + raw_test)) < 1e-8
 
     # cleanup
     shutil.rmtree("tests/test_optimization")
```

### Comparing `optima_ml-0.3.4a1/tests/test_preprocessing.py` & `optima_ml-0.3.4a2/tests/test_preprocessing.py`

 * *Files identical despite different names*

