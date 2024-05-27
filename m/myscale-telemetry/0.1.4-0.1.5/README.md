# Comparing `tmp/myscale-telemetry-0.1.4.tar.gz` & `tmp/myscale-telemetry-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myscale-telemetry-0.1.4.tar", last modified: Fri May 24 07:18:04 2024, max compression
+gzip compressed data, was "myscale-telemetry-0.1.5.tar", last modified: Mon May 27 03:58:54 2024, max compression
```

## Comparing `myscale-telemetry-0.1.4.tar` & `myscale-telemetry-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:18:04.944902 myscale-telemetry-0.1.4/
--rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.4/LICENSE
--rw-r--r--   0 xuj        (501) staff       (20)     6681 2024-05-24 07:18:04.944785 myscale-telemetry-0.1.4/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)     6224 2024-05-24 07:18:02.000000 myscale-telemetry-0.1.4/README.md
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:18:04.943773 myscale-telemetry-0.1.4/myscale_telemetry/
--rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-21 05:08:28.000000 myscale-telemetry-0.1.4/myscale_telemetry/__init__.py
--rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-21 05:09:24.000000 myscale-telemetry-0.1.4/myscale_telemetry/consumer.py
--rw-r--r--   0 xuj        (501) staff       (20)    21572 2024-05-24 04:42:34.000000 myscale-telemetry-0.1.4/myscale_telemetry/handler.py
--rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.4/myscale_telemetry/span_data.py
--rw-r--r--   0 xuj        (501) staff       (20)     6557 2024-05-21 05:11:16.000000 myscale-telemetry-0.1.4/myscale_telemetry/task_manager.py
-drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-24 07:18:04.944556 myscale-telemetry-0.1.4/myscale_telemetry.egg-info/
--rw-r--r--   0 xuj        (501) staff       (20)     6681 2024-05-24 07:18:04.000000 myscale-telemetry-0.1.4/myscale_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-24 07:18:04.000000 myscale-telemetry-0.1.4/myscale_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-24 07:18:04.000000 myscale-telemetry-0.1.4/myscale_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 xuj        (501) staff       (20)       85 2024-05-24 07:18:04.000000 myscale-telemetry-0.1.4/myscale_telemetry.egg-info/requires.txt
--rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-24 07:18:04.000000 myscale-telemetry-0.1.4/myscale_telemetry.egg-info/top_level.txt
--rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-24 07:18:04.944942 myscale-telemetry-0.1.4/setup.cfg
--rw-r--r--   0 xuj        (501) staff       (20)      893 2024-05-24 07:18:02.000000 myscale-telemetry-0.1.4/setup.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 03:58:54.595193 myscale-telemetry-0.1.5/
+-rw-r--r--   0 xuj        (501) staff       (20)     1064 2024-05-21 03:32:44.000000 myscale-telemetry-0.1.5/LICENSE
+-rw-r--r--   0 xuj        (501) staff       (20)     6841 2024-05-27 03:58:54.594895 myscale-telemetry-0.1.5/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)     6384 2024-05-27 03:53:11.000000 myscale-telemetry-0.1.5/README.md
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 03:58:54.593755 myscale-telemetry-0.1.5/myscale_telemetry/
+-rw-r--r--   0 xuj        (501) staff       (20)        0 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.5/myscale_telemetry/__init__.py
+-rw-r--r--   0 xuj        (501) staff       (20)     5569 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.5/myscale_telemetry/consumer.py
+-rw-r--r--   0 xuj        (501) staff       (20)    23749 2024-05-27 03:48:32.000000 myscale-telemetry-0.1.5/myscale_telemetry/handler.py
+-rw-r--r--   0 xuj        (501) staff       (20)     3671 2024-05-27 02:39:30.000000 myscale-telemetry-0.1.5/myscale_telemetry/span_data.py
+-rw-r--r--   0 xuj        (501) staff       (20)     6815 2024-05-27 03:50:06.000000 myscale-telemetry-0.1.5/myscale_telemetry/task_manager.py
+drwxr-xr-x   0 xuj        (501) staff       (20)        0 2024-05-27 03:58:54.594602 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/
+-rw-r--r--   0 xuj        (501) staff       (20)     6841 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 xuj        (501) staff       (20)      384 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 xuj        (501) staff       (20)        1 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 xuj        (501) staff       (20)      101 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/requires.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       18 2024-05-27 03:58:54.000000 myscale-telemetry-0.1.5/myscale_telemetry.egg-info/top_level.txt
+-rw-r--r--   0 xuj        (501) staff       (20)       38 2024-05-27 03:58:54.595230 myscale-telemetry-0.1.5/setup.cfg
+-rw-r--r--   0 xuj        (501) staff       (20)      920 2024-05-27 03:54:39.000000 myscale-telemetry-0.1.5/setup.py
```

### Comparing `myscale-telemetry-0.1.4/LICENSE` & `myscale-telemetry-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.4/PKG-INFO` & `myscale-telemetry-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: myscale-telemetry
-Version: 0.1.4
-Summary: Open-source observability for your LLM application.
-Home-page: https://github.com/myscale/myscale-telemetry
-Author: Xu Jing
-Author-email: xuj@myscale.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MyScale Telemetry
 
 The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in [MyScaleDB](https://github.com/myscale/MyScaleDB) or ClickHouse. This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
 
 ## Installation
 
 Install the MyScale Telemetry package using pip:
@@ -98,14 +84,15 @@
 * `threads`: Number of upload threads (default: 1)
 * `max_retries`: Maximum number of upload retries (default: 10)
 * `max_batch_size`: Maximum upload batch size (default: 1000)
 * `max_task_queue_size`: Maximum upload task queue size (default: 10000)
 * `upload_interval`: Upload interval in seconds (default: 0.5)
 * `database_name`: Name of the trace database (default: "otel")
 * `table_name`: Name of the trace table (default: "otel_traces")
+* `force_count_tokens`: Forces the calculation of LLM token usage, useful when OpenAI LLM streaming is enabled and token usage is not returned (default: False)
 
 ## Observability
 
 To display trace data collected through the MyScale Telemetry from the LLM Application runtime easily and clearly, we also provide a [Grafana Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 The dashboard allows users to monitor the status of the LLM Application which is similar to LangSmith, making it easier to debug and improve its performance.
 
 ### Requirements
```

### Comparing `myscale-telemetry-0.1.4/README.md` & `myscale-telemetry-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: myscale-telemetry
+Version: 0.1.5
+Summary: Open-source observability for your LLM application.
+Home-page: https://github.com/myscale/myscale-telemetry
+Author: Xu Jing
+Author-email: xuj@myscale.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MyScale Telemetry
 
 The MyScale Telemetry is a powerful tool designed to enhance the observability of LLM applications by capturing trace data from LangChain-based applications and storing it in [MyScaleDB](https://github.com/myscale/MyScaleDB) or ClickHouse. This enables developers to diagnose issues, optimize performance, and gain deeper insights into their applications' behavior.
 
 ## Installation
 
 Install the MyScale Telemetry package using pip:
@@ -84,14 +98,15 @@
 * `threads`: Number of upload threads (default: 1)
 * `max_retries`: Maximum number of upload retries (default: 10)
 * `max_batch_size`: Maximum upload batch size (default: 1000)
 * `max_task_queue_size`: Maximum upload task queue size (default: 10000)
 * `upload_interval`: Upload interval in seconds (default: 0.5)
 * `database_name`: Name of the trace database (default: "otel")
 * `table_name`: Name of the trace table (default: "otel_traces")
+* `force_count_tokens`: Forces the calculation of LLM token usage, useful when OpenAI LLM streaming is enabled and token usage is not returned (default: False)
 
 ## Observability
 
 To display trace data collected through the MyScale Telemetry from the LLM Application runtime easily and clearly, we also provide a [Grafana Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 The dashboard allows users to monitor the status of the LLM Application which is similar to LangSmith, making it easier to debug and improve its performance.
 
 ### Requirements
```

### Comparing `myscale-telemetry-0.1.4/myscale_telemetry/consumer.py` & `myscale-telemetry-0.1.5/myscale_telemetry/consumer.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.4/myscale_telemetry/handler.py` & `myscale-telemetry-0.1.5/myscale_telemetry/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import datetime
+import tiktoken
 from typing import Any, Dict, List, Union, Optional, Sequence, cast
 from uuid import UUID
 
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain_core.documents import Document
 from langchain_core.messages import (
     AIMessage,
@@ -67,19 +68,20 @@
             prefix_key + "role": message.role,
             prefix_key + "content": cast(str, message.content),
         }
 
     return {}
 
 
-def _extract_resource_attributes(serialized: Dict[str, Any]) -> Dict[str, str]:
+def _extract_resource_attributes(metadata: Dict[str, Any], serialized: Dict[str, Any]) -> Dict[str, str]:
     """Extract resource attributes from serialized data."""
     resource_attributes: Dict[str, str] = {}
 
     flat_dict = flatten_dict(serialized)
+    flat_dict.update(metadata)
     for resource_key, resource_val in flat_dict.items():
         if isinstance(resource_val, str) and resource_val != "":
             resource_attributes.update({resource_key: resource_val})
 
     return resource_attributes
 
 
@@ -109,14 +111,19 @@
         temperature = str(params.get("temperature"))
         span_attributes.update(
             {"model": model, "chat_type": chat_type, "temperature": temperature}
         )
 
     return span_attributes
 
+def num_tokens_from_string(string: str, encoding_name: str = "cl100k_base") -> int:
+    """Returns the number of tokens in a text string."""
+    encoding = tiktoken.get_encoding(encoding_name)
+    num_tokens = len(encoding.encode(string))
+    return num_tokens
 
 class MyScaleCallbackHandler(BaseCallbackHandler):
     """Callback Handler for MyScale.
 
     Parameters:
         myscale_host (Optional[str]): The hostname of the MyScale database.
         myscale_port (Optional[int]): The port of the MyScale database.
@@ -126,14 +133,17 @@
         max_retries (int): The maximum number of retries for uploading data to MyScale.
         max_batch_size (int): The maximum batch size for uploading data to MyScale.
         max_task_queue_size (int): The maximum size of the task queue.
         upload_interval (float): The interval between uploads in seconds.
         database_name (str): The name of the database to use.
         table_name (str): The name of the table to use.
         log_level (int): The logging level.
+        force_count_tokens (bool): Forces the calculation of LLM token usage,
+                                   useful when OpenAI LLM streaming is enabled
+                                   and token usage is not returned.
 
     This handler utilizes callback methods to extract various elements such as
     questions, retrieved documents, prompts, and messages from each callback
     function, and subsequently uploads this data to the MyScale vector database
     for monitoring and evaluating the performance of the LLM application.
     """
 
@@ -147,14 +157,15 @@
         max_retries: int = 10,
         max_batch_size: int = 1000,
         max_task_queue_size: int = 10000,
         upload_interval: float = 0.5,
         database_name: str = "otel",
         table_name: str = "otel_traces",
         log_level: int = logging.INFO,
+        force_count_tokens: bool = False,
     ) -> None:
         """Set up the MyScale client and the TaskManager,
         which is responsible for uploading data to the MyScale vector database."""
         try:
             from clickhouse_connect import get_client
         except ImportError as exc:
             raise ImportError(
@@ -171,14 +182,15 @@
         self.myscale_client = get_client(
             host=self.myscale_host,
             port=self.myscale_port,
             username=self.myscale_username,
             password=self.myscale_password,
         )
 
+        self.force_count_tokens = force_count_tokens
         self._task_manager = TaskManager(
             client=self.myscale_client,
             threads=threads,
             max_retries=max_retries,
             max_batch_size=max_batch_size,
             max_task_queue_size=max_task_queue_size,
             upload_interval=upload_interval,
@@ -229,15 +241,15 @@
                 trace_id=trace_id,
                 span_id=run_id,
                 parent_span_id=parent_run_id,
                 start_time=get_timestamp(),
                 name=name,
                 kind=kind,
                 span_attributes=span_attributes,
-                resource_attributes=_extract_resource_attributes(serialized),
+                resource_attributes=_extract_resource_attributes(metadata, serialized),
             )
 
         except Exception as e:
             self._log.exception("An error occurred in on_chain_start: %s", e)
 
     def on_chain_end(
         self,
@@ -286,24 +298,34 @@
         )
         try:
             if metadata and metadata.get("trace_id"):
                 trace_id = metadata["trace_id"]
             else:
                 trace_id = self._task_manager.get_trace_id()
             name = serialized.get("name", serialized.get("id", ["Unknown"])[-1])
+            span_attributes = _extract_span_attributes(prompts, **kwargs)
+
+            if self.force_count_tokens:
+                prompt_tokens = 0
+                for i in range(len(prompts)):
+                    content_key = "prompts." + str(i) + ".content"
+                    if content_key in span_attributes:
+                        prompt_tokens += num_tokens_from_string(span_attributes[content_key])
+
+                span_attributes["prompt_tokens"] = str(prompt_tokens)
 
             self._task_manager.create_span(
                 trace_id=trace_id,
                 span_id=run_id,
                 parent_span_id=parent_run_id,
                 start_time=get_timestamp(),
                 name=name,
                 kind="llm",
-                span_attributes=_extract_span_attributes(prompts, **kwargs),
-                resource_attributes=_extract_resource_attributes(serialized),
+                span_attributes=span_attributes,
+                resource_attributes=_extract_resource_attributes(metadata, serialized),
             )
         except Exception as e:
             self._log.exception("An error occurred in on_llm_start: %s", e)
 
     def on_llm_end(
         self,
         response: LLMResult,
@@ -314,42 +336,51 @@
     ) -> Any:
         """Run when LLM ends running."""
         self._log.debug(
             "on llm end run_id: %s parent_run_id: %s", run_id, parent_run_id
         )
         try:
             span_attributes: Dict[str, str] = {}
-
             for i, generation in enumerate(response.generations):
                 generation = generation[0]
                 prefix_key = "completions." + str(i) + "."
                 if isinstance(generation, ChatGeneration):
                     span_attributes.update(
                         _convert_message_to_dict(generation.message, prefix_key)
                     )
                 else:
                     span_attributes[f"{prefix_key}content"] = generation.text
 
-            if response.llm_output is not None and isinstance(
-                response.llm_output, Dict
-            ):
-                token_usage = response.llm_output["token_usage"]
-                if token_usage is not None:
-                    span_attributes["prompt_tokens"] = str(token_usage["prompt_tokens"])
-                    span_attributes["total_tokens"] = str(token_usage["total_tokens"])
-                    span_attributes["completion_tokens"] = str(
-                        token_usage["completion_tokens"]
-                    )
+            if self.force_count_tokens:
+                completion_tokens = 0
+                for i in range(len(response.generations)):
+                    content_key = "completions." + str(i) + ".content"
+                    if content_key in span_attributes:
+                        completion_tokens += num_tokens_from_string(span_attributes[content_key])
+
+                span_attributes["completion_tokens"] = str(completion_tokens)
+            else:
+                if response.llm_output is not None and isinstance(
+                        response.llm_output, Dict
+                ):
+                    token_usage = response.llm_output["token_usage"]
+                    if token_usage is not None:
+                        span_attributes["prompt_tokens"] = str(token_usage["prompt_tokens"])
+                        span_attributes["total_tokens"] = str(token_usage["total_tokens"])
+                        span_attributes["completion_tokens"] = str(
+                            token_usage["completion_tokens"]
+                        )
 
             self._task_manager.end_span(
                 span_id=run_id,
                 end_time=get_timestamp(),
                 span_attributes=span_attributes,
                 status_code=STATUS_SUCCESS,
                 status_message="",
+                force_count_tokens=self.force_count_tokens,
             )
 
         except Exception as e:
             self._log.exception("An error occurred in on_llm_end: %s", e)
 
     def on_chat_model_start(
         self,
@@ -369,23 +400,33 @@
         try:
             if metadata and metadata.get("trace_id"):
                 trace_id = metadata["trace_id"]
             else:
                 trace_id = self._task_manager.get_trace_id()
             name = serialized.get("name", serialized.get("id", ["Unknown"])[-1])
 
+            span_attributes = _extract_span_attributes(messages[0], **kwargs)
+            if self.force_count_tokens:
+                prompt_tokens = 0
+                for i in range(len(messages[0])):
+                    content_key = "prompts." + str(i) + ".content"
+                    if content_key in span_attributes:
+                        prompt_tokens += num_tokens_from_string(span_attributes[content_key])
+
+                span_attributes["prompt_tokens"] = str(prompt_tokens)
+
             self._task_manager.create_span(
                 trace_id=trace_id,
                 span_id=run_id,
                 parent_span_id=parent_run_id,
                 start_time=get_timestamp(),
                 name=name,
                 kind="llm",
-                span_attributes=_extract_span_attributes(messages[0], **kwargs),
-                resource_attributes=_extract_resource_attributes(serialized),
+                span_attributes=span_attributes,
+                resource_attributes=_extract_resource_attributes(metadata, serialized),
             )
         except Exception as e:
             self._log.exception("An error occurred in on_chat_model_start: %s", e)
 
     def on_retriever_start(
         self,
         serialized: Dict[str, Any],
@@ -412,15 +453,15 @@
                 trace_id=trace_id,
                 span_id=run_id,
                 parent_span_id=parent_run_id,
                 start_time=get_timestamp(),
                 name=name,
                 kind="retriever",
                 span_attributes={"query": query},
-                resource_attributes=_extract_resource_attributes(serialized),
+                resource_attributes=_extract_resource_attributes(metadata, serialized),
             )
 
         except Exception as e:
             self._log.exception("An error occurred in on_retriever_start: %s", e)
 
     def on_retriever_end(
         self,
@@ -477,15 +518,15 @@
                 trace_id=trace_id,
                 span_id=run_id,
                 parent_span_id=parent_run_id,
                 start_time=get_timestamp(),
                 name=name,
                 kind="tool",
                 span_attributes={"input": input_str},
-                resource_attributes=_extract_resource_attributes(serialized),
+                resource_attributes=_extract_resource_attributes(metadata, serialized),
             )
 
         except Exception as e:
             self._log.exception("An error occurred in on_tool_start: %s", e)
 
     def on_tool_end(
         self,
```

### Comparing `myscale-telemetry-0.1.4/myscale_telemetry/span_data.py` & `myscale-telemetry-0.1.5/myscale_telemetry/span_data.py`

 * *Files identical despite different names*

### Comparing `myscale-telemetry-0.1.4/myscale_telemetry/task_manager.py` & `myscale-telemetry-0.1.5/myscale_telemetry/task_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -138,19 +138,24 @@
     def end_span(
         self,
         span_id: UUID,
         end_time: datetime,
         span_attributes: Dict[str, str],
         status_code: str,
         status_message: Optional[str] = None,
+        force_count_tokens: bool = False,
     ) -> None:
         """End a span and add its data to the queue."""
         if span_id not in self.spans:
             raise ValueError(f"Span with {span_id} id not exists")
 
+        if force_count_tokens:
+            span_attributes["total_tokens"] = str(
+                int(span_attributes.get("completion_tokens", 0)) + int(self.spans[span_id].span_attributes.get("prompt_tokens", 0)))
+
         self.spans[span_id].update(
             end_time, span_attributes, status_code, status_message
         )
         self.__add_span_data(self.spans[span_id].to_list())
         del self.spans[span_id]
 
     def __add_span_data(self, data: List[Any]) -> None:
```

### Comparing `myscale-telemetry-0.1.4/myscale_telemetry.egg-info/PKG-INFO` & `myscale-telemetry-0.1.5/myscale_telemetry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myscale-telemetry
-Version: 0.1.4
+Version: 0.1.5
 Summary: Open-source observability for your LLM application.
 Home-page: https://github.com/myscale/myscale-telemetry
 Author: Xu Jing
 Author-email: xuj@myscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -98,14 +98,15 @@
 * `threads`: Number of upload threads (default: 1)
 * `max_retries`: Maximum number of upload retries (default: 10)
 * `max_batch_size`: Maximum upload batch size (default: 1000)
 * `max_task_queue_size`: Maximum upload task queue size (default: 10000)
 * `upload_interval`: Upload interval in seconds (default: 0.5)
 * `database_name`: Name of the trace database (default: "otel")
 * `table_name`: Name of the trace table (default: "otel_traces")
+* `force_count_tokens`: Forces the calculation of LLM token usage, useful when OpenAI LLM streaming is enabled and token usage is not returned (default: False)
 
 ## Observability
 
 To display trace data collected through the MyScale Telemetry from the LLM Application runtime easily and clearly, we also provide a [Grafana Trace Dashboard](https://github.com/myscale/myscale-telemetry/blob/main/dashboard/grafana_myscale_trace_dashboard.json).
 The dashboard allows users to monitor the status of the LLM Application which is similar to LangSmith, making it easier to debug and improve its performance.
 
 ### Requirements
```

### Comparing `myscale-telemetry-0.1.4/setup.py` & `myscale-telemetry-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="myscale-telemetry",
-    version="0.1.4",
+    version="0.1.5",
     description="Open-source observability for your LLM application.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Xu Jing",
     author_email="xuj@myscale.com",
     url="https://github.com/myscale/myscale-telemetry",
     packages=find_packages(),
     install_requires=[
         "backoff>=2.2.1",
         "langchain>=0.2.0",
         "langchain-community>=0.2.0",
-        "clickhouse-connect>=0.7.8"
+        "clickhouse-connect>=0.7.8",
+        "tiktoken>=0.7.0"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
```

