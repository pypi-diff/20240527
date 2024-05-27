# Comparing `tmp/simscv-0.0.2.tar.gz` & `tmp/simscv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simscv-0.0.2.tar", last modified: Sun May 26 17:02:16 2024, max compression
+gzip compressed data, was "simscv-0.0.4.tar", last modified: Mon May 27 05:01:04 2024, max compression
```

## Comparing `simscv-0.0.2.tar` & `simscv-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-26 17:02:16.301745 simscv-0.0.2/
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)      539 2024-05-26 17:02:16.301539 simscv-0.0.2/PKG-INFO
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-26 14:44:19.000000 simscv-0.0.2/README.md
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       38 2024-05-26 17:02:16.301780 simscv-0.0.2/setup.cfg
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     1002 2024-05-26 17:00:54.000000 simscv-0.0.2/setup.py
-drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-26 17:02:16.300216 simscv-0.0.2/src/
-drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-26 17:02:16.301332 simscv-0.0.2/src/simscv.egg-info/
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)      539 2024-05-26 17:02:16.000000 simscv-0.0.2/src/simscv.egg-info/PKG-INFO
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)      224 2024-05-26 17:02:16.000000 simscv-0.0.2/src/simscv.egg-info/SOURCES.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        1 2024-05-26 17:02:16.000000 simscv-0.0.2/src/simscv.egg-info/dependency_links.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       39 2024-05-26 17:02:16.000000 simscv-0.0.2/src/simscv.egg-info/entry_points.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       25 2024-05-26 17:02:16.000000 simscv-0.0.2/src/simscv.egg-info/requires.txt
--rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        7 2024-05-26 17:02:16.000000 simscv-0.0.2/src/simscv.egg-info/top_level.txt
+drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:01:04.394406 simscv-0.0.4/
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     5106 2024-05-27 05:01:04.394201 simscv-0.0.4/PKG-INFO
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     4565 2024-05-27 04:30:52.000000 simscv-0.0.4/README.md
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       38 2024-05-27 05:01:04.394440 simscv-0.0.4/setup.cfg
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     1003 2024-05-27 04:55:47.000000 simscv-0.0.4/setup.py
+drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:01:04.392884 simscv-0.0.4/src/
+drwxr-xr-x   0 kanra_no_macbook   (501) staff       (20)        0 2024-05-27 05:01:04.394001 simscv-0.0.4/src/simscv.egg-info/
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)     5106 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/PKG-INFO
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)      224 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/SOURCES.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        1 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/dependency_links.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       39 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/entry_points.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)       25 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/requires.txt
+-rw-r--r--   0 kanra_no_macbook   (501) staff       (20)        7 2024-05-27 05:01:04.000000 simscv-0.0.4/src/simscv.egg-info/top_level.txt
```

### Comparing `simscv-0.0.2/setup.py` & `simscv-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="simscv",
-    version="0.0.2",
+    version="0.0.4",
     author="Kanra_Ishido",
     author_email="s2222002@stu.musashino-u.ac.jp",
     description="A simple csv reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kanra-Ishido/simscv",
     project_urls={
@@ -25,11 +25,11 @@
     install_requires=[
         'numpy',
         'scikit-learn',
         'scipy'
     ],
     entry_points={
         'console_scripts': [
-            'simscv = simscv:main'
+            'simcsv = simcsv:main'
         ]
-    }
+    },
 )
```

