# Comparing `tmp/mentabotix-0.1.5.5.tar.gz` & `tmp/mentabotix-0.1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.5.tar", last modified: Sun May 26 16:09:30 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.6.tar", last modified: Mon May 27 09:37:59 2024, max compression
```

## Comparing `mentabotix-0.1.5.5.tar` & `mentabotix-0.1.5.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1066 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/README.md
--rw-r--r--   0        0        0      613 2024-05-26 16:09:30.207777 mentabotix-0.1.5.5/pyproject.toml
--rw-r--r--   0        0        0     1301 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    76370 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0    20857 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0      867 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/src/mentabotix/tools/selectors.py
--rw-r--r--   0        0        0        0 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_botix.py
--rw-r--r--   0        0        0     2525 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_case_registry.py
--rw-r--r--   0        0        0    11417 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-26 16:09:07.416082 mentabotix-0.1.5.5/tests/test_menta.py
--rw-r--r--   0        0        0     9975 2024-05-26 16:09:07.420082 mentabotix-0.1.5.5/tests/test_moving_state.py
--rw-r--r--   0        0        0     7475 2024-05-26 16:09:07.420082 mentabotix-0.1.5.5/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-27 09:37:33.447224 mentabotix-0.1.5.6/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-27 09:37:33.447224 mentabotix-0.1.5.6/README.md
+-rw-r--r--   0        0        0      613 2024-05-27 09:37:59.531376 mentabotix-0.1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1301 2024-05-27 09:37:33.447224 mentabotix-0.1.5.6/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    76369 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    20857 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0      867 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/tools/selectors.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/find_tests.py
+-rw-r--r--   0        0        0    15660 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_botix.py
+-rw-r--r--   0        0        0     2521 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_case_registry.py
+-rw-r--r--   0        0        0    11493 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_menta.py
+-rw-r--r--   0        0        0     9973 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_moving_state.py
+-rw-r--r--   0        0        0     7475 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.6/PKG-INFO
```

### Comparing `mentabotix-0.1.5.5/LICENSE` & `mentabotix-0.1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/README.md` & `mentabotix-0.1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/pyproject.toml` & `mentabotix-0.1.5.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.5.5"
+version = "0.1.5.6"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.5.5/src/mentabotix/__init__.py` & `mentabotix-0.1.5.6/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.6/src/mentabotix/modules/botix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 from collections import Counter
 from dataclasses import dataclass
 from enum import Enum
 from itertools import zip_longest
 from queue import Queue
+from random import random
 from typing import (
     Tuple,
     TypeAlias,
     Self,
     Unpack,
     Literal,
     Any,
@@ -19,17 +20,17 @@
     List,
     ClassVar,
     Set,
     Sequence,
     get_type_hints,
 )
 
-import numpy as np
 from bdmc import CloseLoopController
-from numpy.random import random
+from numpy import array, full, int32, equal
+from numpy.random import choice
 from terminaltables import SingleTable
 
 from mentabotix.tools.selectors import make_weighted_selector
 from .exceptions import StructuralError, TokenizeError
 from .logger import _logger
 from ..tools.generators import NameGenerator
 
@@ -232,15 +233,15 @@
             used_context_variables (Optional[List[str]]): The set of context variable names used in the speed expressions.
             before_entering (Optional[List[Callable[[], None]]]): The list of functions to be called before entering the state.
             after_exiting (Optional[List[Callable[[], None]]]): The list of functions to be called after exiting the state.
         Raises:
             ValueError: If the provided speeds do not match any of the above patterns.
         """
         self._speed_expressions: IndividualExpressionPattern
-        self._speeds: np.array
+        self._speeds: array
         self._pattern_type: PatternType
         match bool(speed_expressions), bool(speeds):
             case True, False:
                 if used_context_variables is None:
                     raise ValueError(
                         "No used_context_variables provided, You must provide a names set that contains all the name of the variables used in the speed_expressions."
                         "If you do not need use context variables, then you should use *speeds argument to create the MovingState."
@@ -271,23 +272,23 @@
                         )
 
             case False, True:
                 self._speed_expressions = None
                 match speeds:
                     case (int(full_speed),):
                         self._pattern_type = PatternType.Full
-                        self._speeds = np.full((4,), full_speed)
+                        self._speeds = full((4,), full_speed)
                     case (int(left_speed), int(right_speed)):
                         self._pattern_type = PatternType.LR
 
-                        self._speeds = np.array([left_speed, left_speed, right_speed, right_speed])
+                        self._speeds = array([left_speed, left_speed, right_speed, right_speed])
                     case speeds if len(speeds) == 4 and all(isinstance(item, int) for item in speeds):
                         self._pattern_type = PatternType.Individual
 
-                        self._speeds = np.array(speeds)
+                        self._speeds = array(speeds)
                     case _:
                         types = tuple(type(item) for item in speeds)
                         raise ValueError(
                             f"Invalid Speeds. Must be one of [{FullPattern},{LRPattern},{IndividualPattern}], got {types}"
                         )
             case True, True:
                 raise ValueError(
@@ -468,15 +469,14 @@
             Self: An instance of the class configured with the random turning behavior.
         """
         if any(num < 0 for num in turn_speeds):
             _logger.warn(
                 f"All turn speeds should be positive, got {turn_speeds}. "
                 f"Since you should not using the turn left with negative speed to represent turn right."
             )
-        from random import choice
 
         match direction:
             case "l":
                 direction = 1
             case "r":
                 direction = -1
             case _:
@@ -573,15 +573,15 @@
 
         Args:
             multiplier (float): The multiplier to apply to the speeds.
 
         Returns:
             Self: The modified object with the updated speeds.
         """
-        self._speeds = (self._speeds * multiplier).astype(np.int32)
+        self._speeds = (self._speeds * multiplier).astype(int32)
         return self
 
     def unwrap(self) -> Tuple[int, ...]:
         """
         Return the speeds of the MovingState object.
         """
         return tuple(self._speeds)
@@ -748,15 +748,15 @@
             return self._speed_expressions == other._speed_expressions
         elif self._speeds is None:
             return False
         elif other._speeds is None:
             return False
         else:
 
-            return all(np.equal(self._speeds, other._speeds)) and self._speed_expressions == other._speed_expressions
+            return all(equal(self._speeds, other._speeds)) and self._speed_expressions == other._speed_expressions
 
     def __str__(self):
         main_seq = self._speed_expressions if self._speeds is None else tuple(self._speeds)
         if all(main_seq[0] == x for x in main_seq[1:]):
             return f"{self._identifier}-MovingState({repr(main_seq[0])})"
         if main_seq[0] == main_seq[1] != main_seq[-1] == main_seq[-2]:
             return f"{self._identifier}-MovingState{main_seq[1:3]}"
```

### Comparing `mentabotix-0.1.5.5/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.6/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.6/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/src/mentabotix/tools/composers.py` & `mentabotix-0.1.5.6/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.6/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/src/mentabotix/tools/selectors.py` & `mentabotix-0.1.5.6/src/mentabotix/tools/selectors.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/tests/find_tests.py` & `mentabotix-0.1.5.6/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/tests/test_botix.py` & `mentabotix-0.1.5.6/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/tests/test_case_registry.py` & `mentabotix-0.1.5.6/tests/test_case_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     CASE1 = "case1"
     CASE2 = "case2"
     CASE3 = "case3"
 
 
 class TestCaseRegistry(unittest.TestCase):
     def setUp(self):
-        self.case_registry = CaseRegistry({}, TestEnum)
+        self.case_registry = CaseRegistry(TestEnum)
 
     def test_init(self):
         self.assertIsInstance(self.case_registry._case_dict, dict)
         self.assertEqual(self.case_registry._to_cover, TestEnum)
 
     def test_reassign(self):
         self.case_registry.reassign(TestEnum)
```

### Comparing `mentabotix-0.1.5.5/tests/test_composer.py` & `mentabotix-0.1.5.6/tests/test_composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,60 +100,63 @@
 
     # 测试没有breaker的情况
     def test_straight_chain_without_breaker(self):
         start_speed = 50
         end_speed = 100
         duration = 5.0
         power_exponent = 1.0
-        interval = 0.07
-
+        interval = 0.3
+        lead_time = 0
         # 调用待测试函数
         states, transitions = straight_chain(
             start_speed=start_speed,
             end_speed=end_speed,
             duration=duration,
             power_exponent=power_exponent,
             interval=interval,
+            lead_time=lead_time,
         )
 
         # 断言判断结果是否符合预期
-        self.assertEqual(len(states), int(duration / interval) + 1)
+        self.assertEqual(int(duration / interval) + 2, len(states))
         self.assertEqual(states[0].unwrap()[0], start_speed)
         self.assertEqual(states[-1].unwrap()[0], end_speed)
-        for i in range(len(transitions) - 1):
-            self.assertIsInstance(transitions[i], MovingTransition)
-            self.assertEqual(transitions[i].duration, interval)
+        for t in transitions[:-1]:
+            self.assertIsInstance(t, MovingTransition)
+            self.assertEqual(t.duration, interval)
+        self.assertAlmostEqual(duration - lead_time, sum(t.duration for t in transitions))
 
     # 测试有breaker函数的情况
     def test_straight_chain_with_breaker(self):
         start_speed = 50
         end_speed = 100
         duration = 5.0
         power_exponent = 1.0
         interval = 0.1
+        lead_time = 0.05
 
         def break_function() -> bool:
             return random.random() < 0.1
 
         # 调用待测试函数
         states, transitions = straight_chain(
             start_speed=start_speed,
             end_speed=end_speed,
             duration=duration,
             power_exponent=power_exponent,
             interval=interval,
+            lead_time=lead_time,
             breaker=break_function,
         )
 
         # 断言判断结果是否符合预期
         self.assertTrue(any(isinstance(t, MovingTransition) and t.breaker for t in transitions))
         self.assertEqual(int(duration / interval), len(transitions))
-        self.assertAlmostEqual(duration, sum(t.duration for t in transitions))
-        self.assertEqual(int(duration / interval) + 1 + 1, len(states))  # 包含了break状态
-        self.assertIn(MovingState(0), states)  # 确认state_on_break被加入到states列表中
+        self.assertAlmostEqual(duration - lead_time, sum(t.duration for t in transitions))
+        self.assertEqual(int(duration / interval) + 1, len(states))  # 包含了break状态
 
     def test_exp(self):
         start_speed = 50
         end_speed = 100
         duration = 5.0
         power_exponent = 2.0
         interval = 0.1
```

### Comparing `mentabotix-0.1.5.5/tests/test_menta.py` & `mentabotix-0.1.5.6/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/tests/test_moving_state.py` & `mentabotix-0.1.5.6/tests/test_moving_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         print(state)
         end = MovingState(0)
         trans = MovingTransition(1, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
-        for _ in range(10):
+        for _ in range(2):
             fun()
             sleep(0.2)
         con.stop_msg_sending()
         con.serial_client.close()
 
     def test_random_turn_spd_with_weights(self):
         from mentabotix import MovingTransition, Botix
@@ -221,15 +221,15 @@
         print(state)
         end = MovingState(0)
         trans = MovingTransition(1, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
-        for _ in range(20):
+        for _ in range(2):
             fun()
             sleep(0.2)
         con.stop_msg_sending()
         con.serial_client.close()
 
     def test_rand_turn_spd_dir_with_weights(self):
         from mentabotix import MovingTransition, Botix
```

### Comparing `mentabotix-0.1.5.5/tests/test_moving_transition.py` & `mentabotix-0.1.5.6/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.5/PKG-INFO` & `mentabotix-0.1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5.5
+Version: 0.1.5.6
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
```

