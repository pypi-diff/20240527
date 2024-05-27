# Comparing `tmp/dtw_python-1.5.0.tar.gz` & `tmp/dtw_python-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtw_python-1.5.0.tar", last modified: Thu May 23 22:25:25 2024, max compression
+gzip compressed data, was "dtw_python-1.5.1.tar", last modified: Mon May 27 10:01:34 2024, max compression
```

## Comparing `dtw_python-1.5.0.tar` & `dtw_python-1.5.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.694884 dtw_python-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 22:25:18.000000 dtw_python-1.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-05-23 22:25:18.000000 dtw_python-1.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-23 22:25:18.000000 dtw_python-1.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 22:25:18.000000 dtw_python-1.5.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 22:25:18.000000 dtw_python-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    48135 2024-05-23 22:25:25.694884 dtw_python-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-23 22:25:18.000000 dtw_python-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.686884 dtw_python-1.5.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7350 2024-05-23 22:25:18.000000 dtw_python-1.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.690884 dtw_python-1.5.0/dtw/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/_backtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)  1229066 2024-05-23 22:25:24.000000 dtw_python-1.5.0/dtw/_dtw_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/_dtw_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/_globalCostMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/countPaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.690884 dtw_python-1.5.0/dtw/data/
--rw-r--r--   0 runner    (1001) docker     (127)   250698 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/data/aami3a.csv
--rw-r--r--   0 runner    (1001) docker     (127)   252781 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/data/aami3b.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtwPlot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw_core.c
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/mvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    26005 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/stepPattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/warpArea.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.694884 dtw_python-1.5.0/dtw_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    48135 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.690884 dtw_python-1.5.0/maintainer/
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-23 22:25:18.000000 dtw_python-1.5.0/maintainer/roxypick.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-23 22:25:18.000000 dtw_python-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 22:25:25.694884 dtw_python-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-23 22:25:18.000000 dtw_python-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.694884 dtw_python-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/query.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/reference.csv
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_countPaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_cran.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_dtw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_dtw_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:01:34.969237 dtw_python-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-27 10:01:27.000000 dtw_python-1.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-27 10:01:27.000000 dtw_python-1.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-27 10:01:27.000000 dtw_python-1.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 10:01:27.000000 dtw_python-1.5.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-27 10:01:27.000000 dtw_python-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    48135 2024-05-27 10:01:34.969237 dtw_python-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-27 10:01:27.000000 dtw_python-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:01:34.961237 dtw_python-1.5.1/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7350 2024-05-27 10:01:27.000000 dtw_python-1.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:01:34.965237 dtw_python-1.5.1/dtw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/_backtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1229066 2024-05-27 10:01:34.000000 dtw_python-1.5.1/dtw/_dtw_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/_dtw_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/_globalCostMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/countPaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:01:34.965237 dtw_python-1.5.1/dtw/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   250698 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/data/aami3a.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   252781 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/data/aami3b.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/dtw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/dtwPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/dtw_core.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/dtw_core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/dtw_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/mvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26005 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/stepPattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/warpArea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-27 10:01:27.000000 dtw_python-1.5.1/dtw/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:01:34.969237 dtw_python-1.5.1/dtw_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    48135 2024-05-27 10:01:34.000000 dtw_python-1.5.1/dtw_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-27 10:01:34.000000 dtw_python-1.5.1/dtw_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:01:34.000000 dtw_python-1.5.1/dtw_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 10:01:34.000000 dtw_python-1.5.1/dtw_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:01:33.000000 dtw_python-1.5.1/dtw_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 10:01:34.000000 dtw_python-1.5.1/dtw_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 10:01:34.000000 dtw_python-1.5.1/dtw_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:01:34.965237 dtw_python-1.5.1/maintainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-27 10:01:27.000000 dtw_python-1.5.1/maintainer/roxypick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-27 10:01:27.000000 dtw_python-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-27 10:01:34.969237 dtw_python-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-27 10:01:27.000000 dtw_python-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:01:34.969237 dtw_python-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/query.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/reference.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/test_countPaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/test_cran.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/test_dtw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/test_dtw_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-27 10:01:27.000000 dtw_python-1.5.1/tests/test_issues.py
```

### Comparing `dtw_python-1.5.0/CHANGELOG.md` & `dtw_python-1.5.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,39 @@
 Changelog
 =========
 
 
-(unreleased)
-------------
+v1.5.0 (2024-05-23)
+-------------------
+- Modernize build and    attempt to numpy 2. [Toni]
+- Merge pull request #93 from
+  DynamicTimeWarping/dependabot/github_actions/pypa/cibuildwheel-2.18.1.
+  [Toni G]
+
+  Bump pypa/cibuildwheel from 2.17.0 to 2.18.1
+- --- updated-dependencies: - dependency-name: pypa/cibuildwheel
+  dependency-type: direct:production   update-type: version-
+  update:semver-minor ... [dependabot[bot]]
+- No inh diag. [Toni]
+
+
+v1.4.4 (2024-05-18)
+-------------------
+- Update cython 3. [Toni]
+
+
+v1.4.3 (2024-05-18)
+-------------------
+- Fix test for numpy2. [Toni]
+- List new Python versions. [Toni]
+
+
+v1.4.2 (2024-03-19)
+-------------------
+- Changelog. [Toni]
 - Update build_wheels.yml. [Toni G]
 
 
 v1.4.1 (2024-03-18)
 -------------------
 - Update build_wheels.yml. [Toni G]
 - Update build_wheels.yml. [Toni G]
```

### Comparing `dtw_python-1.5.0/CONTRIBUTING.rst` & `dtw_python-1.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/COPYING` & `dtw_python-1.5.1/COPYING`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/PKG-INFO` & `dtw_python-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtw-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: A comprehensive implementation of dynamic time warping (DTW) algorithms.
 Home-page: https://DynamicTimeWarping.github.io
 Author-email: Toni Giorgino <toni.giorgino@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dtw_python-1.5.0/README.rst` & `dtw_python-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/docs/conf.py` & `dtw_python-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/__init__.py` & `dtw_python-1.5.1/dtw/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Please see the help for the dtw.dtw() function which is the package's
 main entry point.
 
 """
 
 __author__ = """Toni Giorgino"""
 __email__ = 'toni.giorgino@gmail.com'
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 
 # There are no comments in this package because it mirrors closely the R sources.
 
 # List of things to export on "from dtw import *"
 from dtw.dtw import *
 from dtw.stepPattern import *
 from dtw.countPaths import *
```

### Comparing `dtw_python-1.5.0/dtw/__main__.py` & `dtw_python-1.5.1/dtw/__main__.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/_backtrack.py` & `dtw_python-1.5.1/dtw/_backtrack.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/_dtw_utils.c` & `dtw_python-1.5.1/dtw/_dtw_utils.c`

 * *Files 1% similar despite different names*

```diff
@@ -1697,159 +1697,159 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":770
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  * ctypedef double complex complex128_t
  * 
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * ctypedef npy_longlong   longlong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":795
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":795
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":798
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":798
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":799
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":799
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":800
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":800
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef float complex       cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1924,24 +1924,24 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1096
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1096
  * 
  * # Iterator API added in v1.6
  * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil             # <<<<<<<<<<<<<<
  * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil
  * 
  */
 typedef int (*__pyx_t_5numpy_NpyIter_IterNextFunc)(NpyIter *);
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1097
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1097
  * # Iterator API added in v1.6
  * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil
  * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "numpy/arrayobject.h":
  */
 typedef void (*__pyx_t_5numpy_NpyIter_GetMultiIndexFunc)(NpyIter *, npy_intp *);
@@ -18516,685 +18516,685 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
  * 
  *         @property
  *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ELSIZE(self)
  * 
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":287
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":287
  *         @property
  *         cdef inline npy_intp itemsize(self) noexcept nogil:
  *             return PyDataType_ELSIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyDataType_ELSIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
  * 
  *         @property
  *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ELSIZE(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  * 
  *         @property
  *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ALIGNMENT(self)
  * 
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
  *         @property
  *         cdef inline npy_intp alignment(self) noexcept nogil:
  *             return PyDataType_ALIGNMENT(self)             # <<<<<<<<<<<<<<
  * 
  *         # Use fields/names with care as they may be NULL.  You must check
  */
   __pyx_r = PyDataType_ALIGNMENT(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  * 
  *         @property
  *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_ALIGNMENT(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
  *         # for this using PyDataType_HASFIELDS.
  *         @property
  *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
  *             return <object>PyDataType_FIELDS(self)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
   __Pyx_RefNannySetupContext("fields", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":297
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":297
  *         @property
  *         cdef inline object fields(self):
  *             return <object>PyDataType_FIELDS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyDataType_FIELDS(__pyx_v_self);
   __Pyx_INCREF(((PyObject *)__pyx_t_1));
   __pyx_r = ((PyObject *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
  *         # for this using PyDataType_HASFIELDS.
  *         @property
  *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
  *             return <object>PyDataType_FIELDS(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
  * 
  *         @property
  *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
  *             return <tuple>PyDataType_NAMES(self)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1;
   __Pyx_RefNannySetupContext("names", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":301
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":301
  *         @property
  *         cdef inline tuple names(self):
  *             return <tuple>PyDataType_NAMES(self)             # <<<<<<<<<<<<<<
  * 
  *         # Use PyDataType_HASSUBARRAY to test whether this field is
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyDataType_NAMES(__pyx_v_self);
   __Pyx_INCREF(((PyObject*)__pyx_t_1));
   __pyx_r = ((PyObject*)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
  * 
  *         @property
  *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
  *             return <tuple>PyDataType_NAMES(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
  *         # this field via the inline helper method PyDataType_SHAPE.
  *         @property
  *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_SUBARRAY(self)
  * 
  */
 
 static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self) {
   PyArray_ArrayDescr *__pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":308
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":308
  *         @property
  *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:
  *             return PyDataType_SUBARRAY(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyDataType_SUBARRAY(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
  *         # this field via the inline helper method PyDataType_SHAPE.
  *         @property
  *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             return PyDataType_SUBARRAY(self)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
  * 
  *         @property
  *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The data types flags."""
  *             return PyDataType_FLAGS(self)
  */
 
 static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self) {
   npy_uint64 __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":313
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":313
  *         cdef inline npy_uint64 flags(self) noexcept nogil:
  *             """The data types flags."""
  *             return PyDataType_FLAGS(self)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyDataType_FLAGS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
  * 
  *         @property
  *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The data types flags."""
  *             return PyDataType_FLAGS(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
  * 
  *         @property
  *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of arrays that need to be broadcast to the same shape."""
  *             return PyArray_MultiIter_NUMITER(self)
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":325
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":325
  *         cdef inline int numiter(self) noexcept nogil:
  *             """The number of arrays that need to be broadcast to the same shape."""
  *             return PyArray_MultiIter_NUMITER(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_NUMITER(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
  * 
  *         @property
  *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of arrays that need to be broadcast to the same shape."""
  *             return PyArray_MultiIter_NUMITER(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The total broadcasted size."""
  *             return PyArray_MultiIter_SIZE(self)
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":330
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":330
  *         cdef inline npy_intp size(self) noexcept nogil:
  *             """The total broadcasted size."""
  *             return PyArray_MultiIter_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The total broadcasted size."""
  *             return PyArray_MultiIter_SIZE(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
  * 
  *         @property
  *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The current (1-d) index into the broadcasted result."""
  *             return PyArray_MultiIter_INDEX(self)
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":335
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":335
  *         cdef inline npy_intp index(self) noexcept nogil:
  *             """The current (1-d) index into the broadcasted result."""
  *             return PyArray_MultiIter_INDEX(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_INDEX(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
  * 
  *         @property
  *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The current (1-d) index into the broadcasted result."""
  *             return PyArray_MultiIter_INDEX(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
  * 
  *         @property
  *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of dimensions in the broadcasted result."""
  *             return PyArray_MultiIter_NDIM(self)
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":340
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":340
  *         cdef inline int nd(self) noexcept nogil:
  *             """The number of dimensions in the broadcasted result."""
  *             return PyArray_MultiIter_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
  * 
  *         @property
  *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The number of dimensions in the broadcasted result."""
  *             return PyArray_MultiIter_NDIM(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
  * 
  *         @property
  *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The shape of the broadcasted result."""
  *             return PyArray_MultiIter_DIMS(self)
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":345
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":345
  *         cdef inline npy_intp* dimensions(self) noexcept nogil:
  *             """The shape of the broadcasted result."""
  *             return PyArray_MultiIter_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_MultiIter_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
  * 
  *         @property
  *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The shape of the broadcasted result."""
  *             return PyArray_MultiIter_DIMS(self)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
  * 
  *         @property
  *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
  *             On return, the iterators are adjusted for broadcasting."""
  */
 
 static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self) {
   void **__pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":351
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":351
  *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
  *             On return, the iterators are adjusted for broadcasting."""
  *             return PyArray_MultiIter_ITERS(self)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyArray_MultiIter_ITERS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
  * 
  *         @property
  *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
  *             On return, the iterators are adjusted for broadcasting."""
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
  *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":369
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":369
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
  *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":375
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":375
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
  *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":381
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":381
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
  *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":389
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":389
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":396
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":396
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":402
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":402
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
  *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
  *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":411
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":411
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
  *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
  * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19203,29 +19203,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":808
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":808
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
  * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19236,15 +19236,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19253,29 +19253,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":811
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":811
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19286,15 +19286,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19303,29 +19303,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":814
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":814
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 814, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19336,15 +19336,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19353,29 +19353,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":817
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":817
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19386,15 +19386,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19403,29 +19403,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":820
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":820
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19436,219 +19436,219 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":824
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":824
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __pyx_f_5numpy_5dtype_8subarray_subarray(__pyx_v_d)->shape;
     __Pyx_INCREF(((PyObject*)__pyx_t_2));
     __pyx_r = ((PyObject*)__pyx_t_2);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":826
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":826
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  * 
  * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1012
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1012
  * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 1012, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1015
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1015
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1018
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1018
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19664,15 +19664,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19680,68 +19680,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1024
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1024
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy._core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1024, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1025, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1026, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1026, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19749,15 +19749,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19772,15 +19772,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19796,15 +19796,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19812,68 +19812,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1030
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1030
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1030, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1031
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1031
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1031, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1032, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1032, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19881,15 +19881,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19904,15 +19904,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19928,15 +19928,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19944,68 +19944,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1036, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1037
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1037
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1037, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+      /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1038, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+    /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20013,15 +20013,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
  *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20036,172 +20036,172 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1068
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1068
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1078
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1078
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1085
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1085
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
+/* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1092
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1092
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23585,26 +23585,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 1026, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../tmp/build-env-r6pau4w0/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_umath_failed_to_impo); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 1032, __pyx_L1_error)
```

### Comparing `dtw_python-1.5.0/dtw/_dtw_utils.pyx` & `dtw_python-1.5.1/dtw/_dtw_utils.pyx`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/_globalCostMatrix.py` & `dtw_python-1.5.1/dtw/_globalCostMatrix.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/countPaths.py` & `dtw_python-1.5.1/dtw/countPaths.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/data/aami3a.csv` & `dtw_python-1.5.1/dtw/data/aami3a.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/data/aami3b.csv` & `dtw_python-1.5.1/dtw/data/aami3b.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/dtw.py` & `dtw_python-1.5.1/dtw/dtw.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/dtwPlot.py` & `dtw_python-1.5.1/dtw/dtwPlot.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/dtw_core.c` & `dtw_python-1.5.1/dtw/dtw_core.c`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/dtw_core.h` & `dtw_python-1.5.1/dtw/dtw_core.h`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/dtw_test_data.py` & `dtw_python-1.5.1/dtw/dtw_test_data.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/mvm.py` & `dtw_python-1.5.1/dtw/mvm.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/stepPattern.py` & `dtw_python-1.5.1/dtw/stepPattern.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/warp.py` & `dtw_python-1.5.1/dtw/warp.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/warpArea.py` & `dtw_python-1.5.1/dtw/warpArea.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw/window.py` & `dtw_python-1.5.1/dtw/window.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/dtw_python.egg-info/PKG-INFO` & `dtw_python-1.5.1/dtw_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtw-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: A comprehensive implementation of dynamic time warping (DTW) algorithms.
 Home-page: https://DynamicTimeWarping.github.io
 Author-email: Toni Giorgino <toni.giorgino@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `dtw_python-1.5.0/dtw_python.egg-info/SOURCES.txt` & `dtw_python-1.5.1/dtw_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/maintainer/roxypick.py` & `dtw_python-1.5.1/maintainer/roxypick.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/pyproject.toml` & `dtw_python-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/setup.py` & `dtw_python-1.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 from setuptools.extension import Extension
 from Cython.Build import cythonize
 import numpy
 
 
 setup(
     include_package_data=True,
-    name='dtw-python',
+    name="dtw-python",
     #    packages=find_packages(include=['dtw']),
-    packages=['dtw'],
+    packages=["dtw"],
     include_dirs=numpy.get_include(),
-    ext_modules=cythonize([Extension('dtw._dtw_utils',
-                 sources=['dtw/_dtw_utils.pyx', 'dtw/dtw_core.c'])]),
-    url='https://DynamicTimeWarping.github.io',
-    version='1.5.0',
+    ext_modules=cythonize(
+        [Extension("dtw._dtw_utils", sources=["dtw/_dtw_utils.pyx", "dtw/dtw_core.c"])],
+        force=True,
+    ),
+    url="https://DynamicTimeWarping.github.io",
+    version="1.5.1",
     zip_safe=False,
 )
```

### Comparing `dtw_python-1.5.0/tests/query.csv` & `dtw_python-1.5.1/tests/query.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/tests/reference.csv` & `dtw_python-1.5.1/tests/reference.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/tests/test_cli.py` & `dtw_python-1.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/tests/test_countPaths.py` & `dtw_python-1.5.1/tests/test_countPaths.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/tests/test_cran.py` & `dtw_python-1.5.1/tests/test_cran.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/tests/test_dtw.py` & `dtw_python-1.5.1/tests/test_dtw.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/tests/test_dtw_s.py` & `dtw_python-1.5.1/tests/test_dtw_s.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.5.0/tests/test_issues.py` & `dtw_python-1.5.1/tests/test_issues.py`

 * *Files identical despite different names*

