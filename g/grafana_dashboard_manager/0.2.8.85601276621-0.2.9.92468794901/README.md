# Comparing `tmp/grafana_dashboard_manager-0.2.8.85601276621.tar.gz` & `tmp/grafana_dashboard_manager-0.2.9.92468794901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana_dashboard_manager-0.2.8.85601276621.tar", max compression
+gzip compressed data, was "grafana_dashboard_manager-0.2.9.92468794901.tar", max compression
```

## Comparing `grafana_dashboard_manager-0.2.8.85601276621.tar` & `grafana_dashboard_manager-0.2.9.92468794901.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1082 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/LICENSE
--rw-r--r--   0        0        0     4370 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/README.md
--rw-r--r--   0        0        0        0 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/__init__.py
--rw-r--r--   0        0        0     3844 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/__main__.py
--rw-r--r--   0        0        0     2260 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/api/auth.py
--rw-r--r--   0        0        0     2086 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/api/rest_client.py
--rw-r--r--   0        0        0      100 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/commands/__init__.py
--rw-r--r--   0        0        0     3252 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/commands/dashboard_download.py
--rw-r--r--   0        0        0     6242 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/commands/dashboard_upload.py
--rw-r--r--   0        0        0      367 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/exceptions.py
--rw-r--r--   0        0        0     3442 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/global_config.py
--rw-r--r--   0        0        0      249 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/grafana/__init__.py
--rw-r--r--   0        0        0     2229 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/grafana/grafana_api.py
--rw-r--r--   0        0        0     4289 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/handlers/api_dashboards.py
--rw-r--r--   0        0        0     3610 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/handlers/api_folders.py
--rw-r--r--   0        0        0     1567 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/handlers/base_handler.py
--rw-r--r--   0        0        0      343 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/models/__init__.py
--rw-r--r--   0        0        0     1185 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/models/dashboard.py
--rw-r--r--   0        0        0      559 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/models/folder.py
--rw-r--r--   0        0        0     3388 2024-04-04 19:18:26.329736 grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/utils.py
--rw-r--r--   0        0        0      857 2024-04-04 19:18:41.941872 grafana_dashboard_manager-0.2.8.85601276621/pyproject.toml
--rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 grafana_dashboard_manager-0.2.8.85601276621/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/LICENSE
+-rw-r--r--   0        0        0     4370 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/__main__.py
+-rw-r--r--   0        0        0     2260 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/api/auth.py
+-rw-r--r--   0        0        0     2086 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/api/rest_client.py
+-rw-r--r--   0        0        0      100 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/commands/__init__.py
+-rw-r--r--   0        0        0     3252 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/commands/dashboard_download.py
+-rw-r--r--   0        0        0     6242 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/commands/dashboard_upload.py
+-rw-r--r--   0        0        0      367 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/exceptions.py
+-rw-r--r--   0        0        0     3442 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/global_config.py
+-rw-r--r--   0        0        0      249 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/grafana/__init__.py
+-rw-r--r--   0        0        0     2229 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/grafana/grafana_api.py
+-rw-r--r--   0        0        0     4289 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/handlers/api_dashboards.py
+-rw-r--r--   0        0        0     3610 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/handlers/api_folders.py
+-rw-r--r--   0        0        0     1567 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/handlers/base_handler.py
+-rw-r--r--   0        0        0      343 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/models/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-26 23:15:57.933326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/models/dashboard.py
+-rw-r--r--   0        0        0      559 2024-05-26 23:15:57.937326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/models/folder.py
+-rw-r--r--   0        0        0     3415 2024-05-26 23:15:57.937326 grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/utils.py
+-rw-r--r--   0        0        0      857 2024-05-26 23:16:19.249254 grafana_dashboard_manager-0.2.9.92468794901/pyproject.toml
+-rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 grafana_dashboard_manager-0.2.9.92468794901/PKG-INFO
```

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/LICENSE` & `grafana_dashboard_manager-0.2.9.92468794901/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/README.md` & `grafana_dashboard_manager-0.2.9.92468794901/README.md`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/__main__.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/api/auth.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/api/auth.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/api/rest_client.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/api/rest_client.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/commands/dashboard_download.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/commands/dashboard_download.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/commands/dashboard_upload.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/commands/dashboard_upload.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/global_config.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/global_config.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/grafana/grafana_api.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/grafana/grafana_api.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/handlers/api_dashboards.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/handlers/api_dashboards.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/handlers/api_folders.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/handlers/api_folders.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/handlers/base_handler.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/models/dashboard.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/models/folder.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/models/folder.py`

 * *Files identical despite different names*

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/grafana_dashboard_manager/utils.py` & `grafana_dashboard_manager-0.2.9.92468794901/grafana_dashboard_manager/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # In normal usage, don't log every http request
     if log_level == "INFO":
         logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
 def parse_pyproject() -> dict:
     """Returns a dict of the pyproject.toml file"""
-    with open("pyproject.toml") as file:
+    with (Path(__file__) / ".." / "pyproject.toml").open() as file:
         return tomllib.loads(file.read())
 
 
 def confirm(user_prompt: str):
     """A user interactive call to confirm an action"""
     should_continue = Confirm.ask(user_prompt)
     if not should_continue:
```

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/pyproject.toml` & `grafana_dashboard_manager-0.2.9.92468794901/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grafana_dashboard_manager"
-version = "0.2.8.85601276621"
+version = "0.2.9.92468794901"
 description = "A cli utility that uses Grafana's HTTP API to easily save and restore dashboards."
 authors = ["Vince Chan <vince@beamconnectivity.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.beamconnectivity.com"
 repository = "https://github.com/Beam-Connectivity/grafana-dashboard-manager"
 keywords = ["grafana", "dashboard", "json"]
```

### Comparing `grafana_dashboard_manager-0.2.8.85601276621/PKG-INFO` & `grafana_dashboard_manager-0.2.9.92468794901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana_dashboard_manager
-Version: 0.2.8.85601276621
+Version: 0.2.9.92468794901
 Summary: A cli utility that uses Grafana's HTTP API to easily save and restore dashboards.
 Home-page: https://www.beamconnectivity.com
 License: MIT
 Keywords: grafana,dashboard,json
 Author: Vince Chan
 Author-email: vince@beamconnectivity.com
 Requires-Python: >=3.11,<4.0
```

