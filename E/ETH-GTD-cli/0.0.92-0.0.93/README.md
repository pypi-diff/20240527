# Comparing `tmp/eth_gtd_cli-0.0.92.tar.gz` & `tmp/eth_gtd_cli-0.0.93.tar.gz`

## Comparing `eth_gtd_cli-0.0.92.tar` & `eth_gtd_cli-0.0.93.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/deploy.sh
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/pyproject.toml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/deploy.sh
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/pyproject.toml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.93/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.92/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.93/src/ETH_GTD_cli/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             response = super().request(method, url, *args, **kwargs)
         return response
 
 
 client = AuthenticatedClient()
 
 
-def login(token: Annotated[str, typer.Option()] = False):
+def login(token: Annotated[str, typer.Option()] = None):
     if token:
         with TOKEN_FILE.open("w") as token_file:
             token_file.write(f"{{\"cli_token\": \"{token}\"}}")
     else:
         print("Opening browser for authentication...")
         webbrowser.open(API_URL + "/auth/google?state=cli")
```

### Comparing `eth_gtd_cli-0.0.92/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.93/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.92/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.93/src/ETH_GTD_cli/main.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.92/LICENSE` & `eth_gtd_cli-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.92/pyproject.toml` & `eth_gtd_cli-0.0.93/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.92"
+version = "0.0.93"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.92/PKG-INFO` & `eth_gtd_cli-0.0.93/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.92
+Version: 0.0.93
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

