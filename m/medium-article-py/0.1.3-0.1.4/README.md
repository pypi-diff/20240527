# Comparing `tmp/medium_article_py-0.1.3.tar.gz` & `tmp/medium_article_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_article_py-0.1.3.tar", last modified: Mon May 27 19:59:23 2024, max compression
+gzip compressed data, was "medium_article_py-0.1.4.tar", last modified: Mon May 27 20:17:36 2024, max compression
```

## Comparing `medium_article_py-0.1.3.tar` & `medium_article_py-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 19:59:23.381692 medium_article_py-0.1.3/
--rw-rw-rw-   0        0        0     1092 2024-05-27 16:13:44.000000 medium_article_py-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1586 2024-05-27 19:59:23.381692 medium_article_py-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2024-05-27 19:58:46.000000 medium_article_py-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-27 19:59:23.366080 medium_article_py-0.1.3/medium_article_py.egg-info/
--rw-rw-rw-   0        0        0     1586 2024-05-27 19:59:23.000000 medium_article_py-0.1.3/medium_article_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-05-27 19:59:23.000000 medium_article_py-0.1.3/medium_article_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 19:59:23.000000 medium_article_py-0.1.3/medium_article_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 19:59:23.000000 medium_article_py-0.1.3/medium_article_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 19:59:23.000000 medium_article_py-0.1.3/medium_article_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 19:59:23.381692 medium_article_py-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      796 2024-05-27 19:57:15.000000 medium_article_py-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:59:23.366080 medium_article_py-0.1.3/src/
--rw-rw-rw-   0        0        0        0 2024-05-27 16:48:26.000000 medium_article_py-0.1.3/src/__init__.py
--rw-rw-rw-   0        0        0     6172 2024-05-27 16:52:49.000000 medium_article_py-0.1.3/src/medium.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:59:23.366080 medium_article_py-0.1.3/test/
--rw-rw-rw-   0        0        0        0 2024-05-27 16:17:19.000000 medium_article_py-0.1.3/test/__init__.py
--rw-rw-rw-   0        0        0      461 2024-05-27 16:56:21.000000 medium_article_py-0.1.3/test/test_medium.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:17:36.030987 medium_article_py-0.1.4/
+-rw-rw-rw-   0        0        0     1092 2024-05-27 16:13:44.000000 medium_article_py-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2527 2024-05-27 20:17:36.030987 medium_article_py-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2024-05-27 20:17:05.000000 medium_article_py-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-27 20:17:36.030987 medium_article_py-0.1.4/medium_article_py.egg-info/
+-rw-rw-rw-   0        0        0     2527 2024-05-27 20:17:35.000000 medium_article_py-0.1.4/medium_article_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-05-27 20:17:35.000000 medium_article_py-0.1.4/medium_article_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:17:35.000000 medium_article_py-0.1.4/medium_article_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 20:17:35.000000 medium_article_py-0.1.4/medium_article_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 20:17:35.000000 medium_article_py-0.1.4/medium_article_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:17:36.046612 medium_article_py-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      796 2024-05-27 20:16:19.000000 medium_article_py-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:17:36.015361 medium_article_py-0.1.4/src/
+-rw-rw-rw-   0        0        0        0 2024-05-27 16:48:26.000000 medium_article_py-0.1.4/src/__init__.py
+-rw-rw-rw-   0        0        0     6172 2024-05-27 16:52:49.000000 medium_article_py-0.1.4/src/medium.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:17:36.030987 medium_article_py-0.1.4/test/
+-rw-rw-rw-   0        0        0        0 2024-05-27 16:17:19.000000 medium_article_py-0.1.4/test/__init__.py
+-rw-rw-rw-   0        0        0      461 2024-05-27 16:56:21.000000 medium_article_py-0.1.4/test/test_medium.py
```

### Comparing `medium_article_py-0.1.3/LICENSE` & `medium_article_py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_article_py-0.1.3/setup.py` & `medium_article_py-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='medium-article-py',
-    version='v0.1.3',
+    version='v0.1.4',
     description='A simple python library for Medium Articles APIs',
     long_description=long_description,
     author='Muhammad Usman',
     author_email='umuhammad202@yahoo.com',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `medium_article_py-0.1.3/src/medium.py` & `medium_article_py-0.1.4/src/medium.py`

 * *Files identical despite different names*

