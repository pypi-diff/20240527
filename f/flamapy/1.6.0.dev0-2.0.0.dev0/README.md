# Comparing `tmp/flamapy-1.6.0.dev0.tar.gz` & `tmp/flamapy-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-1.6.0.dev0.tar", last modified: Mon Jan  8 10:17:48 2024, max compression
+gzip compressed data, was "flamapy-2.0.0.dev0.tar", last modified: Mon May 27 15:40:12 2024, max compression
```

## Comparing `flamapy-1.6.0.dev0.tar` & `flamapy-2.0.0.dev0.tar`

### file list

```diff
@@ -1,65 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.405334 flamapy-1.6.0.dev0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.405334 flamapy-1.6.0.dev0/flamapy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.405334 flamapy-1.6.0.dev0/flamapy/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.405334 flamapy-1.6.0.dev0/flamapy/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/models/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/models/variability_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/flamapy/core/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/abstract_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/atomic_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/average_branching_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/commonality.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/core_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/count_leafs.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/dead_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/error_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/error_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/estimated_products_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/metrics_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/products.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/products_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/valid.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/valid_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/valid_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/operations/variability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/flamapy/core/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/transformations/abstract_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/transformations/model_to_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/transformations/model_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/transformations/text_to_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/flamapy/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/endpoint/diverso_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.405334 flamapy-1.6.0.dev0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/models/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:17:48.405334 flamapy-1.6.0.dev0/flamapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-08 10:17:48.000000 flamapy-1.6.0.dev0/flamapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-01-08 10:17:48.000000 flamapy-1.6.0.dev0/flamapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 10:17:48.000000 flamapy-1.6.0.dev0/flamapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-08 10:17:48.000000 flamapy-1.6.0.dev0/flamapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-08 10:17:48.000000 flamapy-1.6.0.dev0/flamapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-08 10:17:48.000000 flamapy-1.6.0.dev0/flamapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 10:17:48.409334 flamapy-1.6.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-08 10:17:38.000000 flamapy-1.6.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:12.235390 flamapy-2.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-27 15:40:12.235390 flamapy-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-27 15:40:00.000000 flamapy-2.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:12.235390 flamapy-2.0.0.dev0/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:12.235390 flamapy-2.0.0.dev0/flamapy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:00.000000 flamapy-2.0.0.dev0/flamapy/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:12.235390 flamapy-2.0.0.dev0/flamapy/interfaces/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    13930 2024-05-27 15:40:00.000000 flamapy-2.0.0.dev0/flamapy/interfaces/python/FLAMAFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:00.000000 flamapy-2.0.0.dev0/flamapy/interfaces/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:12.235390 flamapy-2.0.0.dev0/flamapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-27 15:40:12.000000 flamapy-2.0.0.dev0/flamapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-27 15:40:12.000000 flamapy-2.0.0.dev0/flamapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:40:12.000000 flamapy-2.0.0.dev0/flamapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-27 15:40:12.000000 flamapy-2.0.0.dev0/flamapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 15:40:12.000000 flamapy-2.0.0.dev0/flamapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 15:40:12.000000 flamapy-2.0.0.dev0/flamapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:40:12.235390 flamapy-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-27 15:40:00.000000 flamapy-2.0.0.dev0/setup.py
```

### Comparing `flamapy-1.6.0.dev0/setup.py` & `flamapy-2.0.0.dev0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,39 +3,42 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy",
-    version="1.6.0.dev0",
+    version="2.0.0.dev0",
     author="Flamapy",
     author_email="flamapy@us.es",
-    description="Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.",
+    description="Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/flamapy/core",
+    url="https://github.com/flamapy/flamapy-feature-model",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
-        'hug>=2.6.1',
+        "wheel",
+        "flamapy-fw~=2.0.0.dev0",
+        "flamapy-fm~=2.0.0.dev0",
+        "flamapy-sat~=2.0.0.dev0",    
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
     entry_points={
         'console_scripts': [
-            'flamapy-admin = flamapy.commands:flamapy_admin',
+            'flamapy-fm-cli = flamapy.interfaces.command_line:flama_fm',
         ],
     },
 )
```

