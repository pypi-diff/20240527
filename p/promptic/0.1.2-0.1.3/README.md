# Comparing `tmp/promptic-0.1.2.tar.gz` & `tmp/promptic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.1.2.tar` & `promptic-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.2/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.2/LICENSE
--rw-r--r--   0        0        0     2924 2024-05-27 09:09:25.199551 promptic-0.1.2/README.md
--rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.2/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 09:09:40.380107 promptic-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 promptic-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.3/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3067 2024-05-27 17:57:01.308970 promptic-0.1.3/README.md
+-rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.3/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 17:57:52.379158 promptic-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 promptic-0.1.3/PKG-INFO
```

### Comparing `promptic-0.1.2/.gitignore` & `promptic-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.1.2/LICENSE` & `promptic-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.1.2/README.md` & `promptic-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # promptic
 
-`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using `litellm`. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm](litellm) With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
 
@@ -37,43 +37,46 @@
 def get_capital(country) -> Capital:
     """What's the capital of {country}?"""
 
 print(get_capital("France"))
 # country='France' capital='Paris'
 ```
 
-### Streaming Response
+### Streaming Response (and [litellm](litellm) integration)
 
 ```python
 from promptic import promptic
 
 @promptic(
     # keyword args are passed to litellm.completion
     stream=True,
+    model="claude-3-haiku-20240307",
 )
-def haiku(subject: str, adjective: str, verb: str) -> str:
+def haiku(subject, adjective, verb) -> str:
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
-print("".join(haiku("nature", "beautiful", "inspires")))
-# Vibrant green leaves sway
-# Birds sing melodies of joy
-# Nature's perfect dance
+print("".join(haiku("programming", "witty", "delights")))
+# Bugs in the code taunt,
+# Syntax errors abound, yet
+# Caffeine fuels the fix.
 ```
 
 ## Features
 
 - **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
 - **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders.
 - **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
 - **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
-- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
+- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. Thanks to [litellm](litellm), `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
 
 
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
 With its legible and concise codebase, `promptic` is easy to understand and extend. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
 
 `promptic` is open-source software licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
+
+[litellm]: https://github.com/BerriAI/litellm
```

### Comparing `promptic-0.1.2/promptic.py` & `promptic-0.1.3/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.1.2/pyproject.toml` & `promptic-0.1.3/pyproject.toml`

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
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.1.2/PKG-INFO` & `promptic-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
 
-`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using `litellm`. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm](litellm) With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
 
@@ -46,44 +46,47 @@
 def get_capital(country) -> Capital:
     """What's the capital of {country}?"""
 
 print(get_capital("France"))
 # country='France' capital='Paris'
 ```
 
-### Streaming Response
+### Streaming Response (and [litellm](litellm) integration)
 
 ```python
 from promptic import promptic
 
 @promptic(
     # keyword args are passed to litellm.completion
     stream=True,
+    model="claude-3-haiku-20240307",
 )
-def haiku(subject: str, adjective: str, verb: str) -> str:
+def haiku(subject, adjective, verb) -> str:
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
-print("".join(haiku("nature", "beautiful", "inspires")))
-# Vibrant green leaves sway
-# Birds sing melodies of joy
-# Nature's perfect dance
+print("".join(haiku("programming", "witty", "delights")))
+# Bugs in the code taunt,
+# Syntax errors abound, yet
+# Caffeine fuels the fix.
 ```
 
 ## Features
 
 - **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
 - **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders.
 - **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
 - **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
-- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
+- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. Thanks to [litellm](litellm), `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
 
 
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
 With its legible and concise codebase, `promptic` is easy to understand and extend. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
 
 `promptic` is open-source software licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
 
+[litellm]: https://github.com/BerriAI/litellm
+
```

