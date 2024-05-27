# Comparing `tmp/pystreed-1.2.3.tar.gz` & `tmp/pystreed-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystreed-1.2.3.tar", last modified: Wed Apr 10 13:33:58 2024, max compression
+gzip compressed data, was "pystreed-1.3.0.tar", last modified: Mon May 27 15:28:16 2024, max compression
```

## Comparing `pystreed-1.2.3.tar` & `pystreed-1.3.0.tar`

### file list

```diff
@@ -1,64 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-10 13:33:49.000000 pystreed-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16146 2024-04-10 13:33:58.209267 pystreed-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14005 2024-04-10 13:33:49.000000 pystreed-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 13:33:52.000000 pystreed-1.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.201267 pystreed-1.2.3/pystreed/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19517 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/binarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/cost_sensitive_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/group_fair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/instance_cost_sensitive_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/prescriptive_policy_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/survival_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-10 13:33:52.000000 pystreed-1.2.3/pystreed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/pystreed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16146 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 13:33:58.000000 pystreed-1.2.3/pystreed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:33:58.209267 pystreed-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-10 13:33:52.000000 pystreed-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.205267 pystreed-1.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.205267 pystreed-1.2.3/src/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/model/branch.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13192 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/model/data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/model/feature_vector.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.205267 pystreed-1.2.3/src/solver/
--rw-r--r--   0 runner    (1001) docker     (127)    10229 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/branch_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/cost_combiner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/cost_storage.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/counter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/data_splitter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/dataset_cache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/define_parameters.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/difference_computer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/feature_selector_gini.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/result.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/similarity_lowerbound.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    45271 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20872 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/solver/terminal_solver.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/src/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/src/tasks/accuracy/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/accuracy/accuracy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/accuracy/cost_complex_accuracy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/cost_sensitive.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/eq_opp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/f1score.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/group_fairness.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/instance_cost_sensitive.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/optimization_task.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/prescriptive_policy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/tasks/survival_analysis.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:58.209267 pystreed-1.2.3/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/file_reader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/key_value_heap.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/parameter_handler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 13:33:52.000000 pystreed-1.2.3/src/utils/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.871137 pystreed-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-27 15:28:09.000000 pystreed-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-05-27 15:28:16.871137 pystreed-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16587 2024-05-27 15:28:09.000000 pystreed-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-27 15:28:12.000000 pystreed-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.863137 pystreed-1.3.0/pystreed/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20575 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16406 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/binarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/cost_sensitive_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/group_fair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/instance_cost_sensitive_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10543 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/prescriptive_policy_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16683 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14543 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/survival_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-27 15:28:12.000000 pystreed-1.3.0/pystreed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.871137 pystreed-1.3.0/pystreed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-05-27 15:28:16.000000 pystreed-1.3.0/pystreed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-27 15:28:16.000000 pystreed-1.3.0/pystreed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:28:16.000000 pystreed-1.3.0/pystreed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 15:28:16.000000 pystreed-1.3.0/pystreed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 15:28:16.000000 pystreed-1.3.0/pystreed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:28:16.871137 pystreed-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 15:28:12.000000 pystreed-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.863137 pystreed-1.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    19423 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.863137 pystreed-1.3.0/src/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/model/branch.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/model/data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/model/feature_vector.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.867137 pystreed-1.3.0/src/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/branch_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19866 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/cost_combiner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/cost_storage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/counter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/data_splitter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/dataset_cache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/define_parameters.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/difference_computer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/feature_selector_gini.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/result.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/similarity_lowerbound.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47390 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/solver/terminal_solver.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.867137 pystreed-1.3.0/src/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.867137 pystreed-1.3.0/src/tasks/accuracy/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/accuracy/accuracy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/accuracy/cost_complex_accuracy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/cost_sensitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/eq_opp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/f1score.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/group_fairness.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/instance_cost_sensitive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/optimization_task.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/prescriptive_policy.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.867137 pystreed-1.3.0/src/tasks/regression/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.871137 pystreed-1.3.0/src/tasks/regression/ckmeans/
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/regression/ckmeans/Ckmeans.1d.dp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/regression/ckmeans/fill_SMAWK.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/regression/ckmeans/fill_log_linear.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/regression/cost_complex_regression.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/regression/piecewise_linear_regression.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19379 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/regression/piecewise_simple_linear_regression.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/regression/regression.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/tasks/survival_analysis.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:28:16.871137 pystreed-1.3.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/utils/file_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/utils/key_value_heap.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19973 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/utils/parameter_handler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 15:28:12.000000 pystreed-1.3.0/src/utils/utils.cpp
```

### Comparing `pystreed-1.2.3/LICENSE` & `pystreed-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/PKG-INFO` & `pystreed-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystreed
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python Implementation of STreeD: Dynamic Programming Approach for Optimal Decision Trees with Separable objectives and Constraints
 Author-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>, Emir Demirović <E.Demirovic@tudelft.nl>, "Mathijs M. de Weerdt" <M.M.deWeerdt@tudelft.nl>
 Maintainer-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>
 License: Copyright 2023 Jacobus G. M. van der Linden, Delft University of Technology
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -31,15 +31,17 @@
 
 # STreeD: Separable Trees with Dynamic programming
 By: Jacobus G. M. van der Linden [(e-mail)](mailto:J.G.M.vanderLinden@tudelft.nl)
 
 STreeD is a framework for optimal binary decision trees with _separable_ optimization tasks. A separable optimization task is a task that can be optimized separately for the left and right subtree. The current STreeD Framework implements a broad set of such optimization tasks, from group fairness constraints to survival analysis. For an explanation of each application, see below.
 For details on what tasks are separable and how the algoritm works, see our paper.
 
-* Van der Linden, Jacobus G. M., Mathijs M. de Weerdt, and Emir Demirović. "Necessary and Sufficient Conditions for Optimal Decision Trees using Dynamic Programming." _Advances in Neural Information Processing Systems_ (Accepted, not published). 2023. [pdf](https://arxiv.org/pdf/2305.19706) 
+If you use STreeD, please cite our paper:
+
+* Van der Linden, Jacobus G. M., Mathijs M. de Weerdt, and Emir Demirović. "Necessary and Sufficient Conditions for Optimal Decision Trees using Dynamic Programming." _Advances in Neural Information Processing Systems_. 2023. [pdf](https://proceedings.neurips.cc/paper_files/paper/2023/file/1d5fce9627e15c84db572a66e029b1fc-Paper-Conference.pdf) 
 
 ## Python usage
 
 ### Install from PyPi
 The `pystreed` python package can be installed from PyPi using `pip`:
 
 ```sh
@@ -127,15 +129,15 @@
 Currently, STreeD implements the following optimization tasks:
 
 ### Classification
 `STreeDClassifier` implements the following optimization tasks:
 
 * `accuracy`: Minimizes the misclassification score. 
 * `cost-complex-accuracy`: Minimizes the misclassification score plus the cost for adding a branching node by the parameter `cost_complexity`.
-* `f1-score`: Minimizes the F1-score.
+* `f1-score`: Maximizes the F1-score.
 
 See [examples/accuracy_example.py](examples/accuracy_example.py) for an example.
 
 ### Cost-Sensitive Classification
 `STreeDCostSensitiveClassifier` implements a cost-sensitive classifier. Costs can both be attributed to features and misclassifications.
 
 The costs can be specified with `CostSpecifier` object. This object is either initialized with a file name for the cost specification and the number of classes; or with the misclassification cost matrix, and the cost specifier per feature. When testing a feature in a branch node, the cost for that feature is paid for every instance that passes through it. When another feature from the same group was tested before, the discounted cost is paid. When another feature that is binarized from the same original feature is already tested, the cost is zero.
@@ -165,39 +167,64 @@
 
 See [examples/group_fair_example.py](examples/group_fair_example.py) for an example.
 
 ### Prescriptive policy generation
 `STreeDPrescriptivePolicyGenerator` implements a policy generation solver. Counterfactual scores need to be provided. The current implementation allows for three different teacher methods, as specified by the `teacher_method` parameter:
 * `DM`: the _direct method_ or _Regress & Compare_ method. This teacher specifies for every treatment (label) what the expected outcome is.
 * `IPW`: the _inverse propensity weighting_ method. This teacher provides the propensity scores mu(x, k): the probability of treatment k happening for feature vector x.
-* `DR`: the _doubly robust_ method: a combination of the direct methodand the inverse propensity weighting method.
+* `DR`: the _doubly robust_ method: a combination of the direct method and the inverse propensity weighting method.
 
 The teacher data needs to be passed to the solver by initializing a `PPGData` object for every instance. The PPGData initializer expects the following parameters:
 * `historic_treatment : int` : the historic treatment label
 * `historic_outcome : float` : the historic outcome
 * `propensity_score : float` : the propensity score for the historic treatment
 * `predicted_outcome : List[float]` : the _regress & compare_ prediction for each possible treatment
 Optional (for testing)
 * `optimal_treatment : int` : the optimal treatment
 * `counterfactual_outcome : List[float]` : the counterfactual outcome 
 
 Only the data which will be used by the teacher method needs to be specified, the rest can be initialized with zero's.
 
 See [examples/prescriptive_policy_example.py](examples/prescriptive_policy_example.py) for an example.
 
+### Regression
+
+`STreeDRegressor` implements two variants of regression, as specified by the optimization task parameter
+* `regression`: Miminimizes the _sum of squared errors_.
+* `cost-complex-regression`: Minimizes the _sum of squared errors_ plus the cost for adding a branching node by the parameter `cost_complexity`. For runtime improvement, custom lower bounds can be specified if `use_task_lower_bound=True`. The custom lower bound `regression_bound` can be set to either `"equivalent"` to use the equivalent-points bound or `"kmeans"` to use a k-means lower bound.
+
+See [examples/regression_example.py](examples/regression_example.py) for an example.
+
+If you use STreeD for _regression_, please cite our paper:
+
+* Van den Bos, M., Jacobus G. M. van der Linden, and Emir Demirović. "Piecewise Constant and Linear Regression Trees: An Optimal Dynamic Programming Approach." In _Proceedings of ICML-24_, 2024.
+
+### Piecewise Linear Regression
+`STreeDPiecewiseLinearRegressor` implements a solver for optimizing piecewise linear regression trees, with a linear elastic net regression predictor in every leaf node. The lasso and ridge penalization can be set with the `lasso_penalty` and `ridge_penalty` and parameters. The addition of a new branching node is penalized by the `cost_complexity` parameter. Alternatively, `STreeDPiecewiseLinearRegressor` can learn a simple linear regression model in every leaf by setting `simple = True`. The simple linear regression model is penalized only with the ridge penalization.
+
+`STreeDPiecewiseLinearRegressor` only uses the continuous features for fitting the linear lasso regression model in every leaf node. These continuous features can be automatically inferred from the data or explicitly specified using the `continuous_columns` parameter of the `fit` method.
+
+To prevent fitting linear models on too little data, `STreeDPiecewiseLinearRegressor` by default sets the `min_leaf_node_size` parameter to at least 5 times the number of continuous features or to at least 5 when fitting a simple linear regression model.
+
+See [examples/piecewise_linear_regression_example.py](examples/piecewise_linear_regression_example.py) for an example.
+
+If you use STreeD for _piecewise linear regression_, please cite our paper:
+
+* Van den Bos, M., Jacobus G. M. van der Linden, and Emir Demirović. "Piecewise Constant and Linear Regression Trees: An Optimal Dynamic Programming Approach." In _Proceedings of ICML-24_, 2024.
+
 ### Survival analysis
-`STreeDSurvivalAnalysis` implements an optimal survival tree method, by optimizing the proportional hazard function of LeBlanc and Crowly, "Relative Risk for Censored Survival Data," _Biometrics_ 48.2 (1992): 411-425. Each leaf node predicts a risk factor $\theta$ which is used to shift the base hazard model $\hat{\Lambda}(t)$.  The Kaplan-Meier estimator is used as a stepwise survival function $\hat{S}(t) = e^{-\theta \hat{\Lambda}(t)}$.
+`STreeDSurvivalAnalysis` implements an optimal survival tree method, by optimizing the proportional hazard function of LeBlanc and Crowly, "Relative Risk for Censored Survival Data," _Biometrics_ 48.2 (1992): 411-425. Each leaf node predicts a risk factor $\theta$ which is used to shift the base hazard model $\hat{\Lambda}(t)$.  The Nelson-Aalen estimator is used as a stepwise survival function $\hat{S}(t) = e^{-\theta \hat{\Lambda}(t)}$.
 
 Instead of a label, the input data expects a two-dimensional array with for each instance 1) a binary censoring indicator and 2) a time-of-event (death or censoring).
 
 See [examples/survival_analysis_example.py](examples/survival_analysis_example.py) for an example.
 
 If you use STreeD for _survival analysis_, please cite our paper:
 
-* Huisman, T., Jacobus G. M. van der Linden, and Emir Demirović. "Optimal Survival Trees: A Dynamic Programming Approach." _Proceedings of AAAI-24_ (Accepted, not published). 2024. 
+* Huisman, T., Jacobus G. M. van der Linden, and Emir Demirović. "Optimal Survival Trees: A Dynamic Programming Approach." _Proceedings of AAAI-24_. 2024. [pdf](https://arxiv.org/pdf/2401.04489.pdf)
 
 ## Parameters
 STreeD can be configured by the following parameters:
 * `max_depth` : The maximum depth of the tree. Note that a tree of depth zero has a single leaf node. A tree of depth one has one branching node and two leaf nodes.
 * `max_num_nodes` : The maximum number of _branching_ nodes in the tree.
 * `min_leaf_node_size` : The minimum number of samples required in each leaf node.
 * `time_limit` : The run time limit in seconds. If the time limit is exceeded a possibly non-optimal tree is returned.
```

### Comparing `pystreed-1.2.3/README.md` & `pystreed-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 # STreeD: Separable Trees with Dynamic programming
 By: Jacobus G. M. van der Linden [(e-mail)](mailto:J.G.M.vanderLinden@tudelft.nl)
 
 STreeD is a framework for optimal binary decision trees with _separable_ optimization tasks. A separable optimization task is a task that can be optimized separately for the left and right subtree. The current STreeD Framework implements a broad set of such optimization tasks, from group fairness constraints to survival analysis. For an explanation of each application, see below.
 For details on what tasks are separable and how the algoritm works, see our paper.
 
-* Van der Linden, Jacobus G. M., Mathijs M. de Weerdt, and Emir Demirović. "Necessary and Sufficient Conditions for Optimal Decision Trees using Dynamic Programming." _Advances in Neural Information Processing Systems_ (Accepted, not published). 2023. [pdf](https://arxiv.org/pdf/2305.19706) 
+If you use STreeD, please cite our paper:
+
+* Van der Linden, Jacobus G. M., Mathijs M. de Weerdt, and Emir Demirović. "Necessary and Sufficient Conditions for Optimal Decision Trees using Dynamic Programming." _Advances in Neural Information Processing Systems_. 2023. [pdf](https://proceedings.neurips.cc/paper_files/paper/2023/file/1d5fce9627e15c84db572a66e029b1fc-Paper-Conference.pdf) 
 
 ## Python usage
 
 ### Install from PyPi
 The `pystreed` python package can be installed from PyPi using `pip`:
 
 ```sh
@@ -99,15 +101,15 @@
 Currently, STreeD implements the following optimization tasks:
 
 ### Classification
 `STreeDClassifier` implements the following optimization tasks:
 
 * `accuracy`: Minimizes the misclassification score. 
 * `cost-complex-accuracy`: Minimizes the misclassification score plus the cost for adding a branching node by the parameter `cost_complexity`.
-* `f1-score`: Minimizes the F1-score.
+* `f1-score`: Maximizes the F1-score.
 
 See [examples/accuracy_example.py](examples/accuracy_example.py) for an example.
 
 ### Cost-Sensitive Classification
 `STreeDCostSensitiveClassifier` implements a cost-sensitive classifier. Costs can both be attributed to features and misclassifications.
 
 The costs can be specified with `CostSpecifier` object. This object is either initialized with a file name for the cost specification and the number of classes; or with the misclassification cost matrix, and the cost specifier per feature. When testing a feature in a branch node, the cost for that feature is paid for every instance that passes through it. When another feature from the same group was tested before, the discounted cost is paid. When another feature that is binarized from the same original feature is already tested, the cost is zero.
@@ -137,39 +139,64 @@
 
 See [examples/group_fair_example.py](examples/group_fair_example.py) for an example.
 
 ### Prescriptive policy generation
 `STreeDPrescriptivePolicyGenerator` implements a policy generation solver. Counterfactual scores need to be provided. The current implementation allows for three different teacher methods, as specified by the `teacher_method` parameter:
 * `DM`: the _direct method_ or _Regress & Compare_ method. This teacher specifies for every treatment (label) what the expected outcome is.
 * `IPW`: the _inverse propensity weighting_ method. This teacher provides the propensity scores mu(x, k): the probability of treatment k happening for feature vector x.
-* `DR`: the _doubly robust_ method: a combination of the direct methodand the inverse propensity weighting method.
+* `DR`: the _doubly robust_ method: a combination of the direct method and the inverse propensity weighting method.
 
 The teacher data needs to be passed to the solver by initializing a `PPGData` object for every instance. The PPGData initializer expects the following parameters:
 * `historic_treatment : int` : the historic treatment label
 * `historic_outcome : float` : the historic outcome
 * `propensity_score : float` : the propensity score for the historic treatment
 * `predicted_outcome : List[float]` : the _regress & compare_ prediction for each possible treatment
 Optional (for testing)
 * `optimal_treatment : int` : the optimal treatment
 * `counterfactual_outcome : List[float]` : the counterfactual outcome 
 
 Only the data which will be used by the teacher method needs to be specified, the rest can be initialized with zero's.
 
 See [examples/prescriptive_policy_example.py](examples/prescriptive_policy_example.py) for an example.
 
+### Regression
+
+`STreeDRegressor` implements two variants of regression, as specified by the optimization task parameter
+* `regression`: Miminimizes the _sum of squared errors_.
+* `cost-complex-regression`: Minimizes the _sum of squared errors_ plus the cost for adding a branching node by the parameter `cost_complexity`. For runtime improvement, custom lower bounds can be specified if `use_task_lower_bound=True`. The custom lower bound `regression_bound` can be set to either `"equivalent"` to use the equivalent-points bound or `"kmeans"` to use a k-means lower bound.
+
+See [examples/regression_example.py](examples/regression_example.py) for an example.
+
+If you use STreeD for _regression_, please cite our paper:
+
+* Van den Bos, M., Jacobus G. M. van der Linden, and Emir Demirović. "Piecewise Constant and Linear Regression Trees: An Optimal Dynamic Programming Approach." In _Proceedings of ICML-24_, 2024.
+
+### Piecewise Linear Regression
+`STreeDPiecewiseLinearRegressor` implements a solver for optimizing piecewise linear regression trees, with a linear elastic net regression predictor in every leaf node. The lasso and ridge penalization can be set with the `lasso_penalty` and `ridge_penalty` and parameters. The addition of a new branching node is penalized by the `cost_complexity` parameter. Alternatively, `STreeDPiecewiseLinearRegressor` can learn a simple linear regression model in every leaf by setting `simple = True`. The simple linear regression model is penalized only with the ridge penalization.
+
+`STreeDPiecewiseLinearRegressor` only uses the continuous features for fitting the linear lasso regression model in every leaf node. These continuous features can be automatically inferred from the data or explicitly specified using the `continuous_columns` parameter of the `fit` method.
+
+To prevent fitting linear models on too little data, `STreeDPiecewiseLinearRegressor` by default sets the `min_leaf_node_size` parameter to at least 5 times the number of continuous features or to at least 5 when fitting a simple linear regression model.
+
+See [examples/piecewise_linear_regression_example.py](examples/piecewise_linear_regression_example.py) for an example.
+
+If you use STreeD for _piecewise linear regression_, please cite our paper:
+
+* Van den Bos, M., Jacobus G. M. van der Linden, and Emir Demirović. "Piecewise Constant and Linear Regression Trees: An Optimal Dynamic Programming Approach." In _Proceedings of ICML-24_, 2024.
+
 ### Survival analysis
-`STreeDSurvivalAnalysis` implements an optimal survival tree method, by optimizing the proportional hazard function of LeBlanc and Crowly, "Relative Risk for Censored Survival Data," _Biometrics_ 48.2 (1992): 411-425. Each leaf node predicts a risk factor $\theta$ which is used to shift the base hazard model $\hat{\Lambda}(t)$.  The Kaplan-Meier estimator is used as a stepwise survival function $\hat{S}(t) = e^{-\theta \hat{\Lambda}(t)}$.
+`STreeDSurvivalAnalysis` implements an optimal survival tree method, by optimizing the proportional hazard function of LeBlanc and Crowly, "Relative Risk for Censored Survival Data," _Biometrics_ 48.2 (1992): 411-425. Each leaf node predicts a risk factor $\theta$ which is used to shift the base hazard model $\hat{\Lambda}(t)$.  The Nelson-Aalen estimator is used as a stepwise survival function $\hat{S}(t) = e^{-\theta \hat{\Lambda}(t)}$.
 
 Instead of a label, the input data expects a two-dimensional array with for each instance 1) a binary censoring indicator and 2) a time-of-event (death or censoring).
 
 See [examples/survival_analysis_example.py](examples/survival_analysis_example.py) for an example.
 
 If you use STreeD for _survival analysis_, please cite our paper:
 
-* Huisman, T., Jacobus G. M. van der Linden, and Emir Demirović. "Optimal Survival Trees: A Dynamic Programming Approach." _Proceedings of AAAI-24_ (Accepted, not published). 2024. 
+* Huisman, T., Jacobus G. M. van der Linden, and Emir Demirović. "Optimal Survival Trees: A Dynamic Programming Approach." _Proceedings of AAAI-24_. 2024. [pdf](https://arxiv.org/pdf/2401.04489.pdf)
 
 ## Parameters
 STreeD can be configured by the following parameters:
 * `max_depth` : The maximum depth of the tree. Note that a tree of depth zero has a single leaf node. A tree of depth one has one branching node and two leaf nodes.
 * `max_num_nodes` : The maximum number of _branching_ nodes in the tree.
 * `min_leaf_node_size` : The minimum number of samples required in each leaf node.
 * `time_limit` : The run time limit in seconds. If the time limit is exceeded a possibly non-optimal tree is returned.
```

### Comparing `pystreed-1.2.3/pyproject.toml` & `pystreed-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "pybind11>=2.10.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pystreed"
-version = "1.2.3"
+version = "1.3.0"
 requires-python = ">=3.8"						 
 description = "Python Implementation of STreeD: Dynamic Programming Approach for Optimal Decision Trees with Separable objectives and Constraints"
 license=  {file = "LICENSE"}
 readme = "README.md"						
 authors = [
     {name = "Jacobus G. M. van der Linden", email="J.G.M.vanderLinden@tudelft.nl"},
     {name = "Emir Demirović", email="E.Demirovic@tudelft.nl"},
```

### Comparing `pystreed-1.2.3/pystreed/base.py` & `pystreed-1.3.0/pystreed/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 import time
 import numbers
 import sys
 
 class BaseSTreeDSolver(BaseEstimator):
 
     _parameter_constraints: dict = {
-        "optimization_task": [StrOptions({"accuracy", "cost-complex-accuracy",  "cost-sensitive", "f1-score",
-                                          "group-fairness", "equality-of-opportunity", "prescriptive-policy",
-                                            "survival-analysis"})],
+        "optimization_task": [StrOptions({"accuracy", "cost-complex-accuracy", 
+                                          "regression", "cost-complex-regression", 
+                                          "piecewise-linear-regression", "simple-linear-regression",
+                                          "cost-sensitive", "f1-score", "prescriptive-policy", "instance-cost-sensitive",
+                                          "group-fairness", "equality-of-opportunity",
+                                          "survival-analysis"})],
         "max_depth": [Interval(numbers.Integral, 0, 20, closed="both")],
         "max_num_nodes": [Interval(numbers.Integral, 0, 1048575, closed="both"), None],
         "min_leaf_node_size": [Interval(numbers.Integral, 1, None, closed="left")],
         "time_limit": [Interval(numbers.Real, 0, None, closed="neither")],
         "cost_complexity": [Interval(numbers.Real, 0, 1, closed="both")],
         "feature_ordering": [StrOptions({"in-order", "gini"})],
         "upper_bound": [Interval(numbers.Real, 0, None, closed="left")],
@@ -243,14 +246,18 @@
             ValueError: If x or y is None or if they have different number of rows.
         """
         # Validate params and data
         self._validate_params()
         X = self._binarize_data(X, y, categorical)
         X, y = self._process_fit_data(X, y)
         extra_data = self._process_extra_data(X, extra_data)
+        # Store train data
+        self.train_X_ = X
+        self.train_y_ = y
+        self.train_extra_data_ = extra_data
 
         if self._should_reset_solver(X, y, extra_data):
             self._initialize_param_handler()
             self._solver = initialize_streed_solver(self._params)
         else:
             self._initialize_param_handler()
             self._solver._update_parameters(self._params)
@@ -349,15 +356,15 @@
         if feature_names is None:
             return f"Feature {feature}"
         feature_name = feature_names[feature]
         if " <= " in feature_name:
             feature_name, threshold = feature_name.split(" <= ")
             if len(threshold) >= 3:
                 threshold = _column_threshold(float(threshold))
-            return f"{feature_name} <= {threshold}"
+            return f"{feature_name} {self.__comparator} {threshold}"
         return feature_name
 
     def _recursive_print_tree(self, out, node, feature_names, label_names, ind=''):
         if node.is_leaf_node():
             label =  self._get_label_str(node.label, label_names)
             out.write(f"{ind}Label: {label}\n")
         else:
@@ -373,14 +380,15 @@
         If feature_names is not None, use the names in feature_names for pretty printing
         If label_names is not None, use the names in label_names for pretty printing (only for classification)
         """
         check_is_fitted(self, "tree_")
         
         if feature_names is None and hasattr(self, "feature_names_in_"):
             feature_names = self.feature_names_in_
+        self.__comparator = "<="
 
         if filename is None:
             self._recursive_print_tree(sys.stdout, self.tree_, feature_names, label_names)
         else:
             with open(filename, "w") as fh:
                 self._recursive_print_tree(fh, self.tree_, feature_names, label_names)
 
@@ -390,36 +398,46 @@
         If feature_names is not None, use the names in feature_names for pretty printing
         If label_names is not None, use the names in label_names for pretty printing (only for classification)
         """
         check_is_fitted(self, "tree_")
 
         if feature_names is None and hasattr(self, "feature_names_in_"):
             feature_names = self.feature_names_in_
+        train_data = (self.train_X_, self.train_y_, self.train_extra_data_)
+        self.__comparator = "&#8804;" # &#8804; is the <= character
 
-        with open(filename, "w") as fh:
+        with open(filename, "w", encoding="utf-8") as fh:
             fh.write("digraph Tree {\n")
             fh.write("node [shape=box, style=\"filled, rounded\", fontname=\"helvetica\", fontsize=\"8\"] ;\n")
             fh.write("edge [fontname=\"helvetica\", fontsize=\"6\"] ;\n")
-            self._recursive_export_dot(fh, self.tree_, 0, feature_names, label_names)
+            self._recursive_export_dot(fh, self.tree_, 0, feature_names, label_names, train_data)
             fh.write("}")
     
-    def _export_dot_leaf_node(self, fh, node, node_id, label_names, color=(200, 200, 200)):
+    def _export_dot_leaf_node(self, fh, node, node_id, label_names, train_data, color=(200, 200, 200)):
         label =  self._get_label_str(node.label, label_names)
         hex_color = "#{:02x}{:02x}{:02x}".format(*color)
         hex_line_color = "#{:02x}{:02x}{:02x}".format(*[int(0.4 * c) for c in color])
         fh.write(f"{node_id}  [label=\"{label}\", color=\"{hex_line_color}\" fillcolor=\"{hex_color}\"] ;\n")
 
-    def _recursive_export_dot(self, fh, node, node_id, feature_names, label_names):
+    def _recursive_export_dot(self, fh, node, node_id, feature_names, label_names, train_data):
         if node.is_leaf_node():
-            self._export_dot_leaf_node(fh, node, node_id, label_names)
+            self._export_dot_leaf_node(fh, node, node_id, label_names, train_data)
         else:
             predicate = self._get_predicate_str(node.feature, feature_names)
             fh.write(f"{node_id} [label=\"{predicate}\", color=\"#222222\", fillcolor=\"#EEEEEE\"] ;\n")
         if node_id > 0:
             parent_id = (node_id - 1) // 2
             feature_label = "True" if (node_id % 2) == 0 else "False"
             angle = 45 if feature_label == "True" else -45
             fh.write(f"{parent_id} -> {node_id} [labeldistance=2.5, labelangle={angle}, label=\"{feature_label}\"] ;\n")
 
         if node.is_branching_node():
-            self._recursive_export_dot(fh, node.left_child, node_id * 2 + 1, feature_names, label_names)
-            self._recursive_export_dot(fh, node.right_child, node_id * 2 + 2, feature_names, label_names)
+            left_data, right_data = self._split(train_data, node.feature)
+            self._recursive_export_dot(fh, node.left_child, node_id * 2 + 1, feature_names, label_names, left_data)
+            self._recursive_export_dot(fh, node.right_child, node_id * 2 + 2, feature_names, label_names, right_data)
+
+    def _split(self, data, feature):
+        x, y, ed = data
+        go_left = x[:, feature] == 0
+        left_data =  (x[ go_left], y[ go_left], [e for i, e in enumerate(ed) if go_left[i]])
+        right_data = (x[~go_left], y[~go_left], [e for i, e in enumerate(ed) if not go_left[i]])
+        return left_data, right_data
```

### Comparing `pystreed-1.2.3/pystreed/binarizer.py` & `pystreed-1.3.0/pystreed/binarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def get_column_types(X, categorical_columns=None):
     if categorical_columns is None: 
         categorical_columns = []
     binary_columns = []
     if isinstance(X, pd.DataFrame):
         categorical_columns = categorical_columns + [col for col in X.columns if not col in categorical_columns and not is_numeric_dtype(X[col])]
-        binary_columns = [col for col in X.columns if not set(np.unique(X[[col]])) - set([0,1])] 
+        binary_columns = [col for col in X.columns if not set(X[col].unique()) - set([0,1])] 
         continuous_columns = [col for col in X.columns if not col in categorical_columns and not col in binary_columns]
     elif isinstance(X, np.ndarray):
         binary_columns = [col for col in range(X.shape[1]) if not set(np.unique(X[:, col])) - set([0,1])]
         continuous_columns = [col for col in range(X.shape[1]) if not col in categorical_columns and not col in binary_columns]
     else:
         raise ValueError("X should be either a numpy array or a pandas data frame.")
     return binary_columns, categorical_columns, continuous_columns
@@ -98,14 +98,17 @@
             if len(self.categorical_columns) > 0:
                 X_cat = X[:, self.categorical_columns]
             if len(self.binary_columns) > 0:
                 X_bin = X[:, self.binary_columns]
             if len(self.continuous_columns) > 0:
                 X_cont = X[:, self.continuous_columns]
         if len(self.binary_columns) > 0:
+            if isinstance(X_bin, pd.DataFrame) and not is_numeric_dtype(X_bin):
+                X_bin.columns = [f"Binary Feature {i+1}" for i in range(X_bin.shape[1])] 
+                X = X.rename(str,axis="columns")
             parts.append(X_bin)
         if len(self.categorical_columns) > 0:
             X_cat = self.categorical_binarizer.transform(X_cat)
             parts.append(X_cat)
         if len(self.continuous_columns) > 0:
             X_cont = self.continuous_binarizer.transform(X_cont)
             parts.append(X_cont)
```

### Comparing `pystreed-1.2.3/pystreed/classification.py` & `pystreed-1.3.0/pystreed/classification.py`

 * *Files 13% similar despite different names*

```diff
@@ -80,16 +80,42 @@
             random_seed=random_seed,
             continuous_binarize_strategy=continuous_binarize_strategy,
             n_thresholds=n_thresholds,
             n_categories=n_categories)
         if optimization_task == "f1-score" and upper_bound != 2**31-1:
             warnings.warn(f"upper_bound parameter is ignored for f1-score", stacklevel=2)
         
-    def fit(self, X, y, extra_data=None):
+    def _initialize_param_handler(self):
+        super()._initialize_param_handler()
+        return self._params
+
+    def fit(self, X, y, extra_data=None, categorical=None):
+        """
+        Fits a STreeD Classification model to the given training data.
+
+        Args:
+            x : array-like, shape = (n_samples, n_features)
+            Data matrix
+
+            y : array-like, shape = (n_samples)
+            Target vector
+
+            extra_data : array-like, shape = (n_samples, n_data_items)
+            An array (optional) that represents extra data per instance
+
+            categorical : array-like, 
+            List of column names that are categorical
+
+        Returns:
+            BaseSTreeDSolver
+
+        Raises:
+            ValueError: If x or y is None or if they have different number of rows.
+        """
         self.n_classes_ = len(np.unique(y))
-        return super().fit(X, y, extra_data)
+        return super().fit(X, y, extra_data, categorical)
         
-    def _export_dot_leaf_node(self, fh, node, node_id, label_names):
+    def _export_dot_leaf_node(self, fh, node, node_id, label_names, train_data):
         if not hasattr(self, "_colors"):
             self._colors = _color_brew(self.n_classes_)
         color = self._colors[node.label]
-        return super()._export_dot_leaf_node(fh, node, node_id, label_names, color=color)
+        return super()._export_dot_leaf_node(fh, node, node_id, label_names, train_data, color=color)
```

### Comparing `pystreed-1.2.3/pystreed/cost_sensitive_classification.py` & `pystreed-1.3.0/pystreed/cost_sensitive_classification.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,36 +59,39 @@
     def _post_initialize_solver(self):
         super()._post_initialize_solver()
         self._solver.specify_costs(self.cost_specifier_)
 
     def _binarize_data(self, X, y=None, categorical_columns=None, reset=True):
         return X
 
-    def fit(self, X, y, cost_specifier : CostSpecifier):
+    def fit(self, X, y, cost_specifier : CostSpecifier, categorical=None):
         """
         Fits a STreeD model to the given training data.
 
         Args:
             X : array-like, shape = (n_samples, n_features)
             Data matrix
 
             y : array-like, shape = (n_samples)
             Target vector
 
             cost_specifier : CostSpecifier
             An object that describes the misclassification matrix and the feature cost function
 
+            categorical : array-like, 
+            List of column names that are categorical
+
         Returns:
             BaseSTreeDSolver
 
         Raises:
             ValueError: If x or y is None or if they have different number of rows.
         """
         self.n_classes_ = len(np.unique(y))
         self.cost_specifier_ = cost_specifier
-        return super().fit(X, y)
+        return super().fit(X, y, categorical)
         
-    def _export_dot_leaf_node(self, fh, node, node_id, label_names):
+    def _export_dot_leaf_node(self, fh, node, node_id, label_names, train_data):
         if not hasattr(self, "_colors"):
             self._colors = _color_brew(self.n_classes_)
         color = self._colors[node.label]
-        return super()._export_dot_leaf_node(fh, node, node_id, label_names, color=color)
+        return super()._export_dot_leaf_node(fh, node, node_id, label_names, train_data, color=color)
```

### Comparing `pystreed-1.2.3/pystreed/group_fair.py` & `pystreed-1.3.0/pystreed/group_fair.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,34 +101,37 @@
                  raise ValueError(f"Column {self.sensitive_feature} is not part of the data.")
             sensitive_column = X.pop(self.sensitive_feature) 
             X.insert(0, self.sensitive_feature, sensitive_column)
             return X
         else:
             raise ValueError(f"The sensitive feature column should be either an index or a string, but is {self.sensitive_feature} of type {type(self.sensitive_feature)}.")
 
-    def fit(self, X, y):
+    def fit(self, X, y, categorical=None):
         """
         Fits a STreeD model to the given training data.
 
         Args:
             x : array-like, shape = (n_samples, n_features)
             Data matrix
 
             y : array-like, shape = (n_samples)
             Target vector
 
+            categorical : array-like, 
+            List of column names that are categorical
+
         Returns:
             BaseSTreeDSolver
 
         Raises:
             ValueError: If x or y is None or if they have different number of rows.
         """
         self.n_classes_ = len(np.unique(y))
         X = self._move_sensitive_feature_first(X)
-        return super().fit(X, y)
+        return super().fit(X, y, categorical)
     
     def predict(self, X):
         """
         Predicts the target variable for the given input feature data.
 
         Args:
             x : array-like, shape = (n_samples, n_features)
@@ -153,12 +156,12 @@
 
         Returns:
             The score
         """
         X = self._move_sensitive_feature_first(X)
         return super().score(X, y_true)
         
-    def _export_dot_leaf_node(self, fh, node, node_id, label_names):
+    def _export_dot_leaf_node(self, fh, node, node_id, label_names, train_data):
         if not hasattr(self, "_colors"):
             self._colors = _color_brew(self.n_classes_)
         color = self._colors[node.label]
-        return super()._export_dot_leaf_node(fh, node, node_id, label_names, color=color)
+        return super()._export_dot_leaf_node(fh, node, node_id, label_names, train_data, color=color)
```

### Comparing `pystreed-1.2.3/pystreed/instance_cost_sensitive_classification.py` & `pystreed-1.3.0/pystreed/instance_cost_sensitive_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,25 +103,28 @@
         if reset or self.n_classes_ is None:
             self.n_classes_ = num_labels
         return np.array(y_out, dtype=np.intc), extra_data
 
     def _process_extra_data(self, X, extra_data):
         return extra_data
 
-    def fit(self, X, y):
+    def fit(self, X, y, categorical=None):
         """
         Fits a STreeD model to the given training data.
 
         Args:
             x : array-like, shape = (n_samples, n_features)
             Data matrix
 
             y : array-like with shape (n_samples, n_labels) 
             Cost vector. For each instance specify the classification costs per label
 
+            categorical : array-like, 
+            List of column names that are categorical
+
         Returns:
             STreeDInstanceCostSensitiveClassifier
 
         Raises:
             ValueError: If x or y is None or if they have different number of rows.
         """
         y, extra_data = self._check_data(y)
@@ -158,12 +161,12 @@
 
         Returns:
             The score
         """
         y_test, extra_data = self._check_data(y_test, reset=False)
         return super().score(X, y_test, extra_data)
 
-    def _export_dot_leaf_node(self, fh, node, node_id, label_names):
+    def _export_dot_leaf_node(self, fh, node, node_id, label_names, train_data):
         if not hasattr(self, "_colors"):
             self._colors = _color_brew(self.n_classes_)
         color = self._colors[node.label]
-        return super()._export_dot_leaf_node(fh, node, node_id, label_names, color=color)
+        return super()._export_dot_leaf_node(fh, node, node_id, label_names, train_data, color=color)
```

### Comparing `pystreed-1.2.3/pystreed/prescriptive_policy_generation.py` & `pystreed-1.3.0/pystreed/prescriptive_policy_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         if reset or self.n_classes_ is None:
             self.n_classes_ = len(np.unique(y_out))
         return np.array(y_out, dtype=np.intc), extra_data
 
     def _process_extra_data(self, X, extra_data):
         return extra_data
 
-    def fit(self, X, y):
+    def fit(self, X, y, categorical=None):
         """
         Fits a STreeD model to the given training data.
 
         Args:
             x : array-like, shape = (n_samples, n_features)
             Data matrix
 
@@ -140,22 +140,25 @@
             * Column 1 is the historic outcome y 
             * Column 2 is the propensity score mu
             * Column 3 .. 3+K-1 is the regress and compare y_hat prediction
             The rest of the data is optional (for testing)
             * Column 3 + K is the optimal treatment
             * Column 4 + K .. 4 + 2K - 1 is the counterfactual outcome y
 
+            categorical : array-like, 
+            List of column names that are categorical
+
         Returns:
             STreeDPrescriptivePolicyGenerator
 
         Raises:
             ValueError: If x or y is None or if they have different number of rows.
         """
         y, extra_data = self._check_data(y)
-        return super().fit(X, y, extra_data)
+        return super().fit(X, y, extra_data, categorical)
     
     def predict(self, X, extra_data=None):
         """
         Predicts the target variable for the given input feature data.
 
         Args:
             x : array-like, shape = (n_samples, n_features)
@@ -197,12 +200,12 @@
 
         Returns:
             The score
         """
         y_test, extra_data = self._check_data(y_test, reset=False)
         return super().score(X, y_test, extra_data)
 
-    def _export_dot_leaf_node(self, fh, node, node_id, label_names):
+    def _export_dot_leaf_node(self, fh, node, node_id, label_names, train_data):
         if not hasattr(self, "_colors"):
             self._colors = _color_brew(self.n_classes_)
         color = self._colors[node.label]
-        return super()._export_dot_leaf_node(fh, node, node_id, label_names, color=color)
+        return super()._export_dot_leaf_node(fh, node, node_id, label_names, train_data, color=color)
```

### Comparing `pystreed-1.2.3/pystreed/survival_analysis.py` & `pystreed-1.3.0/pystreed/survival_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,41 +85,44 @@
         """
         Preprocess the events into a list of SAData objects. Initialize the hazard value with -1
         """
         if events is None:
             return [SAData(1, -1.0) for x in X]    
         return [SAData(e, -1.0) for e in events]
 
-    def fit(self, X, y):
+    def fit(self, X, y, categorical=None):
         """
         Fits a STreeD survival tree model to the given training data.
 
          Parameters
         ----------
         X : array-like, shape = (n_samples, n_features)
             Data matrix
 
         y : structured array, shape = (n_samples,)
             A structured array containing the binary event indicator
             as first field, and time of event or time of censoring as
             second field.
 
+        categorical : array-like, 
+            List of column names that are categorical
+
         Returns
         -------
         self
         """
         if X.shape[0] != y.shape[0]:
             raise ValueError('x and y have different number of rows')
         events, times = check_array_survival(X, y)
         self._baseline_hazard_function = self._compute_baseline_cumulative_hazard_function(events, times)
         self.unique_times_, self.is_event_time_ = get_unique_times(times, events)
         self.n_outputs_ = self.unique_times_.shape[0]
         self.n_classes_ = np.ones(self.n_outputs_, dtype=np.intp) * 2
 
-        return super().fit(X, times, events)
+        return super().fit(X, times, events, categorical)
     
     def score(self, X, y_true):
         """
         Computes the score for the given input feature data and the true
 
         Args:
             x : array-like, shape = (n_samples, n_features)
@@ -339,15 +342,15 @@
         arr = np.array([
                 [math.exp(-theta * self._baseline_hazard_function(t)) for t in self.unique_times_]
                  for theta in thetas])
         if return_array: return arr
         return _array_to_step_function(self.unique_times_, arr)
     
 
-    def _export_dot_leaf_node(self, fh, node, node_id, label_names):
+    def _export_dot_leaf_node(self, fh, node, node_id, label_names, train_data):
         try:
             import matplotlib.pyplot as plt
             theta = node.label
             arr = np.array([[math.exp(-theta * self._baseline_hazard_function(t)) for t in self.unique_times_]])
             fn = _array_to_step_function(self.unique_times_, arr)[0]
             plt.figure(figsize=(2,2))
             plt.step(fn.x, fn(fn.x), where="post")
@@ -356,15 +359,15 @@
             plt.xlabel("time $t$")
             filename = self.__export_directory / f"leaf_KM_{node_id}.png"
             if not os.path.exists(self.__export_directory):
                 os.makedirs(self.__export_directory)
             plt.savefig(filename, dpi=300, bbox_inches="tight")
             fh.write(f"{node_id}  [label=\"\", image=\"{filename}\", width=2, height=2, fixedsize=true] ;\n")
         except:
-            return super()._export_dot_leaf_node(fh, node, node_id, label_names)
+            return super()._export_dot_leaf_node(fh, node, node_id, label_names, train_data)
 
 
     def export_dot(self, filename, feature_names=None, label_names=None):
         """
         Export the tree as a .dot file (for plotting)
         """
         self.__export_directory = Path(filename).parent.absolute() / "leaf-distributions"
```

### Comparing `pystreed-1.2.3/pystreed/utils.py` & `pystreed-1.3.0/pystreed/utils.py`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/pystreed.egg-info/PKG-INFO` & `pystreed-1.3.0/pystreed.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystreed
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python Implementation of STreeD: Dynamic Programming Approach for Optimal Decision Trees with Separable objectives and Constraints
 Author-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>, Emir Demirović <E.Demirovic@tudelft.nl>, "Mathijs M. de Weerdt" <M.M.deWeerdt@tudelft.nl>
 Maintainer-email: "Jacobus G. M. van der Linden" <J.G.M.vanderLinden@tudelft.nl>
 License: Copyright 2023 Jacobus G. M. van der Linden, Delft University of Technology
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -31,15 +31,17 @@
 
 # STreeD: Separable Trees with Dynamic programming
 By: Jacobus G. M. van der Linden [(e-mail)](mailto:J.G.M.vanderLinden@tudelft.nl)
 
 STreeD is a framework for optimal binary decision trees with _separable_ optimization tasks. A separable optimization task is a task that can be optimized separately for the left and right subtree. The current STreeD Framework implements a broad set of such optimization tasks, from group fairness constraints to survival analysis. For an explanation of each application, see below.
 For details on what tasks are separable and how the algoritm works, see our paper.
 
-* Van der Linden, Jacobus G. M., Mathijs M. de Weerdt, and Emir Demirović. "Necessary and Sufficient Conditions for Optimal Decision Trees using Dynamic Programming." _Advances in Neural Information Processing Systems_ (Accepted, not published). 2023. [pdf](https://arxiv.org/pdf/2305.19706) 
+If you use STreeD, please cite our paper:
+
+* Van der Linden, Jacobus G. M., Mathijs M. de Weerdt, and Emir Demirović. "Necessary and Sufficient Conditions for Optimal Decision Trees using Dynamic Programming." _Advances in Neural Information Processing Systems_. 2023. [pdf](https://proceedings.neurips.cc/paper_files/paper/2023/file/1d5fce9627e15c84db572a66e029b1fc-Paper-Conference.pdf) 
 
 ## Python usage
 
 ### Install from PyPi
 The `pystreed` python package can be installed from PyPi using `pip`:
 
 ```sh
@@ -127,15 +129,15 @@
 Currently, STreeD implements the following optimization tasks:
 
 ### Classification
 `STreeDClassifier` implements the following optimization tasks:
 
 * `accuracy`: Minimizes the misclassification score. 
 * `cost-complex-accuracy`: Minimizes the misclassification score plus the cost for adding a branching node by the parameter `cost_complexity`.
-* `f1-score`: Minimizes the F1-score.
+* `f1-score`: Maximizes the F1-score.
 
 See [examples/accuracy_example.py](examples/accuracy_example.py) for an example.
 
 ### Cost-Sensitive Classification
 `STreeDCostSensitiveClassifier` implements a cost-sensitive classifier. Costs can both be attributed to features and misclassifications.
 
 The costs can be specified with `CostSpecifier` object. This object is either initialized with a file name for the cost specification and the number of classes; or with the misclassification cost matrix, and the cost specifier per feature. When testing a feature in a branch node, the cost for that feature is paid for every instance that passes through it. When another feature from the same group was tested before, the discounted cost is paid. When another feature that is binarized from the same original feature is already tested, the cost is zero.
@@ -165,39 +167,64 @@
 
 See [examples/group_fair_example.py](examples/group_fair_example.py) for an example.
 
 ### Prescriptive policy generation
 `STreeDPrescriptivePolicyGenerator` implements a policy generation solver. Counterfactual scores need to be provided. The current implementation allows for three different teacher methods, as specified by the `teacher_method` parameter:
 * `DM`: the _direct method_ or _Regress & Compare_ method. This teacher specifies for every treatment (label) what the expected outcome is.
 * `IPW`: the _inverse propensity weighting_ method. This teacher provides the propensity scores mu(x, k): the probability of treatment k happening for feature vector x.
-* `DR`: the _doubly robust_ method: a combination of the direct methodand the inverse propensity weighting method.
+* `DR`: the _doubly robust_ method: a combination of the direct method and the inverse propensity weighting method.
 
 The teacher data needs to be passed to the solver by initializing a `PPGData` object for every instance. The PPGData initializer expects the following parameters:
 * `historic_treatment : int` : the historic treatment label
 * `historic_outcome : float` : the historic outcome
 * `propensity_score : float` : the propensity score for the historic treatment
 * `predicted_outcome : List[float]` : the _regress & compare_ prediction for each possible treatment
 Optional (for testing)
 * `optimal_treatment : int` : the optimal treatment
 * `counterfactual_outcome : List[float]` : the counterfactual outcome 
 
 Only the data which will be used by the teacher method needs to be specified, the rest can be initialized with zero's.
 
 See [examples/prescriptive_policy_example.py](examples/prescriptive_policy_example.py) for an example.
 
+### Regression
+
+`STreeDRegressor` implements two variants of regression, as specified by the optimization task parameter
+* `regression`: Miminimizes the _sum of squared errors_.
+* `cost-complex-regression`: Minimizes the _sum of squared errors_ plus the cost for adding a branching node by the parameter `cost_complexity`. For runtime improvement, custom lower bounds can be specified if `use_task_lower_bound=True`. The custom lower bound `regression_bound` can be set to either `"equivalent"` to use the equivalent-points bound or `"kmeans"` to use a k-means lower bound.
+
+See [examples/regression_example.py](examples/regression_example.py) for an example.
+
+If you use STreeD for _regression_, please cite our paper:
+
+* Van den Bos, M., Jacobus G. M. van der Linden, and Emir Demirović. "Piecewise Constant and Linear Regression Trees: An Optimal Dynamic Programming Approach." In _Proceedings of ICML-24_, 2024.
+
+### Piecewise Linear Regression
+`STreeDPiecewiseLinearRegressor` implements a solver for optimizing piecewise linear regression trees, with a linear elastic net regression predictor in every leaf node. The lasso and ridge penalization can be set with the `lasso_penalty` and `ridge_penalty` and parameters. The addition of a new branching node is penalized by the `cost_complexity` parameter. Alternatively, `STreeDPiecewiseLinearRegressor` can learn a simple linear regression model in every leaf by setting `simple = True`. The simple linear regression model is penalized only with the ridge penalization.
+
+`STreeDPiecewiseLinearRegressor` only uses the continuous features for fitting the linear lasso regression model in every leaf node. These continuous features can be automatically inferred from the data or explicitly specified using the `continuous_columns` parameter of the `fit` method.
+
+To prevent fitting linear models on too little data, `STreeDPiecewiseLinearRegressor` by default sets the `min_leaf_node_size` parameter to at least 5 times the number of continuous features or to at least 5 when fitting a simple linear regression model.
+
+See [examples/piecewise_linear_regression_example.py](examples/piecewise_linear_regression_example.py) for an example.
+
+If you use STreeD for _piecewise linear regression_, please cite our paper:
+
+* Van den Bos, M., Jacobus G. M. van der Linden, and Emir Demirović. "Piecewise Constant and Linear Regression Trees: An Optimal Dynamic Programming Approach." In _Proceedings of ICML-24_, 2024.
+
 ### Survival analysis
-`STreeDSurvivalAnalysis` implements an optimal survival tree method, by optimizing the proportional hazard function of LeBlanc and Crowly, "Relative Risk for Censored Survival Data," _Biometrics_ 48.2 (1992): 411-425. Each leaf node predicts a risk factor $\theta$ which is used to shift the base hazard model $\hat{\Lambda}(t)$.  The Kaplan-Meier estimator is used as a stepwise survival function $\hat{S}(t) = e^{-\theta \hat{\Lambda}(t)}$.
+`STreeDSurvivalAnalysis` implements an optimal survival tree method, by optimizing the proportional hazard function of LeBlanc and Crowly, "Relative Risk for Censored Survival Data," _Biometrics_ 48.2 (1992): 411-425. Each leaf node predicts a risk factor $\theta$ which is used to shift the base hazard model $\hat{\Lambda}(t)$.  The Nelson-Aalen estimator is used as a stepwise survival function $\hat{S}(t) = e^{-\theta \hat{\Lambda}(t)}$.
 
 Instead of a label, the input data expects a two-dimensional array with for each instance 1) a binary censoring indicator and 2) a time-of-event (death or censoring).
 
 See [examples/survival_analysis_example.py](examples/survival_analysis_example.py) for an example.
 
 If you use STreeD for _survival analysis_, please cite our paper:
 
-* Huisman, T., Jacobus G. M. van der Linden, and Emir Demirović. "Optimal Survival Trees: A Dynamic Programming Approach." _Proceedings of AAAI-24_ (Accepted, not published). 2024. 
+* Huisman, T., Jacobus G. M. van der Linden, and Emir Demirović. "Optimal Survival Trees: A Dynamic Programming Approach." _Proceedings of AAAI-24_. 2024. [pdf](https://arxiv.org/pdf/2401.04489.pdf)
 
 ## Parameters
 STreeD can be configured by the following parameters:
 * `max_depth` : The maximum depth of the tree. Note that a tree of depth zero has a single leaf node. A tree of depth one has one branching node and two leaf nodes.
 * `max_num_nodes` : The maximum number of _branching_ nodes in the tree.
 * `min_leaf_node_size` : The minimum number of samples required in each leaf node.
 * `time_limit` : The run time limit in seconds. If the time limit is exceeded a possibly non-optimal tree is returned.
```

### Comparing `pystreed-1.2.3/pystreed.egg-info/SOURCES.txt` & `pystreed-1.3.0/pystreed.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pystreed/binarizer.py
 pystreed/classification.py
 pystreed/cost_sensitive_classification.py
 pystreed/data.py
 pystreed/group_fair.py
 pystreed/instance_cost_sensitive_classification.py
 pystreed/prescriptive_policy_generation.py
+pystreed/regression.py
 pystreed/survival_analysis.py
 pystreed/utils.py
 pystreed.egg-info/PKG-INFO
 pystreed.egg-info/SOURCES.txt
 pystreed.egg-info/dependency_links.txt
 pystreed.egg-info/requires.txt
 pystreed.egg-info/top_level.txt
@@ -43,11 +44,18 @@
 src/tasks/group_fairness.cpp
 src/tasks/instance_cost_sensitive.cpp
 src/tasks/optimization_task.cpp
 src/tasks/prescriptive_policy.cpp
 src/tasks/survival_analysis.cpp
 src/tasks/accuracy/accuracy.cpp
 src/tasks/accuracy/cost_complex_accuracy.cpp
+src/tasks/regression/cost_complex_regression.cpp
+src/tasks/regression/piecewise_linear_regression.cpp
+src/tasks/regression/piecewise_simple_linear_regression.cpp
+src/tasks/regression/regression.cpp
+src/tasks/regression/ckmeans/Ckmeans.1d.dp.cpp
+src/tasks/regression/ckmeans/fill_SMAWK.cpp
+src/tasks/regression/ckmeans/fill_log_linear.cpp
 src/utils/file_reader.cpp
 src/utils/key_value_heap.cpp
 src/utils/parameter_handler.cpp
 src/utils/utils.cpp
```

### Comparing `pystreed-1.2.3/setup.py` & `pystreed-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 from glob import glob
 
 # Define package metadata
 package_name = 'pystreed'
 extension_name = 'cstreed'
-__version__ = "1.2.3"
+__version__ = "1.3.0"
 
 ext_modules = [
     Pybind11Extension(package_name + '.' + extension_name,
         sorted(glob("src/**/*.cpp", recursive = True)),
         include_dirs = ["include"],
         define_macros = [('VERSION_INFO', __version__)], # passing in the version to the compiled code
         language='c++',
```

### Comparing `pystreed-1.2.3/src/bindings.cpp` & `pystreed-1.3.0/src/bindings.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,34 @@
 
 namespace py = pybind11;
 using namespace STreeD;
 
 enum task_type {
     accuracy,
     cost_complex_accuracy,
+    regression,
+    cost_complex_regression,
+    spwl_regression,
+    pwl_regression,
     cost_sensitive,
     instance_cost_sensitive,
     f1score,
     group_fairness,
     equality_of_opportunity,
     prescriptive_policy,
     survival_analysis
 };
 
 task_type get_task_type_code(std::string& task) {
     if (task == "accuracy") return accuracy;
     else if (task == "cost-complex-accuracy") return cost_complex_accuracy;
+    else if (task == "regression") return regression;
+    else if (task == "cost-complex-regression") return cost_complex_regression;
+    else if (task == "simple-linear-regression") return spwl_regression;
+    else if (task == "piecewise-linear-regression") return pwl_regression;
     else if (task == "cost-sensitive") return cost_sensitive;
     else if (task == "instance-cost-sensitive") return instance_cost_sensitive;
     else if (task == "f1-score") return f1score;
     else if (task == "group-fairness") return group_fairness;
     else if (task == "equality-of-opportunity") return equality_of_opportunity;
     else if (task == "prescriptive-policy") return prescriptive_policy;
     else if (task == "survival-analysis") return survival_analysis;
@@ -242,25 +250,33 @@
     ExposeIntegerProperty(parameter_handler, "min-leaf-node-size", "min_leaf_node_size");
     ExposeBooleanProperty(parameter_handler, "use-branch-caching", "use_branch_caching");
     ExposeBooleanProperty(parameter_handler, "use-dataset-caching", "use_dataset_caching");
     ExposeBooleanProperty(parameter_handler, "use-terminal-solver", "use_terminal_solver");
     ExposeBooleanProperty(parameter_handler, "use-similarity-lower-bound", "use_similarity_lower_bound");
     ExposeBooleanProperty(parameter_handler, "use-upper-bound", "use_upper_bound");
     ExposeBooleanProperty(parameter_handler, "use-lower-bound", "use_lower_bound");
+    ExposeBooleanProperty(parameter_handler, "use-task-lower-bound", "use_task_lower_bound");
     ExposeFloatProperty(parameter_handler, "upper-bound", "upper_bound");
     ExposeStringProperty(parameter_handler, "ppg-teacher-method", "ppg_teacher_method");
+    ExposeFloatProperty(parameter_handler, "lasso-penalty", "lasso_penalty");
+    ExposeFloatProperty(parameter_handler, "ridge-penalty", "ridge_penalty");
+    ExposeStringProperty(parameter_handler, "regression-bound", "regression_lower_bound");
     ExposeFloatProperty(parameter_handler, "discrimination-limit", "discrimination_limit");
     
     /*************************************
            Solver
      ************************************/
 
     DefineSolver<Accuracy>(m, "Accuracy");
     DefineSolver<CostComplexAccuracy>(m, "CostComplexAccuracy");
     DefineSolver<F1Score>(m, "F1Score");
+    DefineSolver<Regression>(m, "Regression");
+    DefineSolver<CostComplexRegression>(m, "CostComplexRegression");
+    DefineSolver<SimpleLinearRegression>(m, "SimpleLinearRegression");
+    DefineSolver<PieceWiseLinearRegression>(m, "PieceWiseLinearRegression");
     DefineSolver<SurvivalAnalysis>(m, "Survival");
     DefineSolver<PrescriptivePolicy>(m, "PrescriptivePolicy");
     DefineSolver<GroupFairness>(m, "GroupFairness");
     DefineSolver<EqOpp>(m, "EqOpp");
     DefineSolver<InstanceCostSensitive>(m, "InstanceCostSensitive");
     py::class_<Solver<CostSensitive>> cost_sensitive_solver = DefineSolver<CostSensitive>(m, "CostSensitive");
     cost_sensitive_solver.def("specify_costs", [](Solver<CostSensitive>& solver, const CostSpecifier& cost_specifier) {
@@ -282,24 +298,30 @@
 	    bool verbose = parameters.GetBooleanParameter("verbose");
 
         STreeD::AbstractSolver* solver;
         std::string task = parameters.GetStringParameter("task");
         switch(get_task_type_code(task)) {
             case accuracy: solver = new Solver<Accuracy>(parameters, &rng); break;
             case cost_complex_accuracy: solver = new Solver<CostComplexAccuracy>(parameters, &rng); break;
+            case regression: solver = new Solver<Regression>(parameters, &rng); break;
+            case cost_complex_regression: solver = new Solver<CostComplexRegression>(parameters, &rng); break;
+            case spwl_regression: solver = new Solver<SimpleLinearRegression>(parameters, &rng); break;
+            case pwl_regression: solver = new Solver<PieceWiseLinearRegression>(parameters, &rng); break;
             case cost_sensitive: solver = new Solver<CostSensitive>(parameters, &rng); break;
             case instance_cost_sensitive: solver = new Solver<InstanceCostSensitive>(parameters, &rng); break;
             case f1score: solver = new Solver<F1Score>(parameters, &rng); break;
             case group_fairness: solver = new Solver<GroupFairness>(parameters, &rng); break;
             case equality_of_opportunity: solver = new Solver<EqOpp>(parameters, &rng); break;
             case prescriptive_policy: solver = new Solver<PrescriptivePolicy>(parameters, &rng); break;
             case survival_analysis: solver = new Solver<SurvivalAnalysis>(parameters, &rng); break;
         }
         return solver;
     }, py::keep_alive<0, 1>());
+
+
     
     /*************************************
            Extra Data
      ************************************/
 
     py::class_<SAData>(m, "SAData")
         .def(py::init<int, double>())
@@ -312,20 +334,29 @@
         .def(py::init<>())
         .def_readonly("historic_treatment", &PPGData::k)
         .def_readonly("historic_outcome", &PPGData::y)
         .def_readonly("propensity_score", &PPGData::mu)
         .def_readonly("predicted_outcome", &PPGData::yhat)
         .def_readonly("optimal_treatment", &PPGData::k_opt)
         .def_readonly("counterfactual_outcome", &PPGData::cf_y);
-       
+
     py::class_<InstanceCostSensitiveData>(m, "CostVector")
         .def(py::init<std::vector<double>&>())
         .def(py::init<>())
         .def_readonly("costs", &InstanceCostSensitiveData::costs);
 
+    py::class_<PieceWiseLinearRegExtraData>(m, "ContinuousFeatureData")
+        .def(py::init<const std::vector<double>&>())
+        .def_readonly("feature_data", &PieceWiseLinearRegExtraData::x);
+
+    py::class_<SimpleLinRegExtraData>(m, "SimpleContinuousFeatureData")
+        .def(py::init<const std::vector<double>&>())
+        .def_readonly("feature_data", &PieceWiseLinearRegExtraData::x);
+
+        
     /*************************************
            Label
      ************************************/
     py::class_<FeatureCostSpecifier>(m, "FeatureCostSpecifier")
         .def(py::init<double, double, const std::string&, int, int>())
         .def_readonly("feature_cost", &FeatureCostSpecifier::feature_cost)
         .def_readonly("discount_cost", &FeatureCostSpecifier::discount_cost)
@@ -334,8 +365,21 @@
         .def_readonly("binary_end", &FeatureCostSpecifier::binary_end)
         .def("__str__", &FeatureCostSpecifier::ToString);
     
     py::class_<CostSpecifier>(m, "CostSpecifier")
         .def(py::init<const std::string&, int>())
         .def(py::init<const std::vector<std::vector<double>>&, const std::vector<FeatureCostSpecifier>&>());
     
+    /*************************************
+           Label
+     ************************************/
+
+    py::class_<LinearModel>(m, "LinearModel")
+        .def_readonly("coefficients", &LinearModel::b)
+        .def_readonly("intercept", &LinearModel::b0)
+        .def("__str__", &LinearModel::ToString)
+        .def("__call__", [](const LinearModel& model, const py::array_t<int, py::array::c_style>& _X, const PieceWiseLinearRegExtraData& extra_data) -> double {
+            const auto fv = NumpyRowToBoolVector(_X);
+            Instance<double, PieceWiseLinearRegExtraData> instance(0, fv, 0, extra_data);
+            return model.Predict(&instance);
+        });
 }
```

### Comparing `pystreed-1.2.3/src/main.cpp` & `pystreed-1.3.0/src/main.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -44,14 +44,26 @@
 	if (verbose) { std::cout << "Reading data...\n"; }
 	if (task == "accuracy") {
 		solver = new STreeD::Solver<STreeD::Accuracy>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::Accuracy>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "cost-complex-accuracy") {
 		solver =  new STreeD::Solver<STreeD::CostComplexAccuracy>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::CostComplexAccuracy>(parameters, data, train_data, test_data, &rng);
+	} else if (task == "regression") {
+		solver =  new STreeD::Solver<STreeD::Regression>(parameters, &rng);
+		STreeD::FileReader::ReadData<STreeD::Regression>(parameters, data, train_data, test_data, &rng);
+	} else if (task == "cost-complex-regression") {
+		solver =  new STreeD::Solver<STreeD::CostComplexRegression>(parameters, &rng);
+		STreeD::FileReader::ReadData<STreeD::CostComplexRegression>(parameters, data, train_data, test_data, &rng);
+	} else if (task == "piecewise-linear-regression") {
+		solver = new STreeD::Solver<STreeD::PieceWiseLinearRegression>(parameters, &rng);
+		STreeD::FileReader::ReadData<STreeD::PieceWiseLinearRegression>(parameters, data, train_data, test_data, &rng);
+	} else if (task == "simple-linear-regression") {
+		solver = new STreeD::Solver<STreeD::SimpleLinearRegression>(parameters, &rng);
+		STreeD::FileReader::ReadData<STreeD::SimpleLinearRegression>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "cost-sensitive") {
 		solver =  new STreeD::Solver<STreeD::CostSensitive>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::CostSensitive>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "instance-cost-sensitive") {
 		solver = new STreeD::Solver<STreeD::InstanceCostSensitive>(parameters, &rng);
 		STreeD::FileReader::ReadData<STreeD::InstanceCostSensitive>(parameters, data, train_data, test_data, &rng);
 	} else if (task == "f1-score") {
@@ -87,15 +99,19 @@
 	auto test_result = solver->TestPerformance(result, test_data);
 	// report results
 	std::cout << "TIME: " << stopwatch.TimeElapsedInSeconds() << " seconds\n";
 	std::cout << "CLOCKS FOR SOLVE: " << ((double)clock() - (double)clock_before_solve) / CLOCKS_PER_SEC << "\n";
 
 
 	if (verbose) {
-		if (result->IsFeasible()) {
+		if (result->NumSolutions() > 0) {
+			if (!result->IsProvenOptimal()) {
+				std::cout << std::endl << "Warning: No proof of optimality. Results are best solution found before the time-out." << std::endl << std::endl;
+			}
+
 			std::cout << "Solutions: " << result->NumSolutions() << " \tD\tN\t\tTrain \t\tTest\t\tAvg. Path length" << std::endl;
 			for (int i = 0; i < result->NumSolutions(); i++) {
 				auto train_score = result->scores[i];
 				auto test_score = test_result->scores[i];
 				std::cout << "Solution " << i << ": \t" << std::setw(2) << result->depths[i] << " \t" << result->num_nodes[i] << " \t\t";
 				std::cout << std::setprecision (std::numeric_limits<double>::digits10 + 1) << train_score->score << " \t";
 				std::cout << std::setprecision (std::numeric_limits<double>::digits10 + 1) << test_score->score << " \t";
```

### Comparing `pystreed-1.2.3/src/model/branch.cpp` & `pystreed-1.3.0/src/model/branch.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/model/data.cpp` & `pystreed-1.3.0/src/model/data.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 		right.data = data;
 		left.instances.resize(NumLabels());
 		right.instances.resize(NumLabels());
 		left.size = 0;
 		right.size = 0;
 		//std::vector<std::vector<std::vector<int>>> label_indices(NumLabels(), std::vector<std::vector<int>>(2)); // second index: 0=left, 1=right
 		for (int label = 0; label < NumLabels(); label++) {
-			for (auto& instance : GetInstancesForLabel(label)) {
+			auto& _instances = GetInstancesForLabel(label);
+			for (auto& instance : _instances) {
 				if (instance->IsFeaturePresent(feature)) {
 					right.instances[label].push_back(instance);
 				} else {
 					left.instances[label].push_back(instance);
 				}
 			}
 			left.size += int(left.instances[label].size());
 			right.size += int(right.instances[label].size());
-			runtime_assert(left.instances[label].size() + right.instances[label].size() == instances[label].size());
+			runtime_assert(left.instances[label].size() + right.instances[label].size() == _instances.size());
 		}
 		runtime_assert(left.size + right.size == size);
 	}
 
 	template<class LT>
 	void ADataView::TrainTestSplitData(const ADataView& data, ADataView& train, ADataView& test, std::default_random_engine* rng, double test_percentage, bool stratify) {
 		runtime_assert(test_percentage >= 0.0 && test_percentage <= 1.0);
```

### Comparing `pystreed-1.2.3/src/model/feature_vector.cpp` & `pystreed-1.3.0/src/model/feature_vector.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/solver/branch_cache.cpp` & `pystreed-1.3.0/src/solver/branch_cache.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,20 @@
 			count += c.size();
 		}
 		return int(count);
 	}
 
 	template class BranchCache<Accuracy>;
 	template class BranchCache<CostComplexAccuracy>;
-	
+
+	template class BranchCache<Regression>;
+	template class BranchCache<CostComplexRegression>;
+	template class BranchCache<PieceWiseLinearRegression>;
+	template class BranchCache<SimpleLinearRegression>;
+
 	template class BranchCache<CostSensitive>;
 	template class BranchCache<InstanceCostSensitive>;
 	template class BranchCache<F1Score>;
 	template class BranchCache<GroupFairness>;
 	template class BranchCache<EqOpp>;
 	template class BranchCache<PrescriptivePolicy>;
 	template class BranchCache<SurvivalAnalysis>;
```

### Comparing `pystreed-1.2.3/src/solver/cache.cpp` & `pystreed-1.3.0/src/solver/cache.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 		if (use_branch_caching) branch_cache.TransferAssignmentsForEquivalentBranches(data_source, branch_source, data_destination, branch_destination);
 		// Dataset caching do not need to transfer equivalent branches
 	}
 
 	template class Cache<Accuracy>;
 	template class Cache<CostComplexAccuracy>;
 
+	template class Cache<Regression>;
+	template class Cache<CostComplexRegression>;
+	template class Cache<PieceWiseLinearRegression>;
+	template class Cache<SimpleLinearRegression>;
+
 	template class Cache<CostSensitive>;
 	template class Cache<InstanceCostSensitive>;
 	template class Cache<F1Score>;
 	template class Cache<GroupFairness>;
 	template class Cache<EqOpp>;
 	template class Cache<PrescriptivePolicy>;
 	template class Cache<SurvivalAnalysis>;
```

### Comparing `pystreed-1.2.3/src/solver/cost_combiner.cpp` & `pystreed-1.3.0/src/solver/cost_combiner.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,18 @@
 	template <class OT, bool update_count, bool update_cost> void UpdateCountCost(
 		const AInstance* data_point,
 		CostStorage<OT>& _cost_storage,
 		Counter& counter,
 		typename OT::SolD2Type& costs,
 		int multiplier,
 		bool only_one_dimension) {
+		
+		if constexpr (OT::use_weights) {
+			multiplier *= int(data_point->GetWeight());
+		}
 
 		const int num_present_features = data_point->NumPresentFeatures();
 		if constexpr (update_cost) {
 			_cost_storage.UpdateTotalCosts(costs);
 		}
 
 		if (only_one_dimension) {
@@ -131,19 +135,24 @@
 						UpdateCountCost<OT, true, false>(data_point, _cost_storage, counter, costs, multiplier, only_one_dimension);
 					} else if (label > 0) {
 						UpdateCountCost<OT, false, true>(data_point, _cost_storage, counter, costs, multiplier, only_one_dimension);
 					} else {
 						UpdateCountCost<OT, true, true>(data_point, _cost_storage, counter, costs, multiplier, only_one_dimension);
 					}
 				}
+				if constexpr (OT::use_weights) {
+					counter.UpdateTotalCount(int(data_point->GetWeight() * multiplier));
+				}
 			}
 			
 
 		}
-		counter.UpdateTotalCount(int(data.Size() * multiplier));			
+		if constexpr (!OT::use_weights) {
+			counter.UpdateTotalCount(int(data.Size() * multiplier));
+		}
 	}
 
 	template <class OT>
 	void CostCalculator<OT>::UpdateCostsReconstruct(const ADataView& data, int feature) {
 		typename CostCalculator<OT>::SolD2Type costs; // dummy values
 		for (int org_label = 0; org_label < data.NumLabels(); org_label++) {
 			for (auto& data_point : data.GetInstancesForLabel(org_label)) {
@@ -168,32 +177,32 @@
 						int feature2 = data_point->GetJthPresentFeature(j);
 						if (feature1 == feature2) continue;
 						if (feature1 > feature2) std::swap(feature1, feature2);
 						_cost_storage.UpdateCosts(feature1, feature2, costs);
 					}
 				}
 				
-				
+				int weight = int(data_point->GetWeight());
+				counter.UpdateTotalCount(weight);
 				for (int j = 0; j < num_present_features; j++) {
 					int feature2 = data_point->GetJthPresentFeature(j);
-					counter.UpdateCount(feature2, feature2, +1);
+					counter.UpdateCount(feature2, feature2, weight);
 				}
 				if (!feature_is_present) continue;
 				for (int j = 0; j < num_present_features; j++) {
 					int feature1 = feature;
 					int feature2 = data_point->GetJthPresentFeature(j);
 					if (feature1 == feature2) continue;
 					if (feature1 > feature2) std::swap(feature1, feature2);
-					counter.UpdateCount(feature1, feature2, +1);
+					counter.UpdateCount(feature1, feature2, weight);
 				}
 			}
 
-
 		}
-		counter.UpdateTotalCount(int(data.Size()));
+		
 	}
 
 	template <class OT>
 	void CostCalculator<OT>::UpdateBranchingCosts(const ADataView& data, const typename CostCalculator<OT>::Context& context) {
 		if constexpr (OT::has_branching_costs) {
 
 			if constexpr (OT::element_branching_costs) {
@@ -230,47 +239,65 @@
 			return task->ComputeD2BranchingCosts(branching_costs[f1][f1], counter.GetTotalCount());
 		} else {
 			return CostCalculator<OT>::SolType();
 		}
 	}
 
 	template <class OT>
-	const typename CostCalculator<OT>::SolType CostCalculator<OT>::GetBranchingCosts0(int f1, int f2) const {
+	const typename CostCalculator<OT>::SolType CostCalculator<OT>::GetBranchingCosts0(int count0, int f1, int f2) const {
 		if constexpr (OT::has_branching_costs) {
-			return task->ComputeD2BranchingCosts(branching_costs[f1][f2], GetCount00(f1, f1));
+			return task->ComputeD2BranchingCosts(branching_costs[f1][f2], count0);
 		} else {
 			return CostCalculator<OT>::SolType();
 		}
 	}
 
 	template <class OT>
-	const typename CostCalculator<OT>::SolType CostCalculator<OT>::GetBranchingCosts1(int f1, int f2) const {
+	const typename CostCalculator<OT>::SolType CostCalculator<OT>::GetBranchingCosts1(int count1, int f1, int f2) const {
 		if constexpr (OT::has_branching_costs) {
-			return task->ComputeD2BranchingCosts(branching_costs[f1][f2], GetCount11(f1, f1));
+			return task->ComputeD2BranchingCosts(branching_costs[f1][f2], count1);
 		} else {
 			return CostCalculator<OT>::SolType();
 		}
 	}
 
 	template <class OT>
+	void CostCalculator<OT>::CalcLeafSol(SolType& sol, int label, SolLabelType& label_out) const {
+		const auto& _cost_storage = cost_storage[label];
+		const auto& total_costs = _cost_storage.GetTotalCosts();
+		int count = counter.GetTotalCount();
+		task->ComputeD2Costs(total_costs, count, sol);
+		if constexpr (OT::custom_get_label || std::is_same<typename OT::LabelType, double>::value) {
+			label_out = GetLabel(label, total_costs, count);
+		} else {
+			label_out = label;
+		}
+	}
+
+	template <class OT>
 	void CostCalculator<OT>::CalcSols(const Counts& counts, Sols<OT>& sols, int label, int f1, int f2) const {
 		bool swap = f1 > f2;
 		if (swap) std::swap(f1, f2);
 		const auto& _cost_storage = cost_storage[label];
 		const auto& total_costs = _cost_storage.GetTotalCosts();
 		const auto& costsf1f2 = _cost_storage.GetCosts(f1, f2);
 		const auto& costsf1f1 = _cost_storage.GetCosts(f1, f1);
 		const auto& costsf2f2 = _cost_storage.GetCosts(f2, f2);
 
 		if (f1 == f2) {
 			task->ComputeD2Costs(total_costs - costsf1f2, counts.count00, sols.sol00);
 			task->ComputeD2Costs(costsf1f2, counts.count11, sols.sol11);
 			return;
 		}
-		task->ComputeD2Costs((total_costs + costsf1f2) - costsf1f1 - costsf2f2 , counts.count00, sols.sol00);
+		temp_costs1 = total_costs;
+		temp_costs1 += costsf1f2;
+		temp_costs1 -= costsf1f1;
+		temp_costs1 -= costsf2f2;
+		//task->ComputeD2Costs((total_costs + costsf1f2) - costsf1f1 - costsf2f2 , counts.count00, sols.sol00);
+		task->ComputeD2Costs(temp_costs1, counts.count00, sols.sol00);
 		task->ComputeD2Costs(costsf1f2, counts.count11, sols.sol11);
 		if (swap) {
 			task->ComputeD2Costs(costsf2f2 - costsf1f2, counts.count10, sols.sol10);
 			task->ComputeD2Costs(costsf1f1 - costsf1f2, counts.count01, sols.sol01);
 			return;
 		}
 		task->ComputeD2Costs(costsf2f2 - costsf1f2, counts.count01, sols.sol01);
@@ -286,23 +313,35 @@
 		const auto& costsf2f2 = _cost_storage.GetCosts(index.ix_f2f2);
 
 		if (index.equal) {
 			task->ComputeD2Costs(total_costs - costsf1f2, counts.count00, sols.sol00);
 			task->ComputeD2Costs(costsf1f2, counts.count11, sols.sol11);
 			return;
 		}
-		task->ComputeD2Costs((total_costs + costsf1f2) - costsf1f1 - costsf2f2, counts.count00, sols.sol00);
+		// Temp_costs2 = costs for f1, but not f2
+		temp_costs2 = costsf1f1;
+		temp_costs2 -= costsf1f2;
+
+		// Temp costs1 = costs for neither f1 nor f2
+		temp_costs1 = total_costs;
+		temp_costs1 -= temp_costs2;
+		temp_costs1 -= costsf2f2;
+		task->ComputeD2Costs(temp_costs1, counts.count00, sols.sol00);
 		task->ComputeD2Costs(costsf1f2, counts.count11, sols.sol11);
 		if (index.swap) {
 			task->ComputeD2Costs(costsf2f2 - costsf1f2, counts.count10, sols.sol10);
 			task->ComputeD2Costs(costsf1f1 - costsf1f2, counts.count01, sols.sol01);
 			return;
 		}
-		task->ComputeD2Costs(costsf2f2 - costsf1f2, counts.count01, sols.sol01);
-		task->ComputeD2Costs(costsf1f1 - costsf1f2, counts.count10, sols.sol10);
+		// Temp costs1 = costs for f2 but not f1
+		temp_costs1 = costsf2f2;
+		temp_costs1 -= costsf1f2;
+		task->ComputeD2Costs(temp_costs1, counts.count01, sols.sol01);
+		// temp costs2 is still costs for f1 but not f2
+		task->ComputeD2Costs(temp_costs2, counts.count10, sols.sol10);
 	}
 
 	template <class OT>
 	void CostCalculator<OT>::CalcSol00(typename CostCalculator<OT>::SolType& sol, int label, int f1, int f2) const {
 		const auto& _cost_storage = cost_storage[label];
 		const auto& total_costs = _cost_storage.GetTotalCosts();
 		if (f1 == f2) {
@@ -314,32 +353,14 @@
 			const auto& costsf1f1 = _cost_storage.GetCosts(f1, f1);
 			const auto& costsf2f2 = _cost_storage.GetCosts(f2, f2);
 			task->ComputeD2Costs(total_costs + costsf1f2 - costsf1f1 - costsf2f2 , GetCount00(f1, f2), sol);
 		}
 	}
 
 	template <class OT>
-	void CostCalculator<OT>::CalcSol01(typename CostCalculator<OT>::SolType& sol, int label, int f1, int f2) const {
-		if (f1 > f2) return CalcSol10(sol, label, f2, f1);
-		const auto& _cost_storage = cost_storage[label];
-		const auto& costsf2f2 = _cost_storage.GetCosts(f2, f2);
-		const auto& costsf1f2 = _cost_storage.GetCosts(f1, f2);
-		task->ComputeD2Costs(costsf2f2 - costsf1f2, GetCount01(f1, f2), sol);
-	}
-
-	template <class OT>
-	void CostCalculator<OT>::CalcSol10(typename CostCalculator<OT>::SolType& sol, int label, int f1, int f2) const {
-		if (f1 > f2) return CalcSol01(sol, label, f2, f1);
-		const auto& _cost_storage = cost_storage[label];
-		const auto& costsf1f1 = _cost_storage.GetCosts(f1, f1);
-		const auto& costsf1f2 = _cost_storage.GetCosts(f1, f2);
-		task->ComputeD2Costs(costsf1f1 - costsf1f2, GetCount10(f1, f2), sol);
-	}
-
-	template <class OT>
 	void CostCalculator<OT>::CalcSol11(typename CostCalculator<OT>::SolType& sol, int label, int f1, int f2) const {
 		if (f1 > f2) std::swap(f1, f2);
 		task->ComputeD2Costs(cost_storage[label].GetCosts(f1, f2), GetCount11(f1, f2), sol);
 	}
 
 	template <class OT>
 	const typename CostCalculator<OT>::SolD2Type CostCalculator<OT>::GetCosts00(int label, int f1, int f2) const {
@@ -421,24 +442,24 @@
 
 	template <class OT>
 	int CostCalculator<OT>::GetCount11(int f1, int f2) const {
 		if (f1 > f2) { std::swap(f1, f2); }
 		return counter.GetCount(f1, f2);
 	}
 
-	template <class OT>
-	const typename CostCalculator<OT>::SolLabelType CostCalculator<OT>::GetLeafLabel(int label) const {
-		if constexpr (OT::custom_get_label || std::is_same<typename OT::LabelType, double>::value) {
-			auto sum = GetCosts00(label, 0, 0) + GetCosts11(label, 0, 0);
-			int count = GetCount00(0, 0) + GetCount11(0, 0);
-			return task->GetLabel(sum, count);
-		} else {
-			return label;
-		}
-	}
+	//template <class OT>
+	//const typename CostCalculator<OT>::SolLabelType CostCalculator<OT>::GetLeafLabel(int label) const {
+	//	if constexpr (OT::custom_get_label || std::is_same<typename OT::LabelType, double>::value) {
+	//		auto sum = GetCosts00(label, 0, 0) + GetCosts11(label, 0, 0);
+	//		int count = GetCount00(0, 0) + GetCount11(0, 0);
+	//		return task->GetLabel(sum, count);
+	//	} else {
+	//		return label;
+	//	}
+	//}
 
 	template <class OT>
 	const typename CostCalculator<OT>::SolLabelType CostCalculator<OT>::GetLabel00(int label, int f1, int f2) const {
 		if constexpr (OT::custom_get_label || std::is_same<typename OT::LabelType, double>::value) {
 			return task->GetLabel(GetCosts00(label, f1, f2), GetCount00(f1, f2));
 		} else {
 			return label;
@@ -468,17 +489,30 @@
 		if constexpr (OT::custom_get_label || std::is_same<typename OT::LabelType, double>::value) {
 			return task->GetLabel(GetCosts11(label, f1, f2), GetCount11(f1, f2));
 		} else {
 			return label;
 		}
 	}
 
+	template <class OT>
+	const typename CostCalculator<OT>::SolLabelType CostCalculator<OT>::GetLabel(int label, const typename CostCalculator<OT>::SolD2Type& costs, int count) const {
+		if constexpr (OT::custom_get_label || std::is_same<typename OT::LabelType, double>::value) {
+			return task->GetLabel(costs, count);
+		} else {
+			return label;
+		}
+	}
+
 	template class CostCalculator<Accuracy>;
 	template class CostCalculator<CostComplexAccuracy>;
 
+	template class CostCalculator<Regression>;
+	template class CostCalculator<CostComplexRegression>;
+	template class CostCalculator<SimpleLinearRegression>;
+
 	template class CostCalculator<CostSensitive>;
 	template class CostCalculator<InstanceCostSensitive>;
 	template class CostCalculator<F1Score>;
 	template class CostCalculator<GroupFairness>;
 
 	template class CostCalculator<EqOpp>;
 	template class CostCalculator<PrescriptivePolicy>;
```

### Comparing `pystreed-1.2.3/src/solver/cost_storage.cpp` & `pystreed-1.3.0/src/solver/cost_storage.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 		runtime_assert(index_row <= index_column);
 		int index = IndexSymmetricMatrix(index_row, index_column);
 		return data2d[index];
 	}
 
 	template <class OT>
 	void CostStorage<OT>::ResetToZeros() {
-		for (int j = 0; j < NumElements(); j++) {
-			data2d[j] = CostStorage<OT>::SolD2Type(); // Must have a default constructor
-			}
+		std::fill(data2d.begin(), data2d.end(), CostStorage<OT>::SolD2Type());
 		total_costs = CostStorage<OT>::SolD2Type();
 	}
 
 	template <class OT>
 	void CostStorage<OT>::ResetToZerosReconstruct(int feature) {
 		for (int j = 0; j < num_features; j++) {
 			int f1 = feature;
@@ -65,14 +63,18 @@
 	int CostStorage<OT>::IndexSymmetricMatrixOneDim(int index_row) const {
 		return num_features * index_row - index_row * (index_row + 1) / 2;
 	}
 
 	template class CostStorage<Accuracy>;
 	template class CostStorage<CostComplexAccuracy>;
 
+	template class CostStorage<Regression>;
+	template class CostStorage<CostComplexRegression>;
+	template class CostStorage<SimpleLinearRegression>;
+
 	template class CostStorage<CostSensitive>;
 	template class CostStorage<InstanceCostSensitive>;
 	template class CostStorage<F1Score>;
 	template class CostStorage<GroupFairness>;
 	template class CostStorage<EqOpp>;
 	template class CostStorage<PrescriptivePolicy>;
 	template class CostStorage<SurvivalAnalysis>;
```

### Comparing `pystreed-1.2.3/src/solver/counter.cpp` & `pystreed-1.3.0/src/solver/counter.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/solver/data_splitter.cpp` & `pystreed-1.3.0/src/solver/data_splitter.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/solver/dataset_cache.cpp` & `pystreed-1.3.0/src/solver/dataset_cache.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -223,14 +223,19 @@
 		stored_iterators[data.Size()].push_front(hehe);
 		return iter;
 	}
 
 	template class DatasetCache<Accuracy>;
 	template class DatasetCache<CostComplexAccuracy>;
 
+	template class DatasetCache<Regression>;
+	template class DatasetCache<CostComplexRegression>;
+	template class DatasetCache<PieceWiseLinearRegression>;
+	template class DatasetCache<SimpleLinearRegression>;
+
 	template class DatasetCache<CostSensitive>;
 	template class DatasetCache<InstanceCostSensitive>;
 	template class DatasetCache<F1Score>;
 	template class DatasetCache<GroupFairness>;
 	template class DatasetCache<EqOpp>;
 	template class DatasetCache<PrescriptivePolicy>;
 	template class DatasetCache<SurvivalAnalysis>;
```

### Comparing `pystreed-1.2.3/src/solver/define_parameters.cpp` & `pystreed-1.3.0/src/solver/define_parameters.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 
 		parameters.DefineStringParameter
 		(
 			"task",
 			"Task to optimize.",
 			"accuracy",
 			"Main Parameters",
-			{"accuracy", "cost-complex-accuracy", "f1-score", "group-fairness", "survival-analysis",
-			"equality-of-opportunity", "cost-sensitive", "prescriptive-policy", "instance-cost-sensitive"}
+			{ "accuracy", "cost-complex-accuracy", 
+			"f1-score", "group-fairness", "survival-analysis",
+			"regression", "cost-complex-regression", "piecewise-linear-regression",
+			"simple-linear-regression", "equality-of-opportunity", "cost-sensitive",
+			"prescriptive-policy", "instance-cost-sensitive" }
 		);
 
 		parameters.DefineBooleanParameter
 		(
 			"hyper-tune",
 			"Enable/disable hyper-tuning.",
 			false,
@@ -182,14 +185,22 @@
 		(
 			"use-lower-bound",
 			"Use lower bounding. Disabling this option may be better for some benchmarks, specifically when the number of objectives is high.",
 			true,
 			"Algorithmic Parameters"
 		);
 
+		parameters.DefineBooleanParameter
+		(
+			"use-task-lower-bound",
+			"Use task defined lower bounding for tasks that define a custom lower bound. Disabling this option may be better for some benchmarks if the custom bound takes long to compute.",
+			true,
+			"Algorithmic Parameters"
+		);
+
 		parameters.DefineFloatParameter(
 			"upper-bound",
 			"Search for a tree better than the provided upper bound (numeric).",
 			INT32_MAX, // default
 			"Algorithmic Parameters",
 			0.0, // min
 			DBL_MAX // max
@@ -214,14 +225,15 @@
 			INT32_MAX
 		);
 
 		parameters.DefineBooleanParameter
 		(
 			"use-branch-caching",
 			"Use branch caching to store computed subtrees.",
+			//\"Dataset\" is more powerful than \"branch\" but may required more computational time. Need to be determined experimentally. \"Closure\" is experimental and typically slower than other options.",
 			false, //default value
 			"Algorithmic Parameters"
 		);
 
 		parameters.DefineBooleanParameter
 		(
 			"use-dataset-caching",
@@ -277,10 +289,40 @@
 			"The cost for adding an extra node to the tree. 0.01 means one extra node is only jusitified if it results in at least one percent better training accuracy score.",
 			0.01, // default value
 			"Objective Parameters",
 			0.0, //min value
 			1.0 //max value
 		);
 
+		parameters.DefineFloatParameter
+		(
+			"lasso-penalty",
+			"The lasso lambda penalty.",
+			0.00, // default value
+			"Objective Parameters",
+			0.0, //min value
+			1e12 //max value
+		);
+
+		parameters.DefineFloatParameter
+		(
+			"ridge-penalty",
+			"The ridge gamma penalty.",
+			0.00, // default value
+			"Objective Parameters",
+			0.0, //min value
+			1e12 //max value
+		);
+
+		parameters.DefineStringParameter
+		(
+			"regression-bound",
+			"The type of bound to use, only for cost-complex-regression task.",
+			"equivalent", //default value
+			"Task-specific Parameters",
+			{ "equivalent", "kmeans" },
+			true
+		);
+
 		return parameters;
 	}
 }
```

### Comparing `pystreed-1.2.3/src/solver/difference_computer.cpp` & `pystreed-1.3.0/src/solver/difference_computer.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/solver/feature_selector_gini.cpp` & `pystreed-1.3.0/src/solver/feature_selector_gini.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/solver/similarity_lowerbound.cpp` & `pystreed-1.3.0/src/solver/similarity_lowerbound.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,19 @@
 		return *best_entry;
 	}
 
 
 	template class SimilarityLowerBoundComputer<Accuracy>;
 	template class SimilarityLowerBoundComputer<CostComplexAccuracy>;
 
+	template class SimilarityLowerBoundComputer<Regression>;
+	template class SimilarityLowerBoundComputer<CostComplexRegression>;
+	template class SimilarityLowerBoundComputer<SimpleLinearRegression>;
+	template class SimilarityLowerBoundComputer<PieceWiseLinearRegression>;
+
 	template class SimilarityLowerBoundComputer<CostSensitive>;
 	template class SimilarityLowerBoundComputer<InstanceCostSensitive>;
 	template class SimilarityLowerBoundComputer<F1Score>;
 	template class SimilarityLowerBoundComputer<GroupFairness>;
 	template class SimilarityLowerBoundComputer<EqOpp>;
 	template class SimilarityLowerBoundComputer<PrescriptivePolicy>;
 }
```

### Comparing `pystreed-1.2.3/src/solver/solver.cpp` & `pystreed-1.3.0/src/solver/solver.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 	************************/
 
 	SolverParameters::SolverParameters(const ParameterHandler& parameters) :
 		verbose(parameters.GetBooleanParameter("verbose")),
 		use_terminal_solver(parameters.GetBooleanParameter("use-terminal-solver")),
 		use_upper_bounding(parameters.GetBooleanParameter("use-upper-bound")),
 		use_lower_bounding(parameters.GetBooleanParameter("use-lower-bound")),
+		use_task_lower_bounding(parameters.GetBooleanParameter("use-task-lower-bound")),
 		similarity_lb(parameters.GetBooleanParameter("use-similarity-lower-bound")),
 		minimum_leaf_node_size(int(parameters.GetIntegerParameter("min-leaf-node-size"))) { }
 
 	/************************
 	*    AbstractSolver     *
 	************************/
 
@@ -59,15 +60,20 @@
 
 		// if no UB is given yet, compute the leaf solutions in the root node and use these as UB
 		auto result = InitializeSol<OT>();
 		if (CheckEmptySol<OT>(global_UB)) {
 			global_UB = InitializeSol<OT>();
 			// If an upper bound is provided, and the objective is numeric, add it to the UB
 			if constexpr (std::is_same<Solver<OT>::SolType, double>::value || std::is_same<Solver<OT>::SolType, int>::value) {
-				AddSol<OT>(global_UB, Node<OT>(parameters.GetFloatParameter("upper-bound")));
+				double ub = parameters.GetFloatParameter("upper-bound");
+				// if INT32-MAX upper bound (default), but the solution value is a double, change the UB to DBL_MAX
+				if (std::abs(ub - INT32_MAX) < 1 && std::is_same<Solver<OT>::SolType, double>::value) {
+					ub = DBL_MAX;
+				}
+				AddSol<OT>(global_UB, Node<OT>(ub));
 			}
 			result = SolveLeafNode(train_data, root_context, global_UB);
 		}
 
 		// If all number of nodes options should be considered, set min_num_nodes to 1, else to max
 		int min_num_nodes = int(parameters.GetIntegerParameter("max-num-nodes"));
 		if (parameters.GetBooleanParameter("all-trees")) { min_num_nodes = 1; }
@@ -85,24 +91,24 @@
 		solver_result->is_proven_optimal = stopwatch.IsWithinTimeLimit();
 		if constexpr (OT::total_order) {
 			if (result.IsFeasible()) {
 				clock_t clock_start = clock();
 				auto tree = ConstructOptimalTree(result, train_data, root_context, int(parameters.GetIntegerParameter("max-depth")), result.NumNodes());
 				stats.time_reconstructing += double(clock() - clock_start) / CLOCKS_PER_SEC;
 				auto score = InternalTrainScore<OT>::ComputeTrainPerformance(&data_splitter, task, tree.get(), train_data);
-				tree->FlipFlippedFeatures(flipped_features);
+				PostProcessTree(tree);
 				solver_result->AddSolution(tree, score);
 			}
 		} else {
 			for (auto& s : result->GetSolutions()) {
 				clock_t clock_start = clock();
 				auto tree = ConstructOptimalTree(s, train_data, root_context, int(parameters.GetIntegerParameter("max-depth")), int(parameters.GetIntegerParameter("max-num-nodes")));
 				stats.time_reconstructing += double(clock() - clock_start) / CLOCKS_PER_SEC;
 				auto score = InternalTrainScore<OT>::ComputeTrainPerformance(&data_splitter, task, tree.get(), train_data);
-				tree->FlipFlippedFeatures(flipped_features);
+				PostProcessTree(tree);
 				solver_result->AddSolution(tree, score);
 			}
 		}
 
 		stats.total_time += stopwatch.TimeElapsedInSeconds();
 		if (solver_parameters.verbose) {
 			stats.Print();
@@ -208,14 +214,21 @@
 						return results;
 					}
 				}
 			}
 
 			//Check LB > UB and return infeasible if true
 			auto lower_bound = cache->RetrieveLowerBound(data, branch, max_depth, num_nodes);
+
+			if constexpr (OT::custom_lower_bound) {
+				if (solver_parameters.use_task_lower_bounding) {
+					auto lb = task->ComputeLowerBound(data, branch, max_depth, num_nodes);
+					AddSolsInv<OT>(lower_bound, lb);
+				}
+			}
 			
 			if (solver_parameters.use_upper_bounding && LeftStrictDominatesRight<OT>(UB, lower_bound)) {
 				return InitializeSol<OT>();
 			}
 
 			//Check lower-bound vs leaf node solution and return if same
 			auto empty_UB = InitializeSol<OT>();
@@ -245,20 +258,26 @@
 		int current_depth = branch.Depth();
 		const int max_size_subtree = std::min((1 << (max_depth - 1)) - 1, num_nodes - 1); //take the minimum between a full tree of max_depth or the number of nodes - 1
 		const int min_size_subtree = num_nodes - 1 - max_size_subtree;
 		typename Solver<OT>::SolContainer lb, left_lower_bound, right_lower_bound;
 
 		auto solutions = SolveLeafNode(data, context, UB);
 		
-		if (data.Size() < 2 * solver_parameters.minimum_leaf_node_size)
+		if (!SatisfiesMinimumLeafNodeSize(data, 2))
 			return solutions;
 
 		auto branch_lb = solver_parameters.use_lower_bounding
 			? cache->RetrieveLowerBound(data, branch, max_depth, num_nodes)
 			: InitializeSol<OT>(true);
+		if constexpr (OT::custom_lower_bound) {
+			if (solver_parameters.use_task_lower_bounding) {
+				auto lb = task->ComputeLowerBound(data, branch, max_depth, num_nodes);
+				AddSolsInv<OT>(branch_lb, lb);
+			}
+		}
 
 		// Initialize the feature selector
 		std::unique_ptr<FeatureSelectorAbstract> feature_selector;
 		if (parameters.GetStringParameter("feature-ordering") == "in-order") {
 			feature_selector = std::make_unique<FeatureSelectorInOrder>(data.NumFeatures());
 		} else if (parameters.GetStringParameter("feature-ordering") == "gini") {
 			runtime_assert(!(std::is_same<typename OT::LabelType, double>::value)); // Regression does not work with Gini
@@ -283,15 +302,15 @@
 				if (solver_parameters.use_upper_bounding && UB.solution < branching_costs) break;				
 			}
 
 			// Split the data and skip if the split does not meet the minimum leaf node size requirements
 			ADataView left_data;
 			ADataView right_data;
 			data_splitter.Split(data, branch, feature, left_data, right_data);
-			if (left_data.Size() < solver_parameters.minimum_leaf_node_size || right_data.Size() < solver_parameters.minimum_leaf_node_size) continue;
+			if (!SatisfiesMinimumLeafNodeSize(left_data) || !SatisfiesMinimumLeafNodeSize(right_data)) continue;
 
 			// Generate the context descriptors for the left and richt sub-branch
 			Solver<OT>::Context left_context, right_context;
 			task->GetLeftContext(data, context, feature, left_context);
 			task->GetRightContext(data, context, feature, right_context);
 
 			// switch the left and right branch if the left has more data
@@ -460,15 +479,15 @@
 		}
 		if (LeftStrictDominatesRight<OT>(UB, results.three_nodes_solutions)) return InitializeSol<OT>();
 		return CopySol<OT>(results.three_nodes_solutions);
 	}
 
 	template<class OT>
 	typename Solver<OT>::SolContainer Solver<OT>::SolveLeafNode(const ADataView& data, const Solver<OT>::Context& context, typename Solver<OT>::SolContainer& UB) const {
-		if (data.Size() < solver_parameters.minimum_leaf_node_size) return InitializeSol<OT>();
+		if (!SatisfiesMinimumLeafNodeSize(data)) return InitializeSol<OT>();
 		const Branch& branch = context.GetBranch();
 
 		// If the optimization task has a custom leaf node function defined, use it
 		if constexpr (OT::custom_leaf) {
 			// Return the optimal feasible solution, requires custom implementation
 			auto sol = task->SolveLeafNode(data, context);
 			if (solver_parameters.use_upper_bounding && LeftStrictDominatesRightSol<OT>(UB, sol)) return InitializeSol<OT>();
@@ -498,14 +517,23 @@
 		lb = InitializeSol<OT>(true);
 		if (solver_parameters.use_lower_bounding) {
 			right_lower_bound = cache->RetrieveLowerBound(right_data, right_branch, right_depth, right_nodes);
 			//if (right_lower_bound->Size() > 0) stats.num_cache_hit_nonzero_bound++;
 			left_lower_bound = cache->RetrieveLowerBound(left_data, left_branch, left_depth, left_nodes);
 			//if (left_lower_bound->Size() > 0) stats.num_cache_hit_nonzero_bound++;
 
+			if constexpr (OT::custom_lower_bound) {
+				if (solver_parameters.use_task_lower_bounding) {
+					auto right_lb = task->ComputeLowerBound(right_data, right_branch, right_depth, right_nodes);
+					AddSolsInv<OT>(right_lower_bound, lb);
+					auto left_lb = task->ComputeLowerBound(left_data, left_branch, left_depth, left_nodes);
+					AddSolsInv<OT>(left_lower_bound, lb);
+				}
+			}
+
 			if constexpr (OT::total_order) {
 				CombineSols(feature, left_lower_bound, right_lower_bound, branching_costs, lb);
 			} else {
 				LBMerge(feature, context, left_lower_bound, right_lower_bound, branching_costs, lb);
 			}
 		}
 	}
@@ -694,14 +722,15 @@
 		}
 	}
 
 	template <class OT>
 	void Solver<OT>::ReduceNodeBudget(const ADataView& data, const Solver<OT>::Context& context, const typename Solver<OT>::SolContainer& UB, int& max_depth, int& num_nodes) const {
 		if constexpr (OT::total_order && OT::has_branching_costs && OT::constant_branching_costs &&
 			std::is_same<typename OT::SolType, double>::value || std::is_same<typename OT::SolType, int>::value) {
+			if (UB.solution >= 0.9 * DBL_MAX) return;
 			auto branching_costs = GetBranchingCosts(data, context, 0);
 			if (branching_costs <= 0) return;
 			int nodes = std::max(0, int((UB.solution + 1e-6) / branching_costs));
 			if (nodes < num_nodes) {
 				int new_max_depth = std::min(max_depth, nodes);
 				if (new_max_depth < max_depth) {
 					max_depth = new_max_depth;
@@ -805,26 +834,21 @@
 
 		if (max_depth == 0 || num_nodes == 0 || sol.NumNodes() == 0) {
 			return Tree<OT>::CreateLabelNode(sol.label);
 		}
 
 		// Special D1 reconstruct
 		bool d1 = max_depth == 1 || num_nodes == 1 || sol.NumNodes() == 1;
-		bool use_cache = cache->UseCache();
 
 		// Special D2 reconstruct
 		if constexpr (OT::use_terminal) {
 			if (!d1 && IsTerminalNode(max_depth, num_nodes)) {
 				try {
 					return terminal_solver1->ConstructOptimalTree(sol, data, context, max_depth, num_nodes);
-				} catch (std::exception& e) {
-					// Could happen because of numerical instability, but could also refer to an actual error. 
-					// Check if the solution value is the same when the terminal-solver is not used.
-					use_cache = false; 
-				}
+				} catch (...){} // Continue to the default way of reconstructing
 			}
 		}
 
 		// Initialize empty UBs
 		auto UB = InitializeSol<OT>();
 		AddSol<OT>(UB, OT::worst);
 		auto UBleft = InitializeSol<OT>();
@@ -833,28 +857,29 @@
 		AddSol<OT>(UBright, OT::worst);
 
 		auto tree = Tree<OT>::CreateFeatureNodeWithNullChildren(sol.feature);
 
 		const Branch& branch = context.GetBranch();
 		ADataView left_data, right_data;
 		data_splitter.Split(data, branch, sol.feature, left_data, right_data);
-		runtime_assert(left_data.Size() >= solver_parameters.minimum_leaf_node_size && right_data.Size() >= solver_parameters.minimum_leaf_node_size);
+		runtime_assert(SatisfiesMinimumLeafNodeSize(left_data) && SatisfiesMinimumLeafNodeSize(right_data));
 		Solver<OT>::Context left_context, right_context;
 		task->GetLeftContext(data, context, sol.feature, left_context);
 		task->GetRightContext(data, context, sol.feature, right_context);
 
 		const int left_subtree_size = sol.num_nodes_left;
 		const int right_subtree_size = sol.num_nodes_right;
 		int left_depth = std::min(max_depth - 1, left_subtree_size);
 		int right_depth = std::min(max_depth - 1, right_subtree_size);
 
 		int left_size = left_subtree_size;
 		int right_size = right_subtree_size;
 		Solver<OT>::SolContainer left_sols, right_sols;
 		
+		bool use_cache = cache->UseCache();
 		if (use_cache) {
 			const int max_size_subtree = std::min((1 << (max_depth - 1)) - 1, num_nodes - 1); //take the minimum between a full tree of max_depth or the number of nodes - 1
 			const int min_size_subtree = num_nodes - 1 - max_size_subtree;
 			int min_left_subtree_size = std::max(sol.num_nodes_left, min_size_subtree);
 			int min_right_subtree_size = std::max(sol.num_nodes_right, min_size_subtree);
 
 			left_size = min_left_subtree_size;
@@ -880,19 +905,27 @@
 			if constexpr (!OT::total_order) right_sols->FilterOnNumberOfNodes(min_right_subtree_size);
 
 		}
 		
 		if (!use_cache || CheckEmptySol<OT>(left_sols)) {
 			left_depth = std::min(max_depth - 1, left_subtree_size);
 			left_sols = SolveSubTree(left_data, left_context, UBleft, left_depth, left_subtree_size);
+			if (CheckEmptySol<OT>(left_sols)) {
+				left_sols = SolveSubTree(left_data, left_context, UBleft, left_depth, left_subtree_size);
+			}
+			runtime_assert(!CheckEmptySol<OT>(left_sols));
 			if constexpr (!OT::total_order) left_sols->FilterOnNumberOfNodes(left_subtree_size);
 		}
 		if (!use_cache || CheckEmptySol<OT>(right_sols)) {
 			right_depth = std::min(max_depth - 1, right_subtree_size);
 			right_sols = SolveSubTree(right_data, right_context, UBright, right_depth, right_subtree_size);
+			if (CheckEmptySol<OT>(right_sols)) {
+				right_sols = SolveSubTree(right_data, right_context, UBright, right_depth, right_subtree_size);
+			}
+			runtime_assert(!CheckEmptySol<OT>(right_sols));
 			if constexpr (!OT::total_order) right_sols->FilterOnNumberOfNodes(right_subtree_size);
 		}
 
 		// Reconstruct Merge
 		if constexpr (!OT::total_order) {
 			TreeNode<OT> tree_node;
 			tree_node.parent = sol;
@@ -935,14 +968,31 @@
 			return OT::best;
 		} else {
 			return task->GetBranchingCosts(data, context, feature);
 		}
 	}
 
 	template <class OT>
+	bool Solver<OT>::SatisfiesMinimumLeafNodeSize(const ADataView& data, int multiplier) const {
+		int mlsz = solver_parameters.minimum_leaf_node_size * multiplier;
+		if constexpr (OT::use_weights) {
+			int weight = 0;
+			for (int k = 0; k < data.NumLabels(); k++) {
+				for (auto& i : data.GetInstancesForLabel(k)) {
+					weight += int(i->GetWeight());
+					if (weight >= mlsz) return true;
+				}
+			}
+			return false;
+		} else {
+			return data.Size() >= mlsz;
+		}
+	}
+
+	template <class OT>
 	void Solver<OT>::PreprocessData(AData& data, bool train) {
 		if (train) {
 			flipped_features.resize(data.NumFeatures(), 0);
 			for (int f = 0; f < data.NumFeatures(); f++) {
 				int positive_count = 0;
 				for (int i = 0; i < data.Size(); i++) {
 					auto instance = data.GetInstance(i);
@@ -986,14 +1036,22 @@
 		test_data = org_test_data;
 		if constexpr (OT::preprocess_train_test_data) {
 			task->PreprocessTestData(test_data);
 		}
 	}
 
 	template <class OT>
+	void Solver<OT>::PostProcessTree(std::shared_ptr<Tree<OT>> tree) {
+		tree->FlipFlippedFeatures(flipped_features);
+		if constexpr (OT::postprocess_tree) {
+			task->PostProcessTree(tree);
+		}
+	}
+
+	template <class OT>
 	std::shared_ptr<SolverResult> Solver<OT>::TestPerformance(const std::shared_ptr<SolverResult>& _result, const ADataView& _test_data) {
 		InitializeTest(_test_data, false);
 		const SolverTaskResult<OT>* result = static_cast<const SolverTaskResult<OT>*>(_result.get());
 		auto solver_result = std::make_shared<SolverTaskResult<OT>>(*result);
 		for (size_t i = 0; i < result->NumSolutions(); i++) {
 			auto score = InternalTestScore<OT>::ComputeTestPerformance(&data_splitter, task, result->trees[i].get(), flipped_features, test_data);
 			solver_result->SetScore(i, score);
@@ -1009,14 +1067,19 @@
 		tree->Classify(&data_splitter, task, context, flipped_features, test_data, labels);
 		return labels;
 	}
 
 	template class Solver<Accuracy>;
 	template class Solver<CostComplexAccuracy>;
 
+	template class Solver<Regression>;
+	template class Solver<CostComplexRegression>;
+	template class Solver<PieceWiseLinearRegression>;
+	template class Solver<SimpleLinearRegression>;
+
 	template class Solver<CostSensitive>;
 	template class Solver<InstanceCostSensitive>;
 	template class Solver<F1Score>;
 	template class Solver<GroupFairness>;
 	template class Solver<EqOpp>;
 	template class Solver<PrescriptivePolicy>;
 	template class Solver<SurvivalAnalysis>;
```

### Comparing `pystreed-1.2.3/src/solver/terminal_solver.cpp` & `pystreed-1.3.0/src/solver/terminal_solver.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 				label_assignments.push_back({ left_label, right_label });
 			}
 		}
 	}
 
 	template <class OT>
 	TerminalResults<OT>& TerminalSolver<OT>::Solve(const ADataView& data, const typename TerminalSolver<OT>::Context& context, typename TerminalSolver<OT>::SolContainer& UB, int num_nodes) {
-		results.Clear();
 		this->UB = UB;
-
 		bool changes_made = cost_calculator.Initialize(data, context, num_nodes);
 		if (!changes_made) return results;
+		results.Clear();
+		if (cost_calculator.GetTotalCount() < solver_parameters->minimum_leaf_node_size) return results;
 		InitialiseChildrenInfo(context, data);
 		SolveOneNode(data, context, true);
 		if (num_nodes == 1) {
 			return results;
 		}
 
 		typename TerminalSolver<OT>::SolType left_sol;
@@ -57,19 +57,19 @@
 				if ((counts.count00 < solver_parameters->minimum_leaf_node_size || counts.count01 < solver_parameters->minimum_leaf_node_size)
 					&& (counts.count10 < solver_parameters->minimum_leaf_node_size || counts.count11 < solver_parameters->minimum_leaf_node_size)
 					&& (counts.count00 < solver_parameters->minimum_leaf_node_size || counts.count10 < solver_parameters->minimum_leaf_node_size)
 					&& (counts.count01 < solver_parameters->minimum_leaf_node_size || counts.count11 < solver_parameters->minimum_leaf_node_size)) {
 					continue;
 				}
 
-				const auto branch_left_costs = cost_calculator.GetBranchingCosts0(f1, f2);
-				const auto branch_right_costs = cost_calculator.GetBranchingCosts1(f1, f2);
+				const auto branch_left_costs = cost_calculator.GetBranchingCosts0(counts.count00  + counts.count01, f1, f2);
+				const auto branch_right_costs = cost_calculator.GetBranchingCosts1(counts.count10 + counts.count11 , f1, f2);
 
-				const auto branch_left_costs_rev = cost_calculator.GetBranchingCosts0(f2, f1);
-				const auto branch_right_costs_rev = cost_calculator.GetBranchingCosts1(f2, f1);
+				const auto branch_left_costs_rev = cost_calculator.GetBranchingCosts0(counts.count00  + counts.count10 , f2, f1);
+				const auto branch_right_costs_rev = cost_calculator.GetBranchingCosts1(counts.count01 + counts.count11, f2, f1);
 
 
 
 				for (int label = 0; label < num_labels; label++) {
 					cost_calculator.CalcSols(counts, sols[label], label, index);
 				}
 
@@ -124,26 +124,27 @@
 	template <class OT>
 	void TerminalSolver<OT>::SolveOneNode(const ADataView& data, const typename TerminalSolver<OT>::Context& context, bool initialized) {
 		runtime_assert(initialized); // for now
 		auto& result = results.one_node_solutions;
 		SetSolSizeBudget<OT>(result, 1, 1);
 
 		Node<OT> node;
-		// Add leaf nodes
-		if constexpr (OT::custom_leaf) {
-			AddSol<OT>(result, task->SolveLeafNode(data, context));
-		} else {
+		typename TerminalSolver<OT>::SolType merged_sol;
+		{
+			typename OT::SolLabelType out_label;
 			for (int label = 0; label < data.NumLabels(); label++) {
-				node = Node<OT>(label, task->GetLeafCosts(data, context, label));
+				cost_calculator.CalcLeafSol(merged_sol, label, out_label);
+				node.Set(INT32_MAX, out_label, merged_sol, 0, 0);
+
 				if (OT::has_constraint && !SatisfiesConstraint(node, context)) continue;
 				if (OT::terminal_filter && LeftStrictDominatesRightSol<OT>(UB, node)) continue;
 				AddSol<OT>(result, node);
 			}
 		}
-		typename TerminalSolver<OT>::SolType merged_sol;
+		
 		bool computed_leaves = false;
 
 		if (initialized) {
 			Counts counts;
 			IndexInfo index;
 			for (int feature = 0; feature < num_features; feature++) {
 				if (!task->MayBranchOnFeature(feature)) continue;
@@ -205,41 +206,52 @@
 	}
 
 	template <class OT>
 	void TerminalSolver<OT>::UpdateBestTwoNodeAssignment(const typename TerminalSolver<OT>::Context& context, int root_feature) {
 		auto& child_info = children_info[root_feature];
 		const auto& left_context = child_info.left_context;
 		const auto& right_context = child_info.right_context;
+		Counts counts;
+		IndexInfo index;
+		
 		auto left_leaves = InitializeSol<OT>();
+		auto right_leaves = InitializeSol<OT>();
+
+		cost_calculator.GetIndexInfo(root_feature, root_feature, index);
+		cost_calculator.GetCounts(counts, index);
+		int left_size = counts.count00;
+		int right_size = counts.count11;
+
+		typename OT::SolD2Type costs;
+		typename TerminalSolver<OT>::SolType leaf_sol;
+		typename OT::SolLabelType assign_label;
 
-		int left_size = cost_calculator.GetCount00(root_feature, root_feature);
+		Node<OT> node;
 		if (left_size >= solver_parameters->minimum_leaf_node_size) {
 			for (int label = 0; label < num_labels; label++) {
-				//PartialSolution left_leaf(cost_calculator.GetCosts00(label, root_feature, root_feature));
-				typename TerminalSolver<OT>::SolType left_leaf;
-				cost_calculator.CalcSol00(left_leaf, label, root_feature, root_feature);
-				auto assign_label = cost_calculator.GetLabel00(label, root_feature, root_feature);
-				Node<OT> left_leaf_sol(assign_label, left_leaf);
-				if (OT::has_constraint && !SatisfiesConstraint(left_leaf_sol, left_context)) continue;
-				if (OT::terminal_filter && LeftStrictDominatesRightSol<OT>(UB, left_leaf_sol)) continue;
-				AddSol<OT>(left_leaves, left_leaf_sol);
+				costs = cost_calculator.GetCosts00(label, root_feature, root_feature);
+				task->ComputeD2Costs(costs, left_size, leaf_sol);
+				assign_label = cost_calculator.GetLabel(label, costs, left_size);
+				node.Set(INT32_MAX, assign_label, leaf_sol, 0, 0);
+				//node.Set(INT32_MAX, OT::worst_label, sols[label].sol00, 0, 0);
+				if (OT::has_constraint && !SatisfiesConstraint(node, left_context)) continue;
+				if (OT::terminal_filter && LeftStrictDominatesRightSol<OT>(UB, node)) continue;
+				AddSol<OT>(left_leaves, node);
 			}
 		}
-
-		auto right_leaves = InitializeSol<OT>();
-		int right_size = cost_calculator.GetCount11(root_feature, root_feature);
 		if (right_size >= solver_parameters->minimum_leaf_node_size) {
 			for (int label = 0; label < num_labels; label++) {
-				typename TerminalSolver<OT>::SolType right_leaf;
-				cost_calculator.CalcSol11(right_leaf, label, root_feature, root_feature);
-				auto assign_label = cost_calculator.GetLabel11(label, root_feature, root_feature);
-				Node<OT> right_leaf_sol(assign_label, right_leaf);
-				if (OT::has_constraint && !SatisfiesConstraint(right_leaf_sol, right_context)) continue;
-				if (OT::terminal_filter && LeftStrictDominatesRightSol<OT>(UB, right_leaf_sol)) continue;
-				AddSol<OT>(right_leaves, right_leaf_sol);
+				costs = cost_calculator.GetCosts11(label, root_feature, root_feature);
+				task->ComputeD2Costs(costs, right_size, leaf_sol);
+				assign_label = cost_calculator.GetLabel(label, costs, right_size);
+				node.Set(INT32_MAX, assign_label, leaf_sol, 0, 0);
+				//node.Set(INT32_MAX, OT::worst_label, sols[label].sol11, 0, 0);
+				if (OT::has_constraint && !SatisfiesConstraint(node, right_context)) continue;
+				if (OT::terminal_filter && LeftStrictDominatesRightSol<OT>(UB, node)) continue;
+				AddSol<OT>(right_leaves, node);
 			}
 		}
 
 		auto left_children = children_info[root_feature].left_child_assignments;
 		auto right_children = children_info[root_feature].right_child_assignments;
 
 		if constexpr (!OT::total_order) {
@@ -377,15 +389,15 @@
 
 				cost_calculator.GetCounts(counts, node.feature, f2);
 				
 				for (int label = 0; label < num_labels; label++) {
 					cost_calculator.CalcSols(counts, sols[label], label, node.feature, f2);
 				}
 				if (node.num_nodes_left > 0 && counts.count00 >= solver_parameters->minimum_leaf_node_size && counts.count01 >= solver_parameters->minimum_leaf_node_size) {
-					auto branching_costs = cost_calculator.GetBranchingCosts0(node.feature, f2);
+					auto branching_costs = cost_calculator.GetBranchingCosts0(counts.count00 + counts.count01, node.feature, f2);
 					for (int left_label = 0; left_label < num_labels; left_label++) {
 						for (int right_label = 0; right_label < num_labels; right_label++) {
 							//if (num_labels > 1 && left_label == right_label) continue;
 							auto left_assigned_label = cost_calculator.GetLabel00(left_label, node.feature, f2);
 							auto right_assigned_label = cost_calculator.GetLabel01(right_label, node.feature, f2);
 							left_node.Set(INT32_MAX, left_assigned_label, sols[left_label].sol00, 0, 0);
 							right_node.Set(INT32_MAX, right_assigned_label, sols[right_label].sol01, 0, 0);
@@ -400,15 +412,15 @@
 								left_solutions.push_back(left_solution);
 							}
 						}
 					}
 				}
 				
 				if (node.num_nodes_right > 0 && counts.count10 >= solver_parameters->minimum_leaf_node_size && counts.count11 >= solver_parameters->minimum_leaf_node_size) {
-					auto branching_costs = cost_calculator.GetBranchingCosts1(node.feature, f2);
+					auto branching_costs = cost_calculator.GetBranchingCosts1(counts.count10 + counts.count11, node.feature, f2);
 					for (int left_label = 0; left_label < num_labels; left_label++) {
 						for (int right_label = 0; right_label < num_labels; right_label++) {
 							//if (num_labels > 1 && left_label == right_label) continue;
 							auto left_assigned_label = cost_calculator.GetLabel10(left_label, node.feature, f2);
 							auto right_assigned_label = cost_calculator.GetLabel11(right_label, node.feature, f2);
 							left_node.Set(INT32_MAX, left_assigned_label, sols[left_label].sol10, 0, 0);
 							right_node.Set(INT32_MAX, right_assigned_label, sols[right_label].sol11, 0, 0);
@@ -424,38 +436,43 @@
 							}
 						}
 					}
 				}
 			}
 		}
 		if constexpr (OT::total_order) {
-			//runtime_assert(left_solution.parent.IsFeasible());
-			//runtime_assert(right_solution.parent.IsFeasible
+			runtime_assert(left_solution.parent.IsFeasible());
+			runtime_assert(right_solution.parent.IsFeasible());
 			if (!left_solution.parent.IsFeasible() || !right_solution.parent.IsFeasible()) {
-				throw std::runtime_error("Could not reconstruct the tree in the terminal solver.");
+				throw std::runtime_error("Could not find a feasible tree for the given solution.");
 			}
 			tree_node.Set(node, left_solution.parent, right_solution.parent);
 			return Tree<OT>::CreateD2TreeFromTreeNodes(tree_node, left_solution, right_solution);
 		} else {
 			auto branching_costs = cost_calculator.GetBranchingCosts(node.feature);
 			tree_node.parent = node;
 			for (const auto& left_sol : left_solutions) {
 				for (const auto& right_sol : right_solutions) {
 					if (CheckReconstructSolution<OT>(left_sol.parent, right_sol.parent, branching_costs, &tree_node)) {
 						return Tree<OT>::CreateD2TreeFromTreeNodes(tree_node, left_sol, right_sol);
 					}
 				}
 			}
 			runtime_assert(1 == 0);
+			throw std::runtime_error("Could not find a feasible tree for the given solution.");
 		}
 	}
 
 	template class TerminalSolver<Accuracy>;
 	template class TerminalSolver<CostComplexAccuracy>;
 
+	template class TerminalSolver<Regression>;
+	template class TerminalSolver<CostComplexRegression>;
+	template class TerminalSolver<SimpleLinearRegression>;
+
 	template class TerminalSolver<CostSensitive>;
 	template class TerminalSolver<InstanceCostSensitive>;
 	template class TerminalSolver<F1Score>;
 	template class TerminalSolver<GroupFairness>;
 	template class TerminalSolver<EqOpp>;
 	template class TerminalSolver<PrescriptivePolicy>;
 	template class TerminalSolver<SurvivalAnalysis>;
```

### Comparing `pystreed-1.2.3/src/tasks/accuracy/cost_complex_accuracy.cpp` & `pystreed-1.3.0/src/tasks/accuracy/cost_complex_accuracy.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/cost_sensitive.cpp` & `pystreed-1.3.0/src/tasks/cost_sensitive.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/eq_opp.cpp` & `pystreed-1.3.0/src/tasks/eq_opp.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/f1score.cpp` & `pystreed-1.3.0/src/tasks/f1score.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/group_fairness.cpp` & `pystreed-1.3.0/src/tasks/group_fairness.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/instance_cost_sensitive.cpp` & `pystreed-1.3.0/src/tasks/instance_cost_sensitive.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/optimization_task.cpp` & `pystreed-1.3.0/src/tasks/optimization_task.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/prescriptive_policy.cpp` & `pystreed-1.3.0/src/tasks/prescriptive_policy.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/tasks/survival_analysis.cpp` & `pystreed-1.3.0/src/tasks/survival_analysis.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/utils/file_reader.cpp` & `pystreed-1.3.0/src/utils/file_reader.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -155,14 +155,19 @@
 		if (data.NumFeatures() > num_features) data.SetNumFeatures(num_features);
 	}
 
 
 	template void FileReader::ReadData<Accuracy>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<CostComplexAccuracy>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 
+	template void FileReader::ReadData<Regression>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
+	template void FileReader::ReadData<CostComplexRegression>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
+	template void FileReader::ReadData<PieceWiseLinearRegression>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
+	template void FileReader::ReadData<SimpleLinearRegression>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
+
 	template void FileReader::ReadData<CostSensitive>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<InstanceCostSensitive>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<F1Score>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<GroupFairness>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<EqOpp>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<PrescriptivePolicy>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
 	template void FileReader::ReadData<SurvivalAnalysis>(ParameterHandler&, AData&, ADataView&, ADataView&, std::default_random_engine*);
```

### Comparing `pystreed-1.2.3/src/utils/key_value_heap.cpp` & `pystreed-1.3.0/src/utils/key_value_heap.cpp`

 * *Files identical despite different names*

### Comparing `pystreed-1.2.3/src/utils/parameter_handler.cpp` & `pystreed-1.3.0/src/utils/parameter_handler.cpp`

 * *Files identical despite different names*

