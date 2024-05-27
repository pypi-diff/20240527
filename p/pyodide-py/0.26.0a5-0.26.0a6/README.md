# Comparing `tmp/pyodide_py-0.26.0a5.tar.gz` & `tmp/pyodide_py-0.26.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_py-0.26.0a5.tar", last modified: Tue May 21 20:08:13 2024, max compression
+gzip compressed data, was "pyodide_py-0.26.0a6.tar", last modified: Wed May 22 01:46:29 2024, max compression
```

## Comparing `pyodide_py-0.26.0a5.tar` & `pyodide_py-0.26.0a6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.702667 pyodide_py-0.26.0a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-21 20:08:13.702667 pyodide_py-0.26.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/_pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19878 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    49263 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/_core_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/docs_argspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/jsbind.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_package_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_run_js.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/code.py
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/pyodide/ffi/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/ffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/ffi/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/http.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21376 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/webloop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/pyodide_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:08:13.702667 pyodide_py-0.26.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:46:29.194260 pyodide_py-0.26.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-22 01:46:29.194260 pyodide_py-0.26.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:46:29.194260 pyodide_py-0.26.0a6/_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19878 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49263 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/_core_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/docs_argspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/jsbind.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/_pyodide/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:46:29.194260 pyodide_py-0.26.0a6/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/_package_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/_run_js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:46:29.194260 pyodide_py-0.26.0a6/pyodide/ffi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/ffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/ffi/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21376 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyodide/webloop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:46:29.194260 pyodide_py-0.26.0a6/pyodide_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-22 01:46:29.000000 pyodide_py-0.26.0a6/pyodide_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-22 01:46:29.000000 pyodide_py-0.26.0a6/pyodide_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:46:29.000000 pyodide_py-0.26.0a6/pyodide_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 01:46:29.000000 pyodide_py-0.26.0a6/pyodide_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:46:29.194260 pyodide_py-0.26.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-22 01:46:16.000000 pyodide_py-0.26.0a6/webbrowser.py
```

### Comparing `pyodide_py-0.26.0a5/PKG-INFO` & `pyodide_py-0.26.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.26.0a5
+Version: 0.26.0a6
 Summary: A Python package providing core interpreter functionality for Pyodide
 Author: Pyodide developers
 Project-URL: Homepage, https://github.com/pyodide/pyodide
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide_py-0.26.0a5/README.md` & `pyodide_py-0.26.0a6/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/_pyodide/__init__.py` & `pyodide_py-0.26.0a6/_pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/_pyodide/_base.py` & `pyodide_py-0.26.0a6/_pyodide/_base.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/_pyodide/_core_docs.py` & `pyodide_py-0.26.0a6/_pyodide/_core_docs.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/_pyodide/_importhook.py` & `pyodide_py-0.26.0a6/_pyodide/_importhook.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/_pyodide/docs_argspec.py` & `pyodide_py-0.26.0a6/_pyodide/docs_argspec.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/_pyodide/docstring.py` & `pyodide_py-0.26.0a6/_pyodide/docstring.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/_pyodide/jsbind.py` & `pyodide_py-0.26.0a6/_pyodide/jsbind.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/__init__.py` & `pyodide_py-0.26.0a6/pyodide/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # All pure Python code that does not require js or pyodide_js should go in
 # the _pyodide package.
 #
 # This package is imported by the test suite as well, and currently we don't use
 # pytest mocks for js or pyodide_js, so make sure to test "if IN_BROWSER" before
 # importing from these.
-__version__ = "0.26.0a5"
+__version__ = "0.26.0a6"
 
 __all__ = ["__version__", "console", "code", "ffi", "http", "webloop"]
 
 from . import _state  # noqa: F401
 from .webloop import _initialize_event_loop
 
 _initialize_event_loop()
```

### Comparing `pyodide_py-0.26.0a5/pyodide/_package_loader.py` & `pyodide_py-0.26.0a6/pyodide/_package_loader.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/_state.py` & `pyodide_py-0.26.0a6/pyodide/_state.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/code.py` & `pyodide_py-0.26.0a6/pyodide/code.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/console.py` & `pyodide_py-0.26.0a6/pyodide/console.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/ffi/__init__.py` & `pyodide_py-0.26.0a6/pyodide/ffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/ffi/wrappers.py` & `pyodide_py-0.26.0a6/pyodide/ffi/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/http.py` & `pyodide_py-0.26.0a6/pyodide/http.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide/webloop.py` & `pyodide_py-0.26.0a6/pyodide/webloop.py`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyodide_py.egg-info/PKG-INFO` & `pyodide_py-0.26.0a6/pyodide_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.26.0a5
+Version: 0.26.0a6
 Summary: A Python package providing core interpreter functionality for Pyodide
 Author: Pyodide developers
 Project-URL: Homepage, https://github.com/pyodide/pyodide
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide_py-0.26.0a5/pyodide_py.egg-info/SOURCES.txt` & `pyodide_py-0.26.0a6/pyodide_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodide_py-0.26.0a5/pyproject.toml` & `pyodide_py-0.26.0a6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyodide-py"
-version = "0.26.0a5"
+version = "0.26.0a6"
 authors = [{name = "Pyodide developers"}]
 description = "A Python package providing core interpreter functionality for Pyodide"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: OS Independent",
 ]
```

