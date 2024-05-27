# Comparing `tmp/fixpoint-0.10.0.tar.gz` & `tmp/fixpoint-0.9.0.tar.gz`

## Comparing `fixpoint-0.10.0.tar` & `fixpoint-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint-0.10.0/.editorconfig
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint-0.10.0/.lintstagedrc.json
--rw-r--r--   0        0        0    21722 2020-02-02 00:00:00.000000 fixpoint-0.10.0/.pylintrc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fixpoint-0.10.0/mypy.ini
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint-0.10.0/pytest.ini
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint-0.10.0/test-requirements.txt
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fixpoint-0.10.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fixpoint-0.10.0/.github/workflows/pypi-release-prod.yml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fixpoint-0.10.0/.github/workflows/pypi-release-test.yml
--rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 fixpoint-0.10.0/bin/pip-freeze
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint-0.10.0/bin/pip-install
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/__init__.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/ab_router.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/direct_logging.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/function_calling.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/main.py
--rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/multi_llm.py
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/router.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 fixpoint-0.10.0/examples/streaming.py
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint-0.10.0/githooks/pre-commit
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/__init__.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/_logging_api.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/_mock_completions.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/client.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/compat.py
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/completions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/__init__.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/_mock_requests.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/debugging.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/env.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/exc.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/iterwrapper.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/logging.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/lib/requests.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/openapi/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/openapi/exceptions.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/types/__init__.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/types/_utils.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 fixpoint-0.10.0/src/fixpoint/types/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/__init__.py
--rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/mock_completions.py
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/test_client.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/test_completions.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/test_types.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/lib/test_iterwrapper.py
--rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/lib/test_requests.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 fixpoint-0.10.0/tests/types/test_openai.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint-0.10.0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint-0.10.0/LICENSE
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 fixpoint-0.10.0/README.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 fixpoint-0.10.0/pyproject.toml
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 fixpoint-0.10.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint-0.9.0/.editorconfig
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint-0.9.0/.lintstagedrc.json
+-rw-r--r--   0        0        0    21722 2020-02-02 00:00:00.000000 fixpoint-0.9.0/.pylintrc
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fixpoint-0.9.0/mypy.ini
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint-0.9.0/pytest.ini
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint-0.9.0/test-requirements.txt
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fixpoint-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fixpoint-0.9.0/.github/workflows/pypi-release-prod.yml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 fixpoint-0.9.0/.github/workflows/pypi-release-test.yml
+-rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 fixpoint-0.9.0/bin/pip-freeze
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint-0.9.0/bin/pip-install
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.9.0/examples/__init__.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fixpoint-0.9.0/examples/direct_logging.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 fixpoint-0.9.0/examples/function_calling.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fixpoint-0.9.0/examples/main.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 fixpoint-0.9.0/examples/multi_llm.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 fixpoint-0.9.0/examples/router.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 fixpoint-0.9.0/examples/streaming.py
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint-0.9.0/githooks/pre-commit
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/_logging_api.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/_mock_completions.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/client.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/compat.py
+-rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/completions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/__init__.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/_mock_requests.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/debugging.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/env.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/exc.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/iterwrapper.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/logging.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/lib/requests.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/openapi/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/openapi/exceptions.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/types/__init__.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/types/_utils.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 fixpoint-0.9.0/src/fixpoint/types/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/mock_completions.py
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/test_client.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/test_completions.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/test_types.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/lib/test_iterwrapper.py
+-rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/lib/test_requests.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 fixpoint-0.9.0/tests/types/test_openai.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 fixpoint-0.9.0/README.md
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 fixpoint-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fixpoint-0.9.0/PKG-INFO
```

### Comparing `fixpoint-0.10.0/.pylintrc` & `fixpoint-0.9.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/mypy.ini` & `fixpoint-0.9.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/.github/workflows/ci.yml` & `fixpoint-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/.github/workflows/pypi-release-prod.yml` & `fixpoint-0.9.0/.github/workflows/pypi-release-prod.yml`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/.github/workflows/pypi-release-test.yml` & `fixpoint-0.9.0/.github/workflows/pypi-release-test.yml`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/bin/pip-freeze` & `fixpoint-0.9.0/bin/pip-freeze`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/examples/ab_router.py` & `fixpoint-0.9.0/examples/multi_llm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,114 @@
 """Example of multi-LLM routing"""
 
 from dataclasses import dataclass
 import os
-import uuid
-from typing import List, Optional
 
 from fixpoint import openapi_client, FixpointClient
 
 
 @dataclass
 class ApiKeys:
     """Various API keys"""
 
     fixpoint: str
+    anthropic: str
     openai: str
 
 
 def main(apikeys: ApiKeys) -> None:
-    """Example of A/B routing
+    """Example of multi-LLM routing
 
-    When you make an A/B routing request, you must specify the experiment ID for
-    your A/B experiment and the user ID that you are routing. For that
-    experiment and user ID, we make sure that they are assigned to one of the
-    arms of the experiment, and every subsequent inference request for that user
-    goes to the same experiment arm.
+    When you make a MultiLLMChatCompletion request, it will make multiple LLM
+    inference requests at once. Your client code will receive the chat
+    completion back for the first model specified, while all subsequent model
+    inference requests occur in the background (aka they do not block your first
+    request from returning).
+
+    All inference requests are logged to Fixpoint, and you can find sibling
+    requests because all siblings will have the same `parent_span_id` set to
+    equal the `span_id` that you passed in on the request. Or if you don't have
+    multiple LLM inference requests in the same trace, you can find all sibling
+    chat completions by filtering to the `trace_id`.
     """
     client = FixpointClient(
         fixpoint_api_key=apikeys.fixpoint,
         openai_api_key=apikeys.openai,
     )
 
-    # This is optional, but it lets you set tracing info on your requests.
-    trace = new_trace(session_id=str(uuid.uuid4()))
+    print("\nWaiting for inference...\n\n")
 
-    # For the same combination of (experiment_id, user_id), we will always route
-    # to the same model arm.
-    experiment_id = "ab_exp_123"
-    user_id = "dylan-000"
-
-    ab_llm_chat_req = openapi_client.V1CreateABChatCompletionRequest(
-        mode=openapi_client.V1Mode.MODE_TEST,
-        experiment_id=experiment_id,
-        user_id=user_id,
-        tracing=trace,
-        # Here you specify the different model arms that are part of your A/B
-        # experiment. You need to pass the API key in for each model arm.
-        models=[
-            openapi_client.V1Model(
-                name="openai/ft:gpt-3.5-turbo-1106:fixpoint::9QJrlP1n",
-                api_key=apikeys.openai,
-            ),
-            openapi_client.V1Model(
-                name="openai/gpt-3.5-turbo-1106", api_key=apikeys.openai
-            ),
-        ],
-        messages=[
-            openapi_client.V1InputMessage(
-                role="user",
-                content="Was Paris always the capital of France?",
-            ),
-        ],
-        # if you want to record additional attributes on the logs, specify them
-        # here
-        log_attributes=[
-            openapi_client.V1LogAttribute(
-                key="prompt-version",
-                value="v0.1.0",
+    multi_completion = client.fixpoint.api.fixpoint_create_multi_llm_chat_completion(
+        openapi_client.V1CreateMultiLLMChatCompletionRequest(
+            mode=openapi_client.V1Mode.MODE_TEST,
+            models=[
+                # This is the model response the Fixpoint API will return to the client
+                openapi_client.V1CreateMultiLLMChatCompletionRequestModel(
+                    name="anthropic/claude-3-sonnet-20240229",
+                    temperature=1.0,
+                    api_key=apikeys.anthropic,
+                    max_tokens=1024,
+                ),
+                # These model chat completion requests will be made in the background
+                openapi_client.V1CreateMultiLLMChatCompletionRequestModel(
+                    name="openai/gpt-3.5-turbo-1106",
+                    temperature=1.8,
+                    api_key=apikeys.openai,
+                ),
+                openapi_client.V1CreateMultiLLMChatCompletionRequestModel(
+                    name="openai/gpt-3.5-turbo-1106",
+                    temperature=0.9,
+                    api_key=apikeys.openai,
+                ),
+            ],
+            messages=[
+                openapi_client.V1InputMessage(
+                    role="system",
+                    content="You are an old curmudgeonly AI. You are helpful, but you don't like being helpful. You are concise.",  # pylint: disable=line-too-long
+                ),
+                openapi_client.V1InputMessage(
+                    role="user", content="How does ChatGPT work?"
+                ),
+            ],
+            # Specify tracing info so that we can correlate these multi-LLM
+            # requests and see what the different base models generated.
+            tracing=openapi_client.V1Tracing(
+                # All children inference requests (one for each model above)
+                # will share this session ID.
+                session_id="27eea3a1-e16e-4643-aa0c-4b0cdb4e826b",
+                # All children inference requests share this trace ID.
+                trace_id="trace_id",
+                # All children inference requests have `parent_span_id` set to this.
+                span_id="46425bf0-6e48-4018-9e34-7539627a09ea",
+                parent_span_id="d6156682-70bd-430b-9701-50c20fc4bf39",
             ),
-        ],
+            user_id="dylan",
+            # You can also attach log attributes to the LLM requests. This can
+            # be useful if you are doing an experiment to try out different LLM
+            # models.
+            log_attributes=[
+                openapi_client.V1LogAttribute(
+                    key="experiment", value="multi-llm-example"
+                )
+            ],
+        )
     )
 
-    print("")
-    print("Making an A/B ChatCompletion request with models:\n")
-    print("\n".join(get_model_info(ab_llm_chat_req)))
-    print("\nUser:", user_id)
-    print("Experiment:", experiment_id)
-    print("\nTracing info:")
-    print(f"Session ID: {trace.session_id}")
-    print(f"Trace ID: {trace.trace_id}")
-    print("")
-    print("\nWaiting for inference...\n\n")
-
-    ab_completion = client.fixpoint.api.fixpoint_create_ab_chat_completion(
-        ab_llm_chat_req
+    completion_id = multi_completion.id
+    external_id = multi_completion.primary_external_id
+    print(
+        f"Made MultiLLMCompletion with ID: {completion_id}, External ID: {external_id}\n"
     )
-
-    completion_id = ab_completion.id
-    # This is the identifier from your inference provider
-    external_id = ab_completion.primary_external_id
-    print("Made AbChatCompletion with:")
-    print(f"ID: {completion_id}")
-    print(f"External ID: {external_id}")
-    print(f"Model: {ab_completion.model.name}\n")
-    choice = ab_completion.completion.choices[0]
+    choice = multi_completion.completion.choices[0]
     role = choice.message.role
     content = choice.message.content
     print(f"{role}: {content}")
 
 
-def new_trace(
-    session_id: str, parent_span_id: Optional[str] = None
-) -> openapi_client.V1Tracing:
-    """Generate a new trace with random IDs."""
-    return openapi_client.V1Tracing(
-        # All children inference requests (one for each model above) will share
-        # this session ID.
-        session_id=session_id,
-        # All children inference requests share this trace ID.
-        trace_id=str(uuid.uuid4()),
-        # All children inference requests have `parent_span_id` set to this.
-        # Aka if the span_id for the CreateMultiLLMChatCompletion request is
-        # "A", then all of the actual inference requests will have
-        # parent_span_ids that are equal to "A", and completely new individual
-        # span IDs.
-        span_id=str(uuid.uuid4()),
-        # If the rest of your app instruments tracing, you can set the parent
-        # span ID here.
-        parent_span_id=parent_span_id,
-    )
-
-
-def get_model_info(
-    req: openapi_client.V1CreateABChatCompletionRequest,
-) -> List[str]:
-    """Return a list of model info strings"""
-    if req.models is None:
-        return []
-    return [f"- {m.name} (temperature {m.temperature})" for m in req.models]
-
-
 if __name__ == "__main__":
     main(
         ApiKeys(
             fixpoint=os.environ["FIXPOINT_API_KEY"],
+            anthropic=os.environ["ANTHROPIC_API_KEY"],
             openai=os.environ["OPENAI_API_KEY"],
         )
     )
```

### Comparing `fixpoint-0.10.0/examples/direct_logging.py` & `fixpoint-0.9.0/examples/direct_logging.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/examples/function_calling.py` & `fixpoint-0.9.0/examples/function_calling.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/examples/main.py` & `fixpoint-0.9.0/examples/main.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/examples/router.py` & `fixpoint-0.9.0/examples/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,27 +48,27 @@
     2. After that, it will try to use gpt-3.5-turbo-0301, until spending $0.0001.
     3. After that, it rejects requests.
     """
     routing_config_req = openapi_client.V1CreateRoutingConfigRequest(
         fallback_strategy=openapi_client.V1FallbackStrategy.FALLBACK_STRATEGY_NEXT,
         terminal_state=openapi_client.V1TerminalState.TERMINAL_STATE_ERROR,
         models=[
-            openapi_client.V1SpendCapModel(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0125",
-                spend_cap=openapi_client.Fixpointv1SpendCap(
+                spend_cap=openapi_client.V1SpendCap(
                     amount="0.0001",
                     currency="USD",
                     reset_interval=openapi_client.V1ResetInterval.RESET_INTERVAL_MONTHLY,
                 ),
             ),
-            openapi_client.V1SpendCapModel(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0301",
-                spend_cap=openapi_client.Fixpointv1SpendCap(
+                spend_cap=openapi_client.V1SpendCap(
                     amount="0.0001",
                     currency="USD",
                     reset_interval=openapi_client.V1ResetInterval.RESET_INTERVAL_MONTHLY,
                 ),
             ),
         ],
         description="This is a test routing config.",
@@ -94,24 +94,24 @@
     1. Tries to use gpt-3.5-turbo-0125 until it has spent $0.0001.
     2. After that, it will use gpt-3.5-turbo-0301, without a spending cap.
     """
     routing_config_req = openapi_client.V1CreateRoutingConfigRequest(
         fallback_strategy=openapi_client.V1FallbackStrategy.FALLBACK_STRATEGY_NEXT,
         terminal_state=openapi_client.V1TerminalState.TERMINAL_STATE_IGNORE_CAP,
         models=[
-            openapi_client.V1SpendCapModel(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0125",
-                spend_cap=openapi_client.Fixpointv1SpendCap(
+                spend_cap=openapi_client.V1SpendCap(
                     amount="0.0001",
                     currency="USD",
                     reset_interval=openapi_client.V1ResetInterval.RESET_INTERVAL_MONTHLY,
                 ),
             ),
-            openapi_client.V1SpendCapModel(
+            openapi_client.Fixpointv1Model(
                 provider="openai",
                 name="gpt-3.5-turbo-0301",
             ),
         ],
         description="This is a test routing config.",
     )
```

### Comparing `fixpoint-0.10.0/examples/streaming.py` & `fixpoint-0.9.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/__init__.py` & `fixpoint-0.9.0/src/fixpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/_logging_api.py` & `fixpoint-0.9.0/src/fixpoint/_logging_api.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/_mock_completions.py` & `fixpoint-0.9.0/src/fixpoint/_mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/client.py` & `fixpoint-0.9.0/src/fixpoint/client.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/compat.py` & `fixpoint-0.9.0/src/fixpoint/compat.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/completions.py` & `fixpoint-0.9.0/src/fixpoint/completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/lib/_mock_requests.py` & `fixpoint-0.9.0/src/fixpoint/lib/_mock_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/lib/debugging.py` & `fixpoint-0.9.0/src/fixpoint/lib/debugging.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/lib/env.py` & `fixpoint-0.9.0/src/fixpoint/lib/env.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/lib/exc.py` & `fixpoint-0.9.0/src/fixpoint/lib/exc.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/lib/iterwrapper.py` & `fixpoint-0.9.0/src/fixpoint/lib/iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/lib/requests.py` & `fixpoint-0.9.0/src/fixpoint/lib/requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/types/__init__.py` & `fixpoint-0.9.0/src/fixpoint/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/types/_utils.py` & `fixpoint-0.9.0/src/fixpoint/types/_utils.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/src/fixpoint/types/openai.py` & `fixpoint-0.9.0/src/fixpoint/types/openai.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/tests/mock_completions.py` & `fixpoint-0.9.0/tests/mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/tests/test_client.py` & `fixpoint-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/tests/test_completions.py` & `fixpoint-0.9.0/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/tests/test_types.py` & `fixpoint-0.9.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/tests/lib/test_iterwrapper.py` & `fixpoint-0.9.0/tests/lib/test_iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/tests/lib/test_requests.py` & `fixpoint-0.9.0/tests/lib/test_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/tests/types/test_openai.py` & `fixpoint-0.9.0/tests/types/test_openai.py`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/LICENSE` & `fixpoint-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/README.md` & `fixpoint-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fixpoint-0.10.0/pyproject.toml` & `fixpoint-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixpoint"
-version = "0.10.0"
+version = "0.9.0"
 
 authors = [
   {name="Fixpoint", email="team@fixpoint.co"},
   { name="Jakub Cichon", email="jakub@fixpoint.co" },
   { name="Dylan Mikus", email="dylan@fixpoint.co" },
 ]
 description = "Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter"
@@ -18,15 +18,15 @@
 
 dependencies = [
   "openai>=1.6.1",
   "requests==2.31.0",
   "python-dateutil>=2.8.2",
   "pydantic>=2",
   "typing-extensions>=4.7.1",
-  "fixpoint-openapi==0.4.0"
+  "fixpoint-openapi==0.3.0"
 ]
 
 [project.optional-dependencies]
 dev = [
   "black>=24",
   "build>=1.1.1",
   "ipdb>=0.13.13",
```

### Comparing `fixpoint-0.10.0/PKG-INFO` & `fixpoint-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: fixpoint
-Version: 0.10.0
+Version: 0.9.0
 Summary: Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter
 Project-URL: Homepage, https://github.com/gofixpoint/python-sdk
 Project-URL: Issues, https://github.com/gofixpoint/python-sdk/issues
 Author-email: Fixpoint <team@fixpoint.co>, Jakub Cichon <jakub@fixpoint.co>, Dylan Mikus <dylan@fixpoint.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: fixpoint-openapi==0.4.0
+Requires-Dist: fixpoint-openapi==0.3.0
 Requires-Dist: openai>=1.6.1
 Requires-Dist: pydantic>=2
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: typing-extensions>=4.7.1
 Provides-Extra: dev
 Requires-Dist: black>=24; extra == 'dev'
```

