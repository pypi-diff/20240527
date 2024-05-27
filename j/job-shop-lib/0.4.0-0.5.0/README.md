# Comparing `tmp/job_shop_lib-0.4.0.tar.gz` & `tmp/job_shop_lib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "job_shop_lib-0.4.0.tar", max compression
+gzip compressed data, was "job_shop_lib-0.5.0.tar", max compression
```

## Comparing `job_shop_lib-0.4.0.tar` & `job_shop_lib-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,48 @@
--rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.4.0/LICENSE
--rw-r--r--   0        0        0    11817 2024-04-24 20:06:27.816437 job_shop_lib-0.4.0/README.md
--rw-r--r--   0        0        0      582 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/__init__.py
--rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.4.0/job_shop_lib/base_solver.py
--rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.4.0/job_shop_lib/benchmarking/__init__.py
--rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.4.0/job_shop_lib/benchmarking/benchmark_instances.json
--rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.4.0/job_shop_lib/benchmarking/load_benchmark.py
--rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.4.0/job_shop_lib/cp_sat/__init__.py
--rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.4.0/job_shop_lib/cp_sat/ortools_solver.py
--rw-r--r--   0        0        0     1568 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/dispatching/__init__.py
--rw-r--r--   0        0        0    12394 2024-05-02 19:39:08.751972 job_shop_lib-0.4.0/job_shop_lib/dispatching/dispatcher.py
--rw-r--r--   0        0        0     4669 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/dispatching/dispatching_rule_solver.py
--rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.4.0/job_shop_lib/dispatching/dispatching_rules.py
--rw-r--r--   0        0        0     7267 2024-04-17 18:36:42.623252 job_shop_lib-0.4.0/job_shop_lib/dispatching/factories.py
--rw-r--r--   0        0        0      649 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/dispatching/history_tracker.py
--rw-r--r--   0        0        0     4378 2024-04-27 08:34:21.170127 job_shop_lib-0.4.0/job_shop_lib/dispatching/pruning_functions.py
--rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.4.0/job_shop_lib/exceptions.py
--rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.4.0/job_shop_lib/generators/__init__.py
--rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.4.0/job_shop_lib/generators/basic_generator.py
--rw-r--r--   0        0        0     5290 2024-04-25 17:39:57.821984 job_shop_lib-0.4.0/job_shop_lib/generators/transformations.py
--rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.4.0/job_shop_lib/graphs/__init__.py
--rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.4.0/job_shop_lib/graphs/build_agent_task_graph.py
--rw-r--r--   0        0        0     2877 2024-04-17 18:51:04.799505 job_shop_lib-0.4.0/job_shop_lib/graphs/build_disjunctive_graph.py
--rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.4.0/job_shop_lib/graphs/constants.py
--rw-r--r--   0        0        0     7404 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/graphs/job_shop_graph.py
--rw-r--r--   0        0        0     5613 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/graphs/node.py
--rw-r--r--   0        0        0    12801 2024-04-03 10:47:39.697352 job_shop_lib-0.4.0/job_shop_lib/job_shop_instance.py
--rw-r--r--   0        0        0     3916 2024-05-02 19:27:14.708781 job_shop_lib-0.4.0/job_shop_lib/operation.py
--rw-r--r--   0        0        0    10393 2024-05-02 19:27:14.708781 job_shop_lib-0.4.0/job_shop_lib/schedule.py
--rw-r--r--   0        0        0     3526 2024-05-02 19:27:14.708781 job_shop_lib-0.4.0/job_shop_lib/scheduled_operation.py
--rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.4.0/job_shop_lib/visualization/__init__.py
--rw-r--r--   0        0        0     8284 2024-04-26 16:30:40.546774 job_shop_lib-0.4.0/job_shop_lib/visualization/agent_task_graph.py
--rw-r--r--   0        0        0     6674 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/visualization/create_gif.py
--rw-r--r--   0        0        0     5905 2024-05-02 11:40:12.230468 job_shop_lib-0.4.0/job_shop_lib/visualization/disjunctive_graph.py
--rw-r--r--   0        0        0     4415 2024-04-17 18:52:22.519817 job_shop_lib-0.4.0/job_shop_lib/visualization/gantt_chart.py
--rw-r--r--   0        0        0     1352 2024-05-02 19:39:08.751972 job_shop_lib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    12624 1970-01-01 00:00:00.000000 job_shop_lib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.5.0/LICENSE
+-rw-r--r--   0        0        0    11732 2024-05-27 16:10:50.146667 job_shop_lib-0.5.0/README.md
+-rw-r--r--   0        0        0      582 2024-05-02 11:40:12.230468 job_shop_lib-0.5.0/job_shop_lib/__init__.py
+-rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.5.0/job_shop_lib/base_solver.py
+-rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.5.0/job_shop_lib/benchmarking/__init__.py
+-rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.5.0/job_shop_lib/benchmarking/benchmark_instances.json
+-rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.5.0/job_shop_lib/benchmarking/load_benchmark.py
+-rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.5.0/job_shop_lib/cp_sat/__init__.py
+-rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.5.0/job_shop_lib/cp_sat/ortools_solver.py
+-rw-r--r--   0        0        0     1568 2024-05-02 11:40:12.230468 job_shop_lib-0.5.0/job_shop_lib/dispatching/__init__.py
+-rw-r--r--   0        0        0    19299 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/dispatcher.py
+-rw-r--r--   0        0        0     4669 2024-05-02 11:40:12.230468 job_shop_lib-0.5.0/job_shop_lib/dispatching/dispatching_rule_solver.py
+-rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.5.0/job_shop_lib/dispatching/dispatching_rules.py
+-rw-r--r--   0        0        0     7267 2024-05-27 15:49:49.372064 job_shop_lib-0.5.0/job_shop_lib/dispatching/factories.py
+-rw-r--r--   0        0        0     1023 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/__init__.py
+-rw-r--r--   0        0        0     3302 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/composite_feature_observer.py
+-rw-r--r--   0        0        0     3804 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/duration_observer.py
+-rw-r--r--   0        0        0     6296 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/earliest_start_time_observer.py
+-rw-r--r--   0        0        0     1941 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/factory.py
+-rw-r--r--   0        0        0     3646 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/feature_observer.py
+-rw-r--r--   0        0        0     4086 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/is_completed_observer.py
+-rw-r--r--   0        0        0     1405 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/is_ready_observer.py
+-rw-r--r--   0        0        0     1477 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/is_scheduled_observer.py
+-rw-r--r--   0        0        0     1344 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/position_in_job_observer.py
+-rw-r--r--   0        0        0     1891 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/dispatching/feature_observers/remaining_operations_observer.py
+-rw-r--r--   0        0        0      649 2024-05-02 11:40:12.230468 job_shop_lib-0.5.0/job_shop_lib/dispatching/history_tracker.py
+-rw-r--r--   0        0        0     4378 2024-04-27 08:34:21.170127 job_shop_lib-0.5.0/job_shop_lib/dispatching/pruning_functions.py
+-rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.5.0/job_shop_lib/exceptions.py
+-rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.5.0/job_shop_lib/generators/__init__.py
+-rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.5.0/job_shop_lib/generators/basic_generator.py
+-rw-r--r--   0        0        0     5290 2024-04-25 17:39:57.821984 job_shop_lib-0.5.0/job_shop_lib/generators/transformations.py
+-rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.5.0/job_shop_lib/graphs/__init__.py
+-rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.5.0/job_shop_lib/graphs/build_agent_task_graph.py
+-rw-r--r--   0        0        0     3705 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/graphs/build_disjunctive_graph.py
+-rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.5.0/job_shop_lib/graphs/constants.py
+-rw-r--r--   0        0        0     7404 2024-05-02 11:40:12.230468 job_shop_lib-0.5.0/job_shop_lib/graphs/job_shop_graph.py
+-rw-r--r--   0        0        0     5613 2024-05-02 11:40:12.230468 job_shop_lib-0.5.0/job_shop_lib/graphs/node.py
+-rw-r--r--   0        0        0    16376 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/job_shop_instance.py
+-rw-r--r--   0        0        0     3916 2024-05-04 17:17:50.609022 job_shop_lib-0.5.0/job_shop_lib/operation.py
+-rw-r--r--   0        0        0    10393 2024-05-04 17:17:50.609022 job_shop_lib-0.5.0/job_shop_lib/schedule.py
+-rw-r--r--   0        0        0     3526 2024-05-09 11:47:22.643190 job_shop_lib-0.5.0/job_shop_lib/scheduled_operation.py
+-rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.5.0/job_shop_lib/visualization/__init__.py
+-rw-r--r--   0        0        0     8284 2024-04-26 16:30:40.546774 job_shop_lib-0.5.0/job_shop_lib/visualization/agent_task_graph.py
+-rw-r--r--   0        0        0     7186 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/visualization/create_gif.py
+-rw-r--r--   0        0        0     5905 2024-05-02 11:40:12.230468 job_shop_lib-0.5.0/job_shop_lib/visualization/disjunctive_graph.py
+-rw-r--r--   0        0        0     4412 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/job_shop_lib/visualization/gantt_chart.py
+-rw-r--r--   0        0        0     1361 2024-05-27 16:10:50.154667 job_shop_lib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    12582 1970-01-01 00:00:00.000000 job_shop_lib-0.5.0/PKG-INFO
```

### Comparing `job_shop_lib-0.4.0/LICENSE` & `job_shop_lib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/README.md` & `job_shop_lib-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ```python
 from job_shop_lib.benchmarking import load_benchmark_instance
 
 ft06 = load_benchmark_instance("ft06")
 ```
 
 The module `benchmarks` contains functions to load the instances from the file and return them as `JobShopInstance` objects without having to download them
-manually. The instances are stored in [benchmark_instances.json](job_shop_lib/benchmarks/benchmark_instances.json).
+manually.
 
 The contributions to this benchmark dataset are as follows:
 
 - `abz5-9`: by Adams et al. (1988).
 
 - `ft06`, `ft10`, `ft20`: by Fisher and Thompson (1963).
 
@@ -145,21 +145,23 @@
     MOST_OPERATION_REMAINING = "most_operation_remaining"
     RANDOM = "random"
 ```
 
 We can visualize the solution with a `DispatchingRuleSolver` as a gif:
 
 ```python
-from job_shop_lib.visualization import create_gif, get_plot_function
+from job_shop_lib.visualization import create_gif, plot_gantt_chart_wrapper
 from job_shop_lib.dispatching import DispatchingRuleSolver, DispatchingRule
 
 plt.style.use("ggplot")
 
 mwkr_solver = DispatchingRuleSolver("most_work_remaining")
-plot_function = get_plot_function(title="Solution with Most Work Remaining Rule")
+plot_function = plot_gantt_chart_wrapper(
+    title="Solution with Most Work Remaining Rule"
+)
 create_gif(
     gif_path="ft06_optimized.gif",
     instance=ft06,
     solver=mwkr_solver,
     plot_function=plot_function,
     fps=4,
 )
@@ -323,8 +325,8 @@
      large-scale job-shop problems," in Proceedings of the Second
      International Workshop on Parallel Problem Solving from Nature
      (PPSN'2), Brussels, Belgium, pp. 281–290, 1992.
 
  - E. Taillard, "Benchmarks for basic scheduling problems," European
      Journal of Operational Research, vol. 64, no. 2, pp. 278–285, 1993.
 
-- Park, Junyoung, Sanjar Bakhtiyar, and Jinkyoo Park. "ScheduleNet: Learn to solve multi-agent scheduling problems with reinforcement learning." arXiv preprint arXiv:2106.03051, 2021. 
+- Park, Junyoung, Sanjar Bakhtiyar, and Jinkyoo Park. "ScheduleNet: Learn to solve multi-agent scheduling problems with reinforcement learning." arXiv preprint arXiv:2106.03051, 2021.
```

### Comparing `job_shop_lib-0.4.0/job_shop_lib/__init__.py` & `job_shop_lib-0.5.0/job_shop_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/base_solver.py` & `job_shop_lib-0.5.0/job_shop_lib/base_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/benchmarking/__init__.py` & `job_shop_lib-0.5.0/job_shop_lib/benchmarking/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/benchmarking/benchmark_instances.json` & `job_shop_lib-0.5.0/job_shop_lib/benchmarking/benchmark_instances.json`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/benchmarking/load_benchmark.py` & `job_shop_lib-0.5.0/job_shop_lib/benchmarking/load_benchmark.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/cp_sat/ortools_solver.py` & `job_shop_lib-0.5.0/job_shop_lib/cp_sat/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/dispatching/__init__.py` & `job_shop_lib-0.5.0/job_shop_lib/dispatching/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/dispatching/dispatcher.py` & `job_shop_lib-0.5.0/job_shop_lib/dispatching/dispatcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,35 +15,67 @@
     ScheduledOperation,
     Operation,
 )
 
 
 # Added here to avoid circular imports
 class DispatcherObserver(abc.ABC):
-    """Interface for classes that observe the dispatcher."""
+    """Interface for classes that observe th"""
+
+    def __init__(
+        self,
+        dispatcher: Dispatcher,
+        is_singleton: bool = True,
+        subscribe: bool = True,
+    ):
+        """Initializes the observer with the `Dispatcher` and subscribes to
+        it.
+
+        Args:
+            subject:
+                The subject to observe.
+            is_singleton:
+                Whether the observer should be a singleton. If True, the
+                observer will be the only instance of its class in the
+                subject's list of subscribers. If False, the observer will
+                be added to the subject's list of subscribers every time
+                it is initialized.
+            subscribe:
+                Whether to subscribe the observer to the subject. If False,
+                the observer will not be subscribed to the subject and will
+                not receive automatic updates.
+        """
+        if is_singleton and any(
+            isinstance(observer, self.__class__)
+            for observer in dispatcher.subscribers
+        ):
+            raise ValueError(
+                f"An observer of type {self.__class__.__name__} already "
+                "exists in the dispatcher's list of subscribers. If you want "
+                "to create multiple instances of this observer, set "
+                "`is_singleton` to False."
+            )
 
-    def __init__(self, dispatcher: Dispatcher):
-        """Initializes the observer with the dispatcher and subscribes to
-        it."""
         self.dispatcher = dispatcher
-        self.dispatcher.subscribe(self)
+        if subscribe:
+            self.dispatcher.subscribe(self)
 
     @abc.abstractmethod
     def update(self, scheduled_operation: ScheduledOperation):
         """Called when an operation is scheduled on a machine."""
 
     @abc.abstractmethod
     def reset(self):
         """Called when the dispatcher is reset."""
 
     def __str__(self) -> str:
         return self.__class__.__name__
 
     def __repr__(self) -> str:
-        return str(self)
+        return self.__class__.__name__
 
 
 def _dispatcher_cache(method):
     """Decorator to cache results of a method based on its name.
 
     This decorator assumes that the class has an attribute called `_cache`
     that is a dictionary. It caches the result of the method based on its
@@ -82,16 +114,14 @@
         instance:
             The instance of the job shop problem to be scheduled.
         schedule:
             The schedule of operations on machines.
         pruning_function:
             A function that filters out operations that are not ready to be
             scheduled.
-        subscribers:
-            A list of observers that are subscribed to the dispatcher.
     """
 
     __slots__ = (
         "instance",
         "schedule",
         "_machine_next_available_time",
         "_job_next_operation_index",
@@ -148,40 +178,14 @@
         return self._job_next_operation_index
 
     @property
     def job_next_available_time(self) -> list[int]:
         """Returns the next available time for each job."""
         return self._job_next_available_time
 
-    @classmethod
-    def create_schedule_from_raw_solution(
-        cls, instance: JobShopInstance, raw_solution: list[list[Operation]]
-    ) -> Schedule:
-        """Deprecated method, use `Schedule.from_job_sequences` instead."""
-        warn(
-            "Dispatcher.create_schedule_from_raw_solution is deprecated. "
-            "Use Schedule.from_job_sequences instead. It will be removed in "
-            "version 1.0.0.",
-            DeprecationWarning,
-        )
-        dispatcher = cls(instance)
-        dispatcher.reset()
-        raw_solution_deques = [
-            deque(operations) for operations in raw_solution
-        ]
-        while not dispatcher.schedule.is_complete():
-            for machine_id, operations in enumerate(raw_solution_deques):
-                if not operations:
-                    continue
-                operation = operations[0]
-                if dispatcher.is_operation_ready(operation):
-                    dispatcher.dispatch(operation, machine_id)
-                    operations.popleft()
-        return dispatcher.schedule
-
     def subscribe(self, observer: DispatcherObserver):
         """Subscribes an observer to the dispatcher."""
         self.subscribers.append(observer)
 
     def unsubscribe(self, observer: DispatcherObserver):
         """Unsubscribes an observer from the dispatcher."""
         self.subscribers.remove(observer)
@@ -301,48 +305,212 @@
         for op in operations:
             for machine_id in op.machines:
                 start_time = self.start_time(op, machine_id)
                 min_start_time = min(min_start_time, start_time)
         return int(min_start_time)
 
     @_dispatcher_cache
-    def uncompleted_operations(self) -> list[Operation]:
-        """Returns the list of operations that have not been scheduled.
-
-        An operation is uncompleted if it has not been scheduled yet.
-
-        It is more efficient than checking all operations in the instance.
-        """
-        uncompleted_operations = []
-        for job_id, next_position in enumerate(self._job_next_operation_index):
-            operations = self.instance.jobs[job_id][next_position:]
-            uncompleted_operations.extend(operations)
-        return uncompleted_operations
-
-    @_dispatcher_cache
     def available_operations(self) -> list[Operation]:
         """Returns a list of available operations for processing, optionally
         filtering out operations using the pruning function.
 
         This method first gathers all possible next operations from the jobs
         being processed. It then optionally filters these operations using the
         pruning function.
 
         Returns:
             A list of Operation objects that are available for scheduling.
         """
-
-        available_operations = self._available_operations()
+        available_operations = self.available_operations_without_pruning()
         if self.pruning_function is not None:
             available_operations = self.pruning_function(
                 self, available_operations
             )
         return available_operations
 
-    def _available_operations(self) -> list[Operation]:
+    @_dispatcher_cache
+    def available_operations_without_pruning(self) -> list[Operation]:
+        """Returns a list of available operations for processing without
+        applying the pruning function.
+
+        Returns:
+            A list of Operation objects that are available for scheduling
+            based on precedence and machine constraints only.
+        """
         available_operations = []
         for job_id, next_position in enumerate(self._job_next_operation_index):
             if next_position == len(self.instance.jobs[job_id]):
                 continue
             operation = self.instance.jobs[job_id][next_position]
             available_operations.append(operation)
         return available_operations
+
+    @_dispatcher_cache
+    def unscheduled_operations(self) -> list[Operation]:
+        """Returns the list of operations that have not been scheduled."""
+        unscheduled_operations = []
+        for job_id, next_position in enumerate(self._job_next_operation_index):
+            operations = self.instance.jobs[job_id][next_position:]
+            unscheduled_operations.extend(operations)
+        return unscheduled_operations
+
+    @_dispatcher_cache
+    def scheduled_operations(self) -> list[Operation]:
+        """Returns the list of operations that have been scheduled."""
+        scheduled_operations = []
+        for job_id, next_position in enumerate(self._job_next_operation_index):
+            operations = self.instance.jobs[job_id][:next_position]
+            scheduled_operations.extend(operations)
+        return scheduled_operations
+
+    @_dispatcher_cache
+    def available_machines(self) -> list[int]:
+        """Returns the list of available machines."""
+        available_operations = self.available_operations()
+        available_machines = set()
+        for operation in available_operations:
+            available_machines.update(operation.machines)
+        return list(available_machines)
+
+    @_dispatcher_cache
+    def available_jobs(self) -> list[int]:
+        """Returns the list of available jobs."""
+        available_operations = self.available_operations()
+        available_jobs = set(
+            operation.job_id for operation in available_operations
+        )
+        return list(available_jobs)
+
+    def earliest_start_time(self, operation: Operation) -> int:
+        """Calculates the earliest start time for a given operation based on
+        machine and job constraints.
+
+        This method is different from the `start_time` method in that it
+        takes into account every machine that can process the operation, not
+        just the one that will process it. However, it also assumes that
+        the operation is ready to be scheduled in the job in favor of
+        performance.
+
+        Args:
+            operation:
+                The operation for which to calculate the earliest start time.
+
+        Returns:
+            The earliest start time for the operation.
+        """
+        machine_earliest_start_time = min(
+            self._machine_next_available_time[machine_id]
+            for machine_id in operation.machines
+        )
+        job_start_time = self._job_next_available_time[operation.job_id]
+        return max(machine_earliest_start_time, job_start_time)
+
+    def remaining_duration(
+        self, scheduled_operation: ScheduledOperation
+    ) -> int:
+        """Calculates the remaining duration of a scheduled operation.
+
+        The method computes the remaining time for an operation to finish,
+        based on the maximum of the operation's start time or the current time.
+        This helps in determining how much time is left from 'now' until the
+        operation is completed.
+
+        Args:
+            scheduled_operation:
+                The operation for which to calculate the remaining time.
+
+        Returns:
+            The remaining duration.
+        """
+        adjusted_start_time = max(
+            scheduled_operation.start_time, self.current_time()
+        )
+        return scheduled_operation.end_time - adjusted_start_time
+
+    @_dispatcher_cache
+    def completed_operations(self) -> set[Operation]:
+        """Returns the set of operations that have been completed.
+
+        This method returns the operations that have been scheduled and the
+        current time is greater than or equal to the end time of the operation.
+        """
+        scheduled_operations = set(self.scheduled_operations())
+        ongoing_operations = set(
+            map(
+                lambda scheduled_op: scheduled_op.operation,
+                self.ongoing_operations(),
+            )
+        )
+        completed_operations = scheduled_operations - ongoing_operations
+        return completed_operations
+
+    @_dispatcher_cache
+    def uncompleted_operations(self) -> list[Operation]:
+        """Returns the list of operations that have not been completed yet.
+
+        This method checks for operations that either haven't been scheduled
+        or have been scheduled but haven't reached their completion time.
+
+        Note:
+        The behavior of this method changed in version 0.5.0. Previously, it
+        only returned unscheduled operations. For the old behavior, use the
+        `unscheduled_operations` method.
+        """
+        uncompleted_operations = self.unscheduled_operations()
+        uncompleted_operations.extend(
+            scheduled_operation.operation
+            for scheduled_operation in self.ongoing_operations()
+        )
+        return uncompleted_operations
+
+    @_dispatcher_cache
+    def ongoing_operations(self) -> list[ScheduledOperation]:
+        """Returns the list of operations that are currently being processed.
+
+        This method returns the operations that have been scheduled and are
+        currently being processed by the machines.
+        """
+        current_time = self.current_time()
+        ongoing_operations = []
+        for machine_schedule in self.schedule.schedule:
+            for scheduled_operation in reversed(machine_schedule):
+                is_completed = scheduled_operation.end_time <= current_time
+                if is_completed:
+                    break
+                ongoing_operations.append(scheduled_operation)
+        return ongoing_operations
+
+    def is_scheduled(self, operation: Operation) -> bool:
+        """Checks if the given operation has been scheduled."""
+        job_next_op_idx = self._job_next_operation_index[operation.job_id]
+        return operation.position_in_job < job_next_op_idx
+
+    def is_ongoing(self, scheduled_operation: ScheduledOperation) -> bool:
+        """Checks if the given operation is currently being processed."""
+        current_time = self.current_time()
+        return scheduled_operation.start_time <= current_time
+
+    @classmethod
+    def create_schedule_from_raw_solution(
+        cls, instance: JobShopInstance, raw_solution: list[list[Operation]]
+    ) -> Schedule:
+        """Deprecated method, use `Schedule.from_job_sequences` instead."""
+        warn(
+            "Dispatcher.create_schedule_from_raw_solution is deprecated. "
+            "Use Schedule.from_job_sequences instead. It will be removed in "
+            "version 1.0.0.",
+            DeprecationWarning,
+        )
+        dispatcher = cls(instance)
+        dispatcher.reset()
+        raw_solution_deques = [
+            deque(operations) for operations in raw_solution
+        ]
+        while not dispatcher.schedule.is_complete():
+            for machine_id, operations in enumerate(raw_solution_deques):
+                if not operations:
+                    continue
+                operation = operations[0]
+                if dispatcher.is_operation_ready(operation):
+                    dispatcher.dispatch(operation, machine_id)
+                    operations.popleft()
+        return dispatcher.schedule
```

### Comparing `job_shop_lib-0.4.0/job_shop_lib/dispatching/dispatching_rule_solver.py` & `job_shop_lib-0.5.0/job_shop_lib/dispatching/dispatching_rule_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/dispatching/dispatching_rules.py` & `job_shop_lib-0.5.0/job_shop_lib/dispatching/dispatching_rules.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/dispatching/factories.py` & `job_shop_lib-0.5.0/job_shop_lib/dispatching/factories.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/dispatching/history_tracker.py` & `job_shop_lib-0.5.0/job_shop_lib/dispatching/history_tracker.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/dispatching/pruning_functions.py` & `job_shop_lib-0.5.0/job_shop_lib/dispatching/pruning_functions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/exceptions.py` & `job_shop_lib-0.5.0/job_shop_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/generators/basic_generator.py` & `job_shop_lib-0.5.0/job_shop_lib/generators/basic_generator.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/generators/transformations.py` & `job_shop_lib-0.5.0/job_shop_lib/generators/transformations.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/graphs/__init__.py` & `job_shop_lib-0.5.0/job_shop_lib/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/graphs/build_agent_task_graph.py` & `job_shop_lib-0.5.0/job_shop_lib/graphs/build_agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/graphs/build_disjunctive_graph.py` & `job_shop_lib-0.5.0/job_shop_lib/graphs/build_disjunctive_graph.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,14 +19,34 @@
 import itertools
 
 from job_shop_lib import JobShopInstance
 from job_shop_lib.graphs import JobShopGraph, EdgeType, NodeType, Node
 
 
 def build_disjunctive_graph(instance: JobShopInstance) -> JobShopGraph:
+    """Builds and returns a disjunctive graph for the given job shop instance.
+
+    This function creates a complete disjunctive graph from a JobShopInstance.
+    It starts by initializing a JobShopGraph object and proceeds by adding
+    disjunctive edges between operations using the same machine, conjunctive
+    edges between successive operations in the same job, and finally, special
+    source and sink nodes with their respective edges to and from all other
+    operations.
+
+    Edges have a "type" attribute indicating whether they are disjunctive or
+    conjunctive.
+
+    Args:
+        instance (JobShopInstance): The job shop instance for which to build
+        the graph.
+
+    Returns:
+        JobShopGraph: A JobShopGraph object representing the disjunctive graph
+        of the job shop scheduling problem.
+    """
     graph = JobShopGraph(instance)
     add_disjunctive_edges(graph)
     add_conjunctive_edges(graph)
     add_source_sink_nodes(graph)
     add_source_sink_edges(graph)
     return graph
```

### Comparing `job_shop_lib-0.4.0/job_shop_lib/graphs/job_shop_graph.py` & `job_shop_lib-0.5.0/job_shop_lib/graphs/job_shop_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/graphs/node.py` & `job_shop_lib-0.5.0/job_shop_lib/graphs/node.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/job_shop_instance.py` & `job_shop_lib-0.5.0/job_shop_lib/job_shop_instance.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 import os
 import functools
 from typing import Any
 
+import numpy as np
+
 from job_shop_lib import Operation
 
 
 class JobShopInstance:
     """Data structure to store a Job Shop Scheduling Problem instance.
 
     Additional attributes such as `num_jobs` or `num_machines` can be computed
@@ -261,14 +263,66 @@
                 [operation.machines for operation in job] for job in self.jobs
             ]
         return [
             [operation.machine_id for operation in job] for job in self.jobs
         ]
 
     @functools.cached_property
+    def durations_matrix_array(self) -> np.ndarray:
+        """Returns the duration matrix of the instance as a numpy array.
+
+        The returned array has shape (num_jobs, max_num_operations_per_job).
+        Non-existing operations are filled with np.nan.
+
+        Example:
+            >>> jobs = [[Operation(0, 2), Operation(1, 3)], [Operation(0, 4)]]
+            >>> instance = JobShopInstance(jobs)
+            >>> instance.durations_matrix_array
+            array([[ 2.,  2.],
+                   [ 4., nan]], dtype=float32)
+        """
+        duration_matrix = self.durations_matrix
+        return self._fill_matrix_with_nans_2d(duration_matrix)
+
+    @functools.cached_property
+    def machines_matrix_array(self) -> np.ndarray:
+        """Returns the machines matrix of the instance as a numpy array.
+
+        The returned array has shape (num_jobs, max_num_operations_per_job,
+        max_num_machines_per_operation). Non-existing machines are filled with
+        np.nan.
+
+        Example:
+            >>> jobs = [
+            ...     [Operation(machines=[0, 1], 2), Operation(machines=1, 3)],
+            ...     [Operation(machines=0, 6)],
+            ... ]
+            >>> instance = JobShopInstance(jobs)
+            >>> instance.machines_matrix_array
+            array([[[ 0.,  1.],
+                    [ 1., nan]],
+                   [[ 0., nan],
+                    [nan, nan]]], dtype=float32)
+        """
+
+        machines_matrix = self.machines_matrix
+        if self.is_flexible:
+            # False positive from mypy, the type of machines_matrix is
+            # list[list[list[int]]] here
+            return self._fill_matrix_with_nans_3d(
+                machines_matrix  # type: ignore[arg-type]
+            )
+
+        # False positive from mypy, the type of machines_matrix is
+        # list[list[int]] here
+        return self._fill_matrix_with_nans_2d(
+            machines_matrix  # type: ignore[arg-type]
+        )
+
+    @functools.cached_property
     def operations_by_machine(self) -> list[list[Operation]]:
         """Returns a list of lists of operations.
 
         The i-th list contains the operations that can be processed in the
         machine with id i.
         """
         operations_by_machine: list[list[Operation]] = [
@@ -349,7 +403,54 @@
 
         return machine_times
 
     @functools.cached_property
     def total_duration(self) -> int:
         """Returns the sum of the durations of all operations in all jobs."""
         return sum(self.job_durations)
+
+    @staticmethod
+    def _fill_matrix_with_nans_2d(matrix: list[list[int]]) -> np.ndarray:
+        """Fills a matrix with np.nan values.
+
+        Args:
+            matrix:
+                A list of lists of integers.
+
+        Returns:
+            A numpy array with the same shape as the input matrix, filled with
+            np.nan values.
+        """
+        max_length = max(len(row) for row in matrix)
+        squared_matrix = np.full(
+            (len(matrix), max_length), np.nan, dtype=np.float32
+        )
+        for i, row in enumerate(matrix):
+            squared_matrix[i, : len(row)] = row
+        return squared_matrix
+
+    @staticmethod
+    def _fill_matrix_with_nans_3d(matrix: list[list[list[int]]]) -> np.ndarray:
+        """Fills a 3D matrix with np.nan values.
+
+        Args:
+            matrix:
+                A list of lists of lists of integers.
+
+        Returns:
+            A numpy array with the same shape as the input matrix, filled with
+            np.nan values.
+        """
+        max_length = max(len(row) for row in matrix)
+        max_inner_length = len(matrix[0][0])
+        for row in matrix:
+            for inner_row in row:
+                max_inner_length = max(max_inner_length, len(inner_row))
+        squared_matrix = np.full(
+            (len(matrix), max_length, max_inner_length),
+            np.nan,
+            dtype=np.float32,
+        )
+        for i, row in enumerate(matrix):
+            for j, inner_row in enumerate(row):
+                squared_matrix[i, j, : len(inner_row)] = inner_row
+        return squared_matrix
```

### Comparing `job_shop_lib-0.4.0/job_shop_lib/operation.py` & `job_shop_lib-0.5.0/job_shop_lib/operation.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/schedule.py` & `job_shop_lib-0.5.0/job_shop_lib/schedule.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/scheduled_operation.py` & `job_shop_lib-0.5.0/job_shop_lib/scheduled_operation.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/visualization/__init__.py` & `job_shop_lib-0.5.0/job_shop_lib/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/visualization/agent_task_graph.py` & `job_shop_lib-0.5.0/job_shop_lib/visualization/agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/visualization/create_gif.py` & `job_shop_lib-0.5.0/job_shop_lib/visualization/create_gif.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 # reduce the number of arguments without losing functionality.
 # pylint: disable=too-many-arguments
 def create_gif(
     gif_path: str,
     instance: JobShopInstance,
     solver: DispatchingRuleSolver,
     plot_function: (
-        Callable[[Schedule, int, list[Operation] | None], Figure] | None
+        Callable[[Schedule, int, list[Operation] | None, int | None], Figure]
+        | None
     ) = None,
     fps: int = 1,
     remove_frames: bool = True,
     frames_dir: str | None = None,
     plot_current_time: bool = True,
 ) -> None:
     """Creates a GIF of the schedule being built by the given solver.
@@ -76,68 +77,79 @@
         shutil.rmtree(frames_dir)
 
 
 def plot_gantt_chart_wrapper(
     title: str | None = None,
     cmap: str = "viridis",
     show_available_operations: bool = False,
-) -> Callable[[Schedule, int, list[Operation] | None], Figure]:
+) -> Callable[[Schedule, int, list[Operation] | None, int | None], Figure]:
     """Returns a function that plots a Gantt chart for an unfinished schedule.
 
     Args:
         title: The title of the Gantt chart.
         cmap: The name of the colormap to use.
+        show_available_operations:
+            Whether to show the available operations in the Gantt chart.
 
     Returns:
         A function that plots a Gantt chart for a schedule. The function takes
-        a `Schedule` object and the makespan of the schedule as input and
-        returns a `Figure` object.
+        the following arguments:
+        - schedule: The schedule to plot.
+        - makespan: The makespan of the schedule.
+        - available_operations: A list of available operations. If None,
+            the available operations are not shown.
+        - current_time: The current time in the schedule. If provided, a
+            red vertical line is plotted at this time.
     """
 
     def plot_function(
         schedule: Schedule,
         makespan: int,
         available_operations: list | None = None,
+        current_time: int | None = None,
     ) -> Figure:
         fig, ax = plot_gantt_chart(
             schedule, title=title, cmap_name=cmap, xlim=makespan
         )
 
-        if not show_available_operations or available_operations is None:
-            return fig
+        if show_available_operations and available_operations is not None:
 
-        operations_text = "\n".join(
-            str(operation) for operation in available_operations
-        )
-        text = f"Available operations:\n{operations_text}"
-        # Print the available operations at the bottom right corner
-        # of the Gantt chart
-        fig.text(
-            1.25,
-            0.05,
-            text,
-            ha="right",
-            va="bottom",
-            transform=ax.transAxes,
-            bbox={
-                "facecolor": "white",
-                "alpha": 0.5,
-                "boxstyle": "round,pad=0.5",
-            },
-        )
+            operations_text = "\n".join(
+                str(operation) for operation in available_operations
+            )
+            text = f"Available operations:\n{operations_text}"
+            # Print the available operations at the bottom right corner
+            # of the Gantt chart
+            fig.text(
+                1.25,
+                0.05,
+                text,
+                ha="right",
+                va="bottom",
+                transform=ax.transAxes,
+                bbox={
+                    "facecolor": "white",
+                    "alpha": 0.5,
+                    "boxstyle": "round,pad=0.5",
+                },
+            )
+        if current_time is not None:
+            ax.axvline(current_time, color="red", linestyle="--")
         return fig
 
     return plot_function
 
 
 def create_gantt_chart_frames(
     frames_dir: str,
     instance: JobShopInstance,
     solver: DispatchingRuleSolver,
-    plot_function: Callable[[Schedule, int, list[Operation] | None], Figure],
+    plot_function: Callable[
+        [Schedule, int, list[Operation] | None, int | None], Figure
+    ],
     plot_current_time: bool = True,
 ) -> None:
     """Creates frames of the Gantt chart for the schedule being built.
 
     Args:
         frames_dir:
             The directory to save the frames in.
@@ -146,41 +158,38 @@
         solver:
             The dispatching rule solver to use.
         plot_function:
             A function that plots a Gantt chart for a schedule. It
             should take a `Schedule` object and the makespan of the schedule as
             input and return a `Figure` object.
         plot_current_time:
-            Whether to plot a vertical line at the current time."""
+            Whether to plot a vertical line at the current time.
+    """
     dispatcher = Dispatcher(instance, pruning_function=solver.pruning_function)
     history_tracker = HistoryTracker(dispatcher)
     makespan = solver.solve(instance, dispatcher).makespan()
     dispatcher.unsubscribe(history_tracker)
     dispatcher.reset()
     for i, scheduled_operation in enumerate(history_tracker.history, start=1):
         dispatcher.dispatch(
             scheduled_operation.operation, scheduled_operation.machine_id
         )
+        current_time = (
+            None if not plot_current_time else dispatcher.current_time()
+        )
         fig = plot_function(
             dispatcher.schedule,
             makespan,
             dispatcher.available_operations(),
+            current_time,
         )
-        current_time = (
-            None if not plot_current_time else dispatcher.current_time()
-        )
-        _save_frame(fig, frames_dir, i, current_time)
-
+        _save_frame(fig, frames_dir, i)
 
-def _save_frame(
-    figure: Figure, frames_dir: str, number: int, current_time: int | None
-) -> None:
-    if current_time is not None:
-        figure.gca().axvline(current_time, color="red", linestyle="--")
 
+def _save_frame(figure: Figure, frames_dir: str, number: int) -> None:
     figure.savefig(f"{frames_dir}/frame_{number:02d}.png", bbox_inches="tight")
     plt.close(figure)
 
 
 def create_gif_from_frames(frames_dir: str, gif_path: str, fps: int) -> None:
     """Creates a GIF from the frames in the given directory.
```

### Comparing `job_shop_lib-0.4.0/job_shop_lib/visualization/disjunctive_graph.py` & `job_shop_lib-0.5.0/job_shop_lib/visualization/disjunctive_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.4.0/job_shop_lib/visualization/gantt_chart.py` & `job_shop_lib-0.5.0/job_shop_lib/visualization/gantt_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 
 def _plot_machine_schedules(
     schedule: Schedule, ax: plt.Axes, cmap_name: str
 ) -> dict[int, Patch]:
     """Plots the schedules for each machine."""
     max_job_id = schedule.instance.num_jobs - 1
-    cmap = plt.cm.get_cmap(cmap_name, max_job_id + 1)
+    cmap = plt.get_cmap(cmap_name, max_job_id + 1)
     norm = Normalize(vmin=0, vmax=max_job_id)
     legend_handles = {}
 
     for machine_index, machine_schedule in enumerate(schedule.schedule):
         y_position_for_machines = (
             _BASE_Y_POSITION + _Y_POSITION_INCREMENT * machine_index
         )
```

### Comparing `job_shop_lib-0.4.0/pyproject.toml` & `job_shop_lib-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "job-shop-lib"
-version = "0.4.0"
+version = "0.5.0"
 description = "An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)"
 authors = ["Pabloo22 <pablete.arino@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "job_shop_lib"}]
 include = ["benchmarks/benchmark_instances.json"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-ortools = "^9"
+ortools = ">=9.9,<9.10"
 matplotlib = "^3"
 pyarrow = "^15.0.0"  # An optional pandas' dependency that will be required in the future
 networkx = "^3"
 imageio = "^2"
 pygraphviz = {version = "^1.12", optional = true}
+numpy = "^1.26.4"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
@@ -34,15 +35,14 @@
 
 [tool.poetry.group.notebooks]
 optional = true
 
 [tool.poetry.group.notebooks.dependencies]
 ipykernel = "^6.29.2"
 nbconvert = "^7.16.0"
-numpy = "^1.26.4"
 pandas = "^2.2.1"
 
 [tool.poetry.extras]
 pygraphviz = ["pygraphviz"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `job_shop_lib-0.4.0/PKG-INFO` & `job_shop_lib-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: job-shop-lib
-Version: 0.4.0
+Version: 0.5.0
 Summary: An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)
 License: MIT
 Author: Pabloo22
 Author-email: pablete.arino@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pygraphviz
 Requires-Dist: imageio (>=2,<3)
 Requires-Dist: matplotlib (>=3,<4)
 Requires-Dist: networkx (>=3,<4)
-Requires-Dist: ortools (>=9,<10)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: ortools (>=9.9,<9.10)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pygraphviz (>=1.12,<2.0) ; extra == "pygraphviz"
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="images/logo_with_transparent_background.png" height="150px">
@@ -79,15 +80,15 @@
 ```python
 from job_shop_lib.benchmarking import load_benchmark_instance
 
 ft06 = load_benchmark_instance("ft06")
 ```
 
 The module `benchmarks` contains functions to load the instances from the file and return them as `JobShopInstance` objects without having to download them
-manually. The instances are stored in [benchmark_instances.json](job_shop_lib/benchmarks/benchmark_instances.json).
+manually.
 
 The contributions to this benchmark dataset are as follows:
 
 - `abz5-9`: by Adams et al. (1988).
 
 - `ft06`, `ft10`, `ft20`: by Fisher and Thompson (1963).
 
@@ -167,21 +168,23 @@
     MOST_OPERATION_REMAINING = "most_operation_remaining"
     RANDOM = "random"
 ```
 
 We can visualize the solution with a `DispatchingRuleSolver` as a gif:
 
 ```python
-from job_shop_lib.visualization import create_gif, get_plot_function
+from job_shop_lib.visualization import create_gif, plot_gantt_chart_wrapper
 from job_shop_lib.dispatching import DispatchingRuleSolver, DispatchingRule
 
 plt.style.use("ggplot")
 
 mwkr_solver = DispatchingRuleSolver("most_work_remaining")
-plot_function = get_plot_function(title="Solution with Most Work Remaining Rule")
+plot_function = plot_gantt_chart_wrapper(
+    title="Solution with Most Work Remaining Rule"
+)
 create_gif(
     gif_path="ft06_optimized.gif",
     instance=ft06,
     solver=mwkr_solver,
     plot_function=plot_function,
     fps=4,
 )
@@ -346,7 +349,8 @@
      International Workshop on Parallel Problem Solving from Nature
      (PPSN'2), Brussels, Belgium, pp. 281–290, 1992.
 
  - E. Taillard, "Benchmarks for basic scheduling problems," European
      Journal of Operational Research, vol. 64, no. 2, pp. 278–285, 1993.
 
 - Park, Junyoung, Sanjar Bakhtiyar, and Jinkyoo Park. "ScheduleNet: Learn to solve multi-agent scheduling problems with reinforcement learning." arXiv preprint arXiv:2106.03051, 2021. 
+
```

