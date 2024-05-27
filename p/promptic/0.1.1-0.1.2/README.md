# Comparing `tmp/promptic-0.1.1.tar.gz` & `tmp/promptic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.1.1.tar` & `promptic-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.1/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.1/LICENSE
--rw-r--r--   0        0        0     2974 2024-05-27 07:03:11.566431 promptic-0.1.1/README.md
--rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.1/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 07:10:50.809224 promptic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3322 1970-01-01 00:00:00.000000 promptic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.2/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2924 2024-05-27 09:09:25.199551 promptic-0.1.2/README.md
+-rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.2/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 09:09:40.380107 promptic-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 promptic-0.1.2/PKG-INFO
```

### Comparing `promptic-0.1.1/.gitignore` & `promptic-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.1.1/LICENSE` & `promptic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.1.1/README.md` & `promptic-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 # promptic
 
 `promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using `litellm`. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
 
-## Features
-
-- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
-- **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders.
-- **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
-- **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
-- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
-
 ## Installation
 
 ```bash
 pip install promptic
 ```
 
 ## Usage
 
-Here are a few examples of how to use `promptic`:
-
 ### Simple Prompt
 
 ```python
 from promptic import promptic
 
 @promptic
 def us_president(year):
@@ -65,14 +55,23 @@
 
 print("".join(haiku("nature", "beautiful", "inspires")))
 # Vibrant green leaves sway
 # Birds sing melodies of joy
 # Nature's perfect dance
 ```
 
+## Features
+
+- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
+- **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders.
+- **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
+- **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
+- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
+
+
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
 With its legible and concise codebase, `promptic` is easy to understand and extend. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
```

### Comparing `promptic-0.1.1/promptic.py` & `promptic-0.1.2/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.1.1/pyproject.toml` & `promptic-0.1.2/pyproject.toml`

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
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.1.1/PKG-INFO` & `promptic-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
 
 `promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using `litellm`. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
 
-## Features
-
-- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
-- **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders.
-- **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
-- **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
-- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
-
 ## Installation
 
 ```bash
 pip install promptic
 ```
 
 ## Usage
 
-Here are a few examples of how to use `promptic`:
-
 ### Simple Prompt
 
 ```python
 from promptic import promptic
 
 @promptic
 def us_president(year):
@@ -74,14 +64,23 @@
 
 print("".join(haiku("nature", "beautiful", "inspires")))
 # Vibrant green leaves sway
 # Birds sing melodies of joy
 # Nature's perfect dance
 ```
 
+## Features
+
+- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
+- **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders.
+- **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
+- **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
+- **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
+
+
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
 With its legible and concise codebase, `promptic` is easy to understand and extend. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
```

