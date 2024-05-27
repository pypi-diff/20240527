# Comparing `tmp/mosqlient-0.1.0.tar.gz` & `tmp/mosqlient-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosqlient-0.1.0.tar", max compression
+gzip compressed data, was "mosqlient-1.0.0.tar", max compression
```

## Comparing `mosqlient-0.1.0.tar` & `mosqlient-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0   329588 2023-12-18 20:19:50.973230 mosqlient-0.1.0/LICENSE
--rw-r--r--   0        0        0      852 2023-12-18 20:19:50.977230 mosqlient-0.1.0/README.md
--rw-r--r--   0        0        0      577 2024-05-23 05:42:25.862474 mosqlient-0.1.0/mosqlient/__init__.py
--rw-r--r--   0        0        0      353 2023-12-18 20:19:50.977230 mosqlient-0.1.0/mosqlient/__main__.py
--rw-r--r--   0        0        0     1222 2024-05-13 17:43:02.282574 mosqlient-0.1.0/mosqlient/cli.py
--rw-r--r--   0        0        0      927 2024-05-23 07:40:43.484448 mosqlient-0.1.0/mosqlient/client.py
--rw-r--r--   0        0        0      207 2024-05-24 21:41:54.346155 mosqlient-0.1.0/mosqlient/config.py
--rw-r--r--   0        0        0        0 2024-05-15 21:41:45.015300 mosqlient-0.1.0/mosqlient/datastore/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 21:42:15.183397 mosqlient-0.1.0/mosqlient/datastore/predictions.py
--rw-r--r--   0        0        0      891 2024-05-23 15:57:17.897420 mosqlient-0.1.0/mosqlient/errors.py
--rw-r--r--   0        0        0      651 2023-12-19 12:54:42.532473 mosqlient-0.1.0/mosqlient/models/__init__.py
--rw-r--r--   0        0        0      133 2023-12-19 11:49:59.878838 mosqlient-0.1.0/mosqlient/models/temporal.py
--rw-r--r--   0        0        0       30 2023-12-19 13:14:44.979055 mosqlient-0.1.0/mosqlient/predictions/__init__.py
--rw-r--r--   0        0        0       26 2024-05-16 16:08:37.991765 mosqlient-0.1.0/mosqlient/registry/__init__.py
--rw-r--r--   0        0        0     5163 2024-05-24 21:59:41.700656 mosqlient-0.1.0/mosqlient/registry/models.py
--rw-r--r--   0        0        0     2645 2024-05-24 21:59:00.184411 mosqlient-0.1.0/mosqlient/requests.py
--rw-r--r--   0        0        0        0 2024-05-08 19:59:43.044664 mosqlient-0.1.0/mosqlient/tests/__init__.py
--rw-r--r--   0        0        0      238 2024-05-08 20:34:42.050299 mosqlient-0.1.0/mosqlient/utils/validate.py
--rw-r--r--   0        0        0     2128 2024-05-24 22:20:56.808459 mosqlient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 mosqlient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0   329588 2024-05-27 12:08:36.682815 mosqlient-1.0.0/LICENSE
+-rw-r--r--   0        0        0      852 2024-05-27 12:08:36.682815 mosqlient-1.0.0/README.md
+-rw-r--r--   0        0        0      577 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/__init__.py
+-rw-r--r--   0        0        0      353 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/__main__.py
+-rw-r--r--   0        0        0     1222 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/cli.py
+-rw-r--r--   0        0        0      927 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/client.py
+-rw-r--r--   0        0        0      204 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/config.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/datastore/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/datastore/predictions.py
+-rw-r--r--   0        0        0      891 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/errors.py
+-rw-r--r--   0        0        0      651 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/models/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/models/temporal.py
+-rw-r--r--   0        0        0       30 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/predictions/__init__.py
+-rw-r--r--   0        0        0       26 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/registry/__init__.py
+-rw-r--r--   0        0        0     5284 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/registry/models.py
+-rw-r--r--   0        0        0     2860 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/requests.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/tests/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-27 12:08:36.682815 mosqlient-1.0.0/mosqlient/utils/validate.py
+-rw-r--r--   0        0        0     2128 2024-05-27 12:09:40.891040 mosqlient-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 mosqlient-1.0.0/PKG-INFO
```

### Comparing `mosqlient-0.1.0/LICENSE` & `mosqlient-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosqlient-0.1.0/README.md` & `mosqlient-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mosqlient-0.1.0/mosqlient/__init__.py` & `mosqlient-1.0.0/mosqlient/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqlient-0.1.0/mosqlient/cli.py` & `mosqlient-1.0.0/mosqlient/cli.py`

 * *Files identical despite different names*

### Comparing `mosqlient-0.1.0/mosqlient/client.py` & `mosqlient-1.0.0/mosqlient/client.py`

 * *Files identical despite different names*

### Comparing `mosqlient-0.1.0/mosqlient/errors.py` & `mosqlient-1.0.0/mosqlient/errors.py`

 * *Files identical despite different names*

### Comparing `mosqlient-0.1.0/mosqlient/models/__init__.py` & `mosqlient-1.0.0/mosqlient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqlient-0.1.0/mosqlient/registry/models.py` & `mosqlient-1.0.0/mosqlient/registry/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import requests
 import nest_asyncio
 from urllib.parse import urlparse
 from typing import Any, Literal, Optional
 
 from mosqlient import Client
-from mosqlient.config import API_BASE_URL
+from mosqlient.config import API_PROD_URL, API_DEV_URL
 from mosqlient.requests import get_all
 from mosqlient.errors import ClientError, ModelPostError
 
 nest_asyncio.apply()
 
 
 def _params(**kwargs) -> dict[str, Any]:
@@ -53,14 +53,15 @@
         implementation_language: str,
         disease: Literal["dengue", "chikungunya", "zika"],
         temporal: bool,
         spatial: bool,
         categorical: bool,
         adm_level: Literal[0, 1, 2, 3],
         time_resolution: Literal["day", "week", "month", "year"],
+        _env: Literal["dev", "prod"] = "prod"
     ):
         if self.client is None:
             raise ClientError(
                 "A Client instance must be provided, please instantiate Model "
                 "passing your Mosqlimate's credentials. For more infor about "
                 "retrieving or inserting data from Mosqlimate, please see the "
                 "API Documentation"
@@ -76,15 +77,16 @@
             "categorical": categorical,
             "ADM_level": adm_level,
             "time_resolution": time_resolution
         }
 
         params = _params(**params)
         self._validate_fields(**params)
-        url = API_BASE_URL + "/".join(("registry", "models")) + "/"
+        base_url = API_DEV_URL if _env == "dev" else API_PROD_URL
+        url = base_url + "/".join(("registry", "models")) + "/"
         headers = {"X-UID-Key": self.client.X_UID_KEY}
         resp = requests.post(url, json=params, headers=headers, timeout=60)
 
         if resp.status_code != 201:
             raise ModelPostError(
                 f"POST request returned status code {resp.status_code}"
             )
```

### Comparing `mosqlient-0.1.0/pyproject.toml` & `mosqlient-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mosqlient"
-version = "0.1.0"  # changed by semantic-release
+version = "1.0.0"  # changed by semantic-release
 description = "client library for the mosqlimate client library"
 authors = ["Flávio Codeço Coelho <fccoelho@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/Mosqlimate-project/mosqlimate-client"
 homepage = "https://github.com/Mosqlimate-project/mosqlimate-client"
 keywords = ["data science", "epidemiology", "forecasting"]
```

### Comparing `mosqlient-0.1.0/PKG-INFO` & `mosqlient-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosqlient
-Version: 0.1.0
+Version: 1.0.0
 Summary: client library for the mosqlimate client library
 Home-page: https://github.com/Mosqlimate-project/mosqlimate-client
 License: GPLv3
 Keywords: data science,epidemiology,forecasting
 Author: Flávio Codeço Coelho
 Author-email: fccoelho@gmail.com
 Requires-Python: >=3.10,<4.0
```

