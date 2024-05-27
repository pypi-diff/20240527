# Comparing `tmp/pyarcamsolo-0.0.6.tar.gz` & `tmp/pyarcamsolo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcamsolo-0.0.6.tar", last modified: Sun May 26 18:19:46 2024, max compression
+gzip compressed data, was "pyarcamsolo-0.1.0.tar", last modified: Mon May 27 16:13:47 2024, max compression
```

## Comparing `pyarcamsolo-0.0.6.tar` & `pyarcamsolo-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/pyarcamsolo/
--rw-r--r--   0 runner    (1001) docker     (127)    22522 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:13:47.156689 pyarcamsolo-0.1.0/pyarcamsolo/
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyarcamsolo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 16:13:47.000000 pyarcamsolo-0.1.0/pyarcamsolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:13:47.160689 pyarcamsolo-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 16:13:22.000000 pyarcamsolo-0.1.0/setup.py
```

### Comparing `pyarcamsolo-0.0.6/LICENSE` & `pyarcamsolo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.6/PKG-INFO` & `pyarcamsolo-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.0.6
+Version: 0.1.0
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.0.6/README.md` & `pyarcamsolo-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.6/pyarcamsolo/__init__.py` & `pyarcamsolo-0.1.0/pyarcamsolo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,34 @@
 
 from .commands import (
     ARCAM_COMM_END,
     ARCAM_COMM_START,
     COMMAND_CODES,
     IR_COMMAND_CODES,
     SOURCE_IR_CONTROL_MAP,
-    ARCAM_QUERY_COMMANDS
+    ARCAM_QUERY_COMMANDS,
+    RADIO_QUERY_COMMANDS
 )
 from .util import sock_set_keepalive, cancel_task, get_backoff_delay, safe_wait_for
 from .parser import parse_response
+from .params import CONF_ENABLED_ZONES
 from ._version import __version__ as VERSION
 
 _LOGGER = logging.getLogger(__name__)
 
 class ArcamSolo:
     """Base Arcam Solo module."""
 
     def __init__(
         self,
         host,
         port,
         timeout=2,
         scan_interval=60,
-        params=None):
+        params: dict | None=None):
         """Initialise the Arcam Solo interface."""
         _LOGGER.info("Starting pyarcamsolo %s", VERSION)
         _LOGGER.debug(
             '>> ArcamSolo.__init__(host="%s", port="%s", timeout="%s", params="%s")',
             host,
             port,
             timeout,
@@ -80,14 +82,19 @@
         self._reconnect_task = None
         self._updater_task = None
         self._command_queue_task = None
         self._initial_query = True
         # Stores a list of commands to run after receiving an event
         self._command_queue = []
 
+        # Handle configuration
+        self._enabled_zones = [1] # Zone 2 is optional
+        if params is not None:
+            self._enabled_zones = params.get(CONF_ENABLED_ZONES, [1]) # Zone 2 is optional
+
     def __del__(self):
         _LOGGER.debug(">> ArcamSolo.__del__()")
 
     def _set_socket_options(self):
         """Set socket keepalive options."""
         sock_set_keepalive(
             self._writer.get_extra_info("socket"),
@@ -137,16 +144,17 @@
     async def _responder_cancel(self):
         """Cancel any active responder task."""
         await cancel_task(self._responder_task, "responder")
         self._responder_task = None
 
     def _set_updated_values(self, value):
         """Set updated values from response parser."""
-        _LOGGER.debug("parsed response %s", value)
+        _LOGGER.debug(">> ArcamSolo._set_updated_values(value=%s)")
         if value["z"] not in self.zones:
+            _LOGGER.debug("Zone does not yet exist so creating one.")
             self.zones[value["z"]] = {}
         self.zones[value["z"]][value["k"]] = value["v"]
         self._call_zone_callbacks(zone=value["z"])
 
     async def _connection_listener(self):
         """Arcam connection listener. Parse responses and update state."""
         _LOGGER.debug(">> ArcamSolo._connection_listener() started")
@@ -170,15 +178,15 @@
                     _LOGGER.debug("received Arcam response: %s", response.hex())
                     action = " parsing response " + response.hex()
                     value = parse_response(response)
                     if isinstance(value, list):
                         for parsed in value:
                             self._set_updated_values(parsed)
                     elif isinstance(value, dict):
-                        self._set_updated_values(value)    
+                        self._set_updated_values(value)
                 else:
                     _LOGGER.debug("Ignoring response %s due to invalid data.", response.hex())
             except asyncio.CancelledError:
                 _LOGGER.debug((">> ArcamSolo._connection_listener() cancelled"))
                 running = False
                 break
             except Exception as exc:
@@ -262,14 +270,15 @@
                             datetime.now().hour.to_bytes(1, 'little'),
                             datetime.now().minute.to_bytes(1, 'little'),
                             datetime.now().second.to_bytes(1, 'little')
                         ]
                     )
                     for zone in self.zones:
                         await self._update_zone(zone)
+                    await self._update_radio_data()
                 except Exception as exc: #pylint: disable=broad-except
                     _LOGGER.error(
                         "could not update Arcam status: %s: %s",
                         type(exc).__name__,
                         str(exc)
                     )
                     _rc = False
@@ -285,14 +294,33 @@
         for query in ARCAM_QUERY_COMMANDS:
             await self.send_raw_command(
                 command=query,
                 data=[b'\xF0'],
                 zone=zone
             )
 
+    async def _update_radio_data(self):
+        """Update radio status information."""
+        _LOGGER.debug(">> ArcamSolo._update_radio_data()")
+        if self.source in ["AM", "FM", "DAB"]:
+            for k, v in RADIO_QUERY_COMMANDS.items():
+                if (k=="request_station_frequency"
+                    and self.source not in ["AM", "FM"]):
+                    continue
+                if (k=="request_mpeg_mode" and self.source != "DAB"):
+                    continue
+                if (k=="request_data_rate" and self.source != "DAB"):
+                    continue
+                await self.send_raw_command(
+                    command="radio_station_info",
+                    data=[b'\xF0', v],
+                    zone=1
+                )
+
+
     async def _updater_schedule(self):
         """Schedule/reschedule the updater task."""
         if self.scan_interval:
             _LOGGER.debug(">> ArcamSolo._updater_schedule()")
             await self._updater_cancel()
             self._full_update = True # always perform a full update on schedule
             self._updater_task = asyncio.create_task(self._updater())
@@ -323,15 +351,15 @@
             self.available = True
             self._reconnect = reconnect
             self._set_socket_options()
 
             await self._responder_cancel()
             await self._listener_schedule()
             await asyncio.sleep(0) # yield to listener task
-            await self.discover_zones([1, 2]) # discover zone 1 and 2
+            await self.discover_zones(self._enabled_zones) # discover zones
             await asyncio.sleep(2)
             await self._updater_schedule()
 
         _LOGGER.debug(">> ArcamSolo.connect() completed")
 
     async def disconnect(self):
         """Shutdown and close telnet connection to Arcam."""
@@ -601,7 +629,14 @@
         # send the command twice as sometimes the device doesn't respond
         await self.send_ir_command(
             command="standby_off"
         )
         await self.send_ir_command(
             command="standby_off"
         )
+
+    @property
+    def source(self) -> str | None:
+        """Return the current input source."""
+        if 1 not in self.zones:
+            return None
+        return self.zones.get(1).get("source", None)
```

### Comparing `pyarcamsolo-0.0.6/pyarcamsolo/commands.py` & `pyarcamsolo-0.1.0/pyarcamsolo/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,26 @@
     "cdusb_current_track": b'\xE8',
     "usb_track_name": b'\x60',
     "usb_folder_name": b'\x61',
     "cdusb_playback_time": b'\xEB',
     "cd_disc_type": b'\xED',
     "time": b'\xF8',
     "rs232_version": b'\xF1',
-    "software_version": b'\xF2'
+    "software_version": b'\xF2',
 }
 
 ARCAM_QUERY_COMMANDS = list(COMMAND_CODES.keys())
 
+RADIO_QUERY_COMMANDS = {
+    "request_station_frequency": b'\x00', # fm/am
+    "request_station_signal": b'\x01', # all
+    "request_mpeg_mode": b'\x02', # dab only
+    "request_data_rate": b'\x03' # dab only
+}
+
 ACCEPTED_ANSWER_CODES = ["status_update", "command_accepted_completed"]
 ANSWER_CODES = {
     "status_update": b'\x00',
     "command_accepted_completed": b'\x01',
     "command_accepted_processing": b'\x02',
     "zone_invalid": b'\x82',
     "command_not_recognised": b'\x83',
@@ -128,14 +135,21 @@
     b'\x08': "No Device",
     b'\x09': "Paused",
     b'\x10': "Invalid File",
     b'\x11': "No Valid Files Present",
     b'\x0D': "Track Skipping"
 }
 
+RADIO_MPEG_MODES = {
+    b'\x00': "Stereo",
+    b'\x01': "Joint Stereo",
+    b'\x02': "Dual Mono",
+    b'\x03': "Mono"
+}
+
 IR_COMMAND_CODES = {
     "src_tv": {
         "system_code": 16,
         "command_code": 0
     },
     "src_av": {
         "system_code": 16,
```

### Comparing `pyarcamsolo-0.0.6/pyarcamsolo/util.py` & `pyarcamsolo-0.1.0/pyarcamsolo/util.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.6/pyarcamsolo.egg-info/PKG-INFO` & `pyarcamsolo-0.1.0/pyarcamsolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.0.6
+Version: 0.1.0
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.0.6/setup.py` & `pyarcamsolo-0.1.0/setup.py`

 * *Files identical despite different names*

