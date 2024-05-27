# Comparing `tmp/createbme-1.2.1.tar.gz` & `tmp/createbme-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "createbme-1.2.1.tar", last modified: Thu May 23 12:50:38 2024, max compression
+gzip compressed data, was "createbme-1.2.2.tar", last modified: Mon May 27 11:59:26 2024, max compression
```

## Comparing `createbme-1.2.1.tar` & `createbme-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.293784 createbme-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 12:50:29.000000 createbme-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-23 12:50:38.293784 createbme-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-23 12:50:29.000000 createbme-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 12:50:29.000000 createbme-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:50:38.293784 createbme-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-23 12:50:29.000000 createbme-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.289784 createbme-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.293784 createbme-1.2.1/src/CreaTeBME/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/ImuSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/SensorEmulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/SensorManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 12:50:29.000000 createbme-1.2.1/src/CreaTeBME/uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:50:38.293784 createbme-1.2.1/src/CreaTeBME.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 12:50:38.000000 createbme-1.2.1/src/CreaTeBME.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:59:26.157943 createbme-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 11:59:21.000000 createbme-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-27 11:59:26.157943 createbme-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-27 11:59:21.000000 createbme-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-27 11:59:21.000000 createbme-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:59:26.157943 createbme-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-27 11:59:21.000000 createbme-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:59:26.157943 createbme-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:59:26.157943 createbme-1.2.2/src/CreaTeBME/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-27 11:59:21.000000 createbme-1.2.2/src/CreaTeBME/ImuSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-27 11:59:21.000000 createbme-1.2.2/src/CreaTeBME/SensorEmulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-27 11:59:21.000000 createbme-1.2.2/src/CreaTeBME/SensorManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-27 11:59:21.000000 createbme-1.2.2/src/CreaTeBME/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-27 11:59:21.000000 createbme-1.2.2/src/CreaTeBME/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-27 11:59:21.000000 createbme-1.2.2/src/CreaTeBME/uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:59:26.157943 createbme-1.2.2/src/CreaTeBME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-27 11:59:26.000000 createbme-1.2.2/src/CreaTeBME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 11:59:26.000000 createbme-1.2.2/src/CreaTeBME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:59:26.000000 createbme-1.2.2/src/CreaTeBME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 11:59:26.000000 createbme-1.2.2/src/CreaTeBME.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 11:59:26.000000 createbme-1.2.2/src/CreaTeBME.egg-info/top_level.txt
```

### Comparing `createbme-1.2.1/LICENSE` & `createbme-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `createbme-1.2.1/PKG-INFO` & `createbme-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CreaTeBME
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
 Author: Jonathan Matarazzi
 Author-email: git@jonathanm.nl
 Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `createbme-1.2.1/README.md` & `createbme-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `createbme-1.2.1/setup.py` & `createbme-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='CreaTeBME',
-    version='1.2.1',
+    version='1.2.2',
     author='Jonathan Matarazzi',
     author_email='git@jonathanm.nl',
     description='Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/CreaTe-M8-BME/CreaTeBME',
     project_urls={
```

### Comparing `createbme-1.2.1/src/CreaTeBME/ImuSensor.py` & `createbme-1.2.2/src/CreaTeBME/ImuSensor.py`

 * *Files identical despite different names*

### Comparing `createbme-1.2.1/src/CreaTeBME/SensorEmulator.py` & `createbme-1.2.2/src/CreaTeBME/SensorEmulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import json
 import copy
+import time
 import warnings
 from threading import Timer, Lock
 from typing import Callable, Dict, List
 
 
 class SensorEmulator:
     """
     An emulator for the SensorManager that reads from a recording file instead.
     """
-    def __init__(self, filename: str):
+    def __init__(self, filename: str, loop: bool = False):
         """
         Construct a SensorEmulator
 
         :param filename: The name of the recording file
+        :param loop: Whether to loop the recorded data when it finishes
         """
         with open(filename+'.tb', 'r') as f:
             text_content = f.read()
         text_data = json.loads(text_content)
         self._sample_rate: int = text_data['sample_rate']
-        self._data: Dict[str, List[float]] = text_data['data']
+        self._recorded_data: Dict[str, List[float]] = text_data['data']
+        self._data = copy.deepcopy(self._recorded_data)
+        self._loop = loop
         self._lock = Lock()
         self._timer = None
         self._queue = {name: [] for name in self._data.keys()}
         self._callback = None
         self._is_running = False
 
+        self._start_time = None
+        self._counter = 0
+
     def start(self) -> None:
         """
         Start the SensorEmulator
         """
         self._timer = Timer(1/self._sample_rate, self._step)
         self._timer.start()
         self._is_running = True
+        self._start_time = time.perf_counter()
+        self._counter = 0
 
     def stop(self) -> None:
         """
         Stop the SensorEmulator
         """
         self._timer.cancel()
         self._is_running = False
@@ -79,22 +88,26 @@
     def record(self) -> None:
         """
         Not implemented
         """
         warnings.warn(f"Emulating sensor, recording not supported.", RuntimeWarning)
 
     def _step(self):
-        self._timer = Timer(1/self._sample_rate, self._step)
+        self._counter += 1
+        self._timer = Timer((self._start_time + self._counter * 1 / self._sample_rate) - time.perf_counter(), self._step)
         self._timer.start()
         with self._lock:
             for name in self._data.keys():
 
                 if len(self._data[name]) < 1:
-                    self.stop()
-                    return
+                    if self._loop:
+                        self._data = copy.deepcopy(self._recorded_data)
+                    else:
+                        self.stop()
+                        return
 
                 data = self._data[name].pop()
                 self._queue[name].append(data)
                 if self._callback:
                     self._callback(name, data)
```

### Comparing `createbme-1.2.1/src/CreaTeBME/SensorManager.py` & `createbme-1.2.2/src/CreaTeBME/SensorManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,21 +35,24 @@
         self._loop.run_until_complete(self._create_sensors(sensor_names))
         for sensor in self._sensors:
             sensor.set_callback(self.__receive_reading)
 
     def start(self) -> None:
         """
         Start the SensorManager
+        Blocks until all sensors are sending data.
         :return:
         """
         if not self._loop.is_running():
             self._thread = Thread(target=self._run)
             self._thread.daemon = True
             self._thread.start()
         self._is_running = True
+        while any([len(self.get_measurements()[key]) == 0 for key in list(self._queue.keys())]):
+            pass
 
     def stop(self) -> None:
         """
         Stop the SensorManager
         :return:
         """
         if not self.is_running():
```

### Comparing `createbme-1.2.1/src/CreaTeBME/connect.py` & `createbme-1.2.2/src/CreaTeBME/connect.py`

 * *Files identical despite different names*

### Comparing `createbme-1.2.1/src/CreaTeBME.egg-info/PKG-INFO` & `createbme-1.2.2/src/CreaTeBME.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CreaTeBME
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
 Author: Jonathan Matarazzi
 Author-email: git@jonathanm.nl
 Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

