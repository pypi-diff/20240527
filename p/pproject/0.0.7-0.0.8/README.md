# Comparing `tmp/pproject-0.0.7.tar.gz` & `tmp/pproject-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pproject-0.0.7.tar", last modified: Mon May 27 05:45:59 2024, max compression
+gzip compressed data, was "pproject-0.0.8.tar", last modified: Mon May 27 19:46:14 2024, max compression
```

## Comparing `pproject-0.0.7.tar` & `pproject-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-27 05:45:59.451380 pproject-0.0.7/
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      974 2024-05-27 05:45:59.451136 pproject-0.0.7/PKG-INFO
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      484 2024-05-27 05:41:56.000000 pproject-0.0.7/README.md
--rw-r--r--   0 sojirotachibana   (501) staff       (20)       38 2024-05-27 05:45:59.451421 pproject-0.0.7/setup.cfg
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      928 2024-05-27 05:45:06.000000 pproject-0.0.7/setup.py
-drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-27 05:45:59.447743 pproject-0.0.7/src/
-drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-27 05:45:59.450378 pproject-0.0.7/src/pproject.egg-info/
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      974 2024-05-27 05:45:59.000000 pproject-0.0.7/src/pproject.egg-info/PKG-INFO
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      217 2024-05-27 05:45:59.000000 pproject-0.0.7/src/pproject.egg-info/SOURCES.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)        1 2024-05-27 05:45:59.000000 pproject-0.0.7/src/pproject.egg-info/dependency_links.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)       43 2024-05-27 05:45:59.000000 pproject-0.0.7/src/pproject.egg-info/entry_points.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)        9 2024-05-27 05:45:59.000000 pproject-0.0.7/src/pproject.egg-info/top_level.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)     3556 2024-05-26 22:36:09.000000 pproject-0.0.7/src/pproject.py
+drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-27 19:46:14.190408 pproject-0.0.8/
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)     1270 2024-05-27 19:46:14.190118 pproject-0.0.8/PKG-INFO
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)      780 2024-05-27 19:44:18.000000 pproject-0.0.8/README.md
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)       38 2024-05-27 19:46:14.190451 pproject-0.0.8/setup.cfg
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)      928 2024-05-27 19:45:28.000000 pproject-0.0.8/setup.py
+drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-27 19:46:14.188284 pproject-0.0.8/src/
+drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-27 19:46:14.189846 pproject-0.0.8/src/pproject.egg-info/
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)     1270 2024-05-27 19:46:14.000000 pproject-0.0.8/src/pproject.egg-info/PKG-INFO
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)      217 2024-05-27 19:46:14.000000 pproject-0.0.8/src/pproject.egg-info/SOURCES.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)        1 2024-05-27 19:46:14.000000 pproject-0.0.8/src/pproject.egg-info/dependency_links.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)       43 2024-05-27 19:46:14.000000 pproject-0.0.8/src/pproject.egg-info/entry_points.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)        9 2024-05-27 19:46:14.000000 pproject-0.0.8/src/pproject.egg-info/top_level.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)     3556 2024-05-26 22:36:09.000000 pproject-0.0.8/src/pproject.py
```

### Comparing `pproject-0.0.7/PKG-INFO` & `pproject-0.0.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,9 @@
-Metadata-Version: 2.1
-Name: pproject
-Version: 0.0.7
-Summary: Predicted price change for iphone in XX years
-Home-page: https://github.com/Sojiro4/pproject
-Author: Sojiro4
-Author-email: s2122097@stu.musashino-u.ac.jp
-Project-URL: Bug Tracker, https://github.com/Sojiro4/pproject
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.3
-Description-Content-Type: text/markdown
-
 # About the pproject
-Predicted price change for iphone in XX years
+Predicted price change for iPhone in XX years
 
 ### how to install pproject
 
 $ pip install pproject
 
 ### required Libraries
 
@@ -28,16 +14,22 @@
 datetime
 
 ### how to run pproject
 < ~ .py><br>
 import pproject<br>
 pproject.price_fluctuation_now()</br></br>
 $python ~.py
-![Figure1](img/Figure_1.png)
+![Figure1](https://raw.githubusercontent.com/Sojiro4/pproject/main/img/Figure_1.png)
+
+classification0 : iPhone SE series</br>
+classification1 : Regular iPhone series</br>
+classification2,3,4 : Other series (Pro, Plus, etc.)</br></br>
 
 
 < ~ .py></br>
-import pproject
+import pproject</br>
 pproject.Predicted_price_change_in_XX_years(100)</br></br>
 $python ~.py
-![Figure2](img/Figure_2.png)
+![Figure2](https://raw.githubusercontent.com/Sojiro4/pproject/main/img/Figure_2.png)
+
+Prediction by regular series
```

### Comparing `pproject-0.0.7/setup.py` & `pproject-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md","r",encoding="utf-8")as fh:
     long_description=fh.read()
 setuptools.setup(
     name="pproject",
-    version="0.0.7",
+    version="0.0.8",
     author="Sojiro4",
     author_email="s2122097@stu.musashino-u.ac.jp",
     description="Predicted price change for iphone in XX years",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sojiro4/pproject",
     project_urls={
```

### Comparing `pproject-0.0.7/src/pproject.py` & `pproject-0.0.8/src/pproject.py`

 * *Files identical despite different names*

