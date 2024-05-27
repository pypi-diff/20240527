# Comparing `tmp/simscv-0.0.4.tar.gz` & `tmp/simscv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simscv-0.0.4.tar", last modified: Mon May 27 05:01:04 2024, max compression
+gzip compressed data, was "simscv-0.0.5.tar", last modified: Mon May 27 05:04:30 2024, max compression
```

## Comparing `simscv-0.0.4.tar` & `simscv-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:01:04.394406 simscv-0.0.4/
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     5106 2024-05-27 05:01:04.394201 simscv-0.0.4/PKG-INFO
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     4565 2024-05-27 04:30:52.000000 simscv-0.0.4/README.md
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       38 2024-05-27 05:01:04.394440 simscv-0.0.4/setup.cfg
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     1003 2024-05-27 04:55:47.000000 simscv-0.0.4/setup.py
-drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:01:04.392884 simscv-0.0.4/src/
-drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:01:04.394001 simscv-0.0.4/src/simscv.egg-info/
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     5106 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/PKG-INFO
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)      224 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/SOURCES.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        1 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/dependency_links.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       39 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/entry_points.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       25 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/requires.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        7 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/top_level.txt
+drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:04:30.171390 simscv-0.0.5/
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     5106 2024-05-27 05:04:30.171172 simscv-0.0.5/PKG-INFO
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     4565 2024-05-27 04:30:52.000000 simscv-0.0.5/README.md
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       38 2024-05-27 05:04:30.171426 simscv-0.0.5/setup.cfg
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     1003 2024-05-27 05:04:05.000000 simscv-0.0.5/setup.py
+drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:04:30.170033 simscv-0.0.5/src/
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)    10310 2024-05-26 13:34:15.000000 simscv-0.0.5/src/simcsv.py
+drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:04:30.170919 simscv-0.0.5/src/simscv.egg-info/
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     5106 2024-05-27 05:04:30.000000 simscv-0.0.5/src/simscv.egg-info/PKG-INFO
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)      238 2024-05-27 05:04:30.000000 simscv-0.0.5/src/simscv.egg-info/SOURCES.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        1 2024-05-27 05:04:30.000000 simscv-0.0.5/src/simscv.egg-info/dependency_links.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       39 2024-05-27 05:04:30.000000 simscv-0.0.5/src/simscv.egg-info/entry_points.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       25 2024-05-27 05:04:30.000000 simscv-0.0.5/src/simscv.egg-info/requires.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        7 2024-05-27 05:04:30.000000 simscv-0.0.5/src/simscv.egg-info/top_level.txt
```

### Comparing `simscv-0.0.4/PKG-INFO` & `simscv-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simscv
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple csv reader
 Home-page: https://github.com/Kanra-Ishido/simscv
 Author: Kanra_Ishido
 Author-email: s2222002@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/Kanra-Ishido/simscv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `simscv-0.0.4/README.md` & `simscv-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `simscv-0.0.4/setup.py` & `simscv-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="simscv",
-    version="0.0.4",
+    version="0.0.5",
     author="Kanra_Ishido",
     author_email="s2222002@stu.musashino-u.ac.jp",
     description="A simple csv reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kanra-Ishido/simscv",
     project_urls={
@@ -15,15 +15,15 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
-    py_modules=["simscv"],
+    py_modules=["simcsv"],
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
     install_requires=[
         'numpy',
         'scikit-learn',
         'scipy'
     ],
```

### Comparing `simscv-0.0.4/src/simscv.egg-info/PKG-INFO` & `simscv-0.0.5/src/simscv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simscv
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple csv reader
 Home-page: https://github.com/Kanra-Ishido/simscv
 Author: Kanra_Ishido
 Author-email: s2222002@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/Kanra-Ishido/simscv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

