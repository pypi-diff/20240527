# Comparing `tmp/myelectricaldatapy-2.2.0.tar.gz` & `tmp/myelectricaldatapy-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-2.2.0.tar", last modified: Mon Apr 29 07:26:24 2024, max compression
+gzip compressed data, was "myelectricaldatapy-2.2.1.tar", last modified: Mon May 27 16:17:10 2024, max compression
```

## Comparing `myelectricaldatapy-2.2.0.tar` & `myelectricaldatapy-2.2.1.tar`

### file list

```diff
@@ -1,43 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.783862 myelectricaldatapy-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/dependbot-auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/mypdl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/myelectricaldatapy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 07:26:24.000000 myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:26:24.791862 myelectricaldatapy-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:24.787862 myelectricaldatapy-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-29 07:26:11.000000 myelectricaldatapy-2.2.0/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.607966 myelectricaldatapy-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.599966 myelectricaldatapy-2.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.599966 myelectricaldatapy-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.599966 myelectricaldatapy-2.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-27 16:17:10.607966 myelectricaldatapy-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.603966 myelectricaldatapy-2.2.1/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/mypdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/myelectricaldatapy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.603966 myelectricaldatapy-2.2.1/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-27 16:17:10.000000 myelectricaldatapy-2.2.1/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-27 16:17:10.000000 myelectricaldatapy-2.2.1/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:17:10.000000 myelectricaldatapy-2.2.1/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 16:17:10.000000 myelectricaldatapy-2.2.1/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 16:17:10.000000 myelectricaldatapy-2.2.1/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:17:10.607966 myelectricaldatapy-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.603966 myelectricaldatapy-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:17:10.603966 myelectricaldatapy-2.2.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/access.json
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/address.json
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/contract.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/daily.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21145 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/detail.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/ecowatt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/invalid_access.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/fixtures/tempo.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12707 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-27 16:16:59.000000 myelectricaldatapy-2.2.1/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-2.2.0/.github/dependabot.yml` & `myelectricaldatapy-2.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.0/.github/workflows/lint.yml` & `myelectricaldatapy-2.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.0/.github/workflows/pythonpublish.yml` & `myelectricaldatapy-2.2.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.0/.github/workflows/release.yml` & `myelectricaldatapy-2.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.0/.gitignore` & `myelectricaldatapy-2.2.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -106,9 +106,9 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 #pyannotate
 type_info.json
 
-#perso
-test_home.py
+# Secret files
+secrets.yaml
```

### Comparing `myelectricaldatapy-2.2.0/.pre-commit-config.yaml` & `myelectricaldatapy-2.2.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.1
+    rev: v0.4.4
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
@@ -43,13 +43,13 @@
         stages: [manual]
         args:
           - --py311-plus
           - --force
           - --keep-updates
         files: ^(/.+)?[^/]+\.py$
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         args: [--strict, --ignore-missing-imports]
         additional_dependencies: [types-requests==2.28.11.7]
         exclude: tests/
```

### Comparing `myelectricaldatapy-2.2.0/LICENSE` & `myelectricaldatapy-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.0/PKG-INFO` & `myelectricaldatapy-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.2.0/README.md` & `myelectricaldatapy-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.0/example.py` & `myelectricaldatapy-2.2.1/example.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """Example code."""
 
 import asyncio
-import logging
 from datetime import datetime, timedelta
+import logging
+
+import yaml
 
 from myelectricaldatapy import Enedis, EnedisByPDL, EnedisException
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 # create console handler and set level to debug
 ch = logging.StreamHandler()
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
-# Please , fill good values...
-PDL = "0123456789"
-TOKEN = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+# Fill out the secrets in secrets.yaml, you can find an example
+# _secrets.yaml file, which has to be renamed after filling out the secrets.
+with open("./secrets.yaml", encoding="UTF-8") as file:
+    secrets = yaml.safe_load(file)
+
+TOKEN = secrets["TOKEN"]
+PDL = secrets["PDL"]
 
 
-async def main() -> None:
+async def async_main() -> None:
     """Main function."""
 
     api = Enedis(token=TOKEN)
 
     try:
         start = datetime.now() - timedelta(days=7)
         end = datetime.now()
@@ -34,14 +39,20 @@
         data = await api.async_get_contract(PDL)
         logger.info(data)
         data = await api.async_get_addresses(PDL)
         logger.info(data)
     except EnedisException as error:
         logger.error(error)
 
+    await api.async_close()
+
     myPdl = EnedisByPDL(PDL, TOKEN)
-    await myPdl.async_update()
-    print(myPdl.stats)
+    try:
+        await myPdl.async_update()
+        logger.info(myPdl.stats)
+    except EnedisException as error:
+        logger.error(error)
 
 
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
+if __name__ == "__main__":
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(async_main())
```

### Comparing `myelectricaldatapy-2.2.0/myelectricaldatapy/analytics.py` & `myelectricaldatapy-2.2.1/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-2.2.0/myelectricaldatapy/auth.py` & `myelectricaldatapy-2.2.1/myelectricaldatapy/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 import asyncio
 import json
 import logging
 import socket
 from typing import Any
 
-import async_timeout
-from aiohttp import ClientError, ClientSession
+from aiohttp import ClientError, ClientResponseError, ClientSession
 
 from .const import TIMEOUT, URL
 from .exceptions import (
     EnedisException,
     HttpRequestError,
     LimitReached,
     TimeoutExceededError,
@@ -22,63 +21,48 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 class EnedisAuth:
     """Class for Enedis Auth API."""
 
     def __init__(
-        self, token: str, session: ClientSession | None = None, timeout: int = TIMEOUT
+        self, session: ClientSession, token: str, timeout: int = TIMEOUT
     ) -> None:
         """Init."""
         self.token = token
         self.timeout = timeout
-        self.session = session if session else ClientSession()
+        self.session = session
 
-    async def async_close(self) -> None:
-        """Close session."""
-        await self.session.close()
-
-    async def request(self, path: str, method: str = "GET", **kwargs: Any) -> Any:
+    async def async_request(self, path: str, method: str = "get", **kwargs: Any) -> Any:
         """Request session."""
-        url = f"{URL}/{path}"
-        if headers := kwargs.get("headers", {}):
-            headers = dict(headers)
-
-        headers.update(
+        kwargs.setdefault("headers", {})
+        kwargs["headers"].update(
             {"Content-Type": "application/json", "Authorization": self.token}
         )
 
         try:
-            async with async_timeout.timeout(TIMEOUT):
-                _LOGGER.debug("Request %s (%s)", url, kwargs)
-                response = await self.session.request(
-                    method, url, **kwargs, headers=headers
-                )
+            async with asyncio.timeout(self.timeout):
+                _LOGGER.debug("Request: %s (%s) - %s", path, method, kwargs.get("json"))
+                response = await self.session.request(method, f"{URL}/{path}", **kwargs)
+                contents = await response.read()
+                response.raise_for_status()
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to MyElectricalData."
             ) from error
+        except ClientResponseError:
+            message = contents.decode("utf8")
+            if "application/json" in response.headers.get("Content-Type", ""):
+                if response.status == 409:
+                    raise LimitReached(json.loads(message))
+                raise EnedisException(json.loads(message))
+            raise EnedisException({"message": message})
         except (ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with MyElectricalData."
             ) from error
 
-        content_type = response.headers.get("Content-Type", "")
-        if response.status // 100 in [4, 5]:
-            contents = await response.read()
-            response.close()
-
-            message = contents.decode("utf8")
-            if content_type == "application/json":
-                if response.status == 409:
-                    raise LimitReached(response.status, json.loads(message))
-                raise EnedisException(response.status, json.loads(message))
-            raise EnedisException(response.status, {"message": message})
-
-        if "application/json" in content_type:
-            rslt = await response.json()
-            _LOGGER.debug("Response %s", rslt)
-            return rslt
-
-        rslt = await response.text()
-        _LOGGER.debug("Response %s", rslt)
-        return rslt
+        return (
+            await response.json()
+            if "application/json" in response.headers.get("Content-Type", "")
+            else await response.text()
+        )
```

### Comparing `myelectricaldatapy-2.2.0/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-2.2.1/myelectricaldatapy/myelectricaldata.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """Class for Enedis Gateway (http://www.myelectricaldata.fr)."""
 
 from __future__ import annotations
 
 from datetime import date, datetime as dt, timedelta
 import logging
 import re
-from types import TracebackType
 from typing import Any, Generator, cast
 
+from aiohttp import ClientSession
+
 from .auth import EnedisAuth
 from .const import DAILY_CONSUM, DAILY_PROD, DETAIL_CONSUM, DETAIL_PROD, TIMEOUT
+from .exceptions import EnedisException
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Enedis:
     """Get data of pdl."""
 
     def __init__(
-        self, token: str, session: Any | None = None, timeout: int = TIMEOUT
+        self,
+        token: str,
+        session: ClientSession = ClientSession(),
+        timeout: int = TIMEOUT,
     ) -> None:
         """Initialize."""
-        self.auth = EnedisAuth(token, session, timeout)
+        self.auth = EnedisAuth(session, token, timeout)
+        self.async_request = self.auth.async_request
         self.offpeaks: list[str] = []
         self.dt_offpeak: list[dt] = []
         self.last_access: date | None = None
 
     async def async_fetch_datas(
         self, service: str, pdl: str, start: dt | None = None, end: dt | None = None
     ) -> Any:
@@ -39,15 +45,15 @@
         self.last_access = dt.now()
         path_range = ""
         if start and end:
             start_date = start.strftime("%Y-%m-%d")
             end_date = end.strftime("%Y-%m-%d")
             path_range = f"/start/{start_date}/end/{end_date}"
         path = f"{service}/{pdl}{path_range}"
-        return await self.auth.request(path=path)
+        return await self.async_request(path=path)
 
     async def async_valid_access(self, pdl: str) -> Any:
         """Return valid access."""
         return await self.async_fetch_datas("valid_access", pdl)
 
     async def async_has_access(self, pdl: str) -> bool:
         """Check valid access."""
@@ -99,29 +105,29 @@
             start.strftime("%Y-%m-%d") if start else dt.now().strftime("%Y-%m-%d")
         )
         str_end = (
             end.strftime("%Y-%m-%d")
             if end
             else (dt.now() + timedelta(days=1)).strftime("%Y-%m-%d")
         )
-        return await self.auth.request(path=f"rte/tempo/{str_start}/{str_end}")
+        return await self.auth.async_request(path=f"rte/tempo/{str_start}/{str_end}")
 
     async def async_get_ecowatt(
         self, start: dt | None = None, end: dt | None = None
     ) -> Any:
         """Return Ecowatt information."""
         str_start = (
             start.strftime("%Y-%m-%d") if start else dt.now().strftime("%Y-%m-%d")
         )
         str_end = (
             end.strftime("%Y-%m-%d")
             if end
             else (dt.now() + timedelta(days=1)).strftime("%Y-%m-%d")
         )
-        return await self.auth.request(path=f"rte/ecowatt/{str_start}/{str_end}")
+        return await self.async_request(path=f"rte/ecowatt/{str_start}/{str_end}")
 
     async def async_has_offpeak(self, pdl: str) -> bool:
         """Has offpeak hours."""
         if not self.offpeaks:
             await self.async_get_contract(pdl)
         return len(self.offpeaks) > 0
 
@@ -146,85 +152,69 @@
 
     async def async_get_daily_production(self, pdl: str, start: dt, end: dt) -> Any:
         """Get daily production."""
         return await self.async_fetch_datas(DAILY_PROD, pdl, start, end)
 
     async def async_get_details_consumption(self, pdl: str, start: dt, end: dt) -> Any:
         """Get consumption details. (max: 7 days)."""
-        data = None
-        for interval in list(self.date_range(start, end, 7)):
-            start, end = interval
-            try:
-                rsp = await self.async_fetch_datas(DETAIL_CONSUM, pdl, start, end)
-            finally:
-                if (
-                    rsp is None
-                    or rsp.get("meter_reading", {}).get("interval_reading") is None
-                ):
-                    continue
-                elif data is None:
-                    data = cast(dict[str, Any], rsp)
-                else:
-                    data["meter_reading"]["interval_reading"].extend(
-                        rsp.get("meter_reading", {}).get("interval_reading")
-                    )
-
-        return data
+        return await self._async_get_details(DETAIL_CONSUM, pdl, start, end)
 
     async def async_get_details_production(self, pdl: str, start: dt, end: dt) -> Any:
         """Get production details. (max: 7 days)."""
+        return await self._async_get_details(DETAIL_PROD, pdl, start, end)
+
+    async def async_get_max_power(self, pdl: str, start: dt, end: dt) -> Any:
+        """Get consumption max power."""
+        return await self.async_fetch_datas(
+            "daily_consumption_max_power", pdl, start, end
+        )
+
+    async def _async_get_details(self, mode: str, pdl: str, start: dt, end: dt) -> Any:
+        """Get production details. (max: 7 days)."""
         data = None
+        response = {}
+        raise_error = False
         for interval in list(self.date_range(start, end, 7)):
             start, end = interval
             try:
-                rsp = await self.async_fetch_datas(DETAIL_PROD, pdl, start, end)
+                if raise_error is False:
+                    response = await self.async_fetch_datas(mode, pdl, start, end)
+            except EnedisException as error:
+                raise_error = True
+                _LOGGER.error(error)
             finally:
-                if (
-                    rsp is None
-                    or rsp.get("meter_reading", {}).get("interval_reading") is None
-                ):
+                new_data = response.get("meter_reading", {}).get("interval_reading")
+                if response is None or new_data is None:
                     continue
                 elif data is None:
-                    data = cast(dict[str, Any], rsp)
+                    data = cast(dict[str, Any], response)
                 else:
-                    data["meter_reading"]["interval_reading"].extend(
-                        rsp.get("meter_reading", {}).get("interval_reading")
-                    )
+                    data["meter_reading"]["interval_reading"].extend(new_data)
 
         return data
 
-    async def async_get_max_power(self, pdl: str, start: dt, end: dt) -> Any:
-        """Get consumption max power."""
-        return await self.async_fetch_datas(
-            "daily_consumption_max_power", pdl, start, end
-        )
-
-    async def __aenter__(self) -> Enedis:
-        """Asynchronous enter."""
-        return self
-
-    async def __aexit__(
-        self,
-        exc_type: type[BaseException] | None,
-        exc_value: BaseException | None,
-        traceback: TracebackType | None,
-    ) -> None:
-        """Asynchronous exit."""
-        await self.close()
-
-    async def close(self) -> None:
-        """Close the session."""
-        await self.auth.async_close()
-
     @staticmethod
     def date_range(start: dt, end: dt, intv: int) -> Generator[tuple[dt, dt], dt, None]:
         """Return range by interval date."""
         diff = (
             (end - start).days // intv
             if (end - start).days % intv == 0
             else ((end - start).days // intv) + 1
         )
         for i in range(1, diff):
             s_end = start + timedelta(days=intv)
             yield (start, s_end)
             start = s_end
         yield (start, end)
+
+    async def __aenter__(self) -> Enedis:
+        """Asynchronous enter."""
+        return self
+
+    async def __aexit__(self, *_exc_info: object) -> None:
+        """Async exit."""
+        await self.async_close()
+
+    async def async_close(self) -> None:
+        """Close the session."""
+        if self.auth.session:
+            await self.auth.session.close()
```

### Comparing `myelectricaldatapy-2.2.0/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-2.2.1/myelectricaldatapy/mypdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from datetime import date, datetime as dt, timedelta
 import logging
 from typing import Any, Callable, Tuple
 
+from aiohttp import ClientSession
 import voluptuous as vol
 
 from myelectricaldatapy import Enedis, EnedisException, LimitReached
 
 from .analytics import EnedisAnalytics
 from .const import (
     ATTR_CUM_PRICE,
@@ -84,15 +85,15 @@
 class EnedisByPDL:
     """PDL class."""
 
     def __init__(
         self,
         pdl: str,
         token: str,
-        session: Any | None = None,
+        session: ClientSession = ClientSession(),
         timeout: int = TIMEOUT,
     ) -> None:
         """Initialize."""
         self._api: Enedis = Enedis(token, session, timeout)
         self.pdl = pdl
         self._connected: bool = False
         self._ecowatt_subs: bool = False
```

### Comparing `myelectricaldatapy-2.2.0/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-2.2.1/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 2.2.0
+Version: 2.2.1
 Summary: Fetch Linky data from myelectricaldata.fr
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `myelectricaldatapy-2.2.0/pyproject.toml` & `myelectricaldatapy-2.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     "aiohttp>=3.8.1",
     "pandas>=2.0.2",
     "voluptuous>=0.13.1",
 ]
 
 [tool.setuptools_scm]
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.flake8-tidy-imports.banned-api]
-"async_timeout".msg = "use asyncio.timeout instead"
-"pytz".msg = "use zoneinfo instead"
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-sort-within-sections = true
 combine-as-imports = true
 split-on-trailing-comma = false
+
+[[tool.mypy.overrides]]
+module = "yaml"
+ignore_missing_imports = true
```

### Comparing `myelectricaldatapy-2.2.0/tests/test_analytics.py` & `myelectricaldatapy-2.2.1/tests/test_analytics.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import Any
 from unittest.mock import Mock, patch
 
 from freezegun import freeze_time
 import pytest
 
 import myelectricaldatapy
-from myelectricaldatapy import EnedisByPDL
+from myelectricaldatapy import EnedisByPDL, LimitReached
 
-from .consts import DATASET_DAILY_COMPARE, PDL, TOKEN
+from .consts import PDL, TOKEN
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
 async def test_compute(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test standard."""
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
@@ -155,18 +155,38 @@
     print(resultat1)
     sum_value = 0
     for rslt in resultat1:
         sum_value += rslt["value"]
     sum_value_1 = resultat1[26]["sum_value"] + resultat1[77]["sum_value"]
     assert round(sum_value, 3) == round(sum_value_1, 3)
 
+    daily_comsumption = {
+        "meter_reading": {
+            "usage_point_id": "01234567890",
+            "start": "2022-03-08",
+            "end": "2023-03-08",
+            "quality": "BRUT",
+            "reading_type": {
+                "measurement_kind": "energy",
+                "measuring_period": "P1D",
+                "unit": "Wh",
+                "aggregate": "sum",
+            },
+            "interval_reading": [
+                {"value": "77559", "date": "2023-03-01"},
+                {"value": "68680", "date": "2023-03-02"},
+                {"value": "81972", "date": "2023-03-03"},
+            ],
+        }
+    }
+
     with patch.object(
         myelectricaldatapy.Enedis,
         "async_get_daily_consumption",
-        return_value=DATASET_DAILY_COMPARE,
+        return_value=daily_comsumption,
     ):
         api.set_collects(
             "daily_consumption",
             prices=prices,
             intervals=intervals,
             cum_value=cumsum_value,
             cum_price=cumsum_price,
@@ -203,33 +223,49 @@
     # standard
     assert resultat[27]["sum_value"] == resultat[27]["value"] + 100
     assert resultat[27]["sum_price"] == resultat[27]["price"] + 50
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
-async def test_extra_date(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
+async def test_extra_date(mock_base: Mock, mock_detail) -> None:  # pylint: disable=unused-argument
     """Test cumulative summary."""
     prices: dict[str, Any] = {"standard": {"price": 0.17}, "offpeak": {"price": 0.18}}
     intervals = [("01:30:00", "08:00:00"), ("12:30:00", "14:00:00")]
     api = EnedisByPDL(pdl=PDL, token=TOKEN)
     api.set_collects(
         "consumption_load_curve",
         start=dt.strptime("2023-03-01", "%Y-%m-%d"),
         end=dt.strptime("2023-03-28", "%Y-%m-%d"),
         prices=prices,
         intervals=intervals,
     )
-    await api.async_update_collects()
+    with patch("myelectricaldatapy.Enedis.async_fetch_datas", return_value=mock_detail):
+        await api.async_update_collects()
     resultat = api.stats["consumption"]
     # offpeak
     assert resultat[0]["sum_value"] is not None
     # standard
     assert resultat[27]["sum_value"] is not None
 
+    api.set_collects(
+        "consumption_load_curve",
+        start=dt.strptime("2023-03-01", "%Y-%m-%d"),
+        end=dt.strptime("2023-03-28", "%Y-%m-%d"),
+        prices=prices,
+        intervals=intervals,
+    )
+    with patch(
+        "myelectricaldatapy.Enedis.async_fetch_datas",
+        side_effect=[mock_detail, LimitReached(500, {"detail": "Limit reached"})],
+    ):
+        await api.async_update_collects()
+        resultat = api.stats["consumption"]
+        assert resultat[0]["sum_value"] is not None
+
 
 @freeze_time("2023-3-1")
 @pytest.mark.asyncio
 async def test_tempo(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test tempo pricings."""
     prices: dict[str, Any] = {
         "standard": {
```

### Comparing `myelectricaldatapy-2.2.0/tests/test_load_data.py` & `myelectricaldatapy-2.2.1/tests/test_load_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Tests  Enedis api."""
 
 from __future__ import annotations
 
 from datetime import datetime as dt
 from unittest.mock import Mock, patch
 
-import pytest
 from freezegun import freeze_time
+import pytest
 
 import myelectricaldatapy
 from myelectricaldatapy import Enedis, EnedisByPDL, EnedisException, LimitReached
 
-from .consts import DATASET_30, INVALID_ACCESS, INVALID_ECOWATT, PDL, TOKEN
+from .consts import PDL, TOKEN
 
 
 @freeze_time("2023-01-23")
 @pytest.mark.asyncio
 async def test_ecowatt(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test get ecowatt."""
     api = Enedis(token=TOKEN)
@@ -23,17 +23,23 @@
     assert resultat["2023-01-22"]["value"] == 1
 
     mypdl = EnedisByPDL(pdl=PDL, token=TOKEN)
     mypdl.ecowatt_subscription(True)
     await mypdl.async_update()
     assert mypdl.ecowatt_day["message"] == "Pas d’alerte."
 
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("mock_ecowatt", [True], indirect=True)
+async def test_invalid_ecowatt(mock_enedis: Mock, mock_ecowatt: bool) -> None:
+    """Test ecowatt."""
     with patch.object(
-        myelectricaldatapy.Enedis, "async_get_ecowatt", return_value=INVALID_ECOWATT
+        myelectricaldatapy.Enedis, "async_get_ecowatt", return_value=mock_ecowatt
     ):
+        api = Enedis(token=TOKEN)
         resultat = await api.async_get_ecowatt()
         assert resultat.get("2023-01-22") is None
 
 
 @freeze_time("2023-3-3")
 @pytest.mark.asyncio
 async def test_tempoday(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
@@ -47,49 +53,55 @@
     mypdl.tempo_subscription(True)
     await mypdl.async_update()
     resultat = mypdl.stats["consumption"]
     assert mypdl.tempo_day == "blue"
 
 
 @pytest.mark.asyncio
-async def test_valid_access(
-    mock_enedis: Mock,  # pylint: disable=unused-argument
-) -> None:
+async def test_valid_access(mock_enedis: Mock) -> None:  # pylint: disable=unused-argument
     """Test access."""
     api = Enedis(token=TOKEN)
     resultat = await api.async_valid_access(PDL)
     assert resultat["valid"] is True
 
     resultat = await api.async_has_access(PDL)
     assert resultat is True
 
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("mock_access", [True], indirect=True)
+async def test_invalid_access(
+    mock_enedis: Mock,
+    mock_access: bool,  # pylint: disable=unused-argument
+) -> None:
+    """Test access."""
     with patch.object(
-        myelectricaldatapy.Enedis, "async_valid_access", return_value=INVALID_ACCESS
+        myelectricaldatapy.Enedis, "async_valid_access", return_value=mock_access
     ):
         api = Enedis(token=TOKEN)
         resultat = await api.async_valid_access(PDL)
         assert resultat["quota_reached"] is True
 
 
 @pytest.mark.asyncio
-async def test_fetch_data() -> None:
+async def test_fetch_data(mock_detail) -> None:
     """Test fetch data."""
     with patch.object(
-        myelectricaldatapy.auth.EnedisAuth, "request", return_value=DATASET_30
+        myelectricaldatapy.auth.EnedisAuth, "async_request", return_value=mock_detail
     ):
         api = Enedis(token=TOKEN)
         resultat = await api.async_fetch_datas(
             service="comsumption_load_curve",
             pdl=PDL,
             start=dt.strptime("2022-12-30", "%Y-%m-%d"),
             end=dt.strptime("2022-12-31", "%Y-%m-%d"),
         )
         assert (
             resultat["meter_reading"]["interval_reading"]
-            == DATASET_30["meter_reading"]["interval_reading"]  # noqa
+            == mock_detail["meter_reading"]["interval_reading"]  # noqa
         )
 
 
 @pytest.mark.asyncio
 async def test_force_refresh(
     mock_enedis: Mock,  # pylint: disable=unused-argument
 ) -> None:
```

