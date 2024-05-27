# Comparing `tmp/promptic-0.2.0.tar.gz` & `tmp/promptic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.2.0.tar` & `promptic-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.2.0/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.2.0/LICENSE
--rw-r--r--   0        0        0     3008 2024-05-27 18:40:19.184245 promptic-0.2.0/README.md
--rw-r--r--   0        0        0     2995 2024-05-27 18:37:01.693673 promptic-0.2.0/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 18:39:06.513288 promptic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 promptic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.3.0/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3008 2024-05-27 18:40:19.184245 promptic-0.3.0/README.md
+-rw-r--r--   0        0        0     3005 2024-05-27 18:43:30.373532 promptic-0.3.0/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 18:44:10.964490 promptic-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 promptic-0.3.0/PKG-INFO
```

### Comparing `promptic-0.2.0/.gitignore` & `promptic-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.2.0/LICENSE` & `promptic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.2.0/README.md` & `promptic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `promptic-0.2.0/promptic.py` & `promptic-0.3.0/promptic.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import wraps
 from typing import Callable
 
 import litellm
 from pydantic import BaseModel
 
 
-def llm(fn=None, model="gpt-3.5-turbo", **litellm_kwargs):
+def promptic(fn=None, model="gpt-3.5-turbo", **litellm_kwargs):
     def decorator(func: Callable):
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Get the function's docstring as the prompt
             prompt_template = func.__doc__
 
             # Get the argument names and values using inspect
@@ -72,8 +72,8 @@
 
 
 def _stream_response(response):
     for part in response:
         yield part.choices[0].delta.content or ""
 
 
-llm = llm
+llm = promptic
```

### Comparing `promptic-0.2.0/pyproject.toml` & `promptic-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.2.0/PKG-INFO` & `promptic-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
```

