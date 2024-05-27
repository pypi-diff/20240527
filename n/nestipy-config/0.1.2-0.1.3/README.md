# Comparing `tmp/nestipy_config-0.1.2.tar.gz` & `tmp/nestipy_config-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_config-0.1.2.tar", max compression
+gzip compressed data, was "nestipy_config-0.1.3.tar", max compression
```

## Comparing `nestipy_config-0.1.2.tar` & `nestipy_config-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_config-0.1.2/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_config-0.1.2/README.md
--rw-r--r--   0        0        0      435 2024-04-30 15:17:30.582179 nestipy_config-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-27 18:09:34.176104 nestipy_config-0.1.2/src/nestipy_config/__init__.py
--rw-r--r--   0        0        0      686 2024-04-30 15:17:39.786102 nestipy_config-0.1.2/src/nestipy_config/config_builder.py
--rw-r--r--   0        0        0      283 2024-04-27 18:06:48.892072 nestipy_config-0.1.2/src/nestipy_config/config_module.py
--rw-r--r--   0        0        0      758 2024-04-29 11:59:37.960181 nestipy_config-0.1.2/src/nestipy_config/config_service.py
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 nestipy_config-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_config-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_config-0.1.3/README.md
+-rw-r--r--   0        0        0      435 2024-05-27 13:15:54.105358 nestipy_config-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-27 18:09:34.176104 nestipy_config-0.1.3/src/nestipy_config/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-30 15:17:39.786102 nestipy_config-0.1.3/src/nestipy_config/config_builder.py
+-rw-r--r--   0        0        0      283 2024-04-27 18:06:48.892072 nestipy_config-0.1.3/src/nestipy_config/config_module.py
+-rw-r--r--   0        0        0      825 2024-05-27 13:08:44.577512 nestipy_config-0.1.3/src/nestipy_config/config_service.py
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 nestipy_config-0.1.3/PKG-INFO
```

### Comparing `nestipy_config-0.1.2/LICENSE` & `nestipy_config-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy_config-0.1.2/README.md` & `nestipy_config-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_config-0.1.2/src/nestipy_config/config_builder.py` & `nestipy_config-0.1.3/src/nestipy_config/config_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy_config-0.1.2/src/nestipy_config/config_service.py` & `nestipy_config-0.1.3/src/nestipy_config/config_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
-
+from typing import Annotated
 from dotenv import dotenv_values
 from nestipy.common import Injectable
-from nestipy_ioc import Inject
+from nestipy.ioc import Inject
 
-from .config_builder import CONFIG_OPTION
+from .config_builder import CONFIG_OPTION, ConfigOption
 
 
 @Injectable()
 class ConfigService:
-    options: Inject[CONFIG_OPTION]
+    options: Annotated[ConfigOption, Inject(CONFIG_OPTION)]
     env: dict = []
 
     def __init__(self):
         if self.options.ignore_env_file:
             self.env = dict(os.environ)
         else:
             env_directory = os.path.join(os.getcwd(), self.options.folder, '.env')
```

### Comparing `nestipy_config-0.1.2/PKG-INFO` & `nestipy_config-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy-config
-Version: 0.1.2
+Version: 0.1.3
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
-Metadata-Version: 2.1 Name: nestipy-config Version: 0.1.2 Summary: Author:
+Metadata-Version: 2.1 Name: nestipy-config Version: 0.1.3 Summary: Author:
 tsiresymila Author-email: tsiresymila@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: nestipy
 (>=0.3.0,<0.4.0) Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Description-
 Content-Type: text/markdown
                                 [Nestipy Logo]
```

