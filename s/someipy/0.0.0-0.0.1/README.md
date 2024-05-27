# Comparing `tmp/someipy-0.0.0.tar.gz` & `tmp/someipy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "someipy-0.0.0.tar", last modified: Tue Feb  6 18:11:25 2024, max compression
+gzip compressed data, was "someipy-0.0.1.tar", last modified: Mon May 27 17:33:24 2024, max compression
```

## Comparing `someipy-0.0.0.tar` & `someipy-0.0.1.tar`

### file list

```diff
@@ -1,31 +1,41 @@
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-02-06 18:11:25.793568 someipy-0.0.0/
--rw-r--r--   0 christian  (1000) christian  (1000)     3465 2024-02-06 18:11:25.793568 someipy-0.0.0/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)     2912 2024-02-04 12:11:59.000000 someipy-0.0.0/README.md
--rw-rw-r--   0 christian  (1000) christian  (1000)       85 2024-02-05 17:51:36.000000 someipy-0.0.0/pyproject.toml
--rw-rw-r--   0 christian  (1000) christian  (1000)      689 2024-02-06 18:11:25.793568 someipy-0.0.0/setup.cfg
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-02-06 18:11:25.793568 someipy-0.0.0/src/
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-02-06 18:11:25.793568 someipy-0.0.0/src/someipy/
--rw-r--r--   0 christian  (1000) christian  (1000)        0 2024-01-05 10:03:40.000000 someipy-0.0.0/src/someipy/__init__.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-02-06 18:11:25.793568 someipy-0.0.0/src/someipy/_internal/
--rw-rw-r--   0 christian  (1000) christian  (1000)        0 2024-01-26 09:28:19.000000 someipy-0.0.0/src/someipy/_internal/__init__.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      558 2024-02-05 18:34:14.000000 someipy-0.0.0/src/someipy/_internal/logging.py
--rw-r--r--   0 christian  (1000) christian  (1000)      280 2024-01-03 12:28:30.000000 someipy-0.0.0/src/someipy/_internal/message_types.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     1336 2024-02-05 18:34:28.000000 someipy-0.0.0/src/someipy/_internal/service_discovery_abcs.py
--rw-r--r--   0 christian  (1000) christian  (1000)      439 2024-01-15 08:08:48.000000 someipy-0.0.0/src/someipy/_internal/session_handler.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1750 2024-02-05 18:34:34.000000 someipy-0.0.0/src/someipy/_internal/simple_timer.py
--rw-r--r--   0 christian  (1000) christian  (1000)     2583 2024-01-31 18:44:07.000000 someipy-0.0.0/src/someipy/_internal/someip_header.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     6594 2024-02-05 18:34:46.000000 someipy-0.0.0/src/someipy/_internal/someip_sd_builder.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     2241 2024-01-31 18:37:36.000000 someipy-0.0.0/src/someipy/_internal/someip_sd_extractors.py
--rw-r--r--   0 christian  (1000) christian  (1000)    10877 2024-02-05 18:34:54.000000 someipy-0.0.0/src/someipy/_internal/someip_sd_header.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     3075 2024-01-26 12:16:23.000000 someipy-0.0.0/src/someipy/_internal/utils.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      218 2024-02-05 18:53:36.000000 someipy-0.0.0/src/someipy/logging.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     6757 2024-02-05 18:53:12.000000 someipy-0.0.0/src/someipy/serialization.py
--rw-r--r--   0 christian  (1000) christian  (1000)     7033 2024-02-05 18:53:40.000000 someipy-0.0.0/src/someipy/server_service_instance.py
--rw-r--r--   0 christian  (1000) christian  (1000)     4807 2024-02-05 18:33:01.000000 someipy-0.0.0/src/someipy/service_discovery.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-02-06 18:11:25.793568 someipy-0.0.0/src/someipy.egg-info/
--rw-r--r--   0 christian  (1000) christian  (1000)     3465 2024-02-06 18:11:25.000000 someipy-0.0.0/src/someipy.egg-info/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)      784 2024-02-06 18:11:25.000000 someipy-0.0.0/src/someipy.egg-info/SOURCES.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        1 2024-02-06 18:11:25.000000 someipy-0.0.0/src/someipy.egg-info/dependency_links.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        8 2024-02-06 18:11:25.000000 someipy-0.0.0/src/someipy.egg-info/top_level.txt
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-02-06 18:11:25.793568 someipy-0.0.0/tests/
--rw-rw-r--   0 christian  (1000) christian  (1000)     3123 2024-02-05 18:41:04.000000 someipy-0.0.0/tests/test_serialization.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-05-27 17:33:24.345662 someipy-0.0.1/
+-rw-r--r--   0 christian  (1000) christian  (1000)     5065 2024-05-27 17:33:24.345662 someipy-0.0.1/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4512 2024-05-22 19:29:29.000000 someipy-0.0.1/README.md
+-rw-rw-r--   0 christian  (1000) christian  (1000)       85 2024-02-06 18:12:42.000000 someipy-0.0.1/pyproject.toml
+-rw-rw-r--   0 christian  (1000) christian  (1000)      689 2024-05-27 17:33:24.345662 someipy-0.0.1/setup.cfg
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-05-27 17:33:24.337663 someipy-0.0.1/src/
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-05-27 17:33:24.341663 someipy-0.0.1/src/someipy/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      322 2024-05-22 18:17:52.000000 someipy-0.0.1/src/someipy/__init__.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-05-27 17:33:24.345662 someipy-0.0.1/src/someipy/_internal/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        0 2024-02-06 18:12:42.000000 someipy-0.0.1/src/someipy/_internal/__init__.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      920 2024-05-22 18:17:52.000000 someipy-0.0.1/src/someipy/_internal/logging.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1181 2024-02-18 13:14:39.000000 someipy-0.0.1/src/someipy/_internal/message_types.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1402 2024-05-04 14:51:06.000000 someipy-0.0.1/src/someipy/_internal/service_discovery_abcs.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      439 2024-02-06 18:12:42.000000 someipy-0.0.1/src/someipy/_internal/session_handler.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1750 2024-02-06 18:12:42.000000 someipy-0.0.1/src/someipy/_internal/simple_timer.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2560 2024-05-04 14:51:06.000000 someipy-0.0.1/src/someipy/_internal/someip_data_processor.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3035 2024-05-22 18:17:52.000000 someipy-0.0.1/src/someipy/_internal/someip_endpoint.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2606 2024-05-04 14:51:06.000000 someipy-0.0.1/src/someipy/_internal/someip_header.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      168 2024-05-04 14:51:06.000000 someipy-0.0.1/src/someipy/_internal/someip_message.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     6594 2024-02-06 18:12:42.000000 someipy-0.0.1/src/someipy/_internal/someip_sd_builder.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2241 2024-02-06 18:12:42.000000 someipy-0.0.1/src/someipy/_internal/someip_sd_extractors.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    10877 2024-03-17 10:51:07.000000 someipy-0.0.1/src/someipy/_internal/someip_sd_header.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1880 2024-05-04 14:51:06.000000 someipy-0.0.1/src/someipy/_internal/subscribers.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4304 2024-05-22 18:17:52.000000 someipy-0.0.1/src/someipy/_internal/tcp_client_manager.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1232 2024-05-22 18:17:52.000000 someipy-0.0.1/src/someipy/_internal/tcp_connection.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3075 2024-02-29 19:50:15.000000 someipy-0.0.1/src/someipy/_internal/utils.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    13292 2024-05-27 17:26:53.000000 someipy-0.0.1/src/someipy/client_service_instance.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      630 2024-05-23 18:49:34.000000 someipy-0.0.1/src/someipy/logging.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    17680 2024-05-22 19:29:07.000000 someipy-0.0.1/src/someipy/serialization.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    15979 2024-05-27 17:06:15.000000 someipy-0.0.1/src/someipy/server_service_instance.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4159 2024-05-23 18:52:58.000000 someipy-0.0.1/src/someipy/service.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     8939 2024-05-23 18:49:07.000000 someipy-0.0.1/src/someipy/service_discovery.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-05-27 17:33:24.345662 someipy-0.0.1/src/someipy.egg-info/
+-rw-r--r--   0 christian  (1000) christian  (1000)     5065 2024-05-27 17:33:24.000000 someipy-0.0.1/src/someipy.egg-info/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1157 2024-05-27 17:33:24.000000 someipy-0.0.1/src/someipy.egg-info/SOURCES.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        1 2024-05-27 17:33:24.000000 someipy-0.0.1/src/someipy.egg-info/dependency_links.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        8 2024-05-27 17:33:24.000000 someipy-0.0.1/src/someipy.egg-info/top_level.txt
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-05-27 17:33:24.345662 someipy-0.0.1/tests/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3281 2024-05-04 14:51:06.000000 someipy-0.0.1/tests/test_serialization.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2286 2024-05-04 14:51:06.000000 someipy-0.0.1/tests/test_someip_data_processor.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2214 2024-05-04 14:51:06.000000 someipy-0.0.1/tests/test_subscribers.py
```

### Comparing `someipy-0.0.0/README.md` & `someipy-0.0.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,69 @@
 # someipy - A Python Library for the SOME/IP Protocol
 
+## Feature Requests, Bugs, Contact
+
+For feature requests or bug reports, send a message on GitHub or write an email to:
+> :email: [someipy.package@gmail.com](mailto:someipy.package@gmail.com)
+
+## What is someipy?
+
 someipy is a Python library implementing the SOME/IP protocol, including the SOME/IP SD (Service Discovery) in Python. It's perfectly suited for fast prototyping of applications that need to provide (server) or use (client) SOME/IP services from other ECUs.
 
 someipy also supports serialization and deserialization of SOME/IP payloads, which is a unique feature compared to other libraries.
 
 someipy is still under development; therefore, it does not yet support all features of the SOME/IP and SOME/IP Service Discovery protocol specification.
 
 someipy is based on the specification version of R22-11:
 - [SOME/IP Protocol Specification](https://www.autosar.org/fileadmin/standards/R22-11/FO/AUTOSAR_PRS_SOMEIPProtocol.pdf)
 - [SOME/IP Service Discovery Protocol Specification](https://www.autosar.org/fileadmin/standards/R22-11/FO/AUTOSAR_PRS_SOMEIPServiceDiscoveryProtocol.pdf)
 
 The library is currently developed and tested under Ubuntu 22.04 and Python 3.12.
 
+## Typical Use Cases
+
+someipy excels in scenarios where a full-scale Autosar (Adaptive or Classic) integration would be excessive:
+
+- :test_tube: **Develop Test Applications**: Easily create test applications to stimulate the SOME/IP interfaces of your system under test. Whether running on a PC in a SIL environment or on an ECU, someipy allows you to efficiently send and receive SOME/IP events or utilize/provide SOME/IP services. Test data can be seamlessly generated or imported in Python, from sources such as .csv files or ROS bag files. Explore the [example applications](#example-applications) for more details.
+
+- :battery: **Prototype Sensor Integration**: Quickly integrate new sensors into your project using SOME/IP, ideal for evaluating the sensor's potential impact without significant effort. Define the message/parameter layout in Python and create a server service instance in minutes. Check out the [example application](#example-applications) *send_events_udp.py* for a practical demonstration.
+
+- :microscope: **Data Recording**: Set up a SOME/IP recording application in just a few minutes and store data in your preferred format, such as ROS bags, .csv files, or databases. Simply dump the received data within your callback function. The [example application](#example-applications) *receive_events_udp.py* illustrates this process.
+
+## Installation
+
+The package can be installed from [PyPi](https://pypi.org/project/someipy/).
+
+```bash
+pip install someipy
+```
+
 ## Example Applications
 
 In the directory [example_apps](./example_apps/), examples including explanations, can be found for using the someipy library. In [temperature_msg.py](./example_apps/temperature_msg.py), a payload interface "TemperatureMsg" is defined, which can be serialized and deserialized. In [send_events.py](./example_apps/send_events.py), the service discovery and two services are instantiated. The "TemperatureMsg" is serialized and used as the payload for sending events.
 
 ## Supported Features, Limitations and Deviations
 
 The library is still under development. The current major limitations and deviations from the protocol specifications are listed below.
 
 ### SOME/IP
 
-- Only events (and field notifiers) are supported. Methods (and field getters/setters) are not supported yet.
-- Receiving events is not supported yet. The server-side only is supported for now. Client service instances for receiving SOME/IP events are supported soon.
-- Only UDP services are supported.
+- Events (and field notifiers) are supported.
+- Methods are only supported on server side (offering methods). Calling methods (clients) is not supported yet.
 - Only unicast services are supported.
 - SOME/IP-TP is not supported.
 - IPv6 endpoints are not supported.
 - Session handling is supported only for SOME/IP-SD and not for SOME/IP messages transporting events.
 
 ### Service Discovery
 
 - Configuration and load balancing options in SOME/IP SD messages are not supported.
 - TTL of Service Discovery entries is not checked yet.
 - The Initial Wait Phase and Repetition Phase of the Service Discovery specification are skipped. For simplification, the Main Phase is directly entered, i.e. SD Offer Entries are immediately sent cyclically.
 - Multiple Service Discovery entries are not packed together in a single SD message, which is sent via UDP.
 
 ### De-/Serialization
 
-- Only fixed size arrays are supported.
+- Only fixed size arrays are supported. Dynamically sized arrays are not supported.
 - Optional length fields for SOME/IP arrays are not supported.
 - Strings are not supported yet.
 - Configuration of padding is not supported yet.
```

### Comparing `someipy-0.0.0/setup.cfg` & `someipy-0.0.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = someipy
-version = 0.0.0
+version = 0.0.1
 author = Christian H.
 author_email = someipy.package@gmail.com
 description = A Python package implementing the SOME/IP protocol
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chrizog/someipy
 project_urls =
```

### Comparing `someipy-0.0.0/src/someipy/_internal/service_discovery_abcs.py` & `someipy-0.0.1/src/someipy/_internal/service_discovery_abcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import ipaddress
 from abc import ABC, abstractmethod
-from someipy._internal.someip_sd_header import *
+from someipy._internal.someip_sd_header import SdService, SdEventGroupEntry, SdIPV4EndpointOption
 from someipy._internal.session_handler import SessionHandler
 
 
 class ServiceDiscoveryObserver(ABC):
     @abstractmethod
     def offer_service_update(self, offered_service: SdService) -> None:
         pass
```

### Comparing `someipy-0.0.0/src/someipy/_internal/simple_timer.py` & `someipy-0.0.1/src/someipy/_internal/simple_timer.py`

 * *Files identical despite different names*

### Comparing `someipy-0.0.0/src/someipy/_internal/someip_header.py` & `someipy-0.0.1/src/someipy/_internal/someip_header.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     client_id: int
     session_id: int
     protocol_version: int
     interface_version: int
     message_type: int
     return_code: int
 
+    MINIMAL_SIZE = 16
+
     def is_sd_header(self) -> bool:
         return (
             self.service_id == SERVICE_ID_SD
             and self.method_id == METHOD_ID_SD
             and self.client_id == CLIENT_ID_SD
             and self.protocol_version == PROTOCOL_VERSION_SD
             and self.interface_version == INTERFACE_VERSION_SD
```

### Comparing `someipy-0.0.0/src/someipy/_internal/someip_sd_builder.py` & `someipy-0.0.1/src/someipy/_internal/someip_sd_builder.py`

 * *Files identical despite different names*

### Comparing `someipy-0.0.0/src/someipy/_internal/someip_sd_extractors.py` & `someipy-0.0.1/src/someipy/_internal/someip_sd_extractors.py`

 * *Files identical despite different names*

### Comparing `someipy-0.0.0/src/someipy/_internal/someip_sd_header.py` & `someipy-0.0.1/src/someipy/_internal/someip_sd_header.py`

 * *Files identical despite different names*

### Comparing `someipy-0.0.0/src/someipy/_internal/utils.py` & `someipy-0.0.1/src/someipy/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `someipy-0.0.0/src/someipy.egg-info/SOURCES.txt` & `someipy-0.0.1/src/someipy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 README.md
 pyproject.toml
 setup.cfg
 src/someipy/__init__.py
+src/someipy/client_service_instance.py
 src/someipy/logging.py
 src/someipy/serialization.py
 src/someipy/server_service_instance.py
+src/someipy/service.py
 src/someipy/service_discovery.py
 src/someipy.egg-info/PKG-INFO
 src/someipy.egg-info/SOURCES.txt
 src/someipy.egg-info/dependency_links.txt
 src/someipy.egg-info/top_level.txt
 src/someipy/_internal/__init__.py
 src/someipy/_internal/logging.py
 src/someipy/_internal/message_types.py
 src/someipy/_internal/service_discovery_abcs.py
 src/someipy/_internal/session_handler.py
 src/someipy/_internal/simple_timer.py
+src/someipy/_internal/someip_data_processor.py
+src/someipy/_internal/someip_endpoint.py
 src/someipy/_internal/someip_header.py
+src/someipy/_internal/someip_message.py
 src/someipy/_internal/someip_sd_builder.py
 src/someipy/_internal/someip_sd_extractors.py
 src/someipy/_internal/someip_sd_header.py
+src/someipy/_internal/subscribers.py
+src/someipy/_internal/tcp_client_manager.py
+src/someipy/_internal/tcp_connection.py
 src/someipy/_internal/utils.py
-tests/test_serialization.py
+tests/test_serialization.py
+tests/test_someip_data_processor.py
+tests/test_subscribers.py
```

### Comparing `someipy-0.0.0/tests/test_serialization.py` & `someipy-0.0.1/tests/test_serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,23 @@
-import sys
-sys.path.append("src")
-
-import pytest
-from someipy.serialization import *
+from dataclasses import dataclass
+from someipy.serialization import (
+    Uint8,
+    Uint16,
+    Uint32,
+    Uint64,
+    Sint8,
+    Sint16,
+    Sint32,
+    Sint64,
+    Bool,
+    Float32,
+    Float64,
+    SomeIpPayload,
+    SomeIpFixedSizeArray,
+)
 
 
 def test_base_types_len():
     assert 1 == len(Uint8(1))
     assert 2 == len(Uint16(1))
     assert 4 == len(Uint32(1))
     assert 8 == len(Uint64(1))
@@ -119,11 +130,11 @@
     assert bytes.fromhex("00000000") == a.serialize()
 
     a.data[0] = Uint8(1)
     a.data[1] = Uint8(2)
     a.data[2] = Uint8(3)
     a.data[3] = Uint8(4)
     # Expected hex: 0x 01 02 03 04
-    assert bytes.fromhex("01020304") == a.serialize()    
+    assert bytes.fromhex("01020304") == a.serialize()
 
     a_again = SomeIpFixedSizeArray(Uint8, 4).deserialize(bytes.fromhex("01020304"))
     assert a_again == a
```

