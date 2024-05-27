# Comparing `tmp/worker_dispatcher-1.0.2.tar.gz` & `tmp/worker_dispatcher-1.0.3.tar.gz`

## Comparing `worker_dispatcher-1.0.2.tar` & `worker_dispatcher-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/img/introduction.planuml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/src/worker_dispatcher/__init__.py
--rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/src/worker_dispatcher/worker_dispatcher.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/LICENSE
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/img/introduction.planuml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/src/worker_dispatcher/__init__.py
+-rw-r--r--   0        0        0    15011 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/src/worker_dispatcher/worker_dispatcher.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/LICENSE
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8698 2020-02-02 00:00:00.000000 worker_dispatcher-1.0.3/PKG-INFO
```

### Comparing `worker_dispatcher-1.0.2/.github/workflows/python-publish.yml` & `worker_dispatcher-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-1.0.2/src/worker_dispatcher/worker_dispatcher.py` & `worker_dispatcher-1.0.3/src/worker_dispatcher/worker_dispatcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import multiprocessing, concurrent.futures
-import time, copy, requests
+import time, datetime, copy, requests
 
 # Sample callback function
 def callback_sample(id: int, config=None, task=None):
     if id == 1:
         print("Runing sample task function, please customize yours according to the actual usage.")
     result = {
         'taskId': id
@@ -27,14 +27,15 @@
     },
     'worker': {
         'number': multiprocessing.cpu_count(),
         'per_second': 0,                # If greater than 0, the specified number of workers run at set intervals.
         'cumulative': False,            # Cumulative mode for per_second method.
         'multiprocessing': False
     },
+    'runtime': None,                    # Dispatcher max runtime in seconds
     'verbose': True
 }
 
 # Global variable
 results = []
 logs = []
 result_info = {}
@@ -94,58 +95,81 @@
             }
             task_list.append(data)
 
     # Worker dispatch
     worker_num = config['worker']['number']
     worker_num = worker_num if isinstance(worker_num, int) else 1
     worker_per_second = config['worker']['per_second'] if config['worker']['per_second'] else 0
-    max_workers = len(task_list) if worker_per_second else worker_num
+    max_workers = min(len(task_list) if worker_per_second else worker_num, 32766)
+    runtime = float(config['runtime']) if config['runtime'] else None
     if config['verbose']:
         print("Worker Dispatcher Configutation:")
-        print("- Task Number: {}".format(len(task_list)))
+        print("- Tasks Count: {}".format(len(task_list)))
+        print("- Runtime: {}".format("{} sec".format(runtime) if runtime else "Unlimited"))
         print("- Worker Type:", "Processing" if use_multiprocessing else "Threading")
         print("- Worker Number: {}".format(worker_num))
         print("- Worker Per Second: {}".format(worker_per_second))
         print("- Max Worker: {}".format(max_workers))
     pool_executor_class = concurrent.futures.ProcessPoolExecutor if use_multiprocessing else concurrent.futures.ThreadPoolExecutor
     result_info['started_at'] = time.time()
-    if config['verbose']:
-        print("\n--- Start to dispatch workers ---\n")
+    datetime_timezone_obj = datetime.timezone(datetime.timedelta(hours=time.localtime().tm_gmtoff / 3600))
+    if config['verbose']: print("\n--- Start to dispatch workers at {} ---\n".format(datetime.datetime.fromtimestamp(result_info['started_at'], datetime_timezone_obj).isoformat()))
 
     # Pool Executor
     with pool_executor_class(max_workers=max_workers) as executor:
+        undispatched_tasks_count = 0
         pool_results = []
-        per_second_count = worker_num
+        per_second_remaining_quota = worker_num
+        per_second_remaining_runtime = runtime
         # Task dispatch
-        for task in task_list:
+        for i, task in enumerate(task_list):
             pool_result = executor.submit(consume_task, task, config)
             pool_results.append(pool_result)
             # Worker per_second setting
-            per_second_count -= 1
-            if worker_per_second and per_second_count <= 0:
+            if worker_per_second and (per_second_remaining_quota := per_second_remaining_quota - 1) <= 0:
                 if config['worker']['cumulative']:
                     worker_num += worker_per_second
-                per_second_count = worker_num
+                per_second_remaining_quota = worker_num
                 time.sleep(float(worker_per_second))
-        timestamp_end_dispatch = time.time()
+                # Max Runtime setting
+                if runtime and (per_second_remaining_runtime := per_second_remaining_runtime - worker_per_second) <= 0:
+                    undispatched_tasks_count = len(task_list) - (i + 1)
+                    if config['verbose']: print(f'Dispathcer timeout reached, {undispatched_tasks_count} remaining tasks were abandoned')
+                    break
+
+        # Wait for the pool to complete or timeout
+        done, not_done = concurrent.futures.wait(
+            pool_results,
+            timeout=runtime,
+            return_when=concurrent.futures.ALL_COMPLETED
+        )
+        # Cancel remaining tasks if the timeout was reached
+        if not_done:
+            if config['verbose']: print(f'Dispathcer timeout reached, cancelling {len(not_done)} remaining tasks...')
+            for future in not_done:
+                future.cancel()
+
         # Get results from the async results
-        for pool_result in concurrent.futures.as_completed(pool_results):
+        for pool_result in concurrent.futures.as_completed(done):
             log = pool_result.result()
             result = log['result']
             if callable(config['task']['result_callback']):
                 result = config['task']['result_callback'](config=config['task']['config'], id=log['task_id'], result=log['result'], log=log)
             logs.append(log)
             results.append(result)
         # results = [result.result() for result in concurrent.futures.as_completed(pool_results)]
 
     result_info['ended_at'] = time.time()
     result_info['duration'] = result_info['ended_at'] - result_info['started_at']
     if config['verbose']:
-        print("\n--- End of worker dispatch ---\n")
+        print("\n--- End of worker dispatch at {}---\n".format(datetime.datetime.fromtimestamp(result_info['started_at'], datetime_timezone_obj).isoformat()))
         print("Spend Time: {:.6f} sec".format(result_info['duration']))
+        print("Completed Tasks Count: {}".format(len(done)))
+        print("Uncompleted Tasks Count: {}".format(len(not_done)))
+        print("Undispatched Tasks Count: {}".format(undispatched_tasks_count))
     return results
 
 # Worker function
 def consume_task(data, config) -> dict:
     started_at = time.time()
     return_value = config['task']['callback'](config=config['task']['config'], id=data['id'], task=data['task'])
     ended_at = time.time()
@@ -199,94 +223,94 @@
     valid_count = total_count - invalid_count
     duration = ended_at - started_at
     exec_time_avg = exec_time_sum / valid_count if exec_time_sum else 0
     exec_time_success_avg = exec_time_success_sum / success_count if exec_time_success_sum else 0
     tps = success_count / duration if success_count else 0
 
     # Peak TPS
-    peak_duration = peak_duration if peak_duration else exec_time_avg * 3
-    # peak_duration = exec_time_max
     peak_tps_data = {}
-    peak_success_count = 0
-    peak_ended_at = ended_at
-    peak_started_at = peak_ended_at
     peak_log_list = []
-    if debug:
-        print("Peak - vaild count:{}, duration/interval:{}".format(valid_count, peak_duration));
-    while peak_started_at > started_at:
-        current_count = 0
-        current_success_count = 0
-        current_invalid_count = 0
-        peak_ended_at = peak_started_at
-        peak_started_at -= peak_duration
-        peak_exec_time_sum = 0
-        peak_exec_time_max = 0
-        peak_exec_time_min = 0
-        peak_exec_time_success_sum = 0
-        peak_exec_time_success_max = 0
-        peak_exec_time_success_min = 0
-        if peak_started_at <= started_at:
-            peak_started_at = started_at
-            peak_duration = peak_ended_at - peak_started_at
-        for log in logs:
-            if not _validate_log_format(log):
-                current_invalid_count += 1
-                continue
-            if log['started_at'] < peak_started_at or log['ended_at'] > peak_ended_at:
-                continue
-            current_count += 1
-            exec_time = log['duration'] if 'duration' in log else log['ended_at'] - log['started_at']
-            peak_exec_time_sum += exec_time
-            peak_exec_time_max = exec_time if not peak_exec_time_max or exec_time > peak_exec_time_max else peak_exec_time_max
-            peak_exec_time_min = exec_time if not peak_exec_time_min or exec_time < peak_exec_time_min else peak_exec_time_min
-            # Success case
-            if log['task_id'] in success_id_set:
-                current_success_count += 1           
-                peak_exec_time_success_sum += exec_time
-                peak_exec_time_success_max = exec_time if not peak_exec_time_success_max or exec_time > peak_exec_time_success_max else peak_exec_time_success_max
-                peak_exec_time_success_min = exec_time if not peak_exec_time_success_min or exec_time < peak_exec_time_success_min else peak_exec_time_success_min
+    if success_count > 0:
+        peak_duration = peak_duration if peak_duration else round(exec_time_avg * 3, 2) if (exec_time_avg * 3) >= 1 else 5
+        peak_success_count = 0
+        peak_ended_at = ended_at
+        peak_started_at = peak_ended_at
         if debug:
-            print("Each Peak - count:{}, start:{}, end:{}".format(current_success_count, peak_started_at, peak_ended_at))
+            print("Peak - vaild count:{}, duration/interval:{}".format(valid_count, peak_duration));
+        while peak_started_at > started_at:
+            current_count = 0
+            current_success_count = 0
+            current_invalid_count = 0
+            peak_ended_at = peak_started_at
+            peak_started_at -= peak_duration
+            peak_exec_time_sum = 0
+            peak_exec_time_max = 0
+            peak_exec_time_min = 0
+            peak_exec_time_success_sum = 0
+            peak_exec_time_success_max = 0
+            peak_exec_time_success_min = 0
+            if peak_started_at <= started_at:
+                peak_started_at = started_at
+                peak_duration = peak_ended_at - peak_started_at
+            for log in logs:
+                if not _validate_log_format(log):
+                    current_invalid_count += 1
+                    continue
+                if log['started_at'] < peak_started_at or log['ended_at'] > peak_ended_at:
+                    continue
+                current_count += 1
+                exec_time = log['duration'] if 'duration' in log else log['ended_at'] - log['started_at']
+                peak_exec_time_sum += exec_time
+                peak_exec_time_max = exec_time if not peak_exec_time_max or exec_time > peak_exec_time_max else peak_exec_time_max
+                peak_exec_time_min = exec_time if not peak_exec_time_min or exec_time < peak_exec_time_min else peak_exec_time_min
+                # Success case
+                if log['task_id'] in success_id_set:
+                    current_success_count += 1           
+                    peak_exec_time_success_sum += exec_time
+                    peak_exec_time_success_max = exec_time if not peak_exec_time_success_max or exec_time > peak_exec_time_success_max else peak_exec_time_success_max
+                    peak_exec_time_success_min = exec_time if not peak_exec_time_success_min or exec_time < peak_exec_time_success_min else peak_exec_time_success_min
+            if debug:
+                print("Each Peak - count:{}, start:{}, end:{}".format(current_success_count, peak_started_at, peak_ended_at))
 
-        current_valid_count = current_count - current_invalid_count
-        peak_exec_time_avg = peak_exec_time_sum / current_valid_count if peak_exec_time_sum else 0
-        peak_exec_time_success_avg = peak_exec_time_success_sum / current_success_count if peak_exec_time_success_sum else 0
-        current_tps = current_success_count / peak_duration
-        tps_data = {
-            'tps': "{:.2f}".format(current_tps, 2),
-            'started_at': peak_started_at,
-            'ended_at': peak_ended_at,
-            'duration': peak_duration,
-            'metrics': {
-                'execution_time': {
-                    'avg': peak_exec_time_avg,
-                    'max': peak_exec_time_max,
-                    'min': peak_exec_time_min
+            current_valid_count = current_count - current_invalid_count
+            peak_exec_time_avg = peak_exec_time_sum / current_valid_count if peak_exec_time_sum else 0
+            peak_exec_time_success_avg = peak_exec_time_success_sum / current_success_count if peak_exec_time_success_sum else 0
+            current_tps = current_success_count / peak_duration
+            tps_data = {
+                'tps': "{:.2f}".format(current_tps, 2),
+                'started_at': peak_started_at,
+                'ended_at': peak_ended_at,
+                'duration': peak_duration,
+                'metrics': {
+                    'execution_time': {
+                        'avg': peak_exec_time_avg,
+                        'max': peak_exec_time_max,
+                        'min': peak_exec_time_min
+                    },
+                    'success_execution_time': {
+                        'avg': peak_exec_time_success_avg,
+                        'max': peak_exec_time_success_max,
+                        'min': peak_exec_time_success_min
+                    },
                 },
-                'success_execution_time': {
-                    'avg': peak_exec_time_success_avg,
-                    'max': peak_exec_time_success_max,
-                    'min': peak_exec_time_success_min
+                'count': {
+                    'success': current_success_count,
+                    'total': current_count,
+                    'invalidity': current_invalid_count
                 },
-            },
-            'count': {
-                'success': current_success_count,
-                'total': current_count,
-                'invalidity': current_invalid_count
-            },
-        }
-        peak_log_list.append(tps_data)
-        # Find the peak
-        if current_success_count and current_success_count > peak_success_count:
-            peak_success_count = current_success_count
-            if debug:
-                print(" - peak_tps:{}, tps:{}".format(current_tps, tps))
-            # Comparing with avg TPS
-            if current_tps > tps:
-                peak_tps_data = tps_data
+            }
+            peak_log_list.append(tps_data)
+            # Find the peak
+            if current_success_count and current_success_count > peak_success_count:
+                peak_success_count = current_success_count
+                if debug:
+                    print(" - peak_tps:{}, tps:{}".format(current_tps, tps))
+                # Comparing with avg TPS
+                if current_tps > tps:
+                    peak_tps_data = tps_data
 
     result = {
         'tps': "{:.2f}".format(tps, 2),
         'started_at': started_at,
         'ended_at': ended_at,
         'duration': duration,
         'metrics': {
```

### Comparing `worker_dispatcher-1.0.2/.gitignore` & `worker_dispatcher-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-1.0.2/LICENSE` & `worker_dispatcher-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `worker_dispatcher-1.0.2/README.md` & `worker_dispatcher-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,17 @@
         'result_callback': your_function_name_for_each_result,
     },
     'worker': {
         'number': 8,
         'per_second': 0,                # If greater than 0, the specified number of workers run forcefully at set intervals.
         'cumulative': False,            # Cumulative mode for per_second method.
         'multiprocessing': False
-    }
+    },
+    'runtime': None,                    # Dispatcher max runtime in seconds
+    'verbose': True
 })
 ```
 
 ### Options
 
 |Option            |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
@@ -147,15 +149,16 @@
 |[task.callback](#taskcallback)             |callable |(sample)          |The callback function called by each worker runs|
 |task.config       |multitype|list         |The custom variable to be passed to the callback function|
 |[task.result_callback](#taskresultcallback) |callable |Null          |The callback function called when each task processes the result|
 |worker.number     |int      |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
 |worker.per_second |float    |0            |If greater than 0, the specified number of workers run forcefully at set intervals.|
 |worker.cumulative |bool     |False        |Cumulative mode for per_second method.|
 |worker.multiprocessing                     |boolean  |False        |Use multi-processing instead of the default multi-threading |
-|verbose|bool      |bool     |True         |Enables or disables verbose mode for detailed output.|
+|runtime           |float    |None         |Dispatcher max runtime in seconds|
+|verbose           |bool     |True         |Enables or disables verbose mode for detailed output.|
 
 
 #### task.callback
 
 The callback function called by each worker runs
 
 ```python
```

### Comparing `worker_dispatcher-1.0.2/pyproject.toml` & `worker_dispatcher-1.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "worker_dispatcher"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Nick Tsai", email="myintaer@gmail.com" },
 ]
 description = "A flexible task dispatcher for Python with multiple threading or processing control"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `worker_dispatcher-1.0.2/PKG-INFO` & `worker_dispatcher-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: worker_dispatcher
-Version: 1.0.2
+Version: 1.0.3
 Summary: A flexible task dispatcher for Python with multiple threading or processing control
 Project-URL: Homepage, https://github.com/yidas/python-worker-dispatcher
 Project-URL: Issues, https://github.com/yidas/python-worker-dispatcher/issues
 Author-email: Nick Tsai <myintaer@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -144,15 +144,17 @@
         'result_callback': your_function_name_for_each_result,
     },
     'worker': {
         'number': 8,
         'per_second': 0,                # If greater than 0, the specified number of workers run forcefully at set intervals.
         'cumulative': False,            # Cumulative mode for per_second method.
         'multiprocessing': False
-    }
+    },
+    'runtime': None,                    # Dispatcher max runtime in seconds
+    'verbose': True
 })
 ```
 
 ### Options
 
 |Option            |Type     |Deafult      |Description|
 |:--               |:--      |:--          |:--        |
@@ -161,15 +163,16 @@
 |[task.callback](#taskcallback)             |callable |(sample)          |The callback function called by each worker runs|
 |task.config       |multitype|list         |The custom variable to be passed to the callback function|
 |[task.result_callback](#taskresultcallback) |callable |Null          |The callback function called when each task processes the result|
 |worker.number     |int      |(auto)       |The number of workers to fork. <br>(The default value is the number of local CPU cores)|
 |worker.per_second |float    |0            |If greater than 0, the specified number of workers run forcefully at set intervals.|
 |worker.cumulative |bool     |False        |Cumulative mode for per_second method.|
 |worker.multiprocessing                     |boolean  |False        |Use multi-processing instead of the default multi-threading |
-|verbose|bool      |bool     |True         |Enables or disables verbose mode for detailed output.|
+|runtime           |float    |None         |Dispatcher max runtime in seconds|
+|verbose           |bool     |True         |Enables or disables verbose mode for detailed output.|
 
 
 #### task.callback
 
 The callback function called by each worker runs
 
 ```python
```

