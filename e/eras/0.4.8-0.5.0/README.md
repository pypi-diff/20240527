# Comparing `tmp/eras-0.4.8.tar.gz` & `tmp/eras-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.4.8.tar", last modified: Sun May 26 23:41:13 2024, max compression
+gzip compressed data, was "eras-0.5.0.tar", last modified: Mon May 27 00:43:39 2024, max compression
```

## Comparing `eras-0.4.8.tar` & `eras-0.5.0.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.776696 eras-0.4.8/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.8/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.8/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     5534 2024-05-26 23:41:13.776348 eras-0.4.8/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4847 2024-05-26 23:40:57.000000 eras-0.4.8/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.746330 eras-0.4.8/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.8/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.748767 eras-0.4.8/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.8/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.8/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      818 2024-05-26 23:28:19.000000 eras-0.4.8/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.750457 eras-0.4.8/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.8/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.753018 eras-0.4.8/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.8/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.8/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.8/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.8/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.8/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.8/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.8/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.8/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.8/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.8/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.8/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.8/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.8/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.753660 eras-0.4.8/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.8/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.754662 eras-0.4.8/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.8/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.8/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.8/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.8/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.755058 eras-0.4.8/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.8/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.755786 eras-0.4.8/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.8/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.8/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.8/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.756963 eras-0.4.8/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.8/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.759235 eras-0.4.8/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.8/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.8/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.8/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.8/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.8/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.8/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.8/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-26 23:29:43.000000 eras-0.4.8/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.762184 eras-0.4.8/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.8/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.766316 eras-0.4.8/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.8/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.8/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.8/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.8/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.8/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.8/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.8/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.8/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.8/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.8/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.8/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.8/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.8/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.8/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.8/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-26 23:29:43.000000 eras-0.4.8/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.767692 eras-0.4.8/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.8/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.769631 eras-0.4.8/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.8/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2655 2024-05-26 23:28:19.000000 eras-0.4.8/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.8/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.8/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7863 2024-05-26 23:17:05.000000 eras-0.4.8/eras/services/__pycache__/user_config_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.771409 eras-0.4.8/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.8/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.774005 eras-0.4.8/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.8/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.8/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.8/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.8/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.8/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.8/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.8/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.8/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.8/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1987 2024-05-26 23:18:45.000000 eras-0.4.8/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.8/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)    10789 2024-05-26 03:49:06.000000 eras-0.4.8/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.774825 eras-0.4.8/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.8/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.775657 eras-0.4.8/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.8/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.8/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.8/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:41:13.747934 eras-0.4.8/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     5534 2024-05-26 23:41:13.000000 eras-0.4.8/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 23:41:13.000000 eras-0.4.8/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 23:41:13.000000 eras-0.4.8/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 23:41:13.000000 eras-0.4.8/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)      102 2024-05-26 23:41:13.000000 eras-0.4.8/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 23:41:13.000000 eras-0.4.8/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 23:41:13.776764 eras-0.4.8/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1093 2024-05-26 23:41:07.000000 eras-0.4.8/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.544944 eras-0.5.0/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.5.0/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.5.0/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     5594 2024-05-27 00:43:39.544328 eras-0.5.0/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4847 2024-05-26 23:40:57.000000 eras-0.5.0/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.507213 eras-0.5.0/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.5.0/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.510209 eras-0.5.0/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.5.0/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.5.0/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-27 00:19:54.000000 eras-0.5.0/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.512931 eras-0.5.0/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.5.0/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.516342 eras-0.5.0/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.0/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.5.0/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.5.0/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.5.0/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.5.0/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.5.0/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.5.0/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.5.0/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.5.0/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.517067 eras-0.5.0/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.5.0/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.518211 eras-0.5.0/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.0/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4250 2024-05-27 00:19:54.000000 eras-0.5.0/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.5.0/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2963 2024-05-27 00:17:47.000000 eras-0.5.0/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.519019 eras-0.5.0/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.5.0/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.520057 eras-0.5.0/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.5.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.5.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.5.0/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.521340 eras-0.5.0/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.5.0/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.523575 eras-0.5.0/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.5.0/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.5.0/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.5.0/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-26 23:29:43.000000 eras-0.5.0/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.527555 eras-0.5.0/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.5.0/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.531662 eras-0.5.0/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.5.0/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.5.0/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.5.0/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.5.0/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.5.0/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.5.0/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.5.0/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.5.0/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.5.0/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.5.0/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.5.0/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.5.0/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.5.0/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.5.0/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.5.0/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-26 23:29:43.000000 eras-0.5.0/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.533923 eras-0.5.0/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.5.0/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.536964 eras-0.5.0/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.5.0/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1842 2024-05-27 00:43:05.000000 eras-0.5.0/eras/services/__pycache__/google_analytics.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2655 2024-05-26 23:28:19.000000 eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-27 00:19:54.000000 eras-0.5.0/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7863 2024-05-26 23:17:05.000000 eras-0.5.0/eras/services/__pycache__/user_config_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2531 2024-05-27 00:42:59.000000 eras-0.5.0/eras/services/google_analytics.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.538852 eras-0.5.0/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.5.0/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.541829 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.5.0/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.5.0/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.5.0/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1987 2024-05-26 23:18:45.000000 eras-0.5.0/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     2018 2024-05-27 00:19:35.000000 eras-0.5.0/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)    10789 2024-05-26 03:49:06.000000 eras-0.5.0/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.542628 eras-0.5.0/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.5.0/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.543468 eras-0.5.0/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.5.0/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.5.0/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.5.0/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-27 00:43:39.509155 eras-0.5.0/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     5594 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3996 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)      132 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-27 00:43:39.000000 eras-0.5.0/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-27 00:43:39.545055 eras-0.5.0/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1145 2024-05-27 00:33:06.000000 eras-0.5.0/setup.py
```

### Comparing `eras-0.4.8/PKG-INFO` & `eras-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.8
+Version: 0.5.0
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: InquirerPy==0.3.4
 Requires-Dist: colorama==0.4.6
+Requires-Dist: requests==2.31.0
+Requires-Dist: ga4mp==2.0.4
 
 # Unlock the Power of Your Terminal with ERAS 🚀
 Welcome to ERAS: the Easily Runnable AI Shell that revolutionizes your command-line experience. 
 
 Say goodbye to the hassle of searching for the right command syntax—ERAS transforms your natural language instructions into precise terminal commands instantly.
 
 ## Why ERAS?
```

### Comparing `eras-0.4.8/README.md` & `eras-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.5.0/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.5.0/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.5.0/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.5.0/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.5.0/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/llama_functions_agent.py` & `eras-0.5.0/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.5.0/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/llm_functions_agent.py` & `eras-0.5.0/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/simple_llm.py` & `eras-0.5.0/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/agents/terminal_llama_agent.py` & `eras-0.5.0/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.5.0/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.5.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/decorators/chatgpt_tool_data.py` & `eras-0.5.0/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.5.0/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.5.0/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/factories/function_details_factory.py` & `eras-0.5.0/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/factories/message_factory.py` & `eras-0.5.0/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/main.py` & `eras-0.5.0/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.5.0/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.5.0/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.5.0/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.5.0/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.5.0/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.5.0/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/conversation.py` & `eras-0.5.0/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/function_details.py` & `eras-0.5.0/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/message.py` & `eras-0.5.0/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/models/transaction.py` & `eras-0.5.0/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/run.ipynb` & `eras-0.5.0/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.5.0/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.5.0/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x84ab5266 (Sun May 26 03:24:52 2024 UTC)
-files sz: 1805
+moddate:  0x97d15366 (Mon May 27 00:19:35 2024 UTC)
+files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
-      045a040100640064046c056d065a060100640064016c075a07640064056c
-      086d095a090100640064016c0a5a0a02004700640684006407a6020000ab
-      0200000000000000005a0b64015300
+      045a040100640064046c056d065a060100640064056c076d085a08010064
+      0064016c095a09640064066c0a6d0b5a0b0100640064016c0c5a0c020047
+      00640784006408a6020000ab0200000000000000005a0d64015300
      0           0 RESUME                   0
    
      2           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -29,92 +29,100 @@
                 24 LOAD_CONST               3 (('config',))
                 26 IMPORT_NAME              3 (eras.config.config)
                 28 IMPORT_FROM              4 (config)
                 30 STORE_NAME               4 (config)
                 32 POP_TOP
    
      6          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               4 (('ShellCommandService',))
-                38 IMPORT_NAME              5 (eras.services.shell_command_service)
-                40 IMPORT_FROM              6 (ShellCommandService)
-                42 STORE_NAME               6 (ShellCommandService)
+                36 LOAD_CONST               4 (('send_analytics_event',))
+                38 IMPORT_NAME              5 (eras.services.google_analytics)
+                40 IMPORT_FROM              6 (send_analytics_event)
+                42 STORE_NAME               6 (send_analytics_event)
                 44 POP_TOP
    
      7          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               1 (None)
-                50 IMPORT_NAME              7 (openai)
-                52 STORE_NAME               7 (openai)
+                48 LOAD_CONST               5 (('ShellCommandService',))
+                50 IMPORT_NAME              7 (eras.services.shell_command_service)
+                52 IMPORT_FROM              8 (ShellCommandService)
+                54 STORE_NAME               8 (ShellCommandService)
+                56 POP_TOP
    
-     9          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               5 (('UserConfigService',))
-                58 IMPORT_NAME              8 (eras.services.user_config_service)
-                60 IMPORT_FROM              9 (UserConfigService)
-                62 STORE_NAME               9 (UserConfigService)
-                64 POP_TOP
+     8          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               1 (None)
+                62 IMPORT_NAME              9 (openai)
+                64 STORE_NAME               9 (openai)
    
     10          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               1 (None)
-                70 IMPORT_NAME             10 (httpx)
-                72 STORE_NAME              10 (httpx)
+                68 LOAD_CONST               6 (('UserConfigService',))
+                70 IMPORT_NAME             10 (eras.services.user_config_service)
+                72 IMPORT_FROM             11 (UserConfigService)
+                74 STORE_NAME              11 (UserConfigService)
+                76 POP_TOP
    
-    12          74 PUSH_NULL
-                76 LOAD_BUILD_CLASS
-                78 LOAD_CONST               6 (<code object UserCommandService, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 12>)
-                80 MAKE_FUNCTION            0
-                82 LOAD_CONST               7 ('UserCommandService')
-                84 PRECALL                  2
-                88 CALL                     2
-                98 STORE_NAME              11 (UserCommandService)
-               100 LOAD_CONST               1 (None)
-               102 RETURN_VALUE
+    11          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               1 (None)
+                82 IMPORT_NAME             12 (httpx)
+                84 STORE_NAME              12 (httpx)
+   
+    13          86 PUSH_NULL
+                88 LOAD_BUILD_CLASS
+                90 LOAD_CONST               7 (<code object UserCommandService, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 13>)
+                92 MAKE_FUNCTION            0
+                94 LOAD_CONST               8 ('UserCommandService')
+                96 PRECALL                  2
+               100 CALL                     2
+               110 STORE_NAME              13 (UserCommandService)
+               112 LOAD_CONST               1 (None)
+               114 RETURN_VALUE
    consts
       0
       None
       ('SimpleLLM',)
       ('config',)
+      ('send_analytics_event',)
       ('ShellCommandService',)
       ('UserConfigService',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640265046602640384045a0564
             0484005a06640584005a07640684005a08640784005a0964085300
-          12           0 RESUME                   0
+          13           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('UserCommandService')
                        8 STORE_NAME               2 (__qualname__)
          
-          13          10 LOAD_CONST               1 (<code object __init__, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 13>)
+          14          10 LOAD_CONST               1 (<code object __init__, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 14>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          22          16 LOAD_CONST               2 ('user_input')
+          23          16 LOAD_CONST               2 ('user_input')
                       18 LOAD_NAME                4 (str)
                       20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object handle_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 22>)
+                      22 LOAD_CONST               3 (<code object handle_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 23>)
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (handle_request)
          
-          32          28 LOAD_CONST               4 (<code object handle_help_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 32>)
+          33          28 LOAD_CONST               4 (<code object handle_help_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 33>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (handle_help_request)
          
-          36          34 LOAD_CONST               5 (<code object handle_chat_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 36>)
+          38          34 LOAD_CONST               5 (<code object handle_chat_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 38>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               7 (handle_chat_request)
          
-          49          40 LOAD_CONST               6 (<code object handle_shell_nli_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 49>)
+          52          40 LOAD_CONST               6 (<code object handle_shell_nli_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 52>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               8 (handle_shell_nli_request)
          
-          52          46 LOAD_CONST               7 (<code object handle_config_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 52>)
+          56          46 LOAD_CONST               7 (<code object handle_config_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 56>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               9 (handle_config_request)
                       52 LOAD_CONST               8 (None)
                       54 RETURN_VALUE
          consts
             'UserCommandService'
             code
@@ -128,52 +136,52 @@
                   007405000000000000000000006a040000000000000000a6000000ab0000
                   00000000000000ac01a6020000ab0200000000000000007c005f05000000
                   0000000000740d000000000000000000007c006a050000000000000000a6
                   010000ab0100000000000000007c005f0700000000000000007411000000
                   000000000000007c006a050000000000000000a6010000ab010000000000
                   0000007c005f090000000000000000741500000000000000000000a60000
                   00ab0000000000000000007c005f0b000000000000000064005300
-                13           0 RESUME                   0
+                14           0 RESUME                   0
                
-                14           2 LOAD_GLOBAL              1 (NULL + openai)
+                15           2 LOAD_GLOBAL              1 (NULL + openai)
                             14 LOAD_ATTR                1 (OpenAI)
                
-                15          24 LOAD_GLOBAL              5 (NULL + config)
+                16          24 LOAD_GLOBAL              5 (NULL + config)
                             36 LOAD_ATTR                3 (get_eras_base_url)
                             46 PRECALL                  0
                             50 CALL                     0
                
-                16          60 LOAD_GLOBAL              5 (NULL + config)
+                17          60 LOAD_GLOBAL              5 (NULL + config)
                             72 LOAD_ATTR                4 (get_eras_open_ai_key)
                             82 PRECALL                  0
                             86 CALL                     0
                
-                14          96 KW_NAMES                 1
+                15          96 KW_NAMES                 1
                             98 PRECALL                  2
                            102 CALL                     2
                            112 LOAD_FAST                0 (self)
                            114 STORE_ATTR               5 (openai_client)
                
-                18         124 LOAD_GLOBAL             13 (NULL + ShellCommandService)
+                19         124 LOAD_GLOBAL             13 (NULL + ShellCommandService)
                            136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                5 (openai_client)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 LOAD_FAST                0 (self)
                            164 STORE_ATTR               7 (shell_command_service)
                
-                19         174 LOAD_GLOBAL             17 (NULL + SimpleLLM)
+                20         174 LOAD_GLOBAL             17 (NULL + SimpleLLM)
                            186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                5 (openai_client)
                            198 PRECALL                  1
                            202 CALL                     1
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               9 (simple_llm)
                
-                20         224 LOAD_GLOBAL             21 (NULL + UserConfigService)
+                21         224 LOAD_GLOBAL             21 (NULL + UserConfigService)
                            236 PRECALL                  0
                            240 CALL                     0
                            250 LOAD_FAST                0 (self)
                            252 STORE_ATTR              11 (user_config_service)
                            262 LOAD_CONST               0 (None)
                            264 RETURN_VALUE
                consts
@@ -181,15 +189,15 @@
                   ('base_url', 'api_key')
                names      ('openai', 'OpenAI', 'config', 'get_eras_base_url', 'get_eras_open_ai_key', 'openai_client', 'ShellCommandService', 'shell_command_service', 'SimpleLLM', 'simple_llm', 'UserConfigService', 'user_config_service')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       '__init__'
-               firstlineno 13
+               firstlineno 14
                lnotab 0x02011601240124fe1c0432013201
             'user_input'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
@@ -201,65 +209,65 @@
                   00ab01000000000000000072177c00a00200000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000000100640053007c
                   01a00000000000000000000000000000000000000000006403a6010000ab
                   01000000000000000072177c00a003000000000000000000000000000000
                   00000000007c01a6010000ab0100000000000000000100640053007c00a0
                   0400000000000000000000000000000000000000007c01a6010000ab0100
                   00000000000000010064005300
-                22           0 RESUME                   0
+                23           0 RESUME                   0
                
-                23           2 LOAD_FAST                1 (user_input)
+                24           2 LOAD_FAST                1 (user_input)
                              4 LOAD_METHOD              0 (startswith)
                             26 LOAD_CONST               1 ('/help')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    23 (to 90)
                
-                24          44 LOAD_FAST                0 (self)
+                25          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (handle_help_request)
                             68 LOAD_FAST                1 (user_input)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 POP_TOP
                             86 LOAD_CONST               0 (None)
                             88 RETURN_VALUE
                
-                25     >>   90 LOAD_FAST                1 (user_input)
+                26     >>   90 LOAD_FAST                1 (user_input)
                             92 LOAD_METHOD              0 (startswith)
                            114 LOAD_CONST               2 ('/chat')
                            116 PRECALL                  1
                            120 CALL                     1
                            130 POP_JUMP_FORWARD_IF_FALSE    23 (to 178)
                
-                26         132 LOAD_FAST                0 (self)
+                27         132 LOAD_FAST                0 (self)
                            134 LOAD_METHOD              2 (handle_chat_request)
                            156 LOAD_FAST                1 (user_input)
                            158 PRECALL                  1
                            162 CALL                     1
                            172 POP_TOP
                            174 LOAD_CONST               0 (None)
                            176 RETURN_VALUE
                
-                27     >>  178 LOAD_FAST                1 (user_input)
+                28     >>  178 LOAD_FAST                1 (user_input)
                            180 LOAD_METHOD              0 (startswith)
                            202 LOAD_CONST               3 ('/config')
                            204 PRECALL                  1
                            208 CALL                     1
                            218 POP_JUMP_FORWARD_IF_FALSE    23 (to 266)
                
-                28         220 LOAD_FAST                0 (self)
+                29         220 LOAD_FAST                0 (self)
                            222 LOAD_METHOD              3 (handle_config_request)
                            244 LOAD_FAST                1 (user_input)
                            246 PRECALL                  1
                            250 CALL                     1
                            260 POP_TOP
                            262 LOAD_CONST               0 (None)
                            264 RETURN_VALUE
                
-                30     >>  266 LOAD_FAST                0 (self)
+                31     >>  266 LOAD_FAST                0 (self)
                            268 LOAD_METHOD              4 (handle_shell_nli_request)
                            290 LOAD_FAST                1 (user_input)
                            292 PRECALL                  1
                            296 CALL                     1
                            306 POP_TOP
                            308 LOAD_CONST               0 (None)
                            310 RETURN_VALUE
@@ -270,120 +278,136 @@
                   '/config'
                names      ('startswith', 'handle_help_request', 'handle_chat_request', 'handle_config_request', 'handle_shell_nli_request')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_request'
-               firstlineno 22
+               firstlineno 23
                lnotab 0x02012a012e012a012e012a012e02
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 2
+               stacksize : 3
                flags     : 3
                code
-                  0x97007c006a000000000000000000a00100000000000000000000000000
-                  00000000000000a6000000ab00000000000000000001007c006a00000000
-                  0000000000a0020000000000000000000000000000000000000000a60000
+                  0x97007401000000000000000000006401a6010000ab0100000000000000
+                  0001007c006a010000000000000000a00200000000000000000000000000
+                  00000000000000a6000000ab00000000000000000001007c006a01000000
+                  0000000000a0030000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                32           0 RESUME                   0
+                33           0 RESUME                   0
                
-                33           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (user_config_service)
-                            14 LOAD_METHOD              1 (print_eras_logo)
-                            36 PRECALL                  0
-                            40 CALL                     0
-                            50 POP_TOP
-               
-                34          52 LOAD_FAST                0 (self)
-                            54 LOAD_ATTR                0 (user_config_service)
-                            64 LOAD_METHOD              2 (show_commands)
-                            86 PRECALL                  0
-                            90 CALL                     0
-                           100 POP_TOP
-                           102 LOAD_CONST               0 (None)
-                           104 RETURN_VALUE
+                34           2 LOAD_GLOBAL              1 (NULL + send_analytics_event)
+                            14 LOAD_CONST               1 ('help')
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 POP_TOP
+               
+                35          32 LOAD_FAST                0 (self)
+                            34 LOAD_ATTR                1 (user_config_service)
+                            44 LOAD_METHOD              2 (print_eras_logo)
+                            66 PRECALL                  0
+                            70 CALL                     0
+                            80 POP_TOP
+               
+                36          82 LOAD_FAST                0 (self)
+                            84 LOAD_ATTR                1 (user_config_service)
+                            94 LOAD_METHOD              3 (show_commands)
+                           116 PRECALL                  0
+                           120 CALL                     0
+                           130 POP_TOP
+                           132 LOAD_CONST               0 (None)
+                           134 RETURN_VALUE
                consts
                   None
-               names      ('user_config_service', 'print_eras_logo', 'show_commands')
+                  'help'
+               names      ('send_analytics_event', 'user_config_service', 'print_eras_logo', 'show_commands')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_help_request'
-               firstlineno 32
-               lnotab 0x02013201
+               firstlineno 33
+               lnotab 0x02011e013201
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 5
                flags     : 3
                code
-                  0x97007401000000000000000000006a01000000000000000064017c01a6
-                  020000ab0200000000000000007d027c0272157c02a00200000000000000
-                  000000000000000000000000006402a6010000ab0100000000000000006e
-                  0164007d03640384007d04640484007d057c006a030000000000000000a0
-                  0400000000000000000000000000000000000000007c037c047c05a60300
+                  0x97007401000000000000000000006401a6010000ab0100000000000000
+                  0001007403000000000000000000006a02000000000000000064027c01a6
+                  020000ab0200000000000000007d027c0272157c02a00300000000000000
+                  000000000000000000000000006403a6010000ab0100000000000000006e
+                  0164007d03640484007d04640584007d057c006a040000000000000000a0
+                  0500000000000000000000000000000000000000007c037c047c05a60300
                   00ab030000000000000000010064005300
-                36           0 RESUME                   0
+                38           0 RESUME                   0
                
-                37           2 LOAD_GLOBAL              1 (NULL + re)
-                            14 LOAD_ATTR                1 (match)
-                            24 LOAD_CONST               1 ('^/chat\\s+(.*)')
-                            26 LOAD_FAST                1 (user_input)
-                            28 PRECALL                  2
-                            32 CALL                     2
-                            42 STORE_FAST               2 (match)
-               
-                38          44 LOAD_FAST                2 (match)
-                            46 POP_JUMP_FORWARD_IF_FALSE    21 (to 90)
-                            48 LOAD_FAST                2 (match)
-                            50 LOAD_METHOD              2 (group)
-                            72 LOAD_CONST               2 (1)
-                            74 PRECALL                  1
-                            78 CALL                     1
-                            88 JUMP_FORWARD             1 (to 92)
-                       >>   90 LOAD_CONST               0 (None)
-                       >>   92 STORE_FAST               3 (prompt)
-               
-                40          94 LOAD_CONST               3 (<code object handle_text_received, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 40>)
-                            96 MAKE_FUNCTION            0
-                            98 STORE_FAST               4 (handle_text_received)
-               
-                43         100 LOAD_CONST               4 (<code object handle_response_complete, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 43>)
-                           102 MAKE_FUNCTION            0
-                           104 STORE_FAST               5 (handle_response_complete)
-               
-                46         106 LOAD_FAST                0 (self)
-                           108 LOAD_ATTR                3 (simple_llm)
-                           118 LOAD_METHOD              4 (stream_inference)
-                           140 LOAD_FAST                3 (prompt)
-                           142 LOAD_FAST                4 (handle_text_received)
-                           144 LOAD_FAST                5 (handle_response_complete)
-                           146 PRECALL                  3
-                           150 CALL                     3
-                           160 POP_TOP
-                           162 LOAD_CONST               0 (None)
-                           164 RETURN_VALUE
+                39           2 LOAD_GLOBAL              1 (NULL + send_analytics_event)
+                            14 LOAD_CONST               1 ('chat')
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 POP_TOP
+               
+                40          32 LOAD_GLOBAL              3 (NULL + re)
+                            44 LOAD_ATTR                2 (match)
+                            54 LOAD_CONST               2 ('^/chat\\s+(.*)')
+                            56 LOAD_FAST                1 (user_input)
+                            58 PRECALL                  2
+                            62 CALL                     2
+                            72 STORE_FAST               2 (match)
+               
+                41          74 LOAD_FAST                2 (match)
+                            76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
+                            78 LOAD_FAST                2 (match)
+                            80 LOAD_METHOD              3 (group)
+                           102 LOAD_CONST               3 (1)
+                           104 PRECALL                  1
+                           108 CALL                     1
+                           118 JUMP_FORWARD             1 (to 122)
+                       >>  120 LOAD_CONST               0 (None)
+                       >>  122 STORE_FAST               3 (prompt)
+               
+                43         124 LOAD_CONST               4 (<code object handle_text_received, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 43>)
+                           126 MAKE_FUNCTION            0
+                           128 STORE_FAST               4 (handle_text_received)
+               
+                46         130 LOAD_CONST               5 (<code object handle_response_complete, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 46>)
+                           132 MAKE_FUNCTION            0
+                           134 STORE_FAST               5 (handle_response_complete)
+               
+                49         136 LOAD_FAST                0 (self)
+                           138 LOAD_ATTR                4 (simple_llm)
+                           148 LOAD_METHOD              5 (stream_inference)
+                           170 LOAD_FAST                3 (prompt)
+                           172 LOAD_FAST                4 (handle_text_received)
+                           174 LOAD_FAST                5 (handle_response_complete)
+                           176 PRECALL                  3
+                           180 CALL                     3
+                           190 POP_TOP
+                           192 LOAD_CONST               0 (None)
+                           194 RETURN_VALUE
                consts
                   None
+                  'chat'
                   '^/chat\\s+(.*)'
                   1
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 4
                      flags     : 19
                      code
                         0x97007401000000000000000000007c006401ac02a6020000ab02000000
                         0000000000010064005300
-                      40           0 RESUME                   0
+                      43           0 RESUME                   0
                      
-                      41           2 LOAD_GLOBAL              1 (NULL + print)
+                      44           2 LOAD_GLOBAL              1 (NULL + print)
                                   14 LOAD_FAST                0 (text)
                                   16 LOAD_CONST               1 ('')
                                   18 KW_NAMES                 2
                                   20 PRECALL                  2
                                   24 CALL                     2
                                   34 POP_TOP
                                   36 LOAD_CONST               0 (None)
@@ -394,118 +418,134 @@
                         ('end',)
                      names      ('print',)
                      varnames   ('text',)
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                      name       'handle_text_received'
-                     firstlineno 40
+                     firstlineno 43
                      lnotab 0x0201
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 2
                      flags     : 19
                      code
                         0x9700740100000000000000000000a6000000ab00000000000000000001
                         0064005300
-                      43           0 RESUME                   0
+                      46           0 RESUME                   0
                      
-                      44           2 LOAD_GLOBAL              1 (NULL + print)
+                      47           2 LOAD_GLOBAL              1 (NULL + print)
                                   14 PRECALL                  0
                                   18 CALL                     0
                                   28 POP_TOP
                                   30 LOAD_CONST               0 (None)
                                   32 RETURN_VALUE
                      consts
                         None
                      names      ('print',)
                      varnames   ()
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                      name       'handle_response_complete'
-                     firstlineno 43
+                     firstlineno 46
                      lnotab 0x0201
-               names      ('re', 'match', 'group', 'simple_llm', 'stream_inference')
+               names      ('send_analytics_event', 're', 'match', 'group', 'simple_llm', 'stream_inference')
                varnames   ('self', 'user_input', 'match', 'prompt', 'handle_text_received', 'handle_response_complete')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_chat_request'
-               firstlineno 36
-               lnotab 0x02012a01320206030603
+               firstlineno 38
+               lnotab 0x02011e012a01320206030603
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
-                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  0x97007401000000000000000000006401a6010000ab0100000000000000
+                  0001007c006a010000000000000000a00200000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000010064005300
-                49           0 RESUME                   0
+                52           0 RESUME                   0
                
-                50           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (shell_command_service)
-                            14 LOAD_METHOD              1 (handle_prompt)
-                            36 LOAD_FAST                1 (user_input)
-                            38 PRECALL                  1
-                            42 CALL                     1
-                            52 POP_TOP
-                            54 LOAD_CONST               0 (None)
-                            56 RETURN_VALUE
+                53           2 LOAD_GLOBAL              1 (NULL + send_analytics_event)
+                            14 LOAD_CONST               1 ('nli')
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 POP_TOP
+               
+                54          32 LOAD_FAST                0 (self)
+                            34 LOAD_ATTR                1 (shell_command_service)
+                            44 LOAD_METHOD              2 (handle_prompt)
+                            66 LOAD_FAST                1 (user_input)
+                            68 PRECALL                  1
+                            72 CALL                     1
+                            82 POP_TOP
+                            84 LOAD_CONST               0 (None)
+                            86 RETURN_VALUE
                consts
                   None
-               names      ('shell_command_service', 'handle_prompt')
+                  'nli'
+               names      ('send_analytics_event', 'shell_command_service', 'handle_prompt')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_shell_nli_request'
-               firstlineno 49
-               lnotab 0x0201
+               firstlineno 52
+               lnotab 0x02011e01
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 2
+               stacksize : 3
                flags     : 3
                code
-                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  0x97007401000000000000000000006401a6010000ab0100000000000000
+                  0001007c006a010000000000000000a00200000000000000000000000000
                   00000000000000a6000000ab000000000000000000010064005300
-                52           0 RESUME                   0
+                56           0 RESUME                   0
                
-                53           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (user_config_service)
-                            14 LOAD_METHOD              1 (prompt_for_all_configs)
-                            36 PRECALL                  0
-                            40 CALL                     0
-                            50 POP_TOP
-                            52 LOAD_CONST               0 (None)
-                            54 RETURN_VALUE
+                57           2 LOAD_GLOBAL              1 (NULL + send_analytics_event)
+                            14 LOAD_CONST               1 ('config')
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 POP_TOP
+               
+                58          32 LOAD_FAST                0 (self)
+                            34 LOAD_ATTR                1 (user_config_service)
+                            44 LOAD_METHOD              2 (prompt_for_all_configs)
+                            66 PRECALL                  0
+                            70 CALL                     0
+                            80 POP_TOP
+                            82 LOAD_CONST               0 (None)
+                            84 RETURN_VALUE
                consts
                   None
-               names      ('user_config_service', 'prompt_for_all_configs')
+                  'config'
+               names      ('send_analytics_event', 'user_config_service', 'prompt_for_all_configs')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_config_request'
-               firstlineno 52
-               lnotab 0x0201
+               firstlineno 56
+               lnotab 0x02011e01
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'str', 'handle_request', 'handle_help_request', 'handle_chat_request', 'handle_shell_nli_request', 'handle_config_request')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
          name       'UserCommandService'
-         firstlineno 12
-         lnotab 0x0a0106090c0a0604060d0603
+         firstlineno 13
+         lnotab 0x0a0106090c0a0605060e0604
       'UserCommandService'
-   names      ('re', 'eras.agents.simple_llm', 'SimpleLLM', 'eras.config.config', 'config', 'eras.services.shell_command_service', 'ShellCommandService', 'openai', 'eras.services.user_config_service', 'UserConfigService', 'httpx', 'UserCommandService')
+   names      ('re', 'eras.agents.simple_llm', 'SimpleLLM', 'eras.config.config', 'config', 'eras.services.google_analytics', 'send_analytics_event', 'eras.services.shell_command_service', 'ShellCommandService', 'openai', 'eras.services.user_config_service', 'UserConfigService', 'httpx', 'UserCommandService')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020208020c010c010c0108020c010802
+   lnotab 0x00ff020208020c010c010c010c0108020c010802
```

### Comparing `eras-0.4.8/eras/services/__pycache__/user_config_service.cpython-311.pyc` & `eras-0.5.0/eras/services/__pycache__/user_config_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.5.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.5.0/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.5.0/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/llm_callable_functions/user_details.py` & `eras-0.5.0/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/shell_command_service.py` & `eras-0.5.0/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/services/user_config_service.py` & `eras-0.5.0/eras/services/user_config_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.5.0/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras/utils/env_vars_and_profile_files.py` & `eras-0.5.0/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.8/eras.egg-info/PKG-INFO` & `eras-0.5.0/eras.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.8
+Version: 0.5.0
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: InquirerPy==0.3.4
 Requires-Dist: colorama==0.4.6
+Requires-Dist: requests==2.31.0
+Requires-Dist: ga4mp==2.0.4
 
 # Unlock the Power of Your Terminal with ERAS 🚀
 Welcome to ERAS: the Easily Runnable AI Shell that revolutionizes your command-line experience. 
 
 Say goodbye to the hassle of searching for the right command syntax—ERAS transforms your natural language instructions into precise terminal commands instantly.
 
 ## Why ERAS?
```

### Comparing `eras-0.4.8/eras.egg-info/SOURCES.txt` & `eras-0.5.0/eras.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,20 @@
 eras/models/__pycache__/conversation.cpython-39.pyc
 eras/models/__pycache__/function_details.cpython-311.pyc
 eras/models/__pycache__/function_details.cpython-39.pyc
 eras/models/__pycache__/message.cpython-311.pyc
 eras/models/__pycache__/message.cpython-39.pyc
 eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
 eras/services/__init__.py
+eras/services/google_analytics.py
 eras/services/shell_command_service.py
 eras/services/user_command_service.py
 eras/services/user_config_service.py
 eras/services/__pycache__/__init__.cpython-311.pyc
+eras/services/__pycache__/google_analytics.cpython-311.pyc
 eras/services/__pycache__/shell_command_service.cpython-311.pyc
 eras/services/__pycache__/shell_command_service.cpython-39.pyc
 eras/services/__pycache__/user_command_service.cpython-311.pyc
 eras/services/__pycache__/user_config_service.cpython-311.pyc
 eras/services/llm_callable_functions/__init__.py
 eras/services/llm_callable_functions/callable_function_service_base.py
 eras/services/llm_callable_functions/terminal_command.py
```

### Comparing `eras-0.4.8/setup.py` & `eras-0.5.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.4.8',
+    version='0.5.0',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
         'openai==1.26.0',
         'keyboard==0.13.5',
         'python-dotenv==1.0.0',
         'asyncio==3.4.3',
         'InquirerPy==0.3.4',
-        'colorama==0.4.6'
+        'colorama==0.4.6',
+        'requests==2.31.0',
+        'ga4mp==2.0.4'
     ],
     entry_points={
         'console_scripts': [
             'eras=eras.main:main',
         ],
     },
     author='Jason McAffee',
```

