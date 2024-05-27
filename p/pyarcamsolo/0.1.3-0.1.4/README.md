# Comparing `tmp/pyarcamsolo-0.1.3.tar.gz` & `tmp/pyarcamsolo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcamsolo-0.1.3.tar", last modified: Mon May 27 18:32:33 2024, max compression
+gzip compressed data, was "pyarcamsolo-0.1.4.tar", last modified: Mon May 27 18:52:59 2024, max compression
```

## Comparing `pyarcamsolo-0.1.3.tar` & `pyarcamsolo-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:32:33.993342 pyarcamsolo-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 18:32:33.993342 pyarcamsolo-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:32:33.989342 pyarcamsolo-0.1.3/pyarcamsolo/
--rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:32:33.989342 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:32:33.993342 pyarcamsolo-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:52:59.687801 pyarcamsolo-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 18:52:59.687801 pyarcamsolo-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:52:59.687801 pyarcamsolo-0.1.4/pyarcamsolo/
+-rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/pyarcamsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/pyarcamsolo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/pyarcamsolo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/pyarcamsolo/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/pyarcamsolo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/pyarcamsolo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:52:59.687801 pyarcamsolo-0.1.4/pyarcamsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 18:52:59.000000 pyarcamsolo-0.1.4/pyarcamsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 18:52:59.000000 pyarcamsolo-0.1.4/pyarcamsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:52:59.000000 pyarcamsolo-0.1.4/pyarcamsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 18:52:59.000000 pyarcamsolo-0.1.4/pyarcamsolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 18:52:59.000000 pyarcamsolo-0.1.4/pyarcamsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 18:52:59.000000 pyarcamsolo-0.1.4/pyarcamsolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:52:59.687801 pyarcamsolo-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 18:52:34.000000 pyarcamsolo-0.1.4/setup.py
```

### Comparing `pyarcamsolo-0.1.3/LICENSE` & `pyarcamsolo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.3/PKG-INFO` & `pyarcamsolo-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.3/README.md` & `pyarcamsolo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.3/pyarcamsolo/__init__.py` & `pyarcamsolo-0.1.4/pyarcamsolo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.3/pyarcamsolo/commands.py` & `pyarcamsolo-0.1.4/pyarcamsolo/commands.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.3/pyarcamsolo/parser.py` & `pyarcamsolo-0.1.4/pyarcamsolo/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,20 +75,18 @@
         output["k"] = cc
         output["v"] = f"{data[0]}.{data[1]}"
     elif cc == "balance":
         output["k"] = cc
         output["v"] = (data[0])-100
     elif cc == "bass":
         output["k"] = cc
-        output["v"] = bytes_to_int_with_offset(data[0], 2, 0x5D,
-                                               range_upper_limit=14)
+        output["v"] = (int.from_bytes(data[0:])-100)*2
     elif cc == "treble":
         output["k"] = cc
-        output["v"] = bytes_to_int_with_offset(data[0], 2, 0x5D,
-                                               range_upper_limit=14)
+        output["v"] = (int.from_bytes(data[0:])-100)*2
     elif cc == "display_brightness":
         output["k"] = cc
         output["v"] = data[0]
     elif cc == "stby_display_brightness":
         output["k"] = "standby_display_brightness"
         output["v"] = data[0]
     elif cc == "cd_playback_state":
@@ -238,17 +236,7 @@
         },
         {
             "k": "lsb_total_track",
             "v": lsb_total_track,
             "z": z
         },
     ]
-
-def bytes_to_int_with_offset(b: bytes, offset: int, normalizer, range_upper_limit: int):
-    """Converts bytes to an int with a provided offset"""
-    i = int.from_bytes(b, byteorder='big', signed=True)
-    # apply a base range from a normalizer
-    i -= normalizer
-    # now apply scaling using the offset provided
-    i *= offset
-    i -= range_upper_limit
-    return i
```

### Comparing `pyarcamsolo-0.1.3/pyarcamsolo/util.py` & `pyarcamsolo-0.1.4/pyarcamsolo/util.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.3/pyarcamsolo.egg-info/PKG-INFO` & `pyarcamsolo-0.1.4/pyarcamsolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.3/setup.py` & `pyarcamsolo-0.1.4/setup.py`

 * *Files identical despite different names*

