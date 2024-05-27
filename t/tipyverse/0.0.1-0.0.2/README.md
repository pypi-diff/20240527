# Comparing `tmp/tipyverse-0.0.1.tar.gz` & `tmp/tipyverse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipyverse-0.0.1.tar", last modified: Thu May 23 16:05:14 2024, max compression
+gzip compressed data, was "tipyverse-0.0.2.tar", last modified: Mon May 27 06:33:26 2024, max compression
```

## Comparing `tipyverse-0.0.1.tar` & `tipyverse-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:05:14.050568 tipyverse-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 16:05:09.000000 tipyverse-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-23 16:05:14.050568 tipyverse-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-23 16:05:09.000000 tipyverse-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 16:05:09.000000 tipyverse-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:05:14.050568 tipyverse-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:05:14.046568 tipyverse-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:05:14.046568 tipyverse-0.0.1/src/tipyverse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:05:09.000000 tipyverse-0.0.1/src/tipyverse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:05:14.050568 tipyverse-0.0.1/src/tipyverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-23 16:05:14.000000 tipyverse-0.0.1/src/tipyverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-23 16:05:14.000000 tipyverse-0.0.1/src/tipyverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:05:14.000000 tipyverse-0.0.1/src/tipyverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 16:05:14.000000 tipyverse-0.0.1/src/tipyverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 16:05:14.000000 tipyverse-0.0.1/src/tipyverse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.956269 tipyverse-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 06:33:22.000000 tipyverse-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 06:33:26.956269 tipyverse-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 06:33:22.000000 tipyverse-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-27 06:33:22.000000 tipyverse-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:33:26.956269 tipyverse-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.952269 tipyverse-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.952269 tipyverse-0.0.2/src/tipyverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/data_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 06:33:22.000000 tipyverse-0.0.2/src/tipyverse/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.956269 tipyverse-0.0.2/src/tipyverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 06:33:26.000000 tipyverse-0.0.2/src/tipyverse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:26.956269 tipyverse-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_data_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:33:22.000000 tipyverse-0.0.2/tests/test_utilities.py
```

### Comparing `tipyverse-0.0.1/LICENSE` & `tipyverse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tipyverse-0.0.1/PKG-INFO` & `tipyverse-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tipyverse
-Version: 0.0.1
-Summary: A package to install Python equivalents of R Tidyverse packages
+Version: 0.0.2
+Summary: A package to install Python equivalents of R tipyverse packages
 Author-email: Sebastian Dunn <sebastiandunn@sdmdigital.co>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Dunn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/axolmain/Tipyverse
 Project-URL: Issues, https://github.com/axolmain/Tipyverse/issues
 Project-URL: Repository, https://github.com/axolmain/Tipyverse.git
-Keywords: tidyverse,R,data science,python
+Keywords: tipyverse,R,data science,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lets-plot
@@ -61,8 +61,8 @@
 Provides-Extra: notebook
 Requires-Dist: swifter; extra == "notebook"
 Provides-Extra: groupby
 Requires-Dist: swifter; extra == "groupby"
 
 # Example Package
 
-This is a simple package which basically just wraps together as many python packages as I could find which help replicate R's `Tidyverse` package.
+This is a simple package which basically just wraps together as many python packages as I could find which help replicate R's `tipyverse` package.
```

### Comparing `tipyverse-0.0.1/pyproject.toml` & `tipyverse-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tipyverse"
-version = "0.0.1"
-description = "A package to install Python equivalents of R Tidyverse packages"
+version = "0.0.2"
+description = "A package to install Python equivalents of R tipyverse packages"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Sebastian Dunn", email = "sebastiandunn@sdmdigital.co" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -38,15 +38,15 @@
     "plotnine",
     "seaborn",
     "numpy",
     "scipy",
     "statsmodels",
     "altair"
 ]
-keywords = ["tidyverse", "R", "data science", "python"]
+keywords = ["tipyverse", "R", "data science", "python"]
 license = { file = "LICENSE" }
 
 [project.optional-dependencies]
 notebook = ["swifter"]
 groupby = ["swifter"]
 
 [project.urls]
```

### Comparing `tipyverse-0.0.1/src/tipyverse.egg-info/PKG-INFO` & `tipyverse-0.0.2/src/tipyverse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tipyverse
-Version: 0.0.1
-Summary: A package to install Python equivalents of R Tidyverse packages
+Version: 0.0.2
+Summary: A package to install Python equivalents of R tipyverse packages
 Author-email: Sebastian Dunn <sebastiandunn@sdmdigital.co>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Dunn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/axolmain/Tipyverse
 Project-URL: Issues, https://github.com/axolmain/Tipyverse/issues
 Project-URL: Repository, https://github.com/axolmain/Tipyverse.git
-Keywords: tidyverse,R,data science,python
+Keywords: tipyverse,R,data science,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lets-plot
@@ -61,8 +61,8 @@
 Provides-Extra: notebook
 Requires-Dist: swifter; extra == "notebook"
 Provides-Extra: groupby
 Requires-Dist: swifter; extra == "groupby"
 
 # Example Package
 
-This is a simple package which basically just wraps together as many python packages as I could find which help replicate R's `Tidyverse` package.
+This is a simple package which basically just wraps together as many python packages as I could find which help replicate R's `tipyverse` package.
```

