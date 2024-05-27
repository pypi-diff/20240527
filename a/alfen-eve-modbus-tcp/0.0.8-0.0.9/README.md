# Comparing `tmp/alfen_eve_modbus_tcp-0.0.8.tar.gz` & `tmp/alfen_eve_modbus_tcp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfen_eve_modbus_tcp-0.0.8.tar", last modified: Thu Sep 21 15:08:43 2023, max compression
+gzip compressed data, was "alfen_eve_modbus_tcp-0.0.9.tar", last modified: Thu Sep 21 15:18:24 2023, max compression
```

## Comparing `alfen_eve_modbus_tcp-0.0.8.tar` & `alfen_eve_modbus_tcp-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:08:43.569407 alfen_eve_modbus_tcp-0.0.8/
--rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.8/LICENSE
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-09-21 15:08:43.569407 alfen_eve_modbus_tcp-0.0.8/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-16 19:44:24.000000 alfen_eve_modbus_tcp-0.0.8/README.md
--rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-09-21 15:08:43.569407 alfen_eve_modbus_tcp-0.0.8/setup.cfg
--rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.8/setup.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:08:43.565407 alfen_eve_modbus_tcp-0.0.8/src/
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:08:43.569407 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp/
--rw-rw-r--   0 luc       (1000) luc       (1000)    25524 2023-09-21 15:03:31.000000 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp/__init__.py
-drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:08:43.569407 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp.egg-info/
--rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-09-21 15:08:43.000000 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
--rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-09-21 15:08:43.000000 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-09-21 15:08:43.000000 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-09-21 15:08:43.000000 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp.egg-info/requires.txt
--rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-09-21 15:08:43.000000 alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:18:24.582951 alfen_eve_modbus_tcp-0.0.9/
+-rw-rw-r--   0 luc       (1000) luc       (1000)     1063 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.9/LICENSE
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-09-21 15:18:24.582951 alfen_eve_modbus_tcp-0.0.9/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)    11717 2023-07-16 19:44:24.000000 alfen_eve_modbus_tcp-0.0.9/README.md
+-rw-rw-r--   0 luc       (1000) luc       (1000)      861 2023-09-21 15:18:24.582951 alfen_eve_modbus_tcp-0.0.9/setup.cfg
+-rwxrwxr-x   0 luc       (1000) luc       (1000)       38 2023-07-14 13:22:32.000000 alfen_eve_modbus_tcp-0.0.9/setup.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:18:24.578951 alfen_eve_modbus_tcp-0.0.9/src/
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:18:24.578951 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    25524 2023-09-21 15:17:46.000000 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp/__init__.py
+drwxrwxr-x   0 luc       (1000) luc       (1000)        0 2023-09-21 15:18:24.582951 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp.egg-info/
+-rw-rw-r--   0 luc       (1000) luc       (1000)    12403 2023-09-21 15:18:24.000000 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO
+-rw-rw-r--   0 luc       (1000) luc       (1000)      312 2023-09-21 15:18:24.000000 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp.egg-info/SOURCES.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)        1 2023-09-21 15:18:24.000000 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp.egg-info/dependency_links.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       40 2023-09-21 15:18:24.000000 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp.egg-info/requires.txt
+-rw-rw-r--   0 luc       (1000) luc       (1000)       21 2023-09-21 15:18:24.000000 alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp.egg-info/top_level.txt
```

### Comparing `alfen_eve_modbus_tcp-0.0.8/LICENSE` & `alfen_eve_modbus_tcp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.8/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfen_eve_modbus_tcp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `alfen_eve_modbus_tcp-0.0.8/README.md` & `alfen_eve_modbus_tcp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alfen_eve_modbus_tcp-0.0.8/setup.cfg` & `alfen_eve_modbus_tcp-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alfen_eve_modbus_tcp
-version = 0.0.8
+version = 0.0.9
 author = nessnaj
 description = Alfen Eve Car Charger parser library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/nessnaj/alfen_eve_modbus_tcp
 project_urls =
```

### Comparing `alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp/__init__.py` & `alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             result = self.client.read_holding_registers(address, length, slave=slave)
 
             if not isinstance(result, ReadHoldingRegistersResponse):
                 continue
             if len(result.registers) != length:
                 continue
 
-            return BinaryPayloadDecoder.fromRegisters(result.registers, byteorder=Endian.Big, wordorder=self.wordorder)
+            return BinaryPayloadDecoder.fromRegisters(result.registers, byteorder=Endian.BIG, wordorder=self.wordorder)
 
         return None
 
     def _write_holding_register(self, slave, address, value):
         return self.client.write_registers(address=address, values=value, slave=slave)
 
     def _encode_value(self, data, dtype):
```

### Comparing `alfen_eve_modbus_tcp-0.0.8/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO` & `alfen_eve_modbus_tcp-0.0.9/src/alfen_eve_modbus_tcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfen-eve-modbus-tcp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Alfen Eve Car Charger parser library
 Home-page: https://github.com/nessnaj/alfen_eve_modbus_tcp
 Author: nessnaj
 License: MIT License
 Project-URL: Issue Tracker, https://github.com/nessnaj/alfen_eve_modbus_tcp/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
```

