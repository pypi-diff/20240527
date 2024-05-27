# Comparing `tmp/promptic-0.3.1.tar.gz` & `tmp/promptic-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.3.1.tar` & `promptic-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.3.1/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.3.1/LICENSE
--rw-r--r--   0        0        0     3017 2024-05-27 18:53:46.313171 promptic-0.3.1/README.md
--rw-r--r--   0        0        0     3005 2024-05-27 18:43:30.373532 promptic-0.3.1/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 18:53:51.504561 promptic-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3156 2024-05-27 19:31:43.907511 promptic-0.4.0/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3017 2024-05-27 18:53:46.313171 promptic-0.4.0/README.md
+-rw-r--r--   0        0        0     3665 2024-05-27 19:36:04.684056 promptic-0.4.0/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 19:37:19.722357 promptic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.4.0/PKG-INFO
```

### Comparing `promptic-0.3.1/.gitignore` & `promptic-0.4.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -158,7 +158,8 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 test.py
+.aider*
```

### Comparing `promptic-0.3.1/LICENSE` & `promptic-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.3.1/README.md` & `promptic-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `promptic-0.3.1/pyproject.toml` & `promptic-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.3.1"
+version = "0.4.0"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.3.1/PKG-INFO` & `promptic-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.3.1
+Version: 0.4.0
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
```

