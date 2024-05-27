# Comparing `tmp/astro_extras-0.1.5.tar.gz` & `tmp/astro_extras-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.1.5.tar", last modified: Sat May 25 13:38:13 2024, max compression
+gzip compressed data, was "astro_extras-0.1.5.1.tar", last modified: Mon May 27 10:57:08 2024, max compression
```

## Comparing `astro_extras-0.1.5.tar` & `astro_extras-0.1.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.371923 astro_extras-0.1.5/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.5/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.5/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-25 13:38:13.371923 astro_extras-0.1.5/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.5/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.5/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-22 07:52:04.000000 astro_extras-0.1.5/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-25 13:38:13.371923 astro_extras-0.1.5/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-25 13:37:40.000000 astro_extras-0.1.5/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.351923 astro_extras-0.1.5/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.351923 astro_extras-0.1.5/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-25 13:37:47.000000 astro_extras-0.1.5/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.363923 astro_extras-0.1.5/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.363923 astro_extras-0.1.5/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.5/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    54346 2024-05-25 13:30:53.000000 astro_extras-0.1.5/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.5/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.5/src/astro_extras/sensors/auto.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.5/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras/templates/
--rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/session_close.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/session_open.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.5/src/astro_extras/templates/table_actuals_select.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/table_timed_update.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/table_transfer_nosess.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/templates/table_transfer_sess.sql
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.5/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.5/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/utils/postgres_sql.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.5/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.5/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-25 13:38:13.000000 astro_extras-0.1.5/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-25 13:38:13.367923 astro_extras-0.1.5/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.5/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.5/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.5/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.5/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.5.1/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7922 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.5.1/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-26 09:28:01.000000 astro_extras-0.1.5.1/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1195 2024-05-27 10:52:04.000000 astro_extras-0.1.5.1/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.444975 astro_extras-0.1.5.1/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.448975 astro_extras-0.1.5.1/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1208 2024-05-27 10:52:15.000000 astro_extras-0.1.5.1/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.464974 astro_extras-0.1.5.1/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.464974 astro_extras-0.1.5.1/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.5.1/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    54666 2024-05-27 10:52:47.000000 astro_extras-0.1.5.1/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.464974 astro_extras-0.1.5.1/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.5.1/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.5.1/src/astro_extras/sensors/auto.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.5.1/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.476975 astro_extras-0.1.5.1/src/astro_extras/templates/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/session_close.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/session_open.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_actuals_select.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_timed_update.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_transfer_nosess.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_transfer_sess.sql
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.476975 astro_extras-0.1.5.1/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.5.1/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.5.1/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/utils/postgres_sql.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.5.1/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7922 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.476975 astro_extras-0.1.5.1/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.5.1/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.5.1/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.5.1/tests/test_utils.py
```

### Comparing `astro_extras-0.1.5/LICENSE` & `astro_extras-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/PKG-INFO` & `astro_extras-0.1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-airflow[pandas,postgres]>=2.7.0
-Requires-Dist: astro-sdk-python[postgres]>=1.6.0
+Requires-Dist: astro-sdk-python[postgres]==1.8.0
 Requires-Dist: openlineage-python>=1.14.0
 Requires-Dist: openpyxl>=3.0.0
 Requires-Dist: python-dateutil>=2.8.0
 
 # Astro SDK extras project
 
 We've been using [Apache Airflow](https://airflow.apache.org/docs/apache-airflow/stable/)
```

### Comparing `astro_extras-0.1.5/README.md` & `astro_extras-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/setup.py` & `astro_extras-0.1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.1.5",
+    version="0.1.5.1",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.1.5/src/astro_extras/__init__.py` & `astro_extras-0.1.5.1/src/astro_extras/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.1.5'
+__version__ = '0.1.5.1'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
```

### Comparing `astro_extras-0.1.5/src/astro_extras/operators/direct.py` & `astro_extras-0.1.5.1/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/operators/session.py` & `astro_extras-0.1.5.1/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/operators/table.py` & `astro_extras-0.1.5.1/src/astro_extras/operators/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 """ Table operations """
 
 import logging
 import warnings
 import pandas as pd
 from functools import cached_property
-from sqlalchemy import text, Table as SqlaTable, Integer, BigInteger, SmallInteger
+from sqlalchemy import Table as SqlaTable, MetaData as SqlaMetadata
+from sqlalchemy import text, Integer, BigInteger, SmallInteger
 from sqlalchemy.engine.base import Connection as SqlaConnection
 from sqlalchemy.exc import InvalidRequestError as SqlaInvalidRequestError
 
 from airflow.models.dag import DagContext
 from airflow.utils.context import Context
 from airflow.models.xcom_arg import XComArg
 from airflow.utils.task_group import TaskGroup
@@ -168,19 +169,22 @@
         if self.source_conn_id == self.destination_conn_id and self.source_table == self.destination_table:
             raise AirflowFailException('Source and destination must not be the same')
 
         self._pre_execute_called = True
 
     def _load_table_def(self, base_table: BaseTable, db: BaseDatabase) -> BaseTable:
         """ Internal - load single table definition """
+        # Use base_table's SQLA metadata to retrieve table columns from database
+        # There's something that looks like a bug in SQLA - 
+        # only lower-case schema/table names could be used with reflect
         try:
-            # Use base_table's SQLA metadata to retrieve table columns from database
-            full_name = db.get_table_qualified_name(base_table)
-            meta = base_table.sqlalchemy_metadata
-            meta.reflect(bind=db.connection, only=[base_table.name])
+            full_name = db.get_table_qualified_name(base_table).lower()
+            meta = SqlaMetadata(schema=base_table.metadata.schema.lower() \
+                                if base_table.metadata and base_table.metadata.schema else None)
+            meta.reflect(bind=db.connection, only=[base_table.name.lower()])
         except SqlaInvalidRequestError as ex:
             self.log.error(f'Could not load table {full_name} structure on {db.conn_id}')
             return base_table
 
         if (sqla_table := meta.tables.get(full_name, None)) is None:
             self.log.error(f'Could not find table {full_name} on {db.conn_id}')
             return base_table
```

### Comparing `astro_extras-0.1.5/src/astro_extras/sensors/auto.py` & `astro_extras-0.1.5.1/src/astro_extras/sensors/auto.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/sensors/file.py` & `astro_extras-0.1.5.1/src/astro_extras/sensors/file.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/templates/table_actuals_select.sql` & `astro_extras-0.1.5.1/src/astro_extras/templates/table_actuals_select.sql`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/utils/data_compare.py` & `astro_extras-0.1.5.1/src/astro_extras/utils/data_compare.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.1.5.1/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/utils/postgres_sql.py` & `astro_extras-0.1.5.1/src/astro_extras/utils/postgres_sql.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/utils/template.py` & `astro_extras-0.1.5.1/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras/utils/utils.py` & `astro_extras-0.1.5.1/src/astro_extras/utils/utils.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.1.5.1/src/astro_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-airflow[pandas,postgres]>=2.7.0
-Requires-Dist: astro-sdk-python[postgres]>=1.6.0
+Requires-Dist: astro-sdk-python[postgres]==1.8.0
 Requires-Dist: openlineage-python>=1.14.0
 Requires-Dist: openpyxl>=3.0.0
 Requires-Dist: python-dateutil>=2.8.0
 
 # Astro SDK extras project
 
 We've been using [Apache Airflow](https://airflow.apache.org/docs/apache-airflow/stable/)
```

### Comparing `astro_extras-0.1.5/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.1.5.1/src/astro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/tests/test_session.py` & `astro_extras-0.1.5.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/tests/test_table.py` & `astro_extras-0.1.5.1/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/tests/test_templates.py` & `astro_extras-0.1.5.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5/tests/test_utils.py` & `astro_extras-0.1.5.1/tests/test_utils.py`

 * *Files identical despite different names*

