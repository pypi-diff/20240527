# Comparing `tmp/flamapy-bdd-1.6.0.tar.gz` & `tmp/flamapy-bdd-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-bdd-1.6.0.tar", last modified: Mon Jan  8 10:51:51 2024, max compression
+gzip compressed data, was "flamapy-bdd-2.0.0.dev1.tar", last modified: Mon May 27 21:05:47 2024, max compression
```

## Comparing `flamapy-bdd-1.6.0.tar` & `flamapy-bdd-2.0.0.dev1.tar`

### file list

```diff
@@ -1,37 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.157057 flamapy-bdd-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-01-08 10:51:51.157057 flamapy-bdd-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.153057 flamapy-bdd-1.6.0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.153057 flamapy-bdd-1.6.0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.153057 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.153057 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/models/bdd_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.153057 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/models/utils/txtcnf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.157057 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_feature_inclusion_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_product_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_products.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_products_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.157057 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/interfaces/feature_inclusion_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/interfaces/product_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.157057 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/transformations/bdd_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/transformations/fm_to_bdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/transformations/sat_to_bdd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:51:51.157057 flamapy-bdd-1.6.0/flamapy_bdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-01-08 10:51:51.000000 flamapy-bdd-1.6.0/flamapy_bdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-01-08 10:51:51.000000 flamapy-bdd-1.6.0/flamapy_bdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-08 10:51:51.000000 flamapy-bdd-1.6.0/flamapy_bdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-08 10:51:51.000000 flamapy-bdd-1.6.0/flamapy_bdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-08 10:51:51.000000 flamapy-bdd-1.6.0/flamapy_bdd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 10:51:51.157057 flamapy-bdd-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-08 10:51:38.000000 flamapy-bdd-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.832248 flamapy-bdd-2.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-27 21:05:47.832248 flamapy-bdd-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.824247 flamapy-bdd-2.0.0.dev1/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.824247 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.824247 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.824247 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/models/bdd_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.828248 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/models/utils/txtcnf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.828248 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_commonality_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_configurations_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_core_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_feature_inclusion_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_homogeneity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_product_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_pure_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_satisfiable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_unique_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_variability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_variant_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.828248 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/commonality_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/feature_inclusion_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/homogeneity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/product_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/pure_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/unique_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/variability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/variant_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.832248 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/_bdd_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/dddmp_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/dddmp_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/fm_to_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/fm_to_bdd_cnf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/fm_to_bdd_pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/json_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/pdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/pickle_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/pickle_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/png_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/sat_to_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/svg_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:05:47.832248 flamapy-bdd-2.0.0.dev1/flamapy_bdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-27 21:05:47.000000 flamapy-bdd-2.0.0.dev1/flamapy_bdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-27 21:05:47.000000 flamapy-bdd-2.0.0.dev1/flamapy_bdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 21:05:47.000000 flamapy-bdd-2.0.0.dev1/flamapy_bdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-27 21:05:47.000000 flamapy-bdd-2.0.0.dev1/flamapy_bdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 21:05:47.000000 flamapy-bdd-2.0.0.dev1/flamapy_bdd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:05:47.832248 flamapy-bdd-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-27 21:05:39.000000 flamapy-bdd-2.0.0.dev1/setup.py
```

### Comparing `flamapy-bdd-1.6.0/PKG-INFO` & `flamapy-bdd-2.0.0.dev1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 2.1
-Name: flamapy-bdd
-Version: 1.6.0
-Summary: bdd-plugin for the automated analysis of feature models
-Home-page: https://github.com/flamapy/bdd_metamodel
-Author: Flamapy
-Author-email: flamapy@us.es
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # BDD plugin for flamapy
 - [BDD plugin for flamapy](#bdd-plugin-for-flamapy)
   - [Description](#description)
   - [Requirements and Installation](#requirements-and-installation)
   - [Functionality and usage](#functionality-and-usage)
-    - [Load a feature model and create the BDD](#load-a-feature-model-and-create-the-bdd)
+    - [Load a feature model in UVL and create the BDD](#load-a-feature-model-in-uvl-and-create-the-bdd)
     - [Save the BDD in a file](#save-the-bdd-in-a-file)
+    - [Load the BDD from a file](#load-the-bdd-from-a-file)
     - [Analysis operations](#analysis-operations)
   - [Contributing to the BDD plugin](#contributing-to-the-bdd-plugin)
 
 
 ## Description
 This plugin supports Binary Decision Diagrams (BDDs) representations for feature models.
 
@@ -60,136 +45,138 @@
 
 ## Functionality and usage
 The executable script [test_bdd_metamodel.py](https://github.com/flamapy/bdd_metamodel/blob/master/tests/test_bdd_metamodel.py) serves as an entry point to show the plugin in action.
 
 The following functionality is provided:
 
 
-### Load a feature model and create the BDD
+### Load a feature model in UVL and create the BDD
 ```python
-from flamapy.metamodels.fm_metamodel.transformations.featureide_reader import FeatureIDEReader
-from flamapy.metamodels.bdd_metamodel.transformations.fm_to_bdd import FmToBDD
+from flamapy.metamodels.fm_metamodel.transformations import UVLReader
+from flamapy.metamodels.bdd_metamodel.transformations import FmToBDD
 
-# Load the feature model from FeatureIDE
-feature_model = FeatureIDEReader('input_fms/featureide_models/pizzas.xml').transform()
+# Load the feature model from UVL
+feature_model = UVLReader('models/uvl_models/pizzas.uvl').transform()
 # Create the BDD from the feature model
 bdd_model = FmToBDD(feature_model).transform()
 ```
 
 
 ### Save the BDD in a file
 ```python
-from flamapy.metamodels.bdd_metamodel.transformations.bdd_writer import BDDWriter, BDDDumpFormat
+from flamapy.metamodels.bdd_metamodel.transformations import PNGWriter, DDDMPv3Writer
 # Save the BDD as an image in PNG
-BDDWriter(path='my_bdd.png',
-          source_model=bdd_model,
-          roots=[bdd_model.root],
-          output_format=BDDDumpFormat.PNG).transform()
+PNGWriter(path='my_bdd.png', bdd_model).transform()
+# Save the BDD in a .dddmp file
+DDDMPv3Writer(f'my_bdd.dddmp', bdd_model).transform()
+```
+Writers available: DDDMPv3 ('dddmp'), DDDMPv2 ('dddmp'), JSON ('json'), Pickle ('p'), PDF ('pdf'), PNG ('png'), SVG ('svg').
+
+### Load the BDD from a file
+```python
+from flamapy.metamodels.bdd_metamodel.transformations import JSONReader
+# Load the BDD from a .json file
+bdd_model = JSONReader(path='path/to/my_bdd.json').transform()
 ```
-Formats supported: DDDMP_V3 ('dddmp'), DDDMP_V2 ('dddmp2'), PDF ('pdf'), PNG ('png'), SVG ('svg').
+Readers available: JSON ('json'), DDDMP ('dddmp'), Pickle ('p').
 
+*NOTE:* DDDMP and Pickle readers are not fully supported yet.
 
 ### Analysis operations
 
-- Products number
+- Satisfiable
 
-    Return the number of products (configurations):
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProductsNumber
-    nof_products = BDDProductsNumber().execute(bdd_model).get_result()
-    print(f'#Products: {nof_products}')
-    ```
-    or alternatively:
+    Return whether the model is satisfiable (valid):
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import products_number
-    nof_products = products_number(bdd_model)
-    print(f'#Products: {nof_products}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDSatisfiable
+    satisfiable = BDDSatisfiable().execute(bdd_model).get_result()
+    print(f'Satisfiable? (valid?): {satisfiable}')
     ```
 
-- Products
+- Configurations number
 
-    Return the list of products (configurations):
+    Return the number of configurations:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProducts
-    list_products = BDDProducts().execute(bdd_model).get_result()
-    for i, prod in enumerate(list_products):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDConfigurationsNumber
+    n_configs = BDDConfigurationsNumber().execute(bdd_model).get_result()
+    print(f'#Configurations: {n_configs}')
     ```
-    or alternatively:
+
+- Configurations
+
+    Enumerate the configurations of the model:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import products
-    nof_products = products(bdd_model)
-    for i, prod in enumerate(list_products):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDConfigurations
+    configurations = BDDConfigurations().execute(bdd_model).get_result()
+    for i, config in enumerate(configurations, 1):
+        print(f'Config {i}: {[feat for feat in config.elements if config.elements[feat]]}')
     ```
 
 - Sampling
 
-    Return a sample of the given size of uniform random products (configurations) with or without replacement:
+    Return a sample of the given size of uniform random configurations with or without replacement:
     ```python
     from flamapy.metamodels.bdd_metamodel.operations import BDDSampling
-    list_sample = BDDSampling(size=5, with_replacement=False).execute(bdd_model).get_result()
-    for i, prod in enumerate(list_sample):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
-    ```
-    or alternatively:
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import sample
-    list_sample = sample(bdd_model, size=5, with_replacement=False)
-    for i, prod in enumerate(list_sample):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    sampling_op = BDDSampling()
+    sampling_op.set_sample_size(5)
+    sampling_op.set_with_replacement(False)  # Default False
+    sample = sampling_op.execute(bdd_model).get_result()
+    for i, config in enumerate(sample, 1):
+        print(f'Config {i}: {[feat for feat in config.elements if config.elements[feat]]}')
     ```
 
 - Product Distribution
 
-    Return the number of products having a given number of features:
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProductDistributionBF
-    dist = BDDProductDistributionBF().execute(bdd_model).get_result()
-    print(f'Product Distribution: {dist}')
-    ```
-    or alternatively:
+    Return the number of products (configurations) having a given number of features:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import product_distribution
-    dist = product_distribution(bdd_model)
+    from flamapy.metamodels.bdd_metamodel.operations import BDDProductDistribution
+    dist = BDDProductDistribution().execute(bdd_model).get_result()
     print(f'Product Distribution: {dist}')
     ```
 
 - Feature Inclusion Probability
 
-    Return the probability for a feature to be included in a valid product:
+    Return the probability for a feature to be included in a valid configuration:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDFeatureInclusionProbabilityBF
-    prob = BDDFeatureInclusionProbabilityBF().execute(bdd_model).get_result()
+    from flamapy.metamodels.bdd_metamodel.operations import BDDFeatureInclusionProbability
+    prob = BDDFeatureInclusionProbability().execute(bdd_model).get_result()
     for feat in prob.keys():
         print(f'{feat}: {prob[feat]}')
     ```
-    or alternatively:
+
+- Core features
+
+    Return the core features (those features that are present in all the configurations):
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import feature_inclusion_probability
-    prob = feature_inclusion_probability(bdd_model)
-    for feat in prob.keys():
-        print(f'{feat}: {prob[feat]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDCoreFeatures
+    core_features = BDDCoreFeatures().execute(bdd_model).get_result()
+    print(f'Core features: {core_features}')
     ```
 
-All analysis operations support also a partial configuration as an additional argument, so the operation will return the result taking into account the given partial configuration. For example:
+- Dead features
+
+    Return the dead features (those features that are not present in any configuration):
+    ```python
+    from flamapy.metamodels.bdd_metamodel.operations import BDDDeadFeatures
+    dead_features = BDDDeadFeatures().execute(bdd_model).get_result()
+    print(f'Dead features: {dead_features}')
+    ```
+
+Most analysis operations support also a partial configuration as an additional argument, so the operation will return the result taking into account the given partial configuration. For example:
 
 ```python
 from flamapy.core.models import Configuration
 # Create a partial configuration
 elements = {'Pizza': True, 'Big': True}
 partial_config = Configuration(elements)
-# Calculate the number of products from the partial configuration
-nof_products = BDDProductsNumber(partial_config).execute(bdd_model).get_result()
-print(f'#Products: {nof_products}')
-```
-or alternatively:
-```python
-nof_products = products(bdd_model, partial_config)
-print(f'#Products: {nof_products}')
+# Calculate the number of configuration from the partial configuration
+configs_number_op = BDDConfigurationsNumber()
+configs_number_op.set_partial_configuration(partial_config)
+n_configs = configs_number_op.execute(bdd_model).get_result()
+print(f'#Configurations: {n_configs}')
 ```
 
 
 ## Contributing to the BDD plugin
 To contribute in the development of this plugin:
 
 1. Fork the repository into your GitHub account.
@@ -205,9 +192,7 @@
 
     `make lint`
 
 - To analyze the static type checker for Python and find bugs, pass the Mypy:
 
     `make mypy`
 
-
-
```

### Comparing `flamapy-bdd-1.6.0/README.md` & `flamapy-bdd-2.0.0.dev1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,31 @@
+Metadata-Version: 2.1
+Name: flamapy-bdd
+Version: 2.0.0.dev1
+Summary: bdd-plugin for the automated analysis of feature models
+Home-page: https://github.com/flamapy/bdd_metamodel
+Author: Flamapy
+Author-email: flamapy@us.es
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # BDD plugin for flamapy
 - [BDD plugin for flamapy](#bdd-plugin-for-flamapy)
   - [Description](#description)
   - [Requirements and Installation](#requirements-and-installation)
   - [Functionality and usage](#functionality-and-usage)
-    - [Load a feature model and create the BDD](#load-a-feature-model-and-create-the-bdd)
+    - [Load a feature model in UVL and create the BDD](#load-a-feature-model-in-uvl-and-create-the-bdd)
     - [Save the BDD in a file](#save-the-bdd-in-a-file)
+    - [Load the BDD from a file](#load-the-bdd-from-a-file)
     - [Analysis operations](#analysis-operations)
   - [Contributing to the BDD plugin](#contributing-to-the-bdd-plugin)
 
 
 ## Description
 This plugin supports Binary Decision Diagrams (BDDs) representations for feature models.
 
@@ -44,136 +61,138 @@
 
 ## Functionality and usage
 The executable script [test_bdd_metamodel.py](https://github.com/flamapy/bdd_metamodel/blob/master/tests/test_bdd_metamodel.py) serves as an entry point to show the plugin in action.
 
 The following functionality is provided:
 
 
-### Load a feature model and create the BDD
+### Load a feature model in UVL and create the BDD
 ```python
-from flamapy.metamodels.fm_metamodel.transformations.featureide_reader import FeatureIDEReader
-from flamapy.metamodels.bdd_metamodel.transformations.fm_to_bdd import FmToBDD
+from flamapy.metamodels.fm_metamodel.transformations import UVLReader
+from flamapy.metamodels.bdd_metamodel.transformations import FmToBDD
 
-# Load the feature model from FeatureIDE
-feature_model = FeatureIDEReader('input_fms/featureide_models/pizzas.xml').transform()
+# Load the feature model from UVL
+feature_model = UVLReader('models/uvl_models/pizzas.uvl').transform()
 # Create the BDD from the feature model
 bdd_model = FmToBDD(feature_model).transform()
 ```
 
 
 ### Save the BDD in a file
 ```python
-from flamapy.metamodels.bdd_metamodel.transformations.bdd_writer import BDDWriter, BDDDumpFormat
+from flamapy.metamodels.bdd_metamodel.transformations import PNGWriter, DDDMPv3Writer
 # Save the BDD as an image in PNG
-BDDWriter(path='my_bdd.png',
-          source_model=bdd_model,
-          roots=[bdd_model.root],
-          output_format=BDDDumpFormat.PNG).transform()
+PNGWriter(path='my_bdd.png', bdd_model).transform()
+# Save the BDD in a .dddmp file
+DDDMPv3Writer(f'my_bdd.dddmp', bdd_model).transform()
+```
+Writers available: DDDMPv3 ('dddmp'), DDDMPv2 ('dddmp'), JSON ('json'), Pickle ('p'), PDF ('pdf'), PNG ('png'), SVG ('svg').
+
+### Load the BDD from a file
+```python
+from flamapy.metamodels.bdd_metamodel.transformations import JSONReader
+# Load the BDD from a .json file
+bdd_model = JSONReader(path='path/to/my_bdd.json').transform()
 ```
-Formats supported: DDDMP_V3 ('dddmp'), DDDMP_V2 ('dddmp2'), PDF ('pdf'), PNG ('png'), SVG ('svg').
+Readers available: JSON ('json'), DDDMP ('dddmp'), Pickle ('p').
 
+*NOTE:* DDDMP and Pickle readers are not fully supported yet.
 
 ### Analysis operations
 
-- Products number
+- Satisfiable
 
-    Return the number of products (configurations):
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProductsNumber
-    nof_products = BDDProductsNumber().execute(bdd_model).get_result()
-    print(f'#Products: {nof_products}')
-    ```
-    or alternatively:
+    Return whether the model is satisfiable (valid):
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import products_number
-    nof_products = products_number(bdd_model)
-    print(f'#Products: {nof_products}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDSatisfiable
+    satisfiable = BDDSatisfiable().execute(bdd_model).get_result()
+    print(f'Satisfiable? (valid?): {satisfiable}')
     ```
 
-- Products
+- Configurations number
 
-    Return the list of products (configurations):
+    Return the number of configurations:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProducts
-    list_products = BDDProducts().execute(bdd_model).get_result()
-    for i, prod in enumerate(list_products):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDConfigurationsNumber
+    n_configs = BDDConfigurationsNumber().execute(bdd_model).get_result()
+    print(f'#Configurations: {n_configs}')
     ```
-    or alternatively:
+
+- Configurations
+
+    Enumerate the configurations of the model:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import products
-    nof_products = products(bdd_model)
-    for i, prod in enumerate(list_products):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDConfigurations
+    configurations = BDDConfigurations().execute(bdd_model).get_result()
+    for i, config in enumerate(configurations, 1):
+        print(f'Config {i}: {[feat for feat in config.elements if config.elements[feat]]}')
     ```
 
 - Sampling
 
-    Return a sample of the given size of uniform random products (configurations) with or without replacement:
+    Return a sample of the given size of uniform random configurations with or without replacement:
     ```python
     from flamapy.metamodels.bdd_metamodel.operations import BDDSampling
-    list_sample = BDDSampling(size=5, with_replacement=False).execute(bdd_model).get_result()
-    for i, prod in enumerate(list_sample):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
-    ```
-    or alternatively:
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import sample
-    list_sample = sample(bdd_model, size=5, with_replacement=False)
-    for i, prod in enumerate(list_sample):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    sampling_op = BDDSampling()
+    sampling_op.set_sample_size(5)
+    sampling_op.set_with_replacement(False)  # Default False
+    sample = sampling_op.execute(bdd_model).get_result()
+    for i, config in enumerate(sample, 1):
+        print(f'Config {i}: {[feat for feat in config.elements if config.elements[feat]]}')
     ```
 
 - Product Distribution
 
-    Return the number of products having a given number of features:
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProductDistributionBF
-    dist = BDDProductDistributionBF().execute(bdd_model).get_result()
-    print(f'Product Distribution: {dist}')
-    ```
-    or alternatively:
+    Return the number of products (configurations) having a given number of features:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import product_distribution
-    dist = product_distribution(bdd_model)
+    from flamapy.metamodels.bdd_metamodel.operations import BDDProductDistribution
+    dist = BDDProductDistribution().execute(bdd_model).get_result()
     print(f'Product Distribution: {dist}')
     ```
 
 - Feature Inclusion Probability
 
-    Return the probability for a feature to be included in a valid product:
+    Return the probability for a feature to be included in a valid configuration:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDFeatureInclusionProbabilityBF
-    prob = BDDFeatureInclusionProbabilityBF().execute(bdd_model).get_result()
+    from flamapy.metamodels.bdd_metamodel.operations import BDDFeatureInclusionProbability
+    prob = BDDFeatureInclusionProbability().execute(bdd_model).get_result()
     for feat in prob.keys():
         print(f'{feat}: {prob[feat]}')
     ```
-    or alternatively:
+
+- Core features
+
+    Return the core features (those features that are present in all the configurations):
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import feature_inclusion_probability
-    prob = feature_inclusion_probability(bdd_model)
-    for feat in prob.keys():
-        print(f'{feat}: {prob[feat]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDCoreFeatures
+    core_features = BDDCoreFeatures().execute(bdd_model).get_result()
+    print(f'Core features: {core_features}')
     ```
 
-All analysis operations support also a partial configuration as an additional argument, so the operation will return the result taking into account the given partial configuration. For example:
+- Dead features
+
+    Return the dead features (those features that are not present in any configuration):
+    ```python
+    from flamapy.metamodels.bdd_metamodel.operations import BDDDeadFeatures
+    dead_features = BDDDeadFeatures().execute(bdd_model).get_result()
+    print(f'Dead features: {dead_features}')
+    ```
+
+Most analysis operations support also a partial configuration as an additional argument, so the operation will return the result taking into account the given partial configuration. For example:
 
 ```python
 from flamapy.core.models import Configuration
 # Create a partial configuration
 elements = {'Pizza': True, 'Big': True}
 partial_config = Configuration(elements)
-# Calculate the number of products from the partial configuration
-nof_products = BDDProductsNumber(partial_config).execute(bdd_model).get_result()
-print(f'#Products: {nof_products}')
-```
-or alternatively:
-```python
-nof_products = products(bdd_model, partial_config)
-print(f'#Products: {nof_products}')
+# Calculate the number of configuration from the partial configuration
+configs_number_op = BDDConfigurationsNumber()
+configs_number_op.set_partial_configuration(partial_config)
+n_configs = configs_number_op.execute(bdd_model).get_result()
+print(f'#Configurations: {n_configs}')
 ```
 
 
 ## Contributing to the BDD plugin
 To contribute in the development of this plugin:
 
 1. Fork the repository into your GitHub account.
@@ -189,7 +208,9 @@
 
     `make lint`
 
 - To analyze the static type checker for Python and find bugs, pass the Mypy:
 
     `make mypy`
 
+
+
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/models/utils/txtcnf.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/models/utils/txtcnf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,210 +1,235 @@
 from typing import Optional
 from enum import Enum, auto
 
+from flamapy.core.exceptions import FlamaException
+
 
 class CNFLogicConnective(Enum):
     """The propositional logic connectives a formula in CNF can contain."""
+
     NOT = auto()
     AND = auto()
     OR = auto()
 
 
 class TextCNFNotation(Enum):
-    """Possible notations of a CNF formula. 
+    """Possible notations of a CNF formula.
 
     Five different notations are available:
         Logical symbols:
             (A) ∧ (¬B ∨ C) ∧ ...
         Textual symbols:
             (A) and (not B or C) and ...
         Java symbols:
             (A) && (!B || C) && ...
         Java Short symbols:
             (A) & (!B | C) && ...
         Short symbols:
             (A) & (-B | C) & ...
     """
-    LOGICAL = {CNFLogicConnective.NOT: '¬', 
-               CNFLogicConnective.AND: '∧', 
-               CNFLogicConnective.OR: '∨'}
-    TEXTUAL = {CNFLogicConnective.NOT: 'not', 
-               CNFLogicConnective.AND: 'and', 
-               CNFLogicConnective.OR: 'or'}
-    JAVA = {CNFLogicConnective.NOT: '!', 
-            CNFLogicConnective.AND: '&&', 
-            CNFLogicConnective.OR: '||'}
-    JAVA_SHORT = {CNFLogicConnective.NOT: '!', 
-                  CNFLogicConnective.AND: '&', 
-                  CNFLogicConnective.OR: '|'}
-    SHORT = {CNFLogicConnective.NOT: '-', 
-             CNFLogicConnective.AND: '&', 
-             CNFLogicConnective.OR: '|'}
 
+    LOGICAL = {
+        CNFLogicConnective.NOT: "¬",
+        CNFLogicConnective.AND: "∧",
+        CNFLogicConnective.OR: "∨",
+    }
+    TEXTUAL = {
+        CNFLogicConnective.NOT: "not",
+        CNFLogicConnective.AND: "and",
+        CNFLogicConnective.OR: "or",
+    }
+    JAVA = {
+        CNFLogicConnective.NOT: "!",
+        CNFLogicConnective.AND: "&&",
+        CNFLogicConnective.OR: "||",
+    }
+    JAVA_SHORT = {
+        CNFLogicConnective.NOT: "!",
+        CNFLogicConnective.AND: "&",
+        CNFLogicConnective.OR: "|",
+    }
+    SHORT = {
+        CNFLogicConnective.NOT: "-",
+        CNFLogicConnective.AND: "&",
+        CNFLogicConnective.OR: "|",
+    }
 
-class TextCNFModel():
+
+class TextCNFModel:
     """Textual representation of a conjunctive normal form (CNF) formula.
 
-    A CNF formula (or clausal normal form) is a conjunction of one or more clauses, 
+    A CNF formula (or clausal normal form) is a conjunction of one or more clauses,
     where a clause is a disjunction of literals.
     """
 
     def __init__(self) -> None:
         self._cnf_formula: Optional[str] = None
         self._cnf_notation: Optional[TextCNFNotation] = None
         self._variables: list[str] = []  # list of str with variables' names
 
     def from_textual_cnf(self, cnf_formula: str) -> None:
         self._cnf_formula = cnf_formula
         self._cnf_notation = identify_notation(cnf_formula)
         self._variables = extract_variables(cnf_formula)
 
     def from_textual_cnf_file(self, filepath: str) -> None:
-        """This method reads any of the available textual notations, 
+        """This method reads any of the available textual notations,
         but only one notation at the same time,
         so the .txt file should include only one of the possible notations in a single line.
         """
-        with open(filepath, 'r', encoding='utf-8') as file:
+        with open(filepath, "r", encoding="utf-8") as file:
             self.from_textual_cnf(file.readline())
 
-    def write_textual_cnf_file(self, filepath: str, 
-                               syntax: TextCNFNotation = TextCNFNotation.JAVA_SHORT) -> None:
-        """Write the textual CNF formula as a string in a file. 
+    def write_textual_cnf_file(
+        self, filepath: str, syntax: TextCNFNotation = TextCNFNotation.JAVA_SHORT
+    ) -> None:
+        """Write the textual CNF formula as a string in a file.
 
         Default syntax is TextCNFNotation.JAVA_SHORT: (A) & (!B | C) && ...
         """
         cnf_formula = self.get_textual_cnf_formula(syntax)
-        with open(filepath, 'w+', encoding='utf-8') as file:
+        with open(filepath, "w+", encoding="utf-8") as file:
             file.write(cnf_formula)
 
     def get_textual_cnf_notation(self) -> TextCNFNotation:
         """Return the notation used for the CNF formula."""
         if self._cnf_formula is None:
-            raise Exception("CNF Model not initialized. Use a `from_` method first.") 
+            raise FlamaException("CNF Model not initialized. Use a `from_` method first.")
         assert self._cnf_notation is not None
         return self._cnf_notation
 
-    def get_textual_cnf_formula(self, 
-                                syntax: TextCNFNotation = TextCNFNotation.JAVA_SHORT) -> str:
+    def get_textual_cnf_formula(
+        self, syntax: TextCNFNotation = TextCNFNotation.JAVA_SHORT
+    ) -> str:
         """Return the CNF formula in the specified notation syntax.
 
         Default syntax is TextCNFNotation.JAVA_SHORT: (A) & (!B | C) && ...
         """
         if self._cnf_formula is None:
-            raise Exception("CNF Model not initialized. Use a `from_` method first.") 
-        assert self._cnf_notation is not None 
+            raise FlamaException("CNF Model not initialized. Use a `from_` method first.")
+        assert self._cnf_notation is not None
 
         cnf_formula = self._cnf_formula
         cnf_notation = self._cnf_notation
 
         if syntax == cnf_notation:
             return cnf_formula
 
         # Translate AND operators
-        symbol_pattern = ' ' + cnf_notation.value[CNFLogicConnective.AND] + ' '
-        new_symbol = ' ' + syntax.value[CNFLogicConnective.AND] + ' '
+        symbol_pattern = " " + cnf_notation.value[CNFLogicConnective.AND] + " "
+        new_symbol = " " + syntax.value[CNFLogicConnective.AND] + " "
         cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
 
         # Translate OR operators
-        symbol_pattern = ' ' + cnf_notation.value[CNFLogicConnective.OR] + ' '
-        new_symbol = ' ' + syntax.value[CNFLogicConnective.OR] + ' '
+        symbol_pattern = " " + cnf_notation.value[CNFLogicConnective.OR] + " "
+        new_symbol = " " + syntax.value[CNFLogicConnective.OR] + " "
         cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
 
-        # Translate NOT operators 
+        # Translate NOT operators
         # This is more complex because the symbol may be part of a feature's name
         if cnf_notation == TextCNFNotation.TEXTUAL:
-            symbol_pattern = cnf_notation.value[CNFLogicConnective.NOT] + ' '
+            symbol_pattern = cnf_notation.value[CNFLogicConnective.NOT] + " "
             new_symbol = syntax.value[CNFLogicConnective.NOT]
             cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
         elif syntax == TextCNFNotation.TEXTUAL:
-            symbol_pattern = ' ' + cnf_notation.value[CNFLogicConnective.NOT]
-            new_symbol = ' ' + syntax.value[CNFLogicConnective.NOT] + ' '
+            symbol_pattern = " " + cnf_notation.value[CNFLogicConnective.NOT]
+            new_symbol = " " + syntax.value[CNFLogicConnective.NOT] + " "
             cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
 
-            symbol_pattern = '(' + cnf_notation.value[CNFLogicConnective.NOT]
-            new_symbol = '(' + syntax.value[CNFLogicConnective.NOT] + ' '
+            symbol_pattern = "(" + cnf_notation.value[CNFLogicConnective.NOT]
+            new_symbol = "(" + syntax.value[CNFLogicConnective.NOT] + " "
             cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
         else:
-            symbol_pattern = ' ' + cnf_notation.value[CNFLogicConnective.NOT]
-            new_symbol = ' ' + syntax.value[CNFLogicConnective.NOT]
+            symbol_pattern = " " + cnf_notation.value[CNFLogicConnective.NOT]
+            new_symbol = " " + syntax.value[CNFLogicConnective.NOT]
             cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
 
-            symbol_pattern = '(' + cnf_notation.value[CNFLogicConnective.NOT]
-            new_symbol = '(' + syntax.value[CNFLogicConnective.NOT]
+            symbol_pattern = "(" + cnf_notation.value[CNFLogicConnective.NOT]
+            new_symbol = "(" + syntax.value[CNFLogicConnective.NOT]
             cnf_formula = cnf_formula.replace(symbol_pattern, new_symbol)
         return cnf_formula
 
     def get_variables(self) -> list[str]:
         """Return the list of variables' names in the CNF formula."""
         if self._cnf_formula is None:
-            raise Exception("CNF Model not initialized. Use a `from_` method first.") 
+            raise FlamaException("CNF Model not initialized. Use a `from_` method first.")
         return self._variables
 
 
 def identify_notation(cnf_formula: str) -> TextCNFNotation:
     """Return the notation used by the given CNF formula.
 
     Default TextCNFNotation.JAVA.
     """
     notation = check_unary_connective(cnf_formula)
-    if notation is None or notation in (TextCNFNotation.JAVA, TextCNFNotation.JAVA_SHORT):
+    if notation is None or notation in (
+        TextCNFNotation.JAVA,
+        TextCNFNotation.JAVA_SHORT,
+    ):
         notation = check_binary_connective(cnf_formula)
     if notation is None:
-        notation = TextCNFNotation.JAVA_SHORT 
+        notation = TextCNFNotation.JAVA_SHORT
     return notation
 
 
 def check_unary_connective(cnf_formula: str) -> Optional[TextCNFNotation]:
     symbol = TextCNFNotation.LOGICAL.value[CNFLogicConnective.NOT]
-    if ' ' + symbol in cnf_formula or '(' + symbol in cnf_formula:
+    if " " + symbol in cnf_formula or "(" + symbol in cnf_formula:
         return TextCNFNotation.LOGICAL
 
     symbol = TextCNFNotation.SHORT.value[CNFLogicConnective.NOT]
-    if ' ' + symbol in cnf_formula or '(' + symbol in cnf_formula:
+    if " " + symbol in cnf_formula or "(" + symbol in cnf_formula:
         return TextCNFNotation.SHORT
 
     symbol = TextCNFNotation.TEXTUAL.value[CNFLogicConnective.NOT]
-    if ' ' + symbol + ' ' in cnf_formula or '(' + symbol + ' ' in cnf_formula:
+    if " " + symbol + " " in cnf_formula or "(" + symbol + " " in cnf_formula:
         return TextCNFNotation.TEXTUAL
 
     symbol = TextCNFNotation.JAVA.value[CNFLogicConnective.NOT]  # JAVA or JAVA_SHORT
-    if ' ' + symbol in cnf_formula or '(' + symbol in cnf_formula:
-        return TextCNFNotation.JAVA 
+    if " " + symbol in cnf_formula or "(" + symbol in cnf_formula:
+        return TextCNFNotation.JAVA
 
     return None
 
 
 def check_binary_connective(cnf_formula: str) -> Optional[TextCNFNotation]:
     for notation in TextCNFNotation:
         for connective in notation.value.keys():
             if connective != CNFLogicConnective.NOT:
                 symbol = notation.value[connective]
-                symbol_pattern = ' ' + symbol + ' '
+                symbol_pattern = " " + symbol + " "
                 if symbol_pattern in cnf_formula:
                     return notation
     return None
 
 
 def extract_variables(cnf_formula: str) -> list[str]:
     """Return the list of variables' names of the CNF formula."""
     variables = set()
     cnf_notation = identify_notation(cnf_formula)
 
     # Remove initial and final parenthesis
-    and_symbol_pattern = ' ' + cnf_notation.value[CNFLogicConnective.AND] + ' '
-    clauses = list(map(lambda c: c[1:len(c) - 1], cnf_formula.split(and_symbol_pattern)))
+    and_symbol_pattern = " " + cnf_notation.value[CNFLogicConnective.AND] + " "
+    clauses = list(
+        map(lambda c: c[1:len(c) - 1], cnf_formula.split(and_symbol_pattern))
+    )
 
     # Remove final parenthesis of last clause (because of the possible end of line: '\n')
-    if ')' in clauses[len(clauses) - 1]:
-        clauses[len(clauses) - 1] = clauses[len(clauses) - 1][:-1]  
+    if ")" in clauses[len(clauses) - 1]:
+        clauses[len(clauses) - 1] = clauses[len(clauses) - 1][:-1]
 
     for clause in clauses:
-        tokens = clause.split(' ')
-        tokens = list(filter(lambda t: t != cnf_notation.value[CNFLogicConnective.OR], tokens))
+        tokens = clause.split(" ")
+        tokens = list(
+            filter(lambda t: t != cnf_notation.value[CNFLogicConnective.OR], tokens)
+        )
         for feature in tokens:
             if feature == cnf_notation.value[CNFLogicConnective.NOT]:
                 continue
             if feature.startswith(cnf_notation.value[CNFLogicConnective.NOT]):
-                variables.add(feature.replace(cnf_notation.value[CNFLogicConnective.NOT], '', 1))
+                variables.add(
+                    feature.replace(cnf_notation.value[CNFLogicConnective.NOT], "", 1)
+                )
             else:
                 variables.add(feature)
     return list(variables)
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_feature_inclusion_probability.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_configurations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-from typing import Optional
-
-from flamapy.metamodels.configuration_metamodel.models.configuration import Configuration
+from typing import Optional, cast
 
+from flamapy.core.models import VariabilityModel
+from flamapy.core.operations import Configurations
+from flamapy.metamodels.configuration_metamodel.models import Configuration
 from flamapy.metamodels.bdd_metamodel.models import BDDModel
-from flamapy.metamodels.bdd_metamodel.operations.interfaces import FeatureInclusionProbability
-from flamapy.metamodels.bdd_metamodel.operations import BDDProducts
-
 
-class BDDFeatureInclusionProbability(FeatureInclusionProbability):
-    """The Feature Inclusion Probability (FIP) operation determines the probability
-    for a variable to be included in a valid solution.
 
-    This is a brute-force implementation that enumerates all solutions
-    for calculating the probabilities.
+class BDDConfigurations(Configurations):
+    """It computes all the solutions of a BDD model.
 
-    Ref.: [Heradio et al. 2019. Supporting the Statistical Analysis of Variability Models. SPLC.
-    (https://doi.org/10.1109/ICSE.2019.00091)]
+    It also supports the computation of all solutions from a partial configuration.
     """
 
-    def __init__(self, partial_configuration: Optional[Configuration] = None) -> None:
-        self.bdd_model = None
-        self.result: dict[str, float] = {}
-        self.partial_configuration = partial_configuration
-
-    def execute(self, model: BDDModel) -> 'BDDFeatureInclusionProbability':
-        self.bdd_model = model
-        self.result = feature_inclusion_probability(self.bdd_model, self.partial_configuration)
+    def __init__(self) -> None:
+        self._result: list[Configuration] = []
+        self._partial_configuration: Optional[Configuration] = None
+
+    def set_partial_configuration(self, partial_configuration: Configuration) -> None:
+        self._partial_configuration = partial_configuration
+
+    def execute(self, model: VariabilityModel) -> 'BDDConfigurations':
+        bdd_model = cast(BDDModel, model)
+        self._result = configurations(bdd_model, self._partial_configuration)
         return self
 
-    def get_result(self) -> dict[str, float]:
-        return self.result
+    def get_result(self) -> list[Configuration]:
+        return self._result
 
-    def feature_inclusion_probability(self) -> dict[str, float]:
-        return feature_inclusion_probability(self.bdd_model, self.partial_configuration)
+    def get_configurations(self) -> list[Configuration]:
+        return self.get_result()
 
 
-def feature_inclusion_probability(bdd_model: BDDModel,
-                                  config: Optional[Configuration] = None) -> dict[str, float]:
-    products = BDDProducts(config).execute(bdd_model).get_result()
-    n_products = len(products)
-    if n_products == 0:
-        return {feature: 0.0 for feature in bdd_model.variables}
-
-    prob = {}
-    for feature in bdd_model.variables:
-        prob[feature] = sum(feature in p.elements for p in products) / n_products
-    return prob
+def configurations(bdd_model: BDDModel,
+                   partial_config: Optional[Configuration] = None) -> list[Configuration]:
+    if partial_config is None:
+        u_func = bdd_model.root
+        care_vars = set(bdd_model.variables)
+        elements = {}
+    else:
+        values = dict(partial_config.elements.items())
+        u_func = bdd_model.bdd.let(values, bdd_model.root)
+        care_vars = set(bdd_model.variables) - set(values.keys())
+        elements = partial_config.elements
+
+    configs = []
+    for assignment in bdd_model.bdd.pick_iter(u_func, care_vars=care_vars):
+        features = {f: True for f in assignment.keys() if assignment[f]}
+        features = features | elements
+        configs.append(Configuration(features))
+    return configs
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_products.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_core_features.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,36 @@
-from typing import Optional
+from typing import Any, Optional, cast
 
-from flamapy.metamodels.configuration_metamodel.models.configuration import Configuration
-from flamapy.core.operations import Products
-from flamapy.metamodels.bdd_metamodel.models.bdd_model import BDDModel
+from flamapy.core.models import VariabilityModel
+from flamapy.metamodels.configuration_metamodel.models import Configuration
+from flamapy.core.operations import CoreFeatures
+from flamapy.metamodels.bdd_metamodel.models import BDDModel
+from flamapy.metamodels.bdd_metamodel.operations import BDDFeatureInclusionProbability
 
 
-class BDDProducts(Products):
-    """It computes all the solutions of a BDD model.
+class BDDCoreFeatures(CoreFeatures):
 
-    It also supports the computation of all solutions from a partial configuration.
-    """
+    def __init__(self) -> None:
+        self._result: list[Any] = []
+        self._partial_configuration: Optional[Configuration] = None
 
-    def __init__(self, partial_configuration: Optional[Configuration] = None) -> None:
-        self.result: list[Configuration] = []
-        self.bdd_model = None
-        self.partial_configuration = partial_configuration
+    def set_partial_configuration(self, partial_configuration: Optional[Configuration]) -> None:
+        self._partial_configuration = partial_configuration
 
-    def execute(self, model: BDDModel) -> 'BDDProducts':
-        self.bdd_model = model
-        self.result = products(self.bdd_model, self.partial_configuration)
+    def execute(self, model: VariabilityModel) -> 'BDDCoreFeatures':
+        bdd_model = cast(BDDModel, model)
+        self._result = core_features(bdd_model, self._partial_configuration)
         return self
 
-    def get_result(self) -> list[Configuration]:
-        return self.result
+    def get_result(self) -> list[Any]:
+        return self._result
 
-    def get_products(self) -> list[Configuration]:
-        return products(self.bdd_model, self.partial_configuration)
+    def get_core_features(self) -> list[Any]:
+        return self.get_result()
 
 
-def products(bdd_model: BDDModel,
-             partial_config: Optional[Configuration] = None) -> list[Configuration]:
-    if partial_config is None:
-        u_func = bdd_model.root
-        care_vars = bdd_model.variables
-        elements = {}
-    else:
-        values = dict(partial_config.elements.items())
-        u_func = bdd_model.bdd.let(values, bdd_model.root)
-        care_vars = set(bdd_model.variables) - values.keys()
-        elements = partial_config.elements
-
-    configs = []
-    for assignment in bdd_model.bdd.pick_iter(u_func, care_vars=care_vars):
-        features = {f: True for f in assignment.keys() if assignment[f]}
-        features = features | elements
-        configs.append(Configuration(features))
-    return configs
+def core_features(bdd_model: BDDModel,
+                  config: Optional[Configuration] = None) -> list[Any]:
+    fip_op = BDDFeatureInclusionProbability()
+    fip_op.set_partial_configuration(config)
+    probs = fip_op.execute(bdd_model).get_result()
+    return [feat for feat, prob, in probs.items() if prob >= 1.0]
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_products_number.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_configurations_number.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-from typing import Optional
+from typing import Optional, cast
 
-from flamapy.metamodels.configuration_metamodel.models.configuration import Configuration
-from flamapy.core.operations import ProductsNumber
-from flamapy.metamodels.bdd_metamodel.models.bdd_model import BDDModel
+from flamapy.core.models import VariabilityModel
+from flamapy.core.operations import ConfigurationsNumber
+from flamapy.metamodels.configuration_metamodel.models import Configuration
+from flamapy.metamodels.bdd_metamodel.models import BDDModel
 
 
-class BDDProductsNumber(ProductsNumber):
+class BDDConfigurationsNumber(ConfigurationsNumber):
     """It computes the number of solutions of the BDD model.
 
     It also supports counting the solutions from a given partial configuration.
     """
 
-    def __init__(self, partial_configuration: Optional[Configuration] = None) -> None:
-        self.result = 0
-        self.bdd_model = None
-        self.feature_model = None
-        self.partial_configuration = partial_configuration
-
-    def execute(self, model: BDDModel) -> 'BDDProductsNumber':
-        self.bdd_model = model
-        self.result = products_number(self.bdd_model, self.partial_configuration)
+    def __init__(self) -> None:
+        self._result: int = 0
+        self._partial_configuration: Optional[Configuration] = None
+
+    def set_partial_configuration(self, partial_configuration: Optional[Configuration]) -> None:
+        self._partial_configuration = partial_configuration
+
+    def execute(self, model: VariabilityModel) -> 'BDDConfigurationsNumber':
+        bdd_model = cast(BDDModel, model)
+        self._result = configurations_number(bdd_model, self._partial_configuration)
         return self
 
     def get_result(self) -> int:
-        return self.result
+        return self._result
 
-    def get_products_number(self) -> int:
-        return products_number(self.bdd_model, self.partial_configuration)
+    def get_configurations_number(self) -> int:
+        return self.get_result()
 
 
-def products_number(bdd_model: BDDModel,
-                    partial_configuration: Optional[Configuration] = None) -> int:
+def configurations_number(bdd_model: BDDModel,
+                          partial_configuration: Optional[Configuration] = None) -> int:
     if partial_configuration is None:
         u_func = bdd_model.root
         n_vars = len(bdd_model.variables)
     else:
         values = dict(partial_configuration.elements.items())
         u_func = bdd_model.bdd.let(values, bdd_model.root)
         n_vars = len(bdd_model.variables) - len(values)
-
-    return bdd_model.bdd.count(u_func, nvars=n_vars)
+    return int(bdd_model.bdd.count(u_func, nvars=n_vars))
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/bdd_sampling.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/bdd_sampling.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
-from typing import Optional
+from typing import Optional, cast
 
-from flamapy.metamodels.configuration_metamodel.models.configuration import Configuration
+from flamapy.core.models import VariabilityModel
+from flamapy.core.exceptions import FlamaException
 from flamapy.core.operations import Sampling
-
+from flamapy.metamodels.configuration_metamodel.models import Configuration
 from flamapy.metamodels.bdd_metamodel.models import BDDModel
-from flamapy.metamodels.bdd_metamodel.operations import BDDProductsNumber
 
 
 class BDDSampling(Sampling):
     """Uniform Random Sampling (URS) using a Binary Decision Diagram (BDD).
 
     This is an adaptation of
     [Heradio et al. 2021.
@@ -17,51 +17,60 @@
     Empirical Software Engineering]
     which relies on counting-based sampling inspired in the original Knuth algorithm.
 
     This implementation supports samples with and without replacement,
     as well as samples from a given partial configuration.
     """
 
-    def __init__(self, size: int, with_replacement: bool = False,
-                 partial_configuration: Optional[Configuration] = None) -> None:
-        self.result: list[Configuration] = []
-        self.bdd_model = None
-        self.size = size
-        self.with_replacement = with_replacement
-        self.partial_configuration = partial_configuration
-
-    def execute(self, model: BDDModel) -> 'BDDSampling':
-        self.bdd_model = model
-        self.result = sample(self.bdd_model, self.size, self.with_replacement,
-                             self.partial_configuration)
-        return self
+    def __init__(self) -> None:
+        self._result: list[Configuration] = []
+        self._sample_size: int = 0
+        self._with_replacement: bool = False
+        self._partial_configuration: Optional[Configuration] = None
+
+    def set_sample_size(self, sample_size: int) -> None:
+        if sample_size < 0:
+            raise FlamaException(f'Sample size {sample_size} cannot be negative.')
+        self._sample_size = sample_size
+
+    def set_with_replacement(self, with_replacement: bool) -> None:
+        self._with_replacement = with_replacement
+
+    def set_partial_configuration(self, partial_configuration: Configuration) -> None:
+        self._partial_configuration = partial_configuration
 
     def get_result(self) -> list[Configuration]:
-        return self.result
+        return self._result
 
-    def sample(self, size: int, with_replacement: bool = False,
-               partial_configuration: Optional[Configuration] = None) -> list[Configuration]:
-        return sample(self.bdd_model, size, with_replacement, partial_configuration)
+    def get_sample(self) -> list[Configuration]:
+        return self.get_result()
 
+    def execute(self, model: VariabilityModel) -> 'BDDSampling':
+        bdd_model = cast(BDDModel, model)
+        self._result = sample(bdd_model, 
+                              self._sample_size, 
+                              self._with_replacement, 
+                              self._partial_configuration)
+        return self
 
-def sample(bdd_model: BDDModel, size: int, with_replacement: bool = False,
-           partial_configuration: Optional[Configuration] = None) -> list[Configuration]:
-    nof_configs = BDDProductsNumber(partial_configuration).execute(bdd_model).get_result()
-    if size < 0 or (size > nof_configs and not with_replacement):
-        raise ValueError('Sample larger than population or is negative.')
 
+def sample(model: BDDModel, 
+           sample_size: int, 
+           with_replacement: bool,
+           partial_configuration: Optional[Configuration]
+           ) -> list[Configuration]:
     configurations = []
-    for _ in range(size):
-        config = random_configuration(bdd_model, partial_configuration)
+    for _ in range(sample_size):
+        config = random_configuration(model, partial_configuration)
         configurations.append(config)
 
     if not with_replacement:
         set_configurations = set(configurations)
-        while len(set_configurations) < size:
-            config = random_configuration(bdd_model, partial_configuration)
+        while len(set_configurations) < sample_size:
+            config = random_configuration(model, partial_configuration)
             set_configurations.add(config)
 
     return list(set_configurations)
 
 
 def random_configuration(bdd_model: BDDModel,
                          p_config: Optional[Configuration] = None) -> Configuration:
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/operations/interfaces/feature_inclusion_probability.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/operations/interfaces/feature_inclusion_probability.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     provides a clear picture of the products' homogeneity (i.e., how much does one product 
     differ from the others).
     The product's homogeneity is one the three core metrics that characterize 
     the complexity of a SPL.
     The other two core metrics are the number of features the SPL manages, 
     and the number of valid product that can be derived.
 
-    Ref.: [Heradio et al. 2019. Supporting the Statistical Analysis of Variability Models. SPLC. 
+    Ref.: [Heradio et al. 2019. Supporting the Statistical Analysis of Variability Models. 
     (https://doi.org/10.1109/ICSE.2019.00091)]
     """
 
     @abstractmethod
     def __init__(self) -> None:
         pass
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/transformations/fm_to_bdd.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/fm_to_bdd_pl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,136 @@
+import re
 import itertools
+from typing import Optional
 
+from flamapy.core.models.ast import ASTOperation
 from flamapy.core.transformations import ModelToModel
-from flamapy.metamodels.fm_metamodel.models import (
-    FeatureModel,
-    Constraint,
-    Feature,
-    Relation,
-)
+from flamapy.metamodels.fm_metamodel.models import FeatureModel, Relation, Constraint
 from flamapy.metamodels.bdd_metamodel.models import BDDModel
 
 
 class FmToBDD(ModelToModel):
+
     @staticmethod
     def get_source_extension() -> str:
-        return 'fm'
+        return "fm"
 
     @staticmethod
     def get_destination_extension() -> str:
-        return 'bdd'
+        return "bdd"
 
     def __init__(self, source_model: FeatureModel) -> None:
         self.source_model = source_model
-        self.counter = 1
-        self.destination_model = BDDModel()
-        self.variables: dict[str, int] = {}
-        self.features: dict[int, str] = {}
-        self.clauses: list[list[int]] = []
-
-    def _get_variable(self, name: str) -> int:
-        variable = self.variables.get(name)
-        if variable is None:
-            raise ValueError("the parent variable wasn't found")
-        return variable
-
-    def add_feature(self, feature: Feature) -> None:
-        if feature.name not in self.variables:
-            self.variables[feature.name] = self.counter
-            self.features[self.counter] = feature.name
-            self.counter += 1
-
-    def add_root(self, feature: Feature) -> None:
-        self.clauses.append([self._get_variable(feature.name)])
-
-    def add_relation(self, relation: Relation) -> None:  # noqa: MC0001
-        # pylint: disable=too-many-nested-blocks
-        var_parent = self._get_variable(relation.parent.name)
-        # TODO: fix too many nested blocks
-        if relation.is_mandatory():
-            var_child = self._get_variable(relation.children[0].name)
-            self.clauses.append([-1 * var_parent, var_child])
-            self.clauses.append([-1 * var_child, var_parent])
-
-        elif relation.is_optional():
-            self.clauses.append([
-                -1 * self._get_variable(relation.children[0].name), var_parent
-            ])
-
-        elif relation.is_or():  # this is a 1 to n relatinship with multiple childs
-            # add the first cnf child1 or child2 or ... or childN or no parent)
-
-            # first elem of the constraint
-            alt_cnf = [-1 * var_parent]
-            for child in relation.children:
-                alt_cnf.append(self._get_variable(child.name))
-            self.clauses.append(alt_cnf)
-
-            for child in relation.children:
-                self.clauses.append([-1 * self._get_variable(child.name), var_parent])
-
-        elif relation.is_alternative():
-            # this is a 1 to 1 relatinship with multiple childs
-            # add the first cnf child1 or child2 or ... or childN or no parent)
-
-            # first elem of the constraint
-            alt_cnf = [-1 * var_parent]
-            for child in relation.children:
-                alt_cnf.append(self._get_variable(child.name))
-            self.clauses.append(alt_cnf)
-
-            for i, _ in enumerate(relation.children):
-                var_child_i = self._get_variable(relation.children[i].name)
-                for j in range(i + 1, len(relation.children)):
-                    if i != j:
-                        self.clauses.append([
-                            -1 * var_child_i, -1 * self._get_variable(relation.children[j].name)
-                        ])
-                self.clauses.append([-1 * var_child_i, var_parent])
-
-        else:
-            # This is a _min to _max relationship
-            _min = relation.card_min
-            _max = relation.card_max
-            for val in range(len(relation.children) + 1):
-                if val < _min or val > _max:
-                    #combinations of val elements
-                    for combination in itertools.combinations(relation.children, val):
-                        cnf = [-1 * self._get_variable(relation.parent.name)]
-                        for feat in relation.children:
-                            if feat in combination:
-                                cnf.append(-1 * self._get_variable(feat.name))
-                            else:
-                                cnf.append(self._get_variable(feat.name))
-                        self.clauses.append(cnf)
-
-            #there is a special case when coping with the upper part of the thru table
-            #In the case of allowing 0 childs, you cannot exclude the option  in that
-            # no feature in this relation is activated
-            for val in range(1, len(relation.children) + 1):
-                for combination in itertools.combinations(relation.children, val):
-                    cnf = [self._get_variable(relation.parent.name)]
-                    for feat in relation.children:
-                        if feat in combination:
-                            cnf.append(-1 * self._get_variable(feat.name))
-                        else:
-                            cnf.append(self._get_variable(feat.name))
-                    self.clauses.append(cnf)
-
-    def add_constraint(self, ctc: Constraint) -> None:
-        clauses = ctc.ast.get_clauses()
-        for clause in clauses:
-            cls = []
-            for term in clause:
-                if term.startswith('-'):
-                    var_term = -1 * self._get_variable(term[1:])
-                else:
-                    var_term = self._get_variable(term)
-                cls.append(var_term)
-            self.clauses.append(cls)
+        self.destination_model: Optional[BDDModel] = None
 
     def transform(self) -> BDDModel:
-        for feature in self.source_model.get_features():
-            self.add_feature(feature)
-
-        self.add_root(self.source_model.root)
-
-        for relation in self.source_model.get_relations():
-            self.add_relation(relation)
-
-        for constraint in self.source_model.get_constraints():
-            self.add_constraint(constraint)
-
-        # Transform clauses to textual CNF notation required by the BDD
-        not_connective = BDDModel.NOT
-        or_connective = ' ' + BDDModel.OR + ' '
-        and_connective = ' ' + BDDModel.AND + ' '
-        cnf_list = []
-        for clause in self.clauses:
-            cnf_list.append('(' + or_connective.join(list(map(lambda l:
-                            not_connective + self.features[abs(l)] if l < 0 else
-                            self.features[abs(l)], clause))) + ')')
+        formula, variables = traverse_feature_tree(self.source_model)
+        self.destination_model = BDDModel.from_logic_formula(formula, variables)
+        return self.destination_model
 
-        cnf_formula = and_connective.join(cnf_list)
-        self.destination_model.from_textual_cnf(cnf_formula, list(self.variables.keys()))
 
-        return self.destination_model
+def traverse_feature_tree(feature_model: FeatureModel) -> tuple[str, list[str]]:
+    """Traverse the feature tree from the root and return the propositional formula and 
+    the list of variables (features's names).
+    """
+    if feature_model is None or feature_model.root is None:
+        return ('', [])
+    formula = [feature_model.root.name]  # The root is always present
+    variables = []
+    for feature in feature_model.get_features():
+        variables.append(feature.name)
+        for relation in feature.get_relations():
+            formula.append(get_relation_formula(relation))
+    for constraint in feature_model.get_constraints():
+        formula.append(get_constraint_formula(constraint))
+    propositional_formula = ' & '.join(f'({f})' for f in formula)
+    return (propositional_formula, variables)
+
+
+def get_relation_formula(relation: Relation) -> str:
+    result = ''
+    if relation.is_mandatory():
+        result = get_mandatory_formula(relation)
+    elif relation.is_optional():
+        result = get_optional_formula(relation)
+    elif relation.is_or():
+        result = get_or_formula(relation)
+    elif relation.is_alternative():
+        result = get_alternative_formula(relation)
+    elif relation.is_mutex():
+        result = get_mutex_formula(relation)
+    elif relation.is_cardinal():
+        result = get_cardinality_formula(relation)
+    return result
+
+
+def get_mandatory_formula(relation: Relation) -> str:
+    return f'{relation.parent.name} <=> {relation.children[0].name}'
+
+
+def get_optional_formula(relation: Relation) -> str:
+    return f'{relation.children[0].name} => {relation.parent.name}'
+
+
+def get_or_formula(relation: Relation) -> str:
+    return f'{relation.parent.name} <=> ({" | ".join(child.name for child in relation.children)})'
+
+
+def get_alternative_formula(relation: Relation) -> str:
+    formula = []
+    for child in relation.children:
+        children_negatives = set(relation.children) - {child}
+        formula.append(f'{child.name} <=> '
+                       f'({" & ".join("!" + f.name for f in children_negatives)} '
+                       f'& {relation.parent.name})')
+    return " & ".join(f'({f})' for f in formula)
+
+
+def get_mutex_formula(relation: Relation) -> str:
+    formula = []
+    for child in relation.children:
+        children_negatives = set(relation.children) - {child}
+        formula.append(f'{child.name} <=> '
+                       f'({" & ".join("!" + f.name for f in children_negatives)} '
+                       f'& {relation.parent.name})')
+    formula_str = " & ".join(f'({f})' for f in formula)
+    return f'({relation.parent.name} <=> ' \
+           f'!({" | ".join(child.name for child in relation.children)})) | ({formula_str})'
+
+
+def get_cardinality_formula(relation: Relation) -> str:
+    children = {child.name for child in relation.children}
+    or_ctc = []
+    for k in range(relation.card_min, relation.card_max + 1):
+        combi_k = list(itertools.combinations(children, k))
+        for positives in combi_k:
+            negatives = children - set(positives)
+            positives_and_ctc = f'{" & ".join(positives)}'
+            negatives_and_ctc = f'{" & ".join("!" + f for f in negatives)}'
+            if positives_and_ctc and negatives_and_ctc:
+                and_ctc = f'{positives_and_ctc} & {negatives_and_ctc}'
+            else:
+                and_ctc = f'{positives_and_ctc}{negatives_and_ctc}'
+            or_ctc.append(and_ctc) 
+    formula_or_ctc = f'{" | ".join(or_ctc)}'
+    return f'{relation.parent.name} <=> {formula_or_ctc}'
+
+
+def get_constraint_formula(ctc: Constraint) -> str:
+    return str(
+        re.sub(rf"\b{ASTOperation.EXCLUDES.value}\b",
+               f'{BDDModel.LogicConnective.IMPLIES.value} {BDDModel.LogicConnective.NOT.value}',
+               re.sub(rf"\b{ASTOperation.REQUIRES.value}\b",
+                      BDDModel.LogicConnective.IMPLIES.value,
+                      re.sub(rf"\b{ASTOperation.EQUIVALENCE.value}\b", 
+                             BDDModel.LogicConnective.EQUIVALENCE.value,
+                             re.sub(rf"\b{ASTOperation.IMPLIES.value}\b",
+                                    BDDModel.LogicConnective.IMPLIES.value,
+                                    re.sub(rf"\b{ASTOperation.OR.value}\b",
+                                           BDDModel.LogicConnective.OR.value,
+                                           re.sub(rf"\b{ASTOperation.AND.value}\b",
+                                                  BDDModel.LogicConnective.AND.value,
+                                                  re.sub(rf"\b{ASTOperation.NOT.value}\b",
+                                                         BDDModel.LogicConnective.NOT.value,
+                                                         re.sub(rf"\b{ASTOperation.XOR.value}\b",
+                                                                BDDModel.LogicConnective.XOR.value,
+                                                                ctc.ast.pretty_str())))))))))
```

### Comparing `flamapy-bdd-1.6.0/flamapy/metamodels/bdd_metamodel/transformations/sat_to_bdd.py` & `flamapy-bdd-2.0.0.dev1/flamapy/metamodels/bdd_metamodel/transformations/sat_to_bdd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-from flamapy.core.transformations import ModelToModel
+from typing import Optional
 
+from flamapy.core.transformations import ModelToModel
 from flamapy.metamodels.bdd_metamodel.models import BDDModel
 from flamapy.metamodels.pysat_metamodel.models import PySATModel
 
 
 class SATToBDD(ModelToModel):
 
     @staticmethod
     def get_source_extension() -> str:
-        return 'pysat'
+        return "pysat"
 
     @staticmethod
     def get_destination_extension() -> str:
-        return 'bdd'
+        return "bdd"
 
     def __init__(self, source_model: PySATModel) -> None:
         self.source_model = source_model
-        self.destination_model = BDDModel()
+        self.destination_model: Optional[BDDModel] = None
 
     def transform(self) -> BDDModel:
         # Transform clauses to textual CNF notation required by the BDD
         not_connective = BDDModel.NOT
-        or_connective = ' ' + BDDModel.OR + ' '
-        and_connective = ' ' + BDDModel.AND + ' '
+        or_connective = " " + BDDModel.OR + " "
+        and_connective = " " + BDDModel.AND + " "
         cnf_list = []
         for clause in self.source_model.get_all_clauses().clauses:
-            cnf_list.append('(' + or_connective.join(list(map(lambda l:
-                            not_connective + self.source_model.features[abs(l)] if l < 0 else
-                            self.source_model.features[abs(l)], clause))) + ')')
-
+            cnf_list.append(
+                "("
+                + or_connective.join(
+                    list(
+                        map(
+                            lambda elem: not_connective
+                            + self.source_model.features[abs(elem)]
+                            if elem < 0
+                            else self.source_model.features[abs(elem)],
+                            clause,
+                        )
+                    )
+                )
+                + ")"
+            )
         cnf_formula = and_connective.join(cnf_list)
-        self.destination_model.from_textual_cnf(cnf_formula, list(self.source_model.variables.keys()))
-
+        bdd_model = BDDModel.from_textual_cnf(cnf_formula, 
+                                              list(self.source_model.variables.keys()))
+        self.destination_model = bdd_model
         return self.destination_model
```

### Comparing `flamapy-bdd-1.6.0/flamapy_bdd.egg-info/PKG-INFO` & `flamapy-bdd-2.0.0.dev1/flamapy_bdd.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-bdd
-Version: 1.6.0
+Version: 2.0.0.dev1
 Summary: bdd-plugin for the automated analysis of feature models
 Home-page: https://github.com/flamapy/bdd_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,17 @@
 Provides-Extra: dev
 
 # BDD plugin for flamapy
 - [BDD plugin for flamapy](#bdd-plugin-for-flamapy)
   - [Description](#description)
   - [Requirements and Installation](#requirements-and-installation)
   - [Functionality and usage](#functionality-and-usage)
-    - [Load a feature model and create the BDD](#load-a-feature-model-and-create-the-bdd)
+    - [Load a feature model in UVL and create the BDD](#load-a-feature-model-in-uvl-and-create-the-bdd)
     - [Save the BDD in a file](#save-the-bdd-in-a-file)
+    - [Load the BDD from a file](#load-the-bdd-from-a-file)
     - [Analysis operations](#analysis-operations)
   - [Contributing to the BDD plugin](#contributing-to-the-bdd-plugin)
 
 
 ## Description
 This plugin supports Binary Decision Diagrams (BDDs) representations for feature models.
 
@@ -60,136 +61,138 @@
 
 ## Functionality and usage
 The executable script [test_bdd_metamodel.py](https://github.com/flamapy/bdd_metamodel/blob/master/tests/test_bdd_metamodel.py) serves as an entry point to show the plugin in action.
 
 The following functionality is provided:
 
 
-### Load a feature model and create the BDD
+### Load a feature model in UVL and create the BDD
 ```python
-from flamapy.metamodels.fm_metamodel.transformations.featureide_reader import FeatureIDEReader
-from flamapy.metamodels.bdd_metamodel.transformations.fm_to_bdd import FmToBDD
+from flamapy.metamodels.fm_metamodel.transformations import UVLReader
+from flamapy.metamodels.bdd_metamodel.transformations import FmToBDD
 
-# Load the feature model from FeatureIDE
-feature_model = FeatureIDEReader('input_fms/featureide_models/pizzas.xml').transform()
+# Load the feature model from UVL
+feature_model = UVLReader('models/uvl_models/pizzas.uvl').transform()
 # Create the BDD from the feature model
 bdd_model = FmToBDD(feature_model).transform()
 ```
 
 
 ### Save the BDD in a file
 ```python
-from flamapy.metamodels.bdd_metamodel.transformations.bdd_writer import BDDWriter, BDDDumpFormat
+from flamapy.metamodels.bdd_metamodel.transformations import PNGWriter, DDDMPv3Writer
 # Save the BDD as an image in PNG
-BDDWriter(path='my_bdd.png',
-          source_model=bdd_model,
-          roots=[bdd_model.root],
-          output_format=BDDDumpFormat.PNG).transform()
+PNGWriter(path='my_bdd.png', bdd_model).transform()
+# Save the BDD in a .dddmp file
+DDDMPv3Writer(f'my_bdd.dddmp', bdd_model).transform()
 ```
-Formats supported: DDDMP_V3 ('dddmp'), DDDMP_V2 ('dddmp2'), PDF ('pdf'), PNG ('png'), SVG ('svg').
+Writers available: DDDMPv3 ('dddmp'), DDDMPv2 ('dddmp'), JSON ('json'), Pickle ('p'), PDF ('pdf'), PNG ('png'), SVG ('svg').
 
+### Load the BDD from a file
+```python
+from flamapy.metamodels.bdd_metamodel.transformations import JSONReader
+# Load the BDD from a .json file
+bdd_model = JSONReader(path='path/to/my_bdd.json').transform()
+```
+Readers available: JSON ('json'), DDDMP ('dddmp'), Pickle ('p').
+
+*NOTE:* DDDMP and Pickle readers are not fully supported yet.
 
 ### Analysis operations
 
-- Products number
+- Satisfiable
 
-    Return the number of products (configurations):
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProductsNumber
-    nof_products = BDDProductsNumber().execute(bdd_model).get_result()
-    print(f'#Products: {nof_products}')
-    ```
-    or alternatively:
+    Return whether the model is satisfiable (valid):
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import products_number
-    nof_products = products_number(bdd_model)
-    print(f'#Products: {nof_products}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDSatisfiable
+    satisfiable = BDDSatisfiable().execute(bdd_model).get_result()
+    print(f'Satisfiable? (valid?): {satisfiable}')
     ```
 
-- Products
+- Configurations number
 
-    Return the list of products (configurations):
+    Return the number of configurations:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProducts
-    list_products = BDDProducts().execute(bdd_model).get_result()
-    for i, prod in enumerate(list_products):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDConfigurationsNumber
+    n_configs = BDDConfigurationsNumber().execute(bdd_model).get_result()
+    print(f'#Configurations: {n_configs}')
     ```
-    or alternatively:
+
+- Configurations
+
+    Enumerate the configurations of the model:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import products
-    nof_products = products(bdd_model)
-    for i, prod in enumerate(list_products):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDConfigurations
+    configurations = BDDConfigurations().execute(bdd_model).get_result()
+    for i, config in enumerate(configurations, 1):
+        print(f'Config {i}: {[feat for feat in config.elements if config.elements[feat]]}')
     ```
 
 - Sampling
 
-    Return a sample of the given size of uniform random products (configurations) with or without replacement:
+    Return a sample of the given size of uniform random configurations with or without replacement:
     ```python
     from flamapy.metamodels.bdd_metamodel.operations import BDDSampling
-    list_sample = BDDSampling(size=5, with_replacement=False).execute(bdd_model).get_result()
-    for i, prod in enumerate(list_sample):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
-    ```
-    or alternatively:
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import sample
-    list_sample = sample(bdd_model, size=5, with_replacement=False)
-    for i, prod in enumerate(list_sample):
-        print(f'Product {i}: {[feat for feat in prod.elements if prod.elements[feat]]}')
+    sampling_op = BDDSampling()
+    sampling_op.set_sample_size(5)
+    sampling_op.set_with_replacement(False)  # Default False
+    sample = sampling_op.execute(bdd_model).get_result()
+    for i, config in enumerate(sample, 1):
+        print(f'Config {i}: {[feat for feat in config.elements if config.elements[feat]]}')
     ```
 
 - Product Distribution
 
-    Return the number of products having a given number of features:
-    ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDProductDistributionBF
-    dist = BDDProductDistributionBF().execute(bdd_model).get_result()
-    print(f'Product Distribution: {dist}')
-    ```
-    or alternatively:
+    Return the number of products (configurations) having a given number of features:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import product_distribution
-    dist = product_distribution(bdd_model)
+    from flamapy.metamodels.bdd_metamodel.operations import BDDProductDistribution
+    dist = BDDProductDistribution().execute(bdd_model).get_result()
     print(f'Product Distribution: {dist}')
     ```
 
 - Feature Inclusion Probability
 
-    Return the probability for a feature to be included in a valid product:
+    Return the probability for a feature to be included in a valid configuration:
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import BDDFeatureInclusionProbabilityBF
-    prob = BDDFeatureInclusionProbabilityBF().execute(bdd_model).get_result()
+    from flamapy.metamodels.bdd_metamodel.operations import BDDFeatureInclusionProbability
+    prob = BDDFeatureInclusionProbability().execute(bdd_model).get_result()
     for feat in prob.keys():
         print(f'{feat}: {prob[feat]}')
     ```
-    or alternatively:
+
+- Core features
+
+    Return the core features (those features that are present in all the configurations):
     ```python
-    from flamapy.metamodels.bdd_metamodel.operations import feature_inclusion_probability
-    prob = feature_inclusion_probability(bdd_model)
-    for feat in prob.keys():
-        print(f'{feat}: {prob[feat]}')
+    from flamapy.metamodels.bdd_metamodel.operations import BDDCoreFeatures
+    core_features = BDDCoreFeatures().execute(bdd_model).get_result()
+    print(f'Core features: {core_features}')
+    ```
+
+- Dead features
+
+    Return the dead features (those features that are not present in any configuration):
+    ```python
+    from flamapy.metamodels.bdd_metamodel.operations import BDDDeadFeatures
+    dead_features = BDDDeadFeatures().execute(bdd_model).get_result()
+    print(f'Dead features: {dead_features}')
     ```
 
-All analysis operations support also a partial configuration as an additional argument, so the operation will return the result taking into account the given partial configuration. For example:
+Most analysis operations support also a partial configuration as an additional argument, so the operation will return the result taking into account the given partial configuration. For example:
 
 ```python
 from flamapy.core.models import Configuration
 # Create a partial configuration
 elements = {'Pizza': True, 'Big': True}
 partial_config = Configuration(elements)
-# Calculate the number of products from the partial configuration
-nof_products = BDDProductsNumber(partial_config).execute(bdd_model).get_result()
-print(f'#Products: {nof_products}')
-```
-or alternatively:
-```python
-nof_products = products(bdd_model, partial_config)
-print(f'#Products: {nof_products}')
+# Calculate the number of configuration from the partial configuration
+configs_number_op = BDDConfigurationsNumber()
+configs_number_op.set_partial_configuration(partial_config)
+n_configs = configs_number_op.execute(bdd_model).get_result()
+print(f'#Configurations: {n_configs}')
 ```
 
 
 ## Contributing to the BDD plugin
 To contribute in the development of this plugin:
 
 1. Fork the repository into your GitHub account.
```

### Comparing `flamapy-bdd-1.6.0/setup.py` & `flamapy-bdd-2.0.0.dev1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-bdd",
-    version="1.6.0",
+    version="2.0.0.dev1",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="bdd-plugin for the automated analysis of feature models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/bdd_metamodel",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
-        'flamapy~=1.6.0.dev0',
-        'flamapy-fm~=1.6.0.dev0',
-        'dd>=0.5.6',
-        'graphviz~=0.20',
+        'flamapy-fw~=2.0.0.dev1',
+        'flamapy-fm~=2.0.0.dev1',
+        'dd>=0.5.7',
+        'graphviz>=0.20',
     ],
     extras_require={
         'dev': [
             'pytest',
             'pytest-mock',
             'prospector',
             'mypy',
             'coverage',
         ]
     },
     dependency_links=[
-        'flamapy~=1.6.0.dev0',
+        'flamapy~=2.0.0.dev1',
     ]
 )
```

