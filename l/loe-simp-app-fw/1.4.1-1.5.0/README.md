# Comparing `tmp/loe_simp_app_fw-1.4.1.tar.gz` & `tmp/loe_simp_app_fw-1.5.0.tar.gz`

## Comparing `loe_simp_app_fw-1.4.1.tar` & `loe_simp_app_fw-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/config-example.yaml
--rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/.github/workflows/workflow.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/config-example.yaml
+-rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.5.0/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.4.1/.github/workflows/workflow.yaml` & `loe_simp_app_fw-1.5.0/.github/workflows/workflow.yaml`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.5.0/src/loe_simp_app_fw/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import os
 import datetime
-from typing import Literal, Dict, Tuple, List
+from typing import Literal, Dict, Tuple, List, TypeAlias
 import tempfile
 from io import TextIOWrapper
 from .helper import create_folder_if_not_exists, ProjectRootChanged
 import atexit
 
 # Do not write the Log until the explicit initialization of the logger
-
-class _LogLevel:
-    numerical_map: Dict[Literal["DEBUG", "INFO", "WARNING", "ERROR"], Literal[0, 1, 2, 3]]= {
-        "DEBUG": 0,
-        "INFO": 1,
-        "WARNING": 2,
-        "ERROR": 3
-    }
+LogLevels: TypeAlias = Literal["DEBUG", "INFO", "WARNING", "ERROR"]    
 
 class Logger:
     # Following parameters should be set at the top-level environment of the project
     _project_root_path = ""
     _log_folder_path = "" # The path of _example_config_path relative to _project_root_path
     
     # Internal variable
-    _log_buffer: List[Tuple[Literal["DEBUG", "INFO", "WARNING", "ERROR"], str]] = []
+    _log_buffer: List[Tuple[LogLevels, str]] = []
     _isInit: bool = False
     _log_file_handle: TextIOWrapper = tempfile.TemporaryFile("w")
-    _log_level: Literal["DEBUG", "INFO", "WARNING", "ERROR"] = "INFO"
+    _log_level: LogLevels = "INFO"
     
+    # Constant
+    numerical_map: Dict[LogLevels, Literal[0, 1, 2, 3]]= {
+        "DEBUG": 0,
+        "INFO": 1,
+        "WARNING": 2,
+        "ERROR": 3
+    }
+
     @classmethod
     def _log_location(cls):
         file_name = f"{datetime.date.today()}.log"
         return os.path.join(cls._project_root_path, cls._log_folder_path, file_name)
 
     @classmethod
     def _create_log_file(cls):
         if not os.path.isfile(cls._log_location()) and not os.path.isdir(cls._log_location()):
             with open(cls._log_location(), "w", encoding="utf-8") as f:
                 print("Create log file successfully.")
 
-    def __init__(self, log_folder_path: str, project_root_path: str = os.getcwd(), log_level: Literal["DEBUG", "INFO", "WARNING", "ERROR"] = "INFO"):
+    def __init__(self, log_folder_path: str, project_root_path: str = os.getcwd(), log_level: LogLevels = "INFO"):
         """Init Logger
 
         Args:
             log_folder_path (str): path to log folder relative to project root path
             project_root_path (str, optional): path to project top-level directory. Defaults to os.getcwd().
                                                 The parent folder of that would be os.path.dirname(os.path.realpath(__file__)).
 
@@ -96,31 +97,36 @@
         cls._log("WARNING", msg)
 
     @classmethod
     def error(cls, msg :str) -> None:
         cls._log("ERROR", msg)
 
     @classmethod
-    def _log(cls, level: Literal["DEBUG", "INFO", "WARNING", "ERROR"], msg: str) -> None:
+    def set_log_level(cls, level: LogLevels) -> None:
+        cls._log_level = level
+        Logger.warning(f"Log level is manually set to {level}")
+
+    @classmethod
+    def _log(cls, level: LogLevels, msg: str) -> None:
         # Compose log
         composed_log_entry = cls._log_composer(level, msg)
         if cls._isInit:
             # Log level filter
-            if _LogLevel.numerical_map[level] >= _LogLevel.numerical_map[cls._log_level]:
+            if cls.numerical_map[level] >= cls.numerical_map[cls._log_level]:
                 # The file handler is only to make static checker happy
                 # Write to file
                 cls._log_file_handle.writelines(composed_log_entry)
         else:
             # Write to buffer, not file
             cls._log_buffer.append((level, msg))
             print(composed_log_entry)
         return
 
     @staticmethod
-    def _log_composer(level: Literal["DEBUG", "INFO", "WARNING", "ERROR"], msg: str) -> str:
+    def _log_composer(level: LogLevels, msg: str) -> str:
         return f"{datetime.datetime.now()} {level.upper()}: {msg}\n"
         
 
 @atexit.register
 def clean_log_buffer():
     Logger.error("Uncatched error! Panic! Exit!")
     # Clean up logger buffer when crashing
```

### Comparing `loe_simp_app_fw-1.4.1/tests/test_import.py` & `loe_simp_app_fw-1.5.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.1/.gitignore` & `loe_simp_app_fw-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.1/LICENSE` & `loe_simp_app_fw-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.1/README.md` & `loe_simp_app_fw-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.1/pyproject.toml` & `loe_simp_app_fw-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.4.1"
+version = "1.5.0"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.4.1/PKG-INFO` & `loe_simp_app_fw-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.4.1
+Version: 1.5.0
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

