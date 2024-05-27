# Comparing `tmp/pinecone_plugin_interface-0.0.2.tar.gz` & `tmp/pinecone_plugin_interface-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_plugin_interface-0.0.2.tar", max compression
+gzip compressed data, was "pinecone_plugin_interface-0.0.3.tar", max compression
```

## Comparing `pinecone_plugin_interface-0.0.2.tar` & `pinecone_plugin_interface-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      356 2024-05-27 16:12:57.613224 pinecone_plugin_interface-0.0.2/README.md
--rw-r--r--   0        0        0      712 2024-05-27 16:13:17.417333 pinecone_plugin_interface-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/__init__.py
--rw-r--r--   0        0        0      197 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/__init__.py
--rw-r--r--   0        0        0       37 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/constants.py
--rw-r--r--   0        0        0      571 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/discover_namespace_packages.py
--rw-r--r--   0        0        0     1338 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/discover_plugins.py
--rw-r--r--   0        0        0     1293 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/installation.py
--rw-r--r--   0        0        0      428 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/load_and_install.py
--rw-r--r--   0        0        0       52 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/logging.py
--rw-r--r--   0        0        0      467 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/pinecone_plugin.py
--rw-r--r--   0        0        0     2407 2024-05-27 16:12:57.617224 pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/plugin_metadata.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 pinecone_plugin_interface-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      356 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/README.md
+-rw-r--r--   0        0        0      712 2024-05-27 17:01:05.985943 pinecone_plugin_interface-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/constants.py
+-rw-r--r--   0        0        0      571 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/discover_namespace_packages.py
+-rw-r--r--   0        0        0     1338 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/discover_plugins.py
+-rw-r--r--   0        0        0     1293 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/installation.py
+-rw-r--r--   0        0        0      428 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/load_and_install.py
+-rw-r--r--   0        0        0       52 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/logging.py
+-rw-r--r--   0        0        0      467 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/pinecone_plugin.py
+-rw-r--r--   0        0        0     2407 2024-05-27 17:00:51.101600 pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/plugin_metadata.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 pinecone_plugin_interface-0.0.3/PKG-INFO
```

### Comparing `pinecone_plugin_interface-0.0.2/pyproject.toml` & `pinecone_plugin_interface-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-plugin-interface"
-version = "0.0.2"
+version = "0.0.3"
 packages = [
     { include="pinecone_plugin_interface", from="src" },
 ]
 description = "Plugin interface for the Pinecone python client"
 authors = ["Pinecone Systems, Inc. <support@pinecone.io>"]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/discover_namespace_packages.py` & `pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/discover_namespace_packages.py`

 * *Files identical despite different names*

### Comparing `pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/discover_plugins.py` & `pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/discover_plugins.py`

 * *Files identical despite different names*

### Comparing `pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/actions/installation.py` & `pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/actions/installation.py`

 * *Files identical despite different names*

### Comparing `pinecone_plugin_interface-0.0.2/src/pinecone_plugin_interface/plugin_metadata.py` & `pinecone_plugin_interface-0.0.3/src/pinecone_plugin_interface/plugin_metadata.py`

 * *Files identical despite different names*

### Comparing `pinecone_plugin_interface-0.0.2/PKG-INFO` & `pinecone_plugin_interface-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-plugin-interface
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plugin interface for the Pinecone python client
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

