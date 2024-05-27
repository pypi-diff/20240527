# Comparing `tmp/audiconnectpy-2.2.6.tar.gz` & `tmp/audiconnectpy-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.2.6.tar", last modified: Mon May 20 17:22:43 2024, max compression
+gzip compressed data, was "audiconnectpy-2.2.7.tar", last modified: Mon May 27 12:36:23 2024, max compression
```

## Comparing `audiconnectpy-2.2.6.tar` & `audiconnectpy-2.2.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.239278 audiconnectpy-2.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.235278 audiconnectpy-2.2.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.235278 audiconnectpy-2.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.235278 audiconnectpy-2.2.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 17:22:43.239278 audiconnectpy-2.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.239278 audiconnectpy-2.2.6/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23299 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.239278 audiconnectpy-2.2.6/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 17:22:43.000000 audiconnectpy-2.2.6/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-20 17:22:43.000000 audiconnectpy-2.2.6/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:22:43.000000 audiconnectpy-2.2.6/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:22:42.000000 audiconnectpy-2.2.6/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 17:22:43.000000 audiconnectpy-2.2.6/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 17:22:43.000000 audiconnectpy-2.2.6/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 17:22:43.239278 audiconnectpy-2.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.239278 audiconnectpy-2.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:22:43.239278 audiconnectpy-2.2.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/fixtures/audi1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/fixtures/audi2.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-20 17:22:32.000000 audiconnectpy-2.2.6/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.850142 audiconnectpy-2.2.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.850142 audiconnectpy-2.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.850142 audiconnectpy-2.2.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26610 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 12:36:23.000000 audiconnectpy-2.2.7/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:36:23.854142 audiconnectpy-2.2.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-27 12:36:13.000000 audiconnectpy-2.2.7/tests/test_home.py
```

### Comparing `audiconnectpy-2.2.6/.github/dependabot.yml` & `audiconnectpy-2.2.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/.github/workflows/auto-approve.yml` & `audiconnectpy-2.2.7/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.2.7/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.2.7/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/.github/workflows/release.yml` & `audiconnectpy-2.2.7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/.gitignore` & `audiconnectpy-2.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/.pre-commit-config.yaml` & `audiconnectpy-2.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/LICENSE` & `audiconnectpy-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/PKG-INFO` & `audiconnectpy-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.6
+Version: 2.2.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.6/README.md` & `audiconnectpy-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/audiconnectpy/api.py` & `audiconnectpy-2.2.7/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/audiconnectpy/auth.py` & `audiconnectpy-2.2.7/audiconnectpy/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 import re
 import socket
 from typing import Any, Literal
 from urllib.parse import parse_qs, urlencode, urlparse
 import uuid
 
-from aiohttp import ClientError, ClientSession
+from aiohttp import ClientError, ClientResponseError, ClientSession
 import async_timeout
 from bs4 import BeautifulSoup
 
 from .const import (
     CLIENT_IDS,
     DELAY,
     HDR_USER_AGENT,
@@ -82,44 +82,42 @@
         raw_reply: bool = False,
         raw_rsp: bool = False,
         **kwargs: Any,
     ) -> Any:
         """Request url with method."""
         try:
             async with async_timeout.timeout(TIMEOUT):
-                _LOGGER.debug("REQUEST HEADERS: %s", kwargs.get("headers"))
-                _LOGGER.debug("REQUEST: %s", url)
-                _LOGGER.debug("REQUEST DATA:%s", kwargs.get("data"))
+                _LOGGER.debug("Request - Header: %s", kwargs.get("headers"))
+                _LOGGER.debug("Request: %s (%s) - %s", url, method, kwargs.get("data"))
                 response = await self._session.request(method, url, **kwargs)
+                contents = (await response.read()).decode("utf8")
+                response.raise_for_status()
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Audi Connect."
             ) from error
+        except ClientResponseError as error:
+            if "application/json" in response.headers.get("Content-Type", ""):
+                raise ServiceNotFoundError(
+                    response.status, json.loads(contents)
+                ) from error
+            raise ServiceNotFoundError(response.status, contents) from error
         except (ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with Audi Connect."
             ) from error
 
-        content_type = response.headers.get("Content-Type", "")
-        contents = (await response.read()).decode("utf8")
-
-        _LOGGER.debug("RESPONSE HEADERS: %s", response.headers)
-        _LOGGER.debug("RESPONSE: %s ,return_code '%s'", contents, response.status)
+        _LOGGER.debug("Response - Headers: %s", response.headers)
+        _LOGGER.debug("Response: %s (%s)", contents, response.status)
         _LOGGER.debug("---------------------------------------------------------")
 
-        if response.status // 100 in [4, 5]:
-            response.close()
-            if "application/json" in content_type:
-                raise ServiceNotFoundError(response.status, json.loads(contents))
-            raise ServiceNotFoundError(response.status, contents)
-
         if raw_reply and raw_rsp is False:
             return response
 
-        if "application/json" in content_type:
+        if "application/json" in response.headers.get("Content-Type", ""):
             rsp = await response.json()
         elif (
             (headers := kwargs.get("headers"))
             and "application/json" in headers.get("Accept", "")
             and contents == ""
         ):
             _LOGGER.debug("JSON FIX: Accept is JSON but Response is None")
```

### Comparing `audiconnectpy-2.2.6/audiconnectpy/const.py` & `audiconnectpy-2.2.7/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/audiconnectpy/helpers.py` & `audiconnectpy-2.2.7/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/audiconnectpy/model.py` & `audiconnectpy-2.2.7/audiconnectpy/model.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/audiconnectpy/vehicle.py` & `audiconnectpy-2.2.7/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.2.7/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.2.6
+Version: 2.2.7
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.2.6/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.2.7/audiconnectpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/example.py` & `audiconnectpy-2.2.7/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/pyproject.toml` & `audiconnectpy-2.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/tests/conftest.py` & `audiconnectpy-2.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/tests/fixtures/audi0.json` & `audiconnectpy-2.2.7/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/tests/fixtures/audi1.json` & `audiconnectpy-2.2.7/tests/fixtures/audi1.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/tests/fixtures/audi2.json` & `audiconnectpy-2.2.7/tests/fixtures/audi2.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.2.7/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/tests/fixtures/location.json` & `audiconnectpy-2.2.7/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.2.6/tests/test_home.py` & `audiconnectpy-2.2.7/tests/test_home.py`

 * *Files identical despite different names*

