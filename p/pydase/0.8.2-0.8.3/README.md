# Comparing `tmp/pydase-0.8.2.tar.gz` & `tmp/pydase-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydase-0.8.2.tar", max compression
+gzip compressed data, was "pydase-0.8.3.tar", max compression
```

## Comparing `pydase-0.8.2.tar` & `pydase-0.8.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1093 2024-04-30 13:57:06.808636 pydase-0.8.2/LICENSE
--rw-r--r--   0        0        0    38837 2024-04-30 13:57:06.808636 pydase-0.8.2/README.md
--rw-r--r--   0        0        0     2529 2024-04-30 13:57:06.816636 pydase-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      243 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/__init__.py
--rw-r--r--   0        0        0       62 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/client/__init__.py
--rw-r--r--   0        0        0     5228 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/client/client.py
--rw-r--r--   0        0        0    14335 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/client/proxy_loader.py
--rw-r--r--   0        0        0     1497 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/components/__init__.py
--rw-r--r--   0        0        0     2172 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/components/coloured_enum.py
--rw-r--r--   0        0        0     3158 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/components/device_connection.py
--rw-r--r--   0        0        0     2496 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/components/image.py
--rw-r--r--   0        0        0     3080 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/components/number_slider.py
--rw-r--r--   0        0        0      639 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/config.py
--rw-r--r--   0        0        0       91 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/data_service/__init__.py
--rw-r--r--   0        0        0      427 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/data_service/abstract_data_service.py
--rw-r--r--   0        0        0     4112 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/data_service/data_service.py
--rw-r--r--   0        0        0     1595 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/data_service/data_service_cache.py
--rw-r--r--   0        0        0     4987 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/data_service/data_service_observer.py
--rw-r--r--   0        0        0    11974 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/data_service/state_manager.py
--rw-r--r--   0        0        0     8766 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/data_service/task_manager.py
--rw-r--r--   0        0        0      369 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/frontend/asset-manifest.json
--rw-r--r--   0        0        0      638 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/frontend/index.html
--rw-r--r--   0        0        0      492 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/frontend/manifest.json
--rw-r--r--   0        0        0       67 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/frontend/robots.txt
--rw-r--r--   0        0        0   236395 2024-04-30 13:57:06.816636 pydase-0.8.2/src/pydase/frontend/static/css/main.7ef670d5.css
--rw-r--r--   0        0        0   544448 2024-04-30 13:57:06.820636 pydase-0.8.2/src/pydase/frontend/static/css/main.7ef670d5.css.map
--rw-r--r--   0        0        0   360367 2024-04-30 13:57:06.820636 pydase-0.8.2/src/pydase/frontend/static/js/main.57f8ec4c.js
--rw-r--r--   0        0        0     1093 2024-04-30 13:57:06.820636 pydase-0.8.2/src/pydase/frontend/static/js/main.57f8ec4c.js.LICENSE.txt
--rw-r--r--   0        0        0  1424759 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/frontend/static/js/main.57f8ec4c.js.map
--rw-r--r--   0        0        0        0 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/observer_pattern/__init__.py
--rw-r--r--   0        0        0       95 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/observer_pattern/observable/__init__.py
--rw-r--r--   0        0        0     2564 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/observer_pattern/observable/observable.py
--rw-r--r--   0        0        0    10558 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/observer_pattern/observable/observable_object.py
--rw-r--r--   0        0        0      198 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/observer_pattern/observer/__init__.py
--rw-r--r--   0        0        0     1007 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/observer_pattern/observer/observer.py
--rw-r--r--   0        0        0     3564 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/observer_pattern/observer/property_observer.py
--rw-r--r--   0        0        0        0 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/py.typed
--rw-r--r--   0        0        0      144 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/server/__init__.py
--rw-r--r--   0        0        0    11199 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/server/server.py
--rw-r--r--   0        0        0       83 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/server/web_server/__init__.py
--rw-r--r--   0        0        0     5518 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/server/web_server/sio_setup.py
--rw-r--r--   0        0        0     8154 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/server/web_server/web_server.py
--rw-r--r--   0        0        0     1826 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/units.py
--rw-r--r--   0        0        0        0 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/decorators.py
--rw-r--r--   0        0        0     6494 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/helpers.py
--rw-r--r--   0        0        0     5161 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/logging.py
--rw-r--r--   0        0        0        0 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/serialization/__init__.py
--rw-r--r--   0        0        0     5505 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/serialization/deserializer.py
--rw-r--r--   0        0        0    18364 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/serialization/serializer.py
--rw-r--r--   0        0        0     2411 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/utils/serialization/types.py
--rw-r--r--   0        0        0      165 2024-04-30 13:57:06.828636 pydase-0.8.2/src/pydase/version.py
--rw-r--r--   0        0        0    39789 1970-01-01 00:00:00.000000 pydase-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-05-27 13:13:11.737394 pydase-0.8.3/LICENSE
+-rw-r--r--   0        0        0    38837 2024-05-27 13:13:11.737394 pydase-0.8.3/README.md
+-rw-r--r--   0        0        0     2529 2024-05-27 13:13:11.745395 pydase-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      243 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/client/__init__.py
+-rw-r--r--   0        0        0     5228 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/client/client.py
+-rw-r--r--   0        0        0    14335 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/client/proxy_loader.py
+-rw-r--r--   0        0        0     1497 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/components/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/components/coloured_enum.py
+-rw-r--r--   0        0        0     3158 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/components/device_connection.py
+-rw-r--r--   0        0        0     2496 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/components/image.py
+-rw-r--r--   0        0        0     3080 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/components/number_slider.py
+-rw-r--r--   0        0        0      639 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/config.py
+-rw-r--r--   0        0        0       91 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/data_service/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/data_service/abstract_data_service.py
+-rw-r--r--   0        0        0     4112 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/data_service/data_service.py
+-rw-r--r--   0        0        0     1595 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/data_service/data_service_cache.py
+-rw-r--r--   0        0        0     4987 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/data_service/data_service_observer.py
+-rw-r--r--   0        0        0    11974 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/data_service/state_manager.py
+-rw-r--r--   0        0        0     8705 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/data_service/task_manager.py
+-rw-r--r--   0        0        0      369 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/frontend/asset-manifest.json
+-rw-r--r--   0        0        0      638 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/frontend/index.html
+-rw-r--r--   0        0        0      492 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/frontend/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/frontend/robots.txt
+-rw-r--r--   0        0        0   236395 2024-05-27 13:13:11.745395 pydase-0.8.3/src/pydase/frontend/static/css/main.7ef670d5.css
+-rw-r--r--   0        0        0   544448 2024-05-27 13:13:11.749395 pydase-0.8.3/src/pydase/frontend/static/css/main.7ef670d5.css.map
+-rw-r--r--   0        0        0   360367 2024-05-27 13:13:11.749395 pydase-0.8.3/src/pydase/frontend/static/js/main.57f8ec4c.js
+-rw-r--r--   0        0        0     1093 2024-05-27 13:13:11.749395 pydase-0.8.3/src/pydase/frontend/static/js/main.57f8ec4c.js.LICENSE.txt
+-rw-r--r--   0        0        0  1424759 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/frontend/static/js/main.57f8ec4c.js.map
+-rw-r--r--   0        0        0        0 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/observer_pattern/__init__.py
+-rw-r--r--   0        0        0       95 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/observer_pattern/observable/__init__.py
+-rw-r--r--   0        0        0     2564 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/observer_pattern/observable/observable.py
+-rw-r--r--   0        0        0    11182 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/observer_pattern/observable/observable_object.py
+-rw-r--r--   0        0        0      198 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/observer_pattern/observer/__init__.py
+-rw-r--r--   0        0        0     1007 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/observer_pattern/observer/observer.py
+-rw-r--r--   0        0        0     3564 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/observer_pattern/observer/property_observer.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/py.typed
+-rw-r--r--   0        0        0      144 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/server/__init__.py
+-rw-r--r--   0        0        0    11199 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/server/server.py
+-rw-r--r--   0        0        0       83 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/server/web_server/__init__.py
+-rw-r--r--   0        0        0     5518 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/server/web_server/sio_setup.py
+-rw-r--r--   0        0        0     8154 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/server/web_server/web_server.py
+-rw-r--r--   0        0        0     1826 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/units.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/__init__.py
+-rw-r--r--   0        0        0     1298 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/decorators.py
+-rw-r--r--   0        0        0     6494 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/helpers.py
+-rw-r--r--   0        0        0     5161 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/logging.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/serialization/__init__.py
+-rw-r--r--   0        0        0     5505 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/serialization/deserializer.py
+-rw-r--r--   0        0        0    18364 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/serialization/serializer.py
+-rw-r--r--   0        0        0     2411 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/utils/serialization/types.py
+-rw-r--r--   0        0        0      165 2024-05-27 13:13:11.757394 pydase-0.8.3/src/pydase/version.py
+-rw-r--r--   0        0        0    39789 1970-01-01 00:00:00.000000 pydase-0.8.3/PKG-INFO
```

### Comparing `pydase-0.8.2/LICENSE` & `pydase-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/README.md` & `pydase-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/pyproject.toml` & `pydase-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydase"
-version = "0.8.2"
+version = "0.8.3"
 description = "A flexible and robust Python library for creating, managing, and interacting with data services, with built-in support for web and RPC servers, and customizable features for diverse use cases."
 authors = ["Mose Mueller <mosmuell@ethz.ch>"]
 readme = "README.md"
 packages = [{ include = "pydase", from = "src" }]
 
 
 [tool.poetry.dependencies]
```

### Comparing `pydase-0.8.2/src/pydase/client/client.py` & `pydase-0.8.3/src/pydase/client/client.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/client/proxy_loader.py` & `pydase-0.8.3/src/pydase/client/proxy_loader.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/components/__init__.py` & `pydase-0.8.3/src/pydase/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/components/coloured_enum.py` & `pydase-0.8.3/src/pydase/components/coloured_enum.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/components/device_connection.py` & `pydase-0.8.3/src/pydase/components/device_connection.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/components/image.py` & `pydase-0.8.3/src/pydase/components/image.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/components/number_slider.py` & `pydase-0.8.3/src/pydase/components/number_slider.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/config.py` & `pydase-0.8.3/src/pydase/config.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/data_service/data_service.py` & `pydase-0.8.3/src/pydase/data_service/data_service.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/data_service/data_service_cache.py` & `pydase-0.8.3/src/pydase/data_service/data_service_cache.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/data_service/data_service_observer.py` & `pydase-0.8.3/src/pydase/data_service/data_service_observer.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/data_service/state_manager.py` & `pydase-0.8.3/src/pydase/data_service/state_manager.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/data_service/task_manager.py` & `pydase-0.8.3/src/pydase/data_service/task_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,14 @@
     from collections.abc import Callable
 
     from .data_service import DataService
 
 logger = logging.getLogger(__name__)
 
 
-class TaskDefinitionError(Exception):
-    pass
-
-
 class TaskStatus(Enum):
     RUNNING = "running"
 
 
 class TaskManager:
     """
     The TaskManager class is a utility designed to manage asynchronous tasks. It
@@ -103,20 +99,21 @@
             # circumvents calling properties
             if is_property_attribute(self.service, name):
                 continue
 
             method = getattr(self.service, name)
             if inspect.iscoroutinefunction(method):
                 if function_has_arguments(method):
-                    raise TaskDefinitionError(
-                        "Asynchronous functions (tasks) should be defined without "
-                        f"arguments. The task '{method.__name__}' has at least one "
-                        "argument. Please remove the argument(s) from this function to "
-                        "use it."
+                    logger.info(
+                        "Async function %a is defined with at least one argument. If "
+                        "you want to use it as a task, remove the argument(s) from the "
+                        "function definition.",
+                        method.__name__,
                     )
+                    continue
 
                 # create start and stop methods for each coroutine
                 setattr(
                     self.service, f"start_{name}", self._make_start_task(name, method)
                 )
                 setattr(self.service, f"stop_{name}", self._make_stop_task(name))
```

### Comparing `pydase-0.8.2/src/pydase/frontend/index.html` & `pydase-0.8.3/src/pydase/frontend/index.html`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/frontend/static/css/main.7ef670d5.css` & `pydase-0.8.3/src/pydase/frontend/static/css/main.7ef670d5.css`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/frontend/static/css/main.7ef670d5.css.map` & `pydase-0.8.3/src/pydase/frontend/static/css/main.7ef670d5.css.map`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/frontend/static/js/main.57f8ec4c.js` & `pydase-0.8.3/src/pydase/frontend/static/js/main.57f8ec4c.js`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/frontend/static/js/main.57f8ec4c.js.LICENSE.txt` & `pydase-0.8.3/src/pydase/frontend/static/js/main.57f8ec4c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/frontend/static/js/main.57f8ec4c.js.map` & `pydase-0.8.3/src/pydase/frontend/static/js/main.57f8ec4c.js.map`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/observer_pattern/observable/observable.py` & `pydase-0.8.3/src/pydase/observer_pattern/observable/observable.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/observer_pattern/observable/observable_object.py` & `pydase-0.8.3/src/pydase/observer_pattern/observable/observable_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,48 @@
+from __future__ import annotations
+
 import logging
+import weakref
 from abc import ABC, abstractmethod
-from collections.abc import Iterable
 from typing import TYPE_CHECKING, Any, ClassVar, SupportsIndex
 
 from pydase.utils.helpers import parse_serialized_key
 
 if TYPE_CHECKING:
+    from collections.abc import Iterable
+
     from pydase.observer_pattern.observer.observer import Observer
 
 logger = logging.getLogger(__name__)
 
 
 class ObservableObject(ABC):
-    _list_mapping: ClassVar[dict[int, "_ObservableList"]] = {}
-    _dict_mapping: ClassVar[dict[int, "_ObservableDict"]] = {}
+    _list_mapping: ClassVar[dict[int, weakref.ReferenceType[_ObservableList]]] = {}
+    _dict_mapping: ClassVar[dict[int, weakref.ReferenceType[_ObservableDict]]] = {}
 
     def __init__(self) -> None:
         if not hasattr(self, "_observers"):
-            self._observers: dict[str, list["ObservableObject | Observer"]] = {}
+            self._observers: dict[str, list[ObservableObject | Observer]] = {}
 
     def add_observer(
-        self, observer: "ObservableObject | Observer", attr_name: str = ""
+        self, observer: ObservableObject | Observer, attr_name: str = ""
     ) -> None:
         if attr_name not in self._observers:
             self._observers[attr_name] = []
         if observer not in self._observers[attr_name]:
             self._observers[attr_name].append(observer)
 
-    def _remove_observer(self, observer: "ObservableObject", attribute: str) -> None:
+    def _remove_observer(self, observer: ObservableObject, attribute: str) -> None:
         if attribute in self._observers:
             self._observers[attribute].remove(observer)
 
+            # remove attribute key from observers dict if list of observers is empty
+            if not self._observers[attribute]:
+                del self._observers[attribute]
+
     @abstractmethod
     def _remove_observer_if_observable(self, name: str) -> None:
         """Removes the current object as an observer from an observable attribute.
 
         This method is called before an attribute of the observable object is
         changed. If the current value of the attribute is an instance of
         `ObservableObject`, this method removes the current object from its list
@@ -84,27 +92,31 @@
                 observer._notify_change_start(extended_attr_path)
 
     def _initialise_new_objects(self, attr_name_or_key: str, value: Any) -> Any:
         new_value = value
         if isinstance(value, list):
             if id(value) in self._list_mapping:
                 # If the list `value` was already referenced somewhere else
-                new_value = self._list_mapping[id(value)]
+                new_value = self._list_mapping[id(value)]()
             else:
                 # convert the builtin list into a ObservableList
                 new_value = _ObservableList(original_list=value)
-                self._list_mapping[id(value)] = new_value
+
+                # Use weakref to allow the GC to collect unused objects
+                self._list_mapping[id(value)] = weakref.ref(new_value)
         elif isinstance(value, dict):
             if id(value) in self._dict_mapping:
                 # If the dict `value` was already referenced somewhere else
-                new_value = self._dict_mapping[id(value)]
+                new_value = self._dict_mapping[id(value)]()
             else:
-                # convert the builtin list into a ObservableList
+                # convert the builtin dict into a ObservableDict
                 new_value = _ObservableDict(original_dict=value)
-                self._dict_mapping[id(value)] = new_value
+
+                # Use weakref to allow the GC to collect unused objects
+                self._dict_mapping[id(value)] = weakref.ref(new_value)
         if isinstance(new_value, ObservableObject):
             new_value.add_observer(self, attr_name_or_key)
         return new_value
 
     @abstractmethod
     def _construct_extended_attr_path(
         self, observer_attr_name: str, instance_attr_name: str
@@ -135,14 +147,17 @@
     ) -> None:
         self._original_list = original_list
         ObservableObject.__init__(self)
         list.__init__(self, self._original_list)
         for i, item in enumerate(self._original_list):
             super().__setitem__(i, self._initialise_new_objects(f"[{i}]", item))
 
+    def __del__(self) -> None:
+        self._list_mapping.pop(id(self._original_list))
+
     def __setitem__(self, key: int, value: Any) -> None:  # type: ignore[override]
         if hasattr(self, "_observers"):
             self._remove_observer_if_observable(f"[{key}]")
             value = self._initialise_new_objects(f"[{key}]", value)
             self._notify_change_start(f"[{key}]")
 
         super().__setitem__(key, value)
@@ -233,14 +248,17 @@
     ) -> None:
         self._original_dict = original_dict
         ObservableObject.__init__(self)
         dict.__init__(self)
         for key, value in self._original_dict.items():
             self.__setitem__(key, self._initialise_new_objects(f'["{key}"]', value))
 
+    def __del__(self) -> None:
+        self._dict_mapping.pop(id(self._original_dict))
+
     def __setitem__(self, key: str, value: Any) -> None:
         if not isinstance(key, str):
             raise ValueError(
                 f"Invalid key type: {key} ({type(key).__name__}). In pydase services, "
                 "dictionary keys must be strings."
             )
```

### Comparing `pydase-0.8.2/src/pydase/observer_pattern/observer/observer.py` & `pydase-0.8.3/src/pydase/observer_pattern/observer/observer.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/observer_pattern/observer/property_observer.py` & `pydase-0.8.3/src/pydase/observer_pattern/observer/property_observer.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/server/server.py` & `pydase-0.8.3/src/pydase/server/server.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/server/web_server/sio_setup.py` & `pydase-0.8.3/src/pydase/server/web_server/sio_setup.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/server/web_server/web_server.py` & `pydase-0.8.3/src/pydase/server/web_server/web_server.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/units.py` & `pydase-0.8.3/src/pydase/units.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/utils/decorators.py` & `pydase-0.8.3/src/pydase/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/utils/helpers.py` & `pydase-0.8.3/src/pydase/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/utils/logging.py` & `pydase-0.8.3/src/pydase/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/utils/serialization/deserializer.py` & `pydase-0.8.3/src/pydase/utils/serialization/deserializer.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/utils/serialization/serializer.py` & `pydase-0.8.3/src/pydase/utils/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/src/pydase/utils/serialization/types.py` & `pydase-0.8.3/src/pydase/utils/serialization/types.py`

 * *Files identical despite different names*

### Comparing `pydase-0.8.2/PKG-INFO` & `pydase-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydase
-Version: 0.8.2
+Version: 0.8.3
 Summary: A flexible and robust Python library for creating, managing, and interacting with data services, with built-in support for web and RPC servers, and customizable features for diverse use cases.
 Author: Mose Mueller
 Author-email: mosmuell@ethz.ch
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

