# Comparing `tmp/pyheos-0.7.3.tar.gz` & `tmp/pyheos-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheos-0.7.3.tar", last modified: Sun May 26 14:32:56 2024, max compression
+gzip compressed data, was "pyheos-0.7.4.tar", last modified: Mon May 27 15:34:01 2024, max compression
```

## Comparing `pyheos-0.7.3.tar` & `pyheos-0.7.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.459844 pyheos-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-26 14:32:43.000000 pyheos-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-26 14:32:56.459844 pyheos-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-26 14:32:43.000000 pyheos-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.455844 pyheos-0.7.3/pyheos/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/heos.py
--rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/player.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.459844 pyheos-0.7.3/pyheos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:32:56.459844 pyheos-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-26 14:32:43.000000 pyheos-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.455844 pyheos-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    30212 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_heos.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:01.160098 pyheos-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-27 15:33:43.000000 pyheos-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-27 15:34:01.160098 pyheos-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-27 15:33:43.000000 pyheos-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:01.156098 pyheos-0.7.4/pyheos/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/heos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyheos/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:01.160098 pyheos-0.7.4/pyheos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-27 15:34:01.000000 pyheos-0.7.4/pyheos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 15:34:01.000000 pyheos-0.7.4/pyheos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:34:01.000000 pyheos-0.7.4/pyheos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:34:00.000000 pyheos-0.7.4/pyheos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 15:34:01.000000 pyheos-0.7.4/pyheos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 15:33:43.000000 pyheos-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:34:01.160098 pyheos-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:01.160098 pyheos-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-27 15:33:43.000000 pyheos-0.7.4/tests/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-27 15:33:43.000000 pyheos-0.7.4/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30212 2024-05-27 15:33:43.000000 pyheos-0.7.4/tests/test_heos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-27 15:33:43.000000 pyheos-0.7.4/tests/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-27 15:33:43.000000 pyheos-0.7.4/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-27 15:33:43.000000 pyheos-0.7.4/tests/test_source.py
```

### Comparing `pyheos-0.7.3/LICENSE` & `pyheos-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/PKG-INFO` & `pyheos-0.7.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyheos
-Version: 0.7.3
+Version: 0.7.4
 Summary: An async python library for controlling HEOS devices through the HEOS CLI Protocol
-Home-page: https://github.com/andrewsayre/pyheos
-Author: Andrew Sayre
-Author-email: andrew@sayre.net
+Author-email: Andrew Sayre <andrew@sayre.net>
 License: ASL 2.0
-Keywords: heos
+Project-URL: Source Code, https://github.com/andrewsayre/pyheo
+Keywords: heos,dennon,maranz
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyheos
 [![CI Status](https://github.com/andrewsayre/pyheos/workflows/CI/badge.svg)](https://github.com/andrewsayre/pyheos/actions)
 [![codecov](https://codecov.io/github/andrewsayre/pyheos/graph/badge.svg?token=PV4P3AN7Z1)](https://codecov.io/github/andrewsayre/pyheos)
 [![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
 
-An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
+An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.17 for players with firmware 2.41.140 or newer).
 
 ## Installation
 ```bash
 pip install pyheos
 ```
 or
 ```bash
```

### Comparing `pyheos-0.7.3/README.md` & `pyheos-0.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyheos
 [![CI Status](https://github.com/andrewsayre/pyheos/workflows/CI/badge.svg)](https://github.com/andrewsayre/pyheos/actions)
 [![codecov](https://codecov.io/github/andrewsayre/pyheos/graph/badge.svg?token=PV4P3AN7Z1)](https://codecov.io/github/andrewsayre/pyheos)
 [![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
 
-An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
+An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.17 for players with firmware 2.41.140 or newer).
 
 ## Installation
 ```bash
 pip install pyheos
 ```
 or
 ```bash
```

### Comparing `pyheos-0.7.3/pyheos/__init__.py` & `pyheos-0.7.4/pyheos/__init__.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/pyheos/command.py` & `pyheos-0.7.4/pyheos/command.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/pyheos/connection.py` & `pyheos-0.7.4/pyheos/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define the connection module."""
 
 import asyncio
-from collections import defaultdict
-from datetime import datetime, timedelta
 import json
 import logging
+from collections import defaultdict
+from datetime import datetime, timedelta
 from typing import Any, Dict, Optional
 
 from . import const
 from .command import HeosCommands
 from .error import CommandError, HeosError, format_error_message
 from .response import HeosResponse
 
@@ -61,17 +61,15 @@
         self._all_progress_events = all_progress_events
         self.host = host  # type: str
         self.commands = HeosCommands(self)
         self.timeout = timeout  # type: int
         self._reader = None  # type: asyncio.StreamReader
         self._writer = None  # type: asyncio.StreamWriter
         self._response_handler_task = None  # type: asyncio.Task
-        self._pending_commands = defaultdict(
-            list
-        )  # type: DefaultDict[str, List[ResponseEvent]]
+        self._pending_commands = defaultdict(list)  # type: DefaultDict[str, List[ResponseEvent]]
         self._sequence = 0  # type: int
         self._state = const.STATE_DISCONNECTED  # type: str
         self._auto_reconnect = False  # type: bool
         self._reconnect_delay = const.DEFAULT_RECONNECT_DELAY  # type: float
         self._reconnect_task = None  # type: asyncio.Task
         self._last_activity = None  # type: datetime
         self._heart_beat_interval = heart_beat  # type: Optional[float]
```

### Comparing `pyheos-0.7.3/pyheos/const.py` & `pyheos-0.7.4/pyheos/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 """Define consts for the pyheos package."""
 
-__title__ = "pyheos"
-__version__ = "0.7.3"
-
 CLI_PORT = 1255
 DEFAULT_TIMEOUT = 10.0
 DEFAULT_RECONNECT_DELAY = 10.0
 DEFAULT_HEART_BEAT = 10.0
 DEFAULT_STEP = 5
 
 STATE_CONNECTED = "connected"
@@ -97,94 +94,102 @@
     MUSIC_SOURCE_TIDAL: {TYPE_SONG: CONTROLS_ALL},
     MUSIC_SOURCE_AMAZON: {TYPE_SONG: CONTROLS_ALL, TYPE_STATION: CONTROLS_ALL},
     MUSIC_SOURCE_AUX_INPUT: {TYPE_STATION: CONTROL_PLAY_STOP},
 }
 
 
 # Inputs
+INPUT_ANALOG_IN_1 = "inputs/analog_in_1"
+INPUT_ANALOG_IN_2 = "inputs/analog_in_2"
+INPUT_AUX_8K = "inputs/aux_8k"
 INPUT_AUX_IN_1 = "inputs/aux_in_1"
 INPUT_AUX_IN_2 = "inputs/aux_in_2"
 INPUT_AUX_IN_3 = "inputs/aux_in_3"
 INPUT_AUX_IN_4 = "inputs/aux_in_4"
 INPUT_AUX_IN_SINGLE = "inputs/aux_single"
 INPUT_AUX1 = "inputs/aux1"
 INPUT_AUX2 = "inputs/aux2"
 INPUT_AUX3 = "inputs/aux3"
 INPUT_AUX4 = "inputs/aux4"
 INPUT_AUX5 = "inputs/aux5"
 INPUT_AUX6 = "inputs/aux6"
 INPUT_AUX7 = "inputs/aux7"
-INPUT_LINE_IN_1 = "inputs/line_in_1"
-INPUT_LINE_IN_2 = "inputs/line_in_2"
-INPUT_LINE_IN_3 = "inputs/line_in_3"
-INPUT_LINE_IN_4 = "inputs/line_in_4"
+INPUT_BLURAY = "inputs/bluray"
+INPUT_CABLE_SAT = "inputs/cable_sat"
+INPUT_CD = "inputs/cd"
 INPUT_COAX_IN_1 = "inputs/coax_in_1"
 INPUT_COAX_IN_2 = "inputs/coax_in_2"
-INPUT_OPTICAL_IN_1 = "inputs/optical_in_1"
-INPUT_OPTICAL_IN_2 = "inputs/optical_in_2"
+INPUT_DVD = "inputs/dvd"
+INPUT_GAME = "inputs/game"
+INPUT_GAME_2 = "inputs/game2"
+INPUT_HD_RADIO = "inputs/hdradio"
+INPUT_HDMI_ARC_1 = "inputs/hdmi_arc_1"
 INPUT_HDMI_IN_1 = "inputs/hdmi_in_1"
 INPUT_HDMI_IN_2 = "inputs/hdmi_in_2"
 INPUT_HDMI_IN_3 = "inputs/hdmi_in_3"
 INPUT_HDMI_IN_4 = "inputs/hdmi_in_4"
-INPUT_HDMI_ARC_1 = "inputs/hdmi_arc_1"
-INPUT_CABLE_SAT = "inputs/cable_sat"
-INPUT_DVD = "inputs/dvd"
-INPUT_BLURAY = "inputs/bluray"
-INPUT_GAME = "inputs/game"
+INPUT_LINE_IN_1 = "inputs/line_in_1"
+INPUT_LINE_IN_2 = "inputs/line_in_2"
+INPUT_LINE_IN_3 = "inputs/line_in_3"
+INPUT_LINE_IN_4 = "inputs/line_in_4"
 INPUT_MEDIA_PLAYER = "inputs/mediaplayer"
-INPUT_CD = "inputs/cd"
+INPUT_OPTICAL_IN_1 = "inputs/optical_in_1"
+INPUT_OPTICAL_IN_2 = "inputs/optical_in_2"
+INPUT_OPTICAL_IN_3 = "inputs/optical_in_3"
+INPUT_PHONO = "inputs/phono"
+INPUT_RECORDER_IN_1 = "inputs/recorder_in_1"
 INPUT_TUNER = "inputs/tuner"
-INPUT_HD_RADIO = "inputs/hdradio"
+INPUT_TV = "inputs/tv"
 INPUT_TV_AUDIO = "inputs/tvaudio"
-INPUT_PHONO = "inputs/phono"
 INPUT_USB_AC = "inputs/usbdac"
-INPUT_ANALOG_IN_1 = "inputs/analog_in_1"
-INPUT_ANALOG_IN_2 = "inputs/analog_in_2"
-INPUT_RECORDER_IN_1 = "inputs/recorder_in_1"
 
 VALID_INPUTS = (
+    INPUT_ANALOG_IN_1,
+    INPUT_ANALOG_IN_2,
+    INPUT_AUX_8K,
     INPUT_AUX_IN_1,
     INPUT_AUX_IN_2,
     INPUT_AUX_IN_3,
     INPUT_AUX_IN_4,
     INPUT_AUX_IN_SINGLE,
     INPUT_AUX1,
     INPUT_AUX2,
     INPUT_AUX3,
     INPUT_AUX4,
     INPUT_AUX5,
     INPUT_AUX6,
     INPUT_AUX7,
-    INPUT_LINE_IN_1,
-    INPUT_LINE_IN_2,
-    INPUT_LINE_IN_3,
-    INPUT_LINE_IN_4,
+    INPUT_BLURAY,
+    INPUT_CABLE_SAT,
+    INPUT_CD,
     INPUT_COAX_IN_1,
     INPUT_COAX_IN_2,
-    INPUT_OPTICAL_IN_1,
-    INPUT_OPTICAL_IN_2,
+    INPUT_DVD,
+    INPUT_GAME_2,
+    INPUT_GAME,
+    INPUT_HD_RADIO,
+    INPUT_HDMI_ARC_1,
     INPUT_HDMI_IN_1,
     INPUT_HDMI_IN_2,
     INPUT_HDMI_IN_3,
     INPUT_HDMI_IN_4,
-    INPUT_HDMI_ARC_1,
-    INPUT_CABLE_SAT,
-    INPUT_DVD,
-    INPUT_BLURAY,
-    INPUT_GAME,
+    INPUT_LINE_IN_1,
+    INPUT_LINE_IN_2,
+    INPUT_LINE_IN_3,
+    INPUT_LINE_IN_4,
     INPUT_MEDIA_PLAYER,
-    INPUT_CD,
+    INPUT_OPTICAL_IN_1,
+    INPUT_OPTICAL_IN_2,
+    INPUT_OPTICAL_IN_3,
+    INPUT_PHONO,
+    INPUT_RECORDER_IN_1,
     INPUT_TUNER,
-    INPUT_HD_RADIO,
     INPUT_TV_AUDIO,
-    INPUT_PHONO,
+    INPUT_TV,
     INPUT_USB_AC,
-    INPUT_ANALOG_IN_1,
-    INPUT_ANALOG_IN_2,
-    INPUT_RECORDER_IN_1,
 )
 
 # Add to Queue Options
 ADD_QUEUE_PLAY_NOW = 1
 ADD_QUEUE_PLAY_NEXT = 2
 ADD_QUEUE_ADD_TO_END = 3
 ADD_QUEUE_REPLACE_AND_PLAY = 4
```

### Comparing `pyheos-0.7.3/pyheos/dispatch.py` & `pyheos-0.7.4/pyheos/dispatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Defines the dispatch component for notifying others of signals."""
 
 import asyncio
-from collections import defaultdict
 import functools
+from collections import defaultdict
 from typing import Any, Callable, Dict, List, Sequence
 
 TargetType = Callable[..., Any]
 DisconnectType = Callable[[], None]
 ConnectType = Callable[[str, TargetType], DisconnectType]
 SendType = Callable[..., Sequence[asyncio.Future]]
 
@@ -16,15 +16,15 @@
 
     def __init__(
         self,
         *,
         connect: ConnectType = None,
         send: SendType = None,
         signal_prefix: str = "",
-        loop=None
+        loop=None,
     ):
         """Create a new instance of the dispatch component."""
         self._signal_prefix = signal_prefix
         self._signals = defaultdict(list)
         self._loop = loop or asyncio.get_event_loop()
         self._connect = connect or self._default_connect
         self._send = send or self._default_send
```

### Comparing `pyheos-0.7.3/pyheos/error.py` & `pyheos-0.7.4/pyheos/error.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/pyheos/group.py` & `pyheos-0.7.4/pyheos/group.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/pyheos/heos.py` & `pyheos-0.7.4/pyheos/heos.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(
         self,
         host: str,
         *,
         timeout: float = const.DEFAULT_TIMEOUT,
         heart_beat: Optional[float] = const.DEFAULT_HEART_BEAT,
         all_progress_events=True,
-        dispatcher: Dispatcher = None
+        dispatcher: Dispatcher = None,
     ):
         """Init a new instance of the Heos CLI API."""
         self._connection = HeosConnection(
             self,
             host,
             timeout=timeout,
             heart_beat=heart_beat,
@@ -41,15 +41,15 @@
         self._groups = {}  # type: Dict[int, HeosGroup]
         self._groups_loaded = False
 
     async def connect(
         self,
         *,
         auto_reconnect=False,
-        reconnect_delay: float = const.DEFAULT_RECONNECT_DELAY
+        reconnect_delay: float = const.DEFAULT_RECONNECT_DELAY,
     ):
         """Connect to the CLI."""
         await self._connection.connect(
             auto_reconnect=auto_reconnect, reconnect_delay=reconnect_delay
         )
         self._signed_in_username = await self._connection.commands.check_account()
```

### Comparing `pyheos-0.7.3/pyheos/player.py` & `pyheos-0.7.4/pyheos/player.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/pyheos/response.py` & `pyheos-0.7.4/pyheos/response.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/pyheos/source.py` & `pyheos-0.7.4/pyheos/source.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/pyheos.egg-info/PKG-INFO` & `pyheos-0.7.4/pyheos.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyheos
-Version: 0.7.3
+Version: 0.7.4
 Summary: An async python library for controlling HEOS devices through the HEOS CLI Protocol
-Home-page: https://github.com/andrewsayre/pyheos
-Author: Andrew Sayre
-Author-email: andrew@sayre.net
+Author-email: Andrew Sayre <andrew@sayre.net>
 License: ASL 2.0
-Keywords: heos
+Project-URL: Source Code, https://github.com/andrewsayre/pyheo
+Keywords: heos,dennon,maranz
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyheos
 [![CI Status](https://github.com/andrewsayre/pyheos/workflows/CI/badge.svg)](https://github.com/andrewsayre/pyheos/actions)
 [![codecov](https://codecov.io/github/andrewsayre/pyheos/graph/badge.svg?token=PV4P3AN7Z1)](https://codecov.io/github/andrewsayre/pyheos)
 [![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
 
-An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
+An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.17 for players with firmware 2.41.140 or newer).
 
 ## Installation
 ```bash
 pip install pyheos
 ```
 or
 ```bash
```

### Comparing `pyheos-0.7.3/tests/test_dispatch.py` & `pyheos-0.7.4/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/tests/test_group.py` & `pyheos-0.7.4/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/tests/test_heos.py` & `pyheos-0.7.4/tests/test_heos.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/tests/test_player.py` & `pyheos-0.7.4/tests/test_player.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.3/tests/test_source.py` & `pyheos-0.7.4/tests/test_source.py`

 * *Files identical despite different names*

