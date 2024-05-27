# Comparing `tmp/spiceai-0.3.7.tar.gz` & `tmp/spiceai-0.3.8.tar.gz`

## Comparing `spiceai-0.3.7.tar` & `spiceai-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,20 @@
--rw-r--r--   0        0        0    28786 2020-02-02 00:00:00.000000 spiceai-0.3.7/tags
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.7/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.3.7/.ropeproject/globalnames
--rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.3.7/.ropeproject/history
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.7/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.7/scripts/prompt.txt
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.7/scripts/run.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/errors.py
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/models.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/providers.py
--rw-r--r--   0        0        0    35385 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/spice_message.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/utils.py
--rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.7/spice/wrapped_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.7/tests/__init__.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.7/tests/conftest.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 spiceai-0.3.7/tests/test_spice.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.7/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.7/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.8/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.8/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.8/scripts/prompt.txt
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.8/scripts/run.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/errors.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/models.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/providers.py
+-rw-r--r--   0        0        0    36631 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/spice_message.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.8/spice/wrapped_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.8/tests/__init__.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 spiceai-0.3.8/tests/conftest.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 spiceai-0.3.8/tests/test_spice.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.8/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.8/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.8/PKG-INFO
```

### Comparing `spiceai-0.3.7/.github/workflows/ruff.yml` & `spiceai-0.3.8/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/scripts/run.py` & `spiceai-0.3.8/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/spice/errors.py` & `spiceai-0.3.8/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/spice/models.py` & `spiceai-0.3.8/spice/models.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/spice/providers.py` & `spiceai-0.3.8/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/spice/spice.py` & `spiceai-0.3.8/spice/spice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from __future__ import annotations
 
 import dataclasses
 import glob
 import json
 from collections import defaultdict
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from json import JSONDecodeError
 from pathlib import Path
 from timeit import default_timer as timer
-from typing import Any, AsyncIterator, Callable, Collection, Dict, List, Optional, cast
+from typing import Any, AsyncIterator, Callable, Collection, Dict, Generic, List, Optional, TypeVar, Union, cast
 
 import httpx
 from jinja2 import DictLoader, Environment
 from openai.types.chat.completion_create_params import ResponseFormat
 
 from spice.errors import InvalidModelError, UnknownModelError
 from spice.models import EmbeddingModel, Model, TextModel, TranscriptionModel, get_model_from_name
 from spice.providers import Provider, get_provider_from_name
 from spice.spice_message import MessagesEncoder, SpiceMessage
-from spice.utils import embeddings_request_cost, text_request_cost, transcription_request_cost
+from spice.utils import embeddings_request_cost, string_identity, text_request_cost, transcription_request_cost
 from spice.wrapped_clients import WrappedClient
 
 
 @dataclass
 class SpiceCallArgs:
     model: str
     messages: Collection[SpiceMessage]
     stream: bool = False
     temperature: Optional[float] = None
     max_tokens: Optional[int] = None
     response_format: Optional[ResponseFormat] = None
 
 
+T = TypeVar("T")
+
+
 @dataclass
-class SpiceResponse:
+class SpiceResponse(Generic[T]):
     """
     Contains a collection of information about a completed LLM call.
     """
 
     call_args: SpiceCallArgs
     """The call arguments given to the model that created this response."""
 
@@ -56,24 +59,33 @@
 
     completed: bool
     """Whether or not this response was fully completed. This will only ever be false for incomplete streamed responses."""
 
     cost: Optional[float]
     """The cost of this request in cents. May be inaccurate for incompleted streamed responses. Will be None if the cost of the model used is not known."""
 
+    _result: T | None = field(default=None, repr=False)
+    """The result of the LLM call. This will be the same as text if no converter was given."""
+
     @property
     def total_tokens(self) -> int:
         """The total tokens, input and output, in this response."""
         return self.input_tokens + self.output_tokens
 
     @property
     def characters_per_second(self) -> float:
         """The characters per second that the model output. May be inaccurate for streamed responses if not iterated over and completed immediately."""
         return len(self.text) / self.total_time
 
+    @property
+    def result(self) -> T:
+        if self._result is None:
+            return cast(T, self.text)
+        return self._result
+
 
 class StreamingSpiceResponse:
     """
     Returned from a streaming llm call. Can be iterated over asynchronously to retrieve the content.
     """
 
     def __init__(
@@ -365,17 +377,18 @@
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
         response_format: Optional[ResponseFormat] = None,
         name: Optional[str] = None,
         validator: Optional[Callable[[str], bool]] = None,
+        converter: Callable[[str], T] = string_identity,
         streaming_callback: Optional[Callable[[str], None]] = None,
         retries: int = 0,
-    ) -> SpiceResponse:
+    ) -> SpiceResponse[T]:
         """
         Asynchronously retrieves a chat completion response.
 
         Args:
             messages: The list of messages given as context for the completion.
             Will raise an ImageError if any invalid images are given.
 
@@ -393,14 +406,16 @@
             response_format: For valid models, will set the response format to 'text' or 'json'.
             If the provider/model does not support response_format, this argument will be ignored.
 
             name: If given, will be given this name when logged.
 
             validator: If given, will be called with the text of the response. If it returns False, the response will be discarded and another attempt will be made.
 
+            converter: If given, will be called with the text of the response. The result of the converter will be the result of the response. If the converter throws an exception, the response will be discarded and another attempt will be made up to retries times.
+
             streaming_callback: If given, will be called with the text of the response as it is received.
 
             retries: The number of times to retry getting a valid response. If 0, will not retry. If after all retries no valid response is received, will raise a ValueError.
         """
         cost = 0
         for i in range(retries + 1):
             start_time = timer()
@@ -430,24 +445,39 @@
 
             completion_cost = text_request_cost(text_model, input_tokens, output_tokens)
             if completion_cost is not None:
                 cost += completion_cost
                 self._total_cost += completion_cost
 
             end_time = timer()
-            response = SpiceResponse(call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost)
+            if name:
+                retry_name = f"{name}-retry-{i}-fail"
+            else:
+                retry_name = f"retry-{i}-fail"
+
             if validator is not None and not validator(text):
-                if name:
-                    retry_name = f"{name}-retry-{i}-fail"
-                else:
-                    retry_name = f"retry-{i}-fail"
+                response = SpiceResponse(
+                    call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost
+                )
                 self._log_response(response, retry_name)
-            else:
+                continue
+            try:
+                result = converter(text)
+                response = SpiceResponse(
+                    call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost, _result=result
+                )
                 self._log_response(response, name)
                 return response
+            except Exception as e:
+                response = SpiceResponse(
+                    call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost
+                )
+                self._log_response(response, retry_name)
+                continue
+
         raise ValueError("Failed to get a valid response after all retries")
 
     async def stream_response(
         self,
         messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
```

### Comparing `spiceai-0.3.7/spice/spice_message.py` & `spiceai-0.3.8/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/spice/utils.py` & `spiceai-0.3.8/spice/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,7 +22,11 @@
         return (model.input_cost * input_length) / 100
     else:
         return None
 
 
 def print_stream(text: str) -> None:
     print(text, end="", flush=True)
+
+
+def string_identity(x: str) -> str:
+    return x
```

### Comparing `spiceai-0.3.7/spice/wrapped_clients.py` & `spiceai-0.3.8/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/tests/conftest.py` & `spiceai-0.3.8/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     @override
     def process_chunk(self, chunk: ChatCompletionChunk) -> tuple[str, Optional[int], Optional[int]]:
         return chunk.choices[0].delta.content or "", None, None
 
     @override
     def extract_text_and_tokens(self, chat_completion) -> tuple[str, int, int]:
-        return (chat_completion.content[0].text, 0, 0)
+        return (chat_completion.choices[0].message.content, 0, 0)
 
     @override
     async def get_embeddings(self, input_texts: List[str], model: str) -> List[List[float]]:
         raise InvalidModelError()
 
     @override
     def get_embeddings_sync(self, input_texts: List[str], model: str) -> List[List[float]]:
```

### Comparing `spiceai-0.3.7/LICENSE` & `spiceai-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/README.md` & `spiceai-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.7/pyproject.toml` & `spiceai-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.3.7"
+version = "0.3.8"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
```

### Comparing `spiceai-0.3.7/PKG-INFO` & `spiceai-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
```

