# Comparing `tmp/dragonion_core-0.1.0.tar.gz` & `tmp/dragonion_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonion_core-0.1.0.tar", max compression
+gzip compressed data, was "dragonion_core-0.1.1.tar", max compression
```

## Comparing `dragonion_core-0.1.0.tar` & `dragonion_core-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        6 2023-07-16 20:50:07.573995 dragonion_core-0.1.0/dragonion_core/__init__.py
--rw-r--r--   0        0        0        6 2023-07-16 20:30:25.007355 dragonion_core-0.1.0/dragonion_core/proto/__init__.py
--rw-r--r--   0        0        0        6 2023-07-13 20:47:53.565137 dragonion_core-0.1.0/dragonion_core/proto/encryption/__init__.py
--rw-r--r--   0        0        0     1677 2023-07-21 17:46:43.162894 dragonion_core-0.1.0/dragonion_core/proto/encryption/identity.py
--rw-r--r--   0        0        0       64 2023-07-16 20:46:21.681187 dragonion_core-0.1.0/dragonion_core/proto/file/__init__.py
--rw-r--r--   0        0        0      534 2023-07-25 18:13:08.566362 dragonion_core-0.1.0/dragonion_core/proto/file/auth.py
--rw-r--r--   0        0        0        6 2023-07-17 12:09:01.714784 dragonion_core-0.1.0/dragonion_core/proto/web/__init__.py
--rw-r--r--   0        0        0      852 2023-07-26 13:50:16.107966 dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/__init__.py
--rw-r--r--   0        0        0     1053 2023-07-27 15:58:01.695965 dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/connection.py
--rw-r--r--   0        0        0     2502 2023-07-27 15:56:22.754575 dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/message.py
--rw-r--r--   0        0        0      808 2023-07-26 13:43:27.783199 dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/server.py
--rw-r--r--   0        0        0     2499 2023-07-27 15:56:09.294722 dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/webmessage.py
--rw-r--r--   0        0        0      489 2023-07-22 11:55:26.022266 dragonion_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      171 2023-07-16 20:27:39.741787 dragonion_core-0.1.0/README.md
--rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 dragonion_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-07-16 20:50:07.573995 dragonion_core-0.1.1/dragonion_core/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-16 20:30:25.007355 dragonion_core-0.1.1/dragonion_core/proto/__init__.py
+-rw-r--r--   0        0        0        6 2023-07-13 20:47:53.565137 dragonion_core-0.1.1/dragonion_core/proto/encryption/__init__.py
+-rw-r--r--   0        0        0     1677 2023-07-21 17:46:43.162894 dragonion_core-0.1.1/dragonion_core/proto/encryption/identity.py
+-rw-r--r--   0        0        0       64 2023-07-16 20:46:21.681187 dragonion_core-0.1.1/dragonion_core/proto/file/__init__.py
+-rw-r--r--   0        0        0      534 2023-07-25 18:13:08.566362 dragonion_core-0.1.1/dragonion_core/proto/file/auth.py
+-rw-r--r--   0        0        0        6 2023-07-17 12:09:01.714784 dragonion_core-0.1.1/dragonion_core/proto/web/__init__.py
+-rw-r--r--   0        0        0      852 2023-07-26 13:50:16.107966 dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/__init__.py
+-rw-r--r--   0        0        0     1053 2023-07-27 15:58:01.695965 dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/connection.py
+-rw-r--r--   0        0        0     2502 2023-07-27 15:56:22.754575 dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/message.py
+-rw-r--r--   0        0        0      808 2023-07-26 13:43:27.783199 dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/server.py
+-rw-r--r--   0        0        0     2499 2023-07-27 15:56:09.294722 dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/webmessage.py
+-rw-r--r--   0        0        0      489 2024-05-27 13:22:04.435776 dragonion_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      181 2024-05-27 13:13:37.431434 dragonion_core-0.1.1/README.md
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 dragonion_core-0.1.1/PKG-INFO
```

### Comparing `dragonion_core-0.1.0/dragonion_core/proto/encryption/identity.py` & `dragonion_core-0.1.1/dragonion_core/proto/encryption/identity.py`

 * *Files identical despite different names*

### Comparing `dragonion_core-0.1.0/dragonion_core/proto/file/auth.py` & `dragonion_core-0.1.1/dragonion_core/proto/file/auth.py`

 * *Files identical despite different names*

### Comparing `dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/__init__.py` & `dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/connection.py` & `dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/connection.py`

 * *Files identical despite different names*

### Comparing `dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/message.py` & `dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/message.py`

 * *Files identical despite different names*

### Comparing `dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/server.py` & `dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/server.py`

 * *Files identical despite different names*

### Comparing `dragonion_core-0.1.0/dragonion_core/proto/web/webmessage/webmessage.py` & `dragonion_core-0.1.1/dragonion_core/proto/web/webmessage/webmessage.py`

 * *Files identical despite different names*

### Comparing `dragonion_core-0.1.0/PKG-INFO` & `dragonion_core-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dragonion-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: BarsTiger
 Author-email: zxcbarstiger@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: cryptography (>=41.0.2,<42.0.0)
+Requires-Dist: cryptography (>=42.0.7,<43.0.0)
 Requires-Dist: dataclasses-json (>=0.5.13,<0.6.0)
 Requires-Dist: sqlitedict (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # dragonion-core
-Core library for both [[dragonion]](https://github.com/dragonionx/dragonion) and 
-[[dragonion-server]](https://github.com/dragonionx/dragonion-server)
+Core library for both [[dragonion]](https://github.com/kotikotprojects/dragonion) and 
+[[dragonion-server]](https://github.com/kotikotprojects/dragonion-server)
```

