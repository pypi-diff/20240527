# Comparing `tmp/promptic-0.1.9.tar.gz` & `tmp/promptic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.1.9.tar` & `promptic-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.9/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.9/LICENSE
--rw-r--r--   0        0        0     3040 2024-05-27 18:16:10.001727 promptic-0.1.9/README.md
--rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.9/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 18:15:42.809416 promptic-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 promptic-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.2.0/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3008 2024-05-27 18:40:19.184245 promptic-0.2.0/README.md
+-rw-r--r--   0        0        0     2995 2024-05-27 18:37:01.693673 promptic-0.2.0/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 18:39:06.513288 promptic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 promptic-0.2.0/PKG-INFO
```

### Comparing `promptic-0.1.9/.gitignore` & `promptic-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.1.9/LICENSE` & `promptic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.1.9/README.md` & `promptic-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: promptic
+Version: 0.2.0
+Summary: A simple yet powerful abstraction for litellm and pydantic
+Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: Apache Software License
+Project-URL: Home, https://github.com/knowsuchagency/promptic
+
 # promptic
 
 `promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
 
 ## Installation
 
 ```bash
@@ -9,74 +18,75 @@
 ```
 
 ## Usage
 
 ### Simple Prompt
 
 ```python
-from promptic import promptic
+from promptic import llm
 
-@promptic
+@llm
 def president(year):
     """Who was the President of the United States in {year}?"""
 
 print(president(2000))
 # The President of the United States in 2000 was Bill Clinton until January 20th, when George W. Bush was inaugurated as the 43rd President.
 ```
 
 ### Structured Output with Pydantic
 
 ```python
 from pydantic import BaseModel
-from promptic import promptic
+from promptic import llm
 
 class Capital(BaseModel):
     country: str
     capital: str
 
-@promptic
+@llm
 def capital(country) -> Capital:
     """What's the capital of {country}?"""
 
 print(capital("France"))
 # country='France' capital='Paris'
 ```
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
-from promptic import promptic
+from promptic import llm
 
-@promptic(
+@llm(
     # keyword args are passed to litellm.completion
     stream=True,
     model="claude-3-haiku-20240307",
 )
-def haiku(subject, adjective, verb) -> str:
+def haiku(subject, adjective, verb):
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
 print("".join(haiku("programming", "witty", "delights")))
-# Bugs in the code taunt,
-# Syntax errors abound, yet
-# Caffeine fuels the fix.
+# Bits and bytes abound,
+# Bugs and features intertwine,
+# Code, the poet's rhyme.
 ```
 
 ## Features
 
-- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
+- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic.llm`.
 - **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders within docstrings.
 - **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
 - **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
 - **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
 
 
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
-With its legible and concise codebase, `promptic` is easy to understand and extend. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
+With its legible and concise codebase, `promptic` is reliable easy to understand. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
 
 `promptic` is open-source software licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
 
 [litellm]: https://github.com/BerriAI/litellm
+
```

### Comparing `promptic-0.1.9/promptic.py` & `promptic-0.2.0/promptic.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import wraps
 from typing import Callable
 
 import litellm
 from pydantic import BaseModel
 
 
-def promptic(fn=None, model="gpt-3.5-turbo", **litellm_kwargs):
+def llm(fn=None, model="gpt-3.5-turbo", **litellm_kwargs):
     def decorator(func: Callable):
         @wraps(func)
         def wrapper(*args, **kwargs):
             # Get the function's docstring as the prompt
             prompt_template = func.__doc__
 
             # Get the argument names and values using inspect
@@ -70,7 +70,10 @@
 
     return decorator(fn) if fn else decorator
 
 
 def _stream_response(response):
     for part in response:
         yield part.choices[0].delta.content or ""
+
+
+llm = llm
```

### Comparing `promptic-0.1.9/pyproject.toml` & `promptic-0.2.0/pyproject.toml`

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
-version = "0.1.9"
+version = "0.2.0"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.1.9/PKG-INFO` & `promptic-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: promptic
-Version: 0.1.9
-Summary: A simple yet powerful abstraction for litellm and pydantic
-Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: Apache Software License
-Project-URL: Home, https://github.com/knowsuchagency/promptic
-
 # promptic
 
 `promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
 
 ## Installation
 
 ```bash
@@ -18,75 +9,74 @@
 ```
 
 ## Usage
 
 ### Simple Prompt
 
 ```python
-from promptic import promptic
+from promptic import llm
 
-@promptic
+@llm
 def president(year):
     """Who was the President of the United States in {year}?"""
 
 print(president(2000))
 # The President of the United States in 2000 was Bill Clinton until January 20th, when George W. Bush was inaugurated as the 43rd President.
 ```
 
 ### Structured Output with Pydantic
 
 ```python
 from pydantic import BaseModel
-from promptic import promptic
+from promptic import llm
 
 class Capital(BaseModel):
     country: str
     capital: str
 
-@promptic
+@llm
 def capital(country) -> Capital:
     """What's the capital of {country}?"""
 
 print(capital("France"))
 # country='France' capital='Paris'
 ```
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
-from promptic import promptic
+from promptic import llm
 
-@promptic(
+@llm(
     # keyword args are passed to litellm.completion
     stream=True,
     model="claude-3-haiku-20240307",
 )
-def haiku(subject, adjective, verb) -> str:
+def haiku(subject, adjective, verb):
     """Write a haiku about {subject} that is {adjective} and {verb}."""
 
 print("".join(haiku("programming", "witty", "delights")))
-# Bugs in the code taunt,
-# Syntax errors abound, yet
-# Caffeine fuels the fix.
+# Bits and bytes abound,
+# Bugs and features intertwine,
+# Code, the poet's rhyme.
 ```
 
 ## Features
 
-- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic`.
+- **Decorator-based API**: Easily define prompts using function docstrings and decorate them with `@promptic.llm`.
 - **Argument interpolation**: Automatically interpolate function arguments into the prompt using `{argument_name}` placeholders within docstrings.
 - **Pydantic model support**: Specify the expected output structure using Pydantic models, and `promptic` will ensure the LLM's response conforms to the defined schema.
 - **Streaming support**: Receive LLM responses in real-time by setting `stream=True` when calling the decorated function.
 - **Simplified LLM interaction**: No need to remember the exact shape of the OpenAPI response object or other LLM-specific details. `promptic` abstracts away the complexities, allowing you to focus on defining prompts and receiving structured outputs.
 
 
 ## Why promptic?
 
 `promptic` is designed to be simple, functional, and robust, providing exactly what you need 90% of the time when working with LLMs. It eliminates the need to remember the specific shapes of OpenAPI response objects or other LLM-specific details, allowing you to focus on creating prompts and receiving structured outputs.
 
-With its legible and concise codebase, `promptic` is easy to understand and extend. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
+With its legible and concise codebase, `promptic` is reliable easy to understand. It leverages the power of `litellm` under the hood, ensuring compatibility with a wide range of LLMs.
 
 ## License
 
 `promptic` is open-source software licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
 
 [litellm]: https://github.com/BerriAI/litellm
-
```

