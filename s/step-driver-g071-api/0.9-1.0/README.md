# Comparing `tmp/step_driver_g071_api-0.9.tar.gz` & `tmp/step_driver_g071_api-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "step_driver_g071_api-0.9.tar", last modified: Tue Nov 14 14:25:02 2023, max compression
+gzip compressed data, was "step_driver_g071_api-1.0.tar", last modified: Mon May 27 12:39:59 2024, max compression
```

## Comparing `step_driver_g071_api-0.9.tar` & `step_driver_g071_api-1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:25:02.539277 step_driver_g071_api-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-14 14:24:52.000000 step_driver_g071_api-0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-14 14:25:02.539277 step_driver_g071_api-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 14:25:02.539277 step_driver_g071_api-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-11-14 14:24:52.000000 step_driver_g071_api-0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:25:02.535277 step_driver_g071_api-0.9/step_driver_g071_api/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-14 14:24:52.000000 step_driver_g071_api-0.9/step_driver_g071_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2023-11-14 14:24:52.000000 step_driver_g071_api-0.9/step_driver_g071_api/step_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:25:02.535277 step_driver_g071_api-0.9/step_driver_g071_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-14 14:25:02.000000 step_driver_g071_api-0.9/step_driver_g071_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-11-14 14:25:02.000000 step_driver_g071_api-0.9/step_driver_g071_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 14:25:02.000000 step_driver_g071_api-0.9/step_driver_g071_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-14 14:25:02.000000 step_driver_g071_api-0.9/step_driver_g071_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-14 14:25:02.000000 step_driver_g071_api-0.9/step_driver_g071_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 14:25:02.000000 step_driver_g071_api-0.9/step_driver_g071_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:39:59.223674 step_driver_g071_api-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 12:39:55.000000 step_driver_g071_api-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-27 12:39:59.223674 step_driver_g071_api-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:39:59.223674 step_driver_g071_api-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-27 12:39:55.000000 step_driver_g071_api-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:39:59.223674 step_driver_g071_api-1.0/step_driver_g071_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-27 12:39:55.000000 step_driver_g071_api-1.0/step_driver_g071_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-27 12:39:55.000000 step_driver_g071_api-1.0/step_driver_g071_api/step_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:39:59.223674 step_driver_g071_api-1.0/step_driver_g071_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-27 12:39:59.000000 step_driver_g071_api-1.0/step_driver_g071_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-27 12:39:59.000000 step_driver_g071_api-1.0/step_driver_g071_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:39:59.000000 step_driver_g071_api-1.0/step_driver_g071_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 12:39:59.000000 step_driver_g071_api-1.0/step_driver_g071_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 12:39:59.000000 step_driver_g071_api-1.0/step_driver_g071_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:39:59.000000 step_driver_g071_api-1.0/step_driver_g071_api.egg-info/zip-safe
```

### Comparing `step_driver_g071_api-0.9/LICENSE` & `step_driver_g071_api-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `step_driver_g071_api-0.9/PKG-INFO` & `step_driver_g071_api-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: step_driver_g071_api
-Version: 0.9
+Version: 1.0
 Summary: Stepper driver using MODBUS communication protocol API
 Home-page: https://github.com/gelio5/step_driver_G071_API.git
 Author: Vladislav Reznik
 Author-email: vlreznik97@gmail.com
 License: MIT
 Platform: Linux
 Platform: Win
```

### Comparing `step_driver_g071_api-0.9/setup.py` & `step_driver_g071_api-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     python setup.py install
 to install the package from the source archive.
 """
 from setuptools import setup
 
 setup(
     name='step_driver_g071_api',
-    version='0.9',
+    version='1.0',
     packages=['step_driver_g071_api'],
     url='https://github.com/gelio5/step_driver_G071_API.git',
     license='MIT',
     author='Vladislav Reznik',
     author_email='vlreznik97@gmail.com',
     description='Stepper driver using MODBUS communication protocol API',
     long_description='''
```

### Comparing `step_driver_g071_api-0.9/step_driver_g071_api/step_driver.py` & `step_driver_g071_api-1.0/step_driver_g071_api/step_driver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,50 @@
 """Stepper driver using MODBUS communication protocol"""
 import logging
+from functools import wraps
 from struct import unpack, pack
 from time import sleep
 
 from pymodbus.client import ModbusSerialClient
+from pymodbus.exceptions import ModbusException
+from serial.serialutil import SerialException
 
 _logger = logging.getLogger(__name__)
 
 
+def retry(
+        exception_to_check,
+        num_retries: int = 5,
+        sleep_time: float = 0.01,
+):
+    """Using for decorate multiple tries of function calling"""
+    def decorate(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            exception_to_raise_in_fall = BaseException
+            for i in range(1, num_retries + 1):
+                try:
+                    return func(*args, **kwargs)
+                except exception_to_check as received_exception:
+                    exception_to_raise_in_fall = received_exception
+                    print(
+                        f"{func.__name__} raised {received_exception.__class__.__name__}. \n "
+                        f"{received_exception} \n"
+                        f"Retrying..."
+                    )
+
+                    if i < num_retries:
+                        sleep(sleep_time)
+            raise exception_to_raise_in_fall
+
+        return wrapper
+
+    return decorate
+
+
 class StepDriver:
     """**StepDriver**.
 
     :param port: Serial port used for communication;
     :param modbus_address: MODBUS address used for communication;
     :param speed_to_search_home_pos: (optional) Number of steps per second used for search home;
 
@@ -48,17 +81,14 @@
         self._current_pos: int = 0
         self._status: bool = False
         self._address = modbus_address
         self._speed_to_search_home_pos = speed_to_search_home_pos
         self._max_position = max_pos
         self._encoder: int = 0
 
-    def _get_status(self) -> bool:
-        return self._status
-
     def search_home(self) -> None:
         """Search home position"""
         _logger.info('Searching home started')
         with self.device:
             self.device.write_registers(slave=self._address,
                                         address=0,
                                         values=[self._commands['INIT'], 0,
@@ -113,32 +143,41 @@
         with self.device:
             self.device.write_registers(slave=self._address,
                                         address=0,
                                         values=[self._commands['MOVE'], speed,
                                                 self._speed_to_search_home_pos,
                                                 *divmod(position, 0xFFFF)[::-1]])
 
+    @retry(exception_to_check=SerialException)
+    @retry(exception_to_check=ModbusException)
     def _update_info(self) -> None:
         """Update info about driver"""
         with self.device:
             received_data = self.device.read_holding_registers(slave=self._address,
                                                                count=3,
                                                                address=8).registers
         self._status = bool(received_data[0])
         self._current_pos = unpack('<I', pack('<HH', *received_data[1:]))[0]
 
+    @retry(exception_to_check=SerialException)
+    @retry(exception_to_check=Exception)
     def _update_encoder(self) -> None:
         """Update encoder value by register 13 READ, expected range [0 ... 4095]"""
         with self.device:
             self.device.write_registers(slave=self._address,
                                         address=0,
                                         values=[self._commands['UPDATE']])
         with self.device:
             received_data = self.device.read_holding_registers(slave=self._address,
                                                                count=1,
                                                                address=12).registers
         self._encoder = unpack('<I', pack('<H', *received_data[0]))[0]
 
-    def _get_encoder(self) -> int:
+    @property
+    def status(self):
+        """Getter for private status field"""
+        return self._status
+
+    @property
+    def encoder(self):
+        """Getter for private encoder field"""
         return self._encoder
-    status = property(fget=_get_status)
-    encoder = property(fget=_get_encoder)
```

### Comparing `step_driver_g071_api-0.9/step_driver_g071_api.egg-info/PKG-INFO` & `step_driver_g071_api-1.0/step_driver_g071_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: step-driver-g071-api
-Version: 0.9
+Name: step_driver_g071_api
+Version: 1.0
 Summary: Stepper driver using MODBUS communication protocol API
 Home-page: https://github.com/gelio5/step_driver_G071_API.git
 Author: Vladislav Reznik
 Author-email: vlreznik97@gmail.com
 License: MIT
 Platform: Linux
 Platform: Win
```

