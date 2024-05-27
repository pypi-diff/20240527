# Comparing `tmp/mentabotix-0.1.5.4.tar.gz` & `tmp/mentabotix-0.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.4.tar", last modified: Sun May 26 15:19:34 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.5.tar", last modified: Sun May 26 16:09:30 2024, max compression
```

## Comparing `mentabotix-0.1.5.4.tar` & `mentabotix-0.1.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1066 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/README.md
--rw-r--r--   0        0        0      613 2024-05-26 15:19:34.993597 mentabotix-0.1.5.4/pyproject.toml
--rw-r--r--   0        0        0     1198 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    76370 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0    20809 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-26 15:19:07.810079 mentabotix-0.1.5.4/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0      867 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/src/mentabotix/tools/selectors.py
--rw-r--r--   0        0        0        0 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_botix.py
--rw-r--r--   0        0        0     2525 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_case_registry.py
--rw-r--r--   0        0        0    11417 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_menta.py
--rw-r--r--   0        0        0     9975 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_moving_state.py
--rw-r--r--   0        0        0     7475 2024-05-26 15:19:07.814079 mentabotix-0.1.5.4/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/README.md
+-rw-r--r--   0        0        0      613 2024-05-26 16:09:30.207777 mentabotix-0.1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1301 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    76370 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    20857 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0      867 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/tools/selectors.py
+-rw-r--r--   0        0        0        0 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/find_tests.py
+-rw-r--r--   0        0        0    15660 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_botix.py
+-rw-r--r--   0        0        0     2525 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_case_registry.py
+-rw-r--r--   0        0        0    11417 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_menta.py
+-rw-r--r--   0        0        0     9975 2024-05-26 16:09:07.420082 mentabotix-0.1.5.5/tests/test_moving_state.py
+-rw-r--r--   0        0        0     7475 2024-05-26 16:09:07.420082 mentabotix-0.1.5.5/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.5/PKG-INFO
```

### Comparing `mentabotix-0.1.5.4/LICENSE` & `mentabotix-0.1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/README.md` & `mentabotix-0.1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/pyproject.toml` & `mentabotix-0.1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.5.4"
+version = "0.1.5.5"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.5.4/src/mentabotix/__init__.py` & `mentabotix-0.1.5.5/src/mentabotix/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     CaseRegistry,
     straight_chain,
     snaking_chain,
     scanning_chain,
     random_lr_turn_branch,
 )
 from .tools.generators import NameGenerator, Multipliers, make_multiplier_generator
-
+from .tools.selectors import make_weighted_selector
 
 __all__ = [
     "set_log_level",
     # botix
     "MovingState",
     "MovingTransition",
     "Botix",
@@ -40,8 +40,10 @@
     "straight_chain",
     "snaking_chain",
     "scanning_chain",
     "random_lr_turn_branch",
     # tools/generators
     "NameGenerator",
     "Multipliers",
+    # tools/selectors
+    "make_weighted_selector",
 ]
```

### Comparing `mentabotix-0.1.5.4/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.5/src/mentabotix/modules/botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.5/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.5/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/src/mentabotix/tools/composers.py` & `mentabotix-0.1.5.5/src/mentabotix/tools/composers.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,19 @@
     Args:
         case_dict (Dict[KT, MovingState]): A dictionary mapping keys of type KT to MovingState objects. Defaults to an empty dictionary if not provided.
         to_cover (Type[Enum]): The enumeration type to cover.
 
 
     """
 
-    def __init__(self, case_dict: Dict[KT, MovingState], to_cover: Type[Enum]):
+    def __init__(
+        self,
+        to_cover: Type[Enum],
+        case_dict: Optional[Dict[KT, MovingState]] = None,
+    ):
         self._case_dict: Dict[KT, MovingState] = case_dict or {}
         self._to_cover: Type[Enum] = to_cover
 
     @property
     def case_dict(self) -> Dict[KT, MovingState]:
         """
```

### Comparing `mentabotix-0.1.5.4/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.5/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/src/mentabotix/tools/selectors.py` & `mentabotix-0.1.5.5/src/mentabotix/tools/selectors.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/tests/find_tests.py` & `mentabotix-0.1.5.5/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/tests/test_botix.py` & `mentabotix-0.1.5.5/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/tests/test_case_registry.py` & `mentabotix-0.1.5.5/tests/test_case_registry.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/tests/test_composer.py` & `mentabotix-0.1.5.5/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/tests/test_menta.py` & `mentabotix-0.1.5.5/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/tests/test_moving_state.py` & `mentabotix-0.1.5.5/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/tests/test_moving_transition.py` & `mentabotix-0.1.5.5/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.4/PKG-INFO` & `mentabotix-0.1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5.4
+Version: 0.1.5.5
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
```

