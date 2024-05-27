# Comparing `tmp/logs_ingestion-0.2.2.tar.gz` & `tmp/logs_ingestion-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logs_ingestion-0.2.2.tar", max compression
+gzip compressed data, was "logs_ingestion-0.2.3.tar", max compression
```

## Comparing `logs_ingestion-0.2.2.tar` & `logs_ingestion-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2299 2024-03-31 16:33:10.041001 logs_ingestion-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-03-31 16:33:10.041216 logs_ingestion-0.2.2/logs_ingestion/__init__.py
--rw-r--r--   0        0        0     1902 2024-03-31 16:33:10.041651 logs_ingestion-0.2.2/logs_ingestion/logs_adapter.py
--rw-r--r--   0        0        0     1340 2024-03-31 16:33:10.041874 logs_ingestion-0.2.2/logs_ingestion/logs_decorator.py
--rw-r--r--   0        0        0     2262 2024-04-02 20:37:11.169350 logs_ingestion-0.2.2/logs_ingestion/logs_ingestion.py
--rw-r--r--   0        0        0     1583 2024-04-02 20:34:53.929260 logs_ingestion-0.2.2/logs_ingestion/logs_record.py
--rw-r--r--   0        0        0      570 2024-04-02 20:41:26.007006 logs_ingestion-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 logs_ingestion-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2299 2024-03-31 16:33:10.041001 logs_ingestion-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-31 16:33:10.041216 logs_ingestion-0.2.3/logs_ingestion/__init__.py
+-rw-r--r--   0        0        0     1902 2024-03-31 16:33:10.041651 logs_ingestion-0.2.3/logs_ingestion/logs_adapter.py
+-rw-r--r--   0        0        0     1340 2024-03-31 16:33:10.041874 logs_ingestion-0.2.3/logs_ingestion/logs_decorator.py
+-rw-r--r--   0        0        0     2262 2024-04-02 20:37:11.169350 logs_ingestion-0.2.3/logs_ingestion/logs_ingestion.py
+-rw-r--r--   0        0        0     1583 2024-04-03 12:47:32.468063 logs_ingestion-0.2.3/logs_ingestion/logs_record.py
+-rw-r--r--   0        0        0      570 2024-05-27 08:23:05.723405 logs_ingestion-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 logs_ingestion-0.2.3/PKG-INFO
```

### Comparing `logs_ingestion-0.2.2/README.md` & `logs_ingestion-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.2/logs_ingestion/logs_adapter.py` & `logs_ingestion-0.2.3/logs_ingestion/logs_adapter.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.2/logs_ingestion/logs_decorator.py` & `logs_ingestion-0.2.3/logs_ingestion/logs_decorator.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.2/logs_ingestion/logs_ingestion.py` & `logs_ingestion-0.2.3/logs_ingestion/logs_ingestion.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.2/logs_ingestion/logs_record.py` & `logs_ingestion-0.2.3/logs_ingestion/logs_record.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.2/pyproject.toml` & `logs_ingestion-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "logs-ingestion"
-version = "0.2.2"
+version = "0.2.3"
 description = "Package for logging to Azure Logs Ingestion API using decorators and regular logging statements."
 authors = ["Richard Kooijman <kooijman.richard@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = "2.6.4"
+pydantic = "2.7.1"
 azure-core = "1.30.1"
 azure-identity = "1.15.0"
 azure-monitor-ingestion = "1.0.3"
 
 
 [tool.poetry.group.dev.dependencies]
 databricks-connect = "^14.3.1"
```

### Comparing `logs_ingestion-0.2.2/PKG-INFO` & `logs_ingestion-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: logs-ingestion
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package for logging to Azure Logs Ingestion API using decorators and regular logging statements.
 License: Apache
 Author: Richard Kooijman
 Author-email: kooijman.richard@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: azure-core (==1.30.1)
 Requires-Dist: azure-identity (==1.15.0)
 Requires-Dist: azure-monitor-ingestion (==1.0.3)
-Requires-Dist: pydantic (==2.6.4)
+Requires-Dist: pydantic (==2.7.1)
 Description-Content-Type: text/markdown
 
 ## Introduction
 
 This logs_ingestion package provides several methods for logging data into Azure Monitor using the Logs Ingestion API.
 
 The following attributes are part of the logging with the coding attribute names between brackets:
```

