# Comparing `tmp/aioshutil-1.3.tar.gz` & `tmp/aioshutil-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioshutil-1.3.tar", last modified: Tue Mar 14 14:01:43 2023, max compression
+gzip compressed data, was "aioshutil-1.4.tar", last modified: Mon May 27 10:58:32 2024, max compression
```

## Comparing `aioshutil-1.3.tar` & `aioshutil-1.4.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:43.327802 aioshutil-1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-14 14:01:10.000000 aioshutil-1.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:43.327802 aioshutil-1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-14 14:01:10.000000 aioshutil-1.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:43.327802 aioshutil-1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-14 14:01:10.000000 aioshutil-1.3/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-14 14:01:10.000000 aioshutil-1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-14 14:01:10.000000 aioshutil-1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-14 14:01:10.000000 aioshutil-1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-14 14:01:10.000000 aioshutil-1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-03-14 14:01:43.327802 aioshutil-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-14 14:01:10.000000 aioshutil-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:43.327802 aioshutil-1.3/aioshutil/
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-03-14 14:01:10.000000 aioshutil-1.3/aioshutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:10.000000 aioshutil-1.3/aioshutil/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:43.327802 aioshutil-1.3/aioshutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-03-14 14:01:42.000000 aioshutil-1.3/aioshutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-14 14:01:42.000000 aioshutil-1.3/aioshutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:01:42.000000 aioshutil-1.3/aioshutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:01:42.000000 aioshutil-1.3/aioshutil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-14 14:01:42.000000 aioshutil-1.3/aioshutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-14 14:01:42.000000 aioshutil-1.3/aioshutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-14 14:01:10.000000 aioshutil-1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-14 14:01:43.327802 aioshutil-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-14 14:01:10.000000 aioshutil-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:43.327802 aioshutil-1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-14 14:01:10.000000 aioshutil-1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-14 14:01:10.000000 aioshutil-1.3/tests/test_aioshutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-14 14:01:10.000000 aioshutil-1.3/tests/test_typehints.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:58:32.658408 aioshutil-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-27 10:58:19.000000 aioshutil-1.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:58:32.658408 aioshutil-1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 10:58:19.000000 aioshutil-1.4/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:58:32.658408 aioshutil-1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-27 10:58:19.000000 aioshutil-1.4/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-27 10:58:19.000000 aioshutil-1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-27 10:58:19.000000 aioshutil-1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-27 10:58:19.000000 aioshutil-1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-27 10:58:19.000000 aioshutil-1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 10:58:32.658408 aioshutil-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-27 10:58:19.000000 aioshutil-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:58:32.658408 aioshutil-1.4/aioshutil/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-27 10:58:19.000000 aioshutil-1.4/aioshutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:58:19.000000 aioshutil-1.4/aioshutil/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:58:32.658408 aioshutil-1.4/aioshutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 10:58:32.000000 aioshutil-1.4/aioshutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-27 10:58:32.000000 aioshutil-1.4/aioshutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:58:32.000000 aioshutil-1.4/aioshutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:58:32.000000 aioshutil-1.4/aioshutil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 10:58:32.000000 aioshutil-1.4/aioshutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 10:58:32.000000 aioshutil-1.4/aioshutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 10:58:19.000000 aioshutil-1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 10:58:32.658408 aioshutil-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-27 10:58:19.000000 aioshutil-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:58:32.658408 aioshutil-1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-27 10:58:19.000000 aioshutil-1.4/tests/test_aioshutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-27 10:58:19.000000 aioshutil-1.4/tests/test_typehints.yml
```

### Comparing `aioshutil-1.3/.gitattributes` & `aioshutil-1.4/.gitattributes`

 * *Files identical despite different names*

### Comparing `aioshutil-1.3/.github/workflows/CI.yml` & `aioshutil-1.4/.github/workflows/CI.yml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jobs:
   ci:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11-dev"]
+        python-version: ["3.8", "3.12"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
```

### Comparing `aioshutil-1.3/.github/workflows/publish.yml` & `aioshutil-1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aioshutil-1.3/.gitignore` & `aioshutil-1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aioshutil-1.3/.pre-commit-config.yaml` & `aioshutil-1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aioshutil-1.3/LICENSE.md` & `aioshutil-1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aioshutil-1.3/PKG-INFO` & `aioshutil-1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioshutil
-Version: 1.3
+Version: 1.4
 Summary: Asynchronous shutil module.
 Home-page: https://github.com/kumaraditya303/aioshutil
 Author: Kumar Aditya
 Author-email: 
 License: BSD License
 Keywords: asyncio,io,shutil
 Platform: UNKNOWN
@@ -12,26 +12,27 @@
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # aioshutil: Asynchronous shutil module.
 
-[![Downloads](https://pepy.tech/badge/aioshutil)](https://pepy.tech/project/aioshutil) ![](https://img.shields.io/pypi/v/aioshutil)  ![](https://img.shields.io/pypi/pyversions/aioshutil) ![](https://img.shields.io/pypi/implementation/aioshutil)
+[![Downloads](https://static.pepy.tech/badge/aioshutil)](https://pepy.tech/project/aioshutil) ![](https://img.shields.io/pypi/v/aioshutil)  ![](https://img.shields.io/pypi/pyversions/aioshutil) ![](https://img.shields.io/pypi/implementation/aioshutil)
 
 # Introduction
 
 `aioshutil` is a Python library which provides asynchronous version of function of shutil module. `shutil` module is blocking and using it in asyncio applications will block the event loop and slow down the application, `aioshutil` provides asynchronous friendly versions of the functions of the `shutil` module as it performs blocking io in a thread pool.
 
 # Installation
```

### Comparing `aioshutil-1.3/README.md` & `aioshutil-1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # aioshutil: Asynchronous shutil module.
 
-[![Downloads](https://pepy.tech/badge/aioshutil)](https://pepy.tech/project/aioshutil) ![](https://img.shields.io/pypi/v/aioshutil)  ![](https://img.shields.io/pypi/pyversions/aioshutil) ![](https://img.shields.io/pypi/implementation/aioshutil)
+[![Downloads](https://static.pepy.tech/badge/aioshutil)](https://pepy.tech/project/aioshutil) ![](https://img.shields.io/pypi/v/aioshutil)  ![](https://img.shields.io/pypi/pyversions/aioshutil) ![](https://img.shields.io/pypi/implementation/aioshutil)
 
 # Introduction
 
 `aioshutil` is a Python library which provides asynchronous version of function of shutil module. `shutil` module is blocking and using it in asyncio applications will block the event loop and slow down the application, `aioshutil` provides asynchronous friendly versions of the functions of the `shutil` module as it performs blocking io in a thread pool.
 
 # Installation
```

### Comparing `aioshutil-1.3/aioshutil/__init__.py` & `aioshutil-1.4/aioshutil/__init__.py`

 * *Files identical despite different names*

### Comparing `aioshutil-1.3/aioshutil.egg-info/PKG-INFO` & `aioshutil-1.4/aioshutil.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioshutil
-Version: 1.3
+Version: 1.4
 Summary: Asynchronous shutil module.
 Home-page: https://github.com/kumaraditya303/aioshutil
 Author: Kumar Aditya
 Author-email: 
 License: BSD License
 Keywords: asyncio,io,shutil
 Platform: UNKNOWN
@@ -12,26 +12,27 @@
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # aioshutil: Asynchronous shutil module.
 
-[![Downloads](https://pepy.tech/badge/aioshutil)](https://pepy.tech/project/aioshutil) ![](https://img.shields.io/pypi/v/aioshutil)  ![](https://img.shields.io/pypi/pyversions/aioshutil) ![](https://img.shields.io/pypi/implementation/aioshutil)
+[![Downloads](https://static.pepy.tech/badge/aioshutil)](https://pepy.tech/project/aioshutil) ![](https://img.shields.io/pypi/v/aioshutil)  ![](https://img.shields.io/pypi/pyversions/aioshutil) ![](https://img.shields.io/pypi/implementation/aioshutil)
 
 # Introduction
 
 `aioshutil` is a Python library which provides asynchronous version of function of shutil module. `shutil` module is blocking and using it in asyncio applications will block the event loop and slow down the application, `aioshutil` provides asynchronous friendly versions of the functions of the `shutil` module as it performs blocking io in a thread pool.
 
 # Installation
```

### Comparing `aioshutil-1.3/setup.py` & `aioshutil-1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         "Framework :: AsyncIO",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: BSD License",
     ],
     setup_requires=["setuptools_scm"],
```

### Comparing `aioshutil-1.3/tests/test_aioshutil.py` & `aioshutil-1.4/tests/test_aioshutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # -*- coding: utf-8 -*-
 import math
 import os
 import stat
 from pathlib import Path
 
+import pytest
+
 import aioshutil
 
+pytestmark = [pytest.mark.asyncio]
+
 
 async def test_copyfileobj(tmp_path: Path):
     (tmp_path / "temp.txt").write_text("Hello World!", encoding="utf-8")
     with open(tmp_path / "temp.txt", "r") as fsrc, open(
         tmp_path / "temp1.txt", "w"
     ) as fdst:
         await aioshutil.copyfileobj(fsrc, fdst)
```

### Comparing `aioshutil-1.3/tests/test_typehints.yml` & `aioshutil-1.4/tests/test_typehints.yml`

 * *Files identical despite different names*

