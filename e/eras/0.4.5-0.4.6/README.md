# Comparing `tmp/eras-0.4.5.tar.gz` & `tmp/eras-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.4.5.tar", last modified: Sun May 26 03:46:36 2024, max compression
+gzip compressed data, was "eras-0.4.6.tar", last modified: Sun May 26 03:49:41 2024, max compression
```

## Comparing `eras-0.4.5.tar` & `eras-0.4.6.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.655073 eras-0.4.5/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.5/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.5/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:46:36.654518 eras-0.4.5/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.5/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.623187 eras-0.4.5/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.5/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.626584 eras-0.4.5/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.5/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.5/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.5/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.628878 eras-0.4.5/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.5/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.631694 eras-0.4.5/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.5/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.5/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.5/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.5/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.5/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.5/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.5/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.632261 eras-0.4.5/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.5/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.633554 eras-0.4.5/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.5/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.5/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.5/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.5/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.634262 eras-0.4.5/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.5/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.635305 eras-0.4.5/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.5/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.636757 eras-0.4.5/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.5/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.639034 eras-0.4.5/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.5/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.5/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.5/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.5/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.641916 eras-0.4.5/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.5/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.645757 eras-0.4.5/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.5/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.5/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.5/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.5/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.5/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.5/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.5/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.5/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.5/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.5/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.5/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.5/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.5/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.5/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.5/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.5/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.647103 eras-0.4.5/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.5/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.649213 eras-0.4.5/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.5/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.5/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7795 2024-05-26 03:46:21.000000 eras-0.4.5/eras/services/__pycache__/user_config_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.650674 eras-0.4.5/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.5/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.652447 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.5/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.5/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.5/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.5/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.5/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)    10761 2024-05-26 03:46:18.000000 eras-0.4.5/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.653134 eras-0.4.5/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.5/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.653854 eras-0.4.5/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.5/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.5/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.5/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.625510 eras-0.4.5/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)      102 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:46:36.655175 eras-0.4.5/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1093 2024-05-26 03:46:30.000000 eras-0.4.5/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.224416 eras-0.4.6/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.6/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.6/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:49:41.223845 eras-0.4.6/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.6/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.193261 eras-0.4.6/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.6/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.195542 eras-0.4.6/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.6/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.6/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.6/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.197445 eras-0.4.6/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.6/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.201115 eras-0.4.6/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.6/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.6/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.6/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.6/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.6/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.6/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.6/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.201923 eras-0.4.6/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.6/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.203126 eras-0.4.6/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.6/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.6/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.6/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.6/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.203732 eras-0.4.6/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.6/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.204434 eras-0.4.6/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.6/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.205381 eras-0.4.6/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.6/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.207369 eras-0.4.6/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.6/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.6/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.6/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.6/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.210399 eras-0.4.6/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.6/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.214741 eras-0.4.6/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.6/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.6/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.6/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.6/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.6/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.6/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.6/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.6/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.6/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.6/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.6/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.6/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.6/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.6/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.6/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.6/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.216284 eras-0.4.6/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.6/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.217747 eras-0.4.6/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.6/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.6/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7795 2024-05-26 03:46:21.000000 eras-0.4.6/eras/services/__pycache__/user_config_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.219398 eras-0.4.6/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.6/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.221845 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.6/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.6/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.6/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.6/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.6/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)    10789 2024-05-26 03:49:06.000000 eras-0.4.6/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.222456 eras-0.4.6/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.6/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.223168 eras-0.4.6/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.6/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.6/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.6/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.194827 eras-0.4.6/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)      102 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:49:41.224527 eras-0.4.6/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1093 2024-05-26 03:49:37.000000 eras-0.4.6/setup.py
```

### Comparing `eras-0.4.5/PKG-INFO` & `eras-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.5
+Version: 0.4.6
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.4.5/README.md` & `eras-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/__pycache__/main.cpython-311.pyc` & `eras-0.4.6/eras/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.4.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.4.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.4.6/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/llama_functions_agent.py` & `eras-0.4.6/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.4.6/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/llm_functions_agent.py` & `eras-0.4.6/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/simple_llm.py` & `eras-0.4.6/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/agents/terminal_llama_agent.py` & `eras-0.4.6/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.4.6/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.4.6/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/config/config.py` & `eras-0.4.6/eras/config/config.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.4.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/decorators/chatgpt_tool_data.py` & `eras-0.4.6/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/factories/function_details_factory.py` & `eras-0.4.6/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/factories/message_factory.py` & `eras-0.4.6/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/main.py` & `eras-0.4.6/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.4.6/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.4.6/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.4.6/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.4.6/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.4.6/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.4.6/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/conversation.py` & `eras-0.4.6/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/function_details.py` & `eras-0.4.6/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/message.py` & `eras-0.4.6/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/models/transaction.py` & `eras-0.4.6/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/run.ipynb` & `eras-0.4.6/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.4.6/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/__pycache__/user_config_service.cpython-311.pyc` & `eras-0.4.6/eras/services/__pycache__/user_config_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.4.6/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.4.6/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/llm_callable_functions/user_details.py` & `eras-0.4.6/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/shell_command_service.py` & `eras-0.4.6/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/user_command_service.py` & `eras-0.4.6/eras/services/user_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/services/user_config_service.py` & `eras-0.4.6/eras/services/user_config_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         print("/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics")
         print("/conf - configure eras. urls, keys, etc")
         print("")
         print("=" * terminal_width)
 
     def print_eras_logo(self):
         # Define ANSI escape codes for 256-color mode with given RGB colors
-
+        init(autoreset=True)
         # colors = [
         #     "\033[94m",  # Bright blue
         #     "\033[96m",  # Bright cyan
         #     "\033[91m",  # Bright red
         #     "\033[93m",  # Bright yellow
         #     "\033[95m"  # Bright magenta
         # ]
```

### Comparing `eras-0.4.5/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.4.6/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras/utils/env_vars_and_profile_files.py` & `eras-0.4.6/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/eras.egg-info/PKG-INFO` & `eras-0.4.6/eras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.5
+Version: 0.4.6
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.4.5/eras.egg-info/SOURCES.txt` & `eras-0.4.6/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.4.5/setup.py` & `eras-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.4.5',
+    version='0.4.6',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

