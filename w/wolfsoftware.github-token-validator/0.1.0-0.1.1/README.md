# Comparing `tmp/wolfsoftware_github_token_validator-0.1.0.tar.gz` & `tmp/wolfsoftware_github_token_validator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolfsoftware_github_token_validator-0.1.0.tar", last modified: Sat May 25 19:29:49 2024, max compression
+gzip compressed data, was "wolfsoftware_github_token_validator-0.1.1.tar", last modified: Mon May 27 10:38:20 2024, max compression
```

## Comparing `wolfsoftware_github_token_validator-0.1.0.tar` & `wolfsoftware_github_token_validator-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:29:49.369892 wolfsoftware_github_token_validator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-25 19:29:49.369892 wolfsoftware_github_token_validator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-25 19:29:49.369892 wolfsoftware_github_token_validator-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:29:49.365893 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:29:49.369892 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-25 19:29:41.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:29:49.369892 wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-25 19:29:49.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-25 19:29:49.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:29:49.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 19:29:49.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-25 19:29:49.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 19:29:49.000000 wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:38:20.964352 wolfsoftware_github_token_validator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-27 10:38:20.964352 wolfsoftware_github_token_validator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-27 10:38:20.964352 wolfsoftware_github_token_validator-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:38:20.960352 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:38:20.964352 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-27 10:38:12.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:38:20.964352 wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-27 10:38:20.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-27 10:38:20.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:38:20.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 10:38:20.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 10:38:20.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 10:38:20.000000 wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/top_level.txt
```

### Comparing `wolfsoftware_github_token_validator-0.1.0/LICENSE.md` & `wolfsoftware_github_token_validator-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wolfsoftware_github_token_validator-0.1.0/PKG-INFO` & `wolfsoftware_github_token_validator-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfsoftware.github-token-validator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to validate GitHub Tokens
 Home-page: https://github.com/GitHubToolbox/github-token-validator
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 Project-URL:  Source, https://github.com/GitHubToolbox/github-token-validator
 Project-URL:  Tracker, https://github.com/GitHubToolbox/github-token-validator/issues/
 Project-URL:  Documentation, https://github.com/GitHubToolbox/github-token-validator
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wolfsoftware.github-token-validator Version: 0.1.0
+Metadata-Version: 2.1 Name: wolfsoftware.github-token-validator Version: 0.1.1
 Summary: A tool to validate GitHub Tokens Home-page: https://github.com/
 GitHubToolbox/github-token-validator Author: Wolf Software Author-email:
 pypi@wolfsoftware.com Project-URL: Source, https://github.com/GitHubToolbox/
 github-token-validator Project-URL: Tracker, https://github.com/GitHubToolbox/
 github-token-validator/issues/ Project-URL: Documentation, https://github.com/
 GitHubToolbox/github-token-validator Project-URL: Sponsor, https://github.com/
 sponsors/WolfSoftware Classifier: Environment :: Console Classifier: Intended
```

### Comparing `wolfsoftware_github_token_validator-0.1.0/README.md` & `wolfsoftware_github_token_validator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wolfsoftware_github_token_validator-0.1.0/setup.cfg` & `wolfsoftware_github_token_validator-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wolfsoftware_github_token_validator-0.1.0/setup.py` & `wolfsoftware_github_token_validator-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     required: list[str] = f.read().splitlines()
 
 with open("README.md", 'r', encoding='UTF-8') as f:
     long_description: str = f.read()
 
 setup(
     name='wolfsoftware.github-token-validator',
-    version='0.1.0',
+    version='0.1.1',
     packages=['wolfsoftware.github_token_validator'],
     entry_points={
         'console_scripts': [
             'gtv=wolfsoftware.github_token_validator.main:main',
         ],
     },
     author='Wolf Software',
```

### Comparing `wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/cli.py` & `wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/cli.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/config.py` & `wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/config.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/globals.py` & `wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/globals.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/main.py` & `wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/main.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_github_token_validator-0.1.0/wolfsoftware/github_token_validator/token.py` & `wolfsoftware_github_token_validator-0.1.1/wolfsoftware/github_token_validator/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     headers: Dict[str, str] = {'Authorization': f'token {config.token}'}
 
     try:
         response: requests.Response = requests.get(user_url, headers=headers, timeout=config.timeout)
         response.raise_for_status()
 
         if response.status_code == 200:
+            user: Any = response.json()
+            json_data['owner'] = user['login']
             json_data['scopes'] = response.headers.get("X-OAuth-Scopes")
             json_data['rate_limit_limit'] = response.headers.get("X-RateLimit-Limit")
             json_data['rate_limit_remaining'] = response.headers.get("X-RateLimit-Remaining")
             json_data['rate_limit_used'] = response.headers.get("X-RateLimit-Used")
 
             rate_limit_reset: Optional[str] = response.headers.get("X-RateLimit-Reset")
 
@@ -98,14 +100,15 @@
 
     Arguments:
         data (Any): Dictionary containing token information to be displayed.
     """
     table = PrettyTable()
 
     table.field_names = ["Name", "Value"]
+    table.add_row(["Token Owner", data['owner']])
     table.add_row(["Token Scope", data['scopes']])
     table.add_row(["Rate Limit", data['rate_limit_limit']])
     table.add_row(["Rate Limit Used", data['rate_limit_used']])
     table.add_row(["Rate Limit Remaining", data['rate_limit_remaining']])
     table.add_row(["Time Till Reset", data['time_till_reset']])
 
     table.align["Name"] = "l"
```

### Comparing `wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/PKG-INFO` & `wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfsoftware.github-token-validator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool to validate GitHub Tokens
 Home-page: https://github.com/GitHubToolbox/github-token-validator
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 Project-URL:  Source, https://github.com/GitHubToolbox/github-token-validator
 Project-URL:  Tracker, https://github.com/GitHubToolbox/github-token-validator/issues/
 Project-URL:  Documentation, https://github.com/GitHubToolbox/github-token-validator
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wolfsoftware.github-token-validator Version: 0.1.0
+Metadata-Version: 2.1 Name: wolfsoftware.github-token-validator Version: 0.1.1
 Summary: A tool to validate GitHub Tokens Home-page: https://github.com/
 GitHubToolbox/github-token-validator Author: Wolf Software Author-email:
 pypi@wolfsoftware.com Project-URL: Source, https://github.com/GitHubToolbox/
 github-token-validator Project-URL: Tracker, https://github.com/GitHubToolbox/
 github-token-validator/issues/ Project-URL: Documentation, https://github.com/
 GitHubToolbox/github-token-validator Project-URL: Sponsor, https://github.com/
 sponsors/WolfSoftware Classifier: Environment :: Console Classifier: Intended
```

### Comparing `wolfsoftware_github_token_validator-0.1.0/wolfsoftware.github_token_validator.egg-info/SOURCES.txt` & `wolfsoftware_github_token_validator-0.1.1/wolfsoftware.github_token_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

