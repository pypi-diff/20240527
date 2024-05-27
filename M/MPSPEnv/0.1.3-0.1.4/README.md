# Comparing `tmp/mpspenv-0.1.3.tar.gz` & `tmp/mpspenv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpspenv-0.1.3.tar", last modified: Wed May 22 09:32:28 2024, max compression
+gzip compressed data, was "mpspenv-0.1.4.tar", last modified: Mon May 27 16:22:25 2024, max compression
```

## Comparing `mpspenv-0.1.3.tar` & `mpspenv-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469648 mpspenv-0.1.3/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-05-07 12:14:46.000000 mpspenv-0.1.3/MANIFEST.in
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.466798 mpspenv-0.1.3/MPSPEnv/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       46 2024-05-17 13:25:45.000000 mpspenv-0.1.3/MPSPEnv/__init__.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.465975 mpspenv-0.1.3/MPSPEnv/c/
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469007 mpspenv-0.1.3/MPSPEnv/c/src/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3686 2024-05-20 17:10:52.000000 mpspenv-0.1.3/MPSPEnv/c/src/array.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      738 2024-05-20 17:18:13.000000 mpspenv-0.1.3/MPSPEnv/c/src/array.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7721 2024-05-20 16:39:13.000000 mpspenv-0.1.3/MPSPEnv/c/src/bay.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      861 2024-05-20 12:41:08.000000 mpspenv-0.1.3/MPSPEnv/c/src/bay.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)    10139 2024-05-22 09:25:42.000000 mpspenv-0.1.3/MPSPEnv/c/src/env.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      615 2024-05-22 09:26:14.000000 mpspenv-0.1.3/MPSPEnv/c/src/env.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1694 2024-05-20 16:47:49.000000 mpspenv-0.1.3/MPSPEnv/c/src/random.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      204 2024-05-20 16:48:38.000000 mpspenv-0.1.3/MPSPEnv/c/src/random.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1472 2024-05-20 16:30:09.000000 mpspenv-0.1.3/MPSPEnv/c/src/sort.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 mpspenv-0.1.3/MPSPEnv/c/src/sort.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     6456 2024-05-20 17:06:41.000000 mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1027 2024-05-20 17:05:53.000000 mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1909 2024-05-22 09:21:19.000000 mpspenv-0.1.3/MPSPEnv/c_interface.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7469 2024-05-22 09:22:28.000000 mpspenv-0.1.3/MPSPEnv/env.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     4927 2024-05-20 17:19:49.000000 mpspenv-0.1.3/MPSPEnv/visualizer.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469269 mpspenv-0.1.3/MPSPEnv.egg-info/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)      570 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/SOURCES.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/dependency_links.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/requires.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/top_level.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-22 09:32:28.469450 mpspenv-0.1.3/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)     2848 2024-05-20 11:08:18.000000 mpspenv-0.1.3/README.md
--rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-05-22 09:32:28.469690 mpspenv-0.1.3/setup.cfg
--rw-r--r--   0 axelhojmark   (501) staff       (20)      890 2024-05-22 09:32:12.000000 mpspenv-0.1.3/setup.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469129 mpspenv-0.1.3/tests/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     2503 2024-05-22 09:22:28.000000 mpspenv-0.1.3/tests/test_env.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-27 16:22:25.381624 mpspenv-0.1.4/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-05-07 12:14:46.000000 mpspenv-0.1.4/MANIFEST.in
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-27 16:22:25.377557 mpspenv-0.1.4/MPSPEnv/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       46 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/__init__.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-27 16:22:25.376167 mpspenv-0.1.4/MPSPEnv/c/
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-27 16:22:25.380803 mpspenv-0.1.4/MPSPEnv/c/src/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3686 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/array.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      738 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/array.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7721 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/bay.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      861 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/bay.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)    10183 2024-05-27 16:14:39.000000 mpspenv-0.1.4/MPSPEnv/c/src/env.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      619 2024-05-27 16:10:38.000000 mpspenv-0.1.4/MPSPEnv/c/src/env.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1694 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/random.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      204 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/random.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1472 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/sort.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 mpspenv-0.1.4/MPSPEnv/c/src/sort.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     6456 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/transportation_matrix.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1027 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/c/src/transportation_matrix.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2012 2024-05-27 16:10:53.000000 mpspenv-0.1.4/MPSPEnv/c_interface.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7352 2024-05-27 16:10:28.000000 mpspenv-0.1.4/MPSPEnv/env.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     4927 2024-05-27 12:22:06.000000 mpspenv-0.1.4/MPSPEnv/visualizer.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-27 16:22:25.381240 mpspenv-0.1.4/MPSPEnv.egg-info/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-27 16:22:25.000000 mpspenv-0.1.4/MPSPEnv.egg-info/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      570 2024-05-27 16:22:25.000000 mpspenv-0.1.4/MPSPEnv.egg-info/SOURCES.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-05-27 16:22:25.000000 mpspenv-0.1.4/MPSPEnv.egg-info/dependency_links.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-05-27 16:22:25.000000 mpspenv-0.1.4/MPSPEnv.egg-info/requires.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-05-27 16:22:25.000000 mpspenv-0.1.4/MPSPEnv.egg-info/top_level.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-27 16:22:25.381441 mpspenv-0.1.4/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2848 2024-05-27 12:22:06.000000 mpspenv-0.1.4/README.md
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-05-27 16:22:25.381666 mpspenv-0.1.4/setup.cfg
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      890 2024-05-27 16:22:09.000000 mpspenv-0.1.4/setup.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-27 16:22:25.380980 mpspenv-0.1.4/tests/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2503 2024-05-27 16:22:01.000000 mpspenv-0.1.4/tests/test_env.py
```

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/array.c` & `mpspenv-0.1.4/MPSPEnv/c/src/array.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/array.h` & `mpspenv-0.1.4/MPSPEnv/c/src/array.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/bay.c` & `mpspenv-0.1.4/MPSPEnv/c/src/bay.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/bay.h` & `mpspenv-0.1.4/MPSPEnv/c/src/bay.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/env.c` & `mpspenv-0.1.4/MPSPEnv/c/src/env.c`

 * *Files 6% similar despite different names*

```diff
@@ -41,23 +41,22 @@
     return output;
 }
 
 int compute_mask_entry(Env env, int i, int empty_spots_to_left, Array identical_columns)
 {
     // RULE 1: The current number of containers plus the number of containers to add must be less than or equal to R
     // RULE 2: The current number of containers minus the number of containers to remove must be greater than or equal to 0
-    // RULE 3: If there is only one available action, the env does it automatically
-    // RULE 4: You may only add one type of container at a time (i.e. you cant add 2x2s and 2x5s in a column at the same time)
-    // The rules below assumes that columns are sorted in priority of 1. Increasing Column height 2. Increasing lexigraphical order
-    // RULE 5: You may only remove if you have not yet added containers (resets after sailing)
-    // RULE 6: You may only add to a column that is to the left of the last column you added to (resets after each container type)
-    // RULE 7: You may only remove from a column that is to the right of the last column you removed from (resets after sailing)
-    // RULE 8: You may not take an action that leaves no options for the next action
-    // RULE 9: If two columns are identical, you may only add to the rightmost column
-    // RULE 10: If two columns are identical, you may only remove from the leftmost column
+    // RULE 3: You may only add one type of container at a time (i.e. you cant add 2x2s and 2x5s in a column at the same time)
+    // The rules below assumes that columns are sorted occarding the values in the rows from bottom to top:
+    // RULE 4: You may only remove if you have not yet added containers (resets after sailing)
+    // RULE 5: You may only add to a column that is to the left of the last column you added to (resets after each container type)
+    // RULE 6: You may only remove from a column that is to the right of the last column you removed from (resets after sailing)
+    // RULE 7: You may not take an action that leaves no options for the next action
+    // RULE 8: If two columns are identical, you may only add to the rightmost column
+    // RULE 9: If two columns are identical, you may only remove from the leftmost column
 
     // Action space is column major order:
     // [c0r1, c0r2, c0r3, …, c0rR, c1r1, c1r2, …, c2*C-1rR]
     int is_add = i < env.bay.C * env.bay.R;
     int column = (i / env.bay.R) % env.bay.C;
     int n_to_place = i % env.bay.R + 1;
     int n_of_type = env.T->matrix.values[env.T->last_non_zero_column];
@@ -119,54 +118,14 @@
     }
     if (n_legal_actions == 1)
         return last_legal_action;
     else
         return -1;
 }
 
-Env build_env(int R, int C, int N, int auto_move, Transportation_Info *T)
-{
-    assert(R > 0 && C > 0 && N > 0);
-    assert(auto_move == 0 || auto_move == 1);
-    Env env;
-
-    env.auto_move = auto_move;
-    env.bay = get_bay(R, C, N);
-    env.T = T;
-    env.mask = get_zeros(2 * env.bay.R * env.bay.C);
-    env.total_reward = malloc(sizeof(int));
-    *env.total_reward = 0;
-    env.containers_placed = malloc(sizeof(int));
-    *env.containers_placed = 0;
-    env.containers_left = malloc(sizeof(int));
-    *env.containers_left = get_sum(T->matrix);
-    env.terminated = malloc(sizeof(int));
-    *env.terminated = 0;
-
-    int only_legal_action = insert_mask(env);
-    if (auto_move && only_legal_action != -1)
-    {
-        step(env, only_legal_action);
-    }
-
-    return env;
-}
-
-Env get_random_env(int R, int C, int N, int auto_move)
-{
-    Transportation_Info *T = get_random_transportation_matrix(N, R * C);
-    return build_env(R, C, N, auto_move, T);
-}
-
-Env get_specific_env(int R, int C, int N, int *T_matrix, int auto_move)
-{
-    Transportation_Info *T = get_specific_transportation_matrix(N, T_matrix);
-    return build_env(R, C, N, auto_move, T);
-}
-
 Env copy_env(Env env)
 {
     Env copy;
     copy.T = copy_transportation_info(env.T);
     copy.bay = copy_bay(env.bay);
     copy.mask = copy_array(env.mask);
     copy.auto_move = env.auto_move;
@@ -283,23 +242,67 @@
 
     if (is_adding_container)
         return add_container(env, action);
     else
         return remove_container(env, action);
 }
 
-StepInfo step(Env env, int action)
+StepInfo env_step(Env env, int action)
 {
     assert(action >= 0 && action < 2 * env.bay.C * env.bay.R);
     assert(env.mask.values[action] == 1);
     StepInfo step_info;
     step_info.reward = step_action(env, action);
     step_info.terminated = decide_is_terminated(env);
     *env.terminated = step_info.terminated;
     *env.total_reward += step_info.reward;
 
     int only_legal_action = insert_mask(env);
     if (env.auto_move && !step_info.terminated && only_legal_action != -1)
-        return step(env, only_legal_action);
+    {
+        StepInfo next_step_info = env_step(env, only_legal_action);
+        step_info.reward += next_step_info.reward;
+        step_info.terminated = next_step_info.terminated;
+    }
 
     return step_info;
-}
+}
+
+Env build_env(int R, int C, int N, int auto_move, Transportation_Info *T)
+{
+    assert(R > 0 && C > 0 && N > 0);
+    assert(auto_move == 0 || auto_move == 1);
+    Env env;
+
+    env.auto_move = auto_move;
+    env.bay = get_bay(R, C, N);
+    env.T = T;
+    env.mask = get_zeros(2 * env.bay.R * env.bay.C);
+    env.total_reward = malloc(sizeof(int));
+    *env.total_reward = 0;
+    env.containers_placed = malloc(sizeof(int));
+    *env.containers_placed = 0;
+    env.containers_left = malloc(sizeof(int));
+    *env.containers_left = get_sum(T->matrix);
+    env.terminated = malloc(sizeof(int));
+    *env.terminated = 0;
+
+    int only_legal_action = insert_mask(env);
+    if (auto_move && only_legal_action != -1)
+    {
+        env_step(env, only_legal_action);
+    }
+
+    return env;
+}
+
+Env get_random_env(int R, int C, int N, int auto_move)
+{
+    Transportation_Info *T = get_random_transportation_matrix(N, R * C);
+    return build_env(R, C, N, auto_move, T);
+}
+
+Env get_specific_env(int R, int C, int N, int *T_matrix, int auto_move)
+{
+    Transportation_Info *T = get_specific_transportation_matrix(N, T_matrix);
+    return build_env(R, C, N, auto_move, T);
+}
```

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/env.h` & `mpspenv-0.1.4/MPSPEnv/c/src/env.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 typedef struct StepInfo
 {
     int terminated;
     int reward;
 } StepInfo;
 
-StepInfo step(Env env, int action);
+StepInfo env_step(Env env, int action);
 
 Env copy_env(Env env);
 
 Env get_random_env(int R, int C, int N, int auto_move);
 
 Env get_specific_env(int R, int C, int N, int *T_matrix, int auto_move);
```

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/random.c` & `mpspenv-0.1.4/MPSPEnv/c/src/random.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/sort.c` & `mpspenv-0.1.4/MPSPEnv/c/src/sort.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.c` & `mpspenv-0.1.4/MPSPEnv/c/src/transportation_matrix.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.h` & `mpspenv-0.1.4/MPSPEnv/c/src/transportation_matrix.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv/c_interface.py` & `mpspenv-0.1.4/MPSPEnv/c_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,20 +61,24 @@
 
 if len(c_lib_files) == 0:
     raise FileNotFoundError("Can't find C library")
 
 c_lib_path = c_lib_files[0]
 c_lib = ctypes.CDLL(c_lib_path)
 
-c_lib.step.argtypes = [Env, c_int]
-c_lib.step.restype = StepInfo
+c_lib.env_step.argtypes = [Env, c_int]
+c_lib.env_step.restype = StepInfo
 
 c_lib.get_random_env.argtypes = [c_int, c_int, c_int, c_int]
 c_lib.get_random_env.restype = Env
 
 c_lib.get_specific_env.argtypes = [c_int, c_int, c_int, POINTER(c_int), c_int]
 c_lib.get_specific_env.restype = Env
 
 c_lib.free_env.argtypes = [Env]
+c_lib.free_env.restype = None
 
 c_lib.copy_env.argtypes = [Env]
 c_lib.copy_env.restype = Env
+
+c_lib.set_seed.argtypes = [c_int]
+c_lib.set_seed.restype = None
```

### Comparing `mpspenv-0.1.3/MPSPEnv/env.py` & `mpspenv-0.1.4/MPSPEnv/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,24 +61,23 @@
         self.auto_move = auto_move
         self.speedy = speedy
 
     def step(self, action: int):
         assert self._env is not None, "The environment must be reset before stepping."
         self._check_action(action)
 
-        step_info = c_lib.step(self._env, action)
-        reward = step_info.reward
+        step_info = c_lib.env_step(self._env, action)
 
         if self.speedy:
             return None
         else:
             return (
                 self._get_observation(),
-                reward,
-                self.terminated,
+                step_info.reward,
+                step_info.terminated,
                 False,
                 {},
             )
 
     def copy(self):
         new_env = Env(
             R=self.R,
@@ -201,27 +200,25 @@
 
         return True
 
     def _get_observation(self):
         return {"bay": self.bay, "T": self.T, "mask": self.mask}
 
     def _reset_random_c_env(self, seed: int = None):
-        if self._env is not None:
-            c_lib.free_env(self._env)
+        self.close()
 
         if seed is not None:
             c_lib.set_seed(seed)
         else:
             c_lib.set_seed(np.random.randint(0, 2**32))
 
         self._env = c_lib.get_random_env(self.R, self.C, self.N, int(self.auto_move))
 
     def _reset_specific_c_env(self, transportation: np.ndarray):
-        if self._env is not None:
-            c_lib.free_env(self._env)
+        self.close()
 
         self._env = c_lib.get_specific_env(
             self.R,
             self.C,
             self.N,
             transportation.ctypes.data_as(ctypes.POINTER(ctypes.c_int)),
             int(self.auto_move),
@@ -239,11 +236,11 @@
             self.bay_store.ndarray.tobytes()
             + self.T_store.ndarray.tobytes()
             + self.mask_store.ndarray.tobytes()
         )
 
     def __eq__(self, other: "Env"):
         return (
-            np.array_equal(self.bay_store.ndarray, other.bay_store.ndarray)
+            np.array_equal(self.mask_store.ndarray, other.mask_store.ndarray)
+            and np.array_equal(self.bay_store.ndarray, other.bay_store.ndarray)
             and np.array_equal(self.T_store.ndarray, other.T_store.ndarray)
-            and np.array_equal(self.mask_store.ndarray, other.mask_store.ndarray)
         )
```

### Comparing `mpspenv-0.1.3/MPSPEnv/visualizer.py` & `mpspenv-0.1.4/MPSPEnv/visualizer.py`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/MPSPEnv.egg-info/PKG-INFO` & `mpspenv-0.1.4/MPSPEnv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.1.3
+Version: 0.1.4
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `mpspenv-0.1.3/MPSPEnv.egg-info/SOURCES.txt` & `mpspenv-0.1.4/MPSPEnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/PKG-INFO` & `mpspenv-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.1.3
+Version: 0.1.4
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `mpspenv-0.1.3/README.md` & `mpspenv-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.3/setup.py` & `mpspenv-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MPSPEnv",
-    version="0.1.3",
+    version="0.1.4",
     author="Axel Højmark",
     author_email="axelhojmark@gmail.com",
     description="A reinforcement learning environment for the Multi Port Stowage Planning problem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[ext_modules],
     packages=["MPSPEnv"],
```

### Comparing `mpspenv-0.1.3/tests/test_env.py` & `mpspenv-0.1.4/tests/test_env.py`

 * *Files identical despite different names*

