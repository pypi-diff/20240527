# Comparing `tmp/jb_manager_bot-0.1.5.tar.gz` & `tmp/jb_manager_bot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jb_manager_bot-0.1.5.tar", max compression
+gzip compressed data, was "jb_manager_bot-0.1.6.tar", max compression
```

## Comparing `jb_manager_bot-0.1.5.tar` & `jb_manager_bot-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       44 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/README.md
--rw-r--r--   0        0        0      277 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/__init__.py
--rw-r--r--   0        0        0     7734 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/abstract_fsm.py
--rw-r--r--   0        0        0     1376 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/data_models.py
--rw-r--r--   0        0        0       89 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/parsers/__init__.py
--rw-r--r--   0        0        0     1641 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/parsers/option_parser/__init__.py
--rw-r--r--   0        0        0     1074 2024-04-01 05:18:18.899539 jb_manager_bot-0.1.5/jb_manager_bot/parsers/option_parser/prompt.txt
--rw-r--r--   0        0        0     4705 2024-04-15 13:11:47.196211 jb_manager_bot-0.1.5/jb_manager_bot/parsers/utils.py
--rw-r--r--   0        0        0      513 2024-04-15 12:04:31.120779 jb_manager_bot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 jb_manager_bot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-17 11:51:20.163794 jb_manager_bot-0.1.6/README.md
+-rw-r--r--   0        0        0      277 2024-05-17 09:54:41.973349 jb_manager_bot-0.1.6/jb_manager_bot/__init__.py
+-rw-r--r--   0        0        0    12032 2024-05-27 06:37:48.091367 jb_manager_bot-0.1.6/jb_manager_bot/abstract_fsm.py
+-rw-r--r--   0        0        0     1376 2024-05-17 09:54:41.973349 jb_manager_bot-0.1.6/jb_manager_bot/data_models.py
+-rw-r--r--   0        0        0      112 2024-05-27 07:20:45.785640 jb_manager_bot-0.1.6/jb_manager_bot/parsers/__init__.py
+-rw-r--r--   0        0        0     3811 2024-05-27 06:37:48.091367 jb_manager_bot-0.1.6/jb_manager_bot/parsers/option_parser/__init__.py
+-rw-r--r--   0        0        0     1074 2024-05-17 09:54:41.973349 jb_manager_bot-0.1.6/jb_manager_bot/parsers/option_parser/prompt.txt
+-rw-r--r--   0        0        0     5080 2024-05-27 06:37:48.091367 jb_manager_bot-0.1.6/jb_manager_bot/parsers/utils.py
+-rw-r--r--   0        0        0      513 2024-05-27 07:27:07.314149 jb_manager_bot-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 jb_manager_bot-0.1.6/PKG-INFO
```

### Comparing `jb_manager_bot-0.1.5/jb_manager_bot/abstract_fsm.py` & `jb_manager_bot-0.1.6/jb_manager_bot/abstract_fsm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Module to define the abstract FSM class.
 """
 
 from abc import ABC
 from typing import Any, Dict, List, Set
 from transitions import Machine
-
+from jb_manager_bot.data_models import (
+    FSMOutput,
+    MessageData,
+    MessageType,
+    OptionsListType,
+)
 from jb_manager_bot.data_models import Status
 
 
 class AbstractFSM(ABC):
     """Abstraction of the FSM class.
     Each use case will have its own FSM class.
     The FSM class will be used to define the states and transitions.
@@ -228,7 +233,146 @@
         fsm.submit_input(user_input)
         fsm.run()
 
         if fsm.status == Status.END:
             fsm.reset()
 
         return fsm._save_state()
+
+    def _add_state(self, state_name):
+        self.states.append(state_name)
+
+    def create_on_enter_input(self, fn_name):
+        def dynamic_fn(self):
+            self.status = Status.WAIT_FOR_ME
+            self.status = Status.WAIT_FOR_USER_INPUT
+
+        dynamic_fn.__name__ = fn_name
+        setattr(self.__class__, fn_name, dynamic_fn)
+
+    def create_on_enter_display(
+        self,
+        fn_name,
+        message,
+        options=None,
+        menu_selector=None,
+        menu_title=None,
+        media_url=None,
+        dest="language",
+    ):
+        if options:
+            type = MessageType.INTERACTIVE
+            options = [
+                OptionsListType(id=str(i + 1), title=option)
+                for i, option in enumerate(options)
+            ]
+        elif media_url:
+            type = MessageType.IMAGE
+        else:
+            type = MessageType.TEXT
+
+        def dynamic_fn(self):
+            self.status = Status.WAIT_FOR_ME
+            self.send_message(
+                FSMOutput(
+                    message_data=MessageData(body=message),
+                    options_list=options,
+                    type=type,
+                    dest=dest,
+                    menu_selector=menu_selector,
+                    menu_title=menu_title,
+                    media_url=media_url,
+                )
+            )
+            self.status = Status.MOVE_FORWARD
+
+        dynamic_fn.__name__ = fn_name
+        setattr(self.__class__, fn_name, dynamic_fn)
+
+    def _add_display_state(self, state_name):
+        if not state_name.endswith("_display"):
+            state_name = f"{state_name}_display"
+        self.states.append(state_name)
+
+    def _add_input_states(self, state_name):
+        self.states.extend(
+            [
+                f"{state_name}_display",
+                f"{state_name}_input",
+                f"{state_name}_logic",
+                f"{state_name}_fail_display",
+            ]
+        )
+
+    def _add_transition(self, source, destination, trigger="next", conditions=None):
+        if conditions:
+            self.transitions.append(
+                {
+                    "source": source,
+                    "dest": destination,
+                    "trigger": trigger,
+                    "conditions": conditions,
+                }
+            )
+        else:
+            self.transitions.append(
+                {"source": source, "dest": destination, "trigger": trigger}
+            )
+
+    def create_display_state(
+        self,
+        source,
+        dest,
+        message,
+        options=None,
+        menu_selector=None,
+        menu_title=None,
+        media_url=None,
+        dest_channel="language",
+        format_variables=None,
+    ):
+        # if format_variables:
+        #     write_variables = {k: self.__class__.variables[k] for k in format_variables}
+        #     message = message.format(write_variables)
+        self._add_display_state(source)
+        self._add_transition(source, dest)
+        self.create_on_enter_display(
+            f"on_enter_{source}",
+            message,
+            options,
+            menu_selector,
+            menu_title,
+            media_url,
+            dest_channel,
+        )
+
+    def create_input_states(
+        self,
+        name,
+        message,
+        success_dest,
+        is_valid=None,
+        options=None,
+        menu_selector=None,
+        menu_title=None,
+        media_url=None,
+        fail_message=None,
+    ):
+        self._add_input_states(name)
+        self._add_transition(f"{name}_display", f"{name}_input")
+        self._add_transition(f"{name}_input", f"{name}_logic")
+        self._add_transition(f"{name}_logic", success_dest, conditions=is_valid)
+        self._add_transition(f"{name}_logic", f"{name}_fail_display")
+        self._add_transition(f"{name}_fail_display", f"{name}_display")
+
+        self.create_on_enter_display(
+            f"on_enter_{name}_display",
+            message,
+            options,
+            menu_selector,
+            menu_title,
+            media_url,
+        )
+
+        self.create_on_enter_input(f"on_enter_{name}_input")
+
+        self.create_on_enter_display(f"on_enter_{name}_fail_display", fail_message)
```

### Comparing `jb_manager_bot-0.1.5/jb_manager_bot/data_models.py` & `jb_manager_bot-0.1.6/jb_manager_bot/data_models.py`

 * *Files identical despite different names*

### Comparing `jb_manager_bot-0.1.5/jb_manager_bot/parsers/option_parser/prompt.txt` & `jb_manager_bot-0.1.6/jb_manager_bot/parsers/option_parser/prompt.txt`

 * *Files identical despite different names*

### Comparing `jb_manager_bot-0.1.5/jb_manager_bot/parsers/utils.py` & `jb_manager_bot-0.1.6/jb_manager_bot/parsers/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import os
 from typing import List
 from openai import OpenAI, AzureOpenAI
 
 
 class LLMManager:
     """Language Model Manager for OpenAI's GPT."""
 
@@ -13,14 +14,15 @@
         cls,
         openai_api_key=None,
         azure_openai_api_key=None,
         azure_openai_api_version=None,
         azure_endpoint=None,
     ):
         """Return the OpenAI client."""
+
         if cls.client is None:
             if azure_openai_api_key is not None:
                 cls.client = AzureOpenAI(
                     api_key=azure_openai_api_key,
                     api_version=azure_openai_api_version,
                     azure_endpoint=azure_endpoint,
                 )
@@ -32,17 +34,24 @@
     def llm(
         cls,
         messages,
         openai_api_key=None,
         azure_openai_api_key=None,
         azure_openai_api_version=None,
         azure_endpoint=None,
-        **kwargs
+        **kwargs,
     ):
         """Use the OpenAI Language Model API to generate a response based on the given messages."""
+        azure_openai_api_key = os.getenv("AZURE_OPENAI_API_KEY", azure_openai_api_key)
+        azure_openai_api_version = os.getenv(
+            "AZURE_OPENAI_API_VERSION", azure_openai_api_version
+        )
+        azure_endpoint = os.getenv("AZURE_OPENAI_API_ENDPOINT", azure_endpoint)
+        openai_api_key = os.getenv("OPENAI_API_KEY", openai_api_key)
+    
         kwargs["model"] = kwargs.get("model")
         kwargs["messages"] = messages
         args = {
             k: v
             for k, v in kwargs.items()
             if k
             in [
@@ -126,15 +135,15 @@
         cls,
         inputs: List[str],
         model: str,
         openai_api_key=None,
         azure_openai_api_key=None,
         azure_openai_api_version=None,
         azure_endpoint=None,
-        **kwargs
+        **kwargs,
     ):
         """Use the OpenAI Embeddings API to generate embeddings for the given inputs."""
         client = cls.get_client(
             openai_api_key=openai_api_key,
             azure_openai_api_key=azure_openai_api_key,
             azure_openai_api_version=azure_openai_api_version,
             azure_endpoint=azure_endpoint,
```

### Comparing `jb_manager_bot-0.1.5/pyproject.toml` & `jb_manager_bot-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jb-manager-bot"
-version = "0.1.5"
+version = "0.1.6"
 description = "Bot for JugalBandi Manager"
 authors = ["Shrey Pandey <shreypandey1509@gmail.com>", "Sameer Segal <sameersegal@gmail.com>", "Atharv Kirtikar <atharv.kirtikar@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^2.6.1"
```

### Comparing `jb_manager_bot-0.1.5/PKG-INFO` & `jb_manager_bot-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jb-manager-bot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Bot for JugalBandi Manager
 Author: Shrey Pandey
 Author-email: shreypandey1509@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

