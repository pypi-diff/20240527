# Comparing `tmp/heatzypy-2.5.4.tar.gz` & `tmp/heatzypy-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatzypy-2.5.4.tar", last modified: Thu May  2 10:57:58 2024, max compression
+gzip compressed data, was "heatzypy-2.5.5.tar", last modified: Mon May 27 16:17:55 2024, max compression
```

## Comparing `heatzypy-2.5.4.tar` & `heatzypy-2.5.5.tar`

### file list

```diff
@@ -1,35 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:57:58.632671 heatzypy-2.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:57:58.628671 heatzypy-2.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:57:58.628671 heatzypy-2.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:57:58.628671 heatzypy-2.5.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 10:57:48.000000 heatzypy-2.5.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 10:57:48.000000 heatzypy-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 10:57:48.000000 heatzypy-2.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-02 10:57:58.632671 heatzypy-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-02 10:57:48.000000 heatzypy-2.5.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2302 2024-05-02 10:57:48.000000 heatzypy-2.5.4/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:57:58.628671 heatzypy-2.5.4/heatzypy/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-02 10:57:48.000000 heatzypy-2.5.4/heatzypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-02 10:57:48.000000 heatzypy-2.5.4/heatzypy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-02 10:57:48.000000 heatzypy-2.5.4/heatzypy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-02 10:57:48.000000 heatzypy-2.5.4/heatzypy/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-02 10:57:48.000000 heatzypy-2.5.4/heatzypy/heatzy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-05-02 10:57:48.000000 heatzypy-2.5.4/heatzypy/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:57:58.632671 heatzypy-2.5.4/heatzypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-02 10:57:58.000000 heatzypy-2.5.4/heatzypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-02 10:57:58.000000 heatzypy-2.5.4/heatzypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:57:58.000000 heatzypy-2.5.4/heatzypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:57:58.000000 heatzypy-2.5.4/heatzypy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 10:57:58.000000 heatzypy-2.5.4/heatzypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 10:57:58.000000 heatzypy-2.5.4/heatzypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-02 10:57:48.000000 heatzypy-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-02 10:57:48.000000 heatzypy-2.5.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 10:57:48.000000 heatzypy-2.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:57:58.632671 heatzypy-2.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.913467 heatzypy-2.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.909467 heatzypy-2.5.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.909467 heatzypy-2.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.909467 heatzypy-2.5.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 16:17:47.000000 heatzypy-2.5.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:17:47.000000 heatzypy-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 16:17:47.000000 heatzypy-2.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-27 16:17:55.913467 heatzypy-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-27 16:17:47.000000 heatzypy-2.5.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2277 2024-05-27 16:17:47.000000 heatzypy-2.5.5/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.913467 heatzypy-2.5.5/heatzypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-27 16:17:47.000000 heatzypy-2.5.5/heatzypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-27 16:17:47.000000 heatzypy-2.5.5/heatzypy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 16:17:47.000000 heatzypy-2.5.5/heatzypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-27 16:17:47.000000 heatzypy-2.5.5/heatzypy/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-27 16:17:47.000000 heatzypy-2.5.5/heatzypy/heatzy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-27 16:17:47.000000 heatzypy-2.5.5/heatzypy/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.913467 heatzypy-2.5.5/heatzypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-27 16:17:55.000000 heatzypy-2.5.5/heatzypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-27 16:17:55.000000 heatzypy-2.5.5/heatzypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:17:55.000000 heatzypy-2.5.5/heatzypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:17:55.000000 heatzypy-2.5.5/heatzypy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 16:17:55.000000 heatzypy-2.5.5/heatzypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 16:17:55.000000 heatzypy-2.5.5/heatzypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-27 16:17:47.000000 heatzypy-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-27 16:17:47.000000 heatzypy-2.5.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 16:17:47.000000 heatzypy-2.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:17:55.913467 heatzypy-2.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.913467 heatzypy-2.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:55.913467 heatzypy-2.5.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    15958 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/fixtures/attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/fixtures/device.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/fixtures/devices.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22458 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/fixtures/devices_rest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/test_climate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-27 16:17:47.000000 heatzypy-2.5.5/tests/test_connection.py
```

### Comparing `heatzypy-2.5.4/.github/dependabot.yml` & `heatzypy-2.5.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/.github/workflows/auto-approve.yml` & `heatzypy-2.5.5/.github/workflows/auto-approve.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 name: Dependency auto-merge
 on: pull_request
 
 permissions:
   pull-requests: write
+  contents: write
 
 jobs:
   dependency:
     runs-on: ubuntu-latest
     if: ${{ github.actor == 'dependabot[bot]' || github.actor == 'pre-commit-ci[bot]' }}
     steps:
       - name: Approve a PR
```

### Comparing `heatzypy-2.5.4/.github/workflows/lint.yml` & `heatzypy-2.5.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/.github/workflows/pythonpublish.yml` & `heatzypy-2.5.5/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/.github/workflows/release.yml` & `heatzypy-2.5.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/.gitignore` & `heatzypy-2.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/.pre-commit-config.yaml` & `heatzypy-2.5.5/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.2
+    rev: v0.4.4
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
```

### Comparing `heatzypy-2.5.4/LICENSE` & `heatzypy-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/PKG-INFO` & `heatzypy-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.4
+Version: 2.5.5
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.4/README.md` & `heatzypy-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/example.py` & `heatzypy-2.5.5/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
 """
 This example can be run safely as it won't change anything.
 
 There are two modes to control Heatzy modules:
     - Classic mode by calling the Rest API
     - Websocket mode by calling the websocket module
 """
```

### Comparing `heatzypy-2.5.4/heatzypy/auth.py` & `heatzypy-2.5.5/heatzypy/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import asyncio
 from json import JSONDecodeError
 import logging
 import socket
-import time
+from time import time
 from typing import Any
 
 from aiohttp import ClientError, ClientResponseError, ClientSession
 from yarl import URL
 
 from .const import APPLICATION_ID, RETRY, URL_PATH
 from .exception import (
@@ -37,58 +37,53 @@
         host: str,
         use_tls: bool = True,
     ):
         """Initialize the auth."""
         self._session = session or ClientSession()
         self._username = username
         self._password = password
-        self._access_token: dict[str, Any] | None = None
+        self._access_token: str | None = None
+        self._expire_at: float = time()
         self._timeout: int = timeout
         self._retry = RETRY
         self._host = host
         self._scheme = "https" if use_tls else "http"
 
-    async def request(
-        self,
-        url: str,
-        method: str = "get",
-        json: dict[str, Any] | None = None,
-        auth: bool = False,
-    ) -> dict[str, Any]:
+    async def async_request(self, path: str, method: str = "get", **kwargs: Any) -> Any:
         """Make a request."""
-        headers: dict[str, Any] = {"X-Gizwits-Application-Id": APPLICATION_ID}
+        kwargs.setdefault("headers", {})
+        kwargs["headers"].update({"X-Gizwits-Application-Id": APPLICATION_ID})
 
-        if auth is False:
-            access_token = await self.async_get_token()
-            headers["X-Gizwits-User-Token"] = access_token.get("token")
+        if path != "login":
+            await self.async_get_token()
+            kwargs["headers"].update({"X-Gizwits-User-Token": self._access_token})
 
         try:
             async with asyncio.timeout(self._timeout):
-                uri = URL.build(
-                    scheme=self._scheme, host=self._host, path=f"{URL_PATH}/{url}"
-                )
-                logger.debug("METHOD:%s URL:%s", method, uri)
-                logger.debug("DATA:%s", json)
-                response = await self._session.request(
-                    method, uri, json=json, headers=headers
+                url = URL.build(
+                    scheme=self._scheme, host=self._host, path=f"{URL_PATH}/{path}"
                 )
+                logger.debug("Request: %s (%s) - %s", path, method, kwargs.get("json"))
+                response = await self._session.request(method, url, **kwargs)
                 response.raise_for_status()
         except ClientResponseError as error:
             if method == "get":
-                raise RetrieveFailed(f"{url} not retrieved ({error.status})") from error
-            if url == "login":
+                raise RetrieveFailed(
+                    f"{path} not retrieved ({error.status})"
+                ) from error
+            if path == "login":
                 raise AuthenticationFailed(
                     f"{error.message} ({error.status})"
                 ) from error
             if method == "post" and error.status in [400, 500, 502] and self._retry > 0:
                 self._retry -= 1
                 await asyncio.sleep(3)
-                return await self.request(url, method, json, auth)
+                return await self.async_request(path, method, **kwargs)
             raise CommandFailed(
-                f"Cmd failed {url} with {json} ({error.status} {error.message})"
+                f"Cmd failed {path} with {kwargs.get('json')} ({error.status} {error.message})"
             ) from error
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Heatzy."
             ) from error
         except (ClientError, socket.gaierror) as error:
             raise HttpRequestFailed(
@@ -102,18 +97,16 @@
         except JSONDecodeError as error:
             raise UnexpectedResponse(f"Error while decoding Json ({error})") from error
 
         logger.debug("RESPONSE: %s", json_response)
 
         return json_response
 
-    async def async_get_token(self) -> dict[str, Any]:
+    async def async_get_token(self, force: bool = False) -> Any:
         """Get Token authentication."""
-        if self._access_token is None or (
-            (expire_at := self._access_token.get("expire_at"))
-            and expire_at < time.time()
-        ):
+        if force or self._expire_at < time():
             payload = {"username": self._username, "password": self._password}
-            self._access_token = await self.request(
-                "login", method="post", json=payload, auth=True
-            )
-        return self._access_token
+            token = await self.async_request("login", "post", json=payload)
+            self._expire_at = token.get("expire_at")
+            self._access_token = token.get("token")
+
+            return token
```

### Comparing `heatzypy-2.5.4/heatzypy/exception.py` & `heatzypy-2.5.5/heatzypy/exception.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.4/heatzypy/heatzy.py` & `heatzypy-2.5.5/heatzypy/heatzy.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,55 +30,54 @@
         if region == "EU":
             host = EU_API_URL
         elif region == "US":
             host = US_API_URL
         else:
             host = DFLT_API_URL
 
-        self._auth = Auth(session, username, password, time_out, host, use_tls)
-        self.websocket = Websocket(session, self._auth, WS_HOST, use_tls)
-        self.session = session
-        self.request = self._auth.request
+        self.auth = Auth(session, username, password, time_out, host, use_tls)
+        self.websocket = Websocket(session, self.auth, WS_HOST, use_tls)
+        self.async_request = self.auth.async_request
 
-    async def async_bindings(self) -> dict[str, list[dict[str, Any]]]:
+    async def async_bindings(self) -> Any:
         """Fetch all configured devices."""
-        return await self.request("bindings")
+        return await self.async_request("bindings")
 
     async def async_get_devices(self) -> dict[str, Any]:
         """Fetch all configured devices."""
         response = await self.async_bindings()
         devices = {device["did"]: device for device in response.get("devices", {})}
         for did, device in devices.items():
             device_data = await self.async_get_device_data(did)
             device_data["attrs"] = device_data.pop("attr", {})
             device.update(**device_data)
         return devices
 
     async def async_get_device(self, device_id: str) -> dict[str, Any]:
         """Fetch device with given id."""
-        device = await self.request(f"devices/{device_id}")
+        device = await self.async_request(f"devices/{device_id}")
         device_data = await self.async_get_device_data(device_id)
         device_data["attrs"] = device_data.pop("attr", {})
         return {**device, **device_data}
 
-    async def async_get_device_data(self, device_id: str) -> dict[str, Any]:
+    async def async_get_device_data(self, device_id: str) -> Any:
         """Fetch detailed data for device with given id."""
-        return await self.request(f"devdata/{device_id}/latest")
+        return await self.async_request(f"devdata/{device_id}/latest")
 
     async def async_control_device(
         self, device_id: str, payload: dict[str, Any]
     ) -> None:
         """Control state of device with given id."""
-        await self.request(f"control/{device_id}", method="post", json=payload)
+        await self.async_request(f"control/{device_id}", "post", json=payload)
 
     async def async_close(self) -> None:
         """Close open client (WebSocket) session."""
         await self.websocket.async_disconnect()
-        if self.session:
-            await self.session.close()
+        if self.auth._session:
+            await self.auth._session.close()
 
     async def __aenter__(self) -> Self:
         """Async enter."""
         return self
 
     async def __aexit__(self, *_exc_info: object) -> None:
         """Async exit."""
```

### Comparing `heatzypy-2.5.4/heatzypy/websocket.py` & `heatzypy-2.5.5/heatzypy/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Class for websocket."""
 
 from __future__ import annotations
 
 import asyncio
+from collections.abc import Callable
 import json
 import logging
 import socket
-from typing import TYPE_CHECKING, Any, Callable, cast
+from typing import TYPE_CHECKING, Any, cast
 
 import aiohttp
 from aiohttp import ClientSession, ClientWebSocketResponse
 from yarl import URL as yurl
 
 from .const import APPLICATION_ID, WS_PING_INTERVAL, WS_PORT, WSS_PORT
 from .exception import AuthenticationFailed, ConnectionFailed, WebsocketError
@@ -57,15 +58,15 @@
         attrs_fills = [
             device["did"] for device in self.devices.values() if device.get("attrs")
         ]
         return list(self.devices.keys()) == attrs_fills and len(self.devices) > 0
 
     async def async_fetch_binding_devices(self) -> None:
         """Return bindings devices."""
-        bindings = await self._auth.request("bindings")
+        bindings = await self._auth.async_request("bindings")
         for info in bindings.get("devices", {}):
             self.devices.update({info["did"]: info})
 
     async def async_get_devices(self) -> dict[str, Any]:
         """Return all devices data while listen connection."""
         for did in self.devices:
             payload = {"cmd": "c2s_read", "data": {"did": did}}
@@ -145,15 +146,15 @@
                 await self.async_get_devices()
             except WebsocketError as error:
                 raise AuthenticationFailed(error) from error
 
     async def async_login(self, auto_subscribe: bool = True) -> None:
         """Login to websocket."""
 
-        token_data = await self._auth.async_get_token()
+        token_data = await self._auth.async_get_token(force=True)
 
         payload = {
             "cmd": "login_req",
             "data": {
                 "appid": APPLICATION_ID,
                 "uid": token_data.get("uid"),
                 "token": token_data.get("token"),
@@ -230,15 +231,14 @@
         """
         dids = [{"did": did} for did in device_ids]
         payload = {"cmd": "subscribe_req", "data": dids}
         await self._send_cmd(payload)
 
     async def _hand_pong(self, data: dict[str, Any]) -> None:
         """Handle ping receive."""
-        pass
 
     async def _handle_login(self, data: dict[str, Any]) -> None:
         """Handle login response."""
         if data.get("success") is False:
             self.is_logged = False
             raise AuthenticationFailed(data)
         logger.debug("WEBSOCKET Successfully authenticated")
@@ -270,22 +270,23 @@
         self.last_invalid_msg = data
 
     async def _handle_binding_change(self, data: dict[str, Any]) -> None:
         """Handle a new binding status."""
         if (did := data.get("did")) and (data.get("bind") is False):
             self.devices.pop(did, None)
         elif did:
-            bindings = await self._auth.request("bindings")
+            bindings = await self._auth.async_request("bindings")
             if bindings and (data := bindings.get(did, {})):
                 self.devices.update({did: data})
 
     async def _handle_status_change(self, data: dict[str, Any]) -> None:
         """Handle a new status."""
-        if device := self.devices.get(data.get("did", "")):
-            await device.async_update(data)
+        did = data.pop("did", None)
+        if device := self.devices.get(did):
+            device.update(data)
 
     async def _send_cmd(self, payload: dict[str, Any]) -> None:
         """Send command to websocket."""
         if not self.ws or not self.is_connected:
             raise WebsocketError("Not connected to a Heatzy WebSocket")
 
         logger.debug("WEBSOCKET >>> %s", payload)
```

### Comparing `heatzypy-2.5.4/heatzypy.egg-info/PKG-INFO` & `heatzypy-2.5.5/heatzypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.4
+Version: 2.5.5
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.4/pyproject.toml` & `heatzypy-2.5.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -31,18 +31,21 @@
 [tool.setuptools_scm]
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe  = false
 include-package-data = true
 
-[tool.ruff.flake8-pytest-style]
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.flake8-tidy-imports.banned-api]
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
 "async_timeout".msg = "use asyncio.timeout instead"
 "pytz".msg = "use zoneinfo instead"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-sort-within-sections = true
 combine-as-imports = true
 split-on-trailing-comma = false
```

