# Comparing `tmp/unionllm-0.1.3.tar.gz` & `tmp/unionllm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unionllm-0.1.3.tar", last modified: Tue May 21 08:56:12 2024, max compression
+gzip compressed data, was "unionllm-0.1.4.tar", last modified: Mon May 27 03:40:01 2024, max compression
```

## Comparing `unionllm-0.1.3.tar` & `unionllm-0.1.4.tar`

### file list

```diff
@@ -1,72 +1,54 @@
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.278652 unionllm-0.1.3/
--rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 unionllm-0.1.3/LICENSE
--rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-21 08:56:12.278478 unionllm-0.1.3/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)     4978 2024-05-20 03:58:24.000000 unionllm-0.1.3/README.md
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.270245 unionllm-0.1.3/cookbook/
--rw-r--r--   0 everfly    (501) staff       (20)     1752 2024-05-12 16:23:53.000000 unionllm-0.1.3/cookbook/chat_with_zhipu.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)     8970 2024-05-08 17:11:35.000000 unionllm-0.1.3/cookbook/coze_non_stream.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)    11763 2024-05-12 22:37:43.000000 unionllm-0.1.3/cookbook/coze_non_stream_func.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)    82911 2024-05-12 09:05:55.000000 unionllm-0.1.3/cookbook/test_generation_by_coze_eval_by_chatglm_faithfulness.ipynb
--rw-r--r--   0 everfly    (501) staff       (20)    29653 2024-05-12 09:05:53.000000 unionllm-0.1.3/cookbook/test_zeval.ipynb
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.273575 unionllm-0.1.3/docs/
--rw-r--r--   0 everfly    (501) staff       (20)      926 2024-05-20 02:32:47.000000 unionllm-0.1.3/docs/baichuan.md
--rw-r--r--   0 everfly    (501) staff       (20)      967 2024-05-20 02:19:02.000000 unionllm-0.1.3/docs/baidu.md
--rw-r--r--   0 everfly    (501) staff       (20)      937 2024-05-20 02:47:22.000000 unionllm-0.1.3/docs/coze.md
--rw-r--r--   0 everfly    (501) staff       (20)      828 2024-05-20 02:51:27.000000 unionllm-0.1.3/docs/dify.md
--rw-r--r--   0 everfly    (501) staff       (20)      856 2024-05-20 02:48:50.000000 unionllm-0.1.3/docs/fastgpt.md
--rw-r--r--   0 everfly    (501) staff       (20)     5951 2024-05-20 03:39:58.000000 unionllm-0.1.3/docs/litellm.md
--rw-r--r--   0 everfly    (501) staff       (20)      872 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/minimax.md
--rw-r--r--   0 everfly    (501) staff       (20)      944 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/moonshot.md
--rw-r--r--   0 everfly    (501) staff       (20)      879 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/qwen.md
--rw-r--r--   0 everfly    (501) staff       (20)      976 2024-05-20 02:41:46.000000 unionllm-0.1.3/docs/tiangong.md
--rw-r--r--   0 everfly    (501) staff       (20)      816 2024-05-20 02:29:57.000000 unionllm-0.1.3/docs/xunfei.md
--rw-r--r--   0 everfly    (501) staff       (20)      884 2024-05-20 02:32:45.000000 unionllm-0.1.3/docs/zhipuai.md
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.273696 unionllm-0.1.3/examples/
--rw-r--r--   0 everfly    (501) staff       (20)       46 2024-05-08 02:19:48.000000 unionllm-0.1.3/examples/example_usage.py
--rw-r--r--   0 everfly    (501) staff       (20)      427 2024-05-21 08:55:32.000000 unionllm-0.1.3/pyproject.toml
--rw-r--r--   0 everfly    (501) staff       (20)      133 2024-05-12 14:58:23.000000 unionllm-0.1.3/pytest.ini
--rw-r--r--   0 everfly    (501) staff       (20)       95 2024-05-16 03:33:55.000000 unionllm-0.1.3/requirements.txt
--rw-r--r--   0 everfly    (501) staff       (20)       38 2024-05-21 08:56:12.278693 unionllm-0.1.3/setup.cfg
--rw-r--r--   0 everfly    (501) staff       (20)      563 2024-05-21 08:56:00.000000 unionllm-0.1.3/setup.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.275416 unionllm-0.1.3/tests/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.3/tests/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)     1409 2024-05-12 15:47:41.000000 unionllm-0.1.3/tests/test_baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     1403 2024-05-13 00:05:32.000000 unionllm-0.1.3/tests/test_coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     1423 2024-05-12 23:54:14.000000 unionllm-0.1.3/tests/test_dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     1406 2024-05-12 23:47:08.000000 unionllm-0.1.3/tests/test_fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     1137 2024-05-13 00:21:07.000000 unionllm-0.1.3/tests/test_litellm.py
--rw-r--r--   0 everfly    (501) staff       (20)     1422 2024-05-12 23:15:34.000000 unionllm-0.1.3/tests/test_minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     1407 2024-05-12 15:50:43.000000 unionllm-0.1.3/tests/test_moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     1377 2024-05-12 22:48:43.000000 unionllm-0.1.3/tests/test_qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     1457 2024-05-12 15:56:14.000000 unionllm-0.1.3/tests/test_tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     4838 2024-05-20 05:46:21.000000 unionllm-0.1.3/tests/test_unionchat.py
--rw-r--r--   0 everfly    (501) staff       (20)     1444 2024-05-12 16:01:29.000000 unionllm-0.1.3/tests/test_wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     1021 2024-05-12 16:19:20.000000 unionllm-0.1.3/tests/test_xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     1371 2024-05-12 22:47:46.000000 unionllm-0.1.3/tests/test_zhipu.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.276084 unionllm-0.1.3/unionllm/
--rw-r--r--   0 everfly    (501) staff       (20)       54 2024-05-20 14:04:18.000000 unionllm-0.1.3/unionllm/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)     5354 2024-05-19 08:13:23.000000 unionllm-0.1.3/unionllm/exceptions.py
--rw-r--r--   0 everfly    (501) staff       (20)     5104 2024-05-20 13:56:42.000000 unionllm-0.1.3/unionllm/main.py
--rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 unionllm-0.1.3/unionllm/models.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.278083 unionllm-0.1.3/unionllm/providers/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.3/unionllm/providers/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)     5579 2024-05-12 10:20:45.000000 unionllm-0.1.3/unionllm/providers/baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     3484 2024-05-16 03:12:50.000000 unionllm-0.1.3/unionllm/providers/base_provider.py
--rw-r--r--   0 everfly    (501) staff       (20)    10431 2024-05-14 02:35:52.000000 unionllm-0.1.3/unionllm/providers/coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     7740 2024-05-12 23:53:57.000000 unionllm-0.1.3/unionllm/providers/dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     7162 2024-05-14 02:35:50.000000 unionllm-0.1.3/unionllm/providers/fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     2119 2024-05-13 16:15:14.000000 unionllm-0.1.3/unionllm/providers/litellm.py
--rw-r--r--   0 everfly    (501) staff       (20)     5247 2024-05-12 22:57:26.000000 unionllm-0.1.3/unionllm/providers/minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2832 2024-05-13 16:15:40.000000 unionllm-0.1.3/unionllm/providers/moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     7055 2024-05-12 10:20:45.000000 unionllm-0.1.3/unionllm/providers/qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     6425 2024-05-12 16:00:03.000000 unionllm-0.1.3/unionllm/providers/tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     6891 2024-05-16 03:05:33.000000 unionllm-0.1.3/unionllm/providers/wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     9372 2024-05-12 10:04:56.000000 unionllm-0.1.3/unionllm/providers/xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     2533 2024-05-16 03:04:34.000000 unionllm-0.1.3/unionllm/providers/zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)    14331 2024-05-13 16:45:47.000000 unionllm-0.1.3/unionllm/utils.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-21 08:56:12.278254 unionllm-0.1.3/unionllm.egg-info/
--rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)     1440 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) staff       (20)        1 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) staff       (20)       84 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) staff       (20)       15 2024-05-21 08:56:12.000000 unionllm-0.1.3/unionllm.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-27 03:40:01.680416 unionllm-0.1.4/
+-rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 unionllm-0.1.4/LICENSE
+-rw-r--r--   0 everfly    (501) staff       (20)      469 2024-05-27 03:40:01.680246 unionllm-0.1.4/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)     5137 2024-05-27 03:28:24.000000 unionllm-0.1.4/README.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-27 03:40:01.676975 unionllm-0.1.4/docs/
+-rw-r--r--   0 everfly    (501) staff       (20)     1133 2024-05-27 03:37:12.000000 unionllm-0.1.4/docs/baichuan.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1414 2024-05-27 03:39:27.000000 unionllm-0.1.4/docs/baidu.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1109 2024-05-27 03:37:16.000000 unionllm-0.1.4/docs/coze.md
+-rw-r--r--   0 everfly    (501) staff       (20)      960 2024-05-27 03:37:18.000000 unionllm-0.1.4/docs/dify.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1007 2024-05-27 03:37:20.000000 unionllm-0.1.4/docs/fastgpt.md
+-rw-r--r--   0 everfly    (501) staff       (20)     5947 2024-05-27 03:38:05.000000 unionllm-0.1.4/docs/litellm.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1057 2024-05-27 03:37:40.000000 unionllm-0.1.4/docs/minimax.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1156 2024-05-27 03:37:41.000000 unionllm-0.1.4/docs/moonshot.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1156 2024-05-27 03:37:42.000000 unionllm-0.1.4/docs/qwen.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1205 2024-05-27 03:37:43.000000 unionllm-0.1.4/docs/tiangong.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1107 2024-05-27 03:37:47.000000 unionllm-0.1.4/docs/xunfei.md
+-rw-r--r--   0 everfly    (501) staff       (20)     1073 2024-05-27 03:37:53.000000 unionllm-0.1.4/docs/zhipuai.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-27 03:40:01.677072 unionllm-0.1.4/examples/
+-rw-r--r--   0 everfly    (501) staff       (20)       46 2024-05-08 02:19:48.000000 unionllm-0.1.4/examples/example_usage.py
+-rw-r--r--   0 everfly    (501) staff       (20)      419 2024-05-27 02:50:55.000000 unionllm-0.1.4/pyproject.toml
+-rw-r--r--   0 everfly    (501) staff       (20)      133 2024-05-12 14:58:23.000000 unionllm-0.1.4/pytest.ini
+-rw-r--r--   0 everfly    (501) staff       (20)       87 2024-05-27 02:50:07.000000 unionllm-0.1.4/requirements.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       38 2024-05-27 03:40:01.680454 unionllm-0.1.4/setup.cfg
+-rw-r--r--   0 everfly    (501) staff       (20)      545 2024-05-27 02:51:02.000000 unionllm-0.1.4/setup.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-27 03:40:01.677229 unionllm-0.1.4/tests/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.4/tests/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     4706 2024-05-27 03:14:07.000000 unionllm-0.1.4/tests/test_unionchat.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-27 03:40:01.677832 unionllm-0.1.4/unionllm/
+-rw-r--r--   0 everfly    (501) staff       (20)       54 2024-05-20 14:04:18.000000 unionllm-0.1.4/unionllm/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5354 2024-05-19 08:13:23.000000 unionllm-0.1.4/unionllm/exceptions.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5095 2024-05-26 16:36:40.000000 unionllm-0.1.4/unionllm/main.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 unionllm-0.1.4/unionllm/models.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-27 03:40:01.679850 unionllm-0.1.4/unionllm/providers/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.4/unionllm/providers/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5579 2024-05-12 10:20:45.000000 unionllm-0.1.4/unionllm/providers/baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     3484 2024-05-16 03:12:50.000000 unionllm-0.1.4/unionllm/providers/base_provider.py
+-rw-r--r--   0 everfly    (501) staff       (20)    10513 2024-05-27 03:33:54.000000 unionllm-0.1.4/unionllm/providers/coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7820 2024-05-27 03:29:16.000000 unionllm-0.1.4/unionllm/providers/dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7245 2024-05-27 03:29:12.000000 unionllm-0.1.4/unionllm/providers/fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2425 2024-05-26 16:36:29.000000 unionllm-0.1.4/unionllm/providers/litellm.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5247 2024-05-12 22:57:26.000000 unionllm-0.1.4/unionllm/providers/minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2832 2024-05-13 16:15:40.000000 unionllm-0.1.4/unionllm/providers/moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7055 2024-05-12 10:20:45.000000 unionllm-0.1.4/unionllm/providers/qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6425 2024-05-12 16:00:03.000000 unionllm-0.1.4/unionllm/providers/tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6891 2024-05-16 03:05:33.000000 unionllm-0.1.4/unionllm/providers/wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9372 2024-05-12 10:04:56.000000 unionllm-0.1.4/unionllm/providers/xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2533 2024-05-16 03:04:34.000000 unionllm-0.1.4/unionllm/providers/zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)    14331 2024-05-13 16:45:47.000000 unionllm-0.1.4/unionllm/utils.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-27 03:40:01.680025 unionllm-0.1.4/unionllm.egg-info/
+-rw-r--r--   0 everfly    (501) staff       (20)      469 2024-05-27 03:40:01.000000 unionllm-0.1.4/unionllm.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)      994 2024-05-27 03:40:01.000000 unionllm-0.1.4/unionllm.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) staff       (20)        1 2024-05-27 03:40:01.000000 unionllm-0.1.4/unionllm.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       77 2024-05-27 03:40:01.000000 unionllm-0.1.4/unionllm.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       15 2024-05-27 03:40:01.000000 unionllm-0.1.4/unionllm.egg-info/top_level.txt
```

### Comparing `unionllm-0.1.3/README.md` & `unionllm-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,25 +42,27 @@
 
 通过UnionLLM调用LiteLLM支持的任何其他模型的方式示例如下：
 ```python
 from unionllm import unionchat
 unionchat(provider="openai", model="gpt-4o", messages=[{"content": "你的开发者是谁？", "role": "user"}], stream=True)
 ```
 
-以下是stream=True的调用方式的增量格式示例：
+以下是stream=False的调用方式的返回格式示例：
 ```python
 ModelResponse(id='8635254124951169203', choices=[Choices(finish_reason='stop', index=0, message=Message(content='我是人工智能助手。', role='assistant'))], created=1715570856, model=model, object='chat.completion', system_fingerprint=None, usage=Usage(prompt_tokens=9, completion_tokens=27, total_tokens=36))
 ```
 
-以下是stream=False的调用方式的返回格式示例：
+以下是stream=True的调用方式的chunk增量格式示例：
 ```python
+......
 ModelResponse(id='8635254124951169203', choices=[Choices(finish_reason='stop', index=0, message=Message(content='我是人工智能助手。', role='assistant'))], created=1715570856, model=model, object='chat.completion', system_fingerprint=None, usage=Usage(prompt_tokens=9, completion_tokens=27, total_tokens=36))
+......
 ```
 
-UnionLLM的返回结果格式与LiteLLM一致且与OpenAI一致，并在此基础上扩展了Context信息的返回，以实现发起知识库检索的RAG调用时返回相关背景知识。
+UnionLLM的返回结果格式与LiteLLM一致且与OpenAI一致，并在此基础上扩展了Context信息的返回，以实现发起知识库检索的RAG调用时返回相关背景知识。(由于Coze, FastGPT和Dify的接口中返回背景信息的方式和格式经常改变，目前版本可能无法成功获取Context信息)
 
 以下是包含知识库检索背景信息的返回结果示例 (非流式调用)：
 ```python
 ModelResponse(id='8635254124951169203', choices=[Choices(finish_reason='stop', index=0, message=Message(content='我是人工智能助手。', role='assistant'))], created=1715570856, model=model, object='chat.completion', system_fingerprint=None, usage=Usage(prompt_tokens=9, completion_tokens=27, total_tokens=36),context=[Context(id=1, content='retrieved context information 1', score=0.96240234375), Context(id=2, content='retrieved context information 2', score=0.7978515625), Context(id=3, content='retrieved context information 3', score=0.71142578125)])
 ```
 
 以下是每一种大语言模型的调用方式的详细文档：
```

### Comparing `unionllm-0.1.3/docs/baichuan.md` & `unionllm-0.1.4/docs/xunfei.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-# 百川AI
+# 讯飞星火
 
-## 设置API KEYS
+## 通过环境变量设置调用鉴权参数
 
-```
+```python
 import os 
-os.environ["BAICHUAN_API_KEY"] = "your-baichuan-api-key"
+os.environ["XUNFEI_APP_ID"] = "your-app-id"
+os.environ["XUNFEI_API_KEY"] = "your-api-key"
+os.environ["XUNFEI_API_SECRET"] = "your-api-secret"
 ```
 
-## 非流式调用
+### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="baichuan",
-    model="Baichuan2-Turbo", 
+response = unionchat(
+    provider="xunfei",
+    model="generalv3.5", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 ```
 
-## 流式调用
-
-```python
-from unionllm import unionchat
-
-## set ENV variables
-os.environ["COHERE_API_KEY"] = "cohere key"
-
-# model call
-response = completion(
-    provider="baichuan",
-    model="Baichuan2-Turbo", 
-    messages = [{ "content": "Hello, how are you?","role": "user"}]
-)
+### 流式调用
 
-print(response)
-```
+暂不支持
 
-## 直接传入API_Key调用
+## 直接传入鉴权参数调用
 
 ```python
 # model call
-response = completion(
-    provider="baichuan",
-    model="Baichuan2-Turbo", 
-    api_key="your-baichuan-api-key",
+response = unionchat(
+    provider="xunfei",
+    model="generalv3.5", 
+    app_id="your-app-id",
+    api_key="your-api-key",
+    api_secret="your-api-secret",
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 for chunk in response:
     print(chunk)
+```
+
+## 支持模型
+
+|模型名称|传入model参数名称|
+|---|---|
+|Spark3.5 Max|generalv3.5|
+|Spark Pro|generalv3|
+|Spark V2.0|generalv2|
+|Spark Lite|general|
+
+## 参考文档：
+- [API调用](https://www.xfyun.cn/doc/spark/Web.html)
+- [模型价格](https://xinghuo.xfyun.cn/sparkapi)
 ```
```

### Comparing `unionllm-0.1.3/docs/baidu.md` & `unionllm-0.1.4/docs/dify.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-# 百度文心一言
+# Dify
 
-## 通过环境变量设置调用参数
+## 通过环境变量设置鉴权参数
 
-```python
+```
 import os 
-os.environ["ERNIE_CLIENT_ID"] = "your-client-id"
-os.environ["ERNIE_CLIENT_SECRET"] = "your-client-secret"
+os.environ["DIFY_API_KEY"] = "your-dify-api-key"
 ```
 
-## 非流式调用
+### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="wenxin",
-    model="ERNIE-3.5-8K", 
+response = unionchat(
+    provider="dify",
+    model="dify", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
+
+print(response)
 ```
 
-## 流式调用
+### 流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="wenxin",
-    model="ERNIE-3.5-8K", 
+response = unionchat(
+    provider="dify",
+    model="dify", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
-print(response)
+for chunk in response:
+    print(chunk)
 ```
 
-## 直接传入API_Key调用
+## 直接传入鉴权参数调用
 
 ```python
 # model call
-response = completion(
-    provider="wenxin",
-    model="ERNIE-3.5-8K", 
-    client_id="your-client-id",
-    client_secret="your-client-secret",
+response = unionchat(
+    provider="dify",
+    model="dify", 
+    api_key="your-dify-api-key",
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
+```
 
-for chunk in response:
-    print(chunk)
-```
+## 注意事项
+- model参数没有实际作用，可以传入任意字符串
+- Dify的API key可以在每个Bot的设置页面找到
```

### Comparing `unionllm-0.1.3/docs/fastgpt.md` & `unionllm-0.1.4/docs/moonshot.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,62 @@
-# FASTGPT
+# 月之暗面 Moonshot
 
-## 通过环境变量设置鉴权参数
+## 通过环境变量设置调用参数
 
-```
+```python
 import os 
-os.environ["FASTGPT_API_KEY"] = "your-fastgpt-api-key"
+os.environ["MOONSHOT_API_KEY"] = "your-moonshot-api-key"
 ```
 
-## 非流式调用
+### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="fastgpt",
-    model="fastgpt", 
+response = unionchat(
+    provider="moonshot",
+    model="moonshot-v1-32k", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
-
-print(response)
 ```
 
-## 流式调用
+### 流式调用
 
 ```python
 from unionllm import unionchat
 
+## set ENV variables
+os.environ["COHERE_API_KEY"] = "cohere key"
+
 # model call
-response = completion(
-    provider="fastgpt",
-    model="fastgpt", 
+response = unionchat(
+    provider="moonshot",
+    model="moonshot-v1-32k", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
-for chunk in response:
-    print(chunk)
+print(response)
 ```
 
-## 直接传入鉴权参数调用
+## 直接传入API_Key调用
 
 ```python
 # model call
-response = completion(
-    provider="fastgpt",
-    model="fastgpt", 
-    app_key="your-fastgpt-api-key",
+response = unionchat(
+    provider="moonshot",
+    model="moonshot-v1-32k", 
+    api_key="your-moonsho-api-key",
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
+
+for chunk in response:
+    print(chunk)
+```
+
+## 支持模型
+支持Moonshot的所有模型
+
+参考文档：
+- [API调用](https://platform.moonshot.cn/docs/api-reference)
+- [模型价格](https://platform.moonshot.cn/docs/pricing)
 ```
```

### Comparing `unionllm-0.1.3/docs/litellm.md` & `unionllm-0.1.4/docs/litellm.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,58 +39,58 @@
 
 ### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
+response = unionchat(
     provider="mistral",
     model="mistral-tiny", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 print(response)
 ```
 
 ### 流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
+response = unionchat(
     provider="mistral",
     model="mistral-tiny", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 for chunk in response:
     print(chunk)
 ```
 
 ## 直接传入鉴权参数调用
 
 ```python
 # model call
-response = completion(
+response = unionchat(
     provider="mistral",
     model="mistral-tiny", 
     app_key="your-mistral-api-key",
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 ```
 
 ## 兼容不传入provider参数的调用方式
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
+response = unionchat(
     model="mistral/mistral-tiny", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 ```
 
 如果你选择传入provider参数，以下是LiteLLM支持厂商的provider列表：
```

### Comparing `unionllm-0.1.3/docs/minimax.md` & `unionllm-0.1.4/docs/tiangong.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,61 @@
-# Minimax
+# 昆仑天工
 
 ## 通过环境变量设置调用参数
 
-```python
+```
 import os 
-os.environ["MINIMAX_API_KEY"] = "your-minimax-api-key"
+os.environ["TIANGONG_APP_KEY"] = "your-tiangong-app-key"
+os.environ["TIANGONG_APP_SECRET"] = "your-tiangong-app-secret"
 ```
 
-## 非流式调用
+### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="minimax",
-    model="abab5.5-chat", 
+response = unionchat(
+    provider="tiangong",
+    model="SkyChat-MegaVerse", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 ```
 
-## 流式调用
+### 流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="minimax",
-    model="abab5.5-chat", 
+response = unionchat(
+    provider="tiangong",
+    model="SkyChat-MegaVerse", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 print(response)
 ```
 
-## 直接传入API_Key调用
+## 接口直接传入鉴权参数调用
 
 ```python
 # model call
-response = completion(
-    apk_key="your-minimax-api-key",
-    provider="minimax",
-    model="abab5.5-chat", 
+response = unionchat(
+    provider="tiangong",
+    model="SkyChat-MegaVerse", 
+    app_key="your-baichuan-api-key",
+    app_secret="your-baichuan-api-secret",
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 for chunk in response:
     print(chunk)
+```
+
+## 支持模型
+支持天工的所有文本模型
+
+参考文档：
+- [API调用](https://model-platform.tiangong.cn/api-reference)
+- [模型价格](https://model-platform.tiangong.cn/pricing)
 ```
```

### Comparing `unionllm-0.1.3/docs/qwen.md` & `unionllm-0.1.4/docs/qwen.md`

 * *Files 27% similar despite different names*

```diff
@@ -3,49 +3,57 @@
 ## 通过环境变量设置调用参数
 
 ```python
 import os 
 os.environ["DASHSCOPE_API_KEY"] = "your-dashscope-api-key"
 ```
 
-## 非流式调用
+### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
+response = unionchat(
     provider="qwen",
     model="qwen-turbo", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 ```
 
-## 流式调用
+### 流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
+response = unionchat(
     provider="qwen",
     model="qwen-turbo", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 print(response)
 ```
 
 ## 直接传入API_Key调用
 
 ```python
 # model call
-response = completion(
+response = unionchat(
     apk_key="your-dashscope-api-key",
     provider="qwen",
     model="qwen-turbo", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 for chunk in response:
     print(chunk)
+```
+
+## 支持模型
+支持通义千问的所有模型
+
+参考文档：
+- [API调用](https://help.aliyun.com/zh/dashscope/developer-reference/api-details)
+- [模型价格](https://help.aliyun.com/zh/dashscope/developer-reference/tongyi-thousand-questions-metering-and-billing)
 ```
```

### Comparing `unionllm-0.1.3/docs/tiangong.md` & `unionllm-0.1.4/docs/coze.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-# 昆仑天工
+# Coze (海外版)
 
-## 设置API KEYS
+## 通过环境变量设置鉴权参数
 
 ```
 import os 
-os.environ["TIANGONG_APP_KEY"] = "your-tiangong-app-key"
-os.environ["TIANGONG_APP_SECRET"] = "your-tiangong-app-secret"
+os.environ["COZE_API_KEY"] = "your-coze-api-key"
+os.environ["COZE_BOT_ID"] = "your-coze-bot-id"
 ```
 
-## 非流式调用
+### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="tiangong",
-    model="SkyChat-MegaVerse", 
+response = unionchat(
+    provider="coze",
+    model="coze", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
+
+print(response)
 ```
 
-## 流式调用
+### 流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
+response = unionchat(
     provider="tiangong",
     model="SkyChat-MegaVerse", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
-print(response)
+for chunk in response:
+    print(chunk)
 ```
 
-## 直接传入API_Key调用
+## 直接传入鉴权参数调用
 
 ```python
 # model call
-response = completion(
-    provider="tiangong",
-    model="SkyChat-MegaVerse", 
-    app_key="your-baichuan-api-key",
-    app_secret="your-baichuan-api-secret",
+response = unionchat(
+    provider="coze",
+    model="coze", 
+    api_key="your-coze-api-key",
+    bot_id="your-coze-bot-id",
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
+```
 
-for chunk in response:
-    print(chunk)
-```
+## 注意事项
+- model参数没有实际作用，可以传入任意字符串
+- Coze API的参考文档：https://www.coze.com/docs/developer_guides/coze_api_overview?_lang=zh
```

### Comparing `unionllm-0.1.3/docs/xunfei.md` & `unionllm-0.1.4/docs/fastgpt.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,55 @@
-# 讯飞星火
+# FASTGPT
 
-## 通过环境变量设置调用鉴权参数
+## 通过环境变量设置鉴权参数
 
-```python
+```
 import os 
-os.environ["XUNFEI_APP_ID"] = "your-app-id"
-os.environ["XUNFEI_API_KEY"] = "your-api-key"
-os.environ["XUNFEI_API_SECRET"] = "your-api-secret"
+os.environ["FASTGPT_API_KEY"] = "your-fastgpt-api-key"
 ```
 
-## 非流式调用
+### 非流式调用
 
 ```python
 from unionllm import unionchat
 
 # model call
-response = completion(
-    provider="xunfei",
-    model="generalv3.5", 
+response = unionchat(
+    provider="fastgpt",
+    model="fastgpt", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
-```
-
-## 流式调用
 
-暂不支持
+print(response)
+```
 
-## 直接传入鉴权参数调用
+### 流式调用
 
 ```python
+from unionllm import unionchat
+
 # model call
-response = completion(
-    provider="xunfei",
-    model="generalv3.5", 
-    app_id="your-app-id",
-    api_key="your-api-key",
-    api_secret="your-api-secret",
+response = unionchat(
+    provider="fastgpt",
+    model="fastgpt", 
     messages = [{ "content": "Hello, how are you?","role": "user"}]
 )
 
 for chunk in response:
     print(chunk)
-```
+```
+
+## 接口直接传入鉴权参数调用
+
+```python
+# model call
+response = unionchat(
+    provider="fastgpt",
+    model="fastgpt", 
+    api_key="your-fastgpt-api-key",
+    messages = [{ "content": "Hello, how are you?","role": "user"}]
+)
+```
+
+## 注意事项
+- model参数没有实际作用，可以传入任何字符串
+- FastGPT的API密钥可以在每个Bot的发布应用页面找到
```

### Comparing `unionllm-0.1.3/setup.py` & `unionllm-0.1.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='unionllm',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     license='MIT',
     description='A Python library for unified access to Chinese domestic large language models.',
     author='everfly',
     author_email='tagriver@gmail.com',
     url='https://github.com/EvalsOne/UnionLLM',
     install_requires=[
         'openai',
         'pydantic',
         'zhipuai',
         'tenacity',
         'dashscope',
         'websocket_client',
         'requests',
-        'pytest',
         'litellm'
     ],
 )
```

### Comparing `unionllm-0.1.3/tests/test_unionchat.py` & `unionllm-0.1.4/tests/test_unionchat.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from dotenv import load_dotenv
 load_dotenv()
 
 # 将项目根目录添加到sys.path中
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
 from unionllm.exceptions import ProviderError
-from unionllm import unionchat  # 确保引入你的模块和函数
-from unionllm.utils import ModelResponse, Message, Choices, Usage, Context  # 确保引入ModelResponse
+from unionllm import unionchat
+from unionllm.utils import ModelResponse, Message, Choices, Usage, Context
 
 common_messages = [{"content": "你的开发者是谁？", "role": "user"}]
 
 @pytest.mark.parametrize("provider, model, messages, expected_exception, stream_mode", [
     # non stream mode
     ("azure", "azure/gpt-35-turbo", common_messages, None, False),
     ("zhipuai", "glm-4", common_messages, None, False),
@@ -23,36 +23,35 @@
     ("moonshot", "moonshot-v1-8k", common_messages, None, False),
     ("minimax", "abab5.5-chat", common_messages, None, False),
     ("baichuan", "Baichuan2-Turbo", common_messages, None, False),
     ("xunfei", "generalv3", common_messages, None, False),
     ("coze", "coze", common_messages, None, False),
     ("dify", "dify", common_messages, None, False),
     ("fastgpt", "fastgpt", common_messages, None, False),    
-    # {"ollama", "ollama/llama3", common_messages, None, False}
+    {"ollama", "ollama/llama3", common_messages, None, False}
     ("mistral", "mistral-large-latest", common_messages, None, False),
     ("cohere", "command-r", common_messages, None, False),
     ("groq", "groq/mixtral-8x7b-32768", common_messages, None, False),
     ("bedrock", "ai21.j2-ultra-v1", common_messages, None, False),
-    # ("", "groq/mixtral-8x7b-32768", common_messages, None, False), #no provider case
+    ("", "groq/mixtral-8x7b-32768", common_messages, None, False), #no provider case
     ("nonexistent", "model", common_messages, ProviderError, False),
     # stream mode
     ("azure", "azure/gpt-35-turbo", common_messages, None, True),
     ("zhipuai", "glm-4", common_messages, None, True),
     ("nonexistent", "model", common_messages, ProviderError, True),
     ("tiangong", "SkyChat-MegaVerse", common_messages, None, True),
     ("wenxin", "ERNIE-3.5-8K", common_messages, None, True),
     ("qwen", "qwen-plus", common_messages, None, True),
     ("moonshot", "moonshot-v1-8k", common_messages, None, True),
     ("minimax", "abab5.5-chat", common_messages, None, True),
     ("baichuan", "Baichuan2-Turbo", common_messages, None, True),
-    # ("xunfei", "generalv3", common_messages, None, True),
     ("coze", "coze", common_messages, None, True),
     ("dify", "dify", common_messages, None, True),
     ("fastgpt", "fastgpt", common_messages, None, True),    
-    # {"ollama", "ollama/llama3", common_messages, None, False}
+    {"ollama", "ollama/llama3", common_messages, None, False}
     ("mistral", "mistral-large-latest", common_messages, None, True),
     ("cohere", "command-r", common_messages, None, True),
     ("groq", "groq/mixtral-8x7b-32768", common_messages, None, True),
     ("bedrock", "ai21.j2-ultra-v1", common_messages, None, True),
     ("nonexistent", "model", common_messages, ProviderError, True),
 ])
```

### Comparing `unionllm-0.1.3/unionllm/exceptions.py` & `unionllm-0.1.4/unionllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/main.py` & `unionllm-0.1.4/unionllm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
             self.provider_instance = litellm.LiteLLMProvider(**kwargs)
 
 
 
     def completion(self, model: str, messages: List[str], **kwargs) -> Any:
         if not self.provider_instance:
             raise ProviderError(f"Provider '{self.provider}' is not initialized.")
-        
         if self.litellm_call_type:
             if self.litellm_call_type == 1:
                 # Jugde whether the model starts with self.provider, if not, add it
                 if not model.startswith(self.provider+"/"):
                     model = f"{self.provider}/{model}"
                 return self.provider_instance.completion(model, messages, **kwargs)
             elif self.litellm_call_type == 2:
```

### Comparing `unionllm-0.1.3/unionllm/models.py` & `unionllm-0.1.4/unionllm/models.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/baichuan.py` & `unionllm-0.1.4/unionllm/providers/baichuan.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/base_provider.py` & `unionllm-0.1.4/unionllm/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/coze.py` & `unionllm-0.1.4/unionllm/providers/coze.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,13 +229,15 @@
                 payload = json.dumps({"query": query,"user": user_id,"bot_id": self.bot_id,"chat_history":history,"steam":False})
 
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
                 }
                 result = requests.post(self.endpoint_url, headers=headers, data=payload)
+                # print("CozeAI response")
+                # print(result.json())
                 return self.create_model_response_wrapper(result, model=model)
         except Exception as e:
             if hasattr(e, "status_code"):
                 raise CozeAIError(status_code=e.status_code, message=str(e))
             else:
                 raise CozeAIError(status_code=500, message=str(e))
```

### Comparing `unionllm-0.1.3/unionllm/providers/dify.py` & `unionllm-0.1.4/unionllm/providers/dify.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,13 +179,15 @@
 
                 payload = json.dumps({"query": query, "response_mode": mode, "user": "abc-123","conversation_id": "","inputs":{}})
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
                 }
                 result = requests.post(self.endpoint_url, headers=headers, data=payload)
+                # print("Dify response")
+                # print(result.json())
                 return self.create_model_response_wrapper(result, model=model)
         except Exception as e:
             if hasattr(e, "status_code"):
                 raise DifyOpenAIError(status_code=e.status_code, message=str(e))
             else:
                 raise DifyOpenAIError(status_code=500, message=str(e))
```

### Comparing `unionllm-0.1.3/unionllm/providers/fastgpt.py` & `unionllm-0.1.4/unionllm/providers/fastgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,13 +161,15 @@
             else:
                 payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
                 }
                 result = requests.post(self.endpoint_url, headers=headers, data=payload)
+                # print("fastgpt response")
+                # print(result.json())
                 return self.create_model_response_wrapper(result)
         except Exception as e:
             if hasattr(e, "status_code"):
                 raise FastGPTError(status_code=e.status_code, message=str(e))
             else:
                 raise FastGPTError(status_code=500, message=str(e))
```

### Comparing `unionllm-0.1.3/unionllm/providers/litellm.py` & `unionllm-0.1.4/unionllm/providers/litellm.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,39 +17,42 @@
     def __init__(self, **model_kwargs):
         pass
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
-            "best_of", "logit_bias"
+            "best_of", "logit_bias", "api_key", "api_secret", "api_url", "provider", "api_version", "api_base"
         ]
         for key in list(kwargs.keys()):
             if key not in supported_params:
-                kwargs.pop(key)
+                # kwargs.pop(key) # This line is commented out to avoid removing the key from the kwargs
+                pass
         return kwargs
 
     def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
         result = completion(
             model=model, messages=messages, **new_kwargs
         )
         return self.post_stream_processing(result)
 
     def create_model_response_wrapper(self, result, model):
         return self.create_model_response(result, model=model)
 
     def completion(self, model: str, messages: list, **kwargs):
         try:
+            if 'provider' in kwargs:
+                print("Litellm provider", kwargs['provider'])
+                kwargs.pop('provider')
             if model is None or messages is None:
                 raise LiteLLMError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
             stream = kwargs.get("stream", False)
-
             if stream:
                 return self.post_stream_processing_wrapper(model=model, messages=messages, **new_kwargs)
             else:
                 result = completion(
                     model=model, messages=messages, **new_kwargs
                 )
                 return self.create_model_response_wrapper(result, model=model)
```

### Comparing `unionllm-0.1.3/unionllm/providers/minimax.py` & `unionllm-0.1.4/unionllm/providers/minimax.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/moonshot.py` & `unionllm-0.1.4/unionllm/providers/moonshot.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/qwen.py` & `unionllm-0.1.4/unionllm/providers/qwen.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/tiangong.py` & `unionllm-0.1.4/unionllm/providers/tiangong.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/wenxin.py` & `unionllm-0.1.4/unionllm/providers/wenxin.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/xunfei.py` & `unionllm-0.1.4/unionllm/providers/xunfei.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/providers/zhipu.py` & `unionllm-0.1.4/unionllm/providers/zhipu.py`

 * *Files identical despite different names*

### Comparing `unionllm-0.1.3/unionllm/utils.py` & `unionllm-0.1.4/unionllm/utils.py`

 * *Files identical despite different names*

