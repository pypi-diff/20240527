# Comparing `tmp/damage_calculator-0.1.0.tar.gz` & `tmp/damage_calculator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damage_calculator-0.1.0.tar", last modified: Fri May 24 04:08:50 2024, max compression
+gzip compressed data, was "damage_calculator-0.2.0.tar", last modified: Mon May 27 04:32:54 2024, max compression
```

## Comparing `damage_calculator-0.1.0.tar` & `damage_calculator-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-24 04:08:50.977395 damage_calculator-0.1.0/
--rw-r--r--   0 siro       (501) staff       (20)     1065 2024-05-24 03:59:28.000000 damage_calculator-0.1.0/LICENSE
--rw-r--r--   0 siro       (501) staff       (20)      605 2024-05-24 04:08:50.976954 damage_calculator-0.1.0/PKG-INFO
--rw-r--r--   0 siro       (501) staff       (20)      142 2024-05-24 03:59:28.000000 damage_calculator-0.1.0/README.md
-drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-24 04:08:50.972779 damage_calculator-0.1.0/damage_calculator/
--rw-r--r--   0 siro       (501) staff       (20)       32 2024-05-24 03:59:28.000000 damage_calculator-0.1.0/damage_calculator/__init__.py
--rw-r--r--   0 siro       (501) staff       (20)     1579 2024-05-24 03:59:28.000000 damage_calculator-0.1.0/damage_calculator/calculator.py
-drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-24 04:08:50.976617 damage_calculator-0.1.0/damage_calculator.egg-info/
--rw-r--r--   0 siro       (501) staff       (20)      605 2024-05-24 04:08:50.000000 damage_calculator-0.1.0/damage_calculator.egg-info/PKG-INFO
--rw-r--r--   0 siro       (501) staff       (20)      296 2024-05-24 04:08:50.000000 damage_calculator-0.1.0/damage_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 siro       (501) staff       (20)        1 2024-05-24 04:08:50.000000 damage_calculator-0.1.0/damage_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 siro       (501) staff       (20)       72 2024-05-24 04:08:50.000000 damage_calculator-0.1.0/damage_calculator.egg-info/entry_points.txt
--rw-r--r--   0 siro       (501) staff       (20)       18 2024-05-24 04:08:50.000000 damage_calculator-0.1.0/damage_calculator.egg-info/top_level.txt
--rw-r--r--   0 siro       (501) staff       (20)       38 2024-05-24 04:08:50.977448 damage_calculator-0.1.0/setup.cfg
--rw-r--r--   0 siro       (501) staff       (20)      794 2024-05-24 04:07:36.000000 damage_calculator-0.1.0/setup.py
+drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:32:54.765582 damage_calculator-0.2.0/
+-rw-r--r--   0 siro       (501) staff       (20)     1065 2024-05-24 03:59:28.000000 damage_calculator-0.2.0/LICENSE
+-rw-r--r--   0 siro       (501) staff       (20)      896 2024-05-27 04:32:54.765207 damage_calculator-0.2.0/PKG-INFO
+-rw-r--r--   0 siro       (501) staff       (20)      433 2024-05-27 04:29:01.000000 damage_calculator-0.2.0/README.md
+drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:32:54.760798 damage_calculator-0.2.0/damage_calculator/
+-rw-r--r--   0 siro       (501) staff       (20)       32 2024-05-24 03:59:28.000000 damage_calculator-0.2.0/damage_calculator/__init__.py
+-rw-r--r--   0 siro       (501) staff       (20)     1579 2024-05-24 03:59:28.000000 damage_calculator-0.2.0/damage_calculator/calculator.py
+drwxr-xr-x   0 siro       (501) staff       (20)        0 2024-05-27 04:32:54.764836 damage_calculator-0.2.0/damage_calculator.egg-info/
+-rw-r--r--   0 siro       (501) staff       (20)      896 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 siro       (501) staff       (20)      296 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 siro       (501) staff       (20)        1 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 siro       (501) staff       (20)       72 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 siro       (501) staff       (20)       18 2024-05-27 04:32:54.000000 damage_calculator-0.2.0/damage_calculator.egg-info/top_level.txt
+-rw-r--r--   0 siro       (501) staff       (20)       38 2024-05-27 04:32:54.765648 damage_calculator-0.2.0/setup.cfg
+-rw-r--r--   0 siro       (501) staff       (20)      794 2024-05-27 04:32:32.000000 damage_calculator-0.2.0/setup.py
```

### Comparing `damage_calculator-0.1.0/LICENSE` & `damage_calculator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `damage_calculator-0.1.0/damage_calculator/calculator.py` & `damage_calculator-0.2.0/damage_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `damage_calculator-0.1.0/setup.py` & `damage_calculator-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="damage_calculator",
-    version="0.1.0",
+    version="0.2.0",
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'damage_calculator = damage_calculator.calculator:main',
         ],
     },
     install_requires=[],
```

