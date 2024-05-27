# Comparing `tmp/autoutils_log-0.1.0.tar.gz` & `tmp/autoutils_log-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoutils_log-0.1.0.tar", max compression
+gzip compressed data, was "autoutils_log-0.2.0.tar", max compression
```

## Comparing `autoutils_log-0.1.0.tar` & `autoutils_log-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-05-24 09:51:08.459971 autoutils_log-0.1.0/LICENSE
--rw-r--r--   0        0        0       15 2024-05-24 19:58:54.498258 autoutils_log-0.1.0/README.md
--rw-r--r--   0        0        0      145 2024-05-24 20:04:31.716923 autoutils_log-0.1.0/autoutils_log/__init__.py
--rw-r--r--   0        0        0     2770 2024-05-24 11:46:55.901305 autoutils_log-0.1.0/autoutils_log/base.py
--rw-r--r--   0        0        0     6239 2024-05-24 20:06:48.732182 autoutils_log-0.1.0/autoutils_log/colorful_stream_handler.py
--rw-r--r--   0        0        0     2039 2024-05-24 21:05:29.602140 autoutils_log-0.1.0/autoutils_log/kafka_handler.py
--rw-r--r--   0        0        0     1263 2024-05-24 11:45:45.476495 autoutils_log-0.1.0/autoutils_log/logstash_handler.py
--rw-r--r--   0        0        0      735 2024-05-24 21:01:34.463028 autoutils_log-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 autoutils_log-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 09:51:08.459971 autoutils_log-0.2.0/LICENSE
+-rw-r--r--   0        0        0       15 2024-05-24 19:58:54.498258 autoutils_log-0.2.0/README.md
+-rw-r--r--   0        0        0      145 2024-05-24 20:04:31.716923 autoutils_log-0.2.0/autoutils_log/__init__.py
+-rw-r--r--   0        0        0     2770 2024-05-24 11:46:55.901305 autoutils_log-0.2.0/autoutils_log/base.py
+-rw-r--r--   0        0        0     6239 2024-05-24 20:06:48.732182 autoutils_log-0.2.0/autoutils_log/colorful_stream_handler.py
+-rw-r--r--   0        0        0     1804 2024-05-27 21:03:17.926701 autoutils_log-0.2.0/autoutils_log/kafka_handler.py
+-rw-r--r--   0        0        0     1263 2024-05-24 11:45:45.476495 autoutils_log-0.2.0/autoutils_log/logstash_handler.py
+-rw-r--r--   0        0        0      740 2024-05-27 21:03:18.958720 autoutils_log-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 autoutils_log-0.2.0/PKG-INFO
```

### Comparing `autoutils_log-0.1.0/LICENSE` & `autoutils_log-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.1.0/autoutils_log/base.py` & `autoutils_log-0.2.0/autoutils_log/base.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.1.0/autoutils_log/colorful_stream_handler.py` & `autoutils_log-0.2.0/autoutils_log/colorful_stream_handler.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.1.0/autoutils_log/logstash_handler.py` & `autoutils_log-0.2.0/autoutils_log/logstash_handler.py`

 * *Files identical despite different names*

### Comparing `autoutils_log-0.1.0/pyproject.toml` & `autoutils_log-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoutils-log"
-version = "0.1.0"
+version = "0.2.0"
 description = "Some Good Function For Log"
 authors = ["Reza Zeiny <rezazeiny1998@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rezazeiny/autoutils-log"
 repository = "https://github.com/rezazeiny/autoutils-log"
 keywords = ["autoutils_log"]
@@ -19,13 +19,13 @@
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pytz = "*"
 termcolor = ">=2.4.0"
 requests = "~=2.32"
 persiantools = "~=4.0"
-aiokafka = "^0.10.0"
+confluent-kafka = "~=2.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autoutils_log-0.1.0/PKG-INFO` & `autoutils_log-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: autoutils-log
-Version: 0.1.0
+Version: 0.2.0
 Summary: Some Good Function For Log
 Home-page: https://github.com/rezazeiny/autoutils-log
 License: MIT
 Keywords: autoutils_log
 Author: Reza Zeiny
 Author-email: rezazeiny1998@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiokafka (>=0.10.0,<0.11.0)
+Requires-Dist: confluent-kafka (>=2.4,<3.0)
 Requires-Dist: persiantools (>=4.0,<5.0)
 Requires-Dist: pytz
 Requires-Dist: requests (>=2.32,<3.0)
 Requires-Dist: termcolor (>=2.4.0)
 Project-URL: Repository, https://github.com/rezazeiny/autoutils-log
 Description-Content-Type: text/markdown
```

