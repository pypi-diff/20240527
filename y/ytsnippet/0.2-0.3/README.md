# Comparing `tmp/ytsnippet-0.2.tar.gz` & `tmp/ytsnippet-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytsnippet-0.2.tar", last modified: Sun May 26 16:38:43 2024, max compression
+gzip compressed data, was "ytsnippet-0.3.tar", last modified: Sun May 26 16:46:26 2024, max compression
```

## Comparing `ytsnippet-0.2.tar` & `ytsnippet-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.905421 ytsnippet-0.2/
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      567 2024-05-26 16:38:43.905213 ytsnippet-0.2/PKG-INFO
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      121 2024-05-26 16:29:24.000000 ytsnippet-0.2/README.md
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       38 2024-05-26 16:38:43.905458 ytsnippet-0.2/setup.cfg
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      748 2024-05-26 16:38:35.000000 ytsnippet-0.2/setup.py
-drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.903745 ytsnippet-0.2/tests/
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:25:31.000000 ytsnippet-0.2/tests/test_manager.py
-drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.904101 ytsnippet-0.2/ytsnippet/
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:44:51.000000 ytsnippet-0.2/ytsnippet/__init__.py
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     3537 2024-05-26 16:29:37.000000 ytsnippet-0.2/ytsnippet/cli.py
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     1658 2024-05-26 16:26:12.000000 ytsnippet-0.2/ytsnippet/database.py
-drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.904959 ytsnippet-0.2/ytsnippet.egg-info/
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      567 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/PKG-INFO
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      301 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/SOURCES.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        1 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/dependency_links.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       49 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/entry_points.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       15 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/requires.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       10 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/top_level.txt
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:46:26.862004 ytsnippet-0.3/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     1346 2024-05-26 16:46:26.861794 ytsnippet-0.3/PKG-INFO
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      900 2024-05-26 16:45:55.000000 ytsnippet-0.3/README.md
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       38 2024-05-26 16:46:26.862053 ytsnippet-0.3/setup.cfg
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      748 2024-05-26 16:46:01.000000 ytsnippet-0.3/setup.py
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:46:26.860292 ytsnippet-0.3/tests/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:25:31.000000 ytsnippet-0.3/tests/test_manager.py
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:46:26.860652 ytsnippet-0.3/ytsnippet/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:44:51.000000 ytsnippet-0.3/ytsnippet/__init__.py
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     3537 2024-05-26 16:29:37.000000 ytsnippet-0.3/ytsnippet/cli.py
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     1658 2024-05-26 16:26:12.000000 ytsnippet-0.3/ytsnippet/database.py
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:46:26.861551 ytsnippet-0.3/ytsnippet.egg-info/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     1346 2024-05-26 16:46:26.000000 ytsnippet-0.3/ytsnippet.egg-info/PKG-INFO
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      301 2024-05-26 16:46:26.000000 ytsnippet-0.3/ytsnippet.egg-info/SOURCES.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        1 2024-05-26 16:46:26.000000 ytsnippet-0.3/ytsnippet.egg-info/dependency_links.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       49 2024-05-26 16:46:26.000000 ytsnippet-0.3/ytsnippet.egg-info/entry_points.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       15 2024-05-26 16:46:26.000000 ytsnippet-0.3/ytsnippet.egg-info/requires.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       10 2024-05-26 16:46:26.000000 ytsnippet-0.3/ytsnippet.egg-info/top_level.txt
```

### Comparing `ytsnippet-0.2/setup.py` & `ytsnippet-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ytsnippet',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'ytsnippet=ytsnippet.cli:main',
         ],
     },
     install_requires=['prompt_toolkit'],
```

### Comparing `ytsnippet-0.2/ytsnippet/cli.py` & `ytsnippet-0.3/ytsnippet/cli.py`

 * *Files identical despite different names*

### Comparing `ytsnippet-0.2/ytsnippet/database.py` & `ytsnippet-0.3/ytsnippet/database.py`

 * *Files identical despite different names*

