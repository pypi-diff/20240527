# Comparing `tmp/njab-0.0.6.tar.gz` & `tmp/njab-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "njab-0.0.6.tar", last modified: Tue May 14 14:47:44 2024, max compression
+gzip compressed data, was "njab-0.0.7.tar", last modified: Mon May 27 16:42:48 2024, max compression
```

## Comparing `njab-0.0.6.tar` & `njab-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-14 14:47:40.000000 njab-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-14 14:47:44.309849 njab-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-14 14:47:40.000000 njab-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 14:47:40.000000 njab-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-14 14:47:44.309849 njab-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 14:47:40.000000 njab-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/njab/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/njab/io/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.305849 njab-0.0.6/src/njab/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/km.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/lifelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/plotting/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/pca.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/sklearn/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/stats/ancova.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-14 14:47:40.000000 njab-0.0.6/src/njab/stats/groups_comparision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/src/njab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 14:47:44.000000 njab-0.0.6/src/njab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:47:44.309849 njab-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 14:47:40.000000 njab-0.0.6/test/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 14:47:40.000000 njab-0.0.6/test/test_pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 14:47:40.000000 njab-0.0.6/test/test_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.217130 njab-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.201130 njab-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.205129 njab-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-27 16:42:42.000000 njab-0.0.7/.github/workflows/colab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-27 16:42:42.000000 njab-0.0.7/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-27 16:42:42.000000 njab-0.0.7/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.205129 njab-0.0.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 16:42:42.000000 njab-0.0.7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-27 16:42:42.000000 njab-0.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 16:42:42.000000 njab-0.0.7/CONTRIBUTE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-27 16:42:42.000000 njab-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-27 16:42:48.217130 njab-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-27 16:42:42.000000 njab-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.205129 njab-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-27 16:42:42.000000 njab-0.0.7/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-27 16:42:42.000000 njab-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 16:42:42.000000 njab-0.0.7/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.209130 njab-0.0.7/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.209130 njab-0.0.7/docs/tutorial/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.209130 njab-0.0.7/docs/tutorial/data/alzheimer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/data/alzheimer/clinic_ml.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/data/alzheimer/meta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  3434747 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/data/alzheimer/proteome.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/data/process_Alzheimer_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/explorative_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9769 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/explorative_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45139 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/log_reg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26841 2024-05-27 16:42:42.000000 njab-0.0.7/docs/tutorial/log_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-27 16:42:42.000000 njab-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-27 16:42:48.217130 njab-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 16:42:42.000000 njab-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.201130 njab-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.213130 njab-0.0.7/src/njab/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.213130 njab-0.0.7/src/njab/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.213130 njab-0.0.7/src/njab/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.213130 njab-0.0.7/src/njab/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/plotting/km.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/plotting/lifelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/plotting/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.213130 njab-0.0.7/src/njab/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/sklearn/pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/sklearn/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/sklearn/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.217130 njab-0.0.7/src/njab/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/stats/ancova.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-27 16:42:42.000000 njab-0.0.7/src/njab/stats/groups_comparision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.217130 njab-0.0.7/src/njab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-27 16:42:48.000000 njab-0.0.7/src/njab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-27 16:42:48.000000 njab-0.0.7/src/njab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:42:48.000000 njab-0.0.7/src/njab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 16:42:48.000000 njab-0.0.7/src/njab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 16:42:48.000000 njab-0.0.7/src/njab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:48.217130 njab-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:42.000000 njab-0.0.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-27 16:42:42.000000 njab-0.0.7/test/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-27 16:42:42.000000 njab-0.0.7/test/test_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-27 16:42:42.000000 njab-0.0.7/test/test_scoring.py
```

### Comparing `njab-0.0.6/LICENSE` & `njab-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/PKG-INFO` & `njab-0.0.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,42 @@
 Metadata-Version: 2.1
 Name: njab
-Version: 0.0.6
+Version: 0.0.7
 Summary: not Just Another Biomarker
-Author: Henry Webel
-Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
-License: MIT
+Author-email: Henry Webel <henry.webel@cpr.ku.dk>
+License: MIT License
+        
+        Copyright (c) 2022 University of Copenhagen
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Bug Tracker, https://github.com/RasmussenLab/njab/issues
+Project-URL: Homepage, https://github.com/RasmussenLab/njab
+Keywords: bioinformatics,biomarker
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: omegaconf
 Requires-Dist: lifelines
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
```

### Comparing `njab-0.0.6/README.md` & `njab-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/pandas/__init__.py` & `njab-0.0.7/src/njab/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/plotting/__init__.py` & `njab-0.0.7/src/njab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/plotting/km.py` & `njab-0.0.7/src/njab/plotting/km.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/plotting/lifelines.py` & `njab-0.0.7/src/njab/plotting/lifelines.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/plotting/metrics.py` & `njab-0.0.7/src/njab/plotting/metrics.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/sklearn/__init__.py` & `njab-0.0.7/src/njab/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/sklearn/pca.py` & `njab-0.0.7/src/njab/sklearn/pca.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/sklearn/preprocessing.py` & `njab-0.0.7/src/njab/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/sklearn/scoring.py` & `njab-0.0.7/src/njab/sklearn/scoring.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/sklearn/types.py` & `njab-0.0.7/src/njab/sklearn/types.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab/stats/ancova.py` & `njab-0.0.7/src/njab/stats/ancova.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Analysis of covariance using pingouin and statsmodels."""
 from __future__ import annotations
+
 import numpy as np
 import pandas as pd
-
 import pingouin as pg
 import statsmodels
 
 
 def ancova_pg(df_long: pd.DataFrame,
               feat_col: str,
               dv: str,
@@ -48,14 +48,15 @@
                     'qvalue',
                     'rejected']
     """
     scores = []
     # num_covar = len(covar)
 
     for feat_name, data_feat in df_long.groupby(feat_col):
+        # ? drop duplicated colummns in long data format?
         ancova = pg.ancova(data=data_feat, dv=dv, between=between, covar=covar)
         ancova[feat_col] = feat_name
         scores.append(ancova)
     scores = pd.concat(scores)
     scores['-Log10 pvalue'] = -np.log10(scores['p-unc'])
 
     return scores
@@ -133,14 +134,16 @@
        of the linear regression for each.
     """
 
     def ancova(self, random_seed=123):
 
         scores = self.get_scores()
         scores = filter_residuals_from_scores(scores)
+        # drop nan values (due to multicollinearity of features - i.e. duplicated features)
+        scores = scores.dropna()
         scores = add_fdr_scores(scores, random_seed=random_seed)
         self.scores = scores
         return scores.set_index('Source', append=True)
 
 
 def filter_all_covars_from_scores(scores: pd.DataFrame,
                                   filter_for: str) -> pd.DataFrame:
```

### Comparing `njab-0.0.6/src/njab/stats/groups_comparision.py` & `njab-0.0.7/src/njab/stats/groups_comparision.py`

 * *Files identical despite different names*

### Comparing `njab-0.0.6/src/njab.egg-info/PKG-INFO` & `njab-0.0.7/src/njab.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,42 @@
 Metadata-Version: 2.1
 Name: njab
-Version: 0.0.6
+Version: 0.0.7
 Summary: not Just Another Biomarker
-Author: Henry Webel
-Author-email: "Henry Webel" <henry.webel@cpr.ku.dk>
-License: MIT
+Author-email: Henry Webel <henry.webel@cpr.ku.dk>
+License: MIT License
+        
+        Copyright (c) 2022 University of Copenhagen
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Bug Tracker, https://github.com/RasmussenLab/njab/issues
+Project-URL: Homepage, https://github.com/RasmussenLab/njab
+Keywords: bioinformatics,biomarker
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: omegaconf
 Requires-Dist: lifelines
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
```

