# Comparing `tmp/flamapy-fw-2.0.0.dev0.tar.gz` & `tmp/flamapy-fw-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-fw-2.0.0.dev0.tar", last modified: Mon May 27 15:16:13 2024, max compression
+gzip compressed data, was "flamapy-fw-2.0.0.dev1.tar", last modified: Mon May 27 21:04:53 2024, max compression
```

## Comparing `flamapy-fw-2.0.0.dev0.tar` & `flamapy-fw-2.0.0.dev1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.196741 flamapy-fw-2.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 15:16:13.196741 flamapy-fw-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.188741 flamapy-fw-2.0.0.dev0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.188741 flamapy-fw-2.0.0.dev0/flamapy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.188741 flamapy-fw-2.0.0.dev0/flamapy/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.188741 flamapy-fw-2.0.0.dev0/flamapy/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/models/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/models/variability_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.192741 flamapy-fw-2.0.0.dev0/flamapy/core/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/abstract_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/atomic_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/average_branching_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/commonality.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/configurations_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/core_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/count_leafs.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/dead_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/error_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/error_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/estimated_configurations_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/metrics_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/satisfiable.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/satisfiable_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/operations/variability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.192741 flamapy-fw-2.0.0.dev0/flamapy/core/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/transformations/abstract_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/transformations/model_to_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/transformations/model_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/transformations/text_to_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.192741 flamapy-fw-2.0.0.dev0/flamapy/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/endpoint/diverso_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.188741 flamapy-fw-2.0.0.dev0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.192741 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.192741 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/models/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.192741 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:16:13.192741 flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 15:16:13.000000 flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-27 15:16:13.000000 flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:16:13.000000 flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 15:16:13.000000 flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 15:16:13.000000 flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 15:16:13.000000 flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:16:13.196741 flamapy-fw-2.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-27 15:15:59.000000 flamapy-fw-2.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.839704 flamapy-fw-2.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 21:04:53.839704 flamapy-fw-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.827704 flamapy-fw-2.0.0.dev1/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.831704 flamapy-fw-2.0.0.dev1/flamapy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.831704 flamapy-fw-2.0.0.dev1/flamapy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.831704 flamapy-fw-2.0.0.dev1/flamapy/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/models/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/models/variability_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.835704 flamapy-fw-2.0.0.dev1/flamapy/core/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/abstract_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/atomic_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/average_branching_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/commonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/configurations_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/core_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/count_leafs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/error_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/error_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/estimated_configurations_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/false_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/metrics_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/satisfiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/satisfiable_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/operations/variability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.835704 flamapy-fw-2.0.0.dev1/flamapy/core/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/transformations/abstract_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/transformations/model_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/transformations/model_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/transformations/text_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.835704 flamapy-fw-2.0.0.dev1/flamapy/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/endpoint/diverso_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.831704 flamapy-fw-2.0.0.dev1/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.835704 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.835704 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/models/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.835704 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:04:53.839704 flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-27 21:04:53.000000 flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-27 21:04:53.000000 flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:04:53.000000 flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 21:04:53.000000 flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 21:04:53.000000 flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 21:04:53.000000 flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:04:53.839704 flamapy-fw-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-27 21:04:44.000000 flamapy-fw-2.0.0.dev1/setup.py
```

### Comparing `flamapy-fw-2.0.0.dev0/PKG-INFO` & `flamapy-fw-2.0.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fw
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.
 Home-page: https://github.com/flamapy/core
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-fw-2.0.0.dev0/README.md` & `flamapy-fw-2.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/commands/__init__.py` & `flamapy-fw-2.0.0.dev1/flamapy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/discover.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/discover.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/models/ast.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/models/ast.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/operations/__init__.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/operations/atomic_sets.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/operations/atomic_sets.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/operations/false_optional_features.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/operations/false_optional_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/operations/metrics_operation.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/operations/metrics_operation.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/operations/sampling.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/operations/sampling.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/core/plugins.py` & `flamapy-fw-2.0.0.dev1/flamapy/core/plugins.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/endpoint/diverso_lab.py` & `flamapy-fw-2.0.0.dev1/flamapy/endpoint/diverso_lab.py`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py` & `flamapy-fw-2.0.0.dev1/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(self, path: str) -> None:
         self._path = path
 
     def transform(self) -> Configuration:
         csv_reader = self.get_configuration_from_csv(self._path)
         elements = {}
         for row in csv_reader:
-            elements[VariabilityElement(row[0])] = True
+            elements[row[0]] = True
         return Configuration(elements)
 
     def get_configuration_from_csv(self, path: str) -> list[list[str]]:
         # Returns a list of list
         if not file_exists(path):
             raise ConfigurationNotFound
```

### Comparing `flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/PKG-INFO` & `flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fw
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.
 Home-page: https://github.com/flamapy/core
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-fw-2.0.0.dev0/flamapy_fw.egg-info/SOURCES.txt` & `flamapy-fw-2.0.0.dev1/flamapy_fw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamapy-fw-2.0.0.dev0/setup.py` & `flamapy-fw-2.0.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-fw",
-    version="2.0.0.dev0",
+    version="2.0.0.dev1",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/core",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
```

