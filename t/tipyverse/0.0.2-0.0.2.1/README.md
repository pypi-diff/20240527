# Comparing `tmp/tipyverse-0.0.2.tar.gz` & `tmp/tipyverse-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipyverse-0.0.2.tar", last modified: Mon May 27 06:33:26 2024, max compression
+gzip compressed data, was "tipyverse-0.0.2.1.tar", last modified: Mon May 27 06:45:11 2024, max compression
```

## Comparing `tipyverse-0.0.2.tar` & `tipyverse-0.0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.956269 tipyverse-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 06:33:22.000000 tipyverse-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 06:33:26.956269 tipyverse-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 06:33:22.000000 tipyverse-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-27 06:33:22.000000 tipyverse-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:33:26.956269 tipyverse-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.952269 tipyverse-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.952269 tipyverse-0.0.2/src/tipyverse/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_tidy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.956269 tipyverse-0.0.2/src/tipyverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.956269 tipyverse-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_tidy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:11.391409 tipyverse-0.0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-27 06:45:11.391409 tipyverse-0.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:45:11.391409 tipyverse-0.0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:11.387409 tipyverse-0.0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:11.387409 tipyverse-0.0.2.1/src/tipyverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/data_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/data_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/src/tipyverse/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:11.391409 tipyverse-0.0.2.1/src/tipyverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-27 06:45:11.000000 tipyverse-0.0.2.1/src/tipyverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 06:45:11.000000 tipyverse-0.0.2.1/src/tipyverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:45:11.000000 tipyverse-0.0.2.1/src/tipyverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-27 06:45:11.000000 tipyverse-0.0.2.1/src/tipyverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 06:45:11.000000 tipyverse-0.0.2.1/src/tipyverse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:11.391409 tipyverse-0.0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/tests/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/tests/test_data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/tests/test_data_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/tests/test_data_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:45:04.000000 tipyverse-0.0.2.1/tests/test_utilities.py
```

### Comparing `tipyverse-0.0.2/LICENSE` & `tipyverse-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tipyverse-0.0.2/PKG-INFO` & `tipyverse-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipyverse
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A package to install Python equivalents of R tipyverse packages
 Author-email: Sebastian Dunn <sebastiandunn@sdmdigital.co>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Dunn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tipyverse-0.0.2/pyproject.toml` & `tipyverse-0.0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tipyverse"
-version = "0.0.2"
+version = "0.0.2.1"
 description = "A package to install Python equivalents of R tipyverse packages"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Sebastian Dunn", email = "sebastiandunn@sdmdigital.co" },
 ]
 classifiers = [
```

### Comparing `tipyverse-0.0.2/src/tipyverse/data_manipulation.py` & `tipyverse-0.0.2.1/src/tipyverse/data_manipulation.py`

 * *Files identical despite different names*

### Comparing `tipyverse-0.0.2/src/tipyverse.egg-info/PKG-INFO` & `tipyverse-0.0.2.1/src/tipyverse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipyverse
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A package to install Python equivalents of R tipyverse packages
 Author-email: Sebastian Dunn <sebastiandunn@sdmdigital.co>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Dunn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tipyverse-0.0.2/src/tipyverse.egg-info/SOURCES.txt` & `tipyverse-0.0.2.1/src/tipyverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tipyverse-0.0.2/tests/test_data_manipulation.py` & `tipyverse-0.0.2.1/tests/test_data_manipulation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import polars as pl
 import pytest
-from src import select, filter, mutate, arrange, summarize, group_by, summarize_grouped
+from src.tipyverse import select, filter, mutate, arrange, summarize, group_by, summarize_grouped
 
 
 @pytest.fixture
 def penguins():
     return pl.DataFrame({
         'island': ['Biscoe', 'Dream', 'Biscoe', 'Dream', 'Torgersen', 'Biscoe'],
         'bill_depth_mm': [18.7, 17.4, 18.0, 17.6, 18.5, 19.3]
```

