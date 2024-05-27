# Comparing `tmp/area_converter-0.1.5.tar.gz` & `tmp/area_converter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "area_converter-0.1.5.tar", last modified: Sun May 26 21:57:00 2024, max compression
+gzip compressed data, was "area_converter-0.1.6.tar", last modified: Mon May 27 05:11:18 2024, max compression
```

## Comparing `area_converter-0.1.5.tar` & `area_converter-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-26 21:57:00.753042 area_converter-0.1.5/
--rw-r--r--   0 takadaharuna   (501) staff       (20)      560 2024-05-26 21:57:00.752929 area_converter-0.1.5/PKG-INFO
--rw-r--r--   0 takadaharuna   (501) staff       (20)       73 2024-05-26 19:34:08.000000 area_converter-0.1.5/README.md
--rw-r--r--   0 takadaharuna   (501) staff       (20)       38 2024-05-26 21:57:00.753077 area_converter-0.1.5/setup.cfg
--rw-r--r--   0 takadaharuna   (501) staff       (20)      965 2024-05-26 21:56:50.000000 area_converter-0.1.5/setup.py
-drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-26 21:57:00.752058 area_converter-0.1.5/src/
-drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-26 21:57:00.752691 area_converter-0.1.5/src/area_converter.egg-info/
--rw-r--r--   0 takadaharuna   (501) staff       (20)      560 2024-05-26 21:57:00.000000 area_converter-0.1.5/src/area_converter.egg-info/PKG-INFO
--rw-r--r--   0 takadaharuna   (501) staff       (20)      271 2024-05-26 21:57:00.000000 area_converter-0.1.5/src/area_converter.egg-info/SOURCES.txt
--rw-r--r--   0 takadaharuna   (501) staff       (20)        1 2024-05-26 21:57:00.000000 area_converter-0.1.5/src/area_converter.egg-info/dependency_links.txt
--rw-r--r--   0 takadaharuna   (501) staff       (20)       56 2024-05-26 21:57:00.000000 area_converter-0.1.5/src/area_converter.egg-info/entry_points.txt
--rw-r--r--   0 takadaharuna   (501) staff       (20)       15 2024-05-26 21:57:00.000000 area_converter-0.1.5/src/area_converter.egg-info/top_level.txt
--rw-r--r--   0 takadaharuna   (501) staff       (20)     1717 2024-05-26 21:55:27.000000 area_converter-0.1.5/src/area_converter.py
-drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-26 21:57:00.752794 area_converter-0.1.5/test/
--rw-r--r--   0 takadaharuna   (501) staff       (20)        0 2024-05-26 21:52:01.000000 area_converter-0.1.5/test/test_area.py
+drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-27 05:11:18.665677 area_converter-0.1.6/
+-rw-r--r--   0 takadaharuna   (501) staff       (20)      729 2024-05-27 05:11:18.665560 area_converter-0.1.6/PKG-INFO
+-rw-r--r--   0 takadaharuna   (501) staff       (20)      242 2024-05-27 05:01:15.000000 area_converter-0.1.6/README.md
+-rw-r--r--   0 takadaharuna   (501) staff       (20)       38 2024-05-27 05:11:18.665714 area_converter-0.1.6/setup.cfg
+-rw-r--r--   0 takadaharuna   (501) staff       (20)      965 2024-05-27 05:10:07.000000 area_converter-0.1.6/setup.py
+drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-27 05:11:18.664666 area_converter-0.1.6/src/
+drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-27 05:11:18.665311 area_converter-0.1.6/src/area_converter.egg-info/
+-rw-r--r--   0 takadaharuna   (501) staff       (20)      729 2024-05-27 05:11:18.000000 area_converter-0.1.6/src/area_converter.egg-info/PKG-INFO
+-rw-r--r--   0 takadaharuna   (501) staff       (20)      271 2024-05-27 05:11:18.000000 area_converter-0.1.6/src/area_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 takadaharuna   (501) staff       (20)        1 2024-05-27 05:11:18.000000 area_converter-0.1.6/src/area_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 takadaharuna   (501) staff       (20)       56 2024-05-27 05:11:18.000000 area_converter-0.1.6/src/area_converter.egg-info/entry_points.txt
+-rw-r--r--   0 takadaharuna   (501) staff       (20)       15 2024-05-27 05:11:18.000000 area_converter-0.1.6/src/area_converter.egg-info/top_level.txt
+-rw-r--r--   0 takadaharuna   (501) staff       (20)     1717 2024-05-26 21:55:27.000000 area_converter-0.1.6/src/area_converter.py
+drwxr-xr-x   0 takadaharuna   (501) staff       (20)        0 2024-05-27 05:11:18.665421 area_converter-0.1.6/test/
+-rw-r--r--   0 takadaharuna   (501) staff       (20)        0 2024-05-26 21:52:01.000000 area_converter-0.1.6/test/test_area.py
```

### Comparing `area_converter-0.1.5/setup.py` & `area_converter-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='area_converter',
-    version='0.1.5',
+    version='0.1.6',
     author='Haruna Takada',
     description="A package that converts area to Tokyo Dome",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/HarunaTakada/area_converter",
     project_urls={
         "Bug Tracker": "https://github.com/HarunaTakada/area_converter",
```

### Comparing `area_converter-0.1.5/src/area_converter.py` & `area_converter-0.1.6/src/area_converter.py`

 * *Files identical despite different names*

