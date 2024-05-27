# Comparing `tmp/krezi-1.2.tar.gz` & `tmp/krezi-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krezi-1.2.tar", last modified: Mon May 27 02:28:12 2024, max compression
+gzip compressed data, was "krezi-1.3.tar", last modified: Mon May 27 03:19:38 2024, max compression
```

## Comparing `krezi-1.2.tar` & `krezi-1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.819468 krezi-1.2/
--rw-r--r--   0 aadilzikre   (501) staff       (20)     1068 2024-03-30 22:15:56.000000 krezi-1.2/LICENSE
--rw-r--r--   0 aadilzikre   (501) staff       (20)     1198 2024-05-27 02:28:12.819327 krezi-1.2/PKG-INFO
--rw-r--r--   0 aadilzikre   (501) staff       (20)      720 2024-05-27 01:28:30.000000 krezi-1.2/README.md
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.814088 krezi-1.2/krezi/
--rw-r--r--   0 aadilzikre   (501) staff       (20)      862 2024-05-27 00:21:16.000000 krezi-1.2/krezi/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)    16868 2024-05-27 00:57:11.000000 krezi-1.2/krezi/common.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.815512 krezi-1.2/krezi/cover_letter_generator_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:23.000000 krezi-1.2/krezi/cover_letter_generator_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     5515 2024-03-07 18:12:30.000000 krezi-1.2/krezi/cover_letter_generator_util/automated_cover_letter_generator.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.816324 krezi-1.2/krezi/email_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)       61 2024-05-27 01:29:45.000000 krezi-1.2/krezi/email_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     4920 2024-05-27 00:59:46.000000 krezi-1.2/krezi/email_util/email_notifier.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.816693 krezi-1.2/krezi/logging_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:31.000000 krezi-1.2/krezi/logging_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     4343 2024-05-26 17:52:33.000000 krezi-1.2/krezi/logging_util/file_logger.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.817232 krezi-1.2/krezi/mssql_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:36.000000 krezi-1.2/krezi/mssql_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     2595 2023-06-03 16:25:44.000000 krezi-1.2/krezi/mssql_util/pymssql_dao.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.818060 krezi-1.2/krezi/multiprocessing_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:41.000000 krezi-1.2/krezi/multiprocessing_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     3334 2024-03-07 18:09:18.000000 krezi-1.2/krezi/multiprocessing_util/mp_class_util.py
--rwx------   0 aadilzikre   (501) staff       (20)     4598 2023-06-30 14:07:35.000000 krezi-1.2/krezi/multiprocessing_util/mp_util.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.818526 krezi-1.2/krezi/posgresql_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:50.000000 krezi-1.2/krezi/posgresql_util/__init__.py
--rwx------   0 aadilzikre   (501) staff       (20)     3575 2023-06-30 14:07:38.000000 krezi-1.2/krezi/posgresql_util/posgresql_util.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.818861 krezi-1.2/krezi/stopwatch_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:54.000000 krezi-1.2/krezi/stopwatch_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     3732 2024-03-08 20:18:16.000000 krezi-1.2/krezi/stopwatch_util/stopwatch.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.815258 krezi-1.2/krezi.egg-info/
--rw-r--r--   0 aadilzikre   (501) staff       (20)     1198 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/PKG-INFO
--rw-r--r--   0 aadilzikre   (501) staff       (20)      770 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/SOURCES.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)        1 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/dependency_links.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)       48 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/requires.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)        6 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/top_level.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)       38 2024-05-27 02:28:12.819516 krezi-1.2/setup.cfg
--rw-r--r--   0 aadilzikre   (501) staff       (20)      931 2024-05-27 02:28:01.000000 krezi-1.2/setup.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.008230 krezi-1.3/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1068 2024-03-30 22:15:56.000000 krezi-1.3/LICENSE
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1249 2024-05-27 03:19:38.008075 krezi-1.3/PKG-INFO
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      771 2024-05-27 02:32:37.000000 krezi-1.3/README.md
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.001450 krezi-1.3/krezi/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      862 2024-05-27 00:21:16.000000 krezi-1.3/krezi/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)    16868 2024-05-27 00:57:11.000000 krezi-1.3/krezi/common.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.003608 krezi-1.3/krezi/cover_letter_generator_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:23.000000 krezi-1.3/krezi/cover_letter_generator_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     5515 2024-03-07 18:12:30.000000 krezi-1.3/krezi/cover_letter_generator_util/automated_cover_letter_generator.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.004551 krezi-1.3/krezi/email_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       61 2024-05-27 01:29:45.000000 krezi-1.3/krezi/email_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     4920 2024-05-27 00:59:46.000000 krezi-1.3/krezi/email_util/email_notifier.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.004970 krezi-1.3/krezi/logging_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:31.000000 krezi-1.3/krezi/logging_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     4344 2024-05-27 03:18:30.000000 krezi-1.3/krezi/logging_util/file_logger.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.005517 krezi-1.3/krezi/mssql_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:36.000000 krezi-1.3/krezi/mssql_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     2595 2023-06-03 16:25:44.000000 krezi-1.3/krezi/mssql_util/pymssql_dao.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.006469 krezi-1.3/krezi/multiprocessing_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:41.000000 krezi-1.3/krezi/multiprocessing_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     3334 2024-03-07 18:09:18.000000 krezi-1.3/krezi/multiprocessing_util/mp_class_util.py
+-rwx------   0 aadilzikre   (501) staff       (20)     4598 2023-06-30 14:07:35.000000 krezi-1.3/krezi/multiprocessing_util/mp_util.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.007169 krezi-1.3/krezi/posgresql_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:50.000000 krezi-1.3/krezi/posgresql_util/__init__.py
+-rwx------   0 aadilzikre   (501) staff       (20)     3575 2023-06-30 14:07:38.000000 krezi-1.3/krezi/posgresql_util/posgresql_util.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.007487 krezi-1.3/krezi/stopwatch_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:54.000000 krezi-1.3/krezi/stopwatch_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     3732 2024-03-08 20:18:16.000000 krezi-1.3/krezi/stopwatch_util/stopwatch.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.003379 krezi-1.3/krezi.egg-info/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1249 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/PKG-INFO
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      770 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/SOURCES.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        1 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/dependency_links.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       48 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/requires.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        6 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/top_level.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       38 2024-05-27 03:19:38.008281 krezi-1.3/setup.cfg
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      766 2024-05-27 03:19:28.000000 krezi-1.3/setup.py
```

### Comparing `krezi-1.2/LICENSE` & `krezi-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `krezi-1.2/PKG-INFO` & `krezi-1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krezi
-Version: 1.2
+Version: 1.3
 Summary: Array of Utilities for Lazy but Efficient Programmers
 Author: Aadil Zikre
 Author-email: aadilzikre@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -24,8 +24,14 @@
 3. Multiprocessing : to work around GIL and utilize multiple cores/threads. Applicable to Dataframes too.
 4. Emailing : to send email alerts on demand/error.
 5. Stopwatch : to profile scripts. IMO there are better profilers out there. This is just a POC. 
 6. Postgresql : Querying from Postgres Databases.
 7. MSSQL : Querying from Microsoft SQL Server Databases.
 8. Mongo : Querying from Mongo Databases. 
 
+---
+## INSTALLATION
+
+```
+    pip install krezi
+```
```

### Comparing `krezi-1.2/README.md` & `krezi-1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,7 +7,14 @@
 2. Subprocessing : to run commands in terminal.
 3. Multiprocessing : to work around GIL and utilize multiple cores/threads. Applicable to Dataframes too.
 4. Emailing : to send email alerts on demand/error.
 5. Stopwatch : to profile scripts. IMO there are better profilers out there. This is just a POC. 
 6. Postgresql : Querying from Postgres Databases.
 7. MSSQL : Querying from Microsoft SQL Server Databases.
 8. Mongo : Querying from Mongo Databases. 
+
+---
+## INSTALLATION
+
+```
+    pip install krezi
+```
```

### Comparing `krezi-1.2/krezi/__init__.py` & `krezi-1.3/krezi/__init__.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/common.py` & `krezi-1.3/krezi/common.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/cover_letter_generator_util/automated_cover_letter_generator.py` & `krezi-1.3/krezi/cover_letter_generator_util/automated_cover_letter_generator.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/email_util/email_notifier.py` & `krezi-1.3/krezi/email_util/email_notifier.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/logging_util/file_logger.py` & `krezi-1.3/krezi/logging_util/file_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Logger:
     def __init__(self, logger_name=None, add_stream_handler = True, std_err = False, level = 'debug', **kwargs):
         self.logger_name = logger_name if logger_name else __name__
         self.add_stream_handler = add_stream_handler
         self.std_err = std_err
         self.level = self.LEVELS.get(level, logging.INFO)
         self.logger = None
-        self.dt_fmt_basic = kwargs.get('dt_fmt_basic', True)
+        self.dt_fmt_basic = kwargs.get('dt_fmt_basic', False)
     
     LEVELS = {'debug': logging.DEBUG, 'info': logging.INFO, 'warning': logging.WARNING, 'error': logging.ERROR, 'critical': logging.CRITICAL}
     
     @staticmethod
     def remove_handlers(logger):
         while logger.handlers:
             handler = logger.handlers[0]
```

### Comparing `krezi-1.2/krezi/mssql_util/pymssql_dao.py` & `krezi-1.3/krezi/mssql_util/pymssql_dao.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/multiprocessing_util/mp_class_util.py` & `krezi-1.3/krezi/multiprocessing_util/mp_class_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/multiprocessing_util/mp_util.py` & `krezi-1.3/krezi/multiprocessing_util/mp_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/posgresql_util/posgresql_util.py` & `krezi-1.3/krezi/posgresql_util/posgresql_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi/stopwatch_util/stopwatch.py` & `krezi-1.3/krezi/stopwatch_util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `krezi-1.2/krezi.egg-info/PKG-INFO` & `krezi-1.3/krezi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krezi
-Version: 1.2
+Version: 1.3
 Summary: Array of Utilities for Lazy but Efficient Programmers
 Author: Aadil Zikre
 Author-email: aadilzikre@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -24,8 +24,14 @@
 3. Multiprocessing : to work around GIL and utilize multiple cores/threads. Applicable to Dataframes too.
 4. Emailing : to send email alerts on demand/error.
 5. Stopwatch : to profile scripts. IMO there are better profilers out there. This is just a POC. 
 6. Postgresql : Querying from Postgres Databases.
 7. MSSQL : Querying from Microsoft SQL Server Databases.
 8. Mongo : Querying from Mongo Databases. 
 
+---
+## INSTALLATION
+
+```
+    pip install krezi
+```
```

### Comparing `krezi-1.2/krezi.egg-info/SOURCES.txt` & `krezi-1.3/krezi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krezi-1.2/setup.py` & `krezi-1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     description = f.read()
 
 setup(
     name='krezi',
-    version='1.2',
+    version='1.3',
     python_requires='>= 3.9',
     author="Aadil Zikre",
     author_email="aadilzikre@gmail.com",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.23.0',
         'pandas>=1.4.2',
@@ -21,12 +21,8 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3'
     ],
     description="Array of Utilities for Lazy but Efficient Programmers",
     long_description=description,
     long_description_content_type='text/markdown'
-)
-
-## To Build the Project : in the directory, run python setup.py sdist bdist_wheel
-## Remove the previous build manually from dist/
-## Upload the Project on PyPI : 
+)
```

