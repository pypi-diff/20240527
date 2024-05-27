# Comparing `tmp/promptic-0.1.3.tar.gz` & `tmp/promptic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.1.3.tar` & `promptic-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.3/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.3/LICENSE
--rw-r--r--   0        0        0     3067 2024-05-27 17:57:01.308970 promptic-0.1.3/README.md
--rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.3/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 17:57:52.379158 promptic-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 promptic-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.4/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3068 2024-05-27 17:58:28.218855 promptic-0.1.4/README.md
+-rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.4/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 17:58:32.882210 promptic-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 promptic-0.1.4/PKG-INFO
```

### Comparing `promptic-0.1.3/.gitignore` & `promptic-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.1.3/LICENSE` & `promptic-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.1.3/README.md` & `promptic-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # promptic
 
-`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm](litellm) With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm](litellm). With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
```

### Comparing `promptic-0.1.3/promptic.py` & `promptic-0.1.4/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.1.3/pyproject.toml` & `promptic-0.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.1.3"
+version = "0.1.4"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.1.3/PKG-INFO` & `promptic-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
 
-`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm](litellm) With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm](litellm). With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, all in under 100 lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
```

