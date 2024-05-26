# Comparing `tmp/alxhttp-0.9.8.tar.gz` & `tmp/alxhttp-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alxhttp-0.9.8.tar", last modified: Sat Mar 23 23:09:59 2024, max compression
+gzip compressed data, was "alxhttp-0.9.9.tar", last modified: Sat Mar 23 23:21:29 2024, max compression
```

## Comparing `alxhttp-0.9.8.tar` & `alxhttp-0.9.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-23 23:09:59.357571 alxhttp-0.9.8/
--rw-r--r--   0 alex       (501) staff       (20)     1076 2024-01-17 08:18:31.000000 alxhttp-0.9.8/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       12 2024-01-17 08:52:08.000000 alxhttp-0.9.8/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)      745 2024-03-23 23:09:59.357373 alxhttp-0.9.8/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      209 2024-03-23 23:08:58.000000 alxhttp-0.9.8/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-23 23:09:59.356061 alxhttp-0.9.8/alxhttp/
--rw-r--r--   0 alex       (501) staff       (20)        0 2024-01-17 08:20:44.000000 alxhttp-0.9.8/alxhttp/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      207 2024-02-04 02:04:38.000000 alxhttp-0.9.8/alxhttp/file.py
--rw-r--r--   0 alex       (501) staff       (20)     2638 2024-02-04 02:45:29.000000 alxhttp-0.9.8/alxhttp/headers.py
--rw-r--r--   0 alex       (501) staff       (20)     1469 2024-01-17 08:27:58.000000 alxhttp-0.9.8/alxhttp/logging.py
--rw-r--r--   0 alex       (501) staff       (20)     2411 2024-02-04 01:53:33.000000 alxhttp-0.9.8/alxhttp/middleware.py
--rw-r--r--   0 alex       (501) staff       (20)      350 2024-01-17 08:27:58.000000 alxhttp-0.9.8/alxhttp/req_id.py
--rw-r--r--   0 alex       (501) staff       (20)     1705 2024-02-04 02:14:12.000000 alxhttp-0.9.8/alxhttp/server.py
--rw-r--r--   0 alex       (501) staff       (20)     1251 2024-03-23 22:45:36.000000 alxhttp-0.9.8/alxhttp/xray.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-23 23:09:59.357090 alxhttp-0.9.8/alxhttp.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      745 2024-03-23 23:09:59.000000 alxhttp-0.9.8/alxhttp.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      346 2024-03-23 23:09:59.000000 alxhttp-0.9.8/alxhttp.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-03-23 23:09:59.000000 alxhttp-0.9.8/alxhttp.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       40 2024-03-23 23:09:59.000000 alxhttp-0.9.8/alxhttp.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        8 2024-03-23 23:09:59.000000 alxhttp-0.9.8/alxhttp.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)      630 2024-03-23 22:48:31.000000 alxhttp-0.9.8/pyproject.toml
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-03-23 23:09:59.357607 alxhttp-0.9.8/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-23 23:21:29.629266 alxhttp-0.9.9/
+-rw-r--r--   0 alex       (501) staff       (20)     1076 2024-01-17 08:18:31.000000 alxhttp-0.9.9/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       12 2024-01-17 08:52:08.000000 alxhttp-0.9.9/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)      745 2024-03-23 23:21:29.629073 alxhttp-0.9.9/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      209 2024-03-23 23:08:58.000000 alxhttp-0.9.9/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-23 23:21:29.628013 alxhttp-0.9.9/alxhttp/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2024-01-17 08:20:44.000000 alxhttp-0.9.9/alxhttp/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      207 2024-02-04 02:04:38.000000 alxhttp-0.9.9/alxhttp/file.py
+-rw-r--r--   0 alex       (501) staff       (20)     2638 2024-02-04 02:45:29.000000 alxhttp-0.9.9/alxhttp/headers.py
+-rw-r--r--   0 alex       (501) staff       (20)     1469 2024-01-17 08:27:58.000000 alxhttp-0.9.9/alxhttp/logging.py
+-rw-r--r--   0 alex       (501) staff       (20)     2658 2024-03-23 23:20:58.000000 alxhttp-0.9.9/alxhttp/middleware.py
+-rw-r--r--   0 alex       (501) staff       (20)      350 2024-01-17 08:27:58.000000 alxhttp-0.9.9/alxhttp/req_id.py
+-rw-r--r--   0 alex       (501) staff       (20)     1705 2024-02-04 02:14:12.000000 alxhttp-0.9.9/alxhttp/server.py
+-rw-r--r--   0 alex       (501) staff       (20)     1251 2024-03-23 22:45:36.000000 alxhttp-0.9.9/alxhttp/xray.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-03-23 23:21:29.628810 alxhttp-0.9.9/alxhttp.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      745 2024-03-23 23:21:29.000000 alxhttp-0.9.9/alxhttp.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      346 2024-03-23 23:21:29.000000 alxhttp-0.9.9/alxhttp.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-03-23 23:21:29.000000 alxhttp-0.9.9/alxhttp.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       40 2024-03-23 23:21:29.000000 alxhttp-0.9.9/alxhttp.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        8 2024-03-23 23:21:29.000000 alxhttp-0.9.9/alxhttp.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)      630 2024-03-23 23:21:09.000000 alxhttp-0.9.9/pyproject.toml
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-03-23 23:21:29.629306 alxhttp-0.9.9/setup.cfg
```

### Comparing `alxhttp-0.9.8/LICENSE` & `alxhttp-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alxhttp-0.9.8/PKG-INFO` & `alxhttp-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alxhttp
-Version: 0.9.8
+Version: 0.9.9
 Summary: A better base server for AioHTTP
 Author-email: Alexander Macdonald <alex@alexmac.cc>
 Project-URL: Homepage, https://github.com/alexmac/alxhttp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `alxhttp-0.9.8/alxhttp/headers.py` & `alxhttp-0.9.9/alxhttp/headers.py`

 * *Files identical despite different names*

### Comparing `alxhttp-0.9.8/alxhttp/logging.py` & `alxhttp-0.9.9/alxhttp/logging.py`

 * *Files identical despite different names*

### Comparing `alxhttp-0.9.8/alxhttp/middleware.py` & `alxhttp-0.9.9/alxhttp/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from aiohttp.typedefs import Handler, Middleware
 from aiohttp.web import HTTPException, Request, json_response, middleware
 from multidict import CIMultiDict
 from alxhttp.headers import content_security_policy
 
 from alxhttp.req_id import get_request_id, set_request_id
 
+try:
+    from aws_xray_sdk.ext.aiohttp.middleware import middleware as xray_middleware
+except ImportError:
+    xray_middleware = None
+
 
 def _apply_security_header_defaults(headers: CIMultiDict[str]) -> None:
     if "content-security-policy" not in headers:
         headers["content-security-policy"] = content_security_policy(
             default_src=["self"]
         )
     if "x-content-type-options" not in headers:
@@ -69,8 +74,13 @@
 @middleware
 async def assign_req_id(request: Request, handler: Handler):
     set_request_id(request)
     return await handler(request)
 
 
 def default_middleware() -> List[Middleware]:
-    return [assign_req_id, default_security_headers, unhandled_error_handler]
+    middlewares = [assign_req_id, default_security_headers, unhandled_error_handler]
+
+    if xray_middleware is not None:
+        middlewares.append(xray_middleware)
+
+    return middlewares
```

### Comparing `alxhttp-0.9.8/alxhttp/server.py` & `alxhttp-0.9.9/alxhttp/server.py`

 * *Files identical despite different names*

### Comparing `alxhttp-0.9.8/alxhttp/xray.py` & `alxhttp-0.9.9/alxhttp/xray.py`

 * *Files identical despite different names*

### Comparing `alxhttp-0.9.8/alxhttp.egg-info/PKG-INFO` & `alxhttp-0.9.9/alxhttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alxhttp
-Version: 0.9.8
+Version: 0.9.9
 Summary: A better base server for AioHTTP
 Author-email: Alexander Macdonald <alex@alexmac.cc>
 Project-URL: Homepage, https://github.com/alexmac/alxhttp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `alxhttp-0.9.8/pyproject.toml` & `alxhttp-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alxhttp"
-version = "0.9.8"
+version = "0.9.9"
 authors = [
   { name="Alexander Macdonald", email="alex@alexmac.cc" },
 ]
 description = "A better base server for AioHTTP"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

