# Comparing `tmp/FlowVisor-0.2.4.tar.gz` & `tmp/FlowVisor-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.2.4.tar", last modified: Sat May 25 13:40:10 2024, max compression
+gzip compressed data, was "FlowVisor-0.2.5.tar", last modified: Mon May 27 09:18:50 2024, max compression
```

## Comparing `FlowVisor-0.2.4.tar` & `FlowVisor-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:40:10.961447 FlowVisor-0.2.4/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:40:10.957447 FlowVisor-0.2.4/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-25 13:40:10.000000 FlowVisor-0.2.4/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-25 13:40:10.000000 FlowVisor-0.2.4/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-25 13:40:10.000000 FlowVisor-0.2.4/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-25 13:40:10.000000 FlowVisor-0.2.4/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-05-25 13:40:10.000000 FlowVisor-0.2.4/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-25 13:40:10.000000 FlowVisor-0.2.4/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.2.4/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-25 13:40:10.961447 FlowVisor-0.2.4/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3055 2024-05-13 12:49:23.000000 FlowVisor-0.2.4/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:40:10.961447 FlowVisor-0.2.4/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.2.4/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:40:10.961447 FlowVisor-0.2.4/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.2.4/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3446 2024-05-25 13:35:23.000000 FlowVisor-0.2.4/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.2.4/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1194 2024-05-22 11:32:42.000000 FlowVisor-0.2.4/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    16597 2024-05-25 13:37:39.000000 FlowVisor-0.2.4/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2350 2024-05-20 17:44:05.000000 FlowVisor-0.2.4/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8076 2024-05-22 09:41:15.000000 FlowVisor-0.2.4/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8494 2024-05-13 10:38:59.000000 FlowVisor-0.2.4/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.2.4/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.2.4/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.2.4/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2288 2024-05-20 18:08:09.000000 FlowVisor-0.2.4/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.2.4/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.2.4/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-25 13:40:10.961447 FlowVisor-0.2.4/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.2.4/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-27 09:18:50.533128 FlowVisor-0.2.5/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-27 09:18:50.529128 FlowVisor-0.2.5/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-27 09:18:50.000000 FlowVisor-0.2.5/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-27 09:18:50.000000 FlowVisor-0.2.5/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-27 09:18:50.000000 FlowVisor-0.2.5/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-27 09:18:50.000000 FlowVisor-0.2.5/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-05-27 09:18:50.000000 FlowVisor-0.2.5/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-27 09:18:50.000000 FlowVisor-0.2.5/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.2.5/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-27 09:18:50.533128 FlowVisor-0.2.5/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3055 2024-05-13 12:49:23.000000 FlowVisor-0.2.5/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-27 09:18:50.529128 FlowVisor-0.2.5/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.2.5/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-27 09:18:50.533128 FlowVisor-0.2.5/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.2.5/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3446 2024-05-25 13:35:23.000000 FlowVisor-0.2.5/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.2.5/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1194 2024-05-22 11:32:42.000000 FlowVisor-0.2.5/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    16597 2024-05-25 13:37:39.000000 FlowVisor-0.2.5/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2350 2024-05-20 17:44:05.000000 FlowVisor-0.2.5/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     7829 2024-05-27 08:48:01.000000 FlowVisor-0.2.5/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8494 2024-05-13 10:38:59.000000 FlowVisor-0.2.5/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.2.5/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.2.5/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.2.5/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2288 2024-05-20 18:08:09.000000 FlowVisor-0.2.5/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.2.5/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.2.5/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-27 09:18:50.533128 FlowVisor-0.2.5/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.2.5/setup.py
```

### Comparing `FlowVisor-0.2.4/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.2.5/FlowVisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.2.4
+Version: 0.2.5
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.2.4/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.2.5/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/LICENSE` & `FlowVisor-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/PKG-INFO` & `FlowVisor-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.2.4
+Version: 0.2.5
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.2.4/README.md` & `FlowVisor-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/cli/add_vis.py` & `FlowVisor-0.2.5/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/cli/remove_vis.py` & `FlowVisor-0.2.5/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/cli/vis_file.py` & `FlowVisor-0.2.5/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/flowvisor.py` & `FlowVisor-0.2.5/flowvisor/flowvisor.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/flowvisor_config.py` & `FlowVisor-0.2.5/flowvisor/flowvisor_config.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.2.5/flowvisor/flowvisor_verifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,23 @@
         res = func(*args, **kwargs)
         FlowVisorVerifier.add_entry(func, time.time() - start)
         return res
 
     return wrapper
 
 
-def vis_verifier2(func):
+def c_vis_verifier(func):
     def wrapper(*args, **kwargs):
-
-        pr = cProfile.Profile()  # create new Profiler object
-        pr.enable()  # start recording of time for Profiler
+        profiler = cProfile.Profile()
+        profiler.enable()
         res = func(*args, **kwargs)
-        pr.disable()  # stop recording of time for Profiler
-        # get the time that the function took
-
-        p = pstats.Stats(pr)
-        total_time = p.total_tt
-        FlowVisorVerifier.add_entry(func, total_time)
-        time_str = utils.get_time_as_string(total_time)
-        print(f"Function {func.__name__} took {time_str} seconds")
+        profiler.disable()
+        stats = pstats.Stats(profiler)
+        time_value = stats.total_tt
+        FlowVisorVerifier.add_entry(func, time_value)
         return res
 
     return wrapper
 
 
 class FlowVisorVerifier:
     """
```

### Comparing `FlowVisor-0.2.4/flowvisor/function_node.py` & `FlowVisor-0.2.5/flowvisor/function_node.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/logger.py` & `FlowVisor-0.2.5/flowvisor/logger.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/sankey.py` & `FlowVisor-0.2.5/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/time_tracker.py` & `FlowVisor-0.2.5/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/time_value.py` & `FlowVisor-0.2.5/flowvisor/time_value.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/flowvisor/utils.py` & `FlowVisor-0.2.5/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.4/setup.py` & `FlowVisor-0.2.5/setup.py`

 * *Files identical despite different names*

