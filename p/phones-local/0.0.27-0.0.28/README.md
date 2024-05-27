# Comparing `tmp/phones_local-0.0.27.tar.gz` & `tmp/phones_local-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.27.tar", last modified: Sun May 26 21:32:41 2024, max compression
+gzip compressed data, was "phones_local-0.0.28.tar", last modified: Sun May 26 21:36:02 2024, max compression
```

## Comparing `phones_local-0.0.27.tar` & `phones_local-0.0.28.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.175127 phones_local-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:32:41.175127 phones_local-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-26 21:32:13.000000 phones_local-0.0.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.171127 phones_local-0.0.27/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.175127 phones_local-0.0.27/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:13.000000 phones_local-0.0.27/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-26 21:32:13.000000 phones_local-0.0.27/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-26 21:32:13.000000 phones_local-0.0.27/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:32:41.175127 phones_local-0.0.27/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 21:32:41.000000 phones_local-0.0.27/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-26 21:32:20.000000 phones_local-0.0.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:32:41.175127 phones_local-0.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 21:32:13.000000 phones_local-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.676454 phones_local-0.0.28/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:36:02.676454 phones_local-0.0.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-26 21:35:37.000000 phones_local-0.0.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.672454 phones_local-0.0.28/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.676454 phones_local-0.0.28/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:35:37.000000 phones_local-0.0.28/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-26 21:35:37.000000 phones_local-0.0.28/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-26 21:35:37.000000 phones_local-0.0.28/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:36:02.676454 phones_local-0.0.28/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 21:36:02.000000 phones_local-0.0.28/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-26 21:35:43.000000 phones_local-0.0.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:36:02.676454 phones_local-0.0.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 21:35:37.000000 phones_local-0.0.28/setup.py
```

### Comparing `phones_local-0.0.27/PKG-INFO` & `phones_local-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.27
+Version: 0.0.28
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.27/README.md` & `phones_local-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.27/phones_local/src/phone_local_constans.py` & `phones_local-0.0.28/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.27/phones_local/src/phones_local.py` & `phones_local-0.0.28/phones_local/src/phones_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+import random
+import string
+
 from database_mysql_local.generic_mapping import GenericMapping
 from logger_local.LoggerLocal import Logger
 from phonenumbers import (NumberParseException, PhoneNumberFormat,
                           format_number, parse)
 from user_context_remote.user_context import UserContext
 
 from .phone_local_constans import code_object_init
 
 logger = Logger.create_logger(object=code_object_init)
 user_context = UserContext()
 
 
 class PhonesLocal(GenericMapping):
-    def __init__(self) -> None:
+    def __init__(self, is_test_data: bool = False) -> None:
         super().__init__(default_schema_name="phone",
                          default_table_name="phone_table",
                          default_view_table_name="phone_view",
-                         default_column_name="phone_id")
+                         default_column_name="phone_id",
+                         is_test_data=is_test_data)
 
     def get_normalized_phone_number_by_phone_id(self, phone_id: int) -> int:
         logger.start(object={"phone_id": phone_id})
         data = self.select_one_dict_by_column_and_value(select_clause_value="local_number_normalized",
                                                         column_value=phone_id)
         if not data:
             logger.end("No phone number found for phone_id " +
@@ -186,7 +190,13 @@
             'full_number_normalized': f'+{international_code}{number_original[1:]}',
             'international_code': international_code,
             'area_code': int(number_original[1:3]),
             'extension': number_original[3],
         }
         test_phone_id = self.insert_phone(phone_data=phone_data)
         return test_phone_id
+
+    @staticmethod
+    def generate_fake_phone_number(prefix: str = "05", length: int = 8) -> str:
+        remaining_digits = ''.join(random.choices(string.digits, k=length - len(prefix)))
+        fake_phone_number = prefix + remaining_digits
+        return fake_phone_number
```

### Comparing `phones_local-0.0.27/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.28/phones_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.27
+Version: 0.0.28
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.27/pyproject.toml` & `phones_local-0.0.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.27/setup.py` & `phones_local-0.0.28/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.27',  # https://pypi.org/project/phones-local/
+    version='0.0.28',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

