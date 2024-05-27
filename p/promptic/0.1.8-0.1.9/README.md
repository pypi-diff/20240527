# Comparing `tmp/promptic-0.1.8.tar.gz` & `tmp/promptic-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptic-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "promptic-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `promptic-0.1.8.tar` & `promptic-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.8/.gitignore
--rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.8/LICENSE
--rw-r--r--   0        0        0     3054 2024-05-27 18:05:49.080141 promptic-0.1.8/README.md
--rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.8/promptic.py
--rw-r--r--   0        0        0      527 2024-05-27 18:05:59.312850 promptic-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 promptic-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3148 2024-05-27 06:28:17.069394 promptic-0.1.9/.gitignore
+-rw-r--r--   0        0        0     9161 2024-05-26 22:14:04.381236 promptic-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3040 2024-05-27 18:16:10.001727 promptic-0.1.9/README.md
+-rw-r--r--   0        0        0     2988 2024-05-27 06:13:46.769310 promptic-0.1.9/promptic.py
+-rw-r--r--   0        0        0      527 2024-05-27 18:15:42.809416 promptic-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 promptic-0.1.9/PKG-INFO
```

### Comparing `promptic-0.1.8/.gitignore` & `promptic-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `promptic-0.1.8/LICENSE` & `promptic-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `promptic-0.1.8/README.md` & `promptic-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 
 ### Simple Prompt
 
 ```python
 from promptic import promptic
 
 @promptic
-def us_president(year):
+def president(year):
     """Who was the President of the United States in {year}?"""
 
-print(us_president(2000))
+print(president(2000))
 # The President of the United States in 2000 was Bill Clinton until January 20th, when George W. Bush was inaugurated as the 43rd President.
 ```
 
 ### Structured Output with Pydantic
 
 ```python
 from pydantic import BaseModel
 from promptic import promptic
 
 class Capital(BaseModel):
     country: str
     capital: str
 
 @promptic
-def get_capital(country) -> Capital:
+def capital(country) -> Capital:
     """What's the capital of {country}?"""
 
-print(get_capital("France"))
+print(capital("France"))
 # country='France' capital='Paris'
 ```
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
 from promptic import promptic
```

### Comparing `promptic-0.1.8/promptic.py` & `promptic-0.1.9/promptic.py`

 * *Files identical despite different names*

### Comparing `promptic-0.1.8/pyproject.toml` & `promptic-0.1.9/pyproject.toml`

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
-version = "0.1.8"
+version = "0.1.9"
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/knowsuchagency/promptic"
```

### Comparing `promptic-0.1.8/PKG-INFO` & `promptic-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptic
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple yet powerful abstraction for litellm and pydantic
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/knowsuchagency/promptic
 
 # promptic
@@ -21,36 +21,36 @@
 
 ### Simple Prompt
 
 ```python
 from promptic import promptic
 
 @promptic
-def us_president(year):
+def president(year):
     """Who was the President of the United States in {year}?"""
 
-print(us_president(2000))
+print(president(2000))
 # The President of the United States in 2000 was Bill Clinton until January 20th, when George W. Bush was inaugurated as the 43rd President.
 ```
 
 ### Structured Output with Pydantic
 
 ```python
 from pydantic import BaseModel
 from promptic import promptic
 
 class Capital(BaseModel):
     country: str
     capital: str
 
 @promptic
-def get_capital(country) -> Capital:
+def capital(country) -> Capital:
     """What's the capital of {country}?"""
 
-print(get_capital("France"))
+print(capital("France"))
 # country='France' capital='Paris'
 ```
 
 ### Streaming Response (and [litellm][litellm] integration)
 
 ```python
 from promptic import promptic
```

