# Comparing `tmp/jaims_py-2.0.0b3.tar.gz` & `tmp/jaims_py-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaims_py-2.0.0b3.tar", last modified: Sun May 19 16:26:32 2024, max compression
+gzip compressed data, was "jaims_py-2.0.0b4.tar", last modified: Sun May 19 16:45:17 2024, max compression
```

## Comparing `jaims_py-2.0.0b3.tar` & `jaims_py-2.0.0b4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.221115 jaims_py-2.0.0b3/
--rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:26:32.220880 jaims_py-2.0.0b3/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)     4692 2024-05-19 16:10:04.000000 jaims_py-2.0.0b3/README.md
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.217547 jaims_py-2.0.0b3/jaims/
--rw-r--r--   0 mush       (501) staff       (20)     1455 2024-05-19 15:19:54.000000 jaims_py-2.0.0b3/jaims/__init__.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.217676 jaims_py-2.0.0b3/jaims/adapters/
--rw-r--r--   0 mush       (501) staff       (20)       74 2024-05-18 20:45:15.000000 jaims_py-2.0.0b3/jaims/adapters/__init__.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.218093 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/
--rw-r--r--   0 mush       (501) staff       (20)      103 2024-05-19 15:10:17.000000 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)     8712 2024-05-19 15:27:59.000000 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/adapter.py
--rw-r--r--   0 mush       (501) staff       (20)     1973 2024-05-19 15:09:20.000000 jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/factory.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.218752 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/
--rw-r--r--   0 mush       (501) staff       (20)      353 2024-05-19 14:46:29.000000 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)    23461 2024-05-19 14:46:37.000000 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/adapter.py
--rw-r--r--   0 mush       (501) staff       (20)     1999 2024-05-19 15:02:51.000000 jaims_py-2.0.0b3/jaims/adapters/openai_adapter/factory.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.219277 jaims_py-2.0.0b3/jaims/adapters/shared/
--rw-r--r--   0 mush       (501) staff       (20)       76 2024-05-19 16:22:55.000000 jaims_py-2.0.0b3/jaims/adapters/shared/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)     2012 2024-05-19 15:30:07.000000 jaims_py-2.0.0b3/jaims/adapters/shared/exponential_backoff_operation.py
--rw-r--r--   0 mush       (501) staff       (20)      709 2024-05-17 18:13:25.000000 jaims_py-2.0.0b3/jaims/adapters/shared/image_utilities.py
--rw-r--r--   0 mush       (501) staff       (20)     7093 2024-05-19 15:42:10.000000 jaims_py-2.0.0b3/jaims/agent.py
--rw-r--r--   0 mush       (501) staff       (20)     1640 2024-05-17 17:46:58.000000 jaims_py-2.0.0b3/jaims/default_history_manager.py
--rw-r--r--   0 mush       (501) staff       (20)     1200 2024-05-15 12:16:49.000000 jaims_py-2.0.0b3/jaims/default_tool_manager.py
--rw-r--r--   0 mush       (501) staff       (20)    14293 2024-05-19 14:44:55.000000 jaims_py-2.0.0b3/jaims/entities.py
--rw-r--r--   0 mush       (501) staff       (20)     2308 2024-05-19 15:13:30.000000 jaims_py-2.0.0b3/jaims/factories.py
--rw-r--r--   0 mush       (501) staff       (20)     1408 2024-05-15 12:13:46.000000 jaims_py-2.0.0b3/jaims/interfaces.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.220375 jaims_py-2.0.0b3/jaims_py.egg-info/
--rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)      840 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/SOURCES.txt
--rw-r--r--   0 mush       (501) staff       (20)        1 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/dependency_links.txt
--rw-r--r--   0 mush       (501) staff       (20)       93 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/requires.txt
--rw-r--r--   0 mush       (501) staff       (20)        6 2024-05-19 16:26:32.000000 jaims_py-2.0.0b3/jaims_py.egg-info/top_level.txt
--rw-r--r--   0 mush       (501) staff       (20)       38 2024-05-19 16:26:32.221155 jaims_py-2.0.0b3/setup.cfg
--rw-r--r--   0 mush       (501) staff       (20)     1015 2024-05-19 16:26:28.000000 jaims_py-2.0.0b3/setup.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:26:32.220212 jaims_py-2.0.0b3/tests/
--rw-r--r--   0 mush       (501) staff       (20)     5042 2024-05-18 19:41:11.000000 jaims_py-2.0.0b3/tests/test_adapters_exponential_backoff.py
--rw-r--r--   0 mush       (501) staff       (20)     3660 2024-05-17 15:46:09.000000 jaims_py-2.0.0b3/tests/test_agent.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.364174 jaims_py-2.0.0b4/
+-rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:45:17.363929 jaims_py-2.0.0b4/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)     4692 2024-05-19 16:10:04.000000 jaims_py-2.0.0b4/README.md
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.359701 jaims_py-2.0.0b4/jaims/
+-rw-r--r--   0 mush       (501) staff       (20)     1455 2024-05-19 15:19:54.000000 jaims_py-2.0.0b4/jaims/__init__.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.359966 jaims_py-2.0.0b4/jaims/adapters/
+-rw-r--r--   0 mush       (501) staff       (20)        0 2024-05-19 16:41:58.000000 jaims_py-2.0.0b4/jaims/adapters/__init__.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.360696 jaims_py-2.0.0b4/jaims/adapters/google_generative_ai_adapter/
+-rw-r--r--   0 mush       (501) staff       (20)      103 2024-05-19 15:10:17.000000 jaims_py-2.0.0b4/jaims/adapters/google_generative_ai_adapter/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)     8712 2024-05-19 15:27:59.000000 jaims_py-2.0.0b4/jaims/adapters/google_generative_ai_adapter/adapter.py
+-rw-r--r--   0 mush       (501) staff       (20)     1973 2024-05-19 15:09:20.000000 jaims_py-2.0.0b4/jaims/adapters/google_generative_ai_adapter/factory.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.361595 jaims_py-2.0.0b4/jaims/adapters/openai_adapter/
+-rw-r--r--   0 mush       (501) staff       (20)      353 2024-05-19 14:46:29.000000 jaims_py-2.0.0b4/jaims/adapters/openai_adapter/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)    23461 2024-05-19 14:46:37.000000 jaims_py-2.0.0b4/jaims/adapters/openai_adapter/adapter.py
+-rw-r--r--   0 mush       (501) staff       (20)     1999 2024-05-19 15:02:51.000000 jaims_py-2.0.0b4/jaims/adapters/openai_adapter/factory.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.362194 jaims_py-2.0.0b4/jaims/adapters/shared/
+-rw-r--r--   0 mush       (501) staff       (20)       76 2024-05-19 16:22:55.000000 jaims_py-2.0.0b4/jaims/adapters/shared/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)     2012 2024-05-19 15:30:07.000000 jaims_py-2.0.0b4/jaims/adapters/shared/exponential_backoff_operation.py
+-rw-r--r--   0 mush       (501) staff       (20)      709 2024-05-17 18:13:25.000000 jaims_py-2.0.0b4/jaims/adapters/shared/image_utilities.py
+-rw-r--r--   0 mush       (501) staff       (20)     7140 2024-05-19 16:41:23.000000 jaims_py-2.0.0b4/jaims/agent.py
+-rw-r--r--   0 mush       (501) staff       (20)     1640 2024-05-17 17:46:58.000000 jaims_py-2.0.0b4/jaims/default_history_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)     1200 2024-05-15 12:16:49.000000 jaims_py-2.0.0b4/jaims/default_tool_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)    14293 2024-05-19 14:44:55.000000 jaims_py-2.0.0b4/jaims/entities.py
+-rw-r--r--   0 mush       (501) staff       (20)     2221 2024-05-19 16:35:59.000000 jaims_py-2.0.0b4/jaims/factories.py
+-rw-r--r--   0 mush       (501) staff       (20)     1408 2024-05-15 12:13:46.000000 jaims_py-2.0.0b4/jaims/interfaces.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.363403 jaims_py-2.0.0b4/jaims_py.egg-info/
+-rw-r--r--   0 mush       (501) staff       (20)     5258 2024-05-19 16:45:17.000000 jaims_py-2.0.0b4/jaims_py.egg-info/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)      840 2024-05-19 16:45:17.000000 jaims_py-2.0.0b4/jaims_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mush       (501) staff       (20)        1 2024-05-19 16:45:17.000000 jaims_py-2.0.0b4/jaims_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mush       (501) staff       (20)       93 2024-05-19 16:45:17.000000 jaims_py-2.0.0b4/jaims_py.egg-info/requires.txt
+-rw-r--r--   0 mush       (501) staff       (20)        6 2024-05-19 16:45:17.000000 jaims_py-2.0.0b4/jaims_py.egg-info/top_level.txt
+-rw-r--r--   0 mush       (501) staff       (20)       38 2024-05-19 16:45:17.364221 jaims_py-2.0.0b4/setup.cfg
+-rw-r--r--   0 mush       (501) staff       (20)     1015 2024-05-19 16:45:14.000000 jaims_py-2.0.0b4/setup.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-05-19 16:45:17.363222 jaims_py-2.0.0b4/tests/
+-rw-r--r--   0 mush       (501) staff       (20)     5042 2024-05-18 19:41:11.000000 jaims_py-2.0.0b4/tests/test_adapters_exponential_backoff.py
+-rw-r--r--   0 mush       (501) staff       (20)     3660 2024-05-17 15:46:09.000000 jaims_py-2.0.0b4/tests/test_agent.py
```

### Comparing `jaims_py-2.0.0b3/PKG-INFO` & `jaims_py-2.0.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: An extensible library to create AI agents using many providers.
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow==10.3.0
```

### Comparing `jaims_py-2.0.0b3/README.md` & `jaims_py-2.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/__init__.py` & `jaims_py-2.0.0b4/jaims/__init__.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/adapter.py` & `jaims_py-2.0.0b4/jaims/adapters/google_generative_ai_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/adapters/google_generative_ai_adapter/factory.py` & `jaims_py-2.0.0b4/jaims/adapters/google_generative_ai_adapter/factory.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/adapters/openai_adapter/adapter.py` & `jaims_py-2.0.0b4/jaims/adapters/openai_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/adapters/openai_adapter/factory.py` & `jaims_py-2.0.0b4/jaims/adapters/openai_adapter/factory.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/adapters/shared/exponential_backoff_operation.py` & `jaims_py-2.0.0b4/jaims/adapters/shared/exponential_backoff_operation.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/adapters/shared/image_utilities.py` & `jaims_py-2.0.0b4/jaims/adapters/shared/image_utilities.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/agent.py` & `jaims_py-2.0.0b4/jaims/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Literal
 
 if TYPE_CHECKING:
     from .interfaces import JAImsLLMInterface, JAImsHistoryManager, JAImsToolManager
 
-from .factories import openai_factory, google_factory
-
 from typing import Generator, List, Optional
 
 
 from jaims.default_tool_manager import JAImsDefaultToolManager
 
 
 from jaims.entities import (
@@ -79,24 +77,28 @@
         # assert provider in ["openai", "google"], "Provider must be either 'openai' or 'google'"
         assert provider in [
             "openai",
             "google",
         ], f"curretnly supported providers are: [openai, google] . If you're targeting an unsupported provider you should supply your own adapter instead."
 
         if provider == "openai":
+            from .factories import openai_factory
+
             return openai_factory(
                 model=model,
                 api_key=api_key,
                 options=options,
                 config=config,
                 history_manager=history_manager,
                 tool_manager=tool_manager,
                 tools=tools,
             )
         elif provider == "google":
+            from .factories import google_factory
+
             return google_factory(
                 model=model,
                 api_key=api_key,
                 options=options,
                 config=config,
                 history_manager=history_manager,
                 tool_manager=tool_manager,
```

### Comparing `jaims_py-2.0.0b3/jaims/default_history_manager.py` & `jaims_py-2.0.0b4/jaims/default_history_manager.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/default_tool_manager.py` & `jaims_py-2.0.0b4/jaims/default_tool_manager.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/entities.py` & `jaims_py-2.0.0b4/jaims/entities.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims/factories.py` & `jaims_py-2.0.0b4/jaims/factories.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     options: Optional[JAImsOptions] = None,
     config: Optional[JAImsLLMConfig] = None,
     history_manager: Optional[JAImsHistoryManager] = None,
     tool_manager: Optional[JAImsToolManager] = None,
     tools: Optional[List[JAImsFunctionTool]] = None,
 ) -> JAImsAgent:
 
-    from jaims.adapters.openai_adapter import create_jaims_openai
-    from jaims.adapters.openai_adapter import JAImsOpenaiKWArgs
+    from .adapters.openai_adapter import create_jaims_openai
+    from .adapters.openai_adapter import JAImsOpenaiKWArgs
 
     config = config or JAImsLLMConfig()
     options = options or JAImsOptions()
 
     kwargs = JAImsOpenaiKWArgs().copy_with_overrides(
         model=model,
         temperature=config.temperature,
@@ -47,17 +47,18 @@
     options: Optional[JAImsOptions] = None,
     config: Optional[JAImsLLMConfig] = None,
     history_manager: Optional[JAImsHistoryManager] = None,
     tool_manager: Optional[JAImsToolManager] = None,
     tools: Optional[List[JAImsFunctionTool]] = None,
 ) -> JAImsAgent:
 
-    from jaims.adapters.google_generative_ai_adapter.factory import create_jaims_gemini
-    from google.generativeai.types import generation_types
-    from google.generativeai.types import content_types
+    from .adapters.google_generative_ai_adapter.factory import (
+        create_jaims_gemini,
+        generation_types,
+    )
 
     config = config or JAImsLLMConfig()
     options = options or JAImsOptions()
 
     generation_config = generation_types.GenerationConfig(
         temperature=config.temperature,
         max_output_tokens=config.max_tokens,
```

### Comparing `jaims_py-2.0.0b3/jaims/interfaces.py` & `jaims_py-2.0.0b4/jaims/interfaces.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/jaims_py.egg-info/PKG-INFO` & `jaims_py-2.0.0b4/jaims_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: An extensible library to create AI agents using many providers.
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow==10.3.0
```

### Comparing `jaims_py-2.0.0b3/jaims_py.egg-info/SOURCES.txt` & `jaims_py-2.0.0b4/jaims_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/setup.py` & `jaims_py-2.0.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Read Google Cloud AI specific requirements
 with open("requirements-googleai.txt") as f:
     requirements_google_ai = f.read().splitlines()
 
 setup(
     name="jaims-py",
-    version="2.0.0-beta.3",
+    version="2.0.0-beta.4",
     packages=find_packages(),
     description="A Python package for creating simple AI Agents using the OpenAI API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Marco Musella",
     url="https://github.com/dev-mush/jaims-py",
     license="MIT",
```

### Comparing `jaims_py-2.0.0b3/tests/test_adapters_exponential_backoff.py` & `jaims_py-2.0.0b4/tests/test_adapters_exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `jaims_py-2.0.0b3/tests/test_agent.py` & `jaims_py-2.0.0b4/tests/test_agent.py`

 * *Files identical despite different names*

