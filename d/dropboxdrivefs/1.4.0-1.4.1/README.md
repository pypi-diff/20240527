# Comparing `tmp/dropboxdrivefs-1.4.0.tar.gz` & `tmp/dropboxdrivefs-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dropboxdrivefs-1.4.0.tar", last modified: Mon May 20 18:59:11 2024, max compression
+gzip compressed data, was "dropboxdrivefs-1.4.1.tar", last modified: Mon May 27 14:04:28 2024, max compression
```

## Comparing `dropboxdrivefs-1.4.0.tar` & `dropboxdrivefs-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/
--rw-rw-r--   0 marine    (1000) marine    (1000)     1528 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.0/LICENSE
--rw-rw-r--   0 marine    (1000) marine    (1000)       35 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.0/MANIFEST.in
--rw-r--r--   0 marine    (1000) marine    (1000)     2221 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/PKG-INFO
--rw-rw-r--   0 marine    (1000) marine    (1000)     1383 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.0/README.md
-drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/dropboxdrivefs/
-drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/
--rw-r--r--   0 marine    (1000) marine    (1000)     2221 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/PKG-INFO
--rw-rw-r--   0 marine    (1000) marine    (1000)      339 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/SOURCES.txt
--rw-rw-r--   0 marine    (1000) marine    (1000)        1 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/dependency_links.txt
--rw-rw-r--   0 marine    (1000) marine    (1000)       24 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/requires.txt
--rw-rw-r--   0 marine    (1000) marine    (1000)        1 2024-05-20 18:59:11.000000 dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/top_level.txt
--rw-rw-r--   0 marine    (1000) marine    (1000)      963 2024-05-20 18:58:57.000000 dropboxdrivefs-1.4.0/pyproject.toml
--rw-rw-r--   0 marine    (1000) marine    (1000)       38 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/setup.cfg
-drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-20 18:59:11.564527 dropboxdrivefs-1.4.0/test/
--rw-rw-r--   0 marine    (1000) marine    (1000)     5615 2024-05-20 18:38:25.000000 dropboxdrivefs-1.4.0/test/test.py
--rw-rw-r--   0 marine    (1000) marine    (1000)     2990 2024-05-20 18:38:25.000000 dropboxdrivefs-1.4.0/test/test_copy.py
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-27 14:04:28.649219 dropboxdrivefs-1.4.1/
+-rw-rw-r--   0 marine    (1000) marine    (1000)     1528 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.1/LICENSE
+-rw-rw-r--   0 marine    (1000) marine    (1000)       35 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.1/MANIFEST.in
+-rw-r--r--   0 marine    (1000) marine    (1000)     2221 2024-05-27 14:04:28.649219 dropboxdrivefs-1.4.1/PKG-INFO
+-rw-rw-r--   0 marine    (1000) marine    (1000)     1383 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.1/README.md
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-27 14:04:28.649219 dropboxdrivefs-1.4.1/dropboxdrivefs/
+-rw-rw-r--   0 marine    (1000) marine    (1000)       57 2024-01-18 18:26:56.000000 dropboxdrivefs-1.4.1/dropboxdrivefs/__init__.py
+-rw-rw-r--   0 marine    (1000) marine    (1000)     9796 2024-05-20 18:38:25.000000 dropboxdrivefs-1.4.1/dropboxdrivefs/core.py
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-27 14:04:28.649219 dropboxdrivefs-1.4.1/dropboxdrivefs.egg-info/
+-rw-r--r--   0 marine    (1000) marine    (1000)     2221 2024-05-27 14:04:28.000000 dropboxdrivefs-1.4.1/dropboxdrivefs.egg-info/PKG-INFO
+-rw-rw-r--   0 marine    (1000) marine    (1000)      314 2024-05-27 14:04:28.000000 dropboxdrivefs-1.4.1/dropboxdrivefs.egg-info/SOURCES.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)        1 2024-05-27 14:04:28.000000 dropboxdrivefs-1.4.1/dropboxdrivefs.egg-info/dependency_links.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)       24 2024-05-27 14:04:28.000000 dropboxdrivefs-1.4.1/dropboxdrivefs.egg-info/requires.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)       51 2024-05-27 14:04:28.000000 dropboxdrivefs-1.4.1/dropboxdrivefs.egg-info/top_level.txt
+-rw-rw-r--   0 marine    (1000) marine    (1000)      950 2024-05-27 14:04:16.000000 dropboxdrivefs-1.4.1/pyproject.toml
+-rw-rw-r--   0 marine    (1000) marine    (1000)       38 2024-05-27 14:04:28.649219 dropboxdrivefs-1.4.1/setup.cfg
+drwxrwxr-x   0 marine    (1000) marine    (1000)        0 2024-05-27 14:04:28.649219 dropboxdrivefs-1.4.1/test/
+-rw-rw-r--   0 marine    (1000) marine    (1000)     5615 2024-05-20 18:38:25.000000 dropboxdrivefs-1.4.1/test/test.py
+-rw-rw-r--   0 marine    (1000) marine    (1000)     2990 2024-05-20 18:38:25.000000 dropboxdrivefs-1.4.1/test/test_copy.py
```

### Comparing `dropboxdrivefs-1.4.0/LICENSE` & `dropboxdrivefs-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dropboxdrivefs-1.4.0/PKG-INFO` & `dropboxdrivefs-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropboxdrivefs
-Version: 1.4.0
+Version: 1.4.1
 Summary: Dropbox implementation for fsspec module
 Author-email: Marine Chaput <marine.chaput@hotmail.fr>
 License: BSD License
 Project-URL: Homepage, https://github.com/fsspec/dropboxdrivefs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dropboxdrivefs-1.4.0/README.md` & `dropboxdrivefs-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dropboxdrivefs-1.4.0/dropboxdrivefs/dropboxdrivefs.egg-info/PKG-INFO` & `dropboxdrivefs-1.4.1/dropboxdrivefs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropboxdrivefs
-Version: 1.4.0
+Version: 1.4.1
 Summary: Dropbox implementation for fsspec module
 Author-email: Marine Chaput <marine.chaput@hotmail.fr>
 License: BSD License
 Project-URL: Homepage, https://github.com/fsspec/dropboxdrivefs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dropboxdrivefs-1.4.0/pyproject.toml` & `dropboxdrivefs-1.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dropboxdrivefs"
-version = "1.4.0"
+version = "1.4.1"
 description = "Dropbox implementation for fsspec module"
 readme = "README.md"
 
 requires-python = ">=3.5"
 license = { text = "BSD License" }
 
 dependencies = [
@@ -30,8 +30,8 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.setuptools.packages.find]
-where = ["dropboxdrivefs"]
+where = ["."]
```

### Comparing `dropboxdrivefs-1.4.0/test/test.py` & `dropboxdrivefs-1.4.1/test/test.py`

 * *Files identical despite different names*

### Comparing `dropboxdrivefs-1.4.0/test/test_copy.py` & `dropboxdrivefs-1.4.1/test/test_copy.py`

 * *Files identical despite different names*

