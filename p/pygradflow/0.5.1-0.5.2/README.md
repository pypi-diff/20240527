# Comparing `tmp/pygradflow-0.5.1.tar.gz` & `tmp/pygradflow-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.5.1.tar", max compression
+gzip compressed data, was "pygradflow-0.5.2.tar", max compression
```

## Comparing `pygradflow-0.5.1.tar` & `pygradflow-0.5.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0    10847 2024-05-24 15:00:26.570915 pygradflow-0.5.1/LICENSE
--rw-r--r--   0        0        0      984 2024-05-24 15:00:26.570915 pygradflow-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/active_set.py
--rw-r--r--   0        0        0     1016 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/callbacks.py
--rw-r--r--   0        0        0     4417 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/controller.py
--rw-r--r--   0        0        0     2431 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     9840 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/display.py
--rw-r--r--   0        0        0     6359 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/eval.py
--rw-r--r--   0        0        0     7472 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/implicit_func.py
--rw-r--r--   0        0        0        0 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/integration/__init__.py
--rw-r--r--   0        0        0     1173 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/integration/events.py
--rw-r--r--   0        0        0     3634 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/integration/flow.py
--rw-r--r--   0        0        0    16999 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/integration/integration_solver.py
--rw-r--r--   0        0        0     4330 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/integration/problem_switches.py
--rw-r--r--   0        0        0     3458 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/integration/restricted_flow.py
--rw-r--r--   0        0        0     6092 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/log.py
--rw-r--r--   0        0        0     9309 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/newton.py
--rw-r--r--   0        0        0     6017 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/py.typed
--rw-r--r--   0        0        0     1872 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/result.py
--rw-r--r--   0        0        0     4746 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      708 2024-05-24 15:00:26.570915 pygradflow-0.5.1/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2019 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     8600 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     7406 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/scale.py
--rw-r--r--   0        0        0    12377 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/solver.py
--rw-r--r--   0        0        0     1738 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/status.py
--rw-r--r--   0        0        0     1284 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     7831 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     3416 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/box_solver.py
--rw-r--r--   0        0        0     2710 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3101 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7326 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2691 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2476 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4713 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2917 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4024 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      492 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/timer.py
--rw-r--r--   0        0        0     3009 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/transform.py
--rw-r--r--   0        0        0     1043 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pygradflow/util.py
--rw-r--r--   0        0        0     1158 2024-05-24 15:00:26.574915 pygradflow-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-27 11:55:10.143766 pygradflow-0.5.2/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-27 11:55:10.143766 pygradflow-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/active_set.py
+-rw-r--r--   0        0        0     1016 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/callbacks.py
+-rw-r--r--   0        0        0     4417 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/controller.py
+-rw-r--r--   0        0        0     2431 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     9840 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/display.py
+-rw-r--r--   0        0        0     6359 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/eval.py
+-rw-r--r--   0        0        0     7472 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/integration/__init__.py
+-rw-r--r--   0        0        0     1173 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/integration/events.py
+-rw-r--r--   0        0        0     3634 2024-05-27 11:55:10.143766 pygradflow-0.5.2/pygradflow/integration/flow.py
+-rw-r--r--   0        0        0    16999 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/integration/integration_solver.py
+-rw-r--r--   0        0        0     4330 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/integration/problem_switches.py
+-rw-r--r--   0        0        0     3458 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/integration/restricted_flow.py
+-rw-r--r--   0        0        0     6092 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/log.py
+-rw-r--r--   0        0        0     9309 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/newton.py
+-rw-r--r--   0        0        0     6017 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/py.typed
+-rw-r--r--   0        0        0     1872 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/result.py
+-rw-r--r--   0        0        0     4746 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      708 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2157 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/runners/mps_runner.py
+-rw-r--r--   0        0        0     2015 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     8600 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     7406 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/scale.py
+-rw-r--r--   0        0        0    12377 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/solver.py
+-rw-r--r--   0        0        0     1738 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/status.py
+-rw-r--r--   0        0        0     1284 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4274 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     7831 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     3416 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/box_solver.py
+-rw-r--r--   0        0        0     2710 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2431 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2058 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3101 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      543 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7326 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2014 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2691 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2476 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4713 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2917 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4024 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      492 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/timer.py
+-rw-r--r--   0        0        0     3009 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/transform.py
+-rw-r--r--   0        0        0     1043 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pygradflow/util.py
+-rw-r--r--   0        0        0     1175 2024-05-27 11:55:10.147766 pygradflow-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.5.2/PKG-INFO
```

### Comparing `pygradflow-0.5.1/LICENSE` & `pygradflow-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/README.md` & `pygradflow-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/active_set.py` & `pygradflow-0.5.2/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/callbacks.py` & `pygradflow-0.5.2/pygradflow/callbacks.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/cons_problem.py` & `pygradflow-0.5.2/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/controller.py` & `pygradflow-0.5.2/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/deriv_check.py` & `pygradflow-0.5.2/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/display.py` & `pygradflow-0.5.2/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/eval.py` & `pygradflow-0.5.2/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/implicit_func.py` & `pygradflow-0.5.2/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/integration/events.py` & `pygradflow-0.5.2/pygradflow/integration/events.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/integration/flow.py` & `pygradflow-0.5.2/pygradflow/integration/flow.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/integration/integration_solver.py` & `pygradflow-0.5.2/pygradflow/integration/integration_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/integration/problem_switches.py` & `pygradflow-0.5.2/pygradflow/integration/problem_switches.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/integration/restricted_flow.py` & `pygradflow-0.5.2/pygradflow/integration/restricted_flow.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/iterate.py` & `pygradflow-0.5.2/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/newton.py` & `pygradflow-0.5.2/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/params.py` & `pygradflow-0.5.2/pygradflow/params.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/penalty.py` & `pygradflow-0.5.2/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/problem.py` & `pygradflow-0.5.2/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/result.py` & `pygradflow-0.5.2/pygradflow/result.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/runners/cutest_runner.py` & `pygradflow-0.5.2/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/runners/instance.py` & `pygradflow-0.5.2/pygradflow/runners/instance.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/runners/qplib_runner.py` & `pygradflow-0.5.2/pygradflow/runners/qplib_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,18 @@
     def cons_jac(self, x):
         return self.problem.cons_jac(x)
 
     def lag_hess(self, x, y):
         return self.problem.lag_hess(x, y)
 
     def x0(self):
-        return self.problem.x0()
+        return self.problem.x0
 
     def y0(self):
-        return self.problem.y0()
+        return self.problem.y0
 
 
 class QPLIBInstance(Instance):
     def __init__(self, description):
         self.description = description
 
         super().__init__(description.name, description.num_vars, description.num_cons)
```

### Comparing `pygradflow-0.5.1/pygradflow/runners/runner.py` & `pygradflow-0.5.2/pygradflow/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/scale.py` & `pygradflow-0.5.2/pygradflow/scale.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/solver.py` & `pygradflow-0.5.2/pygradflow/solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/status.py` & `pygradflow-0.5.2/pygradflow/status.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/__init__.py` & `pygradflow-0.5.2/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.5.2/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/box_control.py` & `pygradflow-0.5.2/pygradflow/step/box_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/box_solver.py` & `pygradflow-0.5.2/pygradflow/step/box_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/cond_estimate.py` & `pygradflow-0.5.2/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.5.2/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/exact_control.py` & `pygradflow-0.5.2/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/extended_step_solver.py` & `pygradflow-0.5.2/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/fixed_control.py` & `pygradflow-0.5.2/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/linear_solver.py` & `pygradflow-0.5.2/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/opti_control.py` & `pygradflow-0.5.2/pygradflow/step/opti_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.5.2/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.5.2/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/standard_step_solver.py` & `pygradflow-0.5.2/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/step_control.py` & `pygradflow-0.5.2/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/step_solver.py` & `pygradflow-0.5.2/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.5.2/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/transform.py` & `pygradflow-0.5.2/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pygradflow/util.py` & `pygradflow-0.5.2/pygradflow/util.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.1/pyproject.toml` & `pygradflow-0.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.5.1"
+version = "0.5.2"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
 
 
@@ -21,14 +21,15 @@
 pytest = "^7.4.0"
 pytest-isort = "^3.1.0"
 pytest-black = "^0.3.12"
 mypy = "^1.7.1"
 types-pyyaml = "^6.0.12"
 pytest-timeout = "^2.3.1"
 pyflakes = "^3.2.0"
+mpspy = "^0.1.3"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 
 [tool.poetry.group.bench]
 optional = true
```

### Comparing `pygradflow-0.5.1/PKG-INFO` & `pygradflow-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.5.1
+Version: 0.5.2
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

