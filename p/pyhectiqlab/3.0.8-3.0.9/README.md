# Comparing `tmp/pyhectiqlab-3.0.8.tar.gz` & `tmp/pyhectiqlab-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhectiqlab-3.0.8.tar", last modified: Fri May 24 15:19:08 2024, max compression
+gzip compressed data, was "pyhectiqlab-3.0.9.tar", last modified: Fri May 24 19:50:19 2024, max compression
```

## Comparing `pyhectiqlab-3.0.8.tar` & `pyhectiqlab-3.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.607113 pyhectiqlab-3.0.8/pyhectiqlab/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.607113 pyhectiqlab-3.0.8/pyhectiqlab/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.607113 pyhectiqlab-3.0.8/pyhectiqlab/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/pyhectiqlab/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:50:19.653876 pyhectiqlab-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 19:50:19.653876 pyhectiqlab-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:50:19.649876 pyhectiqlab-3.0.9/pyhectiqlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:50:19.649876 pyhectiqlab-3.0.9/pyhectiqlab/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:50:19.653876 pyhectiqlab-3.0.9/pyhectiqlab/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/functional/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:50:19.653876 pyhectiqlab-3.0.9/pyhectiqlab/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyhectiqlab/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:50:19.653876 pyhectiqlab-3.0.9/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 19:50:19.000000 pyhectiqlab-3.0.9/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-24 19:50:19.000000 pyhectiqlab-3.0.9/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:50:19.000000 pyhectiqlab-3.0.9/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 19:50:19.000000 pyhectiqlab-3.0.9/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 19:50:19.000000 pyhectiqlab-3.0.9/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 19:50:19.000000 pyhectiqlab-3.0.9/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:50:19.653876 pyhectiqlab-3.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:50:19.653876 pyhectiqlab-3.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-24 19:50:04.000000 pyhectiqlab-3.0.9/tests/test_run.py
```

### Comparing `pyhectiqlab-3.0.8/PKG-INFO` & `pyhectiqlab-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/artifact.py` & `pyhectiqlab-3.0.9/pyhectiqlab/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,29 +88,29 @@
     @staticmethod
     @online_method
     @functional_alias("download_artifact")
     @clisync.include(wait_response=True)
     def download(
         id: str,
         savepath: str = "./",
-        wait_response: bool = False,
+        wait_response: bool = True,
     ):
         """
         Download an artifact from a run.
 
         Args:
             name (str): Name of the artifact.
             savepath (str): Path to save the file. Default: './'.
             block: Name of the block. If None, the block is determined from the context. Default: None.
         """
         savepath = savepath or "./"
 
         async def composition():
             fields = ["download_url", "num_bytes", "name"]
-            artifact = Client.get(f"/app/artifacts/{id}", wait_response=wait_response, params={"fields": fields})
+            artifact = Client.get(f"/app/artifacts/{id}", wait_response=True, params={"fields": fields})
             if not artifact:
                 return
             os.makedirs(savepath, exist_ok=True)
             await Client.download(
                 url=artifact["download_url"],
                 local_path=os.path.join(savepath, artifact["name"]),
                 num_bytes=artifact["num_bytes"],
```

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/auth.py` & `pyhectiqlab-3.0.9/pyhectiqlab/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/block.py` & `pyhectiqlab-3.0.9/pyhectiqlab/block.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/cli/__init__.py` & `pyhectiqlab-3.0.9/pyhectiqlab/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/cli/auth.py` & `pyhectiqlab-3.0.9/pyhectiqlab/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/client.py` & `pyhectiqlab-3.0.9/pyhectiqlab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             num_bytes (Optional[int], optional): Number of bytes to download. Default: None.
         """
         os.makedirs(os.path.dirname(local_path), exist_ok=True)
         with open(local_path, "wb") as f:
             with tqdm.tqdm(
                 total=num_bytes, unit="iB", unit_scale=True, bar_format="{desc:<5.5}{percentage:3.0f}%|{bar:10}{r_bar}"
             ) as pbar:
-                async with (client or httpx).stream("GET", url) as r:
+                async with (client or httpx.AsyncClient()).stream("GET", url) as r:
                     async for data in r.aiter_bytes():
                         f.write(data)
                         pbar.update(len(data))
         return local_path
 
     @staticmethod
     async def download_many(urls: List[str], local_paths: List[str], num_bytes: List[int]) -> None:
```

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/dataset.py` & `pyhectiqlab-3.0.9/pyhectiqlab/dataset.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/decorators.py` & `pyhectiqlab-3.0.9/pyhectiqlab/decorators.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/logging.py` & `pyhectiqlab-3.0.9/pyhectiqlab/logging.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/metrics.py` & `pyhectiqlab-3.0.9/pyhectiqlab/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/model.py` & `pyhectiqlab-3.0.9/pyhectiqlab/model.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/project.py` & `pyhectiqlab-3.0.9/pyhectiqlab/project.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/run.py` & `pyhectiqlab-3.0.9/pyhectiqlab/run.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/settings/__init__.py` & `pyhectiqlab-3.0.9/pyhectiqlab/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/step.py` & `pyhectiqlab-3.0.9/pyhectiqlab/step.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/tag.py` & `pyhectiqlab-3.0.9/pyhectiqlab/tag.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/utils.py` & `pyhectiqlab-3.0.9/pyhectiqlab/utils.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab/versions.py` & `pyhectiqlab-3.0.9/pyhectiqlab/versions.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab.egg-info/PKG-INFO` & `pyhectiqlab-3.0.9/pyhectiqlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.8/pyhectiqlab.egg-info/SOURCES.txt` & `pyhectiqlab-3.0.9/pyhectiqlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/pyproject.toml` & `pyhectiqlab-3.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 maintainers = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
 name = "pyhectiqlab"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "3.0.8"
+version = "3.0.9"
 
 [project.urls]
 Repository = "https://github.com/HectiqAI/hectiq-lab-revision.git"
 
 [project.entry-points.console_scripts]
 hectiq-lab = "pyhectiqlab.cli:main"
```

### Comparing `pyhectiqlab-3.0.8/tests/test_dataset.py` & `pyhectiqlab-3.0.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/tests/test_model.py` & `pyhectiqlab-3.0.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/tests/test_project.py` & `pyhectiqlab-3.0.9/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.8/tests/test_run.py` & `pyhectiqlab-3.0.9/tests/test_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,18 @@
     import os
 
     with mock_client(Run) as r:
         run = r(rank=1, project="hectiq-ai/test")
         path = os.path.join(os.path.dirname(__file__), "dummy/artifact.txt")
         res = run.add_artifact(path, name="content.txt", wait_response=True)
 
+def test_download_artifact():
+    from pyhectiqlab.functional import download_artifact
+    download_artifact(id="00d1a48e-39a7-4276-80ec-e763f9a6835c")
+    
 def test_run_add_figure():
     run = Run(title=random_uuid(), project="hectiq-ai/test")
     import matplotlib.pyplot as plt
     plt.style.use("dark_background")
     plt.figure(figsize=(3, 3))
     plt.plot([1, 2, 3, 4], [1, 4, 9, 16])
     run.add_figure(plt, name="test-figure", wait_response=True)
```

