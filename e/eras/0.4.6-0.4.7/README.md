# Comparing `tmp/eras-0.4.6.tar.gz` & `tmp/eras-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.4.6.tar", last modified: Sun May 26 03:49:41 2024, max compression
+gzip compressed data, was "eras-0.4.7.tar", last modified: Sun May 26 23:39:29 2024, max compression
```

## Comparing `eras-0.4.6.tar` & `eras-0.4.7.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.224416 eras-0.4.6/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.6/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.6/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:49:41.223845 eras-0.4.6/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.6/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.193261 eras-0.4.6/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.6/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.195542 eras-0.4.6/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.6/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.6/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.6/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.197445 eras-0.4.6/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.6/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.201115 eras-0.4.6/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.6/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.6/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.6/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.6/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.6/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.6/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.6/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.201923 eras-0.4.6/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.6/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.203126 eras-0.4.6/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.6/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.6/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.6/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.6/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.203732 eras-0.4.6/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.6/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.204434 eras-0.4.6/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.6/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.205381 eras-0.4.6/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.6/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.207369 eras-0.4.6/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.6/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.6/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.6/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.6/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.210399 eras-0.4.6/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.6/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.214741 eras-0.4.6/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.6/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.6/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.6/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.6/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.6/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.6/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.6/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.6/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.6/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.6/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.6/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.6/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.6/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.6/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.6/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.6/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.216284 eras-0.4.6/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.6/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.217747 eras-0.4.6/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.6/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.6/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7795 2024-05-26 03:46:21.000000 eras-0.4.6/eras/services/__pycache__/user_config_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.219398 eras-0.4.6/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.6/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.221845 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.6/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.6/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.6/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.6/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.6/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)    10789 2024-05-26 03:49:06.000000 eras-0.4.6/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.222456 eras-0.4.6/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.6/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.223168 eras-0.4.6/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.6/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.6/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.6/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:49:41.194827 eras-0.4.6/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)      102 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:49:41.000000 eras-0.4.6/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:49:41.224527 eras-0.4.6/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1093 2024-05-26 03:49:37.000000 eras-0.4.6/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.507256 eras-0.4.7/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.7/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.7/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     5512 2024-05-26 23:39:29.506688 eras-0.4.7/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4825 2024-05-26 23:35:26.000000 eras-0.4.7/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.471492 eras-0.4.7/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.7/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.473820 eras-0.4.7/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.7/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.7/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      818 2024-05-26 23:28:19.000000 eras-0.4.7/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.475869 eras-0.4.7/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.7/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.478774 eras-0.4.7/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.7/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.7/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.7/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.7/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.7/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.7/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.7/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.7/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.7/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.7/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.7/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.7/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.7/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.479638 eras-0.4.7/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.7/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.480880 eras-0.4.7/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.7/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.7/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.7/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.7/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.481792 eras-0.4.7/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.7/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.483024 eras-0.4.7/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.7/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.7/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.7/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.484699 eras-0.4.7/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.7/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.487211 eras-0.4.7/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.7/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.7/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.7/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.7/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.7/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.7/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.7/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-26 23:29:43.000000 eras-0.4.7/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.490749 eras-0.4.7/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.7/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.494732 eras-0.4.7/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.7/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.7/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.7/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.7/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.7/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.7/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.7/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.7/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.7/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.7/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.7/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.7/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.7/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.7/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.7/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-26 23:29:43.000000 eras-0.4.7/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.495941 eras-0.4.7/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.7/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.497917 eras-0.4.7/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.7/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2655 2024-05-26 23:28:19.000000 eras-0.4.7/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.7/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.7/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7863 2024-05-26 23:17:05.000000 eras-0.4.7/eras/services/__pycache__/user_config_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.499861 eras-0.4.7/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.7/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.503735 eras-0.4.7/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.7/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.7/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.7/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1987 2024-05-26 23:18:45.000000 eras-0.4.7/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.7/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)    10789 2024-05-26 03:49:06.000000 eras-0.4.7/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.504615 eras-0.4.7/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.7/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.505937 eras-0.4.7/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.7/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.7/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.7/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 23:39:29.472923 eras-0.4.7/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     5512 2024-05-26 23:39:29.000000 eras-0.4.7/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 23:39:29.000000 eras-0.4.7/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 23:39:29.000000 eras-0.4.7/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 23:39:29.000000 eras-0.4.7/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)      102 2024-05-26 23:39:29.000000 eras-0.4.7/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 23:39:29.000000 eras-0.4.7/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 23:39:29.507385 eras-0.4.7/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1093 2024-05-26 23:39:21.000000 eras-0.4.7/setup.py
```

### Comparing `eras-0.4.6/PKG-INFO` & `eras-0.4.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.6
+Version: 0.4.7
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,28 @@
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: InquirerPy==0.3.4
 Requires-Dist: colorama==0.4.6
 
-# ERAS
-Easily Runnable AI Shell allows you to run shell commands using natural language.   
+# Unlock the Power of Your Terminal with ERAS 🚀
+Welcome to ERAS: the Easily Runnable AI Shell that revolutionizes your command-line experience. 
 
-No more having to leave the terminal to look up how to run a command!
+Say goodbye to the hassle of searching for the right command syntax—ERAS transforms your natural language instructions into precise terminal commands instantly.
 
-Eras works on Windows, Mac, and Linux!
+## Why ERAS?
+- **Seamless Integration** : Compatible with Windows, Mac, and Linux, ERAS fits right into your workflow, regardless of your operating system. 🖥️
+- **Effortless Execution** : No more jumping between your terminal and browser. Just type what you need, and ERAS will do the rest. ⚡
+- **AI-Powered Precision** : Harness the power of OpenAI or any OpenAI-spec-compliant model like Llama.cpp server to ensure your commands are executed accurately and efficiently. 🤖
 
-Eras works with OpenAI, or any model exposed via an OpenAI spec compliant server, such as Llama.cpp server!
+Experience the future of terminal commands with ERAS and elevate your productivity today. 🌟
+
+
+![img_1.png](img_1.png)
 
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 # Install
@@ -63,14 +69,15 @@
 
 ![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
 ## Usage Examples
+
 ```
 % eras list all files in the current directory
 
 ERAS will then populate the next terminal line with the command:
 % ls
 
 All you have to do is confirm and hit enter!
```

### Comparing `eras-0.4.6/README.md` & `eras-0.4.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-# ERAS
-Easily Runnable AI Shell allows you to run shell commands using natural language.   
+# Unlock the Power of Your Terminal with ERAS 🚀
+Welcome to ERAS: the Easily Runnable AI Shell that revolutionizes your command-line experience. 
 
-No more having to leave the terminal to look up how to run a command!
+Say goodbye to the hassle of searching for the right command syntax—ERAS transforms your natural language instructions into precise terminal commands instantly.
 
-Eras works on Windows, Mac, and Linux!
+## Why ERAS?
+- **Seamless Integration** : Compatible with Windows, Mac, and Linux, ERAS fits right into your workflow, regardless of your operating system. 🖥️
+- **Effortless Execution** : No more jumping between your terminal and browser. Just type what you need, and ERAS will do the rest. ⚡
+- **AI-Powered Precision** : Harness the power of OpenAI or any OpenAI-spec-compliant model like Llama.cpp server to ensure your commands are executed accurately and efficiently. 🤖
 
-Eras works with OpenAI, or any model exposed via an OpenAI spec compliant server, such as Llama.cpp server!
+Experience the future of terminal commands with ERAS and elevate your productivity today. 🌟
+
+
+![img_1.png](img_1.png)
 
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 # Install
@@ -43,14 +49,15 @@
 
 ![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
 ## Usage Examples
+
 ```
 % eras list all files in the current directory
 
 ERAS will then populate the next terminal line with the command:
 % ls
 
 All you have to do is confirm and hit enter!
```

### Comparing `eras-0.4.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.4.7/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.4.7/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.4.7/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.4.7/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.4.7/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.4.7/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.4.7/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/llama_functions_agent.py` & `eras-0.4.7/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.4.7/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/llm_functions_agent.py` & `eras-0.4.7/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/simple_llm.py` & `eras-0.4.7/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/agents/terminal_llama_agent.py` & `eras-0.4.7/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.4.7/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.4.7/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/config/config.py` & `eras-0.4.7/eras/config/config.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.4.7/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/decorators/chatgpt_tool_data.py` & `eras-0.4.7/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.4.7/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.4.7/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.4.7/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.4.7/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/factories/function_details_factory.py` & `eras-0.4.7/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/factories/message_factory.py` & `eras-0.4.7/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/main.py` & `eras-0.4.7/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.4.7/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.4.7/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.4.7/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.4.7/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.4.7/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.4.7/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/conversation.py` & `eras-0.4.7/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/function_details.py` & `eras-0.4.7/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/message.py` & `eras-0.4.7/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/models/transaction.py` & `eras-0.4.7/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/run.ipynb` & `eras-0.4.7/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.4.7/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa6af4e66 (Thu May 23 02:53:26 2024 UTC)
-files sz: 1689
+moddate:  0x55c35366 (Sun May 26 23:18:45 2024 UTC)
+files sz: 1987
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -81,18 +81,18 @@
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (handle_prompt)
          
           23          28 LOAD_CONST               4 (<code object populate_terminal_with_shell_command, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 23>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (populate_terminal_with_shell_command)
          
-          26          34 LOAD_CONST               5 ('command')
+          34          34 LOAD_CONST               5 ('command')
                       36 LOAD_NAME                4 (str)
                       38 BUILD_TUPLE              2
-                      40 LOAD_CONST               6 (<code object run_shell_command, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 26>)
+                      40 LOAD_CONST               6 (<code object run_shell_command, file "/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py", line 34>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (run_shell_command)
                       46 LOAD_CONST               7 (None)
                       48 RETURN_VALUE
          consts
             'ShellCommandService'
             code
@@ -136,60 +136,66 @@
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d027c0264016b
-                  020000000072117405000000000000000000007c02a6010000ab01000000
-                  00000000000100640053007c00a003000000000000000000000000000000
-                  00000000007c02a6010000ab010000000000000000010064005300
+                  020000000073067c0264026b020000000072117405000000000000000000
+                  007c02a6010000ab0100000000000000000100640053007c00a003000000
+                  00000000000000000000000000000000007c02a6010000ab010000000000
+                  000000010064005300
                 14           0 RESUME                   0
                
                 15           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (llm_functions_agent)
                             14 LOAD_METHOD              1 (inference)
                             36 LOAD_FAST                1 (prompt)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (response)
                
                 16          54 LOAD_FAST                2 (response)
                             56 LOAD_CONST               1 ('No shell command can facilitate your request')
                             58 COMPARE_OP               2 (==)
-                            64 POP_JUMP_FORWARD_IF_FALSE    17 (to 100)
-               
-                17          66 LOAD_GLOBAL              5 (NULL + print)
-                            78 LOAD_FAST                2 (response)
-                            80 PRECALL                  1
-                            84 CALL                     1
-                            94 POP_TOP
-               
-                18          96 LOAD_CONST               0 (None)
-                            98 RETURN_VALUE
-               
-                21     >>  100 LOAD_FAST                0 (self)
-                           102 LOAD_METHOD              3 (populate_terminal_with_shell_command)
-                           124 LOAD_FAST                2 (response)
-                           126 PRECALL                  1
-                           130 CALL                     1
-                           140 POP_TOP
-                           142 LOAD_CONST               0 (None)
-                           144 RETURN_VALUE
+                            64 POP_JUMP_FORWARD_IF_TRUE     6 (to 78)
+                            66 LOAD_FAST                2 (response)
+                            68 LOAD_CONST               2 ('No shell command can facilitate your request.')
+                            70 COMPARE_OP               2 (==)
+                            76 POP_JUMP_FORWARD_IF_FALSE    17 (to 112)
+               
+                17     >>   78 LOAD_GLOBAL              5 (NULL + print)
+                            90 LOAD_FAST                2 (response)
+                            92 PRECALL                  1
+                            96 CALL                     1
+                           106 POP_TOP
+               
+                18         108 LOAD_CONST               0 (None)
+                           110 RETURN_VALUE
+               
+                21     >>  112 LOAD_FAST                0 (self)
+                           114 LOAD_METHOD              3 (populate_terminal_with_shell_command)
+                           136 LOAD_FAST                2 (response)
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 POP_TOP
+                           154 LOAD_CONST               0 (None)
+                           156 RETURN_VALUE
                consts
                   None
                   'No shell command can facilitate your request'
+                  'No shell command can facilitate your request.'
                names      ('llm_functions_agent', 'inference', 'print', 'populate_terminal_with_shell_command')
                varnames   ('self', 'prompt', 'response')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
                name       'handle_prompt'
                firstlineno 14
-               lnotab 0x020134010c011e010403
+               lnotab 0x0201340118011e010403
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c01a60100
@@ -228,86 +234,86 @@
                   00000000006a05000000000000000064027c02ac03a6060000ab06000000
                   00000000007d037c036a06000000000000000044005d137d04740f000000
                   000000000000007c046404ac05a6020000ab02000000000000000001008c
                   147c03a0080000000000000000000000000000000000000000a6000000ab
                   0000000000000000007d057c0564066b0300000000721b7c036a09000000
                   000000000044005d157d04740f000000000000000000007c046404ac05a6
                   020000ab02000000000000000001008c146400530064005300
-                26           0 RESUME                   0
+                34           0 RESUME                   0
                
-                27           2 LOAD_GLOBAL              0 (os)
+                35           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (path)
                             24 LOAD_METHOD              2 (expanduser)
                             46 LOAD_CONST               1 ('~')
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               2 (home_directory)
                
-                32          64 LOAD_GLOBAL              7 (NULL + subprocess)
+                40          64 LOAD_GLOBAL              7 (NULL + subprocess)
                             76 LOAD_ATTR                4 (Popen)
                             86 LOAD_FAST                1 (command)
                             88 LOAD_CONST               2 (True)
                             90 LOAD_GLOBAL              6 (subprocess)
                            102 LOAD_ATTR                5 (PIPE)
                            112 LOAD_GLOBAL              6 (subprocess)
                            124 LOAD_ATTR                5 (PIPE)
                            134 LOAD_CONST               2 (True)
                
-                33         136 LOAD_FAST                2 (home_directory)
+                41         136 LOAD_FAST                2 (home_directory)
                
-                32         138 KW_NAMES                 3
+                40         138 KW_NAMES                 3
                            140 PRECALL                  6
                            144 CALL                     6
                            154 STORE_FAST               3 (process)
                
-                36         156 LOAD_FAST                3 (process)
+                44         156 LOAD_FAST                3 (process)
                            158 LOAD_ATTR                6 (stdout)
                            168 GET_ITER
                        >>  170 FOR_ITER                19 (to 210)
                            172 STORE_FAST               4 (line)
                
-                37         174 LOAD_GLOBAL             15 (NULL + print)
+                45         174 LOAD_GLOBAL             15 (NULL + print)
                            186 LOAD_FAST                4 (line)
                            188 LOAD_CONST               4 ('')
                            190 KW_NAMES                 5
                            192 PRECALL                  2
                            196 CALL                     2
                            206 POP_TOP
                            208 JUMP_BACKWARD           20 (to 170)
                
-                40     >>  210 LOAD_FAST                3 (process)
+                48     >>  210 LOAD_FAST                3 (process)
                            212 LOAD_METHOD              8 (wait)
                            234 PRECALL                  0
                            238 CALL                     0
                            248 STORE_FAST               5 (return_code)
                
-                43         250 LOAD_FAST                5 (return_code)
+                51         250 LOAD_FAST                5 (return_code)
                            252 LOAD_CONST               6 (0)
                            254 COMPARE_OP               3 (!=)
                            260 POP_JUMP_FORWARD_IF_FALSE    27 (to 316)
                
-                44         262 LOAD_FAST                3 (process)
+                52         262 LOAD_FAST                3 (process)
                            264 LOAD_ATTR                9 (stderr)
                            274 GET_ITER
                        >>  276 FOR_ITER                21 (to 320)
                            278 STORE_FAST               4 (line)
                
-                45         280 LOAD_GLOBAL             15 (NULL + print)
+                53         280 LOAD_GLOBAL             15 (NULL + print)
                            292 LOAD_FAST                4 (line)
                            294 LOAD_CONST               4 ('')
                            296 KW_NAMES                 5
                            298 PRECALL                  2
                            302 CALL                     2
                            312 POP_TOP
                            314 JUMP_BACKWARD           20 (to 276)
                
-                43     >>  316 LOAD_CONST               0 (None)
+                51     >>  316 LOAD_CONST               0 (None)
                            318 RETURN_VALUE
                
-                44     >>  320 LOAD_CONST               0 (None)
+                52     >>  320 LOAD_CONST               0 (None)
                            322 RETURN_VALUE
                consts
                   None
                   '~'
                   True
                   ('shell', 'stdout', 'stderr', 'text', 'cwd')
                   ''
@@ -315,25 +321,25 @@
                   0
                names      ('os', 'path', 'expanduser', 'subprocess', 'Popen', 'PIPE', 'stdout', 'print', 'wait', 'stderr')
                varnames   ('self', 'command', 'home_directory', 'process', 'line', 'return_code')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
                name       'run_shell_command'
-               firstlineno 26
+               firstlineno 34
                lnotab 0x02013e05480102ff12041201240328030c01120124fe0401
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'str', 'handle_prompt', 'populate_terminal_with_shell_command', 'run_shell_command')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
          name       'ShellCommandService'
          firstlineno 8
-         lnotab 0x0a0106050c090603
+         lnotab 0x0a0106050c09060b
       'ShellCommandService'
    names      ('keyboard', 'eras.agents.terminal_llama_agent', 'TerminalLlamaAgent', 'eras.config.config', 'config', 'subprocess', 'os', 'ShellCommandService')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/services/shell_command_service.py'
    name       '<module>'
```

### Comparing `eras-0.4.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.4.7/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.4.7/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/__pycache__/user_config_service.cpython-311.pyc` & `eras-0.4.7/eras/services/__pycache__/user_config_service.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8ab05266 (Sun May 26 03:46:18 2024 UTC)
-files sz: 10761
+moddate:  0x32b15266 (Sun May 26 03:49:06 2024 UTC)
+files sz: 10789
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -560,162 +560,172 @@
                lnotab 0x02013001040124022a011e011e011e011e011e011e01
             code
                argcount  : 1
                nlocals   : 10
                stacksize : 8
                flags     : 3
                code
-                  0x870a97007400000000000000000000006a010000000000000000740000
-                  0000000000000000006a0200000000000000007400000000000000000000
-                  006a0300000000000000007400000000000000000000006a040000000000
-                  0000007400000000000000000000006a05000000000000000067057d0174
-                  0c000000000000000000006a0700000000000000007d0267006401a2017d
-                  03640284007c034400a6000000ab0000000000000000007d047411000000
-                  00000000000000640384007c044400a6000000ab000000000000000000a6
-                  010000ab0100000000000000008a0a880a6601640484087c044400a60000
-                  00ab0000000000000000007d0564057d0674130000000000000000000089
-                  0aa6010000ab01000000000000000044005d5e7d07741500000000000000
-                  0000007c05a6010000ab01000000000000000044005d475c0200007d087d
-                  097c067c017c087417000000000000000000007c01a6010000ab01000000
-                  00000000007a060000190000000000000000007c097c0719000000000000
-                  0000007a0000007c027a0000007a0d00007d067c08741700000000000000
-                  0000007c05a6010000ab01000000000000000064067a0a00006b00000000
-                  0072057c0664077a0d00007d068c487c0664087a0d00007d068c5f741900
-                  0000000000000000007c06a6010000ab0100000000000000000100640053
-                  00
+                  0x870a97007401000000000000000000006401ac02a6010000ab01000000
+                  000000000001007402000000000000000000006a02000000000000000074
+                  02000000000000000000006a030000000000000000740200000000000000
+                  0000006a0400000000000000007402000000000000000000006a05000000
+                  00000000007402000000000000000000006a06000000000000000067057d
+                  01740e000000000000000000006a0800000000000000007d0267006403a2
+                  017d03640484007c034400a6000000ab0000000000000000007d04741300
+                  000000000000000000640584007c044400a6000000ab0000000000000000
+                  00a6010000ab0100000000000000008a0a880a6601640684087c044400a6
+                  000000ab0000000000000000007d0564077d067415000000000000000000
+                  00890aa6010000ab01000000000000000044005d5e7d0774170000000000
+                  00000000007c05a6010000ab01000000000000000044005d475c0200007d
+                  087d097c067c017c087419000000000000000000007c01a6010000ab0100
+                  000000000000007a060000190000000000000000007c097c071900000000
+                  00000000007a0000007c027a0000007a0d00007d067c0874190000000000
+                  00000000007c05a6010000ab01000000000000000064087a0a00006b0000
+                  00000072057c0664097a0d00007d068c487c06640a7a0d00007d068c5f74
+                  1b000000000000000000007c06a6010000ab010000000000000000010064
+                  005300
                              0 MAKE_CELL               10 (max_lines)
                
                 74           2 RESUME                   0
                
-                86           4 LOAD_GLOBAL              0 (Fore)
-                            16 LOAD_ATTR                1 (LIGHTCYAN_EX)
-               
-                87          26 LOAD_GLOBAL              0 (Fore)
-                            38 LOAD_ATTR                2 (LIGHTBLUE_EX)
-               
-                88          48 LOAD_GLOBAL              0 (Fore)
-                            60 LOAD_ATTR                3 (LIGHTRED_EX)
-               
-                89          70 LOAD_GLOBAL              0 (Fore)
-                            82 LOAD_ATTR                4 (LIGHTYELLOW_EX)
-               
-                90          92 LOAD_GLOBAL              0 (Fore)
-                           104 LOAD_ATTR                5 (LIGHTMAGENTA_EX)
-               
-                85         114 BUILD_LIST               5
-                           116 STORE_FAST               1 (colors)
-               
-                92         118 LOAD_GLOBAL             12 (Style)
-                           130 LOAD_ATTR                7 (RESET_ALL)
-                           140 STORE_FAST               2 (RESET)
-               
-                94         142 BUILD_LIST               0
-                           144 LOAD_CONST               1 (('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            '))
-                           146 LIST_EXTEND              1
-                           148 STORE_FAST               3 (text_blocks)
-               
-               150         150 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 150>)
-                           152 MAKE_FUNCTION            0
-                           154 LOAD_FAST                3 (text_blocks)
-                           156 GET_ITER
-                           158 PRECALL                  0
-                           162 CALL                     0
-                           172 STORE_FAST               4 (lines)
-               
-               151         174 LOAD_GLOBAL             17 (NULL + max)
-                           186 LOAD_CONST               3 (<code object <genexpr>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 151>)
-                           188 MAKE_FUNCTION            0
-                           190 LOAD_FAST                4 (lines)
-                           192 GET_ITER
-                           194 PRECALL                  0
-                           198 CALL                     0
-                           208 PRECALL                  1
-                           212 CALL                     1
-                           222 STORE_DEREF             10 (max_lines)
-               
-               152         224 LOAD_CLOSURE            10 (max_lines)
-                           226 BUILD_TUPLE              1
-                           228 LOAD_CONST               4 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 152>)
-                           230 MAKE_FUNCTION            8 (closure)
-                           232 LOAD_FAST                4 (lines)
-                           234 GET_ITER
-                           236 PRECALL                  0
-                           240 CALL                     0
-                           250 STORE_FAST               5 (padded_blocks)
-               
-               154         252 LOAD_CONST               5 ('')
-                           254 STORE_FAST               6 (colored_output)
-               
-               156         256 LOAD_GLOBAL             19 (NULL + range)
-                           268 LOAD_DEREF              10 (max_lines)
-                           270 PRECALL                  1
-                           274 CALL                     1
-                           284 GET_ITER
-                       >>  286 FOR_ITER                94 (to 476)
-                           288 STORE_FAST               7 (i)
-               
-               157         290 LOAD_GLOBAL             21 (NULL + enumerate)
-                           302 LOAD_FAST                5 (padded_blocks)
-                           304 PRECALL                  1
-                           308 CALL                     1
-                           318 GET_ITER
-                       >>  320 FOR_ITER                71 (to 464)
-                           322 UNPACK_SEQUENCE          2
-                           326 STORE_FAST               8 (j)
-                           328 STORE_FAST               9 (block)
-               
-               158         330 LOAD_FAST                6 (colored_output)
-                           332 LOAD_FAST                1 (colors)
-                           334 LOAD_FAST                8 (j)
-                           336 LOAD_GLOBAL             23 (NULL + len)
-                           348 LOAD_FAST                1 (colors)
-                           350 PRECALL                  1
-                           354 CALL                     1
-                           364 BINARY_OP                6 (%)
-                           368 BINARY_SUBSCR
-                           378 LOAD_FAST                9 (block)
-                           380 LOAD_FAST                7 (i)
-                           382 BINARY_SUBSCR
-                           392 BINARY_OP                0 (+)
-                           396 LOAD_FAST                2 (RESET)
-                           398 BINARY_OP                0 (+)
-                           402 BINARY_OP               13 (+=)
-                           406 STORE_FAST               6 (colored_output)
-               
-               159         408 LOAD_FAST                8 (j)
-                           410 LOAD_GLOBAL             23 (NULL + len)
-                           422 LOAD_FAST                5 (padded_blocks)
-                           424 PRECALL                  1
-                           428 CALL                     1
-                           438 LOAD_CONST               6 (1)
-                           440 BINARY_OP               10 (-)
-                           444 COMPARE_OP               0 (<)
-                           450 POP_JUMP_FORWARD_IF_FALSE     5 (to 462)
-               
-               160         452 LOAD_FAST                6 (colored_output)
-                           454 LOAD_CONST               7 (' ')
-                           456 BINARY_OP               13 (+=)
-                           460 STORE_FAST               6 (colored_output)
-                       >>  462 JUMP_BACKWARD           72 (to 320)
-               
-               161     >>  464 LOAD_FAST                6 (colored_output)
-                           466 LOAD_CONST               8 ('\n')
-                           468 BINARY_OP               13 (+=)
-                           472 STORE_FAST               6 (colored_output)
-                           474 JUMP_BACKWARD           95 (to 286)
-               
-               163     >>  476 LOAD_GLOBAL             25 (NULL + print)
-                           488 LOAD_FAST                6 (colored_output)
-                           490 PRECALL                  1
-                           494 CALL                     1
-                           504 POP_TOP
-                           506 LOAD_CONST               0 (None)
-                           508 RETURN_VALUE
+                76           4 LOAD_GLOBAL              1 (NULL + init)
+                            16 LOAD_CONST               1 (True)
+                            18 KW_NAMES                 2
+                            20 PRECALL                  1
+                            24 CALL                     1
+                            34 POP_TOP
+               
+                86          36 LOAD_GLOBAL              2 (Fore)
+                            48 LOAD_ATTR                2 (LIGHTCYAN_EX)
+               
+                87          58 LOAD_GLOBAL              2 (Fore)
+                            70 LOAD_ATTR                3 (LIGHTBLUE_EX)
+               
+                88          80 LOAD_GLOBAL              2 (Fore)
+                            92 LOAD_ATTR                4 (LIGHTRED_EX)
+               
+                89         102 LOAD_GLOBAL              2 (Fore)
+                           114 LOAD_ATTR                5 (LIGHTYELLOW_EX)
+               
+                90         124 LOAD_GLOBAL              2 (Fore)
+                           136 LOAD_ATTR                6 (LIGHTMAGENTA_EX)
+               
+                85         146 BUILD_LIST               5
+                           148 STORE_FAST               1 (colors)
+               
+                92         150 LOAD_GLOBAL             14 (Style)
+                           162 LOAD_ATTR                8 (RESET_ALL)
+                           172 STORE_FAST               2 (RESET)
+               
+                94         174 BUILD_LIST               0
+                           176 LOAD_CONST               3 (('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            '))
+                           178 LIST_EXTEND              1
+                           180 STORE_FAST               3 (text_blocks)
+               
+               150         182 LOAD_CONST               4 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 150>)
+                           184 MAKE_FUNCTION            0
+                           186 LOAD_FAST                3 (text_blocks)
+                           188 GET_ITER
+                           190 PRECALL                  0
+                           194 CALL                     0
+                           204 STORE_FAST               4 (lines)
+               
+               151         206 LOAD_GLOBAL             19 (NULL + max)
+                           218 LOAD_CONST               5 (<code object <genexpr>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 151>)
+                           220 MAKE_FUNCTION            0
+                           222 LOAD_FAST                4 (lines)
+                           224 GET_ITER
+                           226 PRECALL                  0
+                           230 CALL                     0
+                           240 PRECALL                  1
+                           244 CALL                     1
+                           254 STORE_DEREF             10 (max_lines)
+               
+               152         256 LOAD_CLOSURE            10 (max_lines)
+                           258 BUILD_TUPLE              1
+                           260 LOAD_CONST               6 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 152>)
+                           262 MAKE_FUNCTION            8 (closure)
+                           264 LOAD_FAST                4 (lines)
+                           266 GET_ITER
+                           268 PRECALL                  0
+                           272 CALL                     0
+                           282 STORE_FAST               5 (padded_blocks)
+               
+               154         284 LOAD_CONST               7 ('')
+                           286 STORE_FAST               6 (colored_output)
+               
+               156         288 LOAD_GLOBAL             21 (NULL + range)
+                           300 LOAD_DEREF              10 (max_lines)
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 GET_ITER
+                       >>  318 FOR_ITER                94 (to 508)
+                           320 STORE_FAST               7 (i)
+               
+               157         322 LOAD_GLOBAL             23 (NULL + enumerate)
+                           334 LOAD_FAST                5 (padded_blocks)
+                           336 PRECALL                  1
+                           340 CALL                     1
+                           350 GET_ITER
+                       >>  352 FOR_ITER                71 (to 496)
+                           354 UNPACK_SEQUENCE          2
+                           358 STORE_FAST               8 (j)
+                           360 STORE_FAST               9 (block)
+               
+               158         362 LOAD_FAST                6 (colored_output)
+                           364 LOAD_FAST                1 (colors)
+                           366 LOAD_FAST                8 (j)
+                           368 LOAD_GLOBAL             25 (NULL + len)
+                           380 LOAD_FAST                1 (colors)
+                           382 PRECALL                  1
+                           386 CALL                     1
+                           396 BINARY_OP                6 (%)
+                           400 BINARY_SUBSCR
+                           410 LOAD_FAST                9 (block)
+                           412 LOAD_FAST                7 (i)
+                           414 BINARY_SUBSCR
+                           424 BINARY_OP                0 (+)
+                           428 LOAD_FAST                2 (RESET)
+                           430 BINARY_OP                0 (+)
+                           434 BINARY_OP               13 (+=)
+                           438 STORE_FAST               6 (colored_output)
+               
+               159         440 LOAD_FAST                8 (j)
+                           442 LOAD_GLOBAL             25 (NULL + len)
+                           454 LOAD_FAST                5 (padded_blocks)
+                           456 PRECALL                  1
+                           460 CALL                     1
+                           470 LOAD_CONST               8 (1)
+                           472 BINARY_OP               10 (-)
+                           476 COMPARE_OP               0 (<)
+                           482 POP_JUMP_FORWARD_IF_FALSE     5 (to 494)
+               
+               160         484 LOAD_FAST                6 (colored_output)
+                           486 LOAD_CONST               9 (' ')
+                           488 BINARY_OP               13 (+=)
+                           492 STORE_FAST               6 (colored_output)
+                       >>  494 JUMP_BACKWARD           72 (to 352)
+               
+               161     >>  496 LOAD_FAST                6 (colored_output)
+                           498 LOAD_CONST              10 ('\n')
+                           500 BINARY_OP               13 (+=)
+                           504 STORE_FAST               6 (colored_output)
+                           506 JUMP_BACKWARD           95 (to 318)
+               
+               163     >>  508 LOAD_GLOBAL             27 (NULL + print)
+                           520 LOAD_FAST                6 (colored_output)
+                           522 PRECALL                  1
+                           526 CALL                     1
+                           536 POP_TOP
+                           538 LOAD_CONST               0 (None)
+                           540 RETURN_VALUE
                consts
                   None
+                  True
+                  ('autoreset',)
                   ('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            ')
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
@@ -818,24 +828,24 @@
                      name       '<listcomp>'
                      firstlineno 152
                      lnotab 0x
                   ''
                   1
                   ' '
                   '\n'
-               names      ('Fore', 'LIGHTCYAN_EX', 'LIGHTBLUE_EX', 'LIGHTRED_EX', 'LIGHTYELLOW_EX', 'LIGHTMAGENTA_EX', 'Style', 'RESET_ALL', 'max', 'range', 'enumerate', 'len', 'print')
+               names      ('init', 'Fore', 'LIGHTCYAN_EX', 'LIGHTBLUE_EX', 'LIGHTRED_EX', 'LIGHTYELLOW_EX', 'LIGHTMAGENTA_EX', 'Style', 'RESET_ALL', 'max', 'range', 'enumerate', 'len', 'print')
                varnames   ('self', 'colors', 'RESET', 'text_blocks', 'lines', 'padded_blocks', 'colored_output', 'i', 'j', 'block')
                freevars   ()
                cellvars   ('max_lines',)
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                name       'print_eras_logo'
                firstlineno 74
                lnotab
-                  0x040c160116011601160116fb040718020838180132011c020402220128
-                  014e012c010c010c02
+                  0x0402200a160116011601160116fb040718020838180132011c02040222
+                  0128014e012c010c010c02
             None
             (True,)
          names      ('__name__', '__module__', '__qualname__', 'ensure_needed_configs_are_set', 'prompt_for_all_configs', 'reload_prof', 'show_commands', 'print_eras_logo')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
```

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.4.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.4.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.4.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.4.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.4.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.4.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.4.7/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.4.7/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/llm_callable_functions/user_details.py` & `eras-0.4.7/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/user_command_service.py` & `eras-0.4.7/eras/services/user_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/services/user_config_service.py` & `eras-0.4.7/eras/services/user_config_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.4.7/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras/utils/env_vars_and_profile_files.py` & `eras-0.4.7/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/eras.egg-info/PKG-INFO` & `eras-0.4.7/eras.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.6
+Version: 0.4.7
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,22 +14,28 @@
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: InquirerPy==0.3.4
 Requires-Dist: colorama==0.4.6
 
-# ERAS
-Easily Runnable AI Shell allows you to run shell commands using natural language.   
+# Unlock the Power of Your Terminal with ERAS 🚀
+Welcome to ERAS: the Easily Runnable AI Shell that revolutionizes your command-line experience. 
 
-No more having to leave the terminal to look up how to run a command!
+Say goodbye to the hassle of searching for the right command syntax—ERAS transforms your natural language instructions into precise terminal commands instantly.
 
-Eras works on Windows, Mac, and Linux!
+## Why ERAS?
+- **Seamless Integration** : Compatible with Windows, Mac, and Linux, ERAS fits right into your workflow, regardless of your operating system. 🖥️
+- **Effortless Execution** : No more jumping between your terminal and browser. Just type what you need, and ERAS will do the rest. ⚡
+- **AI-Powered Precision** : Harness the power of OpenAI or any OpenAI-spec-compliant model like Llama.cpp server to ensure your commands are executed accurately and efficiently. 🤖
 
-Eras works with OpenAI, or any model exposed via an OpenAI spec compliant server, such as Llama.cpp server!
+Experience the future of terminal commands with ERAS and elevate your productivity today. 🌟
+
+
+![img_1.png](img_1.png)
 
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 # Install
@@ -63,14 +69,15 @@
 
 ![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
 ## Usage Examples
+
 ```
 % eras list all files in the current directory
 
 ERAS will then populate the next terminal line with the command:
 % ls
 
 All you have to do is confirm and hit enter!
```

### Comparing `eras-0.4.6/eras.egg-info/SOURCES.txt` & `eras-0.4.7/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.4.6/setup.py` & `eras-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.4.6',
+    version='0.4.7',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

