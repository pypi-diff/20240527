# Comparing `tmp/promptic-0.1.7.tar.gz` & `tmp/promptic-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.1.7.tar` & `promptic-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.7/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.7/LICENSE
--rw-r--r--   0        0        0     3055 2024-05-27 18:04:47.877804 promptic-0.1.7/README.md
--rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.7/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 18:04:54.250289 promptic-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3403 1970-01-01 00:00:00.000000 promptic-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.8/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3054 2024-05-27 18:05:49.080141 promptic-0.1.8/README.md
+-rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.8/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 18:05:59.312850 promptic-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 promptic-0.1.8/PKG-INFO
```

### Comparing `promptic-0.1.7/.gitignore` & `promptic-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.1.7/LICENSE` & `promptic-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.1.7/README.md` & `promptic-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # promptic
 
-`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, with just a few lines of code.
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
```

### Comparing `promptic-0.1.7/promptic.py` & `promptic-0.1.8/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.1.7/pyproject.toml` & `promptic-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 description = "A simple yet powerful abstraction for litellm and pydantic"
 license = {file = "LICENSE"}
 name = "promptic"
 requires = [
   "litellm~=1.38",
   "pydantic~=2.7",
 ]
-version = "0.1.7"
+version = "0.1.8"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.1.7/PKG-INFO` & `promptic-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
 
-`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs, with just a few lines of code.
+`promptic` is a lightweight, decorator-based Python library that simplifies the process of interacting with large language models (LLMs) using [litellm][litellm]. With `promptic`, you can effortlessly create prompts, handle input arguments, and receive structured outputs from LLMs with just a few lines of code.
 
 ## Installation
 
 ```bash
 pip install promptic
 ```
```

