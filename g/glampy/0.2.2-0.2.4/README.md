# Comparing `tmp/glampy-0.2.2.tar.gz` & `tmp/glampy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glampy-0.2.2.tar", max compression
+gzip compressed data, was "glampy-0.2.4.tar", max compression
```

## Comparing `glampy-0.2.2.tar` & `glampy-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1830 2024-05-15 20:20:43.808432 glampy-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-15 20:20:43.808432 glampy-0.2.2/glampy/__init__.py
--rw-r--r--   0        0        0     2304 2024-05-15 20:20:43.808432 glampy-0.2.2/glampy/io.py
--rw-r--r--   0        0        0     3928 2024-05-15 20:20:43.812432 glampy-0.2.2/glampy/logging.py
--rw-r--r--   0        0        0     1291 2024-05-15 20:20:43.812432 glampy-0.2.2/glampy/style.py
--rw-r--r--   0        0        0     1108 2024-05-15 20:20:43.812432 glampy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 glampy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1830 2024-05-27 09:52:35.665309 glampy-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 09:52:35.665309 glampy-0.2.4/glampy/__init__.py
+-rw-r--r--   0        0        0     2304 2024-05-27 09:52:35.665309 glampy-0.2.4/glampy/io.py
+-rw-r--r--   0        0        0     3928 2024-05-27 09:52:35.665309 glampy-0.2.4/glampy/logging.py
+-rw-r--r--   0        0        0     1291 2024-05-27 09:52:35.665309 glampy-0.2.4/glampy/style.py
+-rw-r--r--   0        0        0     1152 2024-05-27 09:52:35.665309 glampy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2839 1970-01-01 00:00:00.000000 glampy-0.2.4/PKG-INFO
```

### Comparing `glampy-0.2.2/README.md` & `glampy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `glampy-0.2.2/glampy/io.py` & `glampy-0.2.4/glampy/io.py`

 * *Files identical despite different names*

### Comparing `glampy-0.2.2/glampy/logging.py` & `glampy-0.2.4/glampy/logging.py`

 * *Files identical despite different names*

### Comparing `glampy-0.2.2/glampy/style.py` & `glampy-0.2.4/glampy/style.py`

 * *Files identical despite different names*

### Comparing `glampy-0.2.2/pyproject.toml` & `glampy-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "glampy"
-version = "0.2.2"
+version = "0.2.4"
 description = "Make your python CLI prints and logs simple but glamorous"
 authors = ["snaeil <schnegel@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/snaeil/glampy"
 repository = "https://github.com/snaeil/glampy"
 keywords = ["cli", "logging", "styling", "terminal"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
+  "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 pytest-cov = "^5.0.0"
 mypy = "^1.10.0"
 pdoc = "^14.4.0"
 bandit = "^1.7.8"
```

### Comparing `glampy-0.2.2/PKG-INFO` & `glampy-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: glampy
-Version: 0.2.2
+Version: 0.2.4
 Summary: Make your python CLI prints and logs simple but glamorous
 Home-page: https://github.com/snaeil/glampy
 License: MIT
 Keywords: cli,logging,styling,terminal
 Author: snaeil
 Author-email: schnegel@posteo.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Project-URL: Bug Tracker, https://github.com/snaeil/glampy/issues
 Project-URL: Repository, https://github.com/snaeil/glampy
 Description-Content-Type: text/markdown
```

