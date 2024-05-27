# Comparing `tmp/open_aea_ledger_ethereum_flashbots-1.52.0.tar.gz` & `tmp/open_aea_ledger_ethereum_flashbots-1.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_aea_ledger_ethereum_flashbots-1.52.0.tar", last modified: Mon May  6 07:25:17 2024, max compression
+gzip compressed data, was "open_aea_ledger_ethereum_flashbots-1.53.0.tar", last modified: Mon May 27 09:29:41 2024, max compression
```

## Comparing `open_aea_ledger_ethereum_flashbots-1.52.0.tar` & `open_aea_ledger_ethereum_flashbots-1.53.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:17.529401 open_aea_ledger_ethereum_flashbots-1.52.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 07:25:17.529401 open_aea_ledger_ethereum_flashbots-1.52.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:17.529401 open_aea_ledger_ethereum_flashbots-1.52.0/aea_ledger_ethereum_flashbots/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/aea_ledger_ethereum_flashbots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/aea_ledger_ethereum_flashbots/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:17.529401 open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 07:25:17.000000 open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 07:25:17.000000 open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:25:17.000000 open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-06 07:25:17.000000 open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 07:25:17.000000 open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 07:25:17.000000 open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:25:17.529401 open_aea_ledger_ethereum_flashbots-1.52.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:25:17.529401 open_aea_ledger_ethereum_flashbots-1.52.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-06 07:24:46.000000 open_aea_ledger_ethereum_flashbots-1.52.0/tests/test_ethereum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.058302 open_aea_ledger_ethereum_flashbots-1.53.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-27 09:29:41.058302 open_aea_ledger_ethereum_flashbots-1.53.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.058302 open_aea_ledger_ethereum_flashbots-1.53.0/aea_ledger_ethereum_flashbots/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/aea_ledger_ethereum_flashbots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/aea_ledger_ethereum_flashbots/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.058302 open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-27 09:29:41.000000 open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-27 09:29:41.000000 open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:29:41.000000 open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-27 09:29:41.000000 open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 09:29:41.000000 open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 09:29:41.000000 open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:29:41.058302 open_aea_ledger_ethereum_flashbots-1.53.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:29:41.058302 open_aea_ledger_ethereum_flashbots-1.53.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-27 09:29:07.000000 open_aea_ledger_ethereum_flashbots-1.53.0/tests/test_ethereum.py
```

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/LICENSE` & `open_aea_ledger_ethereum_flashbots-1.53.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/PKG-INFO` & `open_aea_ledger_ethereum_flashbots-1.53.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.52.0
+Version: 1.53.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,11 +19,11 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: open-aea-ledger-ethereum~=1.52.0
+Requires-Dist: open-aea-ledger-ethereum~=1.53.0
 Requires-Dist: open-aea-flashbots==1.4.0
 
 Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
```

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/aea_ledger_ethereum_flashbots/__init__.py` & `open_aea_ledger_ethereum_flashbots-1.53.0/aea_ledger_ethereum_flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py` & `open_aea_ledger_ethereum_flashbots-1.53.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO` & `open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.52.0
+Version: 1.53.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,11 +19,11 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9,<4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: open-aea-ledger-ethereum~=1.52.0
+Requires-Dist: open-aea-ledger-ethereum~=1.53.0
 Requires-Dist: open-aea-flashbots==1.4.0
 
 Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
```

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt` & `open_aea_ledger_ethereum_flashbots-1.53.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/setup.py` & `open_aea_ledger_ethereum_flashbots-1.53.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_ethereum_flashbots" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-flashbots",
-    version="1.52.0",
+    version="1.53.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.",
     long_description=(
         "Python package extending the default open-aea ethereum ledger plugin to add support for flashbots."
     ),
     long_description_content_type="text/markdown",
@@ -37,15 +37,15 @@
     package_data={
         "aea_ledger_ethereum_flashbots": [
             "py.typed",
         ]
     },
     python_requires=">=3.9,<4.0",
     install_requires=[
-        "open-aea-ledger-ethereum~=1.52.0",
+        "open-aea-ledger-ethereum~=1.53.0",
         "open-aea-flashbots==1.4.0",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": [
             "ethereum_flashbots = aea_ledger_ethereum_flashbots:EthereumFlashbotCrypto"
         ],
```

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/tests/__init__.py` & `open_aea_ledger_ethereum_flashbots-1.53.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open_aea_ledger_ethereum_flashbots-1.52.0/tests/test_ethereum.py` & `open_aea_ledger_ethereum_flashbots-1.53.0/tests/test_ethereum.py`

 * *Files identical despite different names*

