# Comparing `tmp/pyarcamsolo-0.1.1.tar.gz` & `tmp/pyarcamsolo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcamsolo-0.1.1.tar", last modified: Mon May 27 16:35:31 2024, max compression
+gzip compressed data, was "pyarcamsolo-0.1.2.tar", last modified: Mon May 27 17:59:00 2024, max compression
```

## Comparing `pyarcamsolo-0.1.1.tar` & `pyarcamsolo-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:31.812261 pyarcamsolo-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:35:31.812261 pyarcamsolo-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:31.808261 pyarcamsolo-0.1.1/pyarcamsolo/
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyarcamsolo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:31.808261 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 16:35:31.000000 pyarcamsolo-0.1.1/pyarcamsolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:35:31.812261 pyarcamsolo-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 16:35:05.000000 pyarcamsolo-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/pyarcamsolo/
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:59:00.904209 pyarcamsolo-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/setup.py
```

### Comparing `pyarcamsolo-0.1.1/LICENSE` & `pyarcamsolo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.1/PKG-INFO` & `pyarcamsolo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.1/README.md` & `pyarcamsolo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.1/pyarcamsolo/__init__.py` & `pyarcamsolo-0.1.2/pyarcamsolo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.1/pyarcamsolo/commands.py` & `pyarcamsolo-0.1.2/pyarcamsolo/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -307,8 +307,36 @@
         "system_code": 20,
         "command_code": 32
     },
     "cd_track_previous": {
         "system_code": 20,
         "command_code": 33
     },
+    "cd_scan_back": {
+        "system_code": 20,
+        "command_code": 50
+    },
+    "cd_scan_forward": {
+        "system_code": 20,
+        "command_code": 52
+    },
+    "cd_repeat_off": {
+        "system_code": 20,
+        "command_code": 117
+    },
+    "cd_shuffle_on": {
+        "system_code": 20,
+        "command_code": 118
+    },
+    "cd_shuffle_off": {
+        "system_code": 20,
+        "command_code": 119
+    },
+    "cd_repeat_single": {
+        "system_code": 20,
+        "command_code": 116
+    },
+    "cd_repeat_all": {
+        "system_code": 20,
+        "command_code": 115
+    }
 }
```

### Comparing `pyarcamsolo-0.1.1/pyarcamsolo/parser.py` & `pyarcamsolo-0.1.2/pyarcamsolo/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,14 +95,38 @@
         output["v"] = CD_PLAYBACK_STATUS_CODES.get(data, "Unknown")
     elif cc == "cdusb_playback_time":
         output["k"] = "current_track_position"
         hour = int.from_bytes(data[0:1]) * 3600
         minute = int.from_bytes(data[1:2]) * 60
         sec = int.from_bytes(data[2:3])
         output["v"] = hour+minute+sec
+    elif cc == "cdusb_total_track_time":
+        output["k"] = "current_track_duration"
+        hour = int.from_bytes(data[0:1]) * 3600
+        minute = int.from_bytes(data[1:2]) * 60
+        sec = int.from_bytes(data[2:3])
+        output["v"] = hour+minute+sec
+    elif cc == "cd_play_mode":
+        return [
+            {
+                "k": "repeat",
+                "v": None,
+                "z": output["z"]
+            },
+            {
+                "k": "shuffle",
+                "v": None,
+                "z": output["z"]
+            },
+            {
+                "k": "program",
+                "v": None,
+                "z": output["z"]
+            }
+        ]
     elif cc == "cdusb_current_track":
         return parse_cdusb_current_track(
             z=output["z"],
             b=data
         )
     elif cc == "radio_station_info":
         return parse_radio_station_info(
```

### Comparing `pyarcamsolo-0.1.1/pyarcamsolo/util.py` & `pyarcamsolo-0.1.2/pyarcamsolo/util.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.1/pyarcamsolo.egg-info/PKG-INFO` & `pyarcamsolo-0.1.2/pyarcamsolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.1/setup.py` & `pyarcamsolo-0.1.2/setup.py`

 * *Files identical despite different names*

