# Comparing `tmp/ambient_event_bus_client-0.1.4.tar.gz` & `tmp/ambient_event_bus_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_event_bus_client-0.1.4.tar", last modified: Thu May  9 01:30:08 2024, max compression
+gzip compressed data, was "ambient_event_bus_client-0.1.5.tar", last modified: Mon May 27 21:26:41 2024, max compression
```

## Comparing `ambient_event_bus_client-0.1.4.tar` & `ambient_event_bus_client-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:30:08.279255 ambient_event_bus_client-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-09 01:30:08.279255 ambient_event_bus_client-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 01:30:08.279255 ambient_event_bus_client-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:30:08.279255 ambient_event_bus_client-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:30:08.279255 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:30:08.279255 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/models/event_api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/models/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 01:29:55.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/models/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:30:08.279255 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-09 01:30:08.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 01:30:08.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:30:08.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 01:30:08.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 01:30:08.000000 ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:26:41.417212 ambient_event_bus_client-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-27 21:26:41.417212 ambient_event_bus_client-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:26:41.417212 ambient_event_bus_client-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:26:41.413212 ambient_event_bus_client-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:26:41.417212 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:26:41.417212 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/models/event_api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/models/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-27 21:26:33.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/models/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:26:41.417212 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-27 21:26:41.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-27 21:26:41.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:26:41.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 21:26:41.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 21:26:41.000000 ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/top_level.txt
```

### Comparing `ambient_event_bus_client-0.1.4/PKG-INFO` & `ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: ambient_event_bus_client
-Version: 0.1.4
+Name: ambient-event-bus-client
+Version: 0.1.5
 Summary: A library to interact with the Ambient Labs Event Bus.
 Home-page: https://github.com/ambientlabscomputing/ambient-event-bus-client
 Author: Jose Catarino
 Author-email: jose@ambientlabscomputing.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Ambient Event Bus Client
@@ -33,7 +35,9 @@
 async for message in client.subscribe():
     print(message)
 
 # publish a message
 message = MessageCreate(topic="my_topic", message="my_message")
 await client.publish(message)
 ```
+
+
```

### Comparing `ambient_event_bus_client-0.1.4/README.md` & `ambient_event_bus_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ambient_event_bus_client-0.1.4/setup.py` & `ambient_event_bus_client-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ambient_event_bus_client",
-    version="0.1.4",
+    version="0.1.5",
     description="A library to interact with the Ambient Labs Event Bus.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Jose Catarino",
     author_email="jose@ambientlabscomputing.com",
     url="https://github.com/ambientlabscomputing/ambient-event-bus-client",
     package_dir={"": "src"},
```

### Comparing `ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/client.py` & `ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/client.py`

 * *Files identical despite different names*

### Comparing `ambient_event_bus_client-0.1.4/src/ambient_event_bus_client/models/event_api_models.py` & `ambient_event_bus_client-0.1.5/src/ambient_event_bus_client/models/event_api_models.py`

 * *Files identical despite different names*

### Comparing `ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/PKG-INFO` & `ambient_event_bus_client-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: ambient-event-bus-client
-Version: 0.1.4
+Name: ambient_event_bus_client
+Version: 0.1.5
 Summary: A library to interact with the Ambient Labs Event Bus.
 Home-page: https://github.com/ambientlabscomputing/ambient-event-bus-client
 Author: Jose Catarino
 Author-email: jose@ambientlabscomputing.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Ambient Event Bus Client
@@ -33,7 +35,9 @@
 async for message in client.subscribe():
     print(message)
 
 # publish a message
 message = MessageCreate(topic="my_topic", message="my_message")
 await client.publish(message)
 ```
+
+
```

### Comparing `ambient_event_bus_client-0.1.4/src/ambient_event_bus_client.egg-info/SOURCES.txt` & `ambient_event_bus_client-0.1.5/src/ambient_event_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

