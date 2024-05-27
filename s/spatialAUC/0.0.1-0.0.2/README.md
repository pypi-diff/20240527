# Comparing `tmp/spatialAUC-0.0.1.tar.gz` & `tmp/spatialAUC-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialAUC-0.0.1.tar", last modified: Mon May 27 13:53:36 2024, max compression
+gzip compressed data, was "spatialAUC-0.0.2.tar", last modified: Mon May 27 14:43:36 2024, max compression
```

## Comparing `spatialAUC-0.0.1.tar` & `spatialAUC-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-27 13:53:36.651174 spatialAUC-0.0.1/
--rw-r--r--   0 k23030440   (504) staff       (20)      508 2024-05-27 13:53:36.650946 spatialAUC-0.0.1/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-05-27 13:53:36.651224 spatialAUC-0.0.1/setup.cfg
--rw-r--r--   0 k23030440   (504) staff       (20)      876 2024-05-26 13:12:14.000000 spatialAUC-0.0.1/setup.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-27 13:53:36.650683 spatialAUC-0.0.1/spatialAUC.egg-info/
--rw-r--r--   0 k23030440   (504) staff       (20)      508 2024-05-27 13:53:36.000000 spatialAUC-0.0.1/spatialAUC.egg-info/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)      177 2024-05-27 13:53:36.000000 spatialAUC-0.0.1/spatialAUC.egg-info/SOURCES.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-27 13:53:36.000000 spatialAUC-0.0.1/spatialAUC.egg-info/dependency_links.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       20 2024-05-27 13:53:36.000000 spatialAUC-0.0.1/spatialAUC.egg-info/requires.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-27 13:53:36.000000 spatialAUC-0.0.1/spatialAUC.egg-info/top_level.txt
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-27 14:43:36.445310 spatialAUC-0.0.2/
+-rw-r--r--   0 k23030440   (504) staff       (20)      508 2024-05-27 14:43:36.445084 spatialAUC-0.0.2/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-05-27 14:43:36.445364 spatialAUC-0.0.2/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)      876 2024-05-27 14:43:32.000000 spatialAUC-0.0.2/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-05-27 14:43:36.444791 spatialAUC-0.0.2/spatialAUC.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      508 2024-05-27 14:43:36.000000 spatialAUC-0.0.2/spatialAUC.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      177 2024-05-27 14:43:36.000000 spatialAUC-0.0.2/spatialAUC.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-27 14:43:36.000000 spatialAUC-0.0.2/spatialAUC.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       20 2024-05-27 14:43:36.000000 spatialAUC-0.0.2/spatialAUC.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-05-27 14:43:36.000000 spatialAUC-0.0.2/spatialAUC.egg-info/top_level.txt
```

### Comparing `spatialAUC-0.0.1/setup.py` & `spatialAUC-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python package for gene set enrichment in spatial transcriptomic data'
 LONG_DESCRIPTION = 'Python package for gene set enrichment in spatial transcriptomic data, for more information see https://github.com/BKover99/pseudovisium'
 
 
 setup(
     name="spatialAUC",
     version=VERSION,
```

