# Comparing `tmp/krezi-1.3.tar.gz` & `tmp/krezi-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krezi-1.3.tar", last modified: Mon May 27 03:19:38 2024, max compression
+gzip compressed data, was "krezi-1.4.tar", last modified: Mon May 27 03:30:01 2024, max compression
```

## Comparing `krezi-1.3.tar` & `krezi-1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.008230 krezi-1.3/
--rw-r--r--   0 aadilzikre   (501) staff       (20)     1068 2024-03-30 22:15:56.000000 krezi-1.3/LICENSE
--rw-r--r--   0 aadilzikre   (501) staff       (20)     1249 2024-05-27 03:19:38.008075 krezi-1.3/PKG-INFO
--rw-r--r--   0 aadilzikre   (501) staff       (20)      771 2024-05-27 02:32:37.000000 krezi-1.3/README.md
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.001450 krezi-1.3/krezi/
--rw-r--r--   0 aadilzikre   (501) staff       (20)      862 2024-05-27 00:21:16.000000 krezi-1.3/krezi/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)    16868 2024-05-27 00:57:11.000000 krezi-1.3/krezi/common.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.003608 krezi-1.3/krezi/cover_letter_generator_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:23.000000 krezi-1.3/krezi/cover_letter_generator_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     5515 2024-03-07 18:12:30.000000 krezi-1.3/krezi/cover_letter_generator_util/automated_cover_letter_generator.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.004551 krezi-1.3/krezi/email_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)       61 2024-05-27 01:29:45.000000 krezi-1.3/krezi/email_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     4920 2024-05-27 00:59:46.000000 krezi-1.3/krezi/email_util/email_notifier.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.004970 krezi-1.3/krezi/logging_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:31.000000 krezi-1.3/krezi/logging_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     4344 2024-05-27 03:18:30.000000 krezi-1.3/krezi/logging_util/file_logger.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.005517 krezi-1.3/krezi/mssql_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:36.000000 krezi-1.3/krezi/mssql_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     2595 2023-06-03 16:25:44.000000 krezi-1.3/krezi/mssql_util/pymssql_dao.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.006469 krezi-1.3/krezi/multiprocessing_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:41.000000 krezi-1.3/krezi/multiprocessing_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     3334 2024-03-07 18:09:18.000000 krezi-1.3/krezi/multiprocessing_util/mp_class_util.py
--rwx------   0 aadilzikre   (501) staff       (20)     4598 2023-06-30 14:07:35.000000 krezi-1.3/krezi/multiprocessing_util/mp_util.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.007169 krezi-1.3/krezi/posgresql_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:50.000000 krezi-1.3/krezi/posgresql_util/__init__.py
--rwx------   0 aadilzikre   (501) staff       (20)     3575 2023-06-30 14:07:38.000000 krezi-1.3/krezi/posgresql_util/posgresql_util.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.007487 krezi-1.3/krezi/stopwatch_util/
--rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:54.000000 krezi-1.3/krezi/stopwatch_util/__init__.py
--rw-r--r--   0 aadilzikre   (501) staff       (20)     3732 2024-03-08 20:18:16.000000 krezi-1.3/krezi/stopwatch_util/stopwatch.py
-drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:19:38.003379 krezi-1.3/krezi.egg-info/
--rw-r--r--   0 aadilzikre   (501) staff       (20)     1249 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/PKG-INFO
--rw-r--r--   0 aadilzikre   (501) staff       (20)      770 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/SOURCES.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)        1 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/dependency_links.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)       48 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/requires.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)        6 2024-05-27 03:19:37.000000 krezi-1.3/krezi.egg-info/top_level.txt
--rw-r--r--   0 aadilzikre   (501) staff       (20)       38 2024-05-27 03:19:38.008281 krezi-1.3/setup.cfg
--rw-r--r--   0 aadilzikre   (501) staff       (20)      766 2024-05-27 03:19:28.000000 krezi-1.3/setup.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.373119 krezi-1.4/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1068 2024-03-30 22:15:56.000000 krezi-1.4/LICENSE
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1249 2024-05-27 03:30:01.372973 krezi-1.4/PKG-INFO
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      771 2024-05-27 02:32:37.000000 krezi-1.4/README.md
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.368061 krezi-1.4/krezi/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      862 2024-05-27 00:21:16.000000 krezi-1.4/krezi/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)    16868 2024-05-27 00:57:11.000000 krezi-1.4/krezi/common.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.369260 krezi-1.4/krezi/cover_letter_generator_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:23.000000 krezi-1.4/krezi/cover_letter_generator_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     5515 2024-03-07 18:12:30.000000 krezi-1.4/krezi/cover_letter_generator_util/automated_cover_letter_generator.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.369991 krezi-1.4/krezi/email_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       61 2024-05-27 01:29:45.000000 krezi-1.4/krezi/email_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     4920 2024-05-27 00:59:46.000000 krezi-1.4/krezi/email_util/email_notifier.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.370455 krezi-1.4/krezi/logging_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:31.000000 krezi-1.4/krezi/logging_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     4328 2024-05-27 03:29:23.000000 krezi-1.4/krezi/logging_util/file_logger.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.370805 krezi-1.4/krezi/mssql_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:36.000000 krezi-1.4/krezi/mssql_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     2595 2023-06-03 16:25:44.000000 krezi-1.4/krezi/mssql_util/pymssql_dao.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.371711 krezi-1.4/krezi/multiprocessing_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:41.000000 krezi-1.4/krezi/multiprocessing_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     3334 2024-03-07 18:09:18.000000 krezi-1.4/krezi/multiprocessing_util/mp_class_util.py
+-rwx------   0 aadilzikre   (501) staff       (20)     4598 2023-06-30 14:07:35.000000 krezi-1.4/krezi/multiprocessing_util/mp_util.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.372254 krezi-1.4/krezi/posgresql_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:50.000000 krezi-1.4/krezi/posgresql_util/__init__.py
+-rwx------   0 aadilzikre   (501) staff       (20)     3575 2023-06-30 14:07:38.000000 krezi-1.4/krezi/posgresql_util/posgresql_util.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.372579 krezi-1.4/krezi/stopwatch_util/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        0 2024-03-31 00:12:54.000000 krezi-1.4/krezi/stopwatch_util/__init__.py
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     3732 2024-03-08 20:18:16.000000 krezi-1.4/krezi/stopwatch_util/stopwatch.py
+drwxr-xr-x   0 aadilzikre   (501) staff       (20)        0 2024-05-27 03:30:01.368972 krezi-1.4/krezi.egg-info/
+-rw-r--r--   0 aadilzikre   (501) staff       (20)     1249 2024-05-27 03:30:01.000000 krezi-1.4/krezi.egg-info/PKG-INFO
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      770 2024-05-27 03:30:01.000000 krezi-1.4/krezi.egg-info/SOURCES.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        1 2024-05-27 03:30:01.000000 krezi-1.4/krezi.egg-info/dependency_links.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       48 2024-05-27 03:30:01.000000 krezi-1.4/krezi.egg-info/requires.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)        6 2024-05-27 03:30:01.000000 krezi-1.4/krezi.egg-info/top_level.txt
+-rw-r--r--   0 aadilzikre   (501) staff       (20)       38 2024-05-27 03:30:01.373178 krezi-1.4/setup.cfg
+-rw-r--r--   0 aadilzikre   (501) staff       (20)      766 2024-05-27 03:29:42.000000 krezi-1.4/setup.py
```

### Comparing `krezi-1.3/LICENSE` & `krezi-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `krezi-1.3/PKG-INFO` & `krezi-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krezi
-Version: 1.3
+Version: 1.4
 Summary: Array of Utilities for Lazy but Efficient Programmers
 Author: Aadil Zikre
 Author-email: aadilzikre@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krezi-1.3/README.md` & `krezi-1.4/README.md`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/__init__.py` & `krezi-1.4/krezi/__init__.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/common.py` & `krezi-1.4/krezi/common.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/cover_letter_generator_util/automated_cover_letter_generator.py` & `krezi-1.4/krezi/cover_letter_generator_util/automated_cover_letter_generator.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/email_util/email_notifier.py` & `krezi-1.4/krezi/email_util/email_notifier.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/logging_util/file_logger.py` & `krezi-1.4/krezi/logging_util/file_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
                 stream_handler = logging.StreamHandler(stream = sys.stdout)
             else:
                 stream_handler = logging.StreamHandler(stream = sys.stderr)
             stream_handler.setFormatter(formatter)
             stream_handler.setLevel(self.level)
             self.logger.addHandler(stream_handler)
     
-    def get_logger(self, dt_fmt_basic = True):
+    def get_logger(self):
         if not self.logger:
-            self.set_logger(dt_fmt_basic)
+            self.set_logger(self.dt_fmt_basic)
         return self.logger
     
     def add_file_handler(self, filepath, level = logging.INFO, dt_fmt_basic=None):
         file_handler = logging.FileHandler(filepath)
         file_handler.setLevel(level)
         dt_fmt_basic = self.dt_fmt_basic if dt_fmt_basic is None else dt_fmt_basic
         if dt_fmt_basic:
```

### Comparing `krezi-1.3/krezi/mssql_util/pymssql_dao.py` & `krezi-1.4/krezi/mssql_util/pymssql_dao.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/multiprocessing_util/mp_class_util.py` & `krezi-1.4/krezi/multiprocessing_util/mp_class_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/multiprocessing_util/mp_util.py` & `krezi-1.4/krezi/multiprocessing_util/mp_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/posgresql_util/posgresql_util.py` & `krezi-1.4/krezi/posgresql_util/posgresql_util.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi/stopwatch_util/stopwatch.py` & `krezi-1.4/krezi/stopwatch_util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `krezi-1.3/krezi.egg-info/PKG-INFO` & `krezi-1.4/krezi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krezi
-Version: 1.3
+Version: 1.4
 Summary: Array of Utilities for Lazy but Efficient Programmers
 Author: Aadil Zikre
 Author-email: aadilzikre@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krezi-1.3/krezi.egg-info/SOURCES.txt` & `krezi-1.4/krezi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krezi-1.3/setup.py` & `krezi-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     description = f.read()
 
 setup(
     name='krezi',
-    version='1.3',
+    version='1.4',
     python_requires='>= 3.9',
     author="Aadil Zikre",
     author_email="aadilzikre@gmail.com",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.23.0',
         'pandas>=1.4.2',
```

