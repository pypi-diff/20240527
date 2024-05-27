# Comparing `tmp/approck_fastapi_utils-0.1.5.tar.gz` & `tmp/approck_fastapi_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_fastapi_utils-0.1.5.tar", max compression
+gzip compressed data, was "approck_fastapi_utils-0.1.6.tar", max compression
```

## Comparing `approck_fastapi_utils-0.1.5.tar` & `approck_fastapi_utils-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-05-15 11:40:19.883242 approck_fastapi_utils-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-15 11:40:19.883242 approck_fastapi_utils-0.1.5/approck_fastapi_utils/__init__.py
--rw-r--r--   0        0        0      271 2024-05-15 11:40:19.849243 approck_fastapi_utils-0.1.5/approck_fastapi_utils/auth.py
--rw-r--r--   0        0        0     1130 2024-05-15 11:40:19.849243 approck_fastapi_utils-0.1.5/approck_fastapi_utils/exception_handlers.py
--rw-r--r--   0        0        0      180 2024-05-15 11:40:19.849243 approck_fastapi_utils-0.1.5/approck_fastapi_utils/exceptions.py
--rw-r--r--   0        0        0      325 2024-05-15 11:40:19.850242 approck_fastapi_utils-0.1.5/approck_fastapi_utils/jwt.py
--rw-r--r--   0        0        0      212 2024-05-15 11:40:19.850242 approck_fastapi_utils-0.1.5/approck_fastapi_utils/response.py
--rw-r--r--   0        0        0     1991 2024-05-15 11:40:19.850242 approck_fastapi_utils-0.1.5/approck_fastapi_utils/responses.py
--rw-r--r--   0        0        0        0 2024-05-15 11:40:19.883242 approck_fastapi_utils-0.1.5/approck_fastapi_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      637 2024-05-15 11:40:19.850242 approck_fastapi_utils-0.1.5/approck_fastapi_utils/sqlalchemy/exception_handlers.py
--rw-r--r--   0        0        0     1425 2024-05-15 11:40:19.850242 approck_fastapi_utils-0.1.5/approck_fastapi_utils/types.py
--rw-r--r--   0        0        0      426 2024-05-15 11:40:19.851242 approck_fastapi_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 approck_fastapi_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-27 12:17:33.839905 approck_fastapi_utils-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 12:17:33.840905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0      271 2024-05-27 12:17:33.806905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/auth.py
+-rw-r--r--   0        0        0     1130 2024-05-27 12:17:33.806905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/exception_handlers.py
+-rw-r--r--   0        0        0      180 2024-05-27 12:17:33.806905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/exceptions.py
+-rw-r--r--   0        0        0      325 2024-05-27 12:17:33.807905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/jwt.py
+-rw-r--r--   0        0        0      212 2024-05-27 12:17:33.807905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/response.py
+-rw-r--r--   0        0        0     1991 2024-05-27 12:17:33.807905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/responses.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:17:33.840905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-27 12:17:33.807905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/sqlalchemy/exception_handlers.py
+-rw-r--r--   0        0        0     1425 2024-05-27 12:17:33.807905 approck_fastapi_utils-0.1.6/approck_fastapi_utils/types.py
+-rw-r--r--   0        0        0      427 2024-05-27 12:17:33.808905 approck_fastapi_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 approck_fastapi_utils-0.1.6/PKG-INFO
```

### Comparing `approck_fastapi_utils-0.1.5/approck_fastapi_utils/exception_handlers.py` & `approck_fastapi_utils-0.1.6/approck_fastapi_utils/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `approck_fastapi_utils-0.1.5/approck_fastapi_utils/responses.py` & `approck_fastapi_utils-0.1.6/approck_fastapi_utils/responses.py`

 * *Files identical despite different names*

### Comparing `approck_fastapi_utils-0.1.5/approck_fastapi_utils/sqlalchemy/exception_handlers.py` & `approck_fastapi_utils-0.1.6/approck_fastapi_utils/sqlalchemy/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `approck_fastapi_utils-0.1.5/approck_fastapi_utils/types.py` & `approck_fastapi_utils-0.1.6/approck_fastapi_utils/types.py`

 * *Files identical despite different names*

