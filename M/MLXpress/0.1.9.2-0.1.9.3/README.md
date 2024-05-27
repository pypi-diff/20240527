# Comparing `tmp/MLXpress-0.1.9.2.tar.gz` & `tmp/MLXpress-0.1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLXpress-0.1.9.2.tar", last modified: Sat Apr 27 14:14:57 2024, max compression
+gzip compressed data, was "MLXpress-0.1.9.3.tar", last modified: Mon May 27 11:54:14 2024, max compression
```

## Comparing `MLXpress-0.1.9.2.tar` & `MLXpress-0.1.9.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 14:14:57.639200 MLXpress-0.1.9.2/
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 14:14:57.637812 MLXpress-0.1.9.2/MLXpress/
--rw-rw-r--   0 vinilg7    (501) staff       (20)        0 2023-07-14 01:21:38.000000 MLXpress-0.1.9.2/MLXpress/__init__.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     5478 2023-12-13 11:57:53.000000 MLXpress-0.1.9.2/MLXpress/bigdata.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     2338 2023-07-16 23:45:14.000000 MLXpress-0.1.9.2/MLXpress/diabetes.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     6232 2024-04-14 12:01:28.000000 MLXpress-0.1.9.2/MLXpress/getdata.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     3360 2023-12-14 13:36:32.000000 MLXpress-0.1.9.2/MLXpress/help.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     4011 2023-07-17 06:11:02.000000 MLXpress-0.1.9.2/MLXpress/iris.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     3240 2023-12-13 09:58:20.000000 MLXpress-0.1.9.2/MLXpress/math.py
--rw-r--r--   0 vinilg7    (501) staff       (20)    28135 2023-12-13 09:58:20.000000 MLXpress-0.1.9.2/MLXpress/ml.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     5030 2023-07-17 05:03:38.000000 MLXpress-0.1.9.2/MLXpress/preprocessing.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     1870 2023-07-17 05:24:56.000000 MLXpress-0.1.9.2/MLXpress/stats.py
--rw-r--r--   0 vinilg7    (501) staff       (20)    11741 2024-04-27 13:48:43.000000 MLXpress-0.1.9.2/MLXpress/timeSeries.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     2733 2023-07-17 06:10:32.000000 MLXpress-0.1.9.2/MLXpress/wine.py
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-27 14:14:57.638672 MLXpress-0.1.9.2/MLXpress.egg-info/
--rw-r--r--   0 vinilg7    (501) staff       (20)     2451 2024-04-27 14:14:57.000000 MLXpress-0.1.9.2/MLXpress.egg-info/PKG-INFO
--rw-r--r--   0 vinilg7    (501) staff       (20)      409 2024-04-27 14:14:57.000000 MLXpress-0.1.9.2/MLXpress.egg-info/SOURCES.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)        1 2024-04-27 14:14:57.000000 MLXpress-0.1.9.2/MLXpress.egg-info/dependency_links.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)       87 2024-04-27 14:14:57.000000 MLXpress-0.1.9.2/MLXpress.egg-info/requires.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)        9 2024-04-27 14:14:57.000000 MLXpress-0.1.9.2/MLXpress.egg-info/top_level.txt
--rw-r--r--   0 vinilg7    (501) staff       (20)     2451 2024-04-27 14:14:57.638985 MLXpress-0.1.9.2/PKG-INFO
--rw-rw-r--   0 vinilg7    (501) staff       (20)     1718 2023-07-16 07:37:28.000000 MLXpress-0.1.9.2/README.md
--rw-r--r--   0 vinilg7    (501) staff       (20)       38 2024-04-27 14:14:57.639249 MLXpress-0.1.9.2/setup.cfg
--rw-r--r--   0 vinilg7    (501) staff       (20)      971 2024-04-27 14:12:10.000000 MLXpress-0.1.9.2/setup.py
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-05-27 11:54:14.410338 MLXpress-0.1.9.3/
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-05-27 11:54:14.408613 MLXpress-0.1.9.3/MLXpress/
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        0 2023-07-14 01:21:38.000000 MLXpress-0.1.9.3/MLXpress/__init__.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     5478 2023-12-13 11:57:53.000000 MLXpress-0.1.9.3/MLXpress/bigdata.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     2338 2023-07-16 23:45:14.000000 MLXpress-0.1.9.3/MLXpress/diabetes.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     6232 2024-04-14 12:01:28.000000 MLXpress-0.1.9.3/MLXpress/getdata.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     3914 2024-05-27 11:51:59.000000 MLXpress-0.1.9.3/MLXpress/gt.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     3360 2023-12-14 13:36:32.000000 MLXpress-0.1.9.3/MLXpress/help.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     4011 2023-07-17 06:11:02.000000 MLXpress-0.1.9.3/MLXpress/iris.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     3240 2023-12-13 09:58:20.000000 MLXpress-0.1.9.3/MLXpress/math.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)    28135 2023-12-13 09:58:20.000000 MLXpress-0.1.9.3/MLXpress/ml.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     5030 2023-07-17 05:03:38.000000 MLXpress-0.1.9.3/MLXpress/preprocessing.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     1870 2023-07-17 05:24:56.000000 MLXpress-0.1.9.3/MLXpress/stats.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)    11741 2024-04-27 13:48:43.000000 MLXpress-0.1.9.3/MLXpress/timeSeries.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     2733 2023-07-17 06:10:32.000000 MLXpress-0.1.9.3/MLXpress/wine.py
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-05-27 11:54:14.409624 MLXpress-0.1.9.3/MLXpress.egg-info/
+-rw-r--r--   0 vinilg7    (501) staff       (20)     2451 2024-05-27 11:54:14.000000 MLXpress-0.1.9.3/MLXpress.egg-info/PKG-INFO
+-rw-r--r--   0 vinilg7    (501) staff       (20)      424 2024-05-27 11:54:14.000000 MLXpress-0.1.9.3/MLXpress.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        1 2024-05-27 11:54:14.000000 MLXpress-0.1.9.3/MLXpress.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)       87 2024-05-27 11:54:14.000000 MLXpress-0.1.9.3/MLXpress.egg-info/requires.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        9 2024-05-27 11:54:14.000000 MLXpress-0.1.9.3/MLXpress.egg-info/top_level.txt
+-rw-r--r--   0 vinilg7    (501) staff       (20)     2451 2024-05-27 11:54:14.410123 MLXpress-0.1.9.3/PKG-INFO
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     1718 2023-07-16 07:37:28.000000 MLXpress-0.1.9.3/README.md
+-rw-r--r--   0 vinilg7    (501) staff       (20)       38 2024-05-27 11:54:14.410484 MLXpress-0.1.9.3/setup.cfg
+-rw-r--r--   0 vinilg7    (501) staff       (20)      971 2024-05-27 11:53:40.000000 MLXpress-0.1.9.3/setup.py
```

### Comparing `MLXpress-0.1.9.2/MLXpress/bigdata.py` & `MLXpress-0.1.9.3/MLXpress/bigdata.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/diabetes.py` & `MLXpress-0.1.9.3/MLXpress/diabetes.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/getdata.py` & `MLXpress-0.1.9.3/MLXpress/getdata.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/help.py` & `MLXpress-0.1.9.3/MLXpress/help.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/iris.py` & `MLXpress-0.1.9.3/MLXpress/iris.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/math.py` & `MLXpress-0.1.9.3/MLXpress/math.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/ml.py` & `MLXpress-0.1.9.3/MLXpress/ml.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/preprocessing.py` & `MLXpress-0.1.9.3/MLXpress/preprocessing.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/stats.py` & `MLXpress-0.1.9.3/MLXpress/stats.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/timeSeries.py` & `MLXpress-0.1.9.3/MLXpress/timeSeries.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress/wine.py` & `MLXpress-0.1.9.3/MLXpress/wine.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/MLXpress.egg-info/PKG-INFO` & `MLXpress-0.1.9.3/MLXpress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MLXpress-0.1.9.2/PKG-INFO` & `MLXpress-0.1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MLXpress-0.1.9.2/README.md` & `MLXpress-0.1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.9.2/setup.py` & `MLXpress-0.1.9.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='MLXpress',
-    version='0.1.9.2',
+    version='0.1.9.3',
     author='vinilg7',
     author_email='vinilg7@gmail.com',
     description='A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

