# Comparing `tmp/nestipy_peewee-0.2.0.tar.gz` & `tmp/nestipy_peewee-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_peewee-0.2.0.tar", max compression
+gzip compressed data, was "nestipy_peewee-0.2.1.tar", max compression
```

## Comparing `nestipy_peewee-0.2.0.tar` & `nestipy_peewee-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_peewee-0.2.0/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_peewee-0.2.0/README.md
--rw-r--r--   0        0        0      501 2024-04-30 15:24:03.878876 nestipy_peewee-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.2.0/src/nestipy_peewee/__init__.py
--rw-r--r--   0        0        0      740 2024-04-30 15:23:07.067353 nestipy_peewee-0.2.0/src/nestipy_peewee/peewee_builder.py
--rw-r--r--   0        0        0      410 2024-04-30 15:23:14.671289 nestipy_peewee-0.2.0/src/nestipy_peewee/peewee_decorator.py
--rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.2.0/src/nestipy_peewee/peewee_meta.py
--rw-r--r--   0        0        0     2327 2024-04-30 15:22:51.495484 nestipy_peewee-0.2.0/src/nestipy_peewee/peewee_module.py
--rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 nestipy_peewee-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_peewee-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_peewee-0.2.1/README.md
+-rw-r--r--   0        0        0      501 2024-05-27 13:29:31.556856 nestipy_peewee-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-27 07:50:37.316624 nestipy_peewee-0.2.1/src/nestipy_peewee/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-30 15:23:07.067353 nestipy_peewee-0.2.1/src/nestipy_peewee/peewee_builder.py
+-rw-r--r--   0        0        0      410 2024-04-30 15:23:14.671289 nestipy_peewee-0.2.1/src/nestipy_peewee/peewee_decorator.py
+-rw-r--r--   0        0        0       58 2024-04-27 06:47:04.319886 nestipy_peewee-0.2.1/src/nestipy_peewee/peewee_meta.py
+-rw-r--r--   0        0        0     2377 2024-05-27 13:28:25.171291 nestipy_peewee-0.2.1/src/nestipy_peewee/peewee_module.py
+-rw-r--r--   0        0        0     2429 1970-01-01 00:00:00.000000 nestipy_peewee-0.2.1/PKG-INFO
```

### Comparing `nestipy_peewee-0.2.0/LICENSE` & `nestipy_peewee-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.2.0/README.md` & `nestipy_peewee-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.2.0/src/nestipy_peewee/peewee_builder.py` & `nestipy_peewee-0.2.1/src/nestipy_peewee/peewee_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy_peewee-0.2.0/src/nestipy_peewee/peewee_module.py` & `nestipy_peewee-0.2.1/src/nestipy_peewee/peewee_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import inspect
 from dataclasses import asdict
-from typing import Type
+from typing import Type, Annotated
 from nestipy.common import Module
 from nestipy.dynamic_module import NestipyModule
 from nestipy.ioc import Inject
 from nestipy.metadata import Reflect
 from peewee import Model, Database, SqliteDatabase, MySQLDatabase, PostgresqlDatabase
 
-from .peewee_builder import ConfigurableModuleClass, PEEWEE_DB_CONFIG
+from .peewee_builder import ConfigurableModuleClass, PEEWEE_DB_CONFIG, PeeweeConfig
 from .peewee_meta import PeeweeMetadata
 
 
 @Module()
 class PeeweeModule(ConfigurableModuleClass, NestipyModule):
     _db: Database
-    _config: Inject[PEEWEE_DB_CONFIG]
+    _config: Annotated[PeeweeConfig, Inject(PEEWEE_DB_CONFIG)]
     _models: list = []
     _peewee_models: list = []
 
     async def on_startup(self):
         config_dict = asdict(self._config)
         del config_dict['driver']
         match self._config.driver:
```

### Comparing `nestipy_peewee-0.2.0/PKG-INFO` & `nestipy_peewee-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy-peewee
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy-peewee Version: 0.2.0 Summary: Author:
+Metadata-Version: 2.1 Name: nestipy-peewee Version: 0.2.1 Summary: Author:
 tsiresymila Author-email: tsiresymila@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: nestipy
 (>=0.3.0,<0.4.0) Requires-Dist: nestipy-config (>=0.1.2,<0.2.0) Requires-Dist:
 peewee (>=3.17.3,<4.0.0) Description-Content-Type: text/markdown
                                 [Nestipy Logo]
```

