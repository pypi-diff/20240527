# Comparing `tmp/coveo_testing_extras-2.1.8.tar.gz` & `tmp/coveo_testing_extras-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo_testing_extras-2.1.8.tar", max compression
+gzip compressed data, was "coveo_testing_extras-2.1.9.tar", max compression
```

## Comparing `coveo_testing_extras-2.1.8.tar` & `coveo_testing_extras-2.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1709 2023-10-27 13:49:45.482792 coveo_testing_extras-2.1.8/README.md
--rw-r--r--   0        0        0        0 2023-10-27 13:49:45.482792 coveo_testing_extras-2.1.8/coveo_testing_extras/__init__.py
--rw-r--r--   0        0        0        0 2023-10-27 13:49:45.482792 coveo_testing_extras-2.1.8/coveo_testing_extras/py.typed
--rw-r--r--   0        0        0        0 2023-10-27 13:49:45.482792 coveo_testing_extras-2.1.8/coveo_testing_extras/temporary_resource/__init__.py
--rw-r--r--   0        0        0    10759 2023-10-27 13:49:45.482792 coveo_testing_extras-2.1.8/coveo_testing_extras/temporary_resource/docker_container.py
--rw-r--r--   0        0        0     1033 2023-10-27 13:50:18.912181 coveo_testing_extras-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 coveo_testing_extras-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1709 2023-10-27 17:50:36.668690 coveo_testing_extras-2.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-10-27 17:50:36.668690 coveo_testing_extras-2.1.9/coveo_testing_extras/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-27 17:50:36.668690 coveo_testing_extras-2.1.9/coveo_testing_extras/py.typed
+-rw-r--r--   0        0        0        0 2023-10-27 17:50:36.668690 coveo_testing_extras-2.1.9/coveo_testing_extras/temporary_resource/__init__.py
+-rw-r--r--   0        0        0    10759 2023-10-27 17:50:36.668690 coveo_testing_extras-2.1.9/coveo_testing_extras/temporary_resource/docker_container.py
+-rw-r--r--   0        0        0     1033 2023-10-27 17:51:08.529293 coveo_testing_extras-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 coveo_testing_extras-2.1.9/PKG-INFO
```

### Comparing `coveo_testing_extras-2.1.8/README.md` & `coveo_testing_extras-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `coveo_testing_extras-2.1.8/coveo_testing_extras/temporary_resource/docker_container.py` & `coveo_testing_extras-2.1.9/coveo_testing_extras/temporary_resource/docker_container.py`

 * *Files identical despite different names*

### Comparing `coveo_testing_extras-2.1.8/pyproject.toml` & `coveo_testing_extras-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveo-testing-extras"
-version = "2.1.8"
+version = "2.1.9"
 description = "Dependency-hungry testing helpers"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/coveo-python-oss/tree/main/coveo-testing-extras"
 authors = ["Jonathan Piché <tools@coveo.com>"]
 
 [tool.poetry.dependencies]
```

### Comparing `coveo_testing_extras-2.1.8/PKG-INFO` & `coveo_testing_extras-2.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveo-testing-extras
-Version: 2.1.8
+Version: 2.1.9
 Summary: Dependency-hungry testing helpers
 Home-page: https://github.com/coveooss/coveo-python-oss/tree/main/coveo-testing-extras
 License: Apache-2.0
 Author: Jonathan Piché
 Author-email: tools@coveo.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

