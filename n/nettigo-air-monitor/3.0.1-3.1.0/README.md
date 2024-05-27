# Comparing `tmp/nettigo_air_monitor-3.0.1.tar.gz` & `tmp/nettigo_air_monitor-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettigo_air_monitor-3.0.1.tar", last modified: Fri May  3 12:06:08 2024, max compression
+gzip compressed data, was "nettigo_air_monitor-3.1.0.tar", last modified: Mon May 27 08:15:03 2024, max compression
```

## Comparing `nettigo_air_monitor-3.0.1.tar` & `nettigo_air_monitor-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.258569 nettigo_air_monitor-3.0.1/nettigo_air_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 12:06:08.000000 nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:06:08.262569 nettigo_air_monitor-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:06:08.258569 nettigo_air_monitor-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-05-03 12:05:59.000000 nettigo_air_monitor-3.0.1/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.494492 nettigo_air_monitor-3.1.0/nettigo_air_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/tests/test_init.py
```

### Comparing `nettigo_air_monitor-3.0.1/LICENSE` & `nettigo_air_monitor-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.1/PKG-INFO` & `nettigo_air_monitor-3.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettigo_air_monitor
-Version: 3.0.1
+Version: 3.1.0
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 Requires-Dist: aqipy-atmotech
 Requires-Dist: dacite>=1.7.0
+Requires-Dist: tenacity
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
 [![Buy me a coffee][buy-me-a-coffee-shield]][buy-me-a-coffee]
 [![PayPal_Me][paypal-me-shield]][paypal-me]
```

### Comparing `nettigo_air_monitor-3.0.1/README.md` & `nettigo_air_monitor-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.1/nettigo_air_monitor/__init__.py` & `nettigo_air_monitor-3.1.0/nettigo_air_monitor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 import re
 from http import HTTPStatus
 from typing import Any
 
 from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 from aqipy import caqi_eu
 from dacite import from_dict
+from tenacity import (
+    after_log,
+    retry,
+    retry_if_exception_type,
+    stop_after_attempt,
+    wait_incrementing,
+)
 
 from .const import (
     ATTR_CONFIG,
     ATTR_DATA,
     ATTR_OTA,
     ATTR_RESTART,
     ATTR_UPTIME,
     ATTR_VALUES,
     DEFAULT_TIMEOUT,
     ENDPOINTS,
     MAC_PATTERN,
     RENAME_KEY_MAP,
-    RESPONSES_FROM_CACHE,
 )
 from .exceptions import (
     ApiError,
     AuthFailedError,
     CannotGetMacError,
     InvalidSensorDataError,
     NotRespondingError,
@@ -38,15 +44,14 @@
 
 class NettigoAirMonitor:
     """Main class to perform Nettigo Air Monitor requests."""
 
     def __init__(self, session: ClientSession, options: ConnectionOptions) -> None:
         """Initialize."""
         self.host = options.host
-        self._last_data: dict[str, Any] = {}
         self._options = options
         self._session = session
         self._software_version: str | None = None
         self._update_errors: int = 0
         self._auth_enabled: bool = False
 
     @classmethod
@@ -117,33 +122,27 @@
 
         _LOGGER.debug("Data retrieved from %s, status: %s", self.host, resp.status)
         if resp.status != HTTPStatus.OK.value:
             raise ApiError(f"Invalid response from device {self.host}: {resp.status}")
 
         return resp
 
+    @retry(
+        retry=retry_if_exception_type(NotRespondingError),
+        stop=stop_after_attempt(5),
+        wait=wait_incrementing(start=5, increment=5),
+        after=after_log(_LOGGER, logging.DEBUG),
+    )
     async def async_update(self) -> NAMSensors:
         """Retrieve data from the device."""
         url = self._construct_url(ATTR_DATA, host=self.host)
 
-        try:
-            resp = await self._async_http_request("get", url)
-        except NotRespondingError as error:
-            if self._update_errors <= RESPONSES_FROM_CACHE and self._last_data:
-                _LOGGER.info(
-                    "Using the cached data because the device %s is not responding",
-                    self.host,
-                )
-                data = self._last_data
-                self._update_errors += 1
-            else:
-                raise ApiError(error.status) from error
-        else:
-            data = self._last_data = await resp.json()
-            self._update_errors = 0
+        resp = await self._async_http_request("get", url)
+
+        data = await resp.json()
 
         self._software_version = data["software_version"]
 
         try:
             sensors = self._parse_sensor_data(data["sensordatavalues"])
         except (TypeError, KeyError) as error:
             raise InvalidSensorDataError("Invalid sensor data") from error
```

### Comparing `nettigo_air_monitor-3.0.1/nettigo_air_monitor/const.py` & `nettigo_air_monitor-3.1.0/nettigo_air_monitor/const.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 ATTR_RESTART: Final[str] = "restart"
 ATTR_SENSOR_VALUES: Final[str] = "sensordatavalues"
 ATTR_UPTIME: Final[str] = "uptime"
 ATTR_VALUES: Final[str] = "values"
 
 DEFAULT_TIMEOUT: Final[ClientTimeout] = ClientTimeout(total=5)
 
-RESPONSES_FROM_CACHE: Final[int] = 3
-
 ENDPOINTS: Final[dict[str, str]] = {
     ATTR_CONFIG: "http://{host}/config.json",
     ATTR_DATA: "http://{host}/data.json",
     ATTR_OTA: "http://{host}/ota",
     ATTR_RESTART: "http://{host}/reset",
     ATTR_VALUES: "http://{host}/values",
 }
```

### Comparing `nettigo_air_monitor-3.0.1/nettigo_air_monitor/exceptions.py` & `nettigo_air_monitor-3.1.0/nettigo_air_monitor/exceptions.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.1/nettigo_air_monitor/model.py` & `nettigo_air_monitor-3.1.0/nettigo_air_monitor/model.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.0.1/nettigo_air_monitor.egg-info/PKG-INFO` & `nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettigo_air_monitor
-Version: 3.0.1
+Version: 3.1.0
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 Requires-Dist: aqipy-atmotech
 Requires-Dist: dacite>=1.7.0
+Requires-Dist: tenacity
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
 [![Buy me a coffee][buy-me-a-coffee-shield]][buy-me-a-coffee]
 [![PayPal_Me][paypal-me-shield]][paypal-me]
```

### Comparing `nettigo_air_monitor-3.0.1/pyproject.toml` & `nettigo_air_monitor-3.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 warn_incomplete_stub = true
 warn_redundant_casts = true
 warn_unused_configs = true
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
-disallow_untyped_decorators = true
+disallow_untyped_decorators = false
 disallow_untyped_defs = true
 no_implicit_optional = true
 strict_equality = true
 warn_return_any = true
 warn_unused_ignores = true
 warn_unreachable = true
```

### Comparing `nettigo_air_monitor-3.0.1/setup.py` & `nettigo_air_monitor-3.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "3.0.1"
+VERSION = "3.1.0"
 
 setup(
     name="nettigo_air_monitor",
     version=VERSION,
     author="Maciej Bieniek",
     description=(
         "Python wrapper for getting air quality data from Nettigo Air Monitor devices."
@@ -19,15 +19,15 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/bieniu/nettigo-air-monitor",
     license="Apache-2.0 License",
     packages=["nettigo_air_monitor"],
     package_data={"nettigo_air_monitor": ["py.typed"]},
     python_requires=">=3.11",
-    install_requires=["aiohttp>=3.7.0", "aqipy-atmotech", "dacite>=1.7.0"],
+    install_requires=["aiohttp>=3.7.0", "aqipy-atmotech", "dacite>=1.7.0", "tenacity"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
```

### Comparing `nettigo_air_monitor-3.0.1/tests/test_init.py` & `nettigo_air_monitor-3.1.0/tests/test_init.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Tests for nettigo package."""
 
 import json
 from http import HTTPStatus
 from typing import Any
 from unittest.mock import Mock, patch
 
-import aiohttp
 import pytest
-from aiohttp import ClientResponseError
+from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 from aioresponses import aioresponses
 from syrupy import SnapshotAssertion
+from tenacity import RetryError
 
 from nettigo_air_monitor import (
     ApiError,
     AuthFailedError,
     CannotGetMacError,
     ConnectionOptions,
     InvalidSensorDataError,
@@ -21,36 +21,31 @@
 )
 
 VALID_IP = "192.168.172.12"
 INVALID_HOST = "http://nam.org"
 
 VALUES = "MAC: AA:BB:CC:DD:EE:FF<br/>"
 
+DATA_JSON_URL = "http://192.168.172.12/data.json"
+CONFIG_JSON_URL = "http://192.168.172.12/config.json"
+VALUES_URL = "http://192.168.172.12/values"
+
 
 @pytest.mark.asyncio()
 async def test_valid_data(
     snapshot: SnapshotAssertion, valid_data: dict[str, Any]
 ) -> None:
     """Test with valid data."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            payload=valid_data,
-        )
-        session_mock.get(
-            "http://192.168.172.12/values",
-            payload=VALUES,
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
+        session_mock.get(DATA_JSON_URL, payload=valid_data)
+        session_mock.get(VALUES_URL, payload=VALUES)
 
         nam = await NettigoAirMonitor.create(session, options)
         mac = await nam.async_get_mac_address()
         sensors = await nam.async_update()
 
     await session.close()
 
@@ -61,60 +56,42 @@
 
 
 @pytest.mark.asyncio()
 async def test_caqi_value(snapshot: SnapshotAssertion) -> None:
     """Test CAQI value when PM10 and PM2.5 is None."""
     data = {"software_version": "NAMF-2020-36", "sensordatavalues": []}
 
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            payload=data,
-        )
-        session_mock.get(
-            "http://192.168.172.12/values",
-            payload=VALUES,
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
+        session_mock.get(DATA_JSON_URL, payload=data)
+        session_mock.get(VALUES_URL, payload=VALUES)
 
         nam = await NettigoAirMonitor.create(session, options)
         sensors = await nam.async_update()
 
     await session.close()
 
     assert sensors == snapshot
 
 
 @pytest.mark.asyncio()
 async def test_valid_data_with_auth(
     snapshot: SnapshotAssertion, valid_data: dict[str, Any]
 ) -> None:
     """Test with valid data with authorization."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": True},
-        )
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            payload=valid_data,
-        )
-        session_mock.get(
-            "http://192.168.172.12/values",
-            payload=VALUES,
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": True})
+        session_mock.get(DATA_JSON_URL, payload=valid_data)
+        session_mock.get(VALUES_URL, payload=VALUES)
 
         nam = await NettigoAirMonitor.create(session, options)
         mac = await nam.async_get_mac_address()
         sensors = await nam.async_update()
 
     await session.close()
 
@@ -124,22 +101,19 @@
     assert nam.auth_enabled is True
     assert sensors == snapshot
 
 
 @pytest.mark.asyncio()
 async def test_auth_failed() -> None:
     """Test auth failed."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
         session_mock.post(
             "http://192.168.172.12/reset",
             exception=ClientResponseError(
@@ -154,20 +128,20 @@
 
     await session.close()
 
 
 @pytest.mark.asyncio()
 async def test_auth_enabled() -> None:
     """Test auth failed."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
         session_mock.get(
-            "http://192.168.172.12/config.json",
+            CONFIG_JSON_URL,
             exception=ClientResponseError(
                 Mock(), Mock(), status=HTTPStatus.UNAUTHORIZED.value
             ),
         )
 
         nam = await NettigoAirMonitor.create(session, options)
 
@@ -175,20 +149,20 @@
 
     assert nam.auth_enabled is True
 
 
 @pytest.mark.asyncio()
 async def test_http_404_code() -> None:
     """Test request ends with error."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
         session_mock.get(
-            "http://192.168.172.12/config.json",
+            CONFIG_JSON_URL,
             exception=ClientResponseError(
                 Mock(), Mock(), status=HTTPStatus.NOT_FOUND.value
             ),
         )
         with pytest.raises(ApiError) as excinfo:
             await NettigoAirMonitor.create(session, options)
 
@@ -196,196 +170,109 @@
 
     await session.close()
 
 
 @pytest.mark.asyncio()
 async def test_api_error() -> None:
     """Test API error."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            status=HTTPStatus.ACCEPTED.value,
-        )
+        session_mock.get(DATA_JSON_URL, status=HTTPStatus.ACCEPTED.value)
         with pytest.raises(ApiError) as excinfo:
             await nam.async_update()
 
     assert str(excinfo.value) == "Invalid response from device 192.168.172.12: 202"
 
     await session.close()
 
 
 @pytest.mark.asyncio()
-async def test_cache_empty() -> None:
-    """Test error request when cache is empty."""
-    session = aiohttp.ClientSession()
-    options = ConnectionOptions(VALID_IP)
-
-    with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
-
-        nam = await NettigoAirMonitor.create(session, options)
-
-    with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            exception=TimeoutError(Mock(), Mock()),
-        )
-
-        with pytest.raises(ApiError) as excinfo:
-            await nam.async_update()
-
-    assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
-
-    await session.close()
-
-
-@pytest.mark.asyncio()
-async def test_data_cached(
-    snapshot: SnapshotAssertion, valid_data: dict[str, Any]
-) -> None:
-    """Test error request when the data is cached."""
-    session = aiohttp.ClientSession()
-    options = ConnectionOptions(VALID_IP)
-
-    with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            payload=valid_data,
-        )
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            exception=TimeoutError(Mock(), Mock()),
-        )
-
-        nam = await NettigoAirMonitor.create(session, options)
-        await nam.async_update()
-        sensors = await nam.async_update()
-
-    await session.close()
-
-    assert nam.software_version == "NAMF-2020-36"
-    assert sensors == snapshot
-
-
-@pytest.mark.asyncio()
 async def test_invalid_sensor_data() -> None:
     """Test InvalidSensorDataError."""
     with open("tests/fixtures/invalid_data.json", encoding="utf-8") as file:
         data = json.load(file)
 
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/data.json",
-            payload=data,
-        )
+        session_mock.get(DATA_JSON_URL, payload=data)
 
         with pytest.raises(InvalidSensorDataError) as excinfo:
             await nam.async_update()
 
     assert str(excinfo.value) == "Invalid sensor data"
 
     await session.close()
 
 
 @pytest.mark.asyncio()
 async def test_cannot_get_mac() -> None:
     """Test CannotGetMacError error."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/values",
-            payload="lorem ipsum",
-        )
+        session_mock.get(VALUES_URL, payload="lorem ipsum")
 
         with pytest.raises(CannotGetMacError) as excinfo:
             await nam.async_get_mac_address()
 
     assert str(excinfo.value) == "Cannot get MAC address from device"
 
     await session.close()
 
 
 @pytest.mark.asyncio()
 async def test_init_device_not_repond() -> None:
     """Test init when device is not responding."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            exception=TimeoutError(Mock(), Mock()),
-        )
+        session_mock.get(CONFIG_JSON_URL, exception=TimeoutError(Mock(), Mock()))
 
         with pytest.raises(ApiError) as excinfo:
             await NettigoAirMonitor.create(session, options)
 
     assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
 
     await session.close()
 
 
 @pytest.mark.asyncio()
 async def test_get_ma_device_not_repond() -> None:
     """Test get_mac when device is not responding."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/values",
-            exception=TimeoutError(Mock(), Mock()),
-        )
+        session_mock.get(VALUES_URL, exception=TimeoutError(Mock(), Mock()))
 
         with pytest.raises(ApiError) as excinfo:
             await nam.async_get_mac_address()
 
     await session.close()
 
     assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
@@ -404,22 +291,19 @@
 
 @pytest.mark.asyncio()
 @pytest.mark.parametrize(
     ("method", "endpoint"), [("async_restart", "reset"), ("async_ota_update", "ota")]
 )
 async def test_post_methods(method: str, endpoint: str) -> None:
     """Test post methods."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": False},
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with (
         aioresponses() as session_mock,
         patch(
             "nettigo_air_monitor.NettigoAirMonitor._async_http_request"
@@ -439,31 +323,88 @@
 
 @pytest.mark.asyncio()
 @pytest.mark.parametrize(
     ("method", "endpoint"), [("async_restart", "reset"), ("async_ota_update", "ota")]
 )
 async def test_post_methods_fail(method: str, endpoint: str) -> None:
     """Test fail of the post methods."""
-    session = aiohttp.ClientSession()
+    session = ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
-        session_mock.get(
-            "http://192.168.172.12/config.json",
-            payload={"www_basicauth_enabled": True},
-        )
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": True})
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
         session_mock.post(
-            f"http://192.168.172.12/{endpoint}",
-            exception=TimeoutError(Mock(), Mock()),
+            f"http://192.168.172.12/{endpoint}", exception=TimeoutError(Mock(), Mock())
         )
 
         method_to_call = getattr(nam, method)
         with pytest.raises(ApiError) as excinfo:
             await method_to_call()
 
     assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
 
     await session.close()
+
+
+@pytest.mark.parametrize(
+    "exc", [TimeoutError(Mock(), Mock()), ClientConnectorError(Mock(), Mock())]
+)
+@pytest.mark.asyncio()
+async def test_retry_success(valid_data: dict[str, Any], exc: Exception) -> None:
+    """Test retry which succeeded."""
+    session = ClientSession()
+    options = ConnectionOptions(VALID_IP)
+
+    with aioresponses() as session_mock, patch("asyncio.sleep") as sleep_mock:
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, payload=valid_data)
+
+        nam = await NettigoAirMonitor.create(session, options)
+        await nam.async_update()
+
+    assert sleep_mock.call_count == 4
+    assert sleep_mock.call_args_list[0][0][0] == 5
+    assert sleep_mock.call_args_list[1][0][0] == 10
+    assert sleep_mock.call_args_list[2][0][0] == 15
+    assert sleep_mock.call_args_list[3][0][0] == 20
+
+    await session.close()
+
+
+@pytest.mark.parametrize(
+    "exc", [TimeoutError(Mock(), Mock()), ClientConnectorError(Mock(), Mock())]
+)
+@pytest.mark.asyncio()
+async def test_retry_fail(exc: Exception) -> None:
+    """Test retry that failed."""
+    session = ClientSession()
+    options = ConnectionOptions(VALID_IP)
+
+    with aioresponses() as session_mock, patch("asyncio.sleep") as sleep_mock:
+        session_mock.get(CONFIG_JSON_URL, payload={"www_basicauth_enabled": False})
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, exception=exc)
+        session_mock.get(DATA_JSON_URL, exception=exc)
+
+        nam = await NettigoAirMonitor.create(session, options)
+        with pytest.raises(RetryError) as excinfo:
+            await nam.async_update()
+
+    await session.close()
+
+    assert sleep_mock.call_count == 4
+    assert sleep_mock.call_args_list[0][0][0] == 5
+    assert sleep_mock.call_args_list[1][0][0] == 10
+    assert sleep_mock.call_args_list[2][0][0] == 15
+    assert sleep_mock.call_args_list[3][0][0] == 20
+
+    assert "RetryError" in str(excinfo.value)
```

