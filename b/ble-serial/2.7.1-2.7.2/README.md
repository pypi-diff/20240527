# Comparing `tmp/ble-serial-2.7.1.tar.gz` & `tmp/ble_serial-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ble-serial-2.7.1.tar", last modified: Sat May 13 21:49:21 2023, max compression
+gzip compressed data, was "ble_serial-2.7.2.tar", last modified: Mon May 27 13:33:43 2024, max compression
```

## Comparing `ble-serial-2.7.1.tar` & `ble_serial-2.7.2.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.882350 ble-serial-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-13 21:49:12.000000 ble-serial-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-13 21:49:12.000000 ble-serial-2.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-05-13 21:49:21.878350 ble-serial-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24350 2023-05-13 21:49:12.000000 ble-serial-2.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.878350 ble-serial-2.7.1/ble_serial/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.878350 ble-serial-2.7.1/ble_serial/bluetooth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/bluetooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/bluetooth/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/bluetooth/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.878350 ble-serial-2.7.1/ble_serial/log/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/log/console_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/log/fs_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.878350 ble-serial-2.7.1/ble_serial/ports/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/ports/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/ports/linux_pty.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/ports/print_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/ports/tcp_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/ports/windows_com0com.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.878350 ble-serial-2.7.1/ble_serial/scan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/scan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/scan/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.878350 ble-serial-2.7.1/ble_serial/setup_com0com/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/setup_com0com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/setup_com0com/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-13 21:49:12.000000 ble-serial-2.7.1/ble_serial/setup_com0com/windows_priv_setupc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:49:21.878350 ble-serial-2.7.1/ble_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-05-13 21:49:21.000000 ble-serial-2.7.1/ble_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-13 21:49:21.000000 ble-serial-2.7.1/ble_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 21:49:21.000000 ble-serial-2.7.1/ble_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-13 21:49:21.000000 ble-serial-2.7.1/ble_serial.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-13 21:49:21.000000 ble-serial-2.7.1/ble_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-13 21:49:21.000000 ble-serial-2.7.1/ble_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-13 21:49:12.000000 ble-serial-2.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 21:49:21.882350 ble-serial-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-13 21:49:12.000000 ble-serial-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.576514 ble_serial-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 13:33:35.000000 ble_serial-2.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 13:33:35.000000 ble_serial-2.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-27 13:33:43.576514 ble_serial-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24431 2024-05-27 13:33:35.000000 ble_serial-2.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.572514 ble_serial-2.7.2/ble_serial/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.572514 ble_serial-2.7.2/ble_serial/bluetooth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/bluetooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/bluetooth/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/bluetooth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.572514 ble_serial-2.7.2/ble_serial/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/log/console_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/log/fs_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.576514 ble_serial-2.7.2/ble_serial/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/ports/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/ports/linux_pty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/ports/print_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/ports/tcp_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/ports/windows_com0com.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.576514 ble_serial-2.7.2/ble_serial/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/scan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/scan/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.576514 ble_serial-2.7.2/ble_serial/setup_com0com/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/setup_com0com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/setup_com0com/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-27 13:33:35.000000 ble_serial-2.7.2/ble_serial/setup_com0com/windows_priv_setupc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.576514 ble_serial-2.7.2/ble_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25542 2024-05-27 13:33:43.000000 ble_serial-2.7.2/ble_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 13:33:43.000000 ble_serial-2.7.2/ble_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:33:43.000000 ble_serial-2.7.2/ble_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-27 13:33:43.000000 ble_serial-2.7.2/ble_serial.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 13:33:43.000000 ble_serial-2.7.2/ble_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 13:33:43.000000 ble_serial-2.7.2/ble_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 13:33:35.000000 ble_serial-2.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:33:43.576514 ble_serial-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-27 13:33:35.000000 ble_serial-2.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:33:43.576514 ble_serial-2.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-27 13:33:35.000000 ble_serial-2.7.2/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-27 13:33:35.000000 ble_serial-2.7.2/tests/test_conn_reliability.py
```

### Comparing `ble-serial-2.7.1/LICENSE` & `ble_serial-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ble-serial-2.7.1/PKG-INFO` & `ble_serial-2.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: ble-serial
-Version: 2.7.1
-Summary: A package to connect BLE serial adapters
+Version: 2.7.2
+Summary: Connects BLE adapters with virtual serial ports
 Home-page: https://github.com/Jakeler/ble-serial
 Author: Jake
 Author-email: ble-serial-pypi@ja-ke.tech
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: bleak>=0.20.0
+Requires-Dist: coloredlogs>=15.0
+Requires-Dist: pyserial>=3.4.0; platform_system == "Windows"
 
 # BLE Serial
 A tool to connect Bluetooth 4.0+ Low Energy to UART modules and normal PCs/laptops/RaspberryPi.
 
 It fulfills the same purpose as `rfcomm bind` for the old Bluetooth 2.0, creating a virtual serial port in `/dev/pts/x`, which makes it usable with any terminal or application.
 
 On Windows it provides a `COM` port, similar to the Microsoft "Standard Serial over Bluetooth" (a driver which exists since Windows XP and unsurprisingly also does not support BLE standards).
@@ -153,14 +157,15 @@
                         Duration of the scan in seconds (default: 5.0)
   -i ADAPTER, --interface ADAPTER
                         BLE host adapter number to use (default: hci0)
   -d ADDR, --deep-scan ADDR
                         Try to connect to device and read out service/characteristic UUIDs (default: None)
   -s SERVICE_UUID, --service-uuid SERVICE_UUID
                         The service used for scanning of potential devices (default: None)
+  -v, --verbose         Print all infos from advertisement data (default: False)
 ```
 
 On Bluetooth 2.0 there was a "serial port profile", with 4.0 - 5.2 (BLE) there is unfortunately no standardized mode anymore, every chip manufacturer chooses their own UUIDs to implement the features. 
 ```py
 '0000ff01-0000-1000-8000-00805f9b34fb', # LithiumBatteryPCB adapter: read/notify
 '0000ff02-0000-1000-8000-00805f9b34fb', # LithiumBatteryPCB adapter: write
 '0000ffe1-0000-1000-8000-00805f9b34fb', # TI CC245x (HM-10, HM-11)
```

### Comparing `ble-serial-2.7.1/README.md` & `ble_serial-2.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
                         Duration of the scan in seconds (default: 5.0)
   -i ADAPTER, --interface ADAPTER
                         BLE host adapter number to use (default: hci0)
   -d ADDR, --deep-scan ADDR
                         Try to connect to device and read out service/characteristic UUIDs (default: None)
   -s SERVICE_UUID, --service-uuid SERVICE_UUID
                         The service used for scanning of potential devices (default: None)
+  -v, --verbose         Print all infos from advertisement data (default: False)
 ```
 
 On Bluetooth 2.0 there was a "serial port profile", with 4.0 - 5.2 (BLE) there is unfortunately no standardized mode anymore, every chip manufacturer chooses their own UUIDs to implement the features. 
 ```py
 '0000ff01-0000-1000-8000-00805f9b34fb', # LithiumBatteryPCB adapter: read/notify
 '0000ff02-0000-1000-8000-00805f9b34fb', # LithiumBatteryPCB adapter: write
 '0000ffe1-0000-1000-8000-00805f9b34fb', # TI CC245x (HM-10, HM-11)
```

### Comparing `ble-serial-2.7.1/ble_serial/bluetooth/ble_interface.py` & `ble_serial-2.7.2/ble_serial/bluetooth/ble_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from bleak import BleakClient, BleakScanner
 from bleak.backends.characteristic import BleakGATTCharacteristic
-from bleak.exc import BleakError
 from ble_serial.bluetooth.constants import ble_chars
-import logging, asyncio
-from typing import Optional
+import logging
+import asyncio
+from typing import Optional, List
 
 class BLE_interface():
     def __init__(self, adapter: str, service: str):
         self._send_queue = asyncio.Queue()
 
         self.scan_args = dict(adapter=adapter)
         if service:
             self.scan_args['service_uuids'] = [service]
 
     async def connect(self, addr_str: str, addr_type: str, timeout: float):
         if addr_str:
             device = await BleakScanner.find_device_by_address(addr_str, timeout=timeout, **self.scan_args)
         else:
-            logging.warning(f'Picking first device with matching service, '
+            logging.warning('Picking first device with matching service, '
                 'consider passing a specific device address, especially if there could be multiple devices')
             device = await BleakScanner.find_device_by_filter(lambda dev, ad: True, timeout=timeout, **self.scan_args)
 
-        assert device, f'No matching device found!'
+        assert device, 'No matching device found!'
 
         # address_type used only in Windows .NET currently
         self.dev = BleakClient(device, address_type=addr_type,
             timeout=timeout, disconnected_callback=self.handle_disconnect)
 
         logging.info(f'Trying to connect with {device}')
         await self.dev.connect()
@@ -42,20 +42,20 @@
         
         if self.read_enabled:
             self.read_char = self.find_char(read_uuid, ['notify', 'indicate'])
             await self.dev.start_notify(self.read_char, self.handle_notify)
         else:
             logging.info('Reading disabled, skipping read UUID detection')
 
-    def find_char(self, uuid: Optional[str], req_props: [str]) -> BleakGATTCharacteristic:
+    def find_char(self, uuid: Optional[str], req_props: List[str]) -> BleakGATTCharacteristic:
         name = req_props[0]
 
         # Use user supplied UUID first, otherwise try included list
         if uuid:
-            uuid_candidates = [uuid]
+            uuid_candidates = [uuid.lower()]
         else:
             uuid_candidates = ble_chars
             logging.debug(f'No {name} uuid specified, trying builtin list')
 
         results = []
         for srv in self.dev.services:
             for c in srv.characteristics:
@@ -91,15 +91,15 @@
         self._cb = callback
         logging.info('Receiver set up')
 
     async def send_loop(self):
         assert hasattr(self, '_cb'), 'Callback must be set before receive loop!'
         while True:
             data = await self._send_queue.get()
-            if data == None:
+            if data is None:
                 break # Let future end on shutdown
             if not self.write_enabled:
                 logging.warning(f'Ignoring unexpected write data: {data}')
                 continue
             logging.debug(f'Sending {data}')
             await self.dev.write_gatt_char(self.write_char, data)
```

### Comparing `ble-serial-2.7.1/ble_serial/cli.py` & `ble_serial-2.7.2/ble_serial/cli.py`

 * *Files identical despite different names*

### Comparing `ble-serial-2.7.1/ble_serial/log/console_log.py` & `ble_serial-2.7.2/ble_serial/log/console_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import logging, coloredlogs
+import logging
+import coloredlogs
 
 def setup_logger(verbosity: int):
     bleak_logger = logging.getLogger('bleak')
     bleak_logger.level = logging.DEBUG if verbosity > 1 else logging.INFO
 
     level_colors = {
         'critical': {'bold': True, 'color': 'red'},
```

### Comparing `ble-serial-2.7.1/ble_serial/log/fs_log.py` & `ble_serial-2.7.2/ble_serial/log/fs_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import logging, datetime
-from enum import Enum
+import logging
+import datetime
 
 class Direction:
     BLE_IN = "-> BLE-IN"
     BLE_OUT = "<- BLE-OUT"
 
 class FS_log:
     def __init__(self, filename, binlog):
@@ -17,8 +17,8 @@
             t = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f")
             out = data.decode(errors='replace') if self.binlog else data.hex()
             self.file.write(f'{t} {dir}: {out} \n')
         return ret_func
 
     def finish(self):
         self.file.close()
-        logging.info(f'Logfile closed')
+        logging.info('Logfile closed')
```

### Comparing `ble-serial-2.7.1/ble_serial/main.py` & `ble_serial-2.7.2/ble_serial/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import logging, asyncio
+import logging
+import asyncio
 from bleak.exc import BleakError
 from ble_serial import platform_uart as UART
 from ble_serial.ports.tcp_socket import TCP_Socket
 from ble_serial.bluetooth.ble_interface import BLE_interface
 from ble_serial.log.fs_log import FS_log, Direction
 from ble_serial.log.console_log import setup_logger
 from ble_serial import cli
```

### Comparing `ble-serial-2.7.1/ble_serial/ports/linux_pty.py` & `ble_serial-2.7.2/ble_serial/ports/linux_pty.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from ble_serial.ports.interface import ISerial
-import asyncio, logging
-import os, pty, tty, termios
+import asyncio
+import logging
+import os
+import pty
+import tty
+import termios
 
 class UART(ISerial):
     def __init__(self, symlink: str, ev_loop: asyncio.AbstractEventLoop, mtu: int):
         self.loop = ev_loop
         self.mtu = mtu
         self._send_queue = asyncio.Queue()
 
@@ -30,15 +34,15 @@
         logging.info('Stopping serial event loop')
         self._send_queue.put_nowait(None)
 
     def remove(self):
         # Unregister the fd
         self.loop.remove_reader(self._controller_fd)
         os.remove(self.symlink)
-        logging.info(f'Serial reader and symlink removed')
+        logging.info('Serial reader and symlink removed')
 
 
     def read_handler(self):
         data = self.read_sync()
         self._cb(data)
 
     def read_sync(self):
@@ -48,11 +52,11 @@
 
     def queue_write(self, value: bytes):
         self._send_queue.put_nowait(value)
 
     async def run_loop(self):
         while True:
             data = await self._send_queue.get()
-            if data == None:
+            if data is None:
                 break # Let future end on shutdown
             logging.debug(f'Write: {data}')
             os.write(self._controller_fd, data)
```

### Comparing `ble-serial-2.7.1/ble_serial/ports/print_dummy.py` & `ble_serial-2.7.2/ble_serial/ports/print_dummy.py`

 * *Files identical despite different names*

### Comparing `ble-serial-2.7.1/ble_serial/ports/tcp_socket.py` & `ble_serial-2.7.2/ble_serial/ports/tcp_socket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ble_serial.ports.interface import ISerial
-import asyncio, logging
+import asyncio
+import logging
 
 
 class TCP_Socket(ISerial):
     def __init__(self, host: str, port: int, mtu: int):
         logging.debug(f'{host=}:{port=}, {mtu=}')
         self.host = host
         self.port = port
@@ -14,15 +15,15 @@
         self._cb = callback
 
     def queue_write(self, value: bytes):
         if self.connected:
             logging.debug(f'Sending: {value}')
             self.writer.write(value)
         else:
-            logging.debug(f'No client connected, dropping data...')
+            logging.debug('No client connected, dropping data...')
 
     def handle_connect(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
         logging.info(f'New TCP peer connected: {writer.get_extra_info("peername")}')
         if self.connected:
             logging.warning('More than one connection is not allowed, closing')
             writer.close()
             return
```

### Comparing `ble-serial-2.7.1/ble_serial/ports/windows_com0com.py` & `ble_serial-2.7.2/ble_serial/ports/windows_com0com.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ble_serial.ports.interface import ISerial
-import asyncio, logging
+import asyncio
+import logging
 from serial import Serial # pyserial
 from queue import Queue, Empty
 from concurrent.futures import ThreadPoolExecutor
 
 class COM(ISerial):
     def __init__(self, port: str, ev_loop: asyncio.AbstractEventLoop, mtu: int):
         self.alive = True # to stop executor threads
```

### Comparing `ble-serial-2.7.1/ble_serial/scan/main.py` & `ble_serial-2.7.2/ble_serial/scan/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from bleak import BleakScanner, BleakClient
 from bleak.backends.service import BleakGATTServiceCollection
-from bleak.backends.device import BLEDevice
 from bleak.exc import BleakError
-import argparse, asyncio
+import argparse
+import asyncio
 
 
 async def scan(adapter: str, timeout: float, service_uuid: str) -> dict:
     base_kwargs = dict(adapter=adapter, timeout=timeout, return_adv=True)
 
     if service_uuid:
         devices = await BleakScanner.discover(**base_kwargs, service_uuids=[service_uuid])
```

### Comparing `ble-serial-2.7.1/ble_serial/setup_com0com/__init__.py` & `ble_serial-2.7.2/ble_serial/setup_com0com/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
 
 def run_setup(path: str):
-    import ctypes, sys, os
+    import ctypes
+    import sys
+    import os
 
     script_path = os.path.dirname(__file__)
     res = ctypes.windll.shell32.ShellExecuteW(None, "runas", 
         sys.executable, f'{script_path}\\windows_priv_setupc.py "{path}"', None, 1)
     print('OK' if res == 42 else 'Error: higher privileges required')
 
 def main():
```

### Comparing `ble-serial-2.7.1/ble_serial/setup_com0com/windows_priv_setupc.py` & `ble_serial-2.7.2/ble_serial/setup_com0com/windows_priv_setupc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import os, sys
-import subprocess, re
+import os
+import sys
+import subprocess
+import re
 
 # For compatibility:
 # https://support.microsoft.com/en-us/topic/howto-specify-serial-ports-larger-than-com9-db9078a5-b7b6-bf00-240f-f749ebfd913e
 PORT_USER = 'COM9'
 PORT_INTERNAL = 'BLE'
 
 BIN = 'setupc.exe'
```

### Comparing `ble-serial-2.7.1/ble_serial.egg-info/PKG-INFO` & `ble_serial-2.7.2/ble_serial.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: ble-serial
-Version: 2.7.1
-Summary: A package to connect BLE serial adapters
+Version: 2.7.2
+Summary: Connects BLE adapters with virtual serial ports
 Home-page: https://github.com/Jakeler/ble-serial
 Author: Jake
 Author-email: ble-serial-pypi@ja-ke.tech
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: bleak>=0.20.0
+Requires-Dist: coloredlogs>=15.0
+Requires-Dist: pyserial>=3.4.0; platform_system == "Windows"
 
 # BLE Serial
 A tool to connect Bluetooth 4.0+ Low Energy to UART modules and normal PCs/laptops/RaspberryPi.
 
 It fulfills the same purpose as `rfcomm bind` for the old Bluetooth 2.0, creating a virtual serial port in `/dev/pts/x`, which makes it usable with any terminal or application.
 
 On Windows it provides a `COM` port, similar to the Microsoft "Standard Serial over Bluetooth" (a driver which exists since Windows XP and unsurprisingly also does not support BLE standards).
@@ -153,14 +157,15 @@
                         Duration of the scan in seconds (default: 5.0)
   -i ADAPTER, --interface ADAPTER
                         BLE host adapter number to use (default: hci0)
   -d ADDR, --deep-scan ADDR
                         Try to connect to device and read out service/characteristic UUIDs (default: None)
   -s SERVICE_UUID, --service-uuid SERVICE_UUID
                         The service used for scanning of potential devices (default: None)
+  -v, --verbose         Print all infos from advertisement data (default: False)
 ```
 
 On Bluetooth 2.0 there was a "serial port profile", with 4.0 - 5.2 (BLE) there is unfortunately no standardized mode anymore, every chip manufacturer chooses their own UUIDs to implement the features. 
 ```py
 '0000ff01-0000-1000-8000-00805f9b34fb', # LithiumBatteryPCB adapter: read/notify
 '0000ff02-0000-1000-8000-00805f9b34fb', # LithiumBatteryPCB adapter: write
 '0000ffe1-0000-1000-8000-00805f9b34fb', # TI CC245x (HM-10, HM-11)
```

### Comparing `ble-serial-2.7.1/ble_serial.egg-info/SOURCES.txt` & `ble_serial-2.7.2/ble_serial.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,10 @@
 ble_serial/ports/tcp_socket.py
 ble_serial/ports/windows_com0com.py
 ble_serial/scan/__init__.py
 ble_serial/scan/__main__.py
 ble_serial/scan/main.py
 ble_serial/setup_com0com/__init__.py
 ble_serial/setup_com0com/__main__.py
-ble_serial/setup_com0com/windows_priv_setupc.py
+ble_serial/setup_com0com/windows_priv_setupc.py
+tests/test.py
+tests/test_conn_reliability.py
```

### Comparing `ble-serial-2.7.1/setup.py` & `ble_serial-2.7.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import setuptools, platform
+import setuptools
+import platform
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fr:
     REQUIRES = fr.read()
 
 setuptools.setup(
     name="ble-serial",
-    version="2.7.1",
+    version="2.7.2",
     author="Jake",
     author_email="ble-serial-pypi@ja-ke.tech",
-    description="A package to connect BLE serial adapters",
+    description="Connects BLE adapters with virtual serial ports",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Jakeler/ble-serial",
     packages=[
         "ble_serial",
         "ble_serial.bluetooth",
         "ble_serial.ports",
@@ -30,20 +31,21 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=REQUIRES,
     entry_points={
         'console_scripts': [
             'ble-scan=ble_serial.scan.main:launch',
             'ble-serial=ble_serial.main:launch',
         ] + (
             ['ble-com-setup=ble_serial.setup_com0com:main'] if platform.system() == "Windows"
```

