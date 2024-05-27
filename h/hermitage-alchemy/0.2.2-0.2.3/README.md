# Comparing `tmp/hermitage_alchemy-0.2.2.tar.gz` & `tmp/hermitage_alchemy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.2.2.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.2.3.tar", max compression
```

## Comparing `hermitage_alchemy-0.2.2.tar` & `hermitage_alchemy-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.2/README.md
--rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.2/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10439 2024-05-27 14:15:43.102033 hermitage_alchemy-0.2.2/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.2/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     6852 2024-05-25 14:24:50.956155 hermitage_alchemy-0.2.2/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.2/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.2.2/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.2/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.2/hermitage_alchemy/execution/read.py
--rw-r--r--   0        0        0     1165 2024-05-25 14:24:50.957584 hermitage_alchemy-0.2.2/hermitage_alchemy/execution/write.py
--rw-r--r--   0        0        0      438 2024-05-27 14:15:43.092735 hermitage_alchemy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.3/README.md
+-rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.3/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10439 2024-05-27 14:15:43.102033 hermitage_alchemy-0.2.3/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.3/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     6852 2024-05-25 14:24:50.956155 hermitage_alchemy-0.2.3/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.3/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.2.3/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.3/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.3/hermitage_alchemy/execution/read.py
+-rw-r--r--   0        0        0     1165 2024-05-25 14:24:50.957584 hermitage_alchemy-0.2.3/hermitage_alchemy/execution/write.py
+-rw-r--r--   0        0        0      415 2024-05-27 14:17:46.411863 hermitage_alchemy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.3/PKG-INFO
```

### Comparing `hermitage_alchemy-0.2.2/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.2.3/hermitage_alchemy/assembling.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.2/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.2.3/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.2/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.2.3/hermitage_alchemy/configuration.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.2/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.2.3/hermitage_alchemy/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.2/hermitage_alchemy/execution/read.py` & `hermitage_alchemy-0.2.3/hermitage_alchemy/execution/read.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.2/hermitage_alchemy/execution/write.py` & `hermitage_alchemy-0.2.3/hermitage_alchemy/execution/write.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.2/PKG-INFO` & `hermitage_alchemy-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: hermitage-alchemy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Implementation of hermitage contracts for sqlalchemy engine
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: hermitage (>=0.2.0,<0.3.0)
 Requires-Dist: sqlalchemy (>=2.0.20,<3.0.0)
-Requires-Dist: streamlord (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Hermitage Alchemy
 
 Implementation of [hermitage](https://github.com/smairon/hermitage) contracts for sqlalchemy engine
```

