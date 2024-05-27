# Comparing `tmp/allnc-0.1.1.tar.gz` & `tmp/allnc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allnc-0.1.1.tar", last modified: Mon May 27 10:10:55 2024, max compression
+gzip compressed data, was "allnc-0.1.2.tar", last modified: Mon May 27 10:35:48 2024, max compression
```

## Comparing `allnc-0.1.1.tar` & `allnc-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:10:55.254775 allnc-0.1.1/
--rw-r--r--   0 msi       (1000) msi       (1000)     7232 2024-05-27 10:10:55.254775 allnc-0.1.1/PKG-INFO
--rw-rw-r--   0 msi       (1000) msi       (1000)     6400 2024-05-27 10:00:57.000000 allnc-0.1.1/README.md
-drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:10:55.254775 allnc-0.1.1/allnc/
--rw-rw-r--   0 msi       (1000) msi       (1000)        0 2024-05-26 11:34:50.000000 allnc-0.1.1/allnc/__init__.py
--rw-rw-r--   0 msi       (1000) msi       (1000)     3749 2024-05-26 11:35:28.000000 allnc-0.1.1/allnc/app.py
--rw-rw-r--   0 msi       (1000) msi       (1000)      675 2024-05-23 14:36:01.000000 allnc-0.1.1/allnc/middleware.py
--rw-rw-r--   0 msi       (1000) msi       (1000)      944 2024-05-25 10:24:58.000000 allnc-0.1.1/allnc/response.py
-drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:10:55.254775 allnc-0.1.1/allnc.egg-info/
--rw-r--r--   0 msi       (1000) msi       (1000)     7232 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/PKG-INFO
--rw-rw-r--   0 msi       (1000) msi       (1000)      231 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/SOURCES.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)        1 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/dependency_links.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)      105 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/requires.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)        6 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/top_level.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)       38 2024-05-27 10:10:55.254775 allnc-0.1.1/setup.cfg
--rw-rw-r--   0 msi       (1000) msi       (1000)     3920 2024-05-27 10:10:31.000000 allnc-0.1.1/setup.py
+drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:35:48.298740 allnc-0.1.2/
+-rw-r--r--   0 msi       (1000) msi       (1000)     7230 2024-05-27 10:35:48.298740 allnc-0.1.2/PKG-INFO
+-rw-rw-r--   0 msi       (1000) msi       (1000)     6398 2024-05-27 10:30:23.000000 allnc-0.1.2/README.md
+drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:35:48.294740 allnc-0.1.2/allnc/
+-rw-rw-r--   0 msi       (1000) msi       (1000)        0 2024-05-26 11:34:50.000000 allnc-0.1.2/allnc/__init__.py
+-rw-rw-r--   0 msi       (1000) msi       (1000)     3749 2024-05-26 11:35:28.000000 allnc-0.1.2/allnc/app.py
+-rw-rw-r--   0 msi       (1000) msi       (1000)      675 2024-05-23 14:36:01.000000 allnc-0.1.2/allnc/middleware.py
+-rw-rw-r--   0 msi       (1000) msi       (1000)      944 2024-05-25 10:24:58.000000 allnc-0.1.2/allnc/response.py
+drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:35:48.298740 allnc-0.1.2/allnc.egg-info/
+-rw-r--r--   0 msi       (1000) msi       (1000)     7230 2024-05-27 10:35:48.000000 allnc-0.1.2/allnc.egg-info/PKG-INFO
+-rw-rw-r--   0 msi       (1000) msi       (1000)      231 2024-05-27 10:35:48.000000 allnc-0.1.2/allnc.egg-info/SOURCES.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)        1 2024-05-27 10:35:48.000000 allnc-0.1.2/allnc.egg-info/dependency_links.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)      105 2024-05-27 10:35:48.000000 allnc-0.1.2/allnc.egg-info/requires.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)        6 2024-05-27 10:35:48.000000 allnc-0.1.2/allnc.egg-info/top_level.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)       38 2024-05-27 10:35:48.298740 allnc-0.1.2/setup.cfg
+-rw-rw-r--   0 msi       (1000) msi       (1000)     3920 2024-05-27 10:35:18.000000 allnc-0.1.2/setup.py
```

### Comparing `allnc-0.1.1/PKG-INFO` & `allnc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allnc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Web Framework for building web applications
 Home-page: https://github.com/themusharraf/allnc
 Author: Musharraf Ibragimov
 Author-email: meibrohimov@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -126,15 +126,15 @@
 ```
 
 Note that if you specify `methods` for class based handlers, they will be ignored.
 
 ## Unit Tests
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
-that you may want to use when writing unit tests with Alcazar. The first one is `app` which is an instance of the main `AllNc` class:
+that you may want to use when writing unit tests with AllNc. The first one is `app` which is an instance of the main `AllNc` class:
 
 ```python
 def test_route_overlap_throws_exception(app):
     @app.route("/")
     def home(req, resp):
         resp.text = "Welcome Home."
```

### Comparing `allnc-0.1.1/README.md` & `allnc-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 ```
 
 Note that if you specify `methods` for class based handlers, they will be ignored.
 
 ## Unit Tests
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
-that you may want to use when writing unit tests with Alcazar. The first one is `app` which is an instance of the main `AllNc` class:
+that you may want to use when writing unit tests with AllNc. The first one is `app` which is an instance of the main `AllNc` class:
 
 ```python
 def test_route_overlap_throws_exception(app):
     @app.route("/")
     def home(req, resp):
         resp.text = "Welcome Home."
```

### Comparing `allnc-0.1.1/allnc/app.py` & `allnc-0.1.2/allnc/app.py`

 * *Files identical despite different names*

### Comparing `allnc-0.1.1/allnc/middleware.py` & `allnc-0.1.2/allnc/middleware.py`

 * *Files identical despite different names*

### Comparing `allnc-0.1.1/allnc/response.py` & `allnc-0.1.2/allnc/response.py`

 * *Files identical despite different names*

### Comparing `allnc-0.1.1/allnc.egg-info/PKG-INFO` & `allnc-0.1.2/allnc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allnc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Web Framework for building web applications
 Home-page: https://github.com/themusharraf/allnc
 Author: Musharraf Ibragimov
 Author-email: meibrohimov@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -126,15 +126,15 @@
 ```
 
 Note that if you specify `methods` for class based handlers, they will be ignored.
 
 ## Unit Tests
 
 The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
-that you may want to use when writing unit tests with Alcazar. The first one is `app` which is an instance of the main `AllNc` class:
+that you may want to use when writing unit tests with AllNc. The first one is `app` which is an instance of the main `AllNc` class:
 
 ```python
 def test_route_overlap_throws_exception(app):
     @app.route("/")
     def home(req, resp):
         resp.text = "Welcome Home."
```

### Comparing `allnc-0.1.1/setup.py` & `allnc-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'allnc'
 DESCRIPTION = 'Python Web Framework for building web applications'
 URL = 'https://github.com/themusharraf/allnc'
 EMAIL = 'meibrohimov@gmail.com'
 AUTHOR = 'Musharraf Ibragimov'
 REQUIRES_PYTHON = '>=3.11.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'Jinja2==3.1.4',
     'parse==1.20.1',
     'requests==2.31.0',
     'requests-wsgi-adapter==0.4.1',
```

