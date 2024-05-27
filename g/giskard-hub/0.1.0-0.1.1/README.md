# Comparing `tmp/giskard_hub-0.1.0.tar.gz` & `tmp/giskard_hub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard_hub-0.1.0.tar", max compression
+gzip compressed data, was "giskard_hub-0.1.1.tar", max compression
```

## Comparing `giskard_hub-0.1.0.tar` & `giskard_hub-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-05-27 00:10:04.801724 giskard_hub-0.1.0/LICENSE
--rw-r--r--   0        0        0     5237 2024-05-27 00:10:04.801724 giskard_hub-0.1.0/README.md
--rw-r--r--   0        0        0      800 2024-05-27 00:10:19.625680 giskard_hub-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 00:10:04.801724 giskard_hub-0.1.0/src/giskard_hub/__init__.py
--rw-r--r--   0        0        0     5611 2024-05-27 00:10:04.801724 giskard_hub-0.1.0/src/giskard_hub/cli.py
--rw-r--r--   0        0        0     9894 2024-05-27 00:10:04.801724 giskard_hub-0.1.0/src/giskard_hub/client.py
--rw-r--r--   0        0        0     3900 2024-05-27 00:10:04.801724 giskard_hub-0.1.0/src/giskard_hub/data.py
--rw-r--r--   0        0        0     5703 1970-01-01 00:00:00.000000 giskard_hub-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-27 16:00:50.295335 giskard_hub-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5237 2024-05-27 16:00:50.295335 giskard_hub-0.1.1/README.md
+-rw-r--r--   0        0        0     1282 2024-05-27 16:01:07.259448 giskard_hub-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 16:00:50.295335 giskard_hub-0.1.1/src/giskard_hub/__init__.py
+-rw-r--r--   0        0        0     5663 2024-05-27 16:00:50.295335 giskard_hub-0.1.1/src/giskard_hub/cli.py
+-rw-r--r--   0        0        0     9904 2024-05-27 16:00:50.295335 giskard_hub-0.1.1/src/giskard_hub/client.py
+-rw-r--r--   0        0        0     3900 2024-05-27 16:00:50.295335 giskard_hub-0.1.1/src/giskard_hub/data.py
+-rw-r--r--   0        0        0     6258 1970-01-01 00:00:00.000000 giskard_hub-0.1.1/PKG-INFO
```

### Comparing `giskard_hub-0.1.0/LICENSE` & `giskard_hub-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giskard_hub-0.1.0/README.md` & `giskard_hub-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `giskard_hub-0.1.0/src/giskard_hub/cli.py` & `giskard_hub-0.1.1/src/giskard_hub/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         ),
     ] = None,
     hub_url: Annotated[
         str,
         typer.Option(envvar="GSK_HUB_URL", help="Base url of Hub backend"),
     ] = None,
 ):
-    """Update a started evaluation, to provide agent output to the hub"""
+    """Wait for the results of an execution and output them"""
     client = HubClient(hub_url=hub_url, api_key=api_key)
     print(
         json.dumps(
             [
                 asdict(elt)
                 for elt in client.get_results(
                     execution_id, max_interval=max_interval, interval_time=interval_time
@@ -192,9 +192,11 @@
     ] = None,
 ):
     """List the models in given project on the hub"""
     client = HubClient(hub_url=hub_url, api_key=api_key)
     print(json.dumps([asdict(elt) for elt in client.get_models(project_id=project_id)]))
 
 
+typer_click_object = typer.main.get_group(app)
+
 if __name__ == "__main__":
-    app()
+    typer_click_object()
```

### Comparing `giskard_hub-0.1.0/src/giskard_hub/client.py` & `giskard_hub-0.1.1/src/giskard_hub/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,35 @@
 from dataclasses import asdict
 from pathlib import Path
 from time import sleep
 from typing import List, Optional, Union
 
 import requests
 
-from giskard_hub.data import (Dataset, Evaluation, LLMMessage, Metric, Model,
-                              ModelOutput, Project, TestResult,
-                              TransientEvaluation)
+from giskard_hub.data import (
+    Dataset,
+    Evaluation,
+    LLMMessage,
+    Metric,
+    Model,
+    ModelOutput,
+    Project,
+    TestResult,
+    TransientEvaluation,
+)
 
 
 class HubClient:
     """Client class to handle interaction with the hub."""
 
     # Note(Bazire): This is not async code, because it probably won't be used with async code.
 
-    def __init__(self, hub_url: str, api_key: Optional[str] = None) -> None:
+    def __init__(
+        self, hub_url: Optional[str] = None, api_key: Optional[str] = None
+    ) -> None:
         if hub_url is None:
             hub_url = os.getenv("GSK_HUB_URL")
         if hub_url is None:
             raise ValueError(
                 "Missing Giskard hub url. Please provide it as an argument or with the env variable `GSK_HUB_URL`"
             )
```

### Comparing `giskard_hub-0.1.0/src/giskard_hub/data.py` & `giskard_hub-0.1.1/src/giskard_hub/data.py`

 * *Files identical despite different names*

### Comparing `giskard_hub-0.1.0/PKG-INFO` & `giskard_hub-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: giskard-hub
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: The giskard_hub library allows you to interact with the Giskard Hub, a platform that centralizes the validation process of LLM applications, empowering product teams to ensure all functional, business & legal requirements are met, and keeping them in close contact with the development team to avoid delayed deployment timelines.
+Home-page: https://github.com/Giskard-AI/giskard-hub
 Author: Bazire
 Author-email: bazire@giskard.ai
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.32.2,<3.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
+Project-URL: Documentation, https://docs-hub.giskard.ai/
+Project-URL: Repository, https://github.com/Giskard-AI/giskard-hub
 Description-Content-Type: text/markdown
 
 # Quick Start
 
 ## Evaluating from your Jupyter notebook
 
 Start by initializing a client.
```

