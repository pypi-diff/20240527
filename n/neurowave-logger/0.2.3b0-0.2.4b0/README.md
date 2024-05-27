# Comparing `tmp/neurowave_logger-0.2.3b0.tar.gz` & `tmp/neurowave_logger-0.2.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurowave_logger-0.2.3b0.tar", max compression
+gzip compressed data, was "neurowave_logger-0.2.4b0.tar", max compression
```

## Comparing `neurowave_logger-0.2.3b0.tar` & `neurowave_logger-0.2.4b0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       62 2024-04-11 06:18:56.858797 neurowave_logger-0.2.3b0/README.md
--rw-r--r--   0        0        0        0 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/__init__.py
--rw-r--r--   0        0        0     7115 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/langchain_tracer.py
--rw-r--r--   0        0        0     4150 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/tracer.py
--rw-r--r--   0        0        0        0 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/utils/__init__.py
--rw-r--r--   0        0        0     4878 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/utils/openai_info.py
--rw-r--r--   0        0        0     1105 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/utils/text_print.py
--rw-r--r--   0        0        0      501 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/pyproject.toml
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 neurowave_logger-0.2.3b0/PKG-INFO
+-rw-r--r--   0        0        0       62 2024-05-27 13:54:30.815010 neurowave_logger-0.2.4b0/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 13:54:30.815010 neurowave_logger-0.2.4b0/nwlogger/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-27 13:54:30.815010 neurowave_logger-0.2.4b0/nwlogger/constants.py
+-rw-r--r--   0        0        0     7253 2024-05-27 13:54:30.819010 neurowave_logger-0.2.4b0/nwlogger/langchain_tracer.py
+-rw-r--r--   0        0        0     4150 2024-05-27 13:54:30.819010 neurowave_logger-0.2.4b0/nwlogger/tracer.py
+-rw-r--r--   0        0        0        0 2024-05-27 13:54:30.819010 neurowave_logger-0.2.4b0/nwlogger/utils/__init__.py
+-rw-r--r--   0        0        0     4878 2024-05-27 13:54:30.819010 neurowave_logger-0.2.4b0/nwlogger/utils/openai_info.py
+-rw-r--r--   0        0        0     1105 2024-05-27 13:54:30.819010 neurowave_logger-0.2.4b0/nwlogger/utils/text_print.py
+-rw-r--r--   0        0        0      501 2024-05-27 13:54:30.819010 neurowave_logger-0.2.4b0/pyproject.toml
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 neurowave_logger-0.2.4b0/PKG-INFO
```

### Comparing `neurowave_logger-0.2.3b0/nwlogger/langchain_tracer.py` & `neurowave_logger-0.2.4b0/nwlogger/langchain_tracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 from langchain_core.tracers.context import register_configure_hook
 from contextvars import ContextVar
 from time import perf_counter
 
 from contextlib import contextmanager
 
 import requests
-from .utils.openai_info import standardize_model_name, get_openai_token_cost_for_model, MODEL_COST_PER_1K_TOKENS
-
-LOG_SERVER_URL = "https://api-dev.neurowave.ai/logs/chats"
+from nwlogger.utils.openai_info import standardize_model_name, get_openai_token_cost_for_model, MODEL_COST_PER_1K_TOKENS
+from nwlogger.constants import LOG_SERVER_URL
 
 class CoevalLogger(BaseCallbackHandler):
     """Callback Handler that writes to a file."""
 
     def __init__(
-        self, session_id: str, **kwargs: Any
+        self, session_id: str, server_url: str = None, **kwargs: Any
     ) -> None:
         """Initialize callback handler."""
 
         self.meta_data = kwargs.get("meta_data", {})
 
         self.session_id = session_id
         self.conversation = {
             "messages": []
         }
-
+        self.server_url =  server_url if server_url else LOG_SERVER_URL
         self.turn_cost = 0
         self.turn_latency = 0
         self.turn_token_usage = 0
         self.model_name = None
 
     def __repr__(self) -> str:
         return self.meta_data
@@ -180,26 +179,26 @@
         self.meta_data.update(meta_data)
 
     def on_submit(self) -> None:
         """
         """
         self.format_final_response_to_submit()
         print(f"logging to server ...")
-        response = requests.post(LOG_SERVER_URL, json=self.meta_data)
+        response = requests.post(self.server_url, json=self.meta_data)
         if not response.ok:
             print(f"Error logging to server: {response.status_code} - {response.text}")
         else:
             print(f"logged to server ...")
         return self.meta_data
 
 coeval_callback_var: ContextVar[Optional[CoevalLogger]] = ContextVar(
     "coeval_callback", default=None
 )
 register_configure_hook(coeval_callback_var, True)
 
 @contextmanager
-def get_coeval_logger(session_id, **kwargs: Any) -> Generator[CoevalLogger, None, None]:
+def get_coeval_logger(session_id, server_url: str = None, **kwargs: Any) -> Generator[CoevalLogger, None, None]:
     # session_id = kwargs.get("session_id")
-    cb = CoevalLogger(session_id=session_id, **kwargs)
+    cb = CoevalLogger(session_id=session_id, server_url= server_url, **kwargs)
     coeval_callback_var.set(cb)
     yield cb
     coeval_callback_var.set(None)
```

### Comparing `neurowave_logger-0.2.3b0/nwlogger/tracer.py` & `neurowave_logger-0.2.4b0/nwlogger/tracer.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.3b0/nwlogger/utils/openai_info.py` & `neurowave_logger-0.2.4b0/nwlogger/utils/openai_info.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.3b0/nwlogger/utils/text_print.py` & `neurowave_logger-0.2.4b0/nwlogger/utils/text_print.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.3b0/PKG-INFO` & `neurowave_logger-0.2.4b0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurowave-logger
-Version: 0.2.3b0
+Version: 0.2.4b0
 Summary: Log agent for Neurowave
 License: MIT
 Author: Neurowave AI
 Author-email: it@neurowave.ai
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

