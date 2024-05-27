# Comparing `tmp/approck_services-0.1.0.tar.gz` & `tmp/approck_services-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_services-0.1.0.tar", max compression
+gzip compressed data, was "approck_services-0.1.1.tar", max compression
```

## Comparing `approck_services-0.1.0.tar` & `approck_services-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-02-16 11:22:36.984809 approck_services-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-02-16 11:22:36.984809 approck_services-0.1.0/approck_services/__init__.py
--rw-r--r--   0        0        0       28 2024-02-16 11:22:36.960809 approck_services-0.1.0/approck_services/base.py
--rw-r--r--   0        0        0      367 2024-02-16 11:22:36.960809 approck_services-0.1.0/approck_services/fastapi.py
--rw-r--r--   0        0        0        0 2024-02-16 11:22:36.984809 approck_services-0.1.0/approck_services/integrations/__init__.py
--rw-r--r--   0        0        0     3230 2024-02-16 11:22:36.960809 approck_services-0.1.0/approck_services/integrations/term.py
--rw-r--r--   0        0        0     1216 2024-02-16 11:22:36.960809 approck_services-0.1.0/approck_services/integrations/upload.py
--rw-r--r--   0        0        0     3318 2024-02-16 11:22:36.960809 approck_services-0.1.0/approck_services/sqlalchemy.py
--rw-r--r--   0        0        0      874 2024-02-16 11:22:36.961809 approck_services-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 approck_services-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-27 12:07:43.926687 approck_services-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 12:07:43.927687 approck_services-0.1.1/approck_services/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-27 12:07:43.894688 approck_services-0.1.1/approck_services/base.py
+-rw-r--r--   0        0        0      367 2024-05-27 12:07:43.894688 approck_services-0.1.1/approck_services/fastapi.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:07:43.927687 approck_services-0.1.1/approck_services/integrations/__init__.py
+-rw-r--r--   0        0        0     3230 2024-05-27 12:07:43.894688 approck_services-0.1.1/approck_services/integrations/term.py
+-rw-r--r--   0        0        0     1216 2024-05-27 12:07:43.894688 approck_services-0.1.1/approck_services/integrations/upload.py
+-rw-r--r--   0        0        0     3318 2024-05-27 12:07:43.895687 approck_services-0.1.1/approck_services/sqlalchemy.py
+-rw-r--r--   0        0        0      874 2024-05-27 12:07:43.896687 approck_services-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 approck_services-0.1.1/PKG-INFO
```

### Comparing `approck_services-0.1.0/approck_services/integrations/term.py` & `approck_services-0.1.1/approck_services/integrations/term.py`

 * *Files identical despite different names*

### Comparing `approck_services-0.1.0/approck_services/integrations/upload.py` & `approck_services-0.1.1/approck_services/integrations/upload.py`

 * *Files identical despite different names*

### Comparing `approck_services-0.1.0/approck_services/sqlalchemy.py` & `approck_services-0.1.1/approck_services/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `approck_services-0.1.0/pyproject.toml` & `approck_services-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "approck-services"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Aleksey Dalekin <adalekin@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aioboto3 = { version = "^11.2.0", optional = true }
 approck-sqlalchemy-utils = { version = "^0.1.0", extras = [
     "postgres",
 ], optional = true }
-fastapi = { version = "^0.109.2", optional = true }
+fastapi = { version = "^0.111.0", optional = true }
 html-sanitizer = { version = "^2.3.0", optional = true }
 httpx = { version = "^0.26.0", optional = true }
 multimethod = "^1.11"
 python = "^3.10"
 
 [tool.poetry.extras]
 fastapi = ["fastapi"]
```

### Comparing `approck_services-0.1.0/PKG-INFO` & `approck_services-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: approck-services
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Aleksey Dalekin
 Author-email: adalekin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fastapi
 Provides-Extra: sqlalchemy
 Provides-Extra: term
 Provides-Extra: upload
 Requires-Dist: aioboto3 (>=11.2.0,<12.0.0) ; extra == "upload"
 Requires-Dist: approck-sqlalchemy-utils[postgres] (>=0.1.0,<0.2.0) ; extra == "sqlalchemy"
-Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "fastapi"
+Requires-Dist: fastapi (>=0.111.0,<0.112.0) ; extra == "fastapi"
 Requires-Dist: html-sanitizer (>=2.3.0,<3.0.0) ; extra == "term"
 Requires-Dist: httpx (>=0.26.0,<0.27.0) ; extra == "term"
 Requires-Dist: multimethod (>=1.11,<2.0)
 Description-Content-Type: text/markdown
```

