# Comparing `tmp/pyarcamsolo-0.1.0.tar.gz` & `tmp/pyarcamsolo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcamsolo-0.1.0.tar", last modified: Mon May 27 16:13:47 2024, max compression
+gzip compressed data, was "pyarcamsolo-0.1.1.tar", last modified: Mon May 27 16:35:31 2024, max compression
```

## Comparing `pyarcamsolo-0.1.0.tar` & `pyarcamsolo-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:13:47.156689 pyarcamsolo-0.1.0/pyarcamsolo/
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:31.812261 pyarcamsolo-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:35:31.812261 pyarcamsolo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:31.808261 pyarcamsolo-0.1.1/pyarcamsolo/
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:31.808261 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:35:31.812261 pyarcamsolo-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/setup.py
```

### Comparing `pyarcamsolo-0.1.0/LICENSE` & `pyarcamsolo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.0/PKG-INFO` & `pyarcamsolo-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.0/README.md` & `pyarcamsolo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.0/pyarcamsolo/__init__.py` & `pyarcamsolo-0.1.1/pyarcamsolo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.0/pyarcamsolo/commands.py` & `pyarcamsolo-0.1.1/pyarcamsolo/commands.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.0/pyarcamsolo/parser.py` & `pyarcamsolo-0.1.1/pyarcamsolo/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,17 @@
     """Parse radio ration information."""
     global CURRENT_SOURCE
     d1 = get_radio_query_code(b[0:1])
     if d1 == "request_station_frequency":
         mhz = int.from_bytes(b[1:2])
         khz = int.from_bytes(b[2:3])
         if CURRENT_SOURCE == "AM":
-            val = str(mhz) + str(khz)
+            val = int(str(mhz).zfill(2) + str(khz).zfill(2))
         elif CURRENT_SOURCE == "FM":
-            val = int(str(mhz) + str(khz).zfill(2))/100
+            val = int(str(mhz).zfill(2) + str(khz).zfill(2))/100
         else:
             val = None
         return {
             "k": "radio_frequency",
             "v": val,
             "z": z
         }
```

### Comparing `pyarcamsolo-0.1.0/pyarcamsolo/util.py` & `pyarcamsolo-0.1.1/pyarcamsolo/util.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.0/pyarcamsolo.egg-info/PKG-INFO` & `pyarcamsolo-0.1.1/pyarcamsolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.0/setup.py` & `pyarcamsolo-0.1.1/setup.py`

 * *Files identical despite different names*

