# Comparing `tmp/pearson-2.5.tar.gz` & `tmp/pearson-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pearson-2.5.tar", last modified: Mon May 27 08:09:58 2024, max compression
+gzip compressed data, was "pearson-2.6.tar", last modified: Mon May 27 08:39:12 2024, max compression
```

## Comparing `pearson-2.5.tar` & `pearson-2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.371422 pearson-2.5/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 08:09:53.000000 pearson-2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:09:58.371422 pearson-2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.367422 pearson-2.5/pearson/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.371422 pearson-2.5/pearson/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/model.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-27 08:09:53.000000 pearson-2.5/pearson/__pycache__/pearson.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-05-27 08:09:53.000000 pearson-2.5/pearson/brain.json
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-27 08:09:53.000000 pearson-2.5/pearson/data.pth
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 08:09:53.000000 pearson-2.5/pearson/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-27 08:09:53.000000 pearson-2.5/pearson/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-27 08:09:53.000000 pearson-2.5/pearson/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-27 08:09:53.000000 pearson-2.5/pearson/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:09:58.371422 pearson-2.5/pearson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 08:09:58.000000 pearson-2.5/pearson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 08:09:53.000000 pearson-2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-27 08:09:53.000000 pearson-2.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:09:58.371422 pearson-2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-27 08:09:53.000000 pearson-2.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 08:09:53.000000 pearson-2.5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:39:12.816017 pearson-2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 08:39:08.000000 pearson-2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-27 08:39:12.816017 pearson-2.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:39:12.812017 pearson-2.6/pearson/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 08:39:08.000000 pearson-2.6/pearson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:39:12.816017 pearson-2.6/pearson/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 08:39:08.000000 pearson-2.6/pearson/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 08:39:08.000000 pearson-2.6/pearson/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 08:39:08.000000 pearson-2.6/pearson/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-27 08:39:08.000000 pearson-2.6/pearson/__pycache__/pearson.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-05-27 08:39:08.000000 pearson-2.6/pearson/brain.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-27 08:39:08.000000 pearson-2.6/pearson/data.pth
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 08:39:08.000000 pearson-2.6/pearson/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-27 08:39:08.000000 pearson-2.6/pearson/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-27 08:39:08.000000 pearson-2.6/pearson/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-27 08:39:08.000000 pearson-2.6/pearson/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:39:12.816017 pearson-2.6/pearson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-27 08:39:12.000000 pearson-2.6/pearson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-27 08:39:12.000000 pearson-2.6/pearson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:39:12.000000 pearson-2.6/pearson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 08:39:12.000000 pearson-2.6/pearson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 08:39:12.000000 pearson-2.6/pearson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 08:39:08.000000 pearson-2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-27 08:39:08.000000 pearson-2.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:39:12.816017 pearson-2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-27 08:39:08.000000 pearson-2.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 08:39:08.000000 pearson-2.6/version.py
```

### Comparing `pearson-2.5/PKG-INFO` & `pearson-2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pearson
-Version: 2.5
+Version: 2.6
 Summary: A simple chatbot that can be trained to answer questions based on a dataset
 Home-page: https://github.com/mjfactor/Mr-Pearson.git
 Author: mjfactor
 Author-email: emjayfactor@gmail.com
+Project-URL: Source, https://github.com/mjfactor/Mr-Pearson.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pearson-2.5/pearson/__pycache__/main.cpython-311.pyc` & `pearson-2.6/pearson/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/__pycache__/model.cpython-311.pyc` & `pearson-2.6/pearson/__pycache__/model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/__pycache__/pearson.cpython-311.pyc` & `pearson-2.6/pearson/__pycache__/pearson.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/brain.json` & `pearson-2.6/pearson/brain.json`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/data.pth` & `pearson-2.6/pearson/data.pth`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/main.py` & `pearson-2.6/pearson/main.py`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/model.py` & `pearson-2.6/pearson/model.py`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/pearson.py` & `pearson-2.6/pearson/pearson.py`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson/train.py` & `pearson-2.6/pearson/train.py`

 * *Files identical despite different names*

### Comparing `pearson-2.5/pearson.egg-info/PKG-INFO` & `pearson-2.6/pearson.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pearson
-Version: 2.5
+Version: 2.6
 Summary: A simple chatbot that can be trained to answer questions based on a dataset
 Home-page: https://github.com/mjfactor/Mr-Pearson.git
 Author: mjfactor
 Author-email: emjayfactor@gmail.com
+Project-URL: Source, https://github.com/mjfactor/Mr-Pearson.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pearson-2.5/readme.md` & `pearson-2.6/readme.md`

 * *Files identical despite different names*

### Comparing `pearson-2.5/setup.py` & `pearson-2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,11 +30,14 @@
         'Programming Language :: Python :: 3.10',
         "Operating System :: OS Independent"
     ],
     install_requires=[
         'nltk',
         'torch'
     ],
+    project_urls={
+        'Source': 'https://github.com/mjfactor/Mr-Pearson.git',
+    },
     include_package_data=True,
     python_requires='>=3.7',
     package_data={'': ['readme.md']}
 )
```

