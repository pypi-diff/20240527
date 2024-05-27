# Comparing `tmp/tubesml-0.7.2.tar.gz` & `tmp/tubesml-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tubesml-0.7.2.tar", last modified: Sat May 25 20:35:22 2024, max compression
+gzip compressed data, was "tubesml-0.7.3.tar", last modified: Mon May 27 19:46:33 2024, max compression
```

## Comparing `tubesml-0.7.2.tar` & `tubesml-0.7.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.044701 tubesml-0.7.2/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11357 2020-10-04 18:40:12.000000 tubesml-0.7.2/LICENSE
--rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2024-05-25 20:35:22.044701 tubesml-0.7.2/PKG-INFO
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1781 2023-01-03 21:42:35.000000 tubesml-0.7.2/README.rst
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       38 2024-05-25 20:35:22.044701 tubesml-0.7.2/setup.cfg
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2014 2024-05-25 20:34:32.000000 tubesml-0.7.2/setup.py
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.004701 tubesml-0.7.2/tests/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4045 2023-08-15 20:26:18.000000 tubesml-0.7.2/tests/test_clean.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8307 2023-08-15 20:18:25.000000 tubesml-0.7.2/tests/test_cvscore.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4366 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_dummy.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1785 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_encoders.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1590 2021-05-15 13:05:17.000000 tubesml-0.7.2/tests/test_explore.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5773 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_grid.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11103 2023-08-15 20:18:21.000000 tubesml-0.7.2/tests/test_inspection.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1778 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_pca.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2648 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_pipe.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2074 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_poly.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8690 2023-10-01 17:10:15.000000 tubesml-0.7.2/tests/test_report.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3144 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_scale.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    15362 2024-05-25 20:34:05.000000 tubesml-0.7.2/tests/test_stacker.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4161 2022-09-24 14:30:05.000000 tubesml-0.7.2/tests/test_utility.py
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.032701 tubesml-0.7.2/tubesml/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1457 2021-05-15 13:05:17.000000 tubesml-0.7.2/tubesml/__init__.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2178 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/base.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3579 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/clean.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3887 2021-05-01 16:25:39.000000 tubesml-0.7.2/tubesml/dummy.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4069 2021-05-01 16:25:39.000000 tubesml-0.7.2/tubesml/encoders.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     7598 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/explore.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    16485 2023-10-23 18:29:50.000000 tubesml-0.7.2/tubesml/model_inspection.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10093 2023-10-23 16:56:54.000000 tubesml-0.7.2/tubesml/model_selection.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5213 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/pca.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3909 2022-09-24 14:30:05.000000 tubesml-0.7.2/tubesml/poly.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10282 2023-10-01 17:10:15.000000 tubesml-0.7.2/tubesml/report.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5174 2022-09-25 08:36:06.000000 tubesml-0.7.2/tubesml/scale.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11443 2024-05-25 20:34:05.000000 tubesml-0.7.2/tubesml/stacker.py
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5110 2023-01-02 21:22:19.000000 tubesml-0.7.2/tubesml/utility.py
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.044701 tubesml-0.7.2/tubesml.egg-info/
-drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-25 20:35:22.044701 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      607 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       49 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2020-10-07 20:07:57.000000 tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/PKG-INFO
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      986 2024-05-25 20:35:21.000000 tubesml-0.7.2/tubesml.egg-info/SOURCES.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/dependency_links.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       68 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/requires.txt
--rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2024-05-25 20:35:20.000000 tubesml-0.7.2/tubesml.egg-info/top_level.txt
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-27 19:46:33.205436 tubesml-0.7.3/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11357 2020-10-04 18:40:12.000000 tubesml-0.7.3/LICENSE
+-rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2024-05-27 19:46:33.205436 tubesml-0.7.3/PKG-INFO
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1781 2024-05-27 19:09:50.000000 tubesml-0.7.3/README.rst
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       38 2024-05-27 19:46:33.205436 tubesml-0.7.3/setup.cfg
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2014 2024-05-27 19:46:27.000000 tubesml-0.7.3/setup.py
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-27 19:46:33.177439 tubesml-0.7.3/tests/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4045 2023-08-15 20:26:18.000000 tubesml-0.7.3/tests/test_clean.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8307 2023-08-15 20:18:25.000000 tubesml-0.7.3/tests/test_cvscore.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4366 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_dummy.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1785 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_encoders.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1590 2021-05-15 13:05:17.000000 tubesml-0.7.3/tests/test_explore.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5773 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_grid.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11103 2023-08-15 20:18:21.000000 tubesml-0.7.3/tests/test_inspection.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1778 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_pca.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2648 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_pipe.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2074 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_poly.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8690 2023-10-01 17:10:15.000000 tubesml-0.7.3/tests/test_report.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3144 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_scale.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    15362 2024-05-25 20:34:05.000000 tubesml-0.7.3/tests/test_stacker.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4161 2022-09-24 14:30:05.000000 tubesml-0.7.3/tests/test_utility.py
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-27 19:46:33.201436 tubesml-0.7.3/tubesml/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     1457 2021-05-15 13:05:17.000000 tubesml-0.7.3/tubesml/__init__.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     2178 2022-09-25 08:36:06.000000 tubesml-0.7.3/tubesml/base.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3579 2022-09-25 08:36:06.000000 tubesml-0.7.3/tubesml/clean.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3887 2021-05-01 16:25:39.000000 tubesml-0.7.3/tubesml/dummy.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     4069 2021-05-01 16:25:39.000000 tubesml-0.7.3/tubesml/encoders.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     8010 2024-05-27 19:46:27.000000 tubesml-0.7.3/tubesml/explore.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    16493 2024-05-27 19:46:27.000000 tubesml-0.7.3/tubesml/model_inspection.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10093 2023-10-23 16:56:54.000000 tubesml-0.7.3/tubesml/model_selection.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5213 2022-09-25 08:36:06.000000 tubesml-0.7.3/tubesml/pca.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     3909 2022-09-24 14:30:05.000000 tubesml-0.7.3/tubesml/poly.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    10282 2023-10-01 17:10:15.000000 tubesml-0.7.3/tubesml/report.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5174 2022-09-25 08:36:06.000000 tubesml-0.7.3/tubesml/scale.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)    11443 2024-05-25 20:34:05.000000 tubesml-0.7.3/tubesml/stacker.py
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)     5110 2023-01-02 21:22:19.000000 tubesml-0.7.3/tubesml/utility.py
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-27 19:46:33.205436 tubesml-0.7.3/tubesml.egg-info/
+drwxrwxr-x   0 lucabasa  (1000) lucabasa  (1000)        0 2024-05-27 19:46:33.205436 tubesml-0.7.3/tubesml.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      607 2020-10-07 20:07:57.000000 tubesml-0.7.3/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2020-10-07 20:07:57.000000 tubesml-0.7.3/tubesml.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       49 2020-10-07 20:07:57.000000 tubesml-0.7.3/tubesml.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2020-10-07 20:07:57.000000 tubesml-0.7.3/tubesml.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 lucabasa  (1000) lucabasa  (1000)     2874 2024-05-27 19:46:32.000000 tubesml-0.7.3/tubesml.egg-info/PKG-INFO
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)      986 2024-05-27 19:46:33.000000 tubesml-0.7.3/tubesml.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        1 2024-05-27 19:46:32.000000 tubesml-0.7.3/tubesml.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)       68 2024-05-27 19:46:32.000000 tubesml-0.7.3/tubesml.egg-info/requires.txt
+-rw-rw-r--   0 lucabasa  (1000) lucabasa  (1000)        8 2024-05-27 19:46:32.000000 tubesml-0.7.3/tubesml.egg-info/top_level.txt
```

### Comparing `tubesml-0.7.2/LICENSE` & `tubesml-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/PKG-INFO` & `tubesml-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubesml
-Version: 0.7.2
+Version: 0.7.3
 Summary: tubesML, a package that allows for flexible ML pipelines, model validation, and model inspection
 Home-page: https://pypi.org/project/tubesml/
 Download-URL: https://github.com/lucabasa/tubesML
 Author: Luca Basanisi
 Author-email: luca.basanisi@gmail.com
 Maintainer: Luca Basanisi
 Maintainer-email: luca.basanisi@gmail.com
@@ -21,15 +21,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: scikit-learn>=1.0.2
-Requires-Dist: seaborn>=0.12.0
+Requires-Dist: seaborn>=0.12.2
 
 .. |PythonMinVersion| replace:: 3.7
 .. |PandasMinVersion| replace:: 1.3.5
 .. |SklearnMinVersion| replace:: 1.0.2
 .. |PltMinVersion| replace:: 3.5.3
 .. |SnsMinVersion| replace:: 0.12.0
```

### Comparing `tubesml-0.7.2/README.rst` & `tubesml-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/setup.py` & `tubesml-0.7.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 LICENSE = 'Apache 2.0'
 DOWNLOAD_URL = 'https://github.com/lucabasa/tubesML'
 PROJECT_URLS = {
     #'Bug Tracker': ,
     'Documentation': 'https://tubesml.readthedocs.io/',
     'Source Code': 'https://github.com/lucabasa/tubesML'
 }
-VERSION = '0.7.2'
+VERSION = '0.7.3'
 PYTHON_REQUIRES = ">=3.7"
 
 INSTALL_REQUIRES = [
     'matplotlib>=3.5.3',
     'pandas>=1.3.5',
     'scikit-learn>=1.0.2',
-    'seaborn>=0.12.0'
+    'seaborn>=0.12.2'
 ]
 
 
 PACKAGES = [
     'tubesml',
 ]
```

### Comparing `tubesml-0.7.2/tests/test_clean.py` & `tubesml-0.7.3/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_cvscore.py` & `tubesml-0.7.3/tests/test_cvscore.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_dummy.py` & `tubesml-0.7.3/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_encoders.py` & `tubesml-0.7.3/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_explore.py` & `tubesml-0.7.3/tests/test_explore.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_grid.py` & `tubesml-0.7.3/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_inspection.py` & `tubesml-0.7.3/tests/test_inspection.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_pca.py` & `tubesml-0.7.3/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_pipe.py` & `tubesml-0.7.3/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_poly.py` & `tubesml-0.7.3/tests/test_poly.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_report.py` & `tubesml-0.7.3/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_scale.py` & `tubesml-0.7.3/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_stacker.py` & `tubesml-0.7.3/tests/test_stacker.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tests/test_utility.py` & `tubesml-0.7.3/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/__init__.py` & `tubesml-0.7.3/tubesml/__init__.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/base.py` & `tubesml-0.7.3/tubesml/base.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/clean.py` & `tubesml-0.7.3/tubesml/clean.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/dummy.py` & `tubesml-0.7.3/tubesml/dummy.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/encoders.py` & `tubesml-0.7.3/tubesml/encoders.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/explore.py` & `tubesml-0.7.3/tubesml/explore.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 __author__ = 'lucabasa'
-__version__ = '1.1.3'
+__version__ = '1.2.0'
 __status__ = 'development'
 
 
 import pandas as pd
 import numpy as np
 
 from scipy import stats
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
+import warnings  # Fixme: remove this when Seaborn is updated to 0.13
+warnings.filterwarnings("ignore", "is_categorical_dtype")
+warnings.filterwarnings("ignore", "use_inf_as_na")
+
 
 
 def list_missing(data, verbose=True):
     """
     Find all the columns with missing values and report on the percentage of missing values.
     
     :param data: pandas Dataframe.
@@ -63,15 +67,15 @@
     if target:
         corr['abs'] = abs(corr[target])
         cor_target = corr.sort_values(by='abs', ascending=False)[target]
         cor_target = cor_target[:limit]
         del corr['abs']
         corr = corr.loc[cor_target.index, cor_target.index]
     plt.figure(figsize=figsize)
-    ax = sns.heatmap(corr, cmap='RdBu_r', **kwargs)
+    ax = sns.heatmap(data=corr, cmap='RdBu_r', **kwargs)
     ax.set_xticklabels(ax.get_xticklabels(), rotation=45)
     plt.show()
     if target:
         return cor_target
 
 
 def plot_distribution(data, column, bins=50, correlation=None):
@@ -205,17 +209,21 @@
     return cats
 
 
 def segm_target(data, cat, target):
     '''
     Studies the target segmented by a categorical feature.
     It plots both a boxplot and a distplot for visual support
+    
+    :param data: Pandas Dataframe with the columns cat and target
+    :param cat: str, name of the category used to cut the data
+    :param target: str, name of the continuous target variable
     '''
     df = data.groupby(cat)[target].agg(['count', 'mean', 'max', 
                                         'min', 'median', 'std'])
     fig, ax = plt.subplots(1,2, figsize=(12, 5))
-    sns.boxplot(cat, target, data=data, ax=ax[0])
+    sns.boxplot(x=cat, y=target, data=data, ax=ax[0])
     for val in data[cat].unique():
         tmp = data[data[cat] == val]
-        sns.kdeplot(tmp[target], linewidth=3, alpha=0.7,
-                 label=val, ax=ax[1])  
+        sns.kdeplot(data=tmp[target], linewidth=3, alpha=0.7,
+                 label=val, ax=ax[1], warn_singular=False)  
     return df
```

### Comparing `tubesml-0.7.2/tubesml/model_inspection.py` & `tubesml-0.7.3/tubesml/model_inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         raise KeyError('data must contain the columns feat, mean, and std')
     
     if n > 0:
         fi = data.head(n)
     else:
         fi = data
     
-    fig, ax = plt.subplots(1,1, figsize=(13, int(0.3*fi.shape[0])))
+    fig, ax = plt.subplots(1,1, figsize=(13, max(1, int(0.3*fi.shape[0]))))
 
     sns.barplot(x=fi['mean'], y=fi.index, xerr=fi['std'], ax=ax)
     
     if savename is not None:
         plt.savefig(savename)
         plt.close()
     else:
```

### Comparing `tubesml-0.7.2/tubesml/model_selection.py` & `tubesml-0.7.3/tubesml/model_selection.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/pca.py` & `tubesml-0.7.3/tubesml/pca.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/poly.py` & `tubesml-0.7.3/tubesml/poly.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/report.py` & `tubesml-0.7.3/tubesml/report.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/scale.py` & `tubesml-0.7.3/tubesml/scale.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/stacker.py` & `tubesml-0.7.3/tubesml/stacker.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml/utility.py` & `tubesml-0.7.3/tubesml/utility.py`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `tubesml-0.7.3/tubesml.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `tubesml-0.7.2/tubesml.egg-info/PKG-INFO` & `tubesml-0.7.3/tubesml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tubesml
-Version: 0.7.2
+Version: 0.7.3
 Summary: tubesML, a package that allows for flexible ML pipelines, model validation, and model inspection
 Home-page: https://pypi.org/project/tubesml/
 Download-URL: https://github.com/lucabasa/tubesML
 Author: Luca Basanisi
 Author-email: luca.basanisi@gmail.com
 Maintainer: Luca Basanisi
 Maintainer-email: luca.basanisi@gmail.com
@@ -21,15 +21,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.5.3
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: scikit-learn>=1.0.2
-Requires-Dist: seaborn>=0.12.0
+Requires-Dist: seaborn>=0.12.2
 
 .. |PythonMinVersion| replace:: 3.7
 .. |PandasMinVersion| replace:: 1.3.5
 .. |SklearnMinVersion| replace:: 1.0.2
 .. |PltMinVersion| replace:: 3.5.3
 .. |SnsMinVersion| replace:: 0.12.0
```

### Comparing `tubesml-0.7.2/tubesml.egg-info/SOURCES.txt` & `tubesml-0.7.3/tubesml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

