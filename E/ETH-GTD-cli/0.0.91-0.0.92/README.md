# Comparing `tmp/eth_gtd_cli-0.0.91.tar.gz` & `tmp/eth_gtd_cli-0.0.92.tar.gz`

## Comparing `eth_gtd_cli-0.0.91.tar` & `eth_gtd_cli-0.0.92.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/deploy.sh
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/pyproject.toml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.91/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/deploy.sh
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/pyproject.toml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.92/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.91/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.92/src/ETH_GTD_cli/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,15 +62,18 @@
         try:
             self._load_cookies()
         except:
             print("Not authenticated. Please run 'GTD auth login'.")
 
     def _load_cookies(self):
         tokens = get_token()
-        self.cookies.set("authtoken", tokens["access_token"])
+        if "cli_token" in tokens:
+            self.cookies.set("cli_token", tokens["cli_token"])
+        else:
+            self.cookies.set("authtoken", tokens["access_token"])
 
     def refresh_token(self):
         tokens = get_token()
         refresh_token = tokens.get("refresh_token")
         if not refresh_token:
             print("No refresh token found. Please login again.")
             raise Exception("No refresh token found.")
```

### Comparing `eth_gtd_cli-0.0.91/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.92/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.91/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.92/src/ETH_GTD_cli/main.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.91/LICENSE` & `eth_gtd_cli-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.91/pyproject.toml` & `eth_gtd_cli-0.0.92/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.91"
+version = "0.0.92"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.91/PKG-INFO` & `eth_gtd_cli-0.0.92/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.91
+Version: 0.0.92
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

