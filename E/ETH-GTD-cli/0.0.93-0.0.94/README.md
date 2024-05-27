# Comparing `tmp/eth_gtd_cli-0.0.93.tar.gz` & `tmp/eth_gtd_cli-0.0.94.tar.gz`

## Comparing `eth_gtd_cli-0.0.93.tar` & `eth_gtd_cli-0.0.94.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/deploy.sh
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/pyproject.toml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/deploy.sh
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/pyproject.toml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.93/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.94/src/ETH_GTD_cli/auth.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.93/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.94/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.93/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.94/src/ETH_GTD_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,27 @@
             print(f"* {runs_by_project_uuid[project_uuid][0]['project']['name']}")
             for run in runs:
                 print(f"  - {run['name']}")
 
     except client.HTTPError as e:
         print(f"Failed to fetch runs: {e}")
 
+@runs.command("byUUID")
+def run_by_uuid(
+    uuid: Annotated[str, typer.Argument()],
+):
+    try:
+        url = f"{API_URL}/run/byUUID"
+        response = client.get(url, params={"uuid": uuid})
+        response.raise_for_status()
+        data = response.json()
+        print(f"Run: {data['name']}")
+
+    except client.HTTPError as e:
+        print(f"Failed to fetch runs: {e}")
 
 @topics.command("list")
 def topics(
     file: Annotated[str, typer.Option()] = None,
     full: Annotated[bool, typer.Option()] = False,
 ):
     try:
```

### Comparing `eth_gtd_cli-0.0.93/LICENSE` & `eth_gtd_cli-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.93/pyproject.toml` & `eth_gtd_cli-0.0.94/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.93"
+version = "0.0.94"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.93/PKG-INFO` & `eth_gtd_cli-0.0.94/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.93
+Version: 0.0.94
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

