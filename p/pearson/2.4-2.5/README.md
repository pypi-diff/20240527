# Comparing `tmp/pearson-2.4.tar.gz` & `tmp/pearson-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pearson-2.4.tar", last modified: Mon May 27 08:07:04 2024, max compression
+gzip compressed data, was "pearson-2.5.tar", last modified: Mon May 27 08:09:58 2024, max compression
```

## Comparing `pearson-2.4.tar` & `pearson-2.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 08:06:56.000000 pearson-2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:07:04.663204 pearson-2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/pearson/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/pearson/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/model.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/pearson.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-05-27 08:06:56.000000 pearson-2.4/pearson/brain.json
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-27 08:06:56.000000 pearson-2.4/pearson/data.pth
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 08:06:56.000000 pearson-2.4/pearson/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-27 08:06:56.000000 pearson-2.4/pearson/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-27 08:06:56.000000 pearson-2.4/pearson/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-27 08:06:56.000000 pearson-2.4/pearson/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/pearson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-27 08:06:56.000000 pearson-2.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:07:04.663204 pearson-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-27 08:06:56.000000 pearson-2.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 08:06:56.000000 pearson-2.4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.371422 pearson-2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 08:09:53.000000 pearson-2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:09:58.371422 pearson-2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.367422 pearson-2.5/pearson/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.371422 pearson-2.5/pearson/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/pearson.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-05-27 08:09:53.000000 pearson-2.5/pearson/brain.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-27 08:09:53.000000 pearson-2.5/pearson/data.pth
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 08:09:53.000000 pearson-2.5/pearson/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-27 08:09:53.000000 pearson-2.5/pearson/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-27 08:09:53.000000 pearson-2.5/pearson/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-27 08:09:53.000000 pearson-2.5/pearson/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.371422 pearson-2.5/pearson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 08:09:53.000000 pearson-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-27 08:09:53.000000 pearson-2.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:09:58.371422 pearson-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-27 08:09:53.000000 pearson-2.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 08:09:53.000000 pearson-2.5/version.py
```

### Comparing `pearson-2.4/PKG-INFO` & `pearson-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pearson
-Version: 2.4
+Version: 2.5
 Summary: A simple chatbot that can be trained to answer questions based on a dataset
 Home-page: https://github.com/mjfactor/Mr-Pearson.git
 Author: mjfactor
 Author-email: emjayfactor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pearson-2.4/pearson/__pycache__/main.cpython-311.pyc` & `pearson-2.5/pearson/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/__pycache__/model.cpython-311.pyc` & `pearson-2.5/pearson/__pycache__/model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/__pycache__/pearson.cpython-311.pyc` & `pearson-2.5/pearson/__pycache__/pearson.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/brain.json` & `pearson-2.5/pearson/brain.json`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/data.pth` & `pearson-2.5/pearson/data.pth`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/main.py` & `pearson-2.5/pearson/main.py`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/model.py` & `pearson-2.5/pearson/model.py`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/pearson.py` & `pearson-2.5/pearson/pearson.py`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson/train.py` & `pearson-2.5/pearson/train.py`

 * *Files identical despite different names*

### Comparing `pearson-2.4/pearson.egg-info/PKG-INFO` & `pearson-2.5/pearson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pearson
-Version: 2.4
+Version: 2.5
 Summary: A simple chatbot that can be trained to answer questions based on a dataset
 Home-page: https://github.com/mjfactor/Mr-Pearson.git
 Author: mjfactor
 Author-email: emjayfactor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pearson-2.4/readme.md` & `pearson-2.5/readme.md`

 * *Files identical despite different names*

### Comparing `pearson-2.4/setup.py` & `pearson-2.5/setup.py`

 * *Files identical despite different names*

