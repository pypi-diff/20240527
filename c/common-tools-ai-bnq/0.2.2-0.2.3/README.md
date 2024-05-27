# Comparing `tmp/common-tools-ai-bnq-0.2.2.tar.gz` & `tmp/common-tools-ai-bnq-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.2.2.tar", last modified: Mon May 20 09:49:51 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.2.3.tar", last modified: Mon May 27 08:50:59 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.2.2.tar` & `common-tools-ai-bnq-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 09:49:51.579415 common-tools-ai-bnq-0.2.2/
--rw-rw-rw-   0        0        0     3204 2024-05-20 09:49:51.579415 common-tools-ai-bnq-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2977 2024-05-17 08:21:09.000000 common-tools-ai-bnq-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 09:49:51.563768 common-tools-ai-bnq-0.2.2/bnq_py_core/
--rw-rw-rw-   0        0        0      412 2024-05-14 03:05:23.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/cos_connect.py
--rw-rw-rw-   0        0        0     7798 2024-05-20 09:49:49.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     1574 2024-05-20 08:46:33.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:49:51.563768 common-tools-ai-bnq-0.2.2/bnq_py_core/utils/
--rw-rw-rw-   0        0        0      122 2024-05-20 08:34:05.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/utils/__init__.py
--rw-rw-rw-   0        0        0      662 2024-05-20 08:39:57.000000 common-tools-ai-bnq-0.2.2/bnq_py_core/utils/time_zone.py
-drwxrwxrwx   0        0        0        0 2024-05-20 09:49:51.579415 common-tools-ai-bnq-0.2.2/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0     3204 2024-05-20 09:49:51.000000 common-tools-ai-bnq-0.2.2/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-20 09:49:51.000000 common-tools-ai-bnq-0.2.2/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 09:49:51.000000 common-tools-ai-bnq-0.2.2/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-20 09:49:51.000000 common-tools-ai-bnq-0.2.2/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-20 09:49:51.000000 common-tools-ai-bnq-0.2.2/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 09:49:51.579415 common-tools-ai-bnq-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      881 2024-05-20 09:49:45.000000 common-tools-ai-bnq-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:50:59.347051 common-tools-ai-bnq-0.2.3/
+-rw-rw-rw-   0        0        0     3204 2024-05-27 08:50:59.346051 common-tools-ai-bnq-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2977 2024-05-17 08:21:09.000000 common-tools-ai-bnq-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 08:50:59.324058 common-tools-ai-bnq-0.2.3/bnq_py_core/
+-rw-rw-rw-   0        0        0      412 2024-05-14 03:05:23.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-05-06 07:47:07.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/cos_connect.py
+-rw-rw-rw-   0        0        0     7938 2024-05-27 08:50:02.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     3218 2024-05-06 09:03:26.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     1574 2024-05-20 08:46:33.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:50:59.330058 common-tools-ai-bnq-0.2.3/bnq_py_core/utils/
+-rw-rw-rw-   0        0        0      122 2024-05-20 08:34:05.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/utils/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-20 08:39:57.000000 common-tools-ai-bnq-0.2.3/bnq_py_core/utils/time_zone.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:50:59.346051 common-tools-ai-bnq-0.2.3/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0     3204 2024-05-27 08:50:59.000000 common-tools-ai-bnq-0.2.3/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-27 08:50:59.000000 common-tools-ai-bnq-0.2.3/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 08:50:59.000000 common-tools-ai-bnq-0.2.3/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-27 08:50:59.000000 common-tools-ai-bnq-0.2.3/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 08:50:59.000000 common-tools-ai-bnq-0.2.3/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 08:50:59.347051 common-tools-ai-bnq-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      881 2024-05-27 03:58:49.000000 common-tools-ai-bnq-0.2.3/setup.py
```

### Comparing `common-tools-ai-bnq-0.2.2/PKG-INFO` & `common-tools-ai-bnq-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common tools of AI module for BNQ
 Home-page: UNKNOWN
 Author: BNQ
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common-tools-ai-bnq-0.2.2/README.md` & `common-tools-ai-bnq-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.2.2/bnq_py_core/cos_connect.py` & `common-tools-ai-bnq-0.2.3/bnq_py_core/cos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.2.2/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.2.3/bnq_py_core/logger_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from termcolor import colored
 
 from .utils.time_zone import BeijingFormatter
 
 
 class _LoggingF(object):
     """
-    日志记录父类
+    日志记录父类, 用于记录运行中的信息
     """
 
     def __init__(self, log_dir=None, max_bytes=20 * 1024 * 1024, backup_count=10, log_level=logging.INFO):
         self.record_info = None
         self.logger = None
         self.log_record_path = log_dir  # 日志记录路径
         self.max_bytes = max_bytes  # 日志文件大小
@@ -64,24 +64,27 @@
                     "class": "concurrent_log_handler.ConcurrentTimedRotatingFileHandler",
                     "filename": log_filename,
                     "when": "midnight",
                     "maxBytes": self.max_bytes,
                     "backupCount": self.backup_count,
                     "encoding": "UTF-8"
                 },
+                'null': {
+                    'class': 'logging.NullHandler',
+                },
             },
             "loggers": {
                 "BNQ-AI": {
-                    "handlers": ["console_handler"],
+                    "handlers": ["console_handler", "file_handler"],
                     "level": self.level
                 }
             },
             "root": {
                 "level": self.level,
-                "handlers": ["file_handler"]
+                "handlers": ["null"]
             }
         }
 
 
 class LoggingRecord(_LoggingF):
     """日志记录类，用于记录运行中的信息
```

### Comparing `common-tools-ai-bnq-0.2.2/bnq_py_core/nacos_connect.py` & `common-tools-ai-bnq-0.2.3/bnq_py_core/nacos_connect.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.2.2/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.2.3/bnq_py_core/read_conf_from_ini.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.2.2/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.2.3/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.2.2/bnq_py_core/utils/time_zone.py` & `common-tools-ai-bnq-0.2.3/bnq_py_core/utils/time_zone.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.2.2/common_tools_ai_bnq.egg-info/PKG-INFO` & `common-tools-ai-bnq-0.2.3/common_tools_ai_bnq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-tools-ai-bnq
-Version: 0.2.2
+Version: 0.2.3
 Summary: Common tools of AI module for BNQ
 Home-page: UNKNOWN
 Author: BNQ
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `common-tools-ai-bnq-0.2.2/setup.py` & `common-tools-ai-bnq-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.25',
         'nacos-sdk-python==0.1.12',
         'PyYAML==6.0.1',
```

