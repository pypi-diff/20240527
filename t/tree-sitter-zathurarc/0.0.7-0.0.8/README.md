# Comparing `tmp/tree-sitter-zathurarc-0.0.7.tar.gz` & `tmp/tree_sitter_zathurarc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-sitter-zathurarc-0.0.7.tar", last modified: Tue Mar 26 16:10:28 2024, max compression
+gzip compressed data, was "tree_sitter_zathurarc-0.0.8.tar", last modified: Mon May 27 13:12:01 2024, max compression
```

## Comparing `tree-sitter-zathurarc-0.0.7.tar` & `tree_sitter_zathurarc-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:10:28.459851 tree-sitter-zathurarc-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-03-26 16:10:28.459851 tree-sitter-zathurarc-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:10:28.455851 tree-sitter-zathurarc-0.0.7/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:10:28.455851 tree-sitter-zathurarc-0.0.7/bindings/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:10:28.459851 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc/binding.c
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:10:28.459851 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-03-26 16:10:28.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-26 16:10:28.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:10:28.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:10:28.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 16:10:28.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 16:10:28.000000 tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:10:28.459851 tree-sitter-zathurarc-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:10:28.459851 tree-sitter-zathurarc-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)    45100 2024-03-26 16:10:24.000000 tree-sitter-zathurarc-0.0.7/src/parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:12:01.205868 tree_sitter_zathurarc-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-27 13:12:01.205868 tree_sitter_zathurarc-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:12:01.201868 tree_sitter_zathurarc-0.0.8/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:12:01.201868 tree_sitter_zathurarc-0.0.8/bindings/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:12:01.205868 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc/binding.c
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:12:01.205868 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-27 13:12:01.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-27 13:12:01.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:12:01.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:12:00.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-27 13:12:01.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 13:12:01.000000 tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:12:01.205868 tree_sitter_zathurarc-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:12:01.205868 tree_sitter_zathurarc-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    45100 2024-05-27 13:11:57.000000 tree_sitter_zathurarc-0.0.8/src/parser.c
```

### Comparing `tree-sitter-zathurarc-0.0.7/PKG-INFO` & `tree_sitter_zathurarc-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-zathurarc
-Version: 0.0.7
+Version: 0.0.8
 Summary: Zathurarc grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-zathurarc
 Keywords: incremental,parsing,tree-sitter,zathurarc
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

### Comparing `tree-sitter-zathurarc-0.0.7/README.md` & `tree_sitter_zathurarc-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc/binding.c` & `tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc/binding.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/PKG-INFO` & `tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-zathurarc
-Version: 0.0.7
+Version: 0.0.8
 Summary: Zathurarc grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-zathurarc
 Keywords: incremental,parsing,tree-sitter,zathurarc
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

### Comparing `tree-sitter-zathurarc-0.0.7/bindings/python/tree_sitter_zathurarc.egg-info/SOURCES.txt` & `tree_sitter_zathurarc-0.0.8/bindings/python/tree_sitter_zathurarc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tree-sitter-zathurarc-0.0.7/pyproject.toml` & `tree_sitter_zathurarc-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tree-sitter-zathurarc"
 description = "Zathurarc grammar for tree-sitter"
-version = "0.0.7"
+version = "0.0.8"
 keywords = ["incremental", "parsing", "tree-sitter", "zathurarc"]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Topic :: Software Development :: Compilers",
   "Topic :: Text Processing :: Linguistic",
   "Typing :: Typed"
```

### Comparing `tree-sitter-zathurarc-0.0.7/setup.py` & `tree_sitter_zathurarc-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `tree-sitter-zathurarc-0.0.7/src/parser.c` & `tree_sitter_zathurarc-0.0.8/src/parser.c`

 * *Files identical despite different names*

