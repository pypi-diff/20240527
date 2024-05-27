# Comparing `tmp/eth_gtd_cli-0.0.90.tar.gz` & `tmp/eth_gtd_cli-0.0.91.tar.gz`

## Comparing `eth_gtd_cli-0.0.90.tar` & `eth_gtd_cli-0.0.91.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/deploy.sh
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/pyproject.toml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.90/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/deploy.sh
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/pyproject.toml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.90/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.91/src/ETH_GTD_cli/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,16 @@
 
 
 client = AuthenticatedClient()
 
 
 def login(token: Annotated[str, typer.Option()] = False):
     if token:
-        client.cookies.set("clitoken", token)
+        with TOKEN_FILE.open("w") as token_file:
+            token_file.write(f"{{\"cli_token\": \"{token}\"}}")
     else:
         print("Opening browser for authentication...")
         webbrowser.open(API_URL + "/auth/google?state=cli")
 
         print("Waiting for authentication to complete...")
         auth_tokens = get_auth_tokens()
```

### Comparing `eth_gtd_cli-0.0.90/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.91/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.90/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.91/src/ETH_GTD_cli/main.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.90/LICENSE` & `eth_gtd_cli-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.90/pyproject.toml` & `eth_gtd_cli-0.0.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.90"
+version = "0.0.91"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.90/PKG-INFO` & `eth_gtd_cli-0.0.91/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.90
+Version: 0.0.91
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

