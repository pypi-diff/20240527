# Comparing `tmp/naiveautoml-0.1.0.tar.gz` & `tmp/naiveautoml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naiveautoml-0.1.0.tar", last modified: Wed May 15 12:19:31 2024, max compression
+gzip compressed data, was "naiveautoml-0.1.1.tar", last modified: Mon May 27 17:00:25 2024, max compression
```

## Comparing `naiveautoml-0.1.0.tar` & `naiveautoml-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/
--rw-r--r--   0 felix     (1000) felix     (1000)     1062 2021-10-27 14:20:45.000000 naiveautoml-0.1.0/LICENSE.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      842 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)     5338 2024-05-11 15:11:20.000000 naiveautoml-0.1.0/README.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.702047 naiveautoml-0.1.0/naiveautoml/
--rw-r--r--   0 felix     (1000) felix     (1000)       87 2024-03-01 21:07:57.000000 naiveautoml-0.1.0/naiveautoml/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    10429 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/_interfaces.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9384 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/commons.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8913 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/evaluators.py
--rw-r--r--   0 felix     (1000) felix     (1000)    11228 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/naiveautoml.py
--rw-r--r--   0 felix     (1000) felix     (1000)    56249 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/searchspace-classification.json
--rw-r--r--   0 felix     (1000) felix     (1000)    59071 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/naiveautoml/searchspace-regression.json
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/naiveautoml.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)      842 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)      465 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      122 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       12 2024-05-15 12:19:31.000000 naiveautoml-0.1.0/naiveautoml.egg-info/top_level.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      471 2024-03-01 21:07:57.000000 naiveautoml-0.1.0/pyproject.toml
--rw-r--r--   0 felix     (1000) felix     (1000)       79 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)     1383 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/setup.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-15 12:19:31.705381 naiveautoml-0.1.0/test/
--rw-r--r--   0 felix     (1000) felix     (1000)    31813 2024-05-15 12:17:10.000000 naiveautoml-0.1.0/test/test_naiveautoml.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-27 17:00:25.384810 naiveautoml-0.1.1/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1062 2021-10-27 14:20:45.000000 naiveautoml-0.1.1/LICENSE.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      842 2024-05-27 17:00:25.388143 naiveautoml-0.1.1/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     5338 2024-05-27 16:45:29.000000 naiveautoml-0.1.1/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-27 17:00:25.384810 naiveautoml-0.1.1/naiveautoml/
+-rw-r--r--   0 felix     (1000) felix     (1000)       86 2024-05-27 16:45:35.000000 naiveautoml-0.1.1/naiveautoml/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    10429 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/_interfaces.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-27 17:00:25.384810 naiveautoml-0.1.1/naiveautoml/algorithm_selection/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/algorithm_selection/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      276 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/algorithm_selection/_pipeline.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    34055 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/algorithm_selection/_sklearn_factory.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2654 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/algorithm_selection/_sklearn_hpo.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    28609 2024-05-27 16:45:29.000000 naiveautoml-0.1.1/naiveautoml/algorithm_selection/sklearn.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9384 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/commons.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8913 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/evaluators.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-27 17:00:25.384810 naiveautoml-0.1.1/naiveautoml/hpo/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2024-05-27 16:54:15.000000 naiveautoml-0.1.1/naiveautoml/hpo/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3584 2024-05-27 16:45:29.000000 naiveautoml-0.1.1/naiveautoml/hpo/random_search.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    11200 2024-05-27 16:48:07.000000 naiveautoml-0.1.1/naiveautoml/naiveautoml.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    56249 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/searchspace-classification.json
+-rw-r--r--   0 felix     (1000) felix     (1000)    59071 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/naiveautoml/searchspace-regression.json
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-27 17:00:25.384810 naiveautoml-0.1.1/naiveautoml.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)      842 2024-05-27 17:00:25.000000 naiveautoml-0.1.1/naiveautoml.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)      758 2024-05-27 17:00:25.000000 naiveautoml-0.1.1/naiveautoml.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2024-05-27 17:00:25.000000 naiveautoml-0.1.1/naiveautoml.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      127 2024-05-27 17:00:25.000000 naiveautoml-0.1.1/naiveautoml.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       12 2024-05-27 17:00:25.000000 naiveautoml-0.1.1/naiveautoml.egg-info/top_level.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      471 2024-03-01 21:07:57.000000 naiveautoml-0.1.1/pyproject.toml
+-rw-r--r--   0 felix     (1000) felix     (1000)       79 2024-05-27 17:00:25.388143 naiveautoml-0.1.1/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)     1430 2024-05-27 16:56:35.000000 naiveautoml-0.1.1/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2024-05-27 17:00:25.384810 naiveautoml-0.1.1/test/
+-rw-r--r--   0 felix     (1000) felix     (1000)    31813 2024-05-27 16:30:56.000000 naiveautoml-0.1.1/test/test_naiveautoml.py
```

### Comparing `naiveautoml-0.1.0/LICENSE.txt` & `naiveautoml-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.1.0/PKG-INFO` & `naiveautoml-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naiveautoml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fast and Timeout-Free Automated Machine Learning for Multi-Class classification, Multi-Label classification, and regression.
 Home-page: https://github.com/fmohr/naiveautoml
 Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.27.tar.gz
 Author: Felix Mohr
 Author-email: mail@felixmohr.de
 License: MIT
 Keywords: AutoML,sklearn,naive,simple,multi-class,multi-label,regression,no timeouts
```

### Comparing `naiveautoml-0.1.0/README.md` & `naiveautoml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.1.0/naiveautoml/_interfaces.py` & `naiveautoml-0.1.1/naiveautoml/_interfaces.py`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.1.0/naiveautoml/commons.py` & `naiveautoml-0.1.1/naiveautoml/commons.py`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.1.0/naiveautoml/evaluators.py` & `naiveautoml-0.1.1/naiveautoml/evaluators.py`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.1.0/naiveautoml/naiveautoml.py` & `naiveautoml-0.1.1/naiveautoml/naiveautoml.py`

 * *Files identical despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 import traceback
 
 import pandas as pd
 import time
 
 # naiveautoml commons
+from ._interfaces import SupervisedTask, HPOptimizer
+from .algorithm_selection.sklearn import SKLearnAlgorithmSelector
+from .hpo.random_search import RandomHPO
 from .commons import EvaluationPool
 
 import numpy as np
-from ._interfaces import SupervisedTask, HPOptimizer
 
 
 class NaiveAutoML:
 
     def __init__(self,
                  task_type: str = "auto",
                  algorithm_selector="sklearn",
@@ -59,15 +61,14 @@
         if isinstance(algorithm_selector, str):
             accepted_selectors = ["sklearn"]
             if "logger" not in kwargs_as:
                 kwargs_as["logger"] = self.logger
             if "strictly_naive" not in kwargs_as:
                 kwargs_as["strictly_naive"] = strictly_naive
             if algorithm_selector == "sklearn":
-                from .algorithm_selection.sklearn import SKLearnAlgorithmSelector
                 self.algorithm_selector = SKLearnAlgorithmSelector(
                     show_progress=show_progress,
                     raise_errors=raise_errors,
                     **kwargs_as
                 )
             else:
                 raise ValueError(
@@ -78,15 +79,14 @@
             self.algorithm_selector = algorithm_selector
 
         # configure hyperparameter optimizer
         if isinstance(hp_optimizer, str):
             accepted_optimizers = ["random"]
             if hp_optimizer not in accepted_optimizers:
                 raise ValueError(f"hp_optimizer if string must be in {accepted_optimizers} but is {hp_optimizer}")
-            from .hpo.random_search import RandomHPO
             self.hp_optimizer = RandomHPO(
                 show_progress=show_progress,
                 logger=self.logger,
                 **kwargs_hpo
             )
         else:
             if not isinstance(hp_optimizer, HPOptimizer):
```

### Comparing `naiveautoml-0.1.0/naiveautoml/searchspace-classification.json` & `naiveautoml-0.1.1/naiveautoml/searchspace-classification.json`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.1.0/naiveautoml/searchspace-regression.json` & `naiveautoml-0.1.1/naiveautoml/searchspace-regression.json`

 * *Files identical despite different names*

### Comparing `naiveautoml-0.1.0/naiveautoml.egg-info/PKG-INFO` & `naiveautoml-0.1.1/naiveautoml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naiveautoml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fast and Timeout-Free Automated Machine Learning for Multi-Class classification, Multi-Label classification, and regression.
 Home-page: https://github.com/fmohr/naiveautoml
 Download-URL: https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.27.tar.gz
 Author: Felix Mohr
 Author-email: mail@felixmohr.de
 License: MIT
 Keywords: AutoML,sklearn,naive,simple,multi-class,multi-label,regression,no timeouts
```

### Comparing `naiveautoml-0.1.0/setup.py` & `naiveautoml-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from distutils.core import setup
+from setuptools import setup, find_packages
+
+
 setup(
   name = 'naiveautoml',
-  packages = ['naiveautoml'],
-  version = '0.1.0',
+  packages = find_packages(exclude=["test"]),
+  version = '0.1.1',
   license='MIT',
   description = 'Fast and Timeout-Free Automated Machine Learning for Multi-Class classification, Multi-Label classification, and regression.',
   author = 'Felix Mohr',
   author_email = 'mail@felixmohr.de',
   url = 'https://github.com/fmohr/naiveautoml',
   download_url = 'https://github.com/fmohr/naiveautoml/archive/refs/tags/v0.0.27.tar.gz',
   keywords = ['AutoML', 'sklearn', 'naive', 'simple', 'multi-class', 'multi-label', 'regression', 'no timeouts'],
   install_requires=[
           'numpy',
           'pandas',
-          'scikit-learn>=1.4',
+          'scikit-learn==1.4',
           'scikit-multilearn==0.2.0',
           'configspace<0.7.1',
           'scipy',
           'pynisher',
           'psutil',
           'tqdm',
           'parameterized',
-          'openml'
+          'openml',
+          'lccv'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.7',
```

### Comparing `naiveautoml-0.1.0/test/test_naiveautoml.py` & `naiveautoml-0.1.1/test/test_naiveautoml.py`

 * *Files identical despite different names*

