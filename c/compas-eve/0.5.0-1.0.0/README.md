# Comparing `tmp/compas_eve-0.5.0.tar.gz` & `tmp/compas_eve-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_eve-0.5.0.tar", last modified: Wed May  1 15:51:20 2024, max compression
+gzip compressed data, was "compas_eve-1.0.0.tar", last modified: Mon May 27 18:03:39 2024, max compression
```

## Comparing `compas_eve-0.5.0.tar` & `compas_eve-1.0.0.tar`

### file list

```diff
@@ -1,46 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/
--rw-rw-rw-   0        0        0      102 2024-05-01 15:49:05.000000 compas_eve-0.5.0/AUTHORS.md
--rw-rw-rw-   0        0        0     3053 2024-05-01 15:49:05.000000 compas_eve-0.5.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1102 2024-05-01 15:49:05.000000 compas_eve-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      436 2024-05-01 15:49:05.000000 compas_eve-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3149 2024-05-01 15:51:20.568605 compas_eve-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2101 2024-05-01 15:49:05.000000 compas_eve-0.5.0/README.md
--rw-rw-rw-   0        0        0      713 2024-05-01 15:49:05.000000 compas_eve-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       35 2024-05-01 15:49:05.000000 compas_eve-0.5.0/requirements.txt
--rw-rw-rw-   0        0        0      219 2024-05-01 15:51:20.568605 compas_eve-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2058 2024-05-01 15:49:05.000000 compas_eve-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.552991 compas_eve-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.552991 compas_eve-0.5.0/src/compas_eve/
--rw-rw-rw-   0        0        0     1430 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/__init__.py
--rw-rw-rw-   0        0        0      123 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/__main__.py
--rw-rw-rw-   0        0        0     8299 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/core.py
--rw-rw-rw-   0        0        0     9313 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/event_emitter.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/ghpython/
--rw-rw-rw-   0        0        0      427 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/ghpython/__init__.py
--rw-rw-rw-   0        0        0     9911 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/ghpython/background.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/ghpython/components/
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/
--rw-rw-rw-   0        0        0     2359 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py
--rw-rw-rw-   0        0        0      492 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/icon.png
--rw-rw-rw-   0        0        0     1106 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json
--rw-rw-rw-   0        0        0        0 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/ghpython/components/___init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/ghpython/components/ghuser/
--rw-rw-rw-   0        0        0     2235 2024-05-01 15:51:15.000000 compas_eve-0.5.0/src/compas_eve/ghpython/components/ghuser/Ce_BackgroundTask.ghuser
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/memory/
--rw-rw-rw-   0        0        0     3547 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/memory/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/mqtt/
--rw-rw-rw-   0        0        0      504 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/mqtt/__init__.py
--rw-rw-rw-   0        0        0     5254 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/mqtt/mqtt_cli.py
--rw-rw-rw-   0        0        0     5313 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/mqtt/mqtt_paho.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/mqtt/netlib/
--rw-rw-rw-   0        0        0   303104 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/mqtt/netlib/MQTTnet.dll
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve/rhino/
--rw-rw-rw-   0        0        0        0 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/rhino/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-05-01 15:49:05.000000 compas_eve-0.5.0/src/compas_eve/rhino/install.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:51:20.568605 compas_eve-0.5.0/src/compas_eve.egg-info/
--rw-rw-rw-   0        0        0     3149 2024-05-01 15:51:20.000000 compas_eve-0.5.0/src/compas_eve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2024-05-01 15:51:20.000000 compas_eve-0.5.0/src/compas_eve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:51:20.000000 compas_eve-0.5.0/src/compas_eve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 15:49:28.000000 compas_eve-0.5.0/src/compas_eve.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2024-05-01 15:51:20.000000 compas_eve-0.5.0/src/compas_eve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 15:51:20.000000 compas_eve-0.5.0/src/compas_eve.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.685654 compas_eve-1.0.0/
+-rw-rw-rw-   0        0        0      102 2024-05-27 18:01:43.000000 compas_eve-1.0.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     3254 2024-05-27 18:01:43.000000 compas_eve-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1102 2024-05-27 18:01:43.000000 compas_eve-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      436 2024-05-27 18:01:43.000000 compas_eve-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3149 2024-05-27 18:03:39.685654 compas_eve-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2101 2024-05-27 18:01:43.000000 compas_eve-1.0.0/README.md
+-rw-rw-rw-   0        0        0      713 2024-05-27 18:01:43.000000 compas_eve-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       35 2024-05-27 18:01:43.000000 compas_eve-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0      219 2024-05-27 18:03:39.685654 compas_eve-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2058 2024-05-27 18:01:43.000000 compas_eve-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.654398 compas_eve-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/
+-rw-rw-rw-   0        0        0     1430 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/__main__.py
+-rw-rw-rw-   0        0        0     8299 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/core.py
+-rw-rw-rw-   0        0        0     9313 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/event_emitter.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/
+-rw-rw-rw-   0        0        0      427 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/__init__.py
+-rw-rw-rw-   0        0        0     9911 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/background.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/components/
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/
+-rw-rw-rw-   0        0        0     2359 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py
+-rw-rw-rw-   0        0        0      492 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/icon.png
+-rw-rw-rw-   0        0        0     1106 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Message/
+-rw-rw-rw-   0        0        0     2108 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Message/code.py
+-rw-rw-rw-   0        0        0     1505 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Message/icon.png
+-rw-rw-rw-   0        0        0      638 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Message/metadata.json
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_MqttConnect/
+-rw-rw-rw-   0        0        0     1105 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_MqttConnect/code.py
+-rw-rw-rw-   0        0        0     1439 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_MqttConnect/icon.png
+-rw-rw-rw-   0        0        0     1253 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_MqttConnect/metadata.json
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Publish/
+-rw-rw-rw-   0        0        0     1203 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Publish/code.py
+-rw-rw-rw-   0        0        0     1684 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Publish/icon.png
+-rw-rw-rw-   0        0        0     1292 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Publish/metadata.json
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Subscribe/
+-rw-rw-rw-   0        0        0     1934 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Subscribe/code.py
+-rw-rw-rw-   0        0        0     1671 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Subscribe/icon.png
+-rw-rw-rw-   0        0        0     1299 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_Subscribe/metadata.json
+-rw-rw-rw-   0        0        0        0 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/___init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/ghpython/components/ghuser/
+-rw-rw-rw-   0        0        0     2238 2024-05-27 18:03:36.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/ghuser/Ce_BackgroundTask.ghuser
+-rw-rw-rw-   0        0        0     2795 2024-05-27 18:03:36.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/ghuser/Ce_Message.ghuser
+-rw-rw-rw-   0        0        0     2910 2024-05-27 18:03:36.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/ghuser/Ce_MqttConnect.ghuser
+-rw-rw-rw-   0        0        0     3232 2024-05-27 18:03:36.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/ghuser/Ce_Publish.ghuser
+-rw-rw-rw-   0        0        0     3379 2024-05-27 18:03:36.000000 compas_eve-1.0.0/src/compas_eve/ghpython/components/ghuser/Ce_Subscribe.ghuser
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/memory/
+-rw-rw-rw-   0        0        0     3547 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/memory/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve/mqtt/
+-rw-rw-rw-   0        0        0      504 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/mqtt/__init__.py
+-rw-rw-rw-   0        0        0     5254 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/mqtt/mqtt_cli.py
+-rw-rw-rw-   0        0        0     5313 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/mqtt/mqtt_paho.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.685654 compas_eve-1.0.0/src/compas_eve/mqtt/netlib/
+-rw-rw-rw-   0        0        0   303104 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/mqtt/netlib/MQTTnet.dll
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.685654 compas_eve-1.0.0/src/compas_eve/rhino/
+-rw-rw-rw-   0        0        0        0 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/rhino/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-05-27 18:01:43.000000 compas_eve-1.0.0/src/compas_eve/rhino/install.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:03:39.670027 compas_eve-1.0.0/src/compas_eve.egg-info/
+-rw-rw-rw-   0        0        0     3149 2024-05-27 18:03:39.000000 compas_eve-1.0.0/src/compas_eve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2024-05-27 18:03:39.000000 compas_eve-1.0.0/src/compas_eve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:03:39.000000 compas_eve-1.0.0/src/compas_eve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-27 18:01:58.000000 compas_eve-1.0.0/src/compas_eve.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2024-05-27 18:03:39.000000 compas_eve-1.0.0/src/compas_eve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 18:03:39.000000 compas_eve-1.0.0/src/compas_eve.egg-info/top_level.txt
```

### Comparing `compas_eve-0.5.0/CHANGELOG.md` & `compas_eve-1.0.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.0] 2024-05-27
+
+### Added
+
+* Add Grasshopper components for publishing and subscribing to topics, for creating messages and connecting to MQTT transports.
+
+### Changed
+
+### Removed
+
+
 ## [0.5.0] 2024-05-01
 
 ### Added
 
 ### Changed
 
 * Fix/add json serialization support to `Message` class.
```

### Comparing `compas_eve-0.5.0/LICENSE` & `compas_eve-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/PKG-INFO` & `compas_eve-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_eve
-Version: 0.5.0
+Version: 1.0.0
 Summary: COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.
 Home-page: https://github.com/compas-dev/compas_eve
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_eve-0.5.0/README.md` & `compas_eve-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/pyproject.toml` & `compas_eve-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/setup.py` & `compas_eve-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="compas_eve",
-    version="0.5.0",
+    version="1.0.0",
     description="COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/compas-dev/compas_eve",
     author="Gonzalo Casas",
     author_email="casas@arch.ethz.ch",
     license="MIT license",
```

### Comparing `compas_eve-0.5.0/src/compas_eve/__init__.py` & `compas_eve-1.0.0/src/compas_eve/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import os
 
 
 __author__ = ["Gonzalo Casas"]
 __copyright__ = "Gramazio Kohler Research"
 __license__ = "MIT License"
 __email__ = "casas@arch.ethz.ch"
-__version__ = "0.5.0"
+__version__ = "1.0.0"
 
 from .event_emitter import EventEmitterMixin  # noqa: F401 needed here to avoid circular import on py2.7
 from .core import (
     Message,
     Publisher,
     Subscriber,
     EchoSubscriber,
```

### Comparing `compas_eve-0.5.0/src/compas_eve/core.py` & `compas_eve-1.0.0/src/compas_eve/core.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/event_emitter.py` & `compas_eve-1.0.0/src/compas_eve/event_emitter.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/ghpython/background.py` & `compas_eve-1.0.0/src/compas_eve/ghpython/background.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py` & `compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Background Task component.
 
 Executes a long-running task in the background, while keeping Grasshopper reactive.
 
-COMPAS EVE v0.5.0
+COMPAS EVE v1.0.0
 """
 
 import threading
 import scriptcontext as sc
 
 from compas_eve.ghpython import BackgroundWorker
 from ghpythonlib.componentbase import executingcomponent as component
```

### Comparing `compas_eve-0.5.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json` & `compas_eve-1.0.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/memory/__init__.py` & `compas_eve-1.0.0/src/compas_eve/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/mqtt/mqtt_cli.py` & `compas_eve-1.0.0/src/compas_eve/mqtt/mqtt_cli.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/mqtt/mqtt_paho.py` & `compas_eve-1.0.0/src/compas_eve/mqtt/mqtt_paho.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/mqtt/netlib/MQTTnet.dll` & `compas_eve-1.0.0/src/compas_eve/mqtt/netlib/MQTTnet.dll`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve/rhino/install.py` & `compas_eve-1.0.0/src/compas_eve/rhino/install.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.5.0/src/compas_eve.egg-info/PKG-INFO` & `compas_eve-1.0.0/src/compas_eve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas-eve
-Version: 0.5.0
+Version: 1.0.0
 Summary: COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.
 Home-page: https://github.com/compas-dev/compas_eve
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_eve-0.5.0/src/compas_eve.egg-info/SOURCES.txt` & `compas_eve-1.0.0/src/compas_eve.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,31 @@
 src/compas_eve.egg-info/top_level.txt
 src/compas_eve/ghpython/__init__.py
 src/compas_eve/ghpython/background.py
 src/compas_eve/ghpython/components/___init__.py
 src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py
 src/compas_eve/ghpython/components/Ce_BackgroundTask/icon.png
 src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json
+src/compas_eve/ghpython/components/Ce_Message/code.py
+src/compas_eve/ghpython/components/Ce_Message/icon.png
+src/compas_eve/ghpython/components/Ce_Message/metadata.json
+src/compas_eve/ghpython/components/Ce_MqttConnect/code.py
+src/compas_eve/ghpython/components/Ce_MqttConnect/icon.png
+src/compas_eve/ghpython/components/Ce_MqttConnect/metadata.json
+src/compas_eve/ghpython/components/Ce_Publish/code.py
+src/compas_eve/ghpython/components/Ce_Publish/icon.png
+src/compas_eve/ghpython/components/Ce_Publish/metadata.json
+src/compas_eve/ghpython/components/Ce_Subscribe/code.py
+src/compas_eve/ghpython/components/Ce_Subscribe/icon.png
+src/compas_eve/ghpython/components/Ce_Subscribe/metadata.json
 src/compas_eve/ghpython/components/ghuser/Ce_BackgroundTask.ghuser
+src/compas_eve/ghpython/components/ghuser/Ce_Message.ghuser
+src/compas_eve/ghpython/components/ghuser/Ce_MqttConnect.ghuser
+src/compas_eve/ghpython/components/ghuser/Ce_Publish.ghuser
+src/compas_eve/ghpython/components/ghuser/Ce_Subscribe.ghuser
 src/compas_eve/memory/__init__.py
 src/compas_eve/mqtt/__init__.py
 src/compas_eve/mqtt/mqtt_cli.py
 src/compas_eve/mqtt/mqtt_paho.py
 src/compas_eve/mqtt/netlib/MQTTnet.dll
 src/compas_eve/rhino/__init__.py
 src/compas_eve/rhino/install.py
```

