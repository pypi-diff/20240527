# Comparing `tmp/metabotk-0.1.36.tar.gz` & `tmp/metabotk-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.36.tar", max compression
+gzip compressed data, was "metabotk-0.1.37.tar", max compression
```

## Comparing `metabotk-0.1.36.tar` & `metabotk-0.1.37.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2184 2024-05-23 10:40:32.169618 metabotk-0.1.36/README.md
--rw-r--r--   0        0        0      531 2024-05-23 10:28:10.899057 metabotk-0.1.36/metabotk/__init__.py
--rw-r--r--   0        0        0       23 2024-05-24 14:28:38.002332 metabotk-0.1.36/metabotk/_version.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.36/metabotk/cli.py
--rw-r--r--   0        0        0    26255 2024-05-23 10:33:39.163099 metabotk-0.1.36/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2388 2024-05-21 18:11:30.585916 metabotk-0.1.36/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.36/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.36/metabotk/imputation.py
--rw-r--r--   0        0        0     6549 2024-05-12 14:39:51.768689 metabotk-0.1.36/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.36/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.36/metabotk/models_handler.py
--rw-r--r--   0        0        0     9020 2024-05-24 10:56:48.094307 metabotk-0.1.36/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.36/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.36/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-23 10:29:17.747712 metabotk-0.1.36/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.36/metabotk/utils.py
--rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.36/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      735 2024-05-24 14:28:26.954051 metabotk-0.1.36/pyproject.toml
--rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 metabotk-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0     4442 2024-05-24 14:51:14.708349 metabotk-0.1.37/README.md
+-rw-r--r--   0        0        0      531 2024-05-23 10:28:10.899057 metabotk-0.1.37/metabotk/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-24 14:28:38.002332 metabotk-0.1.37/metabotk/_version.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.37/metabotk/cli.py
+-rw-r--r--   0        0        0    26255 2024-05-23 10:33:39.163099 metabotk-0.1.37/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2388 2024-05-21 18:11:30.585916 metabotk-0.1.37/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.37/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.37/metabotk/imputation.py
+-rw-r--r--   0        0        0     6553 2024-05-24 16:03:17.168372 metabotk-0.1.37/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.37/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.37/metabotk/models_handler.py
+-rw-r--r--   0        0        0     9020 2024-05-24 16:03:07.004132 metabotk-0.1.37/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.37/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-24 14:44:47.434686 metabotk-0.1.37/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     9052 2024-05-24 14:44:35.050377 metabotk-0.1.37/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.37/metabotk/utils.py
+-rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.37/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      735 2024-05-27 10:58:08.641476 metabotk-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 metabotk-0.1.37/PKG-INFO
```

### Comparing `metabotk-0.1.36/metabotk/__init__.py` & `metabotk-0.1.37/metabotk/__init__.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/cli.py` & `metabotk-0.1.37/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/dataset_manager.py` & `metabotk-0.1.37/metabotk/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/dimensionality_reduction.py` & `metabotk-0.1.37/metabotk/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/feature_selection.py` & `metabotk-0.1.37/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/imputation.py` & `metabotk-0.1.37/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/interface.py` & `metabotk-0.1.37/metabotk/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             self._imputation_ = ImputationHandler(self)
         return self._imputation_
 
     @property
     def normalization(self):
         """Lazy initialization of NormalizationHandler instance."""
         if not hasattr(self, "_normalization_"):
-            self._normalization_ = NormalizationHandler()
+            self._normalization_ = NormalizationHandler(self)
         return self._normalization_
 
     @property
     def feature_selection(self):
         """Lazy initialization of FeatureSelection instance."""
         if not hasattr(self, "_feature_selection_"):
             self._feature_selection_ = FeatureSelection(self)
```

### Comparing `metabotk-0.1.36/metabotk/missing_handler.py` & `metabotk-0.1.37/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/models_handler.py` & `metabotk-0.1.37/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/normalization.py` & `metabotk-0.1.37/metabotk/normalization.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/outliers_handler.py` & `metabotk-0.1.37/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/providers_handler.py` & `metabotk-0.1.37/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/statistics_handler.py` & `metabotk-0.1.37/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/utils.py` & `metabotk-0.1.37/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/metabotk/visualization_handler.py` & `metabotk-0.1.37/metabotk/visualization_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.36/pyproject.toml` & `metabotk-0.1.37/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.36"
+version = "0.1.37"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
```

