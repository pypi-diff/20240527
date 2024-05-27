# Comparing `tmp/sslearn-1.0.5.1.tar.gz` & `tmp/sslearn-1.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sslearn-1.0.5.1.tar", last modified: Mon May 20 11:13:44 2024, max compression
+gzip compressed data, was "sslearn-1.0.5.2.tar", last modified: Mon May 27 08:03:58 2024, max compression
```

## Comparing `sslearn-1.0.5.1.tar` & `sslearn-1.0.5.2.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.833571 sslearn-1.0.5.1/sslearn/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.833571 sslearn-1.0.5.1/sslearn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/datasets/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/model_selection/_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/restricted (Copia en conflicto de CROSS-PC 2024-05-14).py
--rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/restricted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn/subview/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/subview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/subview/_subview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60641 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/_co.py
--rw-r--r--   0 runner    (1001) docker     (127)    15721 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/_self.py
--rw-r--r--   0 runner    (1001) docker     (127)    32663 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/sslearn/wrapper/_tritraining.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/sslearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 11:13:44.000000 sslearn-1.0.5.1/sslearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:13:44.837571 sslearn-1.0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_subview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-20 11:13:40.000000 sslearn-1.0.5.1/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.034844 sslearn-1.0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-27 08:03:58.034844 sslearn-1.0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 08:03:58.034844 sslearn-1.0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.030844 sslearn-1.0.5.2/sslearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.030844 sslearn-1.0.5.2/sslearn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/datasets/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/datasets/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/datasets/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.030844 sslearn-1.0.5.2/sslearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/model_selection/_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17475 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/restricted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.034844 sslearn-1.0.5.2/sslearn/subview/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/subview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/subview/_subview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.034844 sslearn-1.0.5.2/sslearn/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60641 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/wrapper/_co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15721 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/wrapper/_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32663 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/sslearn/wrapper/_tritraining.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.034844 sslearn-1.0.5.2/sslearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-27 08:03:58.000000 sslearn-1.0.5.2/sslearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-27 08:03:58.000000 sslearn-1.0.5.2/sslearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:03:58.000000 sslearn-1.0.5.2/sslearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-27 08:03:58.000000 sslearn-1.0.5.2/sslearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 08:03:58.000000 sslearn-1.0.5.2/sslearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:03:58.034844 sslearn-1.0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/test/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/test/test_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/test/test_subview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-27 08:03:53.000000 sslearn-1.0.5.2/test/test_wrapper.py
```

### Comparing `sslearn-1.0.5.1/LICENSE` & `sslearn-1.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/PKG-INFO` & `sslearn-1.0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sslearn
-Version: 1.0.5.1
+Version: 1.0.5.2
 Summary: A Python package for semi-supervised learning with scikit-learn
 Home-page: https://github.com/jlgarridol/sslearn
-Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.1.tar.gz
+Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.2.tar.gz
 Author: José Luis Garrido-Labrador
 Author-email: jlgarrido@ubu.es
 License: new BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sslearn-1.0.5.1/README.md` & `sslearn-1.0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/setup.py` & `sslearn-1.0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/__init__.py` & `sslearn-1.0.5.2/sslearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 elif os.path.exists("README.md"):
     with open("README.md", "r") as f:
         __doc__ = f.read()
 else:
     __doc__ = "Semi-Supervised Learning (SSL) is a Python package that provides tools to train and evaluate semi-supervised learning models."
 
 
-__version__='1.0.5.1'
+__version__='1.0.5.2'
 __AUTHOR__="José Luis Garrido-Labrador"  # Author of the package
 __AUTHOR_EMAIL__="jlgarrido@ubu.es"  # Author's email
 __URL__="https://pypi.org/project/sslearn/"
```

### Comparing `sslearn-1.0.5.1/sslearn/base.py` & `sslearn-1.0.5.2/sslearn/base.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/datasets/__init__.py` & `sslearn-1.0.5.2/sslearn/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/datasets/_loader.py` & `sslearn-1.0.5.2/sslearn/datasets/_loader.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/datasets/_preprocess.py` & `sslearn-1.0.5.2/sslearn/datasets/_preprocess.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/datasets/_writer.py` & `sslearn-1.0.5.2/sslearn/datasets/_writer.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/model_selection/_split.py` & `sslearn-1.0.5.2/sslearn/model_selection/_split.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/restricted.py` & `sslearn-1.0.5.2/sslearn/restricted.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/subview/_subview.py` & `sslearn-1.0.5.2/sslearn/subview/_subview.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/utils.py` & `sslearn-1.0.5.2/sslearn/utils.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/wrapper/__init__.py` & `sslearn-1.0.5.2/sslearn/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/wrapper/_co.py` & `sslearn-1.0.5.2/sslearn/wrapper/_co.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/wrapper/_self.py` & `sslearn-1.0.5.2/sslearn/wrapper/_self.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn/wrapper/_tritraining.py` & `sslearn-1.0.5.2/sslearn/wrapper/_tritraining.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/sslearn.egg-info/PKG-INFO` & `sslearn-1.0.5.2/sslearn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sslearn
-Version: 1.0.5.1
+Version: 1.0.5.2
 Summary: A Python package for semi-supervised learning with scikit-learn
 Home-page: https://github.com/jlgarridol/sslearn
-Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.1.tar.gz
+Download-URL: https://github.com/jlgarridol/sslearn/archive/refs/tags/1.0.5.2.tar.gz
 Author: José Luis Garrido-Labrador
 Author-email: jlgarrido@ubu.es
 License: new BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sslearn-1.0.5.1/sslearn.egg-info/SOURCES.txt` & `sslearn-1.0.5.2/sslearn.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 sslearn/__init__.py
 sslearn/base.py
-sslearn/restricted (Copia en conflicto de CROSS-PC 2024-05-14).py
 sslearn/restricted.py
 sslearn/utils.py
 sslearn.egg-info/PKG-INFO
 sslearn.egg-info/SOURCES.txt
 sslearn.egg-info/dependency_links.txt
 sslearn.egg-info/requires.txt
 sslearn.egg-info/top_level.txt
```

### Comparing `sslearn-1.0.5.1/test/test_datasets.py` & `sslearn-1.0.5.2/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/test/test_general.py` & `sslearn-1.0.5.2/test/test_general.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/test/test_model_selection.py` & `sslearn-1.0.5.2/test/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/test/test_subview.py` & `sslearn-1.0.5.2/test/test_subview.py`

 * *Files identical despite different names*

### Comparing `sslearn-1.0.5.1/test/test_wrapper.py` & `sslearn-1.0.5.2/test/test_wrapper.py`

 * *Files identical despite different names*

