# Comparing `tmp/tracing_auto_instrumentation-0.0.3.tar.gz` & `tmp/tracing_auto_instrumentation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracing_auto_instrumentation-0.0.3.tar", last modified: Wed May 22 16:59:13 2024, max compression
+gzip compressed data, was "tracing_auto_instrumentation-0.0.4.tar", last modified: Mon May 27 16:58:03 2024, max compression
```

## Comparing `tracing_auto_instrumentation-0.0.3.tar` & `tracing_auto_instrumentation-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,32 @@
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.018581 tracing_auto_instrumentation-0.0.3/
--rw-r--r--   0 rossdancraig   (501) staff       (20)    11357 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/LICENSE
--rw-r--r--   0 rossdancraig   (501) staff       (20)      527 2024-05-22 16:59:13.018372 tracing_auto_instrumentation-0.0.3/PKG-INFO
--rw-r--r--   0 rossdancraig   (501) staff       (20)      870 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/pyproject.toml
--rw-r--r--   0 rossdancraig   (501) staff       (20)       35 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/requirements.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)       38 2024-05-22 16:59:13.018766 tracing_auto_instrumentation-0.0.3/setup.cfg
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.015218 tracing_auto_instrumentation-0.0.3/src/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.017031 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/
--rw-r--r--   0 rossdancraig   (501) staff       (20)      340 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/__init__.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     7205 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/ibm.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     5495 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/langchain_instrumentor.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     6532 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/llama_index_callback_handler.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)    14532 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/openai.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)      626 2024-05-22 16:58:23.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/wrap_utils.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-05-22 16:59:13.018139 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/
--rw-r--r--   0 rossdancraig   (501) staff       (20)      527 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/PKG-INFO
--rw-r--r--   0 rossdancraig   (501) staff       (20)      617 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/SOURCES.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)        1 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/dependency_links.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)       36 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/requires.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)       29 2024-05-22 16:59:13.000000 tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.233139 tracing_auto_instrumentation-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-27 16:58:03.233139 tracing_auto_instrumentation-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/requirements-ibm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/requirements-langchain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/requirements-llama-index.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/requirements-openai.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:58:03.233139 tracing_auto_instrumentation-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.225139 tracing_auto_instrumentation-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.229138 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.229138 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/ibm/ibm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.229138 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/langchain/langchain_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.229138 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/llama_index/llama_index_callback_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.229138 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14532 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/openai/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-27 16:57:59.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/wrap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:58:03.229138 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-27 16:58:03.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-27 16:58:03.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:58:03.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 16:58:03.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 16:58:03.000000 tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation.egg-info/top_level.txt
```

### Comparing `tracing_auto_instrumentation-0.0.3/LICENSE` & `tracing_auto_instrumentation-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.3/pyproject.toml` & `tracing_auto_instrumentation-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "tracing_auto_instrumentation"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="LastMile AI" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Intended Audience :: Developers",
   "Programming Language :: Python :: 3",
 ]
-dynamic = ["dependencies"]
+dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
+[tool.setuptools.dynamic.optional-dependencies]
+ibm = {file = ["requirements-ibm.txt"]}
+langchain = {file = ["requirements-langchain.txt"]}
+llama-index = {file = ["requirements-llama-index.txt"]}
+openai = {file = ["requirements-openai.txt"]}
+
+
 [project.urls]
 "Homepage" = "https://github.com/lastmile-ai/tracing_auto_instrumentation"
 "Bug Tracker" = "https://github.com/lastmile-ai/tracing_auto_instrumentation/issues"
 
 
 # Black formatting
 [tool.black]
```

### Comparing `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/ibm.py` & `tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/ibm/ibm.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from lastmile_eval.rag.debugger.common.query_trace_types import (
     LLMOutputReceived,
     PromptResolved,
 )
 
 
-from .wrap_utils import (
+from ..wrap_utils import (
     NamedWrapper,
 )
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: type these correctly
```

### Comparing `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/langchain_instrumentor.py` & `tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/langchain/langchain_instrumentor.py`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/llama_index_callback_handler.py` & `tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/llama_index/llama_index_callback_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,35 +2,69 @@
 from time import time_ns
 from typing import Any, Dict, Optional
 
 from llama_index.core.callbacks import CBEventType, EventPayload
 from openinference.instrumentation.llama_index._callback import (
     OpenInferenceTraceCallbackHandler,
     payload_to_semantic_attributes,
-    _is_streaming_response,
-    _flatten,
-    _ResponseGen,
-    _EventData,
+    _is_streaming_response,  # type: ignore
+    _flatten,  # type: ignore
+    _ResponseGen,  # type: ignore
+    _EventData,  # type: ignore
+    # Opinionated params we explicit want to save, see source for full list
+    DOCUMENT_SCORE,
+    EMBEDDING_MODEL_NAME,
+    INPUT_VALUE,
+    LLM_INVOCATION_PARAMETERS,
+    LLM_MODEL_NAME,
+    LLM_PROMPT_TEMPLATE,
+    MESSAGE_FUNCTION_CALL_NAME,
+    OUTPUT_VALUE,
+    RERANKER_MODEL_NAME,
+    RERANKER_OUTPUT_DOCUMENTS,
+    RERANKER_QUERY,
+    RERANKER_TOP_K,
+    RETRIEVAL_DOCUMENTS,
+    TOOL_CALL_FUNCTION_NAME,
+    TOOL_NAME,
+    # # Explicit chose not to do these two because context can be huge and we
+    # # can extract this from both the prompt template template and variables
+    # LLM_INPUT_MESSAGES,
+    # LLM_OUTPUT_MESSAGES,
 )
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry import trace as trace_api
 from opentelemetry import context as context_api
-from opentelemetry.context import _SUPPRESS_INSTRUMENTATION_KEY
-from typing_extensions import TypeAlias
+from opentelemetry.context import _SUPPRESS_INSTRUMENTATION_KEY  # type: ignore
 from lastmile_eval.rag.debugger.tracing import get_lastmile_tracer
 from lastmile_eval.rag.debugger.common.utils import (
     DEFAULT_PROJECT_NAME,
     LASTMILE_SPAN_KIND_KEY_NAME,
 )
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
-_EventId: TypeAlias = str
-_ParentId: TypeAlias = str
+PARAM_SET_SUBSTRING_MATCHES = (
+    DOCUMENT_SCORE,
+    EMBEDDING_MODEL_NAME,
+    INPUT_VALUE,
+    LLM_INVOCATION_PARAMETERS,
+    LLM_MODEL_NAME,
+    LLM_PROMPT_TEMPLATE,
+    MESSAGE_FUNCTION_CALL_NAME,
+    OUTPUT_VALUE,
+    RERANKER_MODEL_NAME,
+    RERANKER_OUTPUT_DOCUMENTS,
+    RERANKER_QUERY,
+    RERANKER_TOP_K,
+    RETRIEVAL_DOCUMENTS,
+    TOOL_CALL_FUNCTION_NAME,
+    TOOL_NAME,
+)
 
 
 class LlamaIndexCallbackHandler(OpenInferenceTraceCallbackHandler):
     """
     This is a callback handler for automatically instrumenting with
     LLamaIndex. Here's how to use it:
 
@@ -152,20 +186,27 @@
             and "serialized" in span._attributes
         ):
             del span._attributes["serialized"]
 
         if not _should_skip(event_type):
             serializable_payload: Dict[str, Any] = {}
             for key, value in span._attributes.items():
-                serializable_payload[key] = value
+                # Only save the opinionated data to event data and param set
+                if _save_to_param_set(key):
+                    serializable_payload[key] = value
             tracer.add_rag_event_for_span(
                 event_name=str(event_data.event_type),
                 span=span,
                 event_data=serializable_payload,
             )
+            tracer.register_params(
+                params=serializable_payload,
+                should_also_save_in_span=False,
+                span=span,
+            )
 
         # Save span kind into span attribute, but don't add it to trace-level
         # params (since that should be for trace-level data) or rag span event
         # (since it's already used for the event name there)
         span.set_attribute(LASTMILE_SPAN_KIND_KEY_NAME, event_data.event_type)
 
     except Exception:
@@ -180,7 +221,14 @@
     # TODO: Add some actual crieria for skipping to log span events
     return event_type in {
         CBEventType.CHUNKING,
         CBEventType.NODE_PARSING,
         CBEventType.TREE,
         CBEventType.SYNTHESIZE,
     }
+
+
+def _save_to_param_set(key: str):
+    for substring in PARAM_SET_SUBSTRING_MATCHES:
+        if substring in key:
+            return True
+    return False
```

### Comparing `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/openai.py` & `tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `tracing_auto_instrumentation-0.0.3/src/tracing_auto_instrumentation/wrap_utils.py` & `tracing_auto_instrumentation-0.0.4/src/tracing_auto_instrumentation/wrap_utils.py`

 * *Files identical despite different names*

