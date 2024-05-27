# Comparing `tmp/flamapy-sat-1.6.0.dev0.tar.gz` & `tmp/flamapy-sat-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-sat-1.6.0.dev0.tar", last modified: Mon Jan  8 10:35:11 2024, max compression
+gzip compressed data, was "flamapy-sat-2.0.0.dev0.tar", last modified: Mon May 27 15:17:56 2024, max compression
```

## Comparing `flamapy-sat-1.6.0.dev0.tar` & `flamapy-sat-2.0.0.dev0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.061812 flamapy-sat-1.6.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-08 10:35:11.061812 flamapy-sat-1.6.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.053812 flamapy-sat-1.6.0.dev0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.053812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/pysat_diagnosis_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/fastdiag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/hsdag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/fastdiag_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/quickxplain_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/quickxplain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_abstract_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_diagnosis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/fm_to_diag_pysat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.057812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.061812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_commonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_core_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_dead_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_products.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_products_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_valid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_valid_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_valid_product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.061812 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:11.061812 flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-08 10:35:11.000000 flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-01-08 10:35:11.000000 flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-08 10:35:11.000000 flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-08 10:35:11.000000 flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-08 10:35:11.000000 flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 10:35:11.061812 flamapy-sat-1.6.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-08 10:34:58.000000 flamapy-sat-1.6.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.095998 flamapy-sat-2.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 15:17:56.095998 flamapy-sat-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.083998 flamapy-sat-2.0.0.dev0/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.087998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.087998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.087998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/pysat_diagnosis_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.087998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.087998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/fastdiag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.087998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/hsdag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.091998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/fastdiag_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/quickxplain_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/quickxplain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_abstract_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_diagnosis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.091998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/fm_to_diag_pysat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.091998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.091998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/models/pysat_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.091998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_commonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_configurations_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_core_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_false_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_satisfiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_satisfiable_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.091998 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:56.095998 flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 15:17:56.000000 flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-27 15:17:56.000000 flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 15:17:56.000000 flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 15:17:56.000000 flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 15:17:56.000000 flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:17:56.095998 flamapy-sat-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-27 15:17:46.000000 flamapy-sat-2.0.0.dev0/setup.py
```

### Comparing `flamapy-sat-1.6.0.dev0/PKG-INFO` & `flamapy-sat-2.0.0.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.6.0.dev0
+Version: 2.0.0.dev0
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/pysat_diagnosis_model.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/models/pysat_diagnosis_model.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/checker.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/checker.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/fastdiag.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/fastdiag.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/hsdag.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/hsdag.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/fastdiag_labeler.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/fastdiag_labeler.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/labeler.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/labeler.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/quickxplain_labeler.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/labeler/quickxplain_labeler.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/node.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/hsdag/node.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/quickxplain.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/quickxplain.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/utils.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/diagnosis/utils.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_abstract_identifier.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_abstract_identifier.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_conflict.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_conflict.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_diagnosis.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/operations/pysat_diagnosis.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/fm_to_diag_pysat.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_diagnosis_metamodel/transformations/fm_to_diag_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/models/pysat_model.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/models/pysat_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         return 'pysat'
 
     def __init__(self) -> None:
         self._cnf = CNF()
         self.variables: dict[str, int] = {}  # feature's name -> id
         self.features: dict[int, str] = {}  # id -> feature's name
         self.original_model: VariabilityModel
-        
+
     def add_clause(self, clause: list[int]) -> None:
         self._cnf.append(clause)
 
     def get_variable(self, key: str) -> int:
         if key not in self.variables:
             raise FlamaException(f'Feature {key} not found')
         return self.variables[key]
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 from enum import Enum, auto
+
 from flamapy.core.exceptions import FlamaException
 
 
 class CNFLogicConnective(Enum):
     """The propositional logic connectives a formula in CNF can contain."""
     NOT = auto()
     AND = auto()
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/__init__.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from .pysat_valid import PySATValid
-from .pysat_valid_configuration import PySATValidConfiguration
-from .pysat_valid_product import PySATValidProduct
-from .pysat_products import PySATProducts
-from .pysat_products_number import PySATProductsNumber
+from .pysat_satisfiable import PySATSatisfiable
+from .pysat_satisfiable_configuration import PySATSatisfiableConfiguration
+from .pysat_configurations import PySATConfigurations
+from .pysat_configurations_number import PySATConfigurationsNumber
 from .pysat_commonality import PySATCommonality
 from .pysat_filter import PySATFilter
 from .pysat_core_features import PySATCoreFeatures
 from .pysat_dead_features import PySATDeadFeatures
 from .pysat_false_optional_features import PySATFalseOptionalFeatures
 from .pysat_metrics import PySATMetrics
 
+
 __all__ = [
-    'PySATValid',
-    'PySATValidConfiguration',
-    'PySATValidProduct',
-    'PySATProducts',
-    'PySATProductsNumber',
+    'PySATSatisfiable',
+    'PySATSatisfiableConfiguration',
+    'PySATConfigurations',
+    'PySATConfigurationsNumber',
     'PySATCommonality',
     'PySATFilter',
     'PySATCoreFeatures',
     'PySATDeadFeatures',
     'PySATFalseOptionalFeatures',
+    'PySATMetrics',
 ]
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_core_features.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_core_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.core.models import VariabilityModel
 
 
 class PySATCoreFeatures(CoreFeatures):
 
     def __init__(self) -> None:
-        self.core_features: list[list[Any]] = []
+        self.core_features: list[Any] = []
         self.solver = Solver(name='glucose3')
 
-    def get_core_features(self) -> list[list[Any]]:
+    def get_core_features(self) -> list[Any]:
         return self.core_features
 
-    def get_result(self) -> list[list[Any]]:
+    def get_result(self) -> list[Any]:
         return self.get_core_features()
 
     def execute(self, model: VariabilityModel) -> 'PySATCoreFeatures':
         model = cast(PySATModel, model)
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
             self.solver.add_clause(clause)  # añadimos la constraint
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_dead_features.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_dead_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.core.models import VariabilityModel
 
 
 class PySATDeadFeatures(DeadFeatures):
 
     def __init__(self) -> None:
-        self.dead_features: list[list[Any]] = []
+        self.dead_features: list[Any] = []
         self.solver = Solver(name='glucose3')
 
-    def get_dead_features(self) -> list[list[Any]]:
+    def get_dead_features(self) -> list[Any]:
         return self.dead_features
 
-    def get_result(self) -> list[list[Any]]:
+    def get_result(self) -> list[Any]:
         return self.get_dead_features()
 
     def execute(self, model: VariabilityModel) -> 'PySATDeadFeatures':
         model = cast(PySATModel, model)
 
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
             self.solver.add_clause(clause)  # añadimos la constraint
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_false_optional_features.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_false_optional_features.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,53 +2,56 @@
 from typing import Any, cast
 
 from pysat.solvers import Solver
 
 from flamapy.core.operations import FalseOptionalFeatures
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.metamodels.fm_metamodel.models.feature_model import FeatureModel
-from flamapy.core.models import VariabilityModel
+from flamapy.core.models import VariabilityModel, VariabilityElement
 from flamapy.core.exceptions import FlamaException
 
+
 LOGGER = logging.getLogger('PySATFalseOptionalFeatures')
 
 
 class PySATFalseOptionalFeatures(FalseOptionalFeatures):
 
     def __init__(self) -> None:
         self.result: list[Any] = []
         self.solver = Solver(name='glucose3')
 
     def execute(self, model: VariabilityModel) -> 'PySATFalseOptionalFeatures':
-        model = cast(PySATModel, model)
-
-        self.result = self._get_false_optional_features(model)
+        sat_model = cast(PySATModel, model)
+        self.result = self._get_false_optional_features(sat_model)
         return self
 
-    def get_false_optional_features(self) -> list[list[Any]]:
+    def get_false_optional_features(self) -> list[VariabilityElement]:
         return self.get_result()
 
     def get_result(self) -> list[Any]:
         return self.result
 
     def _get_false_optional_features(self, sat_model: PySATModel) -> list[Any]:
         try:
-            feature_model=cast(FeatureModel,sat_model.original_model)
+            feature_model = cast(FeatureModel, sat_model.original_model)
         except FlamaException:
-            LOGGER.exception("The transformation didn't attach the source model, which is required for this operation." )
-        
+            LOGGER.exception("The transformation didn't attach the source model, " 
+                             "which is required for this operation.")
+
         real_optional_features = [f for f in feature_model.get_features()
                                   if not f.is_root() and not f.is_mandatory()]
 
         result = []
         for clause in sat_model.get_all_clauses():
             self.solver.add_clause(clause)
 
         for feature in real_optional_features:
             variable = sat_model.variables.get(feature.name)
-            parent_variable = sat_model.variables.get(feature.get_parent().name)
-            assert variable is not None
-            satisfiable = self.solver.solve(assumptions=[parent_variable, -variable])
-            if not satisfiable:
-                result.append(feature.name)
+            parent_feature = feature.get_parent()
+            if parent_feature is not None:
+                parent_variable = sat_model.variables.get(parent_feature.name)
+                assert variable is not None
+                satisfiable = self.solver.solve(assumptions=[parent_variable, -variable])
+                if not satisfiable:
+                    result.append(feature)
         self.solver.delete()
         return result
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_filter.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,21 +26,24 @@
 
     def execute(self, model: VariabilityModel) -> 'PySATFilter':
         model = cast(PySATModel, model)
 
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
             self.solver.add_clause(clause)  # añadimos la constraint
 
-        assumptions = [
-            model.variables.get(feat[0].name) if feat[1]
-            else -model.variables.get(feat[0].name)
-            for feat in self.configuration.elements.items()
-        ]
+        assumptions = []
+        for feat in self.configuration.elements.items():
+            variable = model.variables.get(feat[0])
+            if variable is not None:
+                if feat[1]:
+                    assumptions.append(variable)
+                else:
+                    assumptions.append(-variable)
 
         for solution in self.solver.enum_models(assumptions=assumptions):
             product = []
             for variable in solution:
-                if variable > 0:
+                if variable is not None and variable > 0:
                     product.append(model.features.get(variable))
             self.filter_products.append(product)
         self.solver.delete()
         return self
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_metrics.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,146 +1,162 @@
-from typing import List, Tuple, Union, cast, Callable, Dict, Any
+from typing import Any, cast, Callable, Optional
 
+from flamapy.core.models import VariabilityModel
+from flamapy.core.exceptions import FlamaException
 from flamapy.core.operations.metrics_operation import Metrics
-from flamapy.core.models.variability_model import VariabilityModel
-
 from flamapy.metamodels.pysat_metamodel.models import PySATModel
 from flamapy.metamodels.pysat_metamodel import operations as sat_operations
 
 
-
 def metric_method(func: Callable) -> Callable:
-        """Decorator to mark a method as a metric method.
-        It has the value of the measure, it can also have a size and a ratio.
-        Example:
-            property name: Abstract Features.
-            description: The description of the property
-            value (optional): the list of abstract features.
-            size (optional): the length of the list.
-            ratio (optional): the percentage of abstract features with regards the total number of features.
-        """
-        if not hasattr(func, '_is_metric_method'):
-            setattr(func, '_is_metric_method', True)
-        return func
+    """Decorator to mark a method as a metric method.
+    It has the value of the measure, it can also have a size and a ratio.
+    Example:
+        property name: Abstract Features.
+        description: The description of the property.
+        value (optional): the list of abstract features.
+        size (optional): the length of the list.
+        ratio (optional): the percentage of abstract features with regards the total number
+                            of features.
+    """
+    if not hasattr(func, '_is_metric_method'):
+        setattr(func, '_is_metric_method', True)
+    return func
+
 
 class PySATMetrics(Metrics):
 
     def __init__(self) -> None:
-        self.model = None
-        self.result: List[Dict[str, Any]] = []
-        self.model_type_extension="pysat"
+        super().__init__()
+        self.model: Optional[VariabilityModel] = None
+        self.result: list[dict[str, Any]] = []
+        self.model_type_extension = "pysat"
+        self._features: dict[int, str] = {}
+        self._common_features: list[Any] = []
+        self._dead_features: list[Any] = []
 
-    def get_result(self) -> Dict[str, Any]:
+    def get_result(self) -> list[dict[str, Any]]:
         return self.result
 
-    def calculate_metamodel_metrics(self,model) -> Dict[str, Any]:
+    def calculate_metamodel_metrics(self, model: VariabilityModel) -> list[dict[str, Any]]:
         self.model = cast(PySATModel, model)
 
         #Do some basic calculations to speedup the rest
         self._features = self.model.features
         self._common_features = sat_operations.PySATCoreFeatures().execute(self.model).get_result()
         self._dead_features = sat_operations.PySATDeadFeatures().execute(self.model).get_result()
         # Get all methods that are marked with the metric_method decorator
-        metric_methods = [getattr(self, method_name) for method_name in dir(self) 
-                          if callable(getattr(self, method_name)) and hasattr(getattr(self, method_name), '_is_metric_method')]
+        metric_methods = [getattr(self, method_name) for method_name in dir(self)
+                          if callable(getattr(self, method_name)) and 
+                          hasattr(getattr(self, method_name), '_is_metric_method')]
         if self.filter is not None:
-            metric_methods = [method for method in metric_methods if method.__name__ in self.filter]
-          
+            metric_methods = [method for method in metric_methods 
+                              if method.__name__ in self.filter]
+
         return [method() for method in metric_methods]
-    
+
     @metric_method
-    def valid(self) -> Dict[str, Any]:
+    def valid(self) -> dict[str, Any]:
         """A feature model is valid if it represents at least one configuration."""
+        if self.model is None:
+            raise FlamaException('Model not initialized.')
         name = "Valid (not void)"
         _valid = sat_operations.PySATValid().execute(self.model).get_result()
-        result = self.construct_result( name=name,
-                        doc=self.valid.__doc__,
-                        result=_valid)
+        result = self.construct_result(name=name, doc=self.valid.__doc__, result=_valid)
         return result
-    
+
     @metric_method
-    def core_features(self) -> Dict[str, Any]:
+    def core_features(self) -> dict[str, Any]:
         """Features that are part of all the configurations (aka 'common features')."""
         name = "Core features"
         _core = self._common_features
-        result = self.construct_result( name=name,
-                        doc=self.core_features.__doc__,
-                        result=_core,
-                        size=len(_core),
-                        ratio=self.get_ratio(_core, self._features, 2))
+        result = self.construct_result(name=name,
+                                       doc=self.core_features.__doc__,
+                                       result=_core,
+                                       size=len(_core),
+                                       ratio=self.get_ratio(_core, self._features, 2))
         return result
 
     @metric_method
-    def variant_features(self) -> Dict[str, Any]:
+    def variant_features(self) -> dict[str, Any]:
         """Features that do not appear in all the configurations."""
         name = "Variant features"
         _variant_features = [f for f in self._features.values() 
-                                        if f not in self._common_features and 
-                                           f not in self._dead_features]
-        result = self.construct_result( name=name,
-                        doc=self.variant_features.__doc__,
-                        result=_variant_features,
-                        size=len(_variant_features),
-                        ratio=self.get_ratio(_variant_features, self._features, 2))
+                             if f not in self._common_features and 
+                             f not in self._dead_features]
+        result = self.construct_result(name=name,
+                                       doc=self.variant_features.__doc__,
+                                       result=_variant_features,
+                                       size=len(_variant_features),
+                                       ratio=self.get_ratio(_variant_features, self._features, 2))
         return result
 
     @metric_method
-    def dead_features(self) -> Dict[str, Any]:
+    def dead_features(self) -> dict[str, Any]:
         """Features that cannot appear in any configuration."""
+        if self.model is None:
+            raise FlamaException('Model not initialized.')
         name = "Dead features"
         _dead_features = sat_operations.PySATDeadFeatures().execute(self.model).get_result()
-        result = self.construct_result( name=name,
-                        doc=self.dead_features.__doc__,
-                        result=_dead_features,
-                        size=len(_dead_features),
-                        ratio=self.get_ratio(_dead_features, self._features, 2))
+        result = self.construct_result(name=name,
+                                       doc=self.dead_features.__doc__,
+                                       result=_dead_features,
+                                       size=len(_dead_features),
+                                       ratio=self.get_ratio(_dead_features, self._features, 2))
         return result
 
     @metric_method
-    def unique_features(self) -> Dict[str, Any]:
+    def unique_features(self) -> dict[str, Any]:
         """Features that appear in exactly one configuration."""
         name = "Unique features"
-        
+
         seen_once = set()
         seen_multiple = set()
 
         # Step 2: Iterate through each configuration
         for config in self.configurations()["result"]:
             for feature in config:
                 if feature in seen_once:
                     seen_multiple.add(feature)
                 else:
                     seen_once.add(feature)
 
         # Step 3: Find features that are in seen_once but not in seen_multiple
         _unique_features = seen_once - seen_multiple
 
-        result = self.construct_result( name=name,
-                        doc=self.unique_features.__doc__,
-                        result=_unique_features,
-                        size=len(_unique_features),
-                        ratio=self.get_ratio(_unique_features, self._features, 2))
+        result = self.construct_result(name=name,
+                                       doc=self.unique_features.__doc__,
+                                       result=_unique_features,
+                                       size=len(_unique_features),
+                                       ratio=self.get_ratio(_unique_features, self._features, 2))
         return result
 
     @metric_method
-    def false_optional_features(self) -> Dict[str, Any]:
-        """Features defined as optionals the selection of their parents make the feature itself selected as well."""
+    def false_optional_features(self) -> dict[str, Any]:
+        """Features defined as optionals the selection of their parents make the feature itself 
+        selected as well."""
+        if self.model is None:
+            raise FlamaException('Model not initialized.')
         name = "False-optional features"
-        _false_optional_features=sat_operations.PySATFalseOptionalFeatures().execute(self.model).get_result()
-        result = self.construct_result( name=name,
-                        doc=self.false_optional_features.__doc__,
-                        result=_false_optional_features,
-                        size=len(_false_optional_features),
-                        ratio=self.get_ratio(_false_optional_features, self._features, 2))
+        _fof = sat_operations.PySATFalseOptionalFeatures().execute(self.model).get_result()
+        result = self.construct_result(name=name,
+                                       doc=self.false_optional_features.__doc__,
+                                       result=_fof,
+                                       size=len(_fof),
+                                       ratio=self.get_ratio(_fof, self._features, 2))
         return result
 
     @metric_method
-    def configurations(self) -> Tuple[str, str, Union[int, float]]:
-        """Number of configurations represented by the feature model. If <= is shown, the number represents an upper estimation bound."""
+    def configurations(self) -> dict[str, Any]:
+        """Number of configurations represented by the feature model. 
+
+           If <= is shown, the number represents an upper estimation bound.
+        """
+        if self.model is None:
+            raise FlamaException('Model not initialized.')
         name = "Configurations"
         _configurations = sat_operations.PySATProducts().execute(self.model).get_result()
-        result = self.construct_result( name=name,
-                        doc=self.configurations.__doc__,
-                        result=_configurations,
-                        size=len(_configurations))
+        result = self.construct_result(name=name,
+                                       doc=self.configurations.__doc__,
+                                       result=_configurations,
+                                       size=len(_configurations))
         return result
-
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_products.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_satisfiable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from typing import Any, cast
+from typing import cast
 
 from pysat.solvers import Solver
 
-from flamapy.core.operations import Products
+from flamapy.core.operations import Satisfiable
+
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.core.models import VariabilityModel
 
 
-class PySATProducts(Products):
+class PySATSatisfiable(Satisfiable):
 
     def __init__(self) -> None:
-        self.products: list[list[Any]] = []
+        self.result = False
         self.solver = Solver(name='glucose3')
 
-    def get_products(self) -> list[list[Any]]:
-        return self.products
-
-    def get_result(self) -> list[list[Any]]:
-        return self.get_products()
+    def is_satisfiable(self) -> bool:
+        return self.get_result()
 
-    def execute(self, model: VariabilityModel) -> 'PySATProducts':
-        model = cast(PySATModel, model)
+    def get_result(self) -> bool:
+        return self.result
 
-        for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
-            self.solver.add_clause(clause)  # añadimos la constraint
-
-        for solutions in self.solver.enum_models():
-            product = []
-            for variable in solutions:
-                if variable > 0:
-                    product.append(model.features.get(variable))
-            self.products.append(product)
-        self.solver.delete()
+    def execute(self, model: VariabilityModel) -> 'PySATSatisfiable':
+        sat_model = cast(PySATModel, model)
+        self.result = valid(self.solver, sat_model)
         return self
+
+
+def valid(solver: Solver, model: PySATModel) -> bool:
+    for clause in model.get_all_clauses():
+        solver.add_clause(clause)
+    result = solver.solve()
+    solver.delete()
+    return result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_products_number.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/operations/pysat_configurations_number.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import cast
 
 from pysat.solvers import Solver
 
-from flamapy.core.operations import ProductsNumber
+from flamapy.core.operations import ConfigurationsNumber
 from flamapy.metamodels.pysat_metamodel.models.pysat_model import PySATModel
 from flamapy.core.models import VariabilityModel
 
 
-class PySATProductsNumber(ProductsNumber):
+class PySATConfigurationsNumber(ConfigurationsNumber):
 
     def __init__(self) -> None:
         self.products_number = 0
         self.solver = Solver(name='glucose3')
 
-    def get_products_number(self) -> int:
+    def get_configurations_number(self) -> int:
         return self.products_number
 
     def get_result(self) -> int:
-        return self.get_products_number()
+        return self.get_configurations_number()
 
-    def execute(self, model: VariabilityModel) -> 'PySATProductsNumber':
+    def execute(self, model: VariabilityModel) -> 'PySATConfigurationsNumber':
         model = cast(PySATModel, model)
 
         for clause in model.get_all_clauses():  # AC es conjunto de conjuntos
             self.solver.add_clause(clause)  # añadimos la constraint
 
         for _ in self.solver.enum_models():
             self.products_number += 1
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py`

 * *Files identical despite different names*

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,25 @@
             features_lines = []
             clauses_lines = []
             for line in lines:
                 if line.startswith('c'):
                     features_lines.append(line)
                 elif line.startswith('p'):
                     problem = line
-                else:
+                elif line != '':
                     clauses_lines.append(line)
             if problem is None:
-                raise FlamaException(f'Incorrect Dimacs format of {self.path}')
+                raise FlamaException(f'Incorrect Dimacs format of {self.path}. '
+                                     f'No problem statement.')
 
             problem_list = problem.split()
-            n_features = int(problem_list[2])
             n_clauses = int(problem_list[3])
-            if n_features != len(features_lines) or n_clauses != len(clauses_lines):
-                raise FlamaException(f'Incorrect Dimacs format of {self.path}')
+            if n_clauses != len(clauses_lines):
+                raise FlamaException(f'Incorrect Dimacs format of {self.path}. '
+                                     f'Inconsistent number of clauses.')
         features, variables = self._parse_features_variables(features_lines)
         sat_model = PySATModel()
         sat_model.features = features
         sat_model.variables = variables
         self._parse_clauses(sat_model, clauses_lines)
         return sat_model
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
     def __init__(self, path: str, source_model: PySATModel) -> None:
         self.path = path
         self.source_model = source_model
 
     def transform(self) -> str:
         dimacs_str = pysat_to_dimacs(self.source_model)
-        with open(self.path, 'w', encoding='utf8') as file:
-            file.write(dimacs_str)
+        if self.path is not None:
+            with open(self.path, 'w', encoding='utf8') as file:
+                file.write(dimacs_str)
         return dimacs_str
 
 
 def pysat_to_dimacs(model: PySATModel) -> str:
     lines = []
     features_dict = model.features
     clauses_list = model.get_all_clauses().clauses
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py` & `flamapy-sat-2.0.0.dev0/flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 from typing import Any, List
-import logging
+
 from flamapy.core.transformations import ModelToModel
 from flamapy.metamodels.fm_metamodel.models.feature_model import (
     FeatureModel,
     Constraint,
     Feature,
     Relation,
 )
@@ -20,86 +20,84 @@
     def get_destination_extension() -> str:
         return 'pysat'
 
     def __init__(self, source_model: FeatureModel) -> None:
         self.source_model = source_model
         self.counter = 1
         self.destination_model = PySATModel()
-        self.destination_model.original_model =source_model
+        self.destination_model.original_model = source_model
         # self.r_cnf = self.destination_model.r_cnf
         # self.ctc_cnf = self.destination_model.ctc_cnf
 
     def add_feature(self, feature: Feature) -> None:
         if feature.name not in self.destination_model.variables:
             self.destination_model.variables[feature.name] = self.counter
             self.destination_model.features[self.counter] = feature.name
             self.counter += 1
 
     def add_root(self, feature: Feature) -> None:
         # self.r_cnf.append([self.destination_model.variables.get(feature.name)])
         value = self.destination_model.get_variable(feature.name)
         self.destination_model.add_clause([value])
-    
+
     def _add_mandatory_relation(self, relation: Relation) -> List[List[int]]:
         value_parent = self.destination_model.get_variable(relation.parent.name)
         value_child = self.destination_model.get_variable(relation.children[0].name)
         clauses = [[-1 * value_parent, value_child], [-1 * value_child, value_parent]]
         return clauses
-    
+
     def _add_optional_relation(self, relation: Relation) -> List[List[int]]:
         value_parent = self.destination_model.get_variable(relation.parent.name)
         value_children = self.destination_model.get_variable(relation.children[0].name)
-
-        clauses =[[-1 * value_children, value_parent]]
+        clauses = [[-1 * value_children, value_parent]]
         return clauses
 
     def _add_or_relation(self, relation: Relation) -> List[List[int]]:
         # this is a 1 to n relatinship with multiple childs
         # add the first cnf child1 or child2 or ... or childN or no parent)
         # first elem of the constraint
         value_parent = self.destination_model.get_variable(relation.parent.name)
 
         alt_cnf = [-1 * value_parent]
         for child in relation.children:
             alt_cnf.append(self.destination_model.get_variable(child.name))
-        clauses=[alt_cnf]
+        clauses = [alt_cnf]
 
         for child in relation.children:
             clauses.append([
                 -1 * self.destination_model.get_variable(child.name),
                 value_parent
             ])
 
         return clauses
-        
+
     def _add_alternative_relation(self, relation: Relation) -> List[List[int]]:
-        # pylint: disable=too-many-nested-blocks
         # this is a 1 to 1 relatinship with multiple childs
         # add the first cnf child1 or child2 or ... or childN or no parent)
 
         value_parent = self.destination_model.get_variable(relation.parent.name)
         # first elem of the constraint
         alt_cnf = [-1 * value_parent]
         for child in relation.children:
             alt_cnf.append(self.destination_model.get_variable(child.name))
-        clauses=[alt_cnf]
+        clauses = [alt_cnf]
 
         for i, _ in enumerate(relation.children):
             for j in range(i + 1, len(relation.children)):
                 if i != j:
                     clauses.append([
                         -1 * self.destination_model.get_variable(relation.children[i].name),
                         -1 * self.destination_model.get_variable(relation.children[j].name)
                     ])
             clauses.append([
                 -1 * self.destination_model.get_variable(relation.children[i].name),
                 value_parent
             ])
         return clauses
-    
+
     def _add_constraint_relation(self, relation: Relation) -> List[List[int]]:
         value_parent = self.destination_model.get_variable(relation.parent.name)
 
         # This is a _min to _max relationship
         _min = relation.card_min
         _max = relation.card_max
 
@@ -126,32 +124,32 @@
                 cnf = [value_parent]
                 for feat in relation.children:
                     if feat in combination:
                         cnf.append(-1 * self.destination_model.get_variable(feat.name))
                     else:
                         cnf.append(self.destination_model.get_variable(feat.name))
                 clauses.append(cnf)
+        return clauses
 
-    def _store_constraint_relation(self, relation: Relation, clauses:List[List[int]]) -> None:
+    def _store_constraint_clauses(self, clauses: List[List[int]]) -> None:
         for clause in clauses:
             self.destination_model.add_clause(clause)
-    
-    def add_relation(self, relation: Relation) -> None:  # noqa: MC0001
+
+    def add_relation(self, relation: Relation) -> None:
         if relation.is_mandatory():
             clauses = self._add_mandatory_relation(relation)
         elif relation.is_optional():
             clauses = self._add_optional_relation(relation)
         elif relation.is_or():  
             clauses = self._add_or_relation(relation)
         elif relation.is_alternative():  
             clauses = self._add_alternative_relation(relation)
         else:
             clauses = self._add_constraint_relation(relation)
-
-        self._store_constraint_relation(relation,clauses)
+        self._store_constraint_clauses(clauses)
 
     def add_constraint(self, ctc: Constraint) -> None:
         def get_term_variable(term: Any) -> int:
             if term.startswith('-'):
                 return -self.destination_model.get_variable(term[1:])
 
             return self.destination_model.get_variable(term)
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/PKG-INFO` & `flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-sat
-Version: 1.6.0.dev0
+Version: 2.0.0.dev0
 Summary: flamapy-sat is a plugin to flamapy module
 Home-page: https://github.com/flamapy/pysat_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-sat-1.6.0.dev0/flamapy_sat.egg-info/SOURCES.txt` & `flamapy-sat-2.0.0.dev0/flamapy_sat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 flamapy/metamodels/pysat_diagnosis_metamodel/transformations/fm_to_diag_pysat.py
 flamapy/metamodels/pysat_metamodel/__init__.py
 flamapy/metamodels/pysat_metamodel/models/__init__.py
 flamapy/metamodels/pysat_metamodel/models/pysat_model.py
 flamapy/metamodels/pysat_metamodel/models/txtcnf_model.py
 flamapy/metamodels/pysat_metamodel/operations/__init__.py
 flamapy/metamodels/pysat_metamodel/operations/pysat_commonality.py
+flamapy/metamodels/pysat_metamodel/operations/pysat_configurations.py
+flamapy/metamodels/pysat_metamodel/operations/pysat_configurations_number.py
 flamapy/metamodels/pysat_metamodel/operations/pysat_core_features.py
 flamapy/metamodels/pysat_metamodel/operations/pysat_dead_features.py
 flamapy/metamodels/pysat_metamodel/operations/pysat_false_optional_features.py
 flamapy/metamodels/pysat_metamodel/operations/pysat_filter.py
 flamapy/metamodels/pysat_metamodel/operations/pysat_metrics.py
-flamapy/metamodels/pysat_metamodel/operations/pysat_products.py
-flamapy/metamodels/pysat_metamodel/operations/pysat_products_number.py
-flamapy/metamodels/pysat_metamodel/operations/pysat_valid.py
-flamapy/metamodels/pysat_metamodel/operations/pysat_valid_configuration.py
-flamapy/metamodels/pysat_metamodel/operations/pysat_valid_product.py
+flamapy/metamodels/pysat_metamodel/operations/pysat_sampling.py
+flamapy/metamodels/pysat_metamodel/operations/pysat_satisfiable.py
+flamapy/metamodels/pysat_metamodel/operations/pysat_satisfiable_configuration.py
 flamapy/metamodels/pysat_metamodel/transformations/__init__.py
 flamapy/metamodels/pysat_metamodel/transformations/cnf_to_pysat.py
 flamapy/metamodels/pysat_metamodel/transformations/dimacs_reader.py
 flamapy/metamodels/pysat_metamodel/transformations/dimacs_writer.py
 flamapy/metamodels/pysat_metamodel/transformations/fm_to_pysat.py
 flamapy_sat.egg-info/PKG-INFO
 flamapy_sat.egg-info/SOURCES.txt
```

### Comparing `flamapy-sat-1.6.0.dev0/setup.py` & `flamapy-sat-2.0.0.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-sat",
-    version="1.6.0.dev0",
+    version="2.0.0.dev0",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="flamapy-sat is a plugin to flamapy module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/pysat_metamodel",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
-        'flamapy~=1.6.0.dev0',
-        'flamapy-fm~=1.5.0.dev0',
+        'flamapy-fw~=2.0.0.dev0',
+        'flamapy-fm~=2.0.0.dev0',
         'python-sat>=0.1.7.dev6'
     ],
     extras_require={
         'dev': [
             'pytest',
             'pytest-mock',
             'prospector',
```

