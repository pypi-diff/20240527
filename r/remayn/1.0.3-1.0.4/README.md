# Comparing `tmp/remayn-1.0.3.tar.gz` & `tmp/remayn-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remayn-1.0.3.tar", last modified: Tue May 21 09:17:51 2024, max compression
+gzip compressed data, was "remayn-1.0.4.tar", last modified: Mon May 27 17:55:01 2024, max compression
```

## Comparing `remayn-1.0.3.tar` & `remayn-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.988904 remayn-1.0.3/
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1492 2024-04-25 06:08:28.000000 remayn-1.0.3/LICENSE
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5943 2024-05-21 09:17:50.964630 remayn-1.0.3/PKG-INFO
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5007 2024-05-21 09:15:50.000000 remayn-1.0.3/README.md
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1068 2024-05-21 09:17:21.000000 remayn-1.0.3/pyproject.toml
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.607350 remayn-1.0.3/remayn/
--rw-r--r--   0 victor   (10038) ayrna     (1001)       35 2024-05-21 09:17:29.000000 remayn-1.0.3/remayn/__init__.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.737295 remayn-1.0.3/remayn/report/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      161 2024-05-19 11:27:24.000000 remayn-1.0.3/remayn/report/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5387 2024-05-21 08:03:44.000000 remayn-1.0.3/remayn/report/excel.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.793807 remayn-1.0.3/remayn/result/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      142 2024-05-01 12:37:43.000000 remayn-1.0.3/remayn/result/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)    18991 2024-05-19 09:56:20.000000 remayn-1.0.3/remayn/result/result.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     4773 2024-05-21 08:02:55.000000 remayn-1.0.3/remayn/result/result_data.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.855765 remayn-1.0.3/remayn/result_set/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      100 2024-05-07 11:34:45.000000 remayn-1.0.3/remayn/result_set/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)    17305 2024-05-21 08:07:09.000000 remayn-1.0.3/remayn/result_set/result_set.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5258 2024-05-21 08:05:29.000000 remayn-1.0.3/remayn/result_set/utils.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.925611 remayn-1.0.3/remayn/utils/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      246 2024-05-12 11:03:44.000000 remayn-1.0.3/remayn/utils/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1635 2024-05-12 12:47:43.000000 remayn-1.0.3/remayn/utils/dicts.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     2008 2024-05-09 10:08:48.000000 remayn-1.0.3/remayn/utils/json.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-21 09:17:50.947892 remayn-1.0.3/remayn.egg-info/
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5943 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/PKG-INFO
--rw-r--r--   0 victor   (10038) ayrna     (1001)      494 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/SOURCES.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)        1 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/dependency_links.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)      111 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/requires.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)        7 2024-05-21 09:17:50.000000 remayn-1.0.3/remayn.egg-info/top_level.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-05-21 09:17:50.989368 remayn-1.0.3/setup.cfg
--rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-04-27 10:55:10.000000 remayn-1.0.3/setup.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.856765 remayn-1.0.4/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1492 2024-04-25 06:08:28.000000 remayn-1.0.4/LICENSE
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5938 2024-05-27 17:55:01.842503 remayn-1.0.4/PKG-INFO
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5002 2024-05-27 10:17:57.000000 remayn-1.0.4/README.md
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1068 2024-05-27 17:49:31.000000 remayn-1.0.4/pyproject.toml
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.501487 remayn-1.0.4/remayn/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       35 2024-05-27 17:49:39.000000 remayn-1.0.4/remayn/__init__.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.605460 remayn-1.0.4/remayn/report/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      161 2024-05-19 11:27:24.000000 remayn-1.0.4/remayn/report/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5387 2024-05-21 08:03:44.000000 remayn-1.0.4/remayn/report/excel.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.652580 remayn-1.0.4/remayn/result/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      142 2024-05-01 12:37:43.000000 remayn-1.0.4/remayn/result/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)    18991 2024-05-19 09:56:20.000000 remayn-1.0.4/remayn/result/result.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     4145 2024-05-27 11:28:38.000000 remayn-1.0.4/remayn/result/result_data.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.725468 remayn-1.0.4/remayn/result_set/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      100 2024-05-07 11:34:45.000000 remayn-1.0.4/remayn/result_set/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)    17304 2024-05-27 17:47:22.000000 remayn-1.0.4/remayn/result_set/result_set.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5258 2024-05-21 08:05:29.000000 remayn-1.0.4/remayn/result_set/utils.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.788552 remayn-1.0.4/remayn/utils/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      296 2024-05-27 11:28:39.000000 remayn-1.0.4/remayn/utils/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      849 2024-05-27 11:28:39.000000 remayn-1.0.4/remayn/utils/array.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1635 2024-05-12 12:47:43.000000 remayn-1.0.4/remayn/utils/dicts.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     2008 2024-05-09 10:08:48.000000 remayn-1.0.4/remayn/utils/json.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.807418 remayn-1.0.4/remayn.egg-info/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5938 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/PKG-INFO
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      516 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/SOURCES.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)        1 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/dependency_links.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      111 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/requires.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)        7 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/top_level.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-05-27 17:55:01.857066 remayn-1.0.4/setup.cfg
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-04-27 10:55:10.000000 remayn-1.0.4/setup.py
```

### Comparing `remayn-1.0.3/LICENSE` & `remayn-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `remayn-1.0.3/PKG-INFO` & `remayn-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remayn
-Version: 1.0.3
+Version: 1.0.4
 Summary: REsults MAde easY in pythoN
 Author-email: Víctor Manuel Vargas <vvargas@uco.es>
 Project-URL: Source, https://github.com/ayrna/remayn
 Project-URL: Documentation, https://remayn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,19 @@
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # REMAYN: REsults MAde easY in pythoN
 
 `remayn` is an open-source Python toolkit focused on results management for machine learning experiments.
-It includes the required functionalities to save the complete results of an experiment, load them, and generate repots.
+It includes the required functionalities to save the complete results of an experiment, load them, and generate reports.
 
 | Overview  |                                                                                                                                          |
 |-----------|------------------------------------------------------------------------------------------------------------------------------------------|
-| **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/dlordinal/badge/?version=latest&style=flat)](https://dlordinal.readthedocs.io/en/latest/)  |
+| **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/remayn/badge/?version=latest&style=flat)](https://remayn.readthedocs.io/en/latest/)  |
 | **Code**  | [![!python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
 
 ## Getting started
 
 ### ⚙️ Installation
 
 `remayn` is supported by Python >=3.8.
```

### Comparing `remayn-1.0.3/README.md` & `remayn-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # REMAYN: REsults MAde easY in pythoN
 
 `remayn` is an open-source Python toolkit focused on results management for machine learning experiments.
-It includes the required functionalities to save the complete results of an experiment, load them, and generate repots.
+It includes the required functionalities to save the complete results of an experiment, load them, and generate reports.
 
 | Overview  |                                                                                                                                          |
 |-----------|------------------------------------------------------------------------------------------------------------------------------------------|
-| **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/dlordinal/badge/?version=latest&style=flat)](https://dlordinal.readthedocs.io/en/latest/)  |
+| **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/remayn/badge/?version=latest&style=flat)](https://remayn.readthedocs.io/en/latest/)  |
 | **Code**  | [![!python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
 
 ## Getting started
 
 ### ⚙️ Installation
 
 `remayn` is supported by Python >=3.8.
```

### Comparing `remayn-1.0.3/pyproject.toml` & `remayn-1.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "toml", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "remayn"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name = "Víctor Manuel Vargas", email = "vvargas@uco.es"},
 ]
 description = "REsults MAde easY in pythoN"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `remayn-1.0.3/remayn/report/excel.py` & `remayn-1.0.4/remayn/report/excel.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.3/remayn/result/result.py` & `remayn-1.0.4/remayn/result/result.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.3/remayn/result/result_data.py` & `remayn-1.0.4/remayn/result/result_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Optional
 
 import numpy as np
 
+from ..utils import check_array
+
 
 class ResultData:
     """Stores the results of a experiment.
     ResultData objects only contain data and are usually stored as pickle files.
 
     Attributes
     ----------
@@ -47,34 +49,26 @@
         val_predictions: Optional[np.ndarray] = None,
         time: Optional[float] = None,
         train_history: Optional[np.ndarray] = None,
         val_history: Optional[np.ndarray] = None,
         best_params: Optional[dict] = None,
         best_model: Optional[object] = None,
     ):
-        if not isinstance(targets, np.ndarray):
-            raise TypeError("targets must be a numpy array")
-        if not isinstance(predictions, np.ndarray):
-            raise TypeError("predictions must be a numpy array")
-        if train_targets is not None and not isinstance(train_targets, np.ndarray):
-            raise TypeError("train_targets must be a numpy array")
-        if train_predictions is not None and not isinstance(
-            train_predictions, np.ndarray
-        ):
-            raise TypeError("train_predictions must be a numpy array")
-        if val_targets is not None and not isinstance(val_targets, np.ndarray):
-            raise TypeError("val_targets must be a numpy array")
-        if val_predictions is not None and not isinstance(val_predictions, np.ndarray):
-            raise TypeError("val_predictions must be a numpy array")
-        if time is not None and not isinstance(time, (int, float)):
-            raise TypeError("time must be a number")
-        if train_history is not None and not isinstance(train_history, np.ndarray):
-            raise TypeError("train_history must be a numpy array")
-        if val_history is not None and not isinstance(val_history, np.ndarray):
-            raise TypeError("val_history must be a numpy array")
+        targets = check_array(targets)
+        predictions = check_array(predictions)
+        train_targets = check_array(train_targets, allow_none=True)
+        train_predictions = check_array(train_predictions, allow_none=True)
+        val_targets = check_array(val_targets, allow_none=True)
+        val_predictions = check_array(val_predictions, allow_none=True)
+        train_history = check_array(train_history, allow_none=True)
+        val_history = check_array(val_history, allow_none=True)
+
+        if not isinstance(time, (float, int)) and time is not None:
+            raise TypeError("time must be a float")
+
         if best_params is not None and not isinstance(best_params, dict):
             raise TypeError("best_params must be a dictionary")
 
         self.targets = targets
         self.predictions = predictions
         self.train_targets = train_targets
         self.train_predictions = train_predictions
```

### Comparing `remayn-1.0.3/remayn/result_set/result_set.py` & `remayn-1.0.4/remayn/result_set/result_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             "ResultSet with"
             f" {len(self.results_)} result{'s' if len(self.results_) > 1 else ''}"
         )
 
     def __repr__(self):
         return self.__str__()
 
-    def __contains__(self, result: Result) -> bool:
+    def __contains__(self, result: Union[str, dict, Result]) -> bool:
         return self.contains(result)
 
 
 class ResultFolder(ResultSet):
     """Stores a set of set of `Result` objects loaded from a directory.
     For each `Result` object, it stores the metadata of the experiment, such as the
     experiment info and the path where the result is stored. The predictions and targets
@@ -426,15 +426,15 @@
         It retrieves all the json files from `base_path`. Also, it checks that each
         json file has a corresponding pkl file. If the number of json files does not
         match the number of pkl files, a ValueError is raised.
 
         Raises
         ------
         ValueError
-            If the number of json files does not match the number of pkl files.
+            If the the pickle file for a given json file is not found.
 
         Examples
         --------
         >>> from remayn.result_set import ResultFolder
         >>> rf = ResultFolder("./results")
         """
 
@@ -446,15 +446,15 @@
         # Check that all the json files have its corresponding pkl file
         if len(json_files) != len(pkl_files):
             for json_file in json_files:
                 if json_file.with_suffix(".pkl") not in pkl_files:
                     raise FileNotFoundError(
                         f"Could not find pkl file for json file {json_file}",
                     )
-            raise FileNotFoundError(
+            warnings.warn(
                 f"Number of json files ({len(json_files)}) does not match"
                 f" number of pkl files ({len(pkl_files)})",
             )
 
         for path in json_files:
             result = Result.load(self.base_path, path.stem)
             key = str(sanitize_json(result.config))
```

### Comparing `remayn-1.0.3/remayn/result_set/utils.py` & `remayn-1.0.4/remayn/result_set/utils.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.3/remayn/utils/dicts.py` & `remayn-1.0.4/remayn/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.3/remayn/utils/json.py` & `remayn-1.0.4/remayn/utils/json.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.3/remayn.egg-info/PKG-INFO` & `remayn-1.0.4/remayn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remayn
-Version: 1.0.3
+Version: 1.0.4
 Summary: REsults MAde easY in pythoN
 Author-email: Víctor Manuel Vargas <vvargas@uco.es>
 Project-URL: Source, https://github.com/ayrna/remayn
 Project-URL: Documentation, https://remayn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,19 @@
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # REMAYN: REsults MAde easY in pythoN
 
 `remayn` is an open-source Python toolkit focused on results management for machine learning experiments.
-It includes the required functionalities to save the complete results of an experiment, load them, and generate repots.
+It includes the required functionalities to save the complete results of an experiment, load them, and generate reports.
 
 | Overview  |                                                                                                                                          |
 |-----------|------------------------------------------------------------------------------------------------------------------------------------------|
-| **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/dlordinal/badge/?version=latest&style=flat)](https://dlordinal.readthedocs.io/en/latest/)  |
+| **CI/CD** | [![!codecov](https://img.shields.io/codecov/c/github/ayrna/remayn?label=codecov&logo=codecov)](https://codecov.io/gh/ayrna/remayn) [![!docs](https://readthedocs.org/projects/remayn/badge/?version=latest&style=flat)](https://remayn.readthedocs.io/en/latest/)  |
 | **Code**  | [![!python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/) [![!black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Linter: Ruff](https://img.shields.io/badge/Linter-Ruff-brightgreen?style=flat-square)](https://github.com/charliermarsh/ruff)                     |
 
 ## Getting started
 
 ### ⚙️ Installation
 
 `remayn` is supported by Python >=3.8.
```

