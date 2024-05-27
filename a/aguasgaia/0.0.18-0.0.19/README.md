# Comparing `tmp/aguasgaia-0.0.18.tar.gz` & `tmp/aguasgaia-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aguasgaia-0.0.18.tar", last modified: Wed May 22 22:32:39 2024, max compression
+gzip compressed data, was "aguasgaia-0.0.19.tar", last modified: Mon May 27 11:30:58 2024, max compression
```

## Comparing `aguasgaia-0.0.18.tar` & `aguasgaia-0.0.19.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:39.003616 aguasgaia-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-22 22:32:39.003616 aguasgaia-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:38.999616 aguasgaia-0.0.18/aguasgaia/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/aguasgaia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/aguasgaia/aguasgaia.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/aguasgaia/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:38.999616 aguasgaia-0.0.18/aguasgaia/models/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/aguasgaia/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/aguasgaia/models/consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/aguasgaia/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/aguasgaia/models/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:39.003616 aguasgaia-0.0.18/aguasgaia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-22 22:32:38.000000 aguasgaia-0.0.18/aguasgaia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 22:32:38.000000 aguasgaia-0.0.18/aguasgaia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:32:38.000000 aguasgaia-0.0.18/aguasgaia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 22:32:38.000000 aguasgaia-0.0.18/aguasgaia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 22:32:38.000000 aguasgaia-0.0.18/aguasgaia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:32:39.003616 aguasgaia-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:38.999616 aguasgaia-0.0.18/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:38.999616 aguasgaia-0.0.18/src/aguasgaia/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/src/aguasgaia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:38.999616 aguasgaia-0.0.18/src/aguasgaia/models/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/src/aguasgaia/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/src/aguasgaia/models/consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/src/aguasgaia/models/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:38.999616 aguasgaia-0.0.18/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-22 22:32:34.000000 aguasgaia-0.0.18/tests/aguasgaia_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.032909 aguasgaia-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-27 11:30:58.032909 aguasgaia-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.028909 aguasgaia-0.0.19/aguasgaia/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/aguasgaia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/aguasgaia/aguasgaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/aguasgaia/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.028909 aguasgaia-0.0.19/aguasgaia/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/aguasgaia/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/aguasgaia/models/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/aguasgaia/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/aguasgaia/models/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.032909 aguasgaia-0.0.19/aguasgaia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-27 11:30:58.000000 aguasgaia-0.0.19/aguasgaia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-27 11:30:58.000000 aguasgaia-0.0.19/aguasgaia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:30:58.000000 aguasgaia-0.0.19/aguasgaia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 11:30:58.000000 aguasgaia-0.0.19/aguasgaia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 11:30:58.000000 aguasgaia-0.0.19/aguasgaia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:30:58.032909 aguasgaia-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.028909 aguasgaia-0.0.19/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.028909 aguasgaia-0.0.19/src/aguasgaia/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/src/aguasgaia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.032909 aguasgaia-0.0.19/src/aguasgaia/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/src/aguasgaia/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/src/aguasgaia/models/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/src/aguasgaia/models/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:58.032909 aguasgaia-0.0.19/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-27 11:30:53.000000 aguasgaia-0.0.19/tests/aguasgaia_test.py
```

### Comparing `aguasgaia-0.0.18/LICENSE` & `aguasgaia-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/PKG-INFO` & `aguasgaia-0.0.19/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: aguasgaia
-Version: 0.0.18
+Version: 0.0.19
 Summary: Python library to retrieve information from "Aguas de Gaia" portal
 Author-email: Jose Rolo <ze.p.rolo@gmail.com>
 License: Apache-2.0
 Keywords: api,aguasgaia
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: python-dateutil
 
 # Aguas de Gaia API
 
 ## Installation
-
-    pip install .
-
+```bash
+$ pip install aguasgaia
+```
 ## Usage
 ```python
 import asyncio
 import aiohttp
 from aguasgaia import AguasGaia
 
 
 async def main():
     session = aiohttp.ClientSession()
 
-    aguas = AguasGaia(session, "<USERNAME>", "<PASSWORD>", subscription_id="<SUBSCRIPTION_ID>")
+    aguas = AguasGaia(session, "<USERNAME>", "<PASSWORD>")
     print("LOGIN: ", await aguas.login())
 
     print("SUBSCRIPTIONS:\n{0}".format(await aguas.get_subscriptions()))
 
     inv = await aguas.get_last_invoice()
     print("INVOICE: {0}\n{1}".format(inv.invoice_value, inv.invoice_attributes))
 
@@ -43,9 +43,15 @@
 
 if __name__ == "__main__":
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
     asyncio.run(main())
 ```
 
 ## Tests
-
-    TBD
+Make sure pytest asyncio is installed
+```bash
+$ pip install pytest-asyncio
+```
+Execute the tests
+```bash
+$ pytest tests/
+```
```

### Comparing `aguasgaia-0.0.18/README.md` & `aguasgaia-0.0.19/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Aguas de Gaia API
 
 ## Installation
-
-    pip install .
-
+```bash
+$ pip install aguasgaia
+```
 ## Usage
 ```python
 import asyncio
 import aiohttp
 from aguasgaia import AguasGaia
 
 
 async def main():
     session = aiohttp.ClientSession()
 
-    aguas = AguasGaia(session, "<USERNAME>", "<PASSWORD>", subscription_id="<SUBSCRIPTION_ID>")
+    aguas = AguasGaia(session, "<USERNAME>", "<PASSWORD>")
     print("LOGIN: ", await aguas.login())
 
     print("SUBSCRIPTIONS:\n{0}".format(await aguas.get_subscriptions()))
 
     inv = await aguas.get_last_invoice()
     print("INVOICE: {0}\n{1}".format(inv.invoice_value, inv.invoice_attributes))
 
@@ -29,9 +29,15 @@
 
 if __name__ == "__main__":
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
     asyncio.run(main())
 ```
 
 ## Tests
-
-    TBD
+Make sure pytest asyncio is installed
+```bash
+$ pip install pytest-asyncio
+```
+Execute the tests
+```bash
+$ pytest tests/
+```
```

### Comparing `aguasgaia-0.0.18/aguasgaia/aguasgaia.py` & `aguasgaia-0.0.19/aguasgaia/aguasgaia.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/aguasgaia/const.py` & `aguasgaia-0.0.19/aguasgaia/const.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/aguasgaia/models/consumption.py` & `aguasgaia-0.0.19/aguasgaia/models/consumption.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/aguasgaia/models/invoice.py` & `aguasgaia-0.0.19/aguasgaia/models/invoice.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/aguasgaia/models/subscription.py` & `aguasgaia-0.0.19/aguasgaia/models/subscription.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/aguasgaia.egg-info/PKG-INFO` & `aguasgaia-0.0.19/aguasgaia.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: aguasgaia
-Version: 0.0.18
+Version: 0.0.19
 Summary: Python library to retrieve information from "Aguas de Gaia" portal
 Author-email: Jose Rolo <ze.p.rolo@gmail.com>
 License: Apache-2.0
 Keywords: api,aguasgaia
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: python-dateutil
 
 # Aguas de Gaia API
 
 ## Installation
-
-    pip install .
-
+```bash
+$ pip install aguasgaia
+```
 ## Usage
 ```python
 import asyncio
 import aiohttp
 from aguasgaia import AguasGaia
 
 
 async def main():
     session = aiohttp.ClientSession()
 
-    aguas = AguasGaia(session, "<USERNAME>", "<PASSWORD>", subscription_id="<SUBSCRIPTION_ID>")
+    aguas = AguasGaia(session, "<USERNAME>", "<PASSWORD>")
     print("LOGIN: ", await aguas.login())
 
     print("SUBSCRIPTIONS:\n{0}".format(await aguas.get_subscriptions()))
 
     inv = await aguas.get_last_invoice()
     print("INVOICE: {0}\n{1}".format(inv.invoice_value, inv.invoice_attributes))
 
@@ -43,9 +43,15 @@
 
 if __name__ == "__main__":
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
     asyncio.run(main())
 ```
 
 ## Tests
-
-    TBD
+Make sure pytest asyncio is installed
+```bash
+$ pip install pytest-asyncio
+```
+Execute the tests
+```bash
+$ pytest tests/
+```
```

### Comparing `aguasgaia-0.0.18/aguasgaia.egg-info/SOURCES.txt` & `aguasgaia-0.0.19/aguasgaia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/src/aguasgaia/models/consumption.py` & `aguasgaia-0.0.19/src/aguasgaia/models/consumption.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/src/aguasgaia/models/invoice.py` & `aguasgaia-0.0.19/src/aguasgaia/models/invoice.py`

 * *Files identical despite different names*

### Comparing `aguasgaia-0.0.18/tests/aguasgaia_test.py` & `aguasgaia-0.0.19/tests/aguasgaia_test.py`

 * *Files identical despite different names*

