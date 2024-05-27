# Comparing `tmp/mentabotix-0.1.5.6.tar.gz` & `tmp/mentabotix-0.1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.5.6.tar", last modified: Mon May 27 09:37:59 2024, max compression
+gzip compressed data, was "mentabotix-0.1.5.7.tar", last modified: Mon May 27 10:06:53 2024, max compression
```

## Comparing `mentabotix-0.1.5.6.tar` & `mentabotix-0.1.5.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1066 2024-05-27 09:37:33.447224 mentabotix-0.1.5.6/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-27 09:37:33.447224 mentabotix-0.1.5.6/README.md
--rw-r--r--   0        0        0      613 2024-05-27 09:37:59.531376 mentabotix-0.1.5.6/pyproject.toml
--rw-r--r--   0        0        0     1301 2024-05-27 09:37:33.447224 mentabotix-0.1.5.6/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    76369 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0    20857 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0      867 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/src/mentabotix/tools/selectors.py
--rw-r--r--   0        0        0        0 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/find_tests.py
--rw-r--r--   0        0        0    15660 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_botix.py
--rw-r--r--   0        0        0     2521 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_case_registry.py
--rw-r--r--   0        0        0    11493 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_menta.py
--rw-r--r--   0        0        0     9973 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_moving_state.py
--rw-r--r--   0        0        0     7475 2024-05-27 09:37:33.451224 mentabotix-0.1.5.6/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-27 10:06:28.724521 mentabotix-0.1.5.7/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-27 10:06:28.724521 mentabotix-0.1.5.7/README.md
+-rw-r--r--   0        0        0      613 2024-05-27 10:06:53.284565 mentabotix-0.1.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1301 2024-05-27 10:06:28.724521 mentabotix-0.1.5.7/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    77701 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0    20857 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0      867 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/src/mentabotix/tools/selectors.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/find_tests.py
+-rw-r--r--   0        0        0    15660 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_botix.py
+-rw-r--r--   0        0        0     2521 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_case_registry.py
+-rw-r--r--   0        0        0    11493 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_menta.py
+-rw-r--r--   0        0        0    10694 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_moving_state.py
+-rw-r--r--   0        0        0     7475 2024-05-27 10:06:28.728521 mentabotix-0.1.5.7/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24152 1970-01-01 00:00:00.000000 mentabotix-0.1.5.7/PKG-INFO
```

### Comparing `mentabotix-0.1.5.6/LICENSE` & `mentabotix-0.1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/README.md` & `mentabotix-0.1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/pyproject.toml` & `mentabotix-0.1.5.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.5.6"
+version = "0.1.5.7"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.5.6/src/mentabotix/__init__.py` & `mentabotix-0.1.5.7/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/src/mentabotix/modules/botix.py` & `mentabotix-0.1.5.7/src/mentabotix/modules/botix.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,48 @@
 
         Returns:
             Self: A new instance of the class with the specified speed.
         """
         return cls(speed)
 
     @classmethod
+    def rand_spd_straight(
+        cls,
+        con: CloseLoopController,
+        speeds: Sequence[int],
+        weights: Optional[Sequence[float | int]] = None,
+        used_ctx_varname: str = "rand_speed",
+    ) -> Self:
+        """
+        Create a new instance of the class with a random speed.
+        Args:
+            con (CloseLoopController): CloseLoopController object, representing the instance to which the random turning control is applied.
+            speeds (Sequence[int]): A sequence of speeds.
+            weights (Optional[Sequence[float | int]]): Weights for each speed.
+            used_ctx_varname (str, optional): The name of the context variable to store the selected speed.
+
+        Returns:
+
+        """
+
+        # Register a context updater to update the turn direction before entering this behavior.
+        _updater = con.register_context_updater(
+            make_weighted_selector(speeds, weights) if weights else lambda: choice(speeds),
+            output_keys=[used_ctx_varname],
+            input_keys=[],
+        )
+
+        # Set speed expressions and actions before entering, implementing random turning.
+        return cls(
+            speed_expressions=used_ctx_varname,
+            used_context_variables=[used_ctx_varname],
+            before_entering=[_updater],
+        )
+
+    @classmethod
     def differential(cls, direction: Literal["l", "r"], radius: float, outer_speed: int) -> Self:
         """
         Create a new instance of the class with the specified differential movement.
         Let the bot make a differential movement with the specified radius and speed.
 
         Note:
             The outer speed is the speed of the outer wheel.
```

### Comparing `mentabotix-0.1.5.6/src/mentabotix/modules/logger.py` & `mentabotix-0.1.5.7/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/src/mentabotix/modules/menta.py` & `mentabotix-0.1.5.7/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/src/mentabotix/tools/composers.py` & `mentabotix-0.1.5.7/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/src/mentabotix/tools/generators.py` & `mentabotix-0.1.5.7/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/src/mentabotix/tools/selectors.py` & `mentabotix-0.1.5.7/src/mentabotix/tools/selectors.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/tests/find_tests.py` & `mentabotix-0.1.5.7/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/tests/test_botix.py` & `mentabotix-0.1.5.7/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/tests/test_case_registry.py` & `mentabotix-0.1.5.7/tests/test_case_registry.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/tests/test_composer.py` & `mentabotix-0.1.5.7/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/tests/test_menta.py` & `mentabotix-0.1.5.7/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/tests/test_moving_state.py` & `mentabotix-0.1.5.7/tests/test_moving_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,35 @@
         print(state)
         end = MovingState(0)
         trans = MovingTransition(1, from_states=[state], to_states={0: end})
 
         b = Botix(controller=con, token_pool=[trans])
 
         fun = b.compile()
-        for _ in range(20):
+        for _ in range(2):
+            fun()
+            sleep(0.2)
+        con.stop_msg_sending()
+        con.serial_client.close()
+
+    def test_rand_spd_straight_with_weights(self):
+        from mentabotix import MovingTransition, Botix
+
+        con = CloseLoopController(
+            [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM10", context={"var1": 10, "var2": 20}
+        ).start_msg_sending()
+        state = MovingState.rand_spd_straight(con, [500, 600, 700], weights=[10, 80, 10])
+        print(state)
+        end = MovingState(0)
+        trans = MovingTransition(1, from_states=[state], to_states={0: end})
+
+        b = Botix(controller=con, token_pool=[trans])
+
+        fun = b.compile()
+        for _ in range(2):
             fun()
             sleep(0.2)
         con.stop_msg_sending()
         con.serial_client.close()
 
 
 if __name__ == "__main__":
```

### Comparing `mentabotix-0.1.5.6/tests/test_moving_transition.py` & `mentabotix-0.1.5.7/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.5.6/PKG-INFO` & `mentabotix-0.1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.5.6
+Version: 0.1.5.7
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: terminaltables>=3.1.10
```

