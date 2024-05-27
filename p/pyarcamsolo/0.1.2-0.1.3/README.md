# Comparing `tmp/pyarcamsolo-0.1.2.tar.gz` & `tmp/pyarcamsolo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcamsolo-0.1.2.tar", last modified: Mon May 27 17:59:00 2024, max compression
+gzip compressed data, was "pyarcamsolo-0.1.3.tar", last modified: Mon May 27 18:32:33 2024, max compression
```

## Comparing `pyarcamsolo-0.1.2.tar` & `pyarcamsolo-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/pyarcamsolo/
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyarcamsolo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:59:00.900209 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 17:59:00.000000 pyarcamsolo-0.1.2/pyarcamsolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:59:00.904209 pyarcamsolo-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 17:58:35.000000 pyarcamsolo-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:32:33.993342 pyarcamsolo-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 18:32:33.993342 pyarcamsolo-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:32:33.989342 pyarcamsolo-0.1.3/pyarcamsolo/
+-rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyarcamsolo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 18:32:33.989342 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 18:32:33.000000 pyarcamsolo-0.1.3/pyarcamsolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 18:32:33.993342 pyarcamsolo-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 18:32:10.000000 pyarcamsolo-0.1.3/setup.py
```

### Comparing `pyarcamsolo-0.1.2/LICENSE` & `pyarcamsolo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.2/PKG-INFO` & `pyarcamsolo-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.2/README.md` & `pyarcamsolo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.2/pyarcamsolo/__init__.py` & `pyarcamsolo-0.1.3/pyarcamsolo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     async def _responder_cancel(self):
         """Cancel any active responder task."""
         await cancel_task(self._responder_task, "responder")
         self._responder_task = None
 
     def _set_updated_values(self, value):
         """Set updated values from response parser."""
-        _LOGGER.debug(">> ArcamSolo._set_updated_values(value=%s)")
+        _LOGGER.debug(">> ArcamSolo._set_updated_values(value=%s)", value)
         if value["z"] not in self.zones:
             _LOGGER.debug("Zone does not yet exist so creating one.")
             self.zones[value["z"]] = {}
         self.zones[value["z"]][value["k"]] = value["v"]
         self._call_zone_callbacks(zone=value["z"])
 
     async def _connection_listener(self):
@@ -354,14 +354,15 @@
 
             await self._responder_cancel()
             await self._listener_schedule()
             await asyncio.sleep(0) # yield to listener task
             await self.discover_zones(self._enabled_zones) # discover zones
             await asyncio.sleep(2)
             await self._updater_schedule()
+            await asyncio.sleep(5) # allow initial queries to complete
 
         _LOGGER.debug(">> ArcamSolo.connect() completed")
 
     async def disconnect(self):
         """Shutdown and close telnet connection to Arcam."""
         _LOGGER.debug(">> ArcamSolo.disconnect() started")
 
@@ -537,17 +538,19 @@
     async def send_raw_command(self,
                                command: str,
                                data: list[bytes],
                                zone: int=1,
                                rate_limit=True):
         """Send a raw command to the Arcam."""
         _LOGGER.debug(
-            '>> ArcamSolo.send_raw_command("%s", rate_limit=%s)',
+            '>> ArcamSolo.send_raw_command(command=%s, rate_limit=%s, zone=%s, data=%s)',
             command,
             rate_limit,
+            zone,
+            data
         )
         if not self.available:
             raise RuntimeError("AVR connection not available")
 
         if rate_limit:
             # Rate limit commands
             command_delay = 0.1
@@ -572,14 +575,15 @@
         self._writer.write(raw_command)
         await self._writer.drain()
         self._last_command = time.time()
 
     async def send_ir_command(self,
                               command: str):
         """Send an IR command to the Arcam."""
+        _LOGGER.debug(">> ArcamSolo.send_ir_command(command=%s)", command)
         ir_data = IR_COMMAND_CODES.get(command, None)
         if ir_data is None:
             raise ValueError("Command does not exist.")
         await self.send_raw_command(
             command="virtual_remote",
             data=[
                 ir_data["system_code"].to_bytes(1, 'little'),
```

### Comparing `pyarcamsolo-0.1.2/pyarcamsolo/commands.py` & `pyarcamsolo-0.1.3/pyarcamsolo/commands.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.2/pyarcamsolo/parser.py` & `pyarcamsolo-0.1.3/pyarcamsolo/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     if ac not in ACCEPTED_ANSWER_CODES:
         if ac == "command_invalid_at_this_time":
             _LOGGER.warning("Command %s is unavailable in current state. Will retry later.", cc)
             return None
         raise ValueError(
             f"Provided response for {cc} is invalid at this time: {get_answer_code(ac)}"
         )
+    _LOGGER.debug(">> Decoded response as command %s", cc)
 
     if cc == "volume":
         output["k"] = cc
         output["v"] = data[0]
     elif cc == "mute":
         output["k"] = "muted"
         output["v"] = bool(data[0])
@@ -102,28 +103,52 @@
     elif cc == "cdusb_total_track_time":
         output["k"] = "current_track_duration"
         hour = int.from_bytes(data[0:1]) * 3600
         minute = int.from_bytes(data[1:2]) * 60
         sec = int.from_bytes(data[2:3])
         output["v"] = hour+minute+sec
     elif cc == "cd_play_mode":
+        binary = bin(int(data.hex(), 16))[2:]
+        if len(binary) == 4:
+            shuffle_value = int(binary[1])
+            repeat_value = binary[2:4]
+            program_value = int(binary[0])
+        elif len(binary) == 3:
+            shuffle_value = int(binary[0])
+            repeat_value = binary[1:3]
+            program_value = "0"
+        elif len(binary) == 2:
+            repeat_value = binary[0:1]
+            program_value = 0
+            shuffle_value = 0
+        else:
+            repeat_value = "0"
+            program_value = 0
+            shuffle_value = 0
+        # sort repeat value properly
+        if repeat_value == "0":
+            repeat_value = "off"
+        elif repeat_value == "1":
+            repeat_value = "single"
+        elif repeat_value == "11":
+            repeat_value = "all"
         return [
             {
                 "k": "repeat",
-                "v": None,
+                "v": repeat_value,
                 "z": output["z"]
             },
             {
                 "k": "shuffle",
-                "v": None,
+                "v": bool(shuffle_value),
                 "z": output["z"]
             },
             {
                 "k": "program",
-                "v": None,
+                "v": bool(program_value),
                 "z": output["z"]
             }
         ]
     elif cc == "cdusb_current_track":
         return parse_cdusb_current_track(
             z=output["z"],
             b=data
```

### Comparing `pyarcamsolo-0.1.2/pyarcamsolo/util.py` & `pyarcamsolo-0.1.3/pyarcamsolo/util.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.2/pyarcamsolo.egg-info/PKG-INFO` & `pyarcamsolo-0.1.3/pyarcamsolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.2/setup.py` & `pyarcamsolo-0.1.3/setup.py`

 * *Files identical despite different names*

