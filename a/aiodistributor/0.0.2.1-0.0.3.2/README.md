# Comparing `tmp/aiodistributor-0.0.2.1.tar.gz` & `tmp/aiodistributor-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodistributor-0.0.2.1.tar", last modified: Sun Apr 30 20:34:45 2023, max compression
+gzip compressed data, was "aiodistributor-0.0.3.2.tar", last modified: Mon May 27 10:37:57 2024, max compression
```

## Comparing `aiodistributor-0.0.2.1.tar` & `aiodistributor-0.0.3.2.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:34:45.450617 aiodistributor-0.0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-30 20:34:45.450617 aiodistributor-0.0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:34:45.450617 aiodistributor-0.0.2.1/aiodistributor/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:34:45.450617 aiodistributor-0.0.2.1/aiodistributor/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/common/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/distributed_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/distributed_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/distributed_sliding_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/distributed_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/distributed_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/aiodistributor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 20:34:45.450617 aiodistributor-0.0.2.1/aiodistributor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-30 20:34:45.000000 aiodistributor-0.0.2.1/aiodistributor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-30 20:34:45.000000 aiodistributor-0.0.2.1/aiodistributor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 20:34:45.000000 aiodistributor-0.0.2.1/aiodistributor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-30 20:34:45.000000 aiodistributor-0.0.2.1/aiodistributor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 20:34:45.000000 aiodistributor-0.0.2.1/aiodistributor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 20:34:45.450617 aiodistributor-0.0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-30 20:34:35.000000 aiodistributor-0.0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:37:57.960675 aiodistributor-0.0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 10:37:57.960675 aiodistributor-0.0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:37:57.960675 aiodistributor-0.0.3.2/aiodistributor/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:37:57.960675 aiodistributor-0.0.3.2/aiodistributor/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/common/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distibuted_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distibuted_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_bounded_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_sliding_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/distributed_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/aiodistributor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:37:57.960675 aiodistributor-0.0.3.2/aiodistributor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-27 10:37:57.000000 aiodistributor-0.0.3.2/aiodistributor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-27 10:37:57.000000 aiodistributor-0.0.3.2/aiodistributor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:37:57.000000 aiodistributor-0.0.3.2/aiodistributor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 10:37:57.000000 aiodistributor-0.0.3.2/aiodistributor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 10:37:57.000000 aiodistributor-0.0.3.2/aiodistributor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:37:57.960675 aiodistributor-0.0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-27 10:37:50.000000 aiodistributor-0.0.3.2/setup.py
```

### Comparing `aiodistributor-0.0.2.1/LICENSE` & `aiodistributor-0.0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodistributor-0.0.2.1/PKG-INFO` & `aiodistributor-0.0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodistributor
-Version: 0.0.2.1
+Version: 0.0.3.2
 Summary: Python asynchronous library for synchronizing replicated microservices
 Home-page: https://github.com/malik89303/aiodistributor
 License: Apache License 2.0
 Platform: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
```

### Comparing `aiodistributor-0.0.2.1/README.md` & `aiodistributor-0.0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aiodistributor-0.0.2.1/aiodistributor/distributed_cache.py` & `aiodistributor-0.0.3.2/aiodistributor/distributed_cache.py`

 * *Files identical despite different names*

### Comparing `aiodistributor-0.0.2.1/aiodistributor/distributed_notifier.py` & `aiodistributor-0.0.3.2/aiodistributor/distributed_notifier.py`

 * *Files identical despite different names*

### Comparing `aiodistributor-0.0.2.1/aiodistributor/distributed_sliding_counter.py` & `aiodistributor-0.0.3.2/aiodistributor/distributed_sliding_counter.py`

 * *Files identical despite different names*

### Comparing `aiodistributor-0.0.2.1/aiodistributor/distributed_task.py` & `aiodistributor-0.0.3.2/aiodistributor/distributed_task.py`

 * *Files identical despite different names*

### Comparing `aiodistributor-0.0.2.1/aiodistributor/distributed_waiter.py` & `aiodistributor-0.0.3.2/aiodistributor/distributed_waiter.py`

 * *Files identical despite different names*

### Comparing `aiodistributor-0.0.2.1/aiodistributor.egg-info/PKG-INFO` & `aiodistributor-0.0.3.2/aiodistributor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodistributor
-Version: 0.0.2.1
+Version: 0.0.3.2
 Summary: Python asynchronous library for synchronizing replicated microservices
 Home-page: https://github.com/malik89303/aiodistributor
 License: Apache License 2.0
 Platform: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
```

### Comparing `aiodistributor-0.0.2.1/aiodistributor.egg-info/SOURCES.txt` & `aiodistributor-0.0.3.2/aiodistributor.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 LICENSE
 README.md
 setup.py
 aiodistributor/__init__.py
+aiodistributor/distibuted_barrier.py
+aiodistributor/distibuted_semaphore.py
+aiodistributor/distributed_bounded_semaphore.py
 aiodistributor/distributed_cache.py
+aiodistributor/distributed_condition.py
+aiodistributor/distributed_event.py
+aiodistributor/distributed_lock.py
 aiodistributor/distributed_notifier.py
 aiodistributor/distributed_sliding_counter.py
 aiodistributor/distributed_task.py
 aiodistributor/distributed_waiter.py
 aiodistributor/py.typed
 aiodistributor.egg-info/PKG-INFO
 aiodistributor.egg-info/SOURCES.txt
```

### Comparing `aiodistributor-0.0.2.1/setup.py` & `aiodistributor-0.0.3.2/setup.py`

 * *Files identical despite different names*

