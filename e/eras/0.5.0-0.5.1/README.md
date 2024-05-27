# Comparing `tmp/eras-0.5.0.tar.gz` & `tmp/eras-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.5.0.tar", last modified: Mon May 27 00:43:39 2024, max compression
+gzip compressed data, was "eras-0.5.1.tar", last modified: Mon May 27 01:21:15 2024, max compression
```

## Comparing `eras-0.5.0.tar` & `eras-0.5.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.544944 eras-0.5.0/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.5.0/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.5.0/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     5594 2024-05-27 00:43:39.544328 eras-0.5.0/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4847 2024-05-26 23:40:57.000000 eras-0.5.0/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.507213 eras-0.5.0/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.5.0/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.510209 eras-0.5.0/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.5.0/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.5.0/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-27 00:19:54.000000 eras-0.5.0/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.512931 eras-0.5.0/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.5.0/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.516342 eras-0.5.0/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.0/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.5.0/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.5.0/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.5.0/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.5.0/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.5.0/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.5.0/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.5.0/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.5.0/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.517067 eras-0.5.0/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.5.0/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.518211 eras-0.5.0/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.0/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4250 2024-05-27 00:19:54.000000 eras-0.5.0/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.5.0/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2963 2024-05-27 00:17:47.000000 eras-0.5.0/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.519019 eras-0.5.0/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.5.0/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.520057 eras-0.5.0/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.5.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.5.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.5.0/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.521340 eras-0.5.0/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.5.0/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.523575 eras-0.5.0/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.5.0/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.5.0/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.5.0/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-26 23:29:43.000000 eras-0.5.0/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.527555 eras-0.5.0/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.5.0/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.531662 eras-0.5.0/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.0/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.5.0/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.5.0/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.5.0/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.5.0/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.5.0/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.5.0/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.5.0/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.5.0/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.5.0/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.5.0/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.5.0/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.5.0/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.5.0/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.5.0/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-26 23:29:43.000000 eras-0.5.0/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.533923 eras-0.5.0/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.5.0/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.536964 eras-0.5.0/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.5.0/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1842 2024-05-27 00:43:05.000000 eras-0.5.0/eras/services/__pycache__/google_analytics.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2655 2024-05-26 23:28:19.000000 eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-27 00:19:54.000000 eras-0.5.0/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7863 2024-05-26 23:17:05.000000 eras-0.5.0/eras/services/__pycache__/user_config_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2531 2024-05-27 00:42:59.000000 eras-0.5.0/eras/services/google_analytics.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.538852 eras-0.5.0/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.5.0/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.541829 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.5.0/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.5.0/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.5.0/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1987 2024-05-26 23:18:45.000000 eras-0.5.0/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     2018 2024-05-27 00:19:35.000000 eras-0.5.0/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)    10789 2024-05-26 03:49:06.000000 eras-0.5.0/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.542628 eras-0.5.0/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.5.0/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.543468 eras-0.5.0/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.5.0/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.5.0/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.5.0/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.509155 eras-0.5.0/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     5594 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3996 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)      132 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-27 00:43:39.545055 eras-0.5.0/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1145 2024-05-27 00:33:06.000000 eras-0.5.0/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.411882 eras-0.5.1/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.5.1/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.5.1/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     5379 2024-05-27 01:21:15.411163 eras-0.5.1/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4632 2024-05-27 01:20:55.000000 eras-0.5.1/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.379582 eras-0.5.1/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.5.1/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.382153 eras-0.5.1/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.5.1/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.5.1/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-27 00:19:54.000000 eras-0.5.1/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.383923 eras-0.5.1/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.5.1/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.388031 eras-0.5.1/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.1/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.5.1/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.5.1/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.5.1/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.5.1/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.5.1/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.5.1/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.5.1/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.5.1/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.5.1/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.5.1/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.5.1/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.5.1/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.388883 eras-0.5.1/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.5.1/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.390027 eras-0.5.1/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.1/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4250 2024-05-27 00:19:54.000000 eras-0.5.1/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.5.1/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2963 2024-05-27 00:17:47.000000 eras-0.5.1/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.390690 eras-0.5.1/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.5.1/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.391579 eras-0.5.1/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.5.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.5.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.5.1/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.392474 eras-0.5.1/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.5.1/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.394507 eras-0.5.1/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.5.1/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.5.1/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.5.1/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.5.1/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.5.1/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.5.1/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.5.1/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-26 23:29:43.000000 eras-0.5.1/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.397266 eras-0.5.1/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.5.1/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.400380 eras-0.5.1/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.1/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.5.1/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.5.1/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.5.1/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.5.1/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.5.1/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.5.1/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.5.1/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.5.1/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.5.1/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.5.1/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.5.1/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.5.1/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.5.1/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.5.1/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-26 23:29:43.000000 eras-0.5.1/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.401997 eras-0.5.1/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.5.1/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.404286 eras-0.5.1/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.5.1/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1842 2024-05-27 00:43:05.000000 eras-0.5.1/eras/services/__pycache__/google_analytics.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2655 2024-05-26 23:28:19.000000 eras-0.5.1/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.5.1/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-27 00:19:54.000000 eras-0.5.1/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7863 2024-05-26 23:17:05.000000 eras-0.5.1/eras/services/__pycache__/user_config_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2531 2024-05-27 00:42:59.000000 eras-0.5.1/eras/services/google_analytics.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.406131 eras-0.5.1/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.5.1/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.408869 eras-0.5.1/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.5.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.5.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.5.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.5.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.5.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.5.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.5.1/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.5.1/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.5.1/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1987 2024-05-26 23:18:45.000000 eras-0.5.1/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     2018 2024-05-27 00:19:35.000000 eras-0.5.1/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)    10789 2024-05-26 03:49:06.000000 eras-0.5.1/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.409542 eras-0.5.1/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.5.1/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.410280 eras-0.5.1/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.5.1/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.5.1/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.5.1/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 01:21:15.381232 eras-0.5.1/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     5379 2024-05-27 01:21:15.000000 eras-0.5.1/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3996 2024-05-27 01:21:15.000000 eras-0.5.1/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-27 01:21:15.000000 eras-0.5.1/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-27 01:21:15.000000 eras-0.5.1/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)      132 2024-05-27 01:21:15.000000 eras-0.5.1/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-27 01:21:15.000000 eras-0.5.1/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-27 01:21:15.412037 eras-0.5.1/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1145 2024-05-27 01:21:04.000000 eras-0.5.1/setup.py
```

### Comparing `eras-0.5.0/PKG-INFO` & `eras-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.5.0
+Version: 0.5.1
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -142,14 +142,9 @@
 cmake --build . --config Release
 ```
 
 Start the Llama server:
 ``` 
 .\bin\Release\server.exe -m C:\shared-drive\llm_models\Llama-3-8B-Instruct-32k-v0.1.Q4_K_M.gguf -ngl 9999 --host 0.0.0.0 --ctx-size 32000
 ```
-# Upcoming functionality
 
-## Llama 3 support
-Llama.cpp provides an API similar to OpenAI, so pointing eras at http://127.0.0.1:8080 works as expected.  
-
-I just need to prompt for the base_url preference and use it.
```

### Comparing `eras-0.5.0/README.md` & `eras-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,9 @@
 cmake --build . --config Release
 ```
 
 Start the Llama server:
 ``` 
 .\bin\Release\server.exe -m C:\shared-drive\llm_models\Llama-3-8B-Instruct-32k-v0.1.Q4_K_M.gguf -ngl 9999 --host 0.0.0.0 --ctx-size 32000
 ```
-# Upcoming functionality
 
-## Llama 3 support
-Llama.cpp provides an API similar to OpenAI, so pointing eras at http://127.0.0.1:8080 works as expected.  
-
-I just need to prompt for the base_url preference and use it.
```

### Comparing `eras-0.5.0/eras/__pycache__/main.cpython-311.pyc` & `eras-0.5.1/eras/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.5.1/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.5.1/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.5.1/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.5.1/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.5.1/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.5.1/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.5.1/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/llama_functions_agent.py` & `eras-0.5.1/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.5.1/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/llm_functions_agent.py` & `eras-0.5.1/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/simple_llm.py` & `eras-0.5.1/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/agents/terminal_llama_agent.py` & `eras-0.5.1/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.5.1/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.5.1/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/config/config.py` & `eras-0.5.1/eras/config/config.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.5.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/decorators/chatgpt_tool_data.py` & `eras-0.5.1/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.5.1/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.5.1/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.5.1/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.5.1/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/factories/function_details_factory.py` & `eras-0.5.1/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/factories/message_factory.py` & `eras-0.5.1/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/main.py` & `eras-0.5.1/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.5.1/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.5.1/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.5.1/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.5.1/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.5.1/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.5.1/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/conversation.py` & `eras-0.5.1/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/function_details.py` & `eras-0.5.1/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/message.py` & `eras-0.5.1/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/models/transaction.py` & `eras-0.5.1/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/run.ipynb` & `eras-0.5.1/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/__pycache__/google_analytics.cpython-311.pyc` & `eras-0.5.1/eras/services/__pycache__/google_analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.5.1/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.5.1/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.5.1/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/__pycache__/user_config_service.cpython-311.pyc` & `eras-0.5.1/eras/services/__pycache__/user_config_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/google_analytics.py` & `eras-0.5.1/eras/services/google_analytics.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.5.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.5.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.5.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.5.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.5.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.5.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.5.1/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.5.1/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/llm_callable_functions/user_details.py` & `eras-0.5.1/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/shell_command_service.py` & `eras-0.5.1/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/user_command_service.py` & `eras-0.5.1/eras/services/user_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/services/user_config_service.py` & `eras-0.5.1/eras/services/user_config_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.5.1/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras/utils/env_vars_and_profile_files.py` & `eras-0.5.1/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/eras.egg-info/PKG-INFO` & `eras-0.5.1/eras.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.5.0
+Version: 0.5.1
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -142,14 +142,9 @@
 cmake --build . --config Release
 ```
 
 Start the Llama server:
 ``` 
 .\bin\Release\server.exe -m C:\shared-drive\llm_models\Llama-3-8B-Instruct-32k-v0.1.Q4_K_M.gguf -ngl 9999 --host 0.0.0.0 --ctx-size 32000
 ```
-# Upcoming functionality
 
-## Llama 3 support
-Llama.cpp provides an API similar to OpenAI, so pointing eras at http://127.0.0.1:8080 works as expected.  
-
-I just need to prompt for the base_url preference and use it.
```

### Comparing `eras-0.5.0/eras.egg-info/SOURCES.txt` & `eras-0.5.1/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.5.0/setup.py` & `eras-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.5.0',
+    version='0.5.1',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

