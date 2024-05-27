# Comparing `tmp/ambient_edge_server-0.1.1.tar.gz` & `tmp/ambient_edge_server-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_edge_server-0.1.1.tar", last modified: Mon May 27 19:40:54 2024, max compression
+gzip compressed data, was "ambient_edge_server-0.1.2.tar", last modified: Mon May 27 20:00:42 2024, max compression
```

## Comparing `ambient_edge_server-0.1.1.tar` & `ambient_edge_server-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:54.673868 ambient_edge_server-0.1.1/ambient_edge_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/deploy_service_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/test_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/ambient_edge_server/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/routers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/routers/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/routers/ports.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/ambient_edge_server/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/services/authorization_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/services/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/services/handler_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/services/port_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/services/service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/ambient_edge_server/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/ambient_edge_server/utils/custom_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/ambient_edge_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 19:40:54.000000 ambient_edge_server-0.1.1/ambient_edge_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-27 19:40:54.000000 ambient_edge_server-0.1.1/ambient_edge_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:40:54.000000 ambient_edge_server-0.1.1/ambient_edge_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 19:40:54.000000 ambient_edge_server-0.1.1/ambient_edge_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 19:40:54.000000 ambient_edge_server-0.1.1/ambient_edge_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 19:40:54.000000 ambient_edge_server-0.1.1/ambient_edge_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:40:54.677868 ambient_edge_server-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-27 19:40:44.000000 ambient_edge_server-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:42.438562 ambient_edge_server-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:00:42.438562 ambient_edge_server-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:42.434562 ambient_edge_server-0.1.2/ambient_edge_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:42.434562 ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/deploy_service_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/test_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:42.438562 ambient_edge_server-0.1.2/ambient_edge_server/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/routers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/routers/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/routers/ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:42.438562 ambient_edge_server-0.1.2/ambient_edge_server/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/services/authorization_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/services/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/services/handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/services/port_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/services/service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:42.438562 ambient_edge_server-0.1.2/ambient_edge_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/ambient_edge_server/utils/custom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:42.434562 ambient_edge_server-0.1.2/ambient_edge_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:00:42.000000 ambient_edge_server-0.1.2/ambient_edge_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-27 20:00:42.000000 ambient_edge_server-0.1.2/ambient_edge_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:00:42.000000 ambient_edge_server-0.1.2/ambient_edge_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-27 20:00:42.000000 ambient_edge_server-0.1.2/ambient_edge_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-27 20:00:42.000000 ambient_edge_server-0.1.2/ambient_edge_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 20:00:42.000000 ambient_edge_server-0.1.2/ambient_edge_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:00:42.438562 ambient_edge_server-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-27 20:00:27.000000 ambient_edge_server-0.1.2/setup.py
```

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/app.py` & `ambient_edge_server-0.1.2/ambient_edge_server/app.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/base_handler.py` & `ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/deploy_service_handler.py` & `ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/deploy_service_handler.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/event_handlers/test_handler.py` & `ambient_edge_server-0.1.2/ambient_edge_server/event_handlers/test_handler.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/routers/auth.py` & `ambient_edge_server-0.1.2/ambient_edge_server/routers/auth.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/routers/ping.py` & `ambient_edge_server-0.1.2/ambient_edge_server/routers/ping.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/routers/ports.py` & `ambient_edge_server-0.1.2/ambient_edge_server/routers/ports.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/services/authorization_service.py` & `ambient_edge_server-0.1.2/ambient_edge_server/services/authorization_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/services/event_service.py` & `ambient_edge_server-0.1.2/ambient_edge_server/services/event_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/services/handler_service.py` & `ambient_edge_server-0.1.2/ambient_edge_server/services/handler_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/services/port_service.py` & `ambient_edge_server-0.1.2/ambient_edge_server/services/port_service.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server/services/service_manager.py` & `ambient_edge_server-0.1.2/ambient_edge_server/services/service_manager.py`

 * *Files identical despite different names*

### Comparing `ambient_edge_server-0.1.1/ambient_edge_server.egg-info/SOURCES.txt` & `ambient_edge_server-0.1.2/ambient_edge_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

