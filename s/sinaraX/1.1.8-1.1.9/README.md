# Comparing `tmp/sinarax-1.1.8.tar.gz` & `tmp/sinarax-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinarax-1.1.8.tar", max compression
+gzip compressed data, was "sinarax-1.1.9.tar", max compression
```

## Comparing `sinarax-1.1.8.tar` & `sinarax-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-05-16 07:51:03.361892 sinarax-1.1.8/LICENSE
--rw-r--r--   0        0        0     2212 2024-05-16 07:51:03.361892 sinarax-1.1.8/README.md
--rw-r--r--   0        0        0     1129 2024-05-16 07:51:03.361892 sinarax-1.1.8/pyproject.toml
--rw-r--r--   0        0        0       61 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/__init__.py
--rw-r--r--   0        0        0      428 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/__main__.py
--rw-r--r--   0        0        0       93 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/_version.py
--rw-r--r--   0        0        0       85 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/__init__.py
--rw-r--r--   0        0        0       68 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/file_screen/__init__.py
--rw-r--r--   0        0        0     3416 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/file_screen/file_tree.py
--rw-r--r--   0        0        0     6458 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/main.py
--rw-r--r--   0        0        0     6278 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/running.py
--rw-r--r--   0        0        0    14035 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/server.py
--rw-r--r--   0        0        0     2948 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/server_cfg.py
--rw-r--r--   0        0        0      963 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/style.css
--rw-r--r--   0        0        0     2403 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/update.py
--rw-r--r--   0        0        0      650 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/config.py
--rw-r--r--   0        0        0     5721 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/infra.py
--rw-r--r--   0        0        0     1564 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/process.py
--rw-r--r--   0        0        0      847 2024-05-16 07:51:03.361892 sinarax-1.1.8/sinaraX/screens/utils/sinara_server_utils.py
--rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 sinarax-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-27 13:08:26.350793 sinarax-1.1.9/LICENSE
+-rw-r--r--   0        0        0     2212 2024-05-27 13:08:26.350793 sinarax-1.1.9/README.md
+-rw-r--r--   0        0        0     1129 2024-05-27 13:08:26.350793 sinarax-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/__init__.py
+-rw-r--r--   0        0        0      428 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/__main__.py
+-rw-r--r--   0        0        0       93 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/_version.py
+-rw-r--r--   0        0        0       85 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/file_screen/__init__.py
+-rw-r--r--   0        0        0     3416 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/file_screen/file_tree.py
+-rw-r--r--   0        0        0     6566 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/main.py
+-rw-r--r--   0        0        0     6278 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/running.py
+-rw-r--r--   0        0        0    13070 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/server.py
+-rw-r--r--   0        0        0     2948 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/server_cfg.py
+-rw-r--r--   0        0        0      963 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/style.css
+-rw-r--r--   0        0        0     2403 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/update.py
+-rw-r--r--   0        0        0      608 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/utils/__init__.py
+-rw-r--r--   0        0        0     4795 2024-05-27 13:08:26.350793 sinarax-1.1.9/sinaraX/screens/utils/config.py
+-rw-r--r--   0        0        0     6018 2024-05-27 13:08:26.354793 sinarax-1.1.9/sinaraX/screens/utils/infra.py
+-rw-r--r--   0        0        0     1564 2024-05-27 13:08:26.354793 sinarax-1.1.9/sinaraX/screens/utils/process.py
+-rw-r--r--   0        0        0      847 2024-05-27 13:08:26.354793 sinarax-1.1.9/sinaraX/screens/utils/sinara_server_utils.py
+-rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 sinarax-1.1.9/PKG-INFO
```

### Comparing `sinarax-1.1.8/LICENSE` & `sinarax-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/README.md` & `sinarax-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/pyproject.toml` & `sinarax-1.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sinaraX"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.md"
 authors = ["MiXaiLL76 <mike.milos@yandex.ru>"]
 description = "sinaraX - TUI for sinaraml clin"
 keywords = ["sinaraX", "tui", "cli", "sinaraml", "sinara"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
@@ -19,15 +19,15 @@
 ]
 packages = [{ include = "sinaraX" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 textual = { version = ">=0.57.1" }
 requests = { version = "*" }
-sinaraml = { version = ">=2024.3.12" }
+sinaraml = { version = ">=2024.4.23" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 sinaraX = "sinaraX.__main__:main"
```

### Comparing `sinarax-1.1.8/sinaraX/screens/file_screen/file_tree.py` & `sinarax-1.1.9/sinaraX/screens/file_screen/file_tree.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/sinaraX/screens/main.py` & `sinarax-1.1.9/sinaraX/screens/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .server_cfg import BaseFunctions
 from .update import UpdateScreen
 from .utils.infra import (
     check_docker,
     check_docker_group,
     check_last_version,
     check_platform,
+    update_sinara_org,
 )
 
 
 class SinaraX(App, BaseFunctions):
     CSS_PATH = "style.css"
     system_info_data = None
     SCREENS = {
@@ -104,14 +105,18 @@
         )
         yield self.log_window
 
         if self.system_info_data is None:
             self.get_system_info()
 
     @work(thread=True)
+    def update_sinara_org(self):
+        update_sinara_org()
+
+    @work(thread=True)
     def get_system_info(self):
         self.system_info_data = {
             "docker_info": check_docker(),
             "platform_info": check_platform(),
             "group_info": check_docker_group(),
             "sinaraX": (
                 check_last_version("sinaraX")
```

### Comparing `sinarax-1.1.8/sinaraX/screens/running.py` & `sinarax-1.1.9/sinaraX/screens/running.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/sinaraX/screens/server.py` & `sinarax-1.1.9/sinaraX/screens/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,29 +133,14 @@
                                 value="jovyan-single-use",
                                 name="instanceName",
                             )
 
                         with Horizontal():
                             with Vertical():
                                 with Collapsible(
-                                    title=(
-                                        "Host where the server is run"
-                                        " (disabled!)"
-                                    ),
-                                    collapsed=False,
-                                ):
-                                    with RadioSet(
-                                        name="platform",
-                                        disabled=True,
-                                    ):
-                                        yield RadioButton("Desktop", value=True)
-                                        yield RadioButton("Remote")
-
-                            with Vertical():
-                                with Collapsible(
                                     title="Sinara image for", collapsed=False
                                 ):
                                     with RadioSet(name="sinara_image_num"):
                                         yield RadioButton("CV", value=True)
                                         yield RadioButton("ML")
 
                     with TabPane("Resource", id="resource"):
@@ -177,17 +162,18 @@
                                 name="memLimit",
                             )
 
                             yield Static(
                                 "Maximum amount of shared memory for"
                                 " server container"
                             )
+                            # shm_size -> shmSize 27.05.2024
                             yield Input(
                                 value=str(base_shm_size) + "g",
-                                name="shm_size",
+                                name="shmSize",
                             )
 
                         with Collapsible(title="Cpu", collapsed=False):
                             yield Static(
                                 " Number of CPU cores to use for"
                                 " server container"
                             )
@@ -198,20 +184,14 @@
                             )
 
                     with TabPane("Extra", id="extra"):
                         with Collapsible(
                             title="Server config", collapsed=False
                         ):
                             yield Checkbox(
-                                "Create Folders (disabled!)",
-                                value=True,
-                                name="createFolders",
-                                disabled=True,
-                            )
-                            yield Checkbox(
                                 "Gpu Enabled", value=True, name="gpuEnabled"
                             )
                             yield Checkbox(
                                 "Run server without password protection",
                                 value=False,
                                 name="insecure",
                             )
```

### Comparing `sinarax-1.1.8/sinaraX/screens/server_cfg.py` & `sinarax-1.1.9/sinaraX/screens/server_cfg.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/sinaraX/screens/style.css` & `sinarax-1.1.9/sinaraX/screens/style.css`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/sinaraX/screens/update.py` & `sinarax-1.1.9/sinaraX/screens/update.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/sinaraX/screens/utils/__init__.py` & `sinarax-1.1.9/sinaraX/screens/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from .config import (
     FilteredConfigTree,
     SinaraImageType,
-    SinaraPlatform,
     SinaraRunMode,
     generate_from_screen,
     load_from_file,
 )
 from .process import decode_lines, start_cmd
 from .sinara_server_utils import (
     get_cpu_cores_limit,
@@ -17,14 +16,13 @@
 __all__ = [
     "generate_from_screen",
     "load_from_file",
     "start_cmd",
     "decode_lines",
     "SinaraImageType",
     "SinaraRunMode",
-    "SinaraPlatform",
     "FilteredConfigTree",
     "get_cpu_cores_limit",
     "get_system_memory_size",
     "get_memory_size_limit",
     "get_default_shm_size",
 ]
```

### Comparing `sinarax-1.1.8/sinaraX/screens/utils/config.py` & `sinarax-1.1.9/sinaraX/screens/utils/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 
 
 class SinaraRunMode(enum.Enum):
     Quick = 0
     Basic = 1
 
 
-class SinaraPlatform(enum.Enum):
-    Desktop = 0
-    Remote = 1
-
-
 class FilteredConfigTree(DirectoryTree):
     def filter_paths(self, paths: Iterable[Path]) -> Iterable[Path]:
         return [
             path
             for path in paths
             if (path.is_file() and path.name.endswith(".json"))
         ]
@@ -48,22 +43,17 @@
             SinaraRunMode.Quick.value: "q",
             SinaraRunMode.Basic.value: "b",
         },
         "sinara_image_num": {
             SinaraImageType.CV.value: "2",
             SinaraImageType.ML.value: "1",
         },
-        "platform": {
-            SinaraPlatform.Desktop.value: "desktop",
-            SinaraPlatform.Remote.value: "remote",
-        },
     }
 
     _remap_checkbox = {
-        "createFolders": {True: "y", False: "n"},
         "gpuEnabled": {True: "y", False: "n"},
         "experimental": {True: " ", False: None},
         "insecure": {True: " ", False: None},
     }
 
     if _dict.get("memLimit"):
         if _from_screen:
@@ -111,15 +101,15 @@
     ]
     if _from_screen:
         image_type_id = int(_dict.get("experimental") is not None)
         image = sinara_images[image_type_id][
             int(_dict.get("sinara_image_num")) - 1
         ]
         _dict["image"] = image
-        _dict["project"] = "cv" if "cv" in image else "ml"
+        _dict["serverType"] = "cv" if "cv" in image else "ml"
         del _dict["sinara_image_num"]
     else:
         image = _dict.get("image")
         if image:
             if "exp" in image:
                 _dict["experimental"] = True
 
@@ -131,19 +121,14 @@
 
 def load_from_file(screen, file):
     with open(file) as fd:
         config = json.load(fd)
 
     remap_config(config, False)
 
-    # disabled
-    for key in ["platform", "createFolders"]:
-        if key in config:
-            del config[key]
-
     for child in screen.walk_children():
         if config.get(child.name) is not None:
             if type(child) is RadioSet:
                 child._selected = config[child.name]
                 child.action_toggle_button()
             else:
                 child.value = config[child.name]
```

### Comparing `sinarax-1.1.8/sinaraX/screens/utils/infra.py` & `sinarax-1.1.9/sinaraX/screens/utils/infra.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,28 @@
 import re
 
 import requests
 
 from .process import start_cmd
 
 
+def update_sinara_org():
+    cmd = "sinara org update"
+    failed = False
+    lines = []
+    for line in start_cmd(cmd):
+        lines.append(line)
+        if "failed" in line:
+            failed = True
+
+        if "docker: not found" in line:
+            failed = True
+    return lines, failed
+
+
 def check_docker():
     check_docker_cmd = "docker info -f json"
     lines = []
     failed = False
     for line in start_cmd(check_docker_cmd):
         lines.append(line)
         if "failed" in line:
```

### Comparing `sinarax-1.1.8/sinaraX/screens/utils/process.py` & `sinarax-1.1.9/sinaraX/screens/utils/process.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/sinaraX/screens/utils/sinara_server_utils.py` & `sinarax-1.1.9/sinaraX/screens/utils/sinara_server_utils.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.8/PKG-INFO` & `sinarax-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinaraX
-Version: 1.1.8
+Version: 1.1.9
 Summary: sinaraX - TUI for sinaraml clin
 Keywords: sinaraX,tui,cli,sinaraml,sinara
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: requests
-Requires-Dist: sinaraml (>=2024.3.12)
+Requires-Dist: sinaraml (>=2024.4.23)
 Requires-Dist: textual (>=0.57.1)
 Project-URL: Homepage, https://github.com/MiXaiLL76/sinaraX
 Description-Content-Type: text/markdown
 
 # SinaraX is a TUI for the [sinaraml](https://github.com/4-DS/sinaraml) library
 [![license](https://img.shields.io/github/license/MiXaiLL76/sinaraX.svg)](https://github.com/MiXaiLL76/sinaraX/blob/main/LICENSE)
```

