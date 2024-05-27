# Comparing `tmp/synthetic_home-2.2.0.tar.gz` & `tmp/synthetic_home-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthetic_home-2.2.0.tar", last modified: Sat May 25 22:13:51 2024, max compression
+gzip compressed data, was "synthetic_home-2.3.0.tar", last modified: Mon May 27 19:20:15 2024, max compression
```

## Comparing `synthetic_home-2.2.0.tar` & `synthetic_home-2.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:13:51.463018 synthetic_home-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-25 22:13:51.463018 synthetic_home-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-25 22:13:51.467018 synthetic_home-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:13:51.459018 synthetic_home-2.2.0/synthetic_home/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:13:51.463018 synthetic_home-2.2.0/synthetic_home/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/door-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/fan-oscilating.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/garage-door.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/gate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/heat-pump.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/hvac.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/light-dimmable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/light-rgbw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/light.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/motion-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/smart-blinds.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/smart-lock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/smart-plug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/smart-speaker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/switch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/temperature-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/todo-list.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/vacuum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/water-valve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/weather-service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/registry/window-sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/synthetic_home/synthetic_home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:13:51.463018 synthetic_home-2.2.0/synthetic_home.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-25 22:13:51.000000 synthetic_home-2.2.0/synthetic_home.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-25 22:13:51.000000 synthetic_home-2.2.0/synthetic_home.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:13:51.000000 synthetic_home-2.2.0/synthetic_home.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 22:13:51.000000 synthetic_home-2.2.0/synthetic_home.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 22:13:51.000000 synthetic_home-2.2.0/synthetic_home.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:13:51.463018 synthetic_home-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/tests/test_device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-25 22:13:47.000000 synthetic_home-2.2.0/tests/test_synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.039875 synthetic_home-2.3.0/synthetic_home/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.043875 synthetic_home-2.3.0/synthetic_home/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/door-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/fan-oscilating.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/garage-door.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/gate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/heat-pump.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/hvac.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/light-dimmable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/light-rgbw.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/light.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/motion-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-blinds.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-lock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-plug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/smart-speaker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/temperature-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/todo-list.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/vacuum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/water-valve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/weather-service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/registry/window-sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/synthetic_home/synthetic_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/synthetic_home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 19:20:15.000000 synthetic_home-2.3.0/synthetic_home.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:15.047875 synthetic_home-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-27 19:20:10.000000 synthetic_home-2.3.0/tests/test_synthetic_home.py
```

### Comparing `synthetic_home-2.2.0/LICENSE` & `synthetic_home-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/PKG-INFO` & `synthetic_home-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_home
-Version: 2.2.0
+Version: 2.3.0
 Summary: Library for managing synthetic home device registry
 Home-page: https://github.com/allenporter/synthetic-home
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synthetic_home-2.2.0/README.md` & `synthetic_home-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/pyproject.toml` & `synthetic_home-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/setup.cfg` & `synthetic_home-2.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = synthetic_home
-version = 2.2.0
+version = 2.3.0
 description = Library for managing synthetic home device registry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/synthetic-home
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `synthetic_home-2.2.0/synthetic_home/device_types.py` & `synthetic_home-2.3.0/synthetic_home/device_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Data model for home assistant synthetic home."""
 
+from functools import cache
 from collections.abc import Generator
 from dataclasses import dataclass, field
 from importlib import resources
 from importlib.resources.abc import Traversable
 import logging
 from typing import Any
 import yaml
@@ -285,15 +286,15 @@
         if device_type_file.name != f"{device_type.device_type}.yaml":
             raise SyntheticHomeError(
                 f"Device type '{device_type.device_type}' name does not match filename '{device_type_file.name}'"
             )
 
         yield device_type
 
-
+@cache
 def load_device_type_registry() -> DeviceTypeRegistry:
     """Load device types from the yaml configuration files."""
     device_types = {}
     for device_type in _read_device_types(DEVICE_TYPES_RESOURCE_PATH):
         if device_type.device_type in device_types:
             raise SyntheticHomeError(
                 f"Device registry contains duplicate device type '{device_type.device_type}"
```

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/README.md` & `synthetic_home-2.3.0/synthetic_home/registry/README.md`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/camera.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/camera.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/door-sensor.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/door-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/heat-pump.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/heat-pump.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/hvac.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/hvac.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/motion-sensor.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/motion-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/smart-blinds.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/smart-blinds.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/smart-lock.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/smart-lock.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/smart-speaker.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/smart-speaker.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,14 @@
     media_player.speaker: paused
 entities:
   media_player:
     speaker:
       device_class: media_player.MediaPlayerDeviceClass.SPEAKER
       supported_features:
         - media_player.MediaPlayerEntityFeature.PLAY
+        - media_player.MediaPlayerEntityFeature.PAUSE
         - media_player.MediaPlayerEntityFeature.STOP
         - media_player.MediaPlayerEntityFeature.VOLUME_STEP
         - media_player.MediaPlayerEntityFeature.VOLUME_MUTE
         - media_player.MediaPlayerEntityFeature.VOLUME_SET
         - media_player.MediaPlayerEntityFeature.TURN_ON
         - media_player.MediaPlayerEntityFeature.TURN_OFF
```

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/temperature-sensor.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/temperature-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/vacuum.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/vacuum.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/water-valve.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/water-valve.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     valve.water-valve: open
     sensor.meter-reading: 2001
     sensor.battery: 75
 entities:
   valve:
     water-valve:
       supported_features:
-        - fan.FanEntityFeature.OSCILLATE
-        - fan.FanEntityFeature.SET_SPEED
+        - valve.ValveEntityFeature.OPEN
+        - valve.ValveEntityFeature.CLOSE
+        - valve.ValveEntityFeature.SET_POSITION
   sensor:
     meter-reading:
       native_unit_of_measurement: m³
       device_class: sensor.SensorDeviceClass.WATER
       state_class: sensor.SensorStateClass.TOTAL_INCREASING
     battery:
       device_class: sensor.SensorDeviceClass.BATTERY
```

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/weather-service.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/weather-service.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/registry/window-sensor.yaml` & `synthetic_home-2.3.0/synthetic_home/registry/window-sensor.yaml`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home/synthetic_home.py` & `synthetic_home-2.3.0/synthetic_home/synthetic_home.py`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/synthetic_home.egg-info/PKG-INFO` & `synthetic_home-2.3.0/synthetic_home.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthetic_home
-Version: 2.2.0
+Version: 2.3.0
 Summary: Library for managing synthetic home device registry
 Home-page: https://github.com/allenporter/synthetic-home
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `synthetic_home-2.2.0/synthetic_home.egg-info/SOURCES.txt` & `synthetic_home-2.3.0/synthetic_home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/tests/test_device_types.py` & `synthetic_home-2.3.0/tests/test_device_types.py`

 * *Files identical despite different names*

### Comparing `synthetic_home-2.2.0/tests/test_synthetic_home.py` & `synthetic_home-2.3.0/tests/test_synthetic_home.py`

 * *Files identical despite different names*

