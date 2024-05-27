# Comparing `tmp/ssvc-1.0.7.tar.gz` & `tmp/ssvc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssvc-1.0.7.tar", max compression
+gzip compressed data, was "ssvc-1.0.8.tar", max compression
```

## Comparing `ssvc-1.0.7.tar` & `ssvc-1.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2024-03-25 11:16:25.817155 ssvc-1.0.7/LICENSE
--rw-r--r--   0        0        0     1949 2024-04-18 11:26:03.741779 ssvc-1.0.7/PYPI.md
--rw-r--r--   0        0        0      640 2024-05-21 11:41:57.123951 ssvc-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     6463 2024-04-18 11:26:03.748446 ssvc-1.0.7/src/ssvc/__init__.py
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 ssvc-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-25 11:16:25.817155 ssvc-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1949 2024-04-18 11:26:03.741779 ssvc-1.0.8/PYPI.md
+-rw-r--r--   0        0        0      639 2024-05-27 12:30:12.541319 ssvc-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6463 2024-04-18 11:26:03.748446 ssvc-1.0.8/src/ssvc/__init__.py
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 ssvc-1.0.8/PKG-INFO
```

### Comparing `ssvc-1.0.7/LICENSE` & `ssvc-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.7/PYPI.md` & `ssvc-1.0.8/PYPI.md`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.7/pyproject.toml` & `ssvc-1.0.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "ssvc"
-version = "1.0.7"
+version = "1.0.8"
 description = "A Python implementation of the Stakeholder-Specific Vulnerability Categorization framework."
 authors = ["Christopher Langton <chris@langton.cloud>"]
 readme = "PYPI.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.dev-dependencies]
 setuptools = "^69.5.1"
-uv = "^0.1.44"
+uv = "^0.2.4"
 isort = "^5.13.2"
 pytest = "^8.2.1"
 pytest-cov = "^5.0.0"
 coverage-badge = "^1.1.1"
-ruff = "^0.4.3"
+ruff = "^0.4.5"
 poetry = "^1.8.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
```

### Comparing `ssvc-1.0.7/src/ssvc/__init__.py` & `ssvc-1.0.8/src/ssvc/__init__.py`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.7/PKG-INFO` & `ssvc-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssvc
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python implementation of the Stakeholder-Specific Vulnerability Categorization framework.
 Author: Christopher Langton
 Author-email: chris@langton.cloud
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

