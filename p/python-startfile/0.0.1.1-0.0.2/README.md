# Comparing `tmp/python_startfile-0.0.1.1.tar.gz` & `tmp/python_startfile-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_startfile-0.0.1.1.tar", max compression
+gzip compressed data, was "python_startfile-0.0.2.tar", max compression
```

## Comparing `python_startfile-0.0.1.1.tar` & `python_startfile-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_startfile-0.0.1.1/LICENSE
--rw-r--r--   0        0        0      961 2024-04-30 08:51:56.932894 python_startfile-0.0.1.1/pyproject.toml
--rw-r--r--   0        0        0      567 2024-04-30 08:49:18.655738 python_startfile-0.0.1.1/readme.md
--rwxr-xr-x   0        0        0     2286 2024-04-30 08:51:23.427355 python_startfile-0.0.1.1/startfile.py
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 python_startfile-0.0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_startfile-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1062 2024-05-27 07:37:37.160949 python_startfile-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-05-27 07:37:30.371142 python_startfile-0.0.2/readme.md
+-rwxr-xr-x   0        0        0     1580 2024-05-27 07:35:24.036252 python_startfile-0.0.2/startfile/__init__.py
+-rwxr-xr-x   0        0        0      850 2024-05-27 07:34:44.021433 python_startfile-0.0.2/startfile/__main__.py
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 python_startfile-0.0.2/PKG-INFO
```

### Comparing `python_startfile-0.0.1.1/LICENSE` & `python_startfile-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_startfile-0.0.1.1/pyproject.toml` & `python_startfile-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-startfile"
-version = "0.0.1.1"
+version = "0.0.2"
 description = "Python startfile."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-startfile"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-startfile"
 keywords = ["startfile"]
@@ -18,13 +18,17 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
 ]
 
+[tool.poetry.scripts]
+python-startfile = "startfile.__main__:main"
+startfile = "startfile.__main__:main"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
-include = "startfile.py"
+include = "startfile"
```

### Comparing `python_startfile-0.0.1.1/readme.md` & `python_startfile-0.0.2/readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ```python
 >>> from startfile import startfile, startfile_async
 ```
 
 ### Commad
 
 ```console
-$ python -m startfile -h
+$ startfile -h
 usage: startfile.py [-h] [-v] [path ...]
 
 Start file(s) with its/their associated application.
 
 positional arguments:
   path           paths to files or directories
```

### Comparing `python_startfile-0.0.1.1/PKG-INFO` & `python_startfile-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-startfile
-Version: 0.0.1.1
+Version: 0.0.2
 Summary: Python startfile.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-startfile
 License: MIT
 Keywords: startfile
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
@@ -47,15 +47,15 @@
 ```python
 >>> from startfile import startfile, startfile_async
 ```
 
 ### Commad
 
 ```console
-$ python -m startfile -h
+$ startfile -h
 usage: startfile.py [-h] [-v] [path ...]
 
 Start file(s) with its/their associated application.
 
 positional arguments:
   path           paths to files or directories
```

