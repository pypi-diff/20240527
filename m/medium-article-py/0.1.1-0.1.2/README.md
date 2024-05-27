# Comparing `tmp/medium_article_py-0.1.1.tar.gz` & `tmp/medium_article_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_article_py-0.1.1.tar", last modified: Mon May 27 19:46:34 2024, max compression
+gzip compressed data, was "medium_article_py-0.1.2.tar", last modified: Mon May 27 19:51:57 2024, max compression
```

## Comparing `medium_article_py-0.1.1.tar` & `medium_article_py-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 19:46:34.341363 medium_article_py-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-05-27 16:13:44.000000 medium_article_py-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      746 2024-05-27 19:46:34.325763 medium_article_py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-27 19:38:26.000000 medium_article_py-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 19:46:34.325763 medium_article_py-0.1.1/medium_article_py.egg-info/
--rw-rw-rw-   0        0        0      746 2024-05-27 19:46:34.000000 medium_article_py-0.1.1/medium_article_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-05-27 19:46:34.000000 medium_article_py-0.1.1/medium_article_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 19:46:34.000000 medium_article_py-0.1.1/medium_article_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 19:46:34.000000 medium_article_py-0.1.1/medium_article_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 19:46:34.000000 medium_article_py-0.1.1/medium_article_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 19:46:34.341363 medium_article_py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      795 2024-05-27 19:31:55.000000 medium_article_py-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:46:34.325763 medium_article_py-0.1.1/src/
--rw-rw-rw-   0        0        0        0 2024-05-27 16:48:26.000000 medium_article_py-0.1.1/src/__init__.py
--rw-rw-rw-   0        0        0     6172 2024-05-27 16:52:49.000000 medium_article_py-0.1.1/src/medium.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:46:34.325763 medium_article_py-0.1.1/test/
--rw-rw-rw-   0        0        0        0 2024-05-27 16:17:19.000000 medium_article_py-0.1.1/test/__init__.py
--rw-rw-rw-   0        0        0      461 2024-05-27 16:56:21.000000 medium_article_py-0.1.1/test/test_medium.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:51:57.717185 medium_article_py-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2024-05-27 16:13:44.000000 medium_article_py-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      746 2024-05-27 19:51:57.717185 medium_article_py-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-27 19:38:26.000000 medium_article_py-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-27 19:51:57.717185 medium_article_py-0.1.2/medium_article_py.egg-info/
+-rw-rw-rw-   0        0        0      746 2024-05-27 19:51:57.000000 medium_article_py-0.1.2/medium_article_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-05-27 19:51:57.000000 medium_article_py-0.1.2/medium_article_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 19:51:57.000000 medium_article_py-0.1.2/medium_article_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 19:51:57.000000 medium_article_py-0.1.2/medium_article_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 19:51:57.000000 medium_article_py-0.1.2/medium_article_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 19:51:57.717185 medium_article_py-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      796 2024-05-27 19:51:18.000000 medium_article_py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:51:57.701044 medium_article_py-0.1.2/src/
+-rw-rw-rw-   0        0        0        0 2024-05-27 16:48:26.000000 medium_article_py-0.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     6172 2024-05-27 16:52:49.000000 medium_article_py-0.1.2/src/medium.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:51:57.717185 medium_article_py-0.1.2/test/
+-rw-rw-rw-   0        0        0        0 2024-05-27 16:17:19.000000 medium_article_py-0.1.2/test/__init__.py
+-rw-rw-rw-   0        0        0      461 2024-05-27 16:56:21.000000 medium_article_py-0.1.2/test/test_medium.py
```

### Comparing `medium_article_py-0.1.1/LICENSE` & `medium_article_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_article_py-0.1.1/PKG-INFO` & `medium_article_py-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-article-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple python library for Medium Articles APIs
 Download-URL: https://github.com/muhammad-usman-108/medium-article-py.git
 Author: Muhammad Usman
 Author-email: umuhammad202@yahoo.com
 Keywords: medium,medium-api,medium-article,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `medium_article_py-0.1.1/medium_article_py.egg-info/PKG-INFO` & `medium_article_py-0.1.2/medium_article_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-article-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple python library for Medium Articles APIs
 Download-URL: https://github.com/muhammad-usman-108/medium-article-py.git
 Author: Muhammad Usman
 Author-email: umuhammad202@yahoo.com
 Keywords: medium,medium-api,medium-article,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `medium_article_py-0.1.1/setup.py` & `medium_article_py-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='medium-article-py',
-    version='v0.1.1',
+    version='v0.1.2',
     description='A simple python library for Medium Articles APIs',
     long_description=long_description,
     author='Muhammad Usman',
     author_email='umuhammad202@yahoo.com',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `medium_article_py-0.1.1/src/medium.py` & `medium_article_py-0.1.2/src/medium.py`

 * *Files identical despite different names*

