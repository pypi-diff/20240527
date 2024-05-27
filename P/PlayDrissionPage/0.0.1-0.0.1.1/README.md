# Comparing `tmp/PlayDrissionPage-0.0.1.tar.gz` & `tmp/PlayDrissionPage-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlayDrissionPage-0.0.1.tar", last modified: Mon May 27 05:48:38 2024, max compression
+gzip compressed data, was "PlayDrissionPage-0.0.1.1.tar", last modified: Mon May 27 05:55:05 2024, max compression
```

## Comparing `PlayDrissionPage-0.0.1.tar` & `PlayDrissionPage-0.0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 05:48:38.022227 PlayDrissionPage-0.0.1/
--rw-rw-rw-   0        0        0      627 2024-05-27 05:48:38.021227 PlayDrissionPage-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 05:48:38.011709 PlayDrissionPage-0.0.1/PlayDrissionPage/
--rw-rw-rw-   0        0        0      129 2024-05-27 05:48:33.000000 PlayDrissionPage-0.0.1/PlayDrissionPage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 05:48:38.020229 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/
--rw-rw-rw-   0        0        0      627 2024-05-27 05:48:37.000000 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-27 05:48:38.000000 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 05:48:37.000000 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-27 05:48:37.000000 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-27 05:38:48.000000 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2024-05-27 05:48:37.000000 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 05:48:37.000000 PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 05:48:38.023228 PlayDrissionPage-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2024-05-27 05:40:47.000000 PlayDrissionPage-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 05:55:05.306650 PlayDrissionPage-0.0.1.1/
+-rw-rw-rw-   0        0        0      629 2024-05-27 05:55:05.305652 PlayDrissionPage-0.0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 05:55:05.297175 PlayDrissionPage-0.0.1.1/PlayDrissionPage/
+-rw-rw-rw-   0        0        0      129 2024-05-27 05:52:47.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 05:55:05.304135 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/
+-rw-rw-rw-   0        0        0      629 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-27 05:38:48.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 05:55:05.000000 PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 05:55:05.306650 PlayDrissionPage-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2024-05-27 05:55:03.000000 PlayDrissionPage-0.0.1.1/setup.py
```

### Comparing `PlayDrissionPage-0.0.1/PKG-INFO` & `PlayDrissionPage-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlayDrissionPage
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Playwright and DrissionPage
 Home-page: https://gitee.com/xx299x/PlayDrissionPage
 Author: xx299x
 Author-email: xx299x@gmail.com
 License: BSD
 Keywords: Playwright,DrissionPage
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `PlayDrissionPage-0.0.1/PlayDrissionPage.egg-info/PKG-INFO` & `PlayDrissionPage-0.0.1.1/PlayDrissionPage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlayDrissionPage
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Playwright and DrissionPage
 Home-page: https://gitee.com/xx299x/PlayDrissionPage
 Author: xx299x
 Author-email: xx299x@gmail.com
 License: BSD
 Keywords: Playwright,DrissionPage
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `PlayDrissionPage-0.0.1/setup.py` & `PlayDrissionPage-0.0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
-from PlayDrissionPage import __version__
+__version__ = '0.0.1.1'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="PlayDrissionPage",
     version=__version__,
```

