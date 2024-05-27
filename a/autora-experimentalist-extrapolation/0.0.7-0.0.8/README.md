# Comparing `tmp/autora_experimentalist_extrapolation-0.0.7.tar.gz` & `tmp/autora_experimentalist_extrapolation-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_experimentalist_extrapolation-0.0.7.tar", last modified: Thu Apr 18 12:58:13 2024, max compression
+gzip compressed data, was "autora_experimentalist_extrapolation-0.0.8.tar", last modified: Mon May 27 17:30:37 2024, max compression
```

## Comparing `autora_experimentalist_extrapolation-0.0.7.tar` & `autora_experimentalist_extrapolation-0.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/.idea/autora-experimentalist-extrapolation.iml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.017148 autora_experimentalist_extrapolation-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.017148 autora_experimentalist_extrapolation-0.0.7/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.017148 autora_experimentalist_extrapolation-0.0.7/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/src/autora/experimentalist/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/src/autora/experimentalist/extrapolation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 12:58:12.000000 autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-18 12:58:13.000000 autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:58:12.000000 autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 12:58:12.000000 autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 12:58:12.000000 autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:58:13.021148 autora_experimentalist_extrapolation-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-18 12:58:03.000000 autora_experimentalist_extrapolation-0.0.7/tests/test_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.450846 autora_experimentalist_extrapolation-0.0.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.450846 autora_experimentalist_extrapolation-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.450846 autora_experimentalist_extrapolation-0.0.8/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/.idea/autora-experimentalist-extrapolation.iml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.450846 autora_experimentalist_extrapolation-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.450846 autora_experimentalist_extrapolation-0.0.8/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.450846 autora_experimentalist_extrapolation-0.0.8/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/src/autora/experimentalist/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/src/autora/experimentalist/extrapolation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-27 17:30:37.000000 autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-27 17:30:37.000000 autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:30:37.000000 autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 17:30:37.000000 autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 17:30:37.000000 autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:30:37.454846 autora_experimentalist_extrapolation-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-27 17:30:32.000000 autora_experimentalist_extrapolation-0.0.8/tests/test_extrapolation.py
```

### Comparing `autora_experimentalist_extrapolation-0.0.7/.github/pull_request_template.md` & `autora_experimentalist_extrapolation-0.0.8/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/.github/workflows/python-publish.yml` & `autora_experimentalist_extrapolation-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/.gitignore` & `autora_experimentalist_extrapolation-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/LICENSE` & `autora_experimentalist_extrapolation-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.7
+Version: 0.0.8
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.7/README.md` & `autora_experimentalist_extrapolation-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/docs/Basic Usage.ipynb` & `autora_experimentalist_extrapolation-0.0.8/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/docs/index.md` & `autora_experimentalist_extrapolation-0.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/mkdocs/base.yml` & `autora_experimentalist_extrapolation-0.0.8/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/pyproject.toml` & `autora_experimentalist_extrapolation-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/src/autora/experimentalist/extrapolation/__init__.py` & `autora_experimentalist_extrapolation-0.0.8/src/autora/experimentalist/extrapolation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             np.isnan(y_r).any()
             or np.isnan(y_c).any()
             or np.isinf(y_r).any()
             or np.isinf(y_c).any()
         ):
             d_y = 0
         else:
-            d_y = dist.pairwise([y_r], [[y_c]])[0]
+            d_y = dist.pairwise([y_r], [y_c])[0]
             if d_y < threshold_y:
                 d_y = 0
         d_x = dist.pairwise([x_r], [x_c])[0]
         if d_x < threshold_x:
             d_x = 0
 
         d_y = np.round(d_y, precision)
```

### Comparing `autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO` & `autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-extrapolation
-Version: 0.0.7
+Version: 0.0.8
 Summary: AutoRA Extrapolation Experimentalist
 Author-email: Younes Strittmatter <younes_strittmatter@brown.edu>
 License: Copyright (c) 2024 Younes Strittmatter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `autora_experimentalist_extrapolation-0.0.7/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt` & `autora_experimentalist_extrapolation-0.0.8/src/autora_experimentalist_extrapolation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora_experimentalist_extrapolation-0.0.7/tests/README.md` & `autora_experimentalist_extrapolation-0.0.8/tests/README.md`

 * *Files identical despite different names*

