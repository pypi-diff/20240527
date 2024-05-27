# Comparing `tmp/wyzeapy-0.5.8.tar.gz` & `tmp/wyzeapy-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wyzeapy-0.5.8.tar", max compression
+gzip compressed data, was "wyzeapy-0.5.9.tar", max compression
```

## Comparing `wyzeapy-0.5.8.tar` & `wyzeapy-0.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0        0        0        0 2021-09-27 12:48:53.333363 wyzeapy-0.5.8/LICENSES/
--rw-r--r--   0        0        0      434 2022-04-05 17:22:38.736455 wyzeapy-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     7926 2021-12-20 13:31:19.477622 wyzeapy-0.5.8/src/wyzeapy/__init__.py
--rw-r--r--   0        0        0      990 2021-09-27 12:48:53.336713 wyzeapy-0.5.8/src/wyzeapy/const.py
--rw-r--r--   0        0        0     1343 2021-12-20 13:31:19.478032 wyzeapy-0.5.8/src/wyzeapy/crypto.py
--rw-r--r--   0        0        0      872 2021-09-27 12:48:53.337292 wyzeapy-0.5.8/src/wyzeapy/exceptions.py
--rw-r--r--   0        0        0     2377 2021-12-20 13:31:19.478764 wyzeapy-0.5.8/src/wyzeapy/payload_factory.py
--rw-r--r--   0        0        0        0 2021-09-27 12:48:53.337695 wyzeapy-0.5.8/src/wyzeapy/services/__init__.py
--rw-r--r--   0        0        0    22910 2022-02-16 15:44:34.670417 wyzeapy-0.5.8/src/wyzeapy/services/base_service.py
--rw-r--r--   0        0        0     5893 2022-03-25 14:09:25.932959 wyzeapy-0.5.8/src/wyzeapy/services/bulb_service.py
--rw-r--r--   0        0        0     5106 2022-04-05 17:22:08.540298 wyzeapy-0.5.8/src/wyzeapy/services/camera_service.py
--rw-r--r--   0        0        0     2460 2021-12-20 13:31:19.481992 wyzeapy-0.5.8/src/wyzeapy/services/hms_service.py
--rw-r--r--   0        0        0     1514 2021-12-20 13:31:19.482669 wyzeapy-0.5.8/src/wyzeapy/services/lock_service.py
--rw-r--r--   0        0        0     3253 2021-12-20 13:31:19.483192 wyzeapy-0.5.8/src/wyzeapy/services/sensor_service.py
--rw-r--r--   0        0        0     1700 2021-12-20 13:31:19.483822 wyzeapy-0.5.8/src/wyzeapy/services/switch_service.py
--rw-r--r--   0        0        0     4161 2021-12-20 13:31:19.484590 wyzeapy-0.5.8/src/wyzeapy/services/thermostat_service.py
--rw-r--r--   0        0        0     5087 2022-02-10 15:33:47.908326 wyzeapy-0.5.8/src/wyzeapy/services/update_manager.py
--rw-r--r--   0        0        0     5359 2022-03-25 14:09:25.934937 wyzeapy-0.5.8/src/wyzeapy/types.py
--rw-r--r--   0        0        0     3718 2021-12-20 13:31:19.486211 wyzeapy-0.5.8/src/wyzeapy/utils.py
--rw-r--r--   0        0        0    12076 2021-12-20 13:31:19.486956 wyzeapy-0.5.8/src/wyzeapy/wyze_auth_lib.py
--rw-r--r--   0        0        0      791 2022-04-05 17:22:55.472075 wyzeapy-0.5.8/setup.py
--rw-r--r--   0        0        0      750 2022-04-05 17:22:55.472438 wyzeapy-0.5.8/PKG-INFO
+drwxr-xr-x   0        0        0        0 2021-12-08 19:26:58.746691 wyzeapy-0.5.9/LICENSES/
+-rw-r--r--   0        0        0      434 2022-04-14 17:52:27.135266 wyzeapy-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     7926 2022-02-04 21:23:52.084105 wyzeapy-0.5.9/src/wyzeapy/__init__.py
+-rw-r--r--   0        0        0      990 2022-02-04 21:23:52.084634 wyzeapy-0.5.9/src/wyzeapy/const.py
+-rw-r--r--   0        0        0     1343 2022-02-04 21:23:52.084993 wyzeapy-0.5.9/src/wyzeapy/crypto.py
+-rw-r--r--   0        0        0      872 2022-02-04 21:23:52.085697 wyzeapy-0.5.9/src/wyzeapy/exceptions.py
+-rw-r--r--   0        0        0     2377 2022-02-04 21:23:52.086417 wyzeapy-0.5.9/src/wyzeapy/payload_factory.py
+-rw-r--r--   0        0        0        0 2021-12-08 19:26:58.752066 wyzeapy-0.5.9/src/wyzeapy/services/__init__.py
+-rw-r--r--   0        0        0    22910 2022-02-04 21:23:57.132272 wyzeapy-0.5.9/src/wyzeapy/services/base_service.py
+-rw-r--r--   0        0        0     5672 2022-04-14 17:51:49.100900 wyzeapy-0.5.9/src/wyzeapy/services/bulb_service.py
+-rw-r--r--   0        0        0     5106 2022-04-14 17:51:49.101649 wyzeapy-0.5.9/src/wyzeapy/services/camera_service.py
+-rw-r--r--   0        0        0     2460 2021-12-10 14:32:33.726477 wyzeapy-0.5.9/src/wyzeapy/services/hms_service.py
+-rw-r--r--   0        0        0     1514 2021-12-10 15:36:35.699877 wyzeapy-0.5.9/src/wyzeapy/services/lock_service.py
+-rw-r--r--   0        0        0     3253 2021-12-10 15:36:35.703576 wyzeapy-0.5.9/src/wyzeapy/services/sensor_service.py
+-rw-r--r--   0        0        0     1700 2021-12-10 14:33:15.053701 wyzeapy-0.5.9/src/wyzeapy/services/switch_service.py
+-rw-r--r--   0        0        0     4161 2021-12-10 14:33:25.530258 wyzeapy-0.5.9/src/wyzeapy/services/thermostat_service.py
+-rw-r--r--   0        0        0     5087 2022-02-04 21:23:57.135801 wyzeapy-0.5.9/src/wyzeapy/services/update_manager.py
+-rw-r--r--   0        0        0     5359 2022-04-14 17:51:49.102443 wyzeapy-0.5.9/src/wyzeapy/types.py
+-rw-r--r--   0        0        0     3718 2021-12-10 14:59:19.333632 wyzeapy-0.5.9/src/wyzeapy/utils.py
+-rw-r--r--   0        0        0    12076 2021-12-10 15:34:38.312136 wyzeapy-0.5.9/src/wyzeapy/wyze_auth_lib.py
+-rw-r--r--   0        0        0      791 2022-04-14 17:53:38.963340 wyzeapy-0.5.9/setup.py
+-rw-r--r--   0        0        0      750 2022-04-14 17:53:38.963915 wyzeapy-0.5.9/PKG-INFO
```

### Comparing `wyzeapy-0.5.8/src/wyzeapy/__init__.py` & `wyzeapy-0.5.9/src/wyzeapy/__init__.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/const.py` & `wyzeapy-0.5.9/src/wyzeapy/const.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/crypto.py` & `wyzeapy-0.5.9/src/wyzeapy/crypto.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/exceptions.py` & `wyzeapy-0.5.9/src/wyzeapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/payload_factory.py` & `wyzeapy-0.5.9/src/wyzeapy/payload_factory.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/base_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/base_service.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/bulb_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/bulb_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,14 @@
 
         return [Bulb(bulb.raw_dict) for bulb in bulbs]
 
     async def turn_on(self, bulb: Bulb, local_control, options=None):
         plist = [
             create_pid_pair(PropertyIDs.ON, "1")
         ]
-        # Put bulb and strip back into basic color mode if it isn't already
-        if bulb.type in [DeviceTypes.LIGHTSTRIP, DeviceTypes.MESH_LIGHT]:
-            plist.append(create_pid_pair(PropertyIDs.COLOR_MODE, "1"))
 
         if options is not None:
             plist.extend(options)
 
         if bulb.type in [
             DeviceTypes.LIGHT
         ]:
```

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/camera_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/camera_service.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/hms_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/hms_service.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/lock_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/lock_service.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/sensor_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/sensor_service.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/switch_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/switch_service.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/thermostat_service.py` & `wyzeapy-0.5.9/src/wyzeapy/services/thermostat_service.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/services/update_manager.py` & `wyzeapy-0.5.9/src/wyzeapy/services/update_manager.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/types.py` & `wyzeapy-0.5.9/src/wyzeapy/types.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/utils.py` & `wyzeapy-0.5.9/src/wyzeapy/utils.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/src/wyzeapy/wyze_auth_lib.py` & `wyzeapy-0.5.9/src/wyzeapy/wyze_auth_lib.py`

 * *Files identical despite different names*

### Comparing `wyzeapy-0.5.8/setup.py` & `wyzeapy-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['aiodns>=3.0.0,<4.0.0',
  'aiohttp>=3.7,<4.0',
  'cchardet>=2.1.7,<3.0.0',
  'pycryptodome>=3.12.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'wyzeapy',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'A library for interacting with Wyze devices',
     'long_description': None,
     'author': 'Joshua Mulliken',
     'author_email': 'joshua@mulliken.net',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `wyzeapy-0.5.8/PKG-INFO` & `wyzeapy-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wyzeapy
-Version: 0.5.8
+Version: 0.5.9
 Summary: A library for interacting with Wyze devices
 License: GPL-3.0-only
 Author: Joshua Mulliken
 Author-email: joshua@mulliken.net
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

