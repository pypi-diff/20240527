# Comparing `tmp/contact_user_external_local-0.0.5.tar.gz` & `tmp/contact_user_external_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_user_external_local-0.0.5.tar", last modified: Fri May 17 15:00:40 2024, max compression
+gzip compressed data, was "contact_user_external_local-0.0.7.tar", last modified: Sun May 26 23:32:34 2024, max compression
```

## Comparing `contact_user_external_local-0.0.5.tar` & `contact_user_external_local-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.534534 contact_user_external_local-0.0.5/contact_user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/contact_user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/contact_user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 15:00:40.000000 contact_user_external_local-0.0.5/contact_user_external_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:00:40.538534 contact_user_external_local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-17 15:00:23.000000 contact_user_external_local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.046302 contact_user_external_local-0.0.7/contact_user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/contact_user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/contact_user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/contact_user_external_local/src/contact_user_external_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/contact_user_external_local/src/contact_user_external_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-26 23:32:34.000000 contact_user_external_local-0.0.7/contact_user_external_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-26 23:32:10.000000 contact_user_external_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:32:34.050302 contact_user_external_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-26 23:32:03.000000 contact_user_external_local-0.0.7/setup.py
```

### Comparing `contact_user_external_local-0.0.5/PKG-INFO` & `contact_user_external_local-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.5
+Version: 0.0.7
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local.py` & `contact_user_external_local-0.0.7/contact_user_external_local/src/contact_user_external_local.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 from database_mysql_local.generic_mapping import GenericMapping
-from logger_local.LoggerLocal import Logger
+from logger_local.MetaLogger import MetaLogger
 from user_context_remote.user_context import UserContext
 from user_external_local.user_externals_local import UserExternalsLocal
 
 from .contact_user_external_local_constants import CONTACT_USER_EXTERNAL_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
 
 DEFAULT_SCHEMA_NAME = 'contact_user_external'
 DEFAULT_ENTITY_NAME1 = 'contact'
 DEFAULT_ENTITY_NAME2 = 'user_external'
 DEFAULT_ID_COLUMN_NAME = 'contact_user_external_id'
 DEFAULT_TABLE_NAME = 'contact_user_external_table'
 DEFAULT_VIEW_TABLE_NAME = 'contact_user_external_view'
 DEFAULT_SYSTEM_ID = 6
 
-logger = Logger.create_logger(object=CONTACT_USER_EXTERNAL_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
-
 user_context = UserContext()
 
 
-class ContactUserExternalLocal(GenericMapping):
-    def __init__(self, default_schema_name: str = DEFAULT_SCHEMA_NAME, default_entity_name1: str = DEFAULT_ENTITY_NAME1,
-                 default_entity_name2: str = DEFAULT_ENTITY_NAME2, default_id_column_name: str = DEFAULT_ID_COLUMN_NAME,
-                 default_table_name: str = DEFAULT_TABLE_NAME, default_view_table_name: str = DEFAULT_VIEW_TABLE_NAME,
-                 system_id: int = DEFAULT_SYSTEM_ID, is_test_data: bool = False):
-
-        GenericMapping.__init__(self, default_schema_name=default_schema_name,
-                                default_entity_name1=default_entity_name1,
-                                default_entity_name2=default_entity_name2,
-                                default_id_column_name=default_id_column_name,
-                                default_table_name=default_table_name, default_view_table_name=default_view_table_name,
+class ContactUserExternalLocal(GenericMapping, metaclass=MetaLogger,
+                               object=CONTACT_USER_EXTERNAL_PYTHON_PACKAGE_CODE_LOGGER_OBJECT):
+    def __init__(self, system_id: int = DEFAULT_SYSTEM_ID, is_test_data: bool = False):
+
+        GenericMapping.__init__(self, default_schema_name=DEFAULT_SCHEMA_NAME,
+                                default_entity_name1=DEFAULT_ENTITY_NAME1,
+                                default_entity_name2=DEFAULT_ENTITY_NAME2,
+                                default_column_name=DEFAULT_ID_COLUMN_NAME,
+                                default_table_name=DEFAULT_TABLE_NAME,
+                                default_view_table_name=DEFAULT_VIEW_TABLE_NAME,
                                 is_test_data=is_test_data)
         self.user_externals = UserExternalsLocal(is_test_data=is_test_data)
         self.system_id = system_id
 
     def insert_contact_and_link_to_existing_or_new_user_external(
-            # TODO change dict -> dict[Contact]
+            # TODO change dict -> dict[Contact] (not used)
             # TODO change str -> EmailAddress
-            self, contact_dict: dict, contact_email_address: str,
+            self, *, contact_dict: dict, contact_email_address: str,
             contact_id: int, system_id: int = None, user_external_dict: dict = None) -> int or None:
         """
         Insert contact and link to existing or new user_external
         :param contact_dict: contact dict
         :param contact_id: contact id
         :param contact_email_address: contact email address
         :param system_id: system id
         :param user_external_dict: user_external dict
         :return: contact_user-external_id
         """
-        logger.start(object={"contact_dict": contact_dict, "contact_email_address": contact_email_address,
-                             "contact_id": contact_id, "system_id": system_id,
-                             "user_external_dict": user_external_dict})
         profile_id = user_context.get_effective_profile_id()
         system_id = system_id or self.system_id
         access_token = expiry = refresh_token = None
         if user_external_dict:
             # username = user_external_dict.get("username", contact_email_address)
             profile_id = user_external_dict.get("profile_id", profile_id)
             system_id = user_external_dict.get("system_id", system_id)
@@ -68,50 +62,45 @@
         user_external_id = self.user_externals.select_one_value_by_where(
             select_clause_value="user_external_id", where="username=%s AND system_id=%s",
             # TODO allow to send to order_by also order_by_array with two items "start_timestamp" and DESC enum- This way we can move to other non SQL databases
             params=(contact_email_address, system_id), order_by="start_timestamp DESC")
 
         if not user_external_id:
             if not access_token:
-                logger.warning(exception_message="access_token is None")
-                logger.end(object={"contact_user_external_id": None})
-                return None
+                self.logger.warning("access_token is None")
+                return
             # create new user_external and add it to user_external_table
-            logger.info(log_message="user_external_id is None, creating new user_external")
+            self.logger.info("user_external_id is None, creating new user_external")
             # TODO: when ready, use the minsert method that returns the id
             self.user_externals.insert_or_update_user_external_access_token(
                 username=contact_email_address, profile_id=profile_id, system_id=system_id,
                 access_token=access_token, expiry=expiry, refresh_token=refresh_token)
             # TODO: when ready, use the minsert method that returns the id
             user_external_id = self.user_externals.select_one_value_by_where(
                 select_clause_value="user_external_id",
                 where="username=%s AND system_id=%s",
-                params=(
-                    contact_email_address, system_id),
+                params=(contact_email_address, system_id),
                 order_by="start_timestamp DESC")
             if not user_external_id:
-                exception_message = "user_external_id not found"
-                logger.exception(exception_message)
-                raise Exception(exception_message)
+                raise Exception("user_external_id not found")
             contact_user_external_id = self.insert_mapping(
                 entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
                 entity_id1=contact_id, entity_id2=user_external_id,
                 ignore_duplicate=True)
         else:
             # link to existing user_external
-            logger.info(log_message="user_external_id is not None, linking to existing user_external")
+            self.logger.info("user_external_id is not None, linking to existing user_external")
             # TODO contact_user_external_mapping_result_tuple
             mapping_tuple = self.select_multi_mapping_tuple_by_id(
                 entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
                 entity_id1=contact_id, entity_id2=user_external_id)
             if not mapping_tuple:
-                logger.info(log_message="mapping_tuple is None, creating new mapping")
+                self.logger.info("mapping_tuple is None, creating new mapping")
                 contact_user_external_id = self.insert_mapping(
                     entity_name1=self.default_entity_name1, entity_name2=self.default_entity_name2,
                     entity_id1=contact_id, entity_id2=user_external_id,
                     ignore_duplicate=True)
             else:
-                logger.info(log_message="mapping_tuple is not None")
+                self.logger.info("mapping_tuple is not None")
                 contact_user_external_id = mapping_tuple[0]
 
-        logger.end(object={"contact_user_external_id": contact_user_external_id})
         return contact_user_external_id
```

### Comparing `contact_user_external_local-0.0.5/contact_user_external_local/src/contact_user_external_local_constants.py` & `contact_user_external_local-0.0.7/contact_user_external_local/src/contact_user_external_local_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
-
 CONTACT_USER_EXTERNAL_LOCAL_PYTHON_COMPONENT_ID = 278
 CONTACT_USER_EXTERNAL_LOCAL_PYTHON_COMPONENT_NAME = "contact-user-external-local-python-package"
 DEVELOPER_EMAIL = "tal.g@circ.zone"
 CONTACT_USER_EXTERNAL_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
     'component_id': CONTACT_USER_EXTERNAL_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': CONTACT_USER_EXTERNAL_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': DEVELOPER_EMAIL
 }
 
-
 CONTACT_USER_EXTERNAL_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
     'component_id': CONTACT_USER_EXTERNAL_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': CONTACT_USER_EXTERNAL_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Unit_Test.value,
     'testing_framework': LoggerComponentEnum.testingFramework.pytest.value,
     'developer_email': DEVELOPER_EMAIL
 }
```

### Comparing `contact_user_external_local-0.0.5/contact_user_external_local.egg-info/PKG-INFO` & `contact_user_external_local-0.0.7/contact_user_external_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-user-external-local
-Version: 0.0.5
+Version: 0.0.7
 Summary: PyPI Package for Circles contact-user-external-local Python
 Home-page: https://github.com/circles-zone/contact-user-external-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_user_external_local-0.0.5/setup.py` & `contact_user_external_local-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.5',  # https://pypi.org/project/contact-user-external-local/
+    version='0.0.7',  # https://pypi.org/project/contact-user-external-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-user-external-local Python",
     long_description="PyPI Package for Circles contact-user-external-local Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     package_dir={package_dir: f'{package_dir}/src'},
```

