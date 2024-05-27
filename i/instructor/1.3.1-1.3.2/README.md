# Comparing `tmp/instructor-1.3.1.tar.gz` & `tmp/instructor-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.3.1.tar", max compression
+gzip compressed data, was "instructor-1.3.2.tar", max compression
```

## Comparing `instructor-1.3.1.tar` & `instructor-1.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1066 2024-05-23 19:59:00.731766 instructor-1.3.1/LICENSE
--rw-r--r--   0        0        0    11018 2024-05-23 19:59:00.731766 instructor-1.3.1/README.md
--rw-r--r--   0        0        0     1641 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/_types/__init__.py
--rw-r--r--   0        0        0      668 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/cli/cli.py
--rw-r--r--   0        0        0     3865 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/cli/files.py
--rw-r--r--   0        0        0     5441 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/cli/hub.py
--rw-r--r--   0        0        0     8314 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6889 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/cli/usage.py
--rw-r--r--   0        0        0    13312 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/client.py
--rw-r--r--   0        0        0     2581 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2427 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/client_cohere.py
--rw-r--r--   0        0        0      756 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/client_gemini.py
--rw-r--r--   0        0        0     1399 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/client_groq.py
--rw-r--r--   0        0        0     1735 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/client_mistral.py
--rw-r--r--   0        0        0     9579 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2927 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/citation.py
--rw-r--r--   0        0        0     8721 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2168 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2562 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11564 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1879 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4360 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/dsl/validators.py
--rw-r--r--   0        0        0      471 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/exceptions.py
--rw-r--r--   0        0        0     9843 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/function_calls.py
--rw-r--r--   0        0        0      878 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/mode.py
--rw-r--r--   0        0        0     5001 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/patch.py
--rw-r--r--   0        0        0    15906 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/py.typed
--rw-r--r--   0        0        0    10007 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/retry.py
--rw-r--r--   0        0        0     7919 2024-05-23 19:59:00.815766 instructor-1.3.1/instructor/utils.py
--rw-r--r--   0        0        0     2907 2024-05-23 19:59:00.815766 instructor-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    13136 1970-01-01 00:00:00.000000 instructor-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-27 13:50:11.490289 instructor-1.3.2/LICENSE
+-rw-r--r--   0        0        0    11020 2024-05-27 13:50:11.490289 instructor-1.3.2/README.md
+-rw-r--r--   0        0        0     1641 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3865 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/cli/files.py
+-rw-r--r--   0        0        0     5441 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8314 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6889 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/cli/usage.py
+-rw-r--r--   0        0        0    13312 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/client.py
+-rw-r--r--   0        0        0     2581 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2427 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/client_cohere.py
+-rw-r--r--   0        0        0      756 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/client_gemini.py
+-rw-r--r--   0        0        0     1438 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/client_groq.py
+-rw-r--r--   0        0        0     1735 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/client_mistral.py
+-rw-r--r--   0        0        0     9579 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     8721 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2168 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2562 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11564 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1879 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4360 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      471 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/exceptions.py
+-rw-r--r--   0        0        0     9843 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/function_calls.py
+-rw-r--r--   0        0        0      878 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/mode.py
+-rw-r--r--   0        0        0     5001 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/patch.py
+-rw-r--r--   0        0        0    16718 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/py.typed
+-rw-r--r--   0        0        0    10007 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/retry.py
+-rw-r--r--   0        0        0     7919 2024-05-27 13:50:11.574289 instructor-1.3.2/instructor/utils.py
+-rw-r--r--   0        0        0     2907 2024-05-27 13:50:11.578289 instructor-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    13138 1970-01-01 00:00:00.000000 instructor-1.3.2/PKG-INFO
```

### Comparing `instructor-1.3.1/LICENSE` & `instructor-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/README.md` & `instructor-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 )
 ```
 
 ![with_completion](./docs/blog/posts/img/with_completion.png)
 
 ### Streaming Partial Objects: `create_partial`
 
-In order to handle streams, we still support `Iterable[T]` and `Partial[T]` but to simply the type inference, we've added `create_iterable` and `create_partial` methods as well!
+In order to handle streams, we still support `Iterable[T]` and `Partial[T]` but to simplify the type inference, we've added `create_iterable` and `create_partial` methods as well!
 
 ```python
 import openai
 import instructor
 from pydantic import BaseModel
```

### Comparing `instructor-1.3.1/instructor/__init__.py` & `instructor-1.3.2/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/_types/_alias.py` & `instructor-1.3.2/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/cli/cli.py` & `instructor-1.3.2/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/cli/files.py` & `instructor-1.3.2/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/cli/hub.py` & `instructor-1.3.2/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/cli/jobs.py` & `instructor-1.3.2/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/cli/usage.py` & `instructor-1.3.2/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/client.py` & `instructor-1.3.2/instructor/client.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/client_anthropic.py` & `instructor-1.3.2/instructor/client_anthropic.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/client_cohere.py` & `instructor-1.3.2/instructor/client_cohere.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/client_gemini.py` & `instructor-1.3.2/instructor/client_gemini.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/client_groq.py` & `instructor-1.3.2/instructor/client_groq.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 
 
 @overload
 def from_groq(
     client: groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs: Any,
-) -> instructor.Instructor:
+) -> instructor.AsyncInstructor:
     ...
 
 
 def from_groq(
     client: groq.Groq | groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
     **kwargs: Any,
-) -> instructor.Instructor:
+) -> instructor.Instructor | instructor.AsyncInstructor:
     assert mode in {
         instructor.Mode.JSON,
         instructor.Mode.TOOLS,
     }, "Mode be one of {instructor.Mode.JSON, instructor.Mode.TOOLS}"
 
     assert isinstance(
         client, (groq.Groq, groq.AsyncGroq)
@@ -44,14 +44,14 @@
             create=instructor.patch(create=client.chat.completions.create, mode=mode),
             provider=instructor.Provider.GROQ,
             mode=mode,
             **kwargs,
         )
 
     else:
-        return instructor.Instructor(
+        return instructor.AsyncInstructor(
             client=client,
             create=instructor.patch(create=client.chat.completions.create, mode=mode),
             provider=instructor.Provider.GROQ,
             mode=mode,
             **kwargs,
         )
```

### Comparing `instructor-1.3.1/instructor/client_mistral.py` & `instructor-1.3.2/instructor/client_mistral.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/distil.py` & `instructor-1.3.2/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/dsl/citation.py` & `instructor-1.3.2/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/dsl/iterable.py` & `instructor-1.3.2/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/dsl/maybe.py` & `instructor-1.3.2/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/dsl/parallel.py` & `instructor-1.3.2/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/dsl/partial.py` & `instructor-1.3.2/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/dsl/simple_type.py` & `instructor-1.3.2/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/dsl/validators.py` & `instructor-1.3.2/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/function_calls.py` & `instructor-1.3.2/instructor/function_calls.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/mode.py` & `instructor-1.3.2/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/patch.py` & `instructor-1.3.2/instructor/patch.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/process_response.py` & `instructor-1.3.2/instructor/process_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -353,14 +353,17 @@
                         "role": message["role"],
                         "message": message["content"],
                     }
                 )
             new_kwargs["message"] = instruction
             new_kwargs["chat_history"] = chat_history
         elif mode == Mode.GEMINI_JSON:
+            assert (
+                "model" not in new_kwargs
+            ), "Gemini `model` must be set while patching the client, not passed as a parameter to the create method"
             message = dedent(
                 f"""
                 As a genius expert, your task is to understand the content and provide
                 the parsed objects in json that match the following json_schema:\n
 
                 {json.dumps(response_model.model_json_schema(), indent=2)}
 
@@ -382,23 +385,42 @@
                 new_kwargs["messages"][0]["content"] += f"\n\n{message}"
 
             # default to json response type
             new_kwargs["generation_config"] = new_kwargs.get(
                 "generation_config", {}
             ) | {"response_mime_type": "application/json"}
 
+            map_openai_args_to_gemini = {
+                "max_tokens": "max_output_tokens",
+                "temperature": "temperature",
+                "n": "candidate_count",
+                "top_p": "top_p",
+                "stop": "stop_sequences",
+            }
+
+            # update gemini config if any params are set
+            for k, v in map_openai_args_to_gemini.items():
+                val = new_kwargs.pop(k, None)
+                if val == None:
+                    continue
+                new_kwargs["generation_config"][v] = val
+
+            # gemini has a different prompt format and params from other providers
+            new_kwargs["contents"] = transform_to_gemini_prompt(
+                new_kwargs.pop("messages")
+            )
+
             # minimize gemini safety related errors - model is highly prone to false alarms
+            from google.generativeai.types import HarmCategory, HarmBlockThreshold
+
             new_kwargs["safety_settings"] = new_kwargs.get("safety_settings", {}) | {
                 HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_ONLY_HIGH,
                 HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
                 HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_ONLY_HIGH,
             }
-            # gemini has a different prompt format and params from other providers
-            new_kwargs["contents"] = transform_to_gemini_prompt(new_kwargs["messages"])
-            del new_kwargs["messages"]
         else:
             raise ValueError(f"Invalid patch mode: {mode}")
 
     logger.debug(
         f"Instructor Request: {mode.value=}, {response_model=}, {new_kwargs=}",
         extra={
             "mode": mode.value,
```

### Comparing `instructor-1.3.1/instructor/retry.py` & `instructor-1.3.2/instructor/retry.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/instructor/utils.py` & `instructor-1.3.2/instructor/utils.py`

 * *Files identical despite different names*

### Comparing `instructor-1.3.1/pyproject.toml` & `instructor-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instructor"
-version = "1.3.1"
+version = "1.3.2"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
```

### Comparing `instructor-1.3.1/PKG-INFO` & `instructor-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.3.1
+Version: 1.3.2
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -335,15 +335,15 @@
 )
 ```
 
 ![with_completion](./docs/blog/posts/img/with_completion.png)
 
 ### Streaming Partial Objects: `create_partial`
 
-In order to handle streams, we still support `Iterable[T]` and `Partial[T]` but to simply the type inference, we've added `create_iterable` and `create_partial` methods as well!
+In order to handle streams, we still support `Iterable[T]` and `Partial[T]` but to simplify the type inference, we've added `create_iterable` and `create_partial` methods as well!
 
 ```python
 import openai
 import instructor
 from pydantic import BaseModel
```

