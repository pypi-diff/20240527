# Comparing `tmp/py-seal-0.0.3.tar.gz` & `tmp/py-seal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-seal-0.0.3.tar", last modified: Mon May 27 13:55:45 2024, max compression
+gzip compressed data, was "py-seal-0.0.4.tar", last modified: Mon May 27 14:00:12 2024, max compression
```

## Comparing `py-seal-0.0.3.tar` & `py-seal-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.664922 py-seal-0.0.3/
--rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.3/LICENSE
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-27 13:55:45.664746 py-seal-0.0.3/PKG-INFO
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.660079 py-seal-0.0.3/py-seal/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:53:59.000000 py-seal-0.0.3/py-seal/__init__.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.660360 py-seal-0.0.3/py-seal/config/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:28.000000 py-seal-0.0.3/py-seal/config/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      309 2024-05-27 11:24:33.000000 py-seal-0.0.3/py-seal/config/config.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.660655 py-seal-0.0.3/py-seal/context/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:22.000000 py-seal-0.0.3/py-seal/context/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      621 2024-05-27 11:28:12.000000 py-seal-0.0.3/py-seal/context/context.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.660988 py-seal-0.0.3/py-seal/db/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.3/py-seal/db/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.3/py-seal/db/connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.661883 py-seal-0.0.3/py-seal/db/mysql/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.3/py-seal/db/mysql/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)    10061 2024-05-27 11:28:12.000000 py-seal-0.0.3/py-seal/db/mysql/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6655 2024-05-27 11:28:12.000000 py-seal-0.0.3/py-seal/db/mysql/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      722 2024-05-27 11:28:24.000000 py-seal-0.0.3/py-seal/db/mysql/mysql_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.662726 py-seal-0.0.3/py-seal/db/sqlite/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.3/py-seal/db/sqlite/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     9496 2024-05-27 11:28:12.000000 py-seal-0.0.3/py-seal/db/sqlite/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6388 2024-05-27 11:28:12.000000 py-seal-0.0.3/py-seal/db/sqlite/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      285 2024-05-27 11:29:16.000000 py-seal-0.0.3/py-seal/db/sqlite/sqlite_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.663216 py-seal-0.0.3/py-seal/model/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:05.000000 py-seal-0.0.3/py-seal/model/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.3/py-seal/model/base_entity.py
--rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.3/py-seal/model/response.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.663592 py-seal-0.0.3/py-seal/router/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:10.000000 py-seal-0.0.3/py-seal/router/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     2194 2024-05-27 11:25:37.000000 py-seal-0.0.3/py-seal/router/router.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.663892 py-seal-0.0.3/py-seal/wrapper/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:34.000000 py-seal-0.0.3/py-seal/wrapper/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     1096 2024-05-26 00:54:07.000000 py-seal-0.0.3/py-seal/wrapper/decorator.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 13:55:45.664524 py-seal-0.0.3/py_seal.egg-info/
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-27 13:55:45.000000 py-seal-0.0.3/py_seal.egg-info/PKG-INFO
--rw-r--r--   0 yehao      (501) staff       (20)      771 2024-05-27 13:55:45.000000 py-seal-0.0.3/py_seal.egg-info/SOURCES.txt
--rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-27 13:55:45.000000 py-seal-0.0.3/py_seal.egg-info/dependency_links.txt
--rw-r--r--   0 yehao      (501) staff       (20)        8 2024-05-27 13:55:45.000000 py-seal-0.0.3/py_seal.egg-info/top_level.txt
--rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-27 13:55:45.664982 py-seal-0.0.3/setup.cfg
--rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-27 13:46:46.000000 py-seal-0.0.3/setup.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.840067 py-seal-0.0.4/
+-rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.4/LICENSE
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-27 14:00:12.839873 py-seal-0.0.4/PKG-INFO
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.833027 py-seal-0.0.4/py_seal.egg-info/
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-27 14:00:12.000000 py-seal-0.0.4/py_seal.egg-info/PKG-INFO
+-rw-r--r--   0 yehao      (501) staff       (20)      705 2024-05-27 14:00:12.000000 py-seal-0.0.4/py_seal.egg-info/SOURCES.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-27 14:00:12.000000 py-seal-0.0.4/py_seal.egg-info/dependency_links.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        5 2024-05-27 14:00:12.000000 py-seal-0.0.4/py_seal.egg-info/top_level.txt
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.833217 py-seal-0.0.4/seal/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:53:59.000000 py-seal-0.0.4/seal/__init__.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.833510 py-seal-0.0.4/seal/config/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:28.000000 py-seal-0.0.4/seal/config/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      309 2024-05-27 11:24:33.000000 py-seal-0.0.4/seal/config/config.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.833794 py-seal-0.0.4/seal/context/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:22.000000 py-seal-0.0.4/seal/context/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      621 2024-05-27 11:28:12.000000 py-seal-0.0.4/seal/context/context.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.834142 py-seal-0.0.4/seal/db/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.4/seal/db/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.4/seal/db/connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.834995 py-seal-0.0.4/seal/db/mysql/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.4/seal/db/mysql/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)    10061 2024-05-27 11:28:12.000000 py-seal-0.0.4/seal/db/mysql/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6655 2024-05-27 11:28:12.000000 py-seal-0.0.4/seal/db/mysql/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      722 2024-05-27 11:28:24.000000 py-seal-0.0.4/seal/db/mysql/mysql_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.837223 py-seal-0.0.4/seal/db/sqlite/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:13.000000 py-seal-0.0.4/seal/db/sqlite/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     9496 2024-05-27 11:28:12.000000 py-seal-0.0.4/seal/db/sqlite/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6388 2024-05-27 11:28:12.000000 py-seal-0.0.4/seal/db/sqlite/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      285 2024-05-27 11:29:16.000000 py-seal-0.0.4/seal/db/sqlite/sqlite_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.838391 py-seal-0.0.4/seal/model/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:05.000000 py-seal-0.0.4/seal/model/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.4/seal/model/base_entity.py
+-rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.4/seal/model/response.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.838878 py-seal-0.0.4/seal/router/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:10.000000 py-seal-0.0.4/seal/router/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     2194 2024-05-27 11:25:37.000000 py-seal-0.0.4/seal/router/router.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-27 14:00:12.839564 py-seal-0.0.4/seal/wrapper/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-27 13:54:34.000000 py-seal-0.0.4/seal/wrapper/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     1096 2024-05-26 00:54:07.000000 py-seal-0.0.4/seal/wrapper/decorator.py
+-rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-27 14:00:12.840139 py-seal-0.0.4/setup.cfg
+-rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-27 14:00:03.000000 py-seal-0.0.4/setup.py
```

### Comparing `py-seal-0.0.3/LICENSE` & `py-seal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/context/context.py` & `py-seal-0.0.4/seal/context/context.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/db/mysql/base_mapper.py` & `py-seal-0.0.4/seal/db/mysql/base_mapper.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/db/mysql/chained_query.py` & `py-seal-0.0.4/seal/db/mysql/chained_query.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/db/mysql/mysql_connector.py` & `py-seal-0.0.4/seal/db/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/db/sqlite/base_mapper.py` & `py-seal-0.0.4/seal/db/sqlite/base_mapper.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/db/sqlite/chained_query.py` & `py-seal-0.0.4/seal/db/sqlite/chained_query.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/model/response.py` & `py-seal-0.0.4/seal/model/response.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/router/router.py` & `py-seal-0.0.4/seal/router/router.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.3/py-seal/wrapper/decorator.py` & `py-seal-0.0.4/seal/wrapper/decorator.py`

 * *Files identical despite different names*

