# Comparing `tmp/promptic-0.4.1.tar.gz` & `tmp/promptic-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.4.1.tar` & `promptic-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3156 2024-05-27 19:31:43.907511 promptic-0.4.1/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.4.1/LICENSE
--rw-r--r--   0        0        0     3017 2024-05-27 18:53:46.313171 promptic-0.4.1/README.md
--rw-r--r--   0        0        0     3766 2024-05-27 19:38:50.417600 promptic-0.4.1/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 19:39:10.372303 promptic-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3156 2024-05-27 19:31:43.907511 promptic-0.4.2/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3017 2024-05-27 18:53:46.313171 promptic-0.4.2/README.md
+-rw-r--r--   0        0        0     3767 2024-05-27 19:39:51.368363 promptic-0.4.2/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 19:40:16.245975 promptic-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.4.2/PKG-INFO
```

### Comparing `promptic-0.4.1/.gitignore` & `promptic-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.4.1/LICENSE` & `promptic-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.4.1/README.md` & `promptic-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `promptic-0.4.1/promptic.py` & `promptic-0.4.2/promptic.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import litellm
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
 
 def promptic(fn=None, model="gpt-3.5-turbo", **litellm_kwargs):
-    logger.debug("{fn = }")
+    logger.debug(f"{fn = }")
     logger.debug(f"{model = }")
     logger.debug(f"{litellm_kwargs = }")
 
     def decorator(func: Callable):
         @wraps(func)
         def wrapper(*args, **kwargs):
             logger.debug(f"{args = }")
```

### Comparing `promptic-0.4.1/pyproject.toml` & `promptic-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.4.1"
+version = "0.4.2"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.4.1/PKG-INFO` & `promptic-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
```

