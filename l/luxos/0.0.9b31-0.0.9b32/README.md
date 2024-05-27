# Comparing `tmp/luxos-0.0.9b31.tar.gz` & `tmp/luxos-0.0.9b32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.9b31.tar", last modified: Mon May 27 15:40:06 2024, max compression
+gzip compressed data, was "luxos-0.0.9b32.tar", last modified: Mon May 27 15:41:16 2024, max compression
```

## Comparing `luxos-0.0.9b31.tar` & `luxos-0.0.9b32.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:06.862275 luxos-0.0.9b31/
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-27 15:40:06.862275 luxos-0.0.9b31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-27 15:39:25.000000 luxos-0.0.9b31/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-27 15:40:04.000000 luxos-0.0.9b31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:40:06.862275 luxos-0.0.9b31/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:06.858276 luxos-0.0.9b31/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:06.858276 luxos-0.0.9b31/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 15:40:04.000000 luxos-0.0.9b31/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:06.862275 luxos-0.0.9b31/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:06.862275 luxos-0.0.9b31/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-27 15:39:25.000000 luxos-0.0.9b31/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:06.862275 luxos-0.0.9b31/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-27 15:40:06.000000 luxos-0.0.9b31/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-27 15:40:06.000000 luxos-0.0.9b31/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:40:06.000000 luxos-0.0.9b31/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 15:40:06.000000 luxos-0.0.9b31/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 15:40:06.000000 luxos-0.0.9b31/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 15:40:06.000000 luxos-0.0.9b31/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:06.862275 luxos-0.0.9b31/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-27 15:39:25.000000 luxos-0.0.9b31/tests/test_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-27 15:39:25.000000 luxos-0.0.9b31/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-27 15:39:25.000000 luxos-0.0.9b31/tests/test_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-27 15:39:25.000000 luxos-0.0.9b31/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-27 15:39:25.000000 luxos-0.0.9b31/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-27 15:39:25.000000 luxos-0.0.9b31/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-27 15:39:25.000000 luxos-0.0.9b31/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:41:16.568781 luxos-0.0.9b32/
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-27 15:41:16.568781 luxos-0.0.9b32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-27 15:40:36.000000 luxos-0.0.9b32/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-27 15:41:14.000000 luxos-0.0.9b32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:41:16.568781 luxos-0.0.9b32/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:41:16.564781 luxos-0.0.9b32/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:41:16.564781 luxos-0.0.9b32/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 15:41:14.000000 luxos-0.0.9b32/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:41:16.568781 luxos-0.0.9b32/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:41:16.568781 luxos-0.0.9b32/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-27 15:40:36.000000 luxos-0.0.9b32/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:41:16.568781 luxos-0.0.9b32/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-27 15:41:16.000000 luxos-0.0.9b32/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-27 15:41:16.000000 luxos-0.0.9b32/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:41:16.000000 luxos-0.0.9b32/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 15:41:16.000000 luxos-0.0.9b32/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 15:41:16.000000 luxos-0.0.9b32/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 15:41:16.000000 luxos-0.0.9b32/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:41:16.568781 luxos-0.0.9b32/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-27 15:40:36.000000 luxos-0.0.9b32/tests/test_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-27 15:40:36.000000 luxos-0.0.9b32/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-27 15:40:36.000000 luxos-0.0.9b32/tests/test_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-27 15:40:36.000000 luxos-0.0.9b32/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-27 15:40:36.000000 luxos-0.0.9b32/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-27 15:40:36.000000 luxos-0.0.9b32/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-27 15:40:36.000000 luxos-0.0.9b32/tests/test_utils.py
```

### Comparing `luxos-0.0.9b31/PKG-INFO` & `luxos-0.0.9b32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.9b31
+Version: 0.0.9b32
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.9b31/README.md` & `luxos-0.0.9b32/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/pyproject.toml` & `luxos-0.0.9b32/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.9b31"
+version = "0.0.9b32"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.9b31/src/luxos/api.json` & `luxos-0.0.9b32/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/api.py` & `luxos-0.0.9b32/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/asyncops.py` & `luxos-0.0.9b32/src/luxos/asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/cli/flags.py` & `luxos-0.0.9b32/src/luxos/cli/flags.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/cli/v1.py` & `luxos-0.0.9b32/src/luxos/cli/v1.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/exceptions.py` & `luxos-0.0.9b32/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/ips.py` & `luxos-0.0.9b32/src/luxos/ips.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/misc.py` & `luxos-0.0.9b32/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/scripts/async_luxos.py` & `luxos-0.0.9b32/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/scripts/health_checker.py` & `luxos-0.0.9b32/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/scripts/luxos.py` & `luxos-0.0.9b32/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/text.py` & `luxos-0.0.9b32/src/luxos/text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos/utils.py` & `luxos-0.0.9b32/src/luxos/utils.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.9b32/src/luxos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.9b31
+Version: 0.0.9b32
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.9b31/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.9b32/src/luxos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/tests/test_asyncops.py` & `luxos-0.0.9b32/tests/test_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/tests/test_cli.py` & `luxos-0.0.9b32/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/tests/test_ips.py` & `luxos-0.0.9b32/tests/test_ips.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/tests/test_misc.py` & `luxos-0.0.9b32/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/tests/test_text.py` & `luxos-0.0.9b32/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.9b31/tests/test_utils.py` & `luxos-0.0.9b32/tests/test_utils.py`

 * *Files identical despite different names*

