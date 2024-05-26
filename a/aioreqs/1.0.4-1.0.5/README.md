# Comparing `tmp/aioreqs-1.0.4.tar.gz` & `tmp/aioreqs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioreqs-1.0.4.tar", max compression
+gzip compressed data, was "aioreqs-1.0.5.tar", max compression
```

## Comparing `aioreqs-1.0.4.tar` & `aioreqs-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4965 2024-05-26 23:05:02.485182 aioreqs-1.0.4/aioreqs/__init__.py
--rw-r--r--   0        0        0     2384 2024-05-26 21:21:29.286601 aioreqs-1.0.4/aioreqs/sync/__init__.py
--rw-r--r--   0        0        0      333 2024-05-26 23:21:43.030460 aioreqs-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-26 21:16:45.746607 aioreqs-1.0.4/README.md
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 aioreqs-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4997 2024-05-26 23:24:00.470126 aioreqs-1.0.5/aioreqs/__init__.py
+-rw-r--r--   0        0        0     2384 2024-05-26 21:21:29.286601 aioreqs-1.0.5/aioreqs/sync/__init__.py
+-rw-r--r--   0        0        0      333 2024-05-26 23:24:18.209231 aioreqs-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-26 21:16:45.746607 aioreqs-1.0.5/README.md
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 aioreqs-1.0.5/PKG-INFO
```

### Comparing `aioreqs-1.0.4/aioreqs/__init__.py` & `aioreqs-1.0.5/aioreqs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import typing
 import asyncio
 import requests
 import functools
 import concurrent.futures
 
+# Local imports
+import sync
+
 
 # ==------------------------------------------------------------== #
 # Decorators                                                       #
 # ==------------------------------------------------------------== #
 def coroutine(func: callable = None, *, pool: concurrent.futures.ThreadPoolExecutor | None = None):
 
     def outer_wrapper(wrapped_func: callable):
```

### Comparing `aioreqs-1.0.4/aioreqs/sync/__init__.py` & `aioreqs-1.0.5/aioreqs/sync/__init__.py`

 * *Files identical despite different names*

