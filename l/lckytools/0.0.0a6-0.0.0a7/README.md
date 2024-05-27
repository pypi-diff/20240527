# Comparing `tmp/lckytools-0.0.0a6.tar.gz` & `tmp/lckytools-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0a6.tar", max compression
+gzip compressed data, was "lckytools-0.0.0a7.tar", max compression
```

## Comparing `lckytools-0.0.0a6.tar` & `lckytools-0.0.0a7.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     1096 2024-05-27 03:04:13.567796 lckytools-0.0.0a6/LICENSE
--rw-r--r--   0        0        0      516 2024-05-27 04:00:52.639676 lckytools-0.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a6/README.md
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a6/src/lckytools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a6/src/lckytools/core/__init__.py
--rw-r--r--   0        0        0       42 2024-05-27 03:49:27.940843 lckytools-0.0.0a6/src/lckytools/core/hello.py
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a6/src/lckytools.ai/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 02:49:11.736063 lckytools-0.0.0a6/src/lckytools.ai/ai/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 02:49:12.032838 lckytools-0.0.0a6/src/lckytools.ai/ai/metrics/__init__.py
--rw-r--r--   0        0        0      911 2024-05-27 03:07:44.681865 lckytools-0.0.0a6/src/lckytools.ai/ai/metrics/confusion_matrix.py
--rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 lckytools-0.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-27 03:04:13.567796 lckytools-0.0.0a7/LICENSE
+-rw-r--r--   0        0        0      516 2024-05-27 04:14:05.726123 lckytools-0.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a7/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a7/src/lckytools/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-27 03:49:27.940843 lckytools-0.0.0a7/src/lckytools/hello.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a7/src/lckytools.ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:49:12.032838 lckytools-0.0.0a7/src/lckytools.ai/metrics/__init__.py
+-rw-r--r--   0        0        0      911 2024-05-27 03:07:44.681865 lckytools-0.0.0a7/src/lckytools.ai/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 lckytools-0.0.0a7/PKG-INFO
```

### Comparing `lckytools-0.0.0a6/LICENSE` & `lckytools-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a6/pyproject.toml` & `lckytools-0.0.0a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lckytools"
-version = "0.0.0a6"
+version = "0.0.0a7"
 description = ""
 authors = ["LCKYN <T.Pawarit@lckyn.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "lckytools", from = "src" },
```

### Comparing `lckytools-0.0.0a6/README.md` & `lckytools-0.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a6/src/lckytools.ai/ai/metrics/confusion_matrix.py` & `lckytools-0.0.0a7/src/lckytools.ai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a6/PKG-INFO` & `lckytools-0.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: 
 License: MIT
 Author: LCKYN
 Author-email: T.Pawarit@lckyn.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

