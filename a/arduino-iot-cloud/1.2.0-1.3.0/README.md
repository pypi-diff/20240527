# Comparing `tmp/arduino_iot_cloud-1.2.0.tar.gz` & `tmp/arduino_iot_cloud-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arduino_iot_cloud-1.2.0.tar", last modified: Wed May 15 14:43:11 2024, max compression
+gzip compressed data, was "arduino_iot_cloud-1.3.0.tar", last modified: Mon May 27 11:02:53 2024, max compression
```

## Comparing `arduino_iot_cloud-1.2.0.tar` & `arduino_iot_cloud-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.563544 arduino_iot_cloud-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/examples/micropython_async_wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/examples/micropython_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.563544 arduino_iot_cloud-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/ucloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/umqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/ussl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 14:43:11.000000 arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:11.567544 arduino_iot_cloud-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/tests/ci.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1938 2024-05-15 14:43:03.000000 arduino_iot_cloud-1.2.0/tests/ci.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:02:53.000676 arduino_iot_cloud-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-27 11:02:53.000676 arduino_iot_cloud-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:02:52.996676 arduino_iot_cloud-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/examples/micropython_async_wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/examples/micropython_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:02:53.000676 arduino_iot_cloud-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:02:52.996676 arduino_iot_cloud-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:02:52.996676 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 11:02:52.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/ucloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/umqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/ussl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:02:53.000676 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-27 11:02:52.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-27 11:02:52.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:02:52.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:02:52.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 11:02:52.000000 arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:02:53.000676 arduino_iot_cloud-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/tests/ci.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1938 2024-05-27 11:02:48.000000 arduino_iot_cloud-1.3.0/tests/ci.sh
```

### Comparing `arduino_iot_cloud-1.2.0/LICENSE` & `arduino_iot_cloud-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.2.0/PKG-INFO` & `arduino_iot_cloud-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino_iot_cloud
-Version: 1.2.0
+Version: 1.3.0
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cbor2>=5.6.2
 Requires-Dist: micropython-senml>=0.1.1
 
 # Arduino IoT Cloud Python client ☁️🐍☁️
-This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
+This is a Python client for the Arduino IoT Cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, synchronous and asynchronous modes and provides a user-friendly API that allows users to connect to the cloud and create and link local objects to cloud objects with just a few lines of code.
 
 ## Minimal Example
 The following basic example shows how to connect to the Arduino IoT cloud using basic username and password authentication, and control an LED from a dashboard's switch widget.
 ```python
 from secrets import DEVICE_ID
 from secrets import SECRET_KEY
 
@@ -54,14 +54,31 @@
 ```python
 WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
 WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
 DEVICE_ID  = "" # Provided by Arduino cloud when creating a device.
 SECRET_KEY = "" # Provided by Arduino cloud when creating a device.
 ```
 
+Note that by default, the client runs in asynchronous mode. In this mode, the client takes runs an asyncio loop that updates tasks and records, polls networking events, etc. The client also supports a synchronous mode, which requires periodic client polling. To run the client in synchronous mode, pass `sync_mode=True` when creating a client object and call `client.update()` periodically after connecting. For example:
+
+```Python
+# Run the client in synchronous mode.
+client = ArduinoCloudClient(device_id=DEVICE_ID, ..., sync_mode=True)
+....
+client.register("led", value=None)
+....
+# In synchronous mode, this function returns immediately after connecting to the cloud.
+client.start()
+
+# Update the client periodically.
+while True:
+    client.update()
+    time.sleep(0.100)
+```
+
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
 
 #### Create softhsm token
 Using the first available slot, in this case 0
```

### Comparing `arduino_iot_cloud-1.2.0/README.md` & `arduino_iot_cloud-1.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Arduino IoT Cloud Python client ☁️🐍☁️
-This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
+This is a Python client for the Arduino IoT Cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, synchronous and asynchronous modes and provides a user-friendly API that allows users to connect to the cloud and create and link local objects to cloud objects with just a few lines of code.
 
 ## Minimal Example
 The following basic example shows how to connect to the Arduino IoT cloud using basic username and password authentication, and control an LED from a dashboard's switch widget.
 ```python
 from secrets import DEVICE_ID
 from secrets import SECRET_KEY
 
@@ -37,14 +37,31 @@
 ```python
 WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
 WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
 DEVICE_ID  = "" # Provided by Arduino cloud when creating a device.
 SECRET_KEY = "" # Provided by Arduino cloud when creating a device.
 ```
 
+Note that by default, the client runs in asynchronous mode. In this mode, the client takes runs an asyncio loop that updates tasks and records, polls networking events, etc. The client also supports a synchronous mode, which requires periodic client polling. To run the client in synchronous mode, pass `sync_mode=True` when creating a client object and call `client.update()` periodically after connecting. For example:
+
+```Python
+# Run the client in synchronous mode.
+client = ArduinoCloudClient(device_id=DEVICE_ID, ..., sync_mode=True)
+....
+client.register("led", value=None)
+....
+# In synchronous mode, this function returns immediately after connecting to the cloud.
+client.start()
+
+# Update the client periodically.
+while True:
+    client.update()
+    time.sleep(0.100)
+```
+
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
 
 #### Create softhsm token
 Using the first available slot, in this case 0
```

### Comparing `arduino_iot_cloud-1.2.0/examples/example.py` & `arduino_iot_cloud-1.3.0/examples/example.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     client["clight"].bri = round(uniform(0, 100), 1)
 
 
 if __name__ == "__main__":
     # Parse command line args.
     parser = argparse.ArgumentParser(description="arduino_iot_cloud.py")
     parser.add_argument("-d", "--debug", action="store_true",  help="Enable debugging messages")
+    parser.add_argument("-s", "--sync", action="store_true",  help="Run in synchronous mode")
     args = parser.parse_args()
 
     # Assume the host has an active Internet connection.
 
     # Configure the logger.
     # All message equal or higher to the logger level are printed.
     # To see more debugging messages, pass --debug on the command line.
@@ -56,27 +57,28 @@
         format="%(asctime)s.%(msecs)03d %(message)s",
         level=logging.DEBUG if args.debug else logging.INFO,
     )
 
     # Create a client object to connect to the Arduino IoT cloud.
     # The most basic authentication method uses a username and password. The username is the device
     # ID, and the password is the secret key obtained from the IoT cloud when provisioning a device.
-    client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
+    client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY, sync_mode=args.sync)
 
     # Alternatively, the client also supports key and certificate-based authentication. To use this
     # mode, set "keyfile" and "certfile", and the CA certificate (if any) in "ssl_params".
     # Furthermore, secure elements, which can be used to store the key and cert, are also supported.
     # To secure elements, set "use_hsm" to True in "ssl_params" and set the token's "pin" if any.
     # client = ArduinoCloudClient(
     #     device_id=DEVICE_ID,
     #     ssl_params={
     #         "use_hsm": True, "pin": "1234",
     #         "keyfile": KEY_PATH, "certfile": CERT_PATH, "cafile": CA_PATH,
     #         "verify_mode": ssl.CERT_REQUIRED, "server_hostname" : "iot.arduino.cc"
     #     },
+    #     sync_mode=args.sync,
     # )
 
     # Register cloud objects.
     # Note: The following objects must be created first in the dashboard and linked to the device.
     # This cloud object is initialized with its last known value from the cloud. When this object is updated
     # from the dashboard, the on_switch_changed function is called with the client object and the new value.
     client.register("sw1", value=None, on_write=on_switch_changed, interval=0.250)
@@ -103,9 +105,15 @@
     client.register(Schedule("schedule", on_active=lambda client, value: logging.info(f"Schedule activated {value}!")))
 
     # The client can also schedule user code in a task and run it along with the other cloud objects.
     # To schedule a user function, use the Task object and pass the task name and function in "on_run"
     # to client.register().
     client.register(Task("user_task", on_run=user_task, interval=1.0))
 
-    # Start the Arduino IoT cloud client.
+    # Start the Arduino IoT cloud client. In synchronous mode, this function returns immediately
+    # after connecting to the cloud.
     client.start()
+
+    # In sync mode, start returns after connecting, and the client must be polled periodically.
+    while True:
+        client.update()
+        time.sleep(0.100)
```

### Comparing `arduino_iot_cloud-1.2.0/examples/micropython_async_wifi.py` & `arduino_iot_cloud-1.3.0/examples/micropython_async_wifi.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.2.0/examples/micropython_basic.py` & `arduino_iot_cloud-1.3.0/examples/micropython_basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,34 +62,35 @@
 if __name__ == "__main__":
     # Configure the logger.
     # All message equal or higher to the logger level are printed.
     # To see more debugging messages, set level=logging.DEBUG.
     logging.basicConfig(
         datefmt="%H:%M:%S",
         format="%(asctime)s.%(msecs)03d %(message)s",
-        level=logging.INFO,
+        level=logging.DEBUG,
     )
 
     # NOTE: Add networking code here or in boot.py
     wifi_connect()
 
     # Create a client object to connect to the Arduino IoT cloud.
     # The most basic authentication method uses a username and password. The username is the device
     # ID, and the password is the secret key obtained from the IoT cloud when provisioning a device.
-    client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
+    client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY, sync_mode=False)
 
     # Alternatively, the client also supports key and certificate-based authentication. To use this
     # mode, set "keyfile" and "certfile", and the CA certificate (if any) in "ssl_params".
     # Note that for MicroPython, the key and cert files must be stored in DER format on the filesystem.
     # client = ArduinoCloudClient(
     #     device_id=DEVICE_ID,
     #     ssl_params={
     #         "keyfile": KEY_PATH, "certfile": CERT_PATH, "cadata": CADATA,
     #         "verify_mode": ssl.CERT_REQUIRED, "server_hostname" : "iot.arduino.cc"
     #     },
+    #     sync_mode=False,
     # )
 
     # Register cloud objects.
     # Note: The following objects must be created first in the dashboard and linked to the device.
     # This cloud object is initialized with its last known value from the cloud. When this object is updated
     # from the dashboard, the on_switch_changed function is called with the client object and the new value.
     client.register("sw1", value=None, on_write=on_switch_changed, interval=0.250)
@@ -129,9 +130,15 @@
             from machine import WDT
             # Enable the WDT with a timeout of 5s (1s is the minimum)
             wdt = WDT(timeout=7500)
             client.register(Task("watchdog_task", on_run=wdt_task, interval=1.0))
         except (ImportError, AttributeError):
             pass
 
-    # Start the Arduino IoT cloud client.
+    # Start the Arduino IoT cloud client. In synchronous mode, this function returns immediately
+    # after connecting to the cloud.
     client.start()
+
+    # In sync mode, start returns after connecting, and the client must be polled periodically.
+    while True:
+        client.update()
+        time.sleep(0.100)
```

### Comparing `arduino_iot_cloud-1.2.0/package.json` & `arduino_iot_cloud-1.3.0/package.json`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.2.0/pyproject.toml` & `arduino_iot_cloud-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/__init__.py` & `arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file is part of the Arduino IoT Cloud Python client.
 # Copyright (c) 2022 Arduino SA
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-import asyncio
 import binascii
 from .ucloud import ArduinoCloudClient  # noqa
 from .ucloud import ArduinoCloudObject
+from .ucloud import ArduinoCloudObject as Task  # noqa
 from .ucloud import timestamp
 
 
 CADATA = binascii.unhexlify(
     b"308201cf30820174a00302010202141f101deba7e125e727c1a391e3ec0d"
     b"174ded4a59300a06082a8648ce3d0403023045310b300906035504061302"
     b"555331173015060355040a130e41726475696e6f204c4c43205553310b30"
@@ -26,41 +26,14 @@
     b"0106300f0603551d130101ff040530030101ff301d0603551d0e04160414"
     b"5b3e2a6b8ec9b01aa854e6369b8c09f9fce1b980300a06082a8648ce3d04"
     b"03020349003046022100bfd3dc236668b50adc3f0d0ec373e20ac7f760aa"
     b"100dd320bfe102969b6b05d8022100ead9d9da5acd12529709a8ed660fe1"
     b"8d6444ffe82217304ff2b89aafca8ecf"
 )
 
-async def coro():  # noqa
-    pass
-
-
-def is_async(obj):
-    if hasattr(asyncio, "iscoroutinefunction"):
-        return asyncio.iscoroutinefunction(obj)
-    else:
-        return isinstance(obj, type(coro))
-
-
-class Task(ArduinoCloudObject):
-    def __init__(self, name, **kwargs):
-        kwargs.update({("runnable", True)})  # Force task creation.
-        self.on_run = kwargs.pop("on_run", None)
-        if not callable(self.on_run):
-            raise TypeError("Expected a callable object")
-        super().__init__(name, **kwargs)
-
-    async def run(self, aiot):
-        if is_async(self.on_run):
-            await self.on_run(aiot)
-        else:
-            while True:
-                self.on_run(aiot)
-                await asyncio.sleep(self.interval)
-
 
 class Location(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         super().__init__(name, keys={"lat", "lon"}, **kwargs)
 
 
 class Color(ArduinoCloudObject):
@@ -76,32 +49,30 @@
 class DimmedLight(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
         super().__init__(name, keys={"swi", "bri"}, **kwargs)
 
 
 class Schedule(ArduinoCloudObject):
     def __init__(self, name, **kwargs):
-        kwargs.update({("runnable", True)})  # Force task creation.
+        kwargs.update({("on_run", self.on_run)})
         self.on_active = kwargs.pop("on_active", None)
         # Uncomment to allow the schedule to change in runtime.
         # kwargs["on_write"] = kwargs.get("on_write", lambda aiot, value: None)
         self.active = False
         super().__init__(name, keys={"frm", "to", "len", "msk"}, **kwargs)
 
-    async def run(self, aiot):
-        while True:
-            if self.initialized:
-                ts = timestamp() + aiot.get("tz_offset", 0)
-                if ts > self.frm and ts < (self.frm + self.len):
-                    if not self.active and self.on_active is not None:
-                        self.on_active(aiot, self.value)
-                    self.active = True
-                else:
-                    self.active = False
-            await asyncio.sleep(self.interval)
+    def on_run(self, aiot):
+        if self.initialized:
+            ts = timestamp() + aiot.get("tz_offset", 0)
+            if ts > self.frm and ts < (self.frm + self.len):
+                if not self.active and self.on_active is not None:
+                    self.on_active(aiot, self.value)
+                self.active = True
+            else:
+                self.active = False
 
 
 class Television(ArduinoCloudObject):
     PLAYBACK_FASTFORWARD = 0
     PLAYBACK_NEXT = 1
     PLAYBACK_PAUSE = 2
     PLAYBACK_PLAY = 3
```

### Comparing `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/ucloud.py` & `arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/ucloud.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import time
 import sys
 import logging
+import cbor2
 from senml import SenmlPack
 from senml import SenmlRecord
 from arduino_iot_cloud.umqtt import MQTTClient
-
 import asyncio
 from asyncio import CancelledError
 try:
     from asyncio import InvalidStateError
 except (ImportError, AttributeError):
     # MicroPython doesn't have this exception
     class InvalidStateError(Exception):
         pass
+try:
+    from arduino_iot_cloud._version import __version__
+except (ImportError, AttributeError):
+    __version__ = "1.3.0"
 
 # Server/port for basic auth.
 _DEFAULT_SERVER = "iot.arduino.cc"
 
 # Default port for cert based auth and basic auth.
 _DEFAULT_PORT = (8883, 8884)
 
@@ -31,33 +35,40 @@
     pass
 
 
 def timestamp():
     return int(time.time())
 
 
+def timestamp_ms():
+    return time.time_ns()//1000000
+
+
 def log_level_enabled(level):
     return logging.getLogger().isEnabledFor(level)
 
 
 class ArduinoCloudObject(SenmlRecord):
     def __init__(self, name, **kwargs):
         self.on_read = kwargs.pop("on_read", None)
         self.on_write = kwargs.pop("on_write", None)
+        self.on_run = kwargs.pop("on_run", None)
         self.interval = kwargs.pop("interval", 1.0)
-        self._runnable = kwargs.pop("runnable", False)
+        self.backoff = kwargs.pop("backoff", None)
         value = kwargs.pop("value", None)
         if keys := kwargs.pop("keys", {}):
             value = {   # Create a complex object (with sub-records).
                 k: ArduinoCloudObject(f"{name}:{k}", value=v, callback=self.senml_callback)
                 for (k, v) in {k: kwargs.pop(k, None) for k in keys}.items()
             }
         self._updated = False
         self.on_write_scheduled = False
         self.timestamp = timestamp()
+        self.last_poll = timestamp_ms()
+        self.runnable = any((self.on_run, self.on_read, self.on_write))
         callback = kwargs.pop("callback", self.senml_callback)
         for key in kwargs:  # kwargs should be empty by now, unless a wrong attr was used.
             raise TypeError(f"'{self.__class__.__name__}' got an unexpected keyword argument '{key}'")
         super().__init__(name, value=value, callback=callback)
 
     def __repr__(self):
         return f"{self.value}"
@@ -80,18 +91,14 @@
 
     @property
     def initialized(self):
         if isinstance(self.value, dict):
             return all(r.initialized for r in self.value.values())
         return self.value is not None
 
-    @property
-    def runnable(self):
-        return self.on_read is not None or self.on_write is not None or self._runnable
-
     @SenmlRecord.value.setter
     def value(self, value):
         if value is not None:
             if self.value is not None:
                 # This is a workaround for the cloud float/int conversion bug.
                 if isinstance(self.value, float) and isinstance(value, int):
                     value = float(value)
@@ -148,44 +155,53 @@
         # The updated flag is cleared to avoid sending the same value again to the cloud,
         # and the on_write function flag is set to so it gets called on the next run.
         self.updated = False
         self.on_write_scheduled = True
 
     async def run(self, client):
         while True:
-            if self.on_read is not None:
-                self.value = self.on_read(client)
-            if self.on_write is not None and self.on_write_scheduled:
-                self.on_write_scheduled = False
-                self.on_write(client, self if isinstance(self.value, dict) else self.value)
+            self.run_sync(client)
             await asyncio.sleep(self.interval)
+            if self.backoff is not None:
+                self.interval = min(self.interval * self.backoff, 5.0)
+
+    def run_sync(self, client):
+        if self.on_run is not None:
+            self.on_run(client)
+        if self.on_read is not None:
+            self.value = self.on_read(client)
+        if self.on_write is not None and self.on_write_scheduled:
+            self.on_write_scheduled = False
+            self.on_write(client, self if isinstance(self.value, dict) else self.value)
 
 
 class ArduinoCloudClient:
     def __init__(
             self,
             device_id,
             username=None,
             password=None,
             ssl_params={},
             server=None,
             port=None,
             keepalive=10,
             ntp_server="pool.ntp.org",
-            ntp_timeout=3
+            ntp_timeout=3,
+            sync_mode=False
     ):
         self.tasks = {}
         self.records = {}
         self.thing_id = None
         self.keepalive = keepalive
         self.last_ping = timestamp()
         self.senmlpack = SenmlPack("", self.senml_generic_callback)
-        self.started = False
         self.ntp_server = ntp_server
         self.ntp_timeout = ntp_timeout
+        self.async_mode = not sync_mode
+        self.connected = False
 
         if "pin" in ssl_params:
             try:
                 # Use M2Crypto to load key and cert from HSM.
                 import M2Crypto  # noqa
             except (ImportError, AttributeError):
                 logging.error("The m2crypto module is required to use HSM.")
@@ -196,28 +212,29 @@
             device_id = bytes(device_id, "utf-8")
         if username is not None and isinstance(username, str):
             username = bytes(username, "utf-8")
         if password is not None and isinstance(password, str):
             password = bytes(password, "utf-8")
 
         self.device_topic = b"/a/d/" + device_id + b"/e/i"
+        self.command_topic = b"/a/d/" + device_id + b"/c/up"
 
         # Update RTC from NTP server on MicroPython.
         self.update_systime()
 
         # If no server/port were passed in args, set the default server/port
         # based on authentication type.
         if server is None:
             server = _DEFAULT_SERVER
         if port is None:
             port = _DEFAULT_PORT[0] if password is None else _DEFAULT_PORT[1]
 
         # Create MQTT client.
         self.mqtt = MQTTClient(
-                device_id, server, port, ssl_params, username, password, keepalive, self.mqtt_callback
+            device_id, server, port, ssl_params, username, password, keepalive, self.mqtt_callback
         )
 
         # Add internal objects initialized by the cloud.
         for name in ["thing_id", "tz_offset", "tz_dst_until"]:
             self.register(name, value=None)
 
     def __getitem__(self, key):
@@ -248,19 +265,20 @@
         except Exception as e:
             if log_level_enabled(logging.ERROR):
                 logging.error(f"Failed to set RTC time from NTP: {e}.")
 
     def create_task(self, name, coro, *args, **kwargs):
         if callable(coro):
             coro = coro(*args)
-        if self.started:
+        try:
+            asyncio.get_event_loop()
             self.tasks[name] = asyncio.create_task(coro)
             if log_level_enabled(logging.INFO):
                 logging.info(f"task: {name} created.")
-        else:
+        except Exception:
             # Defer task creation until there's a running event loop.
             self.tasks[name] = coro
 
     def create_topic(self, topic, inout):
         return bytes(f"/a/t/{self.thing_id}/{topic}/{inout}", "utf-8")
 
     def register(self, aiotobj, coro=None, **kwargs):
@@ -268,22 +286,22 @@
             if kwargs.get("value", None) is None and kwargs.get("on_read", None) is not None:
                 kwargs["value"] = kwargs.get("on_read")(self)
             aiotobj = ArduinoCloudObject(aiotobj, **kwargs)
 
         # Register the ArduinoCloudObject
         self.records[aiotobj.name] = aiotobj
 
-        # Create a task for this object if it has any callbacks.
-        if aiotobj.runnable:
-            self.create_task(aiotobj.name, aiotobj.run, self)
-
         # Check if object needs to be initialized from the cloud.
         if not aiotobj.initialized and "r:m" not in self.records:
             self.register("r:m", value="getLastValues")
 
+        # Create a task for this object if it has any callbacks.
+        if self.async_mode and aiotobj.runnable:
+            self.create_task(aiotobj.name, aiotobj.run, self)
+
     def senml_generic_callback(self, record, **kwargs):
         # This callback catches all unknown/umatched sub/records that were not part of the pack.
         rname, sname = record.name.split(":") if ":" in record.name else [record.name, None]
         if rname in self.records:
             if log_level_enabled(logging.INFO):
                 logging.info(f"Ignoring cloud initialization for record: {record.name}")
         else:
@@ -299,84 +317,99 @@
             # object. Otherwise, for initialized objects, updates are only allowed if the object
             # is writable (on_write function is set) and the value is received from the out topic.
             if not record.initialized or (record.on_write is not None and b"shadow" not in topic):
                 record.add_to_pack(self.senmlpack)
         self.senmlpack.from_cbor(message)
         self.senmlpack.clear()
 
-    async def discovery_task(self, interval=0.100):
-        self.mqtt.subscribe(self.device_topic, qos=1)
-        while self.thing_id is None:
-            self.mqtt.check_msg()
-            if self.records.get("thing_id").value is not None:
-                self.thing_id = self.records.pop("thing_id").value
-                if not self.thing_id:  # Empty thing ID should not happen.
-                    raise (Exception("Device is not linked to a Thing ID."))
-
-                self.topic_out = self.create_topic("e", "o")
-                self.mqtt.subscribe(self.create_topic("e", "i"))
-
-                if lastval_record := self.records.pop("r:m", None):
-                    lastval_record.add_to_pack(self.senmlpack)
-                    self.mqtt.subscribe(self.create_topic("shadow", "i"), qos=1)
-                    self.mqtt.publish(self.create_topic("shadow", "o"), self.senmlpack.to_cbor(), qos=1)
-                logging.info("Device configured via discovery protocol.")
-            await asyncio.sleep(interval)
-        raise DoneException()
+    def ts_expired(self, ts, last_ts_ms, interval_s):
+        return last_ts_ms == 0 or (ts - last_ts_ms) > int(interval_s * 1000)
 
-    async def conn_task(self, interval=1.0, backoff=1.2):
+    def poll_records(self):
+        ts = timestamp_ms()
+        try:
+            for record in self.records.values():
+                if record.runnable and self.ts_expired(ts, record.last_poll, record.interval):
+                    record.run_sync(self)
+                    record.last_poll = ts
+        except Exception as e:
+            self.records.pop(record.name)
+            if log_level_enabled(logging.ERROR):
+                logging.error(f"task: {record.name} raised exception: {str(e)}.")
+
+    def poll_connect(self, aiot=None):
         logging.info("Connecting to Arduino IoT cloud...")
-        while True:
-            try:
-                self.mqtt.connect()
-                break
-            except Exception as e:
-                if log_level_enabled(logging.WARNING):
-                    logging.warning(f"Connection failed {e}, retrying after {interval}s")
-                await asyncio.sleep(interval)
-                interval = min(interval * backoff, 4.0)
+        try:
+            self.mqtt.connect()
+        except Exception as e:
+            if log_level_enabled(logging.WARNING):
+                logging.warning(f"Connection failed {e}, retrying...")
+            return
 
         if self.thing_id is None:
-            self.create_task("discovery", self.discovery_task)
+            self.mqtt.subscribe(self.device_topic, qos=1)
         else:
             self.mqtt.subscribe(self.create_topic("e", "i"))
-        self.create_task("mqtt_task", self.mqtt_task)
-        raise DoneException()
 
-    async def mqtt_task(self, interval=0.100):
-        while True:
-            self.mqtt.check_msg()
-            if self.thing_id is not None:
-                self.senmlpack.clear()
-                for record in self.records.values():
-                    if record.updated:
-                        record.add_to_pack(self.senmlpack, push=True)
-                if len(self.senmlpack._data):
-                    logging.debug("Pushing records to Arduino IoT cloud:")
-                    if log_level_enabled(logging.DEBUG):
-                        for record in self.senmlpack._data:
-                            logging.debug(f"  ==> record: {record.name} value: {str(record.value)[:48]}...")
-                    self.mqtt.publish(self.topic_out, self.senmlpack.to_cbor(), qos=1)
-                    self.last_ping = timestamp()
-                elif self.keepalive and (timestamp() - self.last_ping) > self.keepalive:
-                    self.mqtt.ping()
-                    self.last_ping = timestamp()
-                    logging.debug("No records to push, sent a ping request.")
-            await asyncio.sleep(interval)
-        raise DoneException()
+        if self.async_mode:
+            if self.thing_id is None:
+                self.register("discovery", on_run=self.poll_discovery, interval=0.200)
+            self.register("mqtt_task", on_run=self.poll_mqtt, interval=0.100)
+            raise DoneException()
+        self.connected = True
+
+    def poll_discovery(self, aiot=None):
+        self.mqtt.check_msg()
+        if self.records.get("thing_id").value is not None:
+            self.thing_id = self.records.pop("thing_id").value
+            if not self.thing_id:  # Empty thing ID should not happen.
+                raise Exception("Device is not linked to a Thing ID.")
 
-    async def run(self):
-        self.started = True
+            self.topic_out = self.create_topic("e", "o")
+            self.mqtt.subscribe(self.create_topic("e", "i"))
+
+            if lastval_record := self.records.pop("r:m", None):
+                lastval_record.add_to_pack(self.senmlpack)
+                self.mqtt.subscribe(self.create_topic("shadow", "i"), qos=1)
+                self.mqtt.publish(self.create_topic("shadow", "o"), self.senmlpack.to_cbor(), qos=1)
+
+            # Push library version and mode.
+            libv = "%s-%s" % (__version__, "async" if self.async_mode else "sync")
+            self.mqtt.publish(self.command_topic, cbor2.dumps(cbor2.CBORTag(67328, [libv])), qos=1)
+            logging.info("Device configured via discovery protocol.")
+            if self.async_mode:
+                raise DoneException()
+
+    def poll_mqtt(self, aiot=None):
+        self.mqtt.check_msg()
+        if self.thing_id is not None:
+            self.senmlpack.clear()
+            for record in self.records.values():
+                if record.updated:
+                    record.add_to_pack(self.senmlpack, push=True)
+            if len(self.senmlpack._data):
+                logging.debug("Pushing records to Arduino IoT cloud:")
+                if log_level_enabled(logging.DEBUG):
+                    for record in self.senmlpack._data:
+                        logging.debug(f"  ==> record: {record.name} value: {str(record.value)[:48]}...")
+                self.mqtt.publish(self.topic_out, self.senmlpack.to_cbor(), qos=1)
+                self.last_ping = timestamp()
+            elif self.keepalive and (timestamp() - self.last_ping) > self.keepalive:
+                self.mqtt.ping()
+                self.last_ping = timestamp()
+                logging.debug("No records to push, sent a ping request.")
+
+    async def run(self, interval, backoff):
         # Creates tasks from coros here manually before calling
         # gather, so we can keep track of tasks in self.tasks dict.
         for name, coro in self.tasks.items():
             self.create_task(name, coro)
 
         # Create connection task.
-        self.create_task("conn_task", self.conn_task)
+        self.register("connection_task", on_run=self.poll_connect, interval=interval, backoff=backoff)
 
         while True:
             task_except = None
             try:
                 await asyncio.gather(*self.tasks.values(), return_exceptions=False)
                 break   # All tasks are done, not likely.
             except Exception as e:
@@ -390,14 +423,59 @@
                         self.tasks.pop(name)
                         self.records.pop(name, None)
                         if isinstance(task_except, DoneException) and log_level_enabled(logging.INFO):
                             logging.info(f"task: {name} complete.")
                         elif task_except is not None and log_level_enabled(logging.ERROR):
                             logging.error(f"task: {name} raised exception: {str(task_except)}.")
                         if name == "mqtt_task":
-                            self.create_task("conn_task", self.conn_task)
+                            self.register(
+                                "connection_task",
+                                on_run=self.poll_connect,
+                                interval=interval,
+                                backoff=backoff
+                            )
                         break   # Break after the first task is removed.
                 except (CancelledError, InvalidStateError):
                     pass
 
-    def start(self):
-        asyncio.run(self.run())
+    def start(self, interval=1.0, backoff=1.2):
+        if self.async_mode:
+            asyncio.run(self.run(interval, backoff))
+            return
+
+        last_conn_ms = 0
+        last_disc_ms = 0
+
+        while True:
+            ts = timestamp_ms()
+            if not self.connected and self.ts_expired(ts, last_conn_ms, interval):
+                self.poll_connect()
+                if last_conn_ms != 0:
+                    interval = min(interval * backoff, 5.0)
+                last_conn_ms = ts
+
+            if self.connected and self.thing_id is None and self.ts_expired(ts, last_disc_ms, 0.250):
+                self.poll_discovery()
+                last_disc_ms = ts
+
+            if self.connected and self.thing_id is not None:
+                break
+            self.poll_records()
+
+    def update(self):
+        if self.async_mode:
+            raise RuntimeError("This function can't be called in asyncio mode.")
+
+        if not self.connected:
+            try:
+                self.start()
+            except Exception as e:
+                raise e
+
+        self.poll_records()
+
+        try:
+            self.poll_mqtt()
+        except Exception as e:
+            self.connected = False
+            if log_level_enabled(logging.WARNING):
+                logging.warning(f"Connection lost {e}")
```

### Comparing `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/umqtt.py` & `arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/umqtt.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud/ussl.py` & `arduino_iot_cloud-1.3.0/src/arduino_iot_cloud/ussl.py`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/PKG-INFO` & `arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arduino_iot_cloud
-Version: 1.2.0
+Version: 1.3.0
 Summary: Arduino IoT Cloud Python client
 Author-email: Ibrahim Abdelkader <i.abdelkader@arduino.cc>
 Project-URL: Homepage, https://github.com/arduino/arduino-iot-cloud-py
 Project-URL: Bug Tracker, https://github.com/arduino/arduino-iot-cloud-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cbor2>=5.6.2
 Requires-Dist: micropython-senml>=0.1.1
 
 # Arduino IoT Cloud Python client ☁️🐍☁️
-This is a Python client for the Arduino IoT cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, and provides a user-friendly API that allows the user to connect to the cloud, and create and link local objects to cloud objects with a just a few lines of code.
+This is a Python client for the Arduino IoT Cloud, which runs on both CPython and MicroPython. The client supports basic and advanced authentication methods, synchronous and asynchronous modes and provides a user-friendly API that allows users to connect to the cloud and create and link local objects to cloud objects with just a few lines of code.
 
 ## Minimal Example
 The following basic example shows how to connect to the Arduino IoT cloud using basic username and password authentication, and control an LED from a dashboard's switch widget.
 ```python
 from secrets import DEVICE_ID
 from secrets import SECRET_KEY
 
@@ -54,14 +54,31 @@
 ```python
 WIFI_SSID  = ""  # WiFi network SSID (for MicroPython)
 WIFI_PASS  = ""  # WiFi network key  (for MicroPython)
 DEVICE_ID  = "" # Provided by Arduino cloud when creating a device.
 SECRET_KEY = "" # Provided by Arduino cloud when creating a device.
 ```
 
+Note that by default, the client runs in asynchronous mode. In this mode, the client takes runs an asyncio loop that updates tasks and records, polls networking events, etc. The client also supports a synchronous mode, which requires periodic client polling. To run the client in synchronous mode, pass `sync_mode=True` when creating a client object and call `client.update()` periodically after connecting. For example:
+
+```Python
+# Run the client in synchronous mode.
+client = ArduinoCloudClient(device_id=DEVICE_ID, ..., sync_mode=True)
+....
+client.register("led", value=None)
+....
+# In synchronous mode, this function returns immediately after connecting to the cloud.
+client.start()
+
+# Update the client periodically.
+while True:
+    client.update()
+    time.sleep(0.100)
+```
+
 For more detailed examples and advanced API features, please see the [examples](https://github.com/arduino/arduino-iot-cloud-py/tree/main/examples).
 
 ## Testing on CPython/Linux
 The client supports basic authentication using a username and password, and the more advanced key/cert pair stored on filesystem or in a crypto device. To test this functionality, the following steps can be used to emulate a crypto device (if one is not available) using SoftHSM on Linux.
 
 #### Create softhsm token
 Using the first available slot, in this case 0
```

### Comparing `arduino_iot_cloud-1.2.0/src/arduino_iot_cloud.egg-info/SOURCES.txt` & `arduino_iot_cloud-1.3.0/src/arduino_iot_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arduino_iot_cloud-1.2.0/tests/ci.py` & `arduino_iot_cloud-1.3.0/tests/ci.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 # This file is part of the Python Arduino IoT Cloud.
 # Any copyright is dedicated to the Public Domain.
 # https://creativecommons.org/publicdomain/zero/1.0/
 import logging
 import os
+import time
 import sys
 import asyncio
 from arduino_iot_cloud import ArduinoCloudClient
+from arduino_iot_cloud import Task
 import argparse
 
 
 def exception_handler(loop, context):
     pass
 
 
 def on_value_changed(client, value):
     logging.info(f"The answer to life, the universe, and everything is {value}")
     loop = asyncio.get_event_loop()
     loop.set_exception_handler(exception_handler)
     sys.exit(0)
 
 
+def wdt_task(client, ts=[None]):
+    if ts[0] is None:
+        ts[0] = time.time()
+    if time.time() - ts[0] > 5:
+        loop = asyncio.get_event_loop()
+        loop.set_exception_handler(exception_handler)
+        logging.error("Timeout waiting for variable")
+        sys.exit(1)
+
+
 if __name__ == "__main__":
     # Parse command line args.
     parser = argparse.ArgumentParser(description="arduino_iot_cloud.py")
     parser.add_argument(
         "-d", "--debug", action="store_true", help="Enable debugging messages"
     )
     parser.add_argument(
@@ -31,14 +43,17 @@
     )
     parser.add_argument(
         "-c", "--crypto-device", action="store_true", help="Use soft-hsm/crypto device",
     )
     parser.add_argument(
         "-f", "--file-auth", action="store_true", help="Use key/cert files"
     )
+    parser.add_argument(
+        "-s", "--sync", action="store_true",  help="Run in synchronous mode"
+    )
     args = parser.parse_args()
 
     # Configure the logger.
     # All message equal or higher to the logger level are printed.
     # To see more debugging messages, pass --debug on the command line.
     logging.basicConfig(
         datefmt="%H:%M:%S",
@@ -52,45 +67,49 @@
     # be used to authenticate, for example:
     #   client = ArduinoCloudClient(device_id=DEVICE_ID, username=DEVICE_ID, password=SECRET_KEY)
     if args.basic_auth:
         client = ArduinoCloudClient(
             device_id=os.getenv("DEVICE_ID"),
             username=os.getenv("DEVICE_ID"),
             password=os.getenv("SECRET_KEY"),
+            sync_mode=args.sync,
         )
     elif args.file_auth:
         import ssl
         client = ArduinoCloudClient(
             device_id=os.getenv("DEVICE_ID"),
             ssl_params={
                 "keyfile": "key.pem",
                 "certfile": "cert.pem",
                 "ca_certs": "ca-root.pem",
                 "cert_reqs": ssl.CERT_REQUIRED,
             },
+            sync_mode=args.sync,
         )
     elif args.crypto_device:
         import ssl
         client = ArduinoCloudClient(
             device_id=os.getenv("DEVICE_ID"),
             ssl_params={
                 "pin": "1234",
+                "use_hsm": True,
                 "keyfile": "pkcs11:token=arduino",
                 "certfile": "pkcs11:token=arduino",
                 "ca_certs": "ca-root.pem",
                 "cert_reqs": ssl.CERT_REQUIRED,
                 "engine_path": "/lib/x86_64-linux-gnu/engines-3/libpkcs11.so",
                 "module_path": "/lib/x86_64-linux-gnu/softhsm/libsofthsm2.so",
             },
+            sync_mode=args.sync,
         )
     else:
         parser.print_help()
         sys.exit(1)
 
     # Register cloud objects.
-    # Note: The following objects must be created first in the dashboard and linked to the device.
-    # This cloud object is initialized with its last known value from the cloud. When this object is updated
-    # from the dashboard, the on_switch_changed function is called with the client object and the new value.
+    # When this object gets initialized from the cloud the test is complete.
     client.register("answer", value=None, on_write=on_value_changed)
+    # This task will exist with failure after a timeout.
+    client.register(Task("wdt_task", on_run=wdt_task, interval=1.0))
 
     # Start the Arduino IoT cloud client.
     client.start()
```

### Comparing `arduino_iot_cloud-1.2.0/tests/ci.sh` & `arduino_iot_cloud-1.3.0/tests/ci.sh`

 * *Files identical despite different names*

