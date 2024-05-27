# Comparing `tmp/pearson-2.3.tar.gz` & `tmp/pearson-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pearson-2.3.tar", last modified: Sat Mar 30 03:27:35 2024, max compression
+gzip compressed data, was "pearson-2.4.tar", last modified: Mon May 27 08:07:04 2024, max compression
```

## Comparing `pearson-2.3.tar` & `pearson-2.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:27:35.561481 pearson-2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-30 03:27:31.000000 pearson-2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-30 03:27:35.561481 pearson-2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:27:35.561481 pearson-2.3/pearson/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-30 03:27:31.000000 pearson-2.3/pearson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:27:35.561481 pearson-2.3/pearson/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-30 03:27:31.000000 pearson-2.3/pearson/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-03-30 03:27:31.000000 pearson-2.3/pearson/__pycache__/pearson.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-03-30 03:27:31.000000 pearson-2.3/pearson/brain.json
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-30 03:27:31.000000 pearson-2.3/pearson/data.pth
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-30 03:27:31.000000 pearson-2.3/pearson/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-30 03:27:31.000000 pearson-2.3/pearson/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-30 03:27:31.000000 pearson-2.3/pearson/pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-30 03:27:31.000000 pearson-2.3/pearson/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:27:35.561481 pearson-2.3/pearson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-30 03:27:35.000000 pearson-2.3/pearson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-30 03:27:35.000000 pearson-2.3/pearson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 03:27:35.000000 pearson-2.3/pearson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-30 03:27:35.000000 pearson-2.3/pearson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-30 03:27:35.000000 pearson-2.3/pearson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-30 03:27:31.000000 pearson-2.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 03:27:35.561481 pearson-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-30 03:27:31.000000 pearson-2.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 03:27:31.000000 pearson-2.3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 08:06:56.000000 pearson-2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:07:04.663204 pearson-2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/pearson/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/pearson/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-27 08:06:56.000000 pearson-2.4/pearson/__pycache__/pearson.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-05-27 08:06:56.000000 pearson-2.4/pearson/brain.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-27 08:06:56.000000 pearson-2.4/pearson/data.pth
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 08:06:56.000000 pearson-2.4/pearson/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-27 08:06:56.000000 pearson-2.4/pearson/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-27 08:06:56.000000 pearson-2.4/pearson/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-27 08:06:56.000000 pearson-2.4/pearson/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:07:04.663204 pearson-2.4/pearson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 08:07:04.000000 pearson-2.4/pearson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-27 08:06:56.000000 pearson-2.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:07:04.663204 pearson-2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-27 08:06:56.000000 pearson-2.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 08:06:56.000000 pearson-2.4/version.py
```

### Comparing `pearson-2.3/PKG-INFO` & `pearson-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pearson
-Version: 2.3
+Version: 2.4
 Summary: A simple chatbot that can be trained to answer questions based on a dataset
-Home-page: https://github.com/mjfactor/Mr-Pearson
+Home-page: https://github.com/mjfactor/Mr-Pearson.git
 Author: mjfactor
 Author-email: emjayfactor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pearson-2.3/pearson/__pycache__/pearson.cpython-311.pyc` & `pearson-2.4/pearson/__pycache__/pearson.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pearson-2.3/pearson/brain.json` & `pearson-2.4/pearson/brain.json`

 * *Files identical despite different names*

### Comparing `pearson-2.3/pearson/data.pth` & `pearson-2.4/pearson/data.pth`

 * *Files identical despite different names*

### Comparing `pearson-2.3/pearson/main.py` & `pearson-2.4/pearson/main.py`

 * *Files identical despite different names*

### Comparing `pearson-2.3/pearson/model.py` & `pearson-2.4/pearson/model.py`

 * *Files identical despite different names*

### Comparing `pearson-2.3/pearson/pearson.py` & `pearson-2.4/pearson/pearson.py`

 * *Files identical despite different names*

### Comparing `pearson-2.3/pearson/train.py` & `pearson-2.4/pearson/train.py`

 * *Files identical despite different names*

### Comparing `pearson-2.3/pearson.egg-info/PKG-INFO` & `pearson-2.4/pearson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pearson
-Version: 2.3
+Version: 2.4
 Summary: A simple chatbot that can be trained to answer questions based on a dataset
-Home-page: https://github.com/mjfactor/Mr-Pearson
+Home-page: https://github.com/mjfactor/Mr-Pearson.git
 Author: mjfactor
 Author-email: emjayfactor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pearson-2.3/readme.md` & `pearson-2.4/readme.md`

 * *Files identical despite different names*

### Comparing `pearson-2.3/setup.py` & `pearson-2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 setup(
     name='pearson',
     version=version,
     packages=find_packages(),
     author='mjfactor',
-    url='https://github.com/mjfactor/Mr-Pearson',
+    url='https://github.com/mjfactor/Mr-Pearson.git',
     author_email='emjayfactor@gmail.com',
     description='A simple chatbot that can be trained to answer questions based on a dataset',
     long_description= long_description,
     long_description_content_type='text/markdown',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
```

