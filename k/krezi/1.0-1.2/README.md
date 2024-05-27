# Comparing `tmp/krezi-1.0.tar.gz` & `tmp/krezi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krezi-1.0.tar", last modified: Mon May 27 01:53:30 2024, max compression
+gzip compressed data, was "krezi-1.2.tar", last modified: Mon May 27 02:28:12 2024, max compression
```

## Comparing `krezi-1.0.tar` & `krezi-1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:30.004113 krezi-1.0/
--rw-r--r--   0 aadilzikre   (501) staff       (20)     1068 2024-03-30 22:15:56.000000 krezi-1.0/LICENSE
--rw-r--r--   0 aadilzikre   (501) staff       (20)      939 2024-05-27 01:53:30.003423 krezi-1.0/PKG-INFO
--rw-r--r--   0 aadilzikre   (501) staff       (20)      720 2024-05-27 01:28:30.000000 krezi-1.0/README.md
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:29.978305 krezi-1.0/krezi/
--rw-r--r--   0 aadilzikre   (501) staff       (20)      862 2024-05-27 00:21:16.000000 krezi-1.0/krezi/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)    16868 2024-05-27 00:57:11.000000 krezi-1.0/krezi/common.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:29.988777 krezi-1.0/krezi/cover_letter_generator_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:23.000000 krezi-1.0/krezi/cover_letter_generator_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     5515 2024-03-07 18:12:30.000000 krezi-1.0/krezi/cover_letter_generator_util/automated_cover_letter_generator.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:29.993035 krezi-1.0/krezi/email_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)       61 2024-05-27 01:29:45.000000 krezi-1.0/krezi/email_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     4920 2024-05-27 00:59:46.000000 krezi-1.0/krezi/email_util/email_notifier.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:29.995118 krezi-1.0/krezi/logging_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:31.000000 krezi-1.0/krezi/logging_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     4343 2024-05-26 17:52:33.000000 krezi-1.0/krezi/logging_util/file_logger.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:29.999912 krezi-1.0/krezi/mssql_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:36.000000 krezi-1.0/krezi/mssql_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     2595 2023-06-03 16:25:44.000000 krezi-1.0/krezi/mssql_util/pymssql_dao.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:30.001150 krezi-1.0/krezi/multiprocessing_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:41.000000 krezi-1.0/krezi/multiprocessing_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     3334 2024-03-07 18:09:18.000000 krezi-1.0/krezi/multiprocessing_util/mp_class_util.py
--rwx------   0 aadilzikre   (501) staff       (20)     4598 2023-06-30 14:07:35.000000 krezi-1.0/krezi/multiprocessing_util/mp_util.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:30.002098 krezi-1.0/krezi/posgresql_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:50.000000 krezi-1.0/krezi/posgresql_util/__init__.py
--rwx------   0 aadilzikre   (501) staff       (20)     3575 2023-06-30 14:07:38.000000 krezi-1.0/krezi/posgresql_util/posgresql_util.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:30.002520 krezi-1.0/krezi/stopwatch_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:54.000000 krezi-1.0/krezi/stopwatch_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     3732 2024-03-08 20:18:16.000000 krezi-1.0/krezi/stopwatch_util/stopwatch.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 01:53:29.988523 krezi-1.0/krezi.egg-info/
--rw-r--r--   0 aadilzikre   (501) staff       (20)      939 2024-05-27 01:53:29.000000 krezi-1.0/krezi.egg-info/PKG-INFO
--rw-r--r--   0 aadilzikre   (501) staff       (20)      770 2024-05-27 01:53:29.000000 krezi-1.0/krezi.egg-info/SOURCES.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)        1 2024-05-27 01:53:29.000000 krezi-1.0/krezi.egg-info/dependency_links.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)       48 2024-05-27 01:53:29.000000 krezi-1.0/krezi.egg-info/requires.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)        6 2024-05-27 01:53:29.000000 krezi-1.0/krezi.egg-info/top_level.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)       38 2024-05-27 01:53:30.004199 krezi-1.0/setup.cfg
--rw-r--r--   0 aadilzikre   (501) staff       (20)      454 2024-05-27 01:52:42.000000 krezi-1.0/setup.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.819468 krezi-1.2/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1068 2024-03-30 22:15:56.000000 krezi-1.2/LICENSE
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1198 2024-05-27 02:28:12.819327 krezi-1.2/PKG-INFO
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      720 2024-05-27 01:28:30.000000 krezi-1.2/README.md
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.814088 krezi-1.2/krezi/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      862 2024-05-27 00:21:16.000000 krezi-1.2/krezi/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)    16868 2024-05-27 00:57:11.000000 krezi-1.2/krezi/common.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.815512 krezi-1.2/krezi/cover_letter_generator_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:23.000000 krezi-1.2/krezi/cover_letter_generator_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     5515 2024-03-07 18:12:30.000000 krezi-1.2/krezi/cover_letter_generator_util/automated_cover_letter_generator.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.816324 krezi-1.2/krezi/email_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       61 2024-05-27 01:29:45.000000 krezi-1.2/krezi/email_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     4920 2024-05-27 00:59:46.000000 krezi-1.2/krezi/email_util/email_notifier.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.816693 krezi-1.2/krezi/logging_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:31.000000 krezi-1.2/krezi/logging_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     4343 2024-05-26 17:52:33.000000 krezi-1.2/krezi/logging_util/file_logger.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.817232 krezi-1.2/krezi/mssql_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:36.000000 krezi-1.2/krezi/mssql_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     2595 2023-06-03 16:25:44.000000 krezi-1.2/krezi/mssql_util/pymssql_dao.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.818060 krezi-1.2/krezi/multiprocessing_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:41.000000 krezi-1.2/krezi/multiprocessing_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     3334 2024-03-07 18:09:18.000000 krezi-1.2/krezi/multiprocessing_util/mp_class_util.py
+-rwx------   0 aadilzikre   (501) staff       (20)     4598 2023-06-30 14:07:35.000000 krezi-1.2/krezi/multiprocessing_util/mp_util.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.818526 krezi-1.2/krezi/posgresql_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:50.000000 krezi-1.2/krezi/posgresql_util/__init__.py
+-rwx------   0 aadilzikre   (501) staff       (20)     3575 2023-06-30 14:07:38.000000 krezi-1.2/krezi/posgresql_util/posgresql_util.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.818861 krezi-1.2/krezi/stopwatch_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:54.000000 krezi-1.2/krezi/stopwatch_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     3732 2024-03-08 20:18:16.000000 krezi-1.2/krezi/stopwatch_util/stopwatch.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 02:28:12.815258 krezi-1.2/krezi.egg-info/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1198 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/PKG-INFO
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      770 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/SOURCES.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        1 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/dependency_links.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       48 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/requires.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        6 2024-05-27 02:28:12.000000 krezi-1.2/krezi.egg-info/top_level.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       38 2024-05-27 02:28:12.819516 krezi-1.2/setup.cfg
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      931 2024-05-27 02:28:01.000000 krezi-1.2/setup.py
```

### Comparing `krezi-1.0/LICENSE` & `krezi-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `krezi-1.0/PKG-INFO` & `krezi-1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: krezi
-Version: 1.0
-Summary: UNKNOWN
+Version: 1.2
+Summary: Array of Utilities for Lazy but Efficient Programmers
 Author: Aadil Zikre
 Author-email: aadilzikre@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # krezi
 
 Commonly used functions to improve coding experience and avoid repeatability. As I am publishing this package for learning purposes, this library is not written to be foolproof. Use wisely.
```

### Comparing `krezi-1.0/README.md` & `krezi-1.2/README.md`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/__init__.py` & `krezi-1.2/krezi/__init__.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/common.py` & `krezi-1.2/krezi/common.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/cover_letter_generator_util/automated_cover_letter_generator.py` & `krezi-1.2/krezi/cover_letter_generator_util/automated_cover_letter_generator.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/email_util/email_notifier.py` & `krezi-1.2/krezi/email_util/email_notifier.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/logging_util/file_logger.py` & `krezi-1.2/krezi/logging_util/file_logger.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/mssql_util/pymssql_dao.py` & `krezi-1.2/krezi/mssql_util/pymssql_dao.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/multiprocessing_util/mp_class_util.py` & `krezi-1.2/krezi/multiprocessing_util/mp_class_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/multiprocessing_util/mp_util.py` & `krezi-1.2/krezi/multiprocessing_util/mp_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/posgresql_util/posgresql_util.py` & `krezi-1.2/krezi/posgresql_util/posgresql_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi/stopwatch_util/stopwatch.py` & `krezi-1.2/krezi/stopwatch_util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `krezi-1.0/krezi.egg-info/PKG-INFO` & `krezi-1.2/krezi.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: krezi
-Version: 1.0
-Summary: UNKNOWN
+Version: 1.2
+Summary: Array of Utilities for Lazy but Efficient Programmers
 Author: Aadil Zikre
 Author-email: aadilzikre@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # krezi
 
 Commonly used functions to improve coding experience and avoid repeatability. As I am publishing this package for learning purposes, this library is not written to be foolproof. Use wisely.
```

### Comparing `krezi-1.0/krezi.egg-info/SOURCES.txt` & `krezi-1.2/krezi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

