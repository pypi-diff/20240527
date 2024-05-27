# Comparing `tmp/promptic-0.3.0.tar.gz` & `tmp/promptic-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.3.0.tar` & `promptic-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.3.0/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.3.0/LICENSE
--rw-r--r--   0        0        0     3008 2024-05-27 18:40:19.184245 promptic-0.3.0/README.md
--rw-r--r--   0        0        0     3005 2024-05-27 18:43:30.373532 promptic-0.3.0/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 18:44:10.964490 promptic-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 promptic-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.3.1/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3017 2024-05-27 18:53:46.313171 promptic-0.3.1/README.md
+-rw-r--r--   0        0        0     3005 2024-05-27 18:43:30.373532 promptic-0.3.1/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 18:53:51.504561 promptic-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 promptic-0.3.1/PKG-INFO
```

### Comparing `promptic-0.3.0/.gitignore` & `promptic-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.3.0/LICENSE` & `promptic-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.3.0/README.md` & `promptic-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,14 @@
 - **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
 
 
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
-With its legible and concise codebase, `promptic` is reliable easy to understand. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
+With its legible and concise codebase, `promptic` is reliable easy to understand. It leverages the power of [litellm][litellm] under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
 
 `promptic` is open-source software licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
 
 [litellm]: https://github.com/BerriAI/litellm
```

### Comparing `promptic-0.3.0/promptic.py` & `promptic-0.3.1/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.3.0/pyproject.toml` & `promptic-0.3.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.3.0"
+version = "0.3.1"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.3.0/PKG-INFO` & `promptic-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
@@ -78,15 +78,15 @@
 - **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
 
 
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
-With its legible and concise codebase, `promptic` is reliable easy to understand. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
+With its legible and concise codebase, `promptic` is reliable easy to understand. It leverages the power of [litellm][litellm] under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
 
 `promptic` is open-source software licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
 
 [litellm]: https://github.com/BerriAI/litellm
```

