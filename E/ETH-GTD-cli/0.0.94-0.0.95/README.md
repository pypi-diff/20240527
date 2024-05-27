# Comparing `tmp/eth_gtd_cli-0.0.94.tar.gz` & `tmp/eth_gtd_cli-0.0.95.tar.gz`

## Comparing `eth_gtd_cli-0.0.94.tar` & `eth_gtd_cli-0.0.95.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/deploy.sh
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/pyproject.toml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.94/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/deploy.sh
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/pyproject.toml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.95/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.94/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.95/src/ETH_GTD_cli/auth.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.94/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.95/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.94/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.95/src/ETH_GTD_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         response = client.get(f"{API_URL}/project")
         response.raise_for_status()
         projects = response.json()
         print("Projects:")
         for project in projects:
             print(f"- {project['name']}")
 
-    except client.HTTPError as e:
+    except httpx.HTTPError as e:
         print(f"Failed to fetch projects: {e}")
 
 
 @runs.command("list")
 def list_runs(
     project: Annotated[str, typer.Option()] = None,
 ):
@@ -119,29 +119,29 @@
 
         print("Runs by Project:")
         for project_uuid, runs in runs_by_project_uuid.items():
             print(f"* {runs_by_project_uuid[project_uuid][0]['project']['name']}")
             for run in runs:
                 print(f"  - {run['name']}")
 
-    except client.HTTPError as e:
+    except httpx.HTTPError as e:
         print(f"Failed to fetch runs: {e}")
 
 @runs.command("byUUID")
 def run_by_uuid(
     uuid: Annotated[str, typer.Argument()],
 ):
     try:
         url = f"{API_URL}/run/byUUID"
         response = client.get(url, params={"uuid": uuid})
         response.raise_for_status()
         data = response.json()
         print(f"Run: {data['name']}")
 
-    except client.HTTPError as e:
+    except httpx.HTTPError as e:
         print(f"Failed to fetch runs: {e}")
 
 @topics.command("list")
 def topics(
     file: Annotated[str, typer.Option()] = None,
     full: Annotated[bool, typer.Option()] = False,
 ):
@@ -161,27 +161,27 @@
                     topic["name"],
                     topic["type"],
                     topic["nrMessages"],
                     f"{topic['frequency']}",
                 )
             print(table)
 
-    except client.HTTPError as e:
+    except httpx.HTTPError as e:
         print(f"Failed")
 
 
 @projects.command("create")
 def create_project(name: Annotated[str, typer.Option()]):
     try:
         url = API_URL + "/project/create"
         response = client.post(url, json={"name": name})
         response.raise_for_status()
         print("Project created")
 
-    except client.HTTPError as e:
+    except httpx.HTTPError as e:
         print(f"Failed to create project: {e}")
 
 
 @app.command("upload")
 def upload(
     path: Annotated[str, typer.Option(prompt=True)],
     project: Annotated[str, typer.Option(prompt=True)],
@@ -234,15 +234,15 @@
         presigned_urls = response_2.json()
         for file in filenames:
             if not file in presigned_urls.keys():
                 print("Could not upload File '" + file + "'. Is the filename unique? ")
         if len(presigned_urls) > 0:
             uploadFiles(presigned_urls, filepaths, 4)
 
-    except client.HTTPError as e:
+    except httpx.HTTPError as e:
         print(e)
 
 
 @queue.command("clear")
 def clear_queue():
     """Clear queue"""
     # Prompt the user for confirmation
```

### Comparing `eth_gtd_cli-0.0.94/LICENSE` & `eth_gtd_cli-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.94/pyproject.toml` & `eth_gtd_cli-0.0.95/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.94"
+version = "0.0.95"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.94/PKG-INFO` & `eth_gtd_cli-0.0.95/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.94
+Version: 0.0.95
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

