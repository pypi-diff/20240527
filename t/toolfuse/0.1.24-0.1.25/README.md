# Comparing `tmp/toolfuse-0.1.24.tar.gz` & `tmp/toolfuse-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.24.tar", max compression
+gzip compressed data, was "toolfuse-0.1.25.tar", max compression
```

## Comparing `toolfuse-0.1.24.tar` & `toolfuse-0.1.25.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.24/LICENSE
--rw-r--r--   0        0        0     4594 2024-05-05 16:31:27.833089 toolfuse-0.1.24/README.md
--rw-r--r--   0        0        0      803 2024-05-20 20:55:38.506063 toolfuse-0.1.24/pyproject.toml
--rw-r--r--   0        0        0      435 2024-05-05 03:00:01.092317 toolfuse-0.1.24/toolfuse/__init__.py
--rw-r--r--   0        0        0    30555 2024-05-20 20:56:34.273635 toolfuse-0.1.24/toolfuse/base.py
--rw-r--r--   0        0        0      231 2024-05-20 20:55:10.878956 toolfuse-0.1.24/toolfuse/models.py
--rw-r--r--   0        0        0      996 2024-05-05 02:09:19.322511 toolfuse-0.1.24/toolfuse/multi.py
--rw-r--r--   0        0        0      543 2024-05-05 03:06:09.263475 toolfuse-0.1.24/toolfuse/util.py
--rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 toolfuse-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.25/LICENSE
+-rw-r--r--   0        0        0     4594 2024-05-05 16:31:27.833089 toolfuse-0.1.25/README.md
+-rw-r--r--   0        0        0      826 2024-05-27 19:15:24.920226 toolfuse-0.1.25/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-05-05 03:00:01.092317 toolfuse-0.1.25/toolfuse/__init__.py
+-rw-r--r--   0        0        0    31375 2024-05-27 19:15:16.238851 toolfuse-0.1.25/toolfuse/base.py
+-rw-r--r--   0        0        0      231 2024-05-20 20:55:10.878956 toolfuse-0.1.25/toolfuse/models.py
+-rw-r--r--   0        0        0      996 2024-05-05 02:09:19.322511 toolfuse-0.1.25/toolfuse/multi.py
+-rw-r--r--   0        0        0      543 2024-05-05 03:06:09.263475 toolfuse-0.1.25/toolfuse/util.py
+-rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 toolfuse-0.1.25/PKG-INFO
```

### Comparing `toolfuse-0.1.24/LICENSE` & `toolfuse-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.24/README.md` & `toolfuse-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.24/pyproject.toml` & `toolfuse-0.1.25/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.24"
+version = "0.1.25"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 docstring-parser = "^0.15"
 urllib3 = "^1.26.0"
 python-dotenv = "^1.0.1"
 openai = "^1.12.0"
 toolcore = "^0.1.0"
+jsonschema = "^4.22.0"
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 recommonmark = "^0.7.1"
 flake8 = "^7.0.0"
 black = "^24.2.0"
```

### Comparing `toolfuse-0.1.24/toolfuse/base.py` & `toolfuse-0.1.25/toolfuse/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from abc import ABC
-from typing import List, Callable, Any, Dict, Optional, TypeVar, Type, Union
-from inspect import getdoc, getmodule
 import inspect
 import re
+from abc import ABC
 from importlib.metadata import version as pkgversion
+from inspect import getdoc, getmodule
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union
 
+from jsonschema import ValidationError, validate
 from toolcore import FunctionWrapper
+
 from .models import V1ToolRef
 
 
 class Action:
     """
     Represents an action that an agent can perform in an environment.
 
@@ -256,28 +258,30 @@
             action (Action): The Action instance representing the action to perform.
             *args: Variable length argument list for the action.
             **kwargs: Arbitrary keyword arguments for the action.
 
         Returns:
             Any: The result of the action execution, which can vary depending on the action.
         """
+        self._validate_parameters(action.schema, kwargs)
         return action(*args, **kwargs)
 
     def observe(self, observation: Observation, *args, **kwargs) -> Any:
         """
         Executes an observation with the provided arguments and keyword arguments.
 
         Args:
             observation (Observation): The Observation instance representing the observation to run.
             *args: Variable length argument list for the observation.
             **kwargs: Arbitrary keyword arguments for the observation.
 
         Returns:
             Any: The result of the observation execution, which can vary depending on the observation.
         """
+        self._validate_parameters(observation.schema, kwargs)
         if not isinstance(observation, Observation):
             raise ValueError(
                 "Actions are not observable. Use the 'use' method to perform an action."
             )
         return observation(*args, **kwargs)
 
     def json_schema(
@@ -303,14 +307,32 @@
                 out.append(action.schema)
         if not actions_only:
             for observation in self.observations():
                 if observation.name not in exclude_names:
                     out.append(observation.schema)
         return out
 
+    def _validate_parameters(
+        self, schema: Dict[str, Any], parameters: Dict[str, Any]
+    ) -> None:
+        """
+        Validates the provided parameters against the given schema.
+
+        Args:
+            schema (Dict[str, Any]): The schema defining the structure of the parameters.
+            parameters (Dict[str, Any]): The parameters to validate.
+
+        Raises:
+            ValidationError: If the parameters do not conform to the schema.
+        """
+        try:
+            validate(instance=parameters, schema=schema)
+        except ValidationError as e:
+            raise ValueError(f"Parameter validation error: {e.message}")
+
     def find_action(self, name: str) -> Optional[Action]:
         """
         Searches for an action or observation by name and returns it if found.
 
         This method checks both the actions and observations lists for a match.
 
         Args:
```

### Comparing `toolfuse-0.1.24/toolfuse/multi.py` & `toolfuse-0.1.25/toolfuse/multi.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.24/toolfuse/util.py` & `toolfuse-0.1.25/toolfuse/util.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.24/PKG-INFO` & `toolfuse-0.1.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.24
+Version: 0.1.25
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: jsonschema (>=4.22.0,<5.0.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: toolcore (>=0.1.0,<0.2.0)
 Requires-Dist: urllib3 (>=1.26.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <!-- PROJECT LOGO -->
```

