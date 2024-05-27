# Comparing `tmp/lckytools-0.0.0b4.tar.gz` & `tmp/lckytools-0.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0b4.tar", max compression
+gzip compressed data, was "lckytools-0.0.0b5.tar", max compression
```

## Comparing `lckytools-0.0.0b4.tar` & `lckytools-0.0.0b5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1096 2024-05-27 01:00:50.888092 lckytools-0.0.0b4/LICENSE
--rw-r--r--   0        0        0     1238 2024-05-27 01:45:51.183441 lckytools-0.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0b4/README.md
--rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b4/src/lckytools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b4/src/lckytools/NN/__init__.py
--rw-r--r--   0        0        0       71 2024-05-27 01:45:34.829772 lckytools-0.0.0b4/src/lckytools/NN/metrics/__init__.py
--rw-r--r--   0        0        0      794 2024-05-27 01:33:41.944308 lckytools-0.0.0b4/src/lckytools/NN/metrics/confusion_matrix.py
--rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b4/src/lckytools/NN/torch/__init__.py
--rw-r--r--   0        0        0       34 2024-05-27 01:45:10.349737 lckytools-0.0.0b4/src/lckytools/NN/torch/summary_model.py
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 lckytools-0.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-27 01:00:50.888092 lckytools-0.0.0b5/LICENSE
+-rw-r--r--   0        0        0     1238 2024-05-27 01:48:01.858425 lckytools-0.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0b5/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 00:52:12.425121 lckytools-0.0.0b5/src/lckytools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b5/src/lckytools/NN/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:47:43.559396 lckytools-0.0.0b5/src/lckytools/NN/metrics/__init__.py
+-rw-r--r--   0        0        0      794 2024-05-27 01:33:41.944308 lckytools-0.0.0b5/src/lckytools/NN/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0b5/src/lckytools/NN/torch/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-27 01:45:10.349737 lckytools-0.0.0b5/src/lckytools/NN/torch/summary_model.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 lckytools-0.0.0b5/PKG-INFO
```

### Comparing `lckytools-0.0.0b4/LICENSE` & `lckytools-0.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0b4/pyproject.toml` & `lckytools-0.0.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lckytools"
-version = "0.0.0b4"
+version = "0.0.0b5"
 description = "A collection of helpful utility functions and tools."
 authors = ["Your Name <your.email@example.com>"]
 license = "MIT"
 
 readme = "README.md"
 homepage = "https://github.com/yourusername/lckytools"
 repository = "https://github.com/yourusername/lckytools"
```

### Comparing `lckytools-0.0.0b4/README.md` & `lckytools-0.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0b4/src/lckytools/NN/metrics/confusion_matrix.py` & `lckytools-0.0.0b5/src/lckytools/NN/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0b4/PKG-INFO` & `lckytools-0.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0b4
+Version: 0.0.0b5
 Summary: A collection of helpful utility functions and tools.
 Home-page: https://github.com/yourusername/lckytools
 License: MIT
 Author: Your Name
 Author-email: your.email@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

