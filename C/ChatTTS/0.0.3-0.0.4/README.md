# Comparing `tmp/ChatTTS-0.0.3.tar.gz` & `tmp/ChatTTS-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatTTS-0.0.3.tar", last modified: Sat May 25 07:27:42 2024, max compression
+gzip compressed data, was "ChatTTS-0.0.4.tar", last modified: Mon May 27 03:01:04 2024, max compression
```

## Comparing `ChatTTS-0.0.3.tar` & `ChatTTS-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/ChatTTS/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-25 07:13:39.000000 ChatTTS-0.0.3/ChatTTS/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4503 2024-05-25 07:13:39.000000 ChatTTS-0.0.3/ChatTTS/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/ChatTTS/experimental/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:36.000000 ChatTTS-0.0.3/ChatTTS/experimental/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3124 2024-05-25 07:13:39.000000 ChatTTS-0.0.3/ChatTTS/experimental/llm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/ChatTTS/infer/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:41.000000 ChatTTS-0.0.3/ChatTTS/infer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4287 2024-05-25 07:27:05.000000 ChatTTS-0.0.3/ChatTTS/infer/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/ChatTTS/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:43.000000 ChatTTS-0.0.3/ChatTTS/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4958 2024-05-25 07:13:39.000000 ChatTTS-0.0.3/ChatTTS/model/dvae.py
--rw-r--r--   0 root         (0) root         (0)    11713 2024-05-25 07:13:39.000000 ChatTTS-0.0.3/ChatTTS/model/gpt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/ChatTTS/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:45.000000 ChatTTS-0.0.3/ChatTTS/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-05-25 07:13:39.000000 ChatTTS-0.0.3/ChatTTS/utils/gpu_utils.py
--rw-r--r--   0 root         (0) root         (0)     1733 2024-05-25 07:13:39.000000 ChatTTS-0.0.3/ChatTTS/utils/infer_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/ChatTTS.egg-info/
--rw-r--r--   0 root         (0) root         (0)      156 2024-05-25 07:27:41.000000 ChatTTS-0.0.3/ChatTTS.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-25 07:27:41.000000 ChatTTS-0.0.3/ChatTTS.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 07:27:41.000000 ChatTTS-0.0.3/ChatTTS.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-25 07:27:41.000000 ChatTTS-0.0.3/ChatTTS.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-25 07:27:41.000000 ChatTTS-0.0.3/ChatTTS.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      156 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 07:27:42.282091 ChatTTS-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-25 07:27:38.000000 ChatTTS-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 03:01:04.883869 ChatTTS-0.0.4/ChatTTS/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-25 07:13:39.000000 ChatTTS-0.0.4/ChatTTS/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2024-05-27 03:00:30.000000 ChatTTS-0.0.4/ChatTTS/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/ChatTTS/experimental/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:36.000000 ChatTTS-0.0.4/ChatTTS/experimental/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3124 2024-05-25 07:13:39.000000 ChatTTS-0.0.4/ChatTTS/experimental/llm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/ChatTTS/infer/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:41.000000 ChatTTS-0.0.4/ChatTTS/infer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2024-05-25 07:27:05.000000 ChatTTS-0.0.4/ChatTTS/infer/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/ChatTTS/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:43.000000 ChatTTS-0.0.4/ChatTTS/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2024-05-25 07:13:39.000000 ChatTTS-0.0.4/ChatTTS/model/dvae.py
+-rw-r--r--   0 root         (0) root         (0)    11713 2024-05-25 07:13:39.000000 ChatTTS-0.0.4/ChatTTS/model/gpt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/ChatTTS/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-25 07:26:45.000000 ChatTTS-0.0.4/ChatTTS/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-05-25 07:13:39.000000 ChatTTS-0.0.4/ChatTTS/utils/gpu_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2024-05-25 07:13:39.000000 ChatTTS-0.0.4/ChatTTS/utils/infer_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/ChatTTS.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      156 2024-05-27 03:01:04.000000 ChatTTS-0.0.4/ChatTTS.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-27 03:01:04.000000 ChatTTS-0.0.4/ChatTTS.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 03:01:04.000000 ChatTTS-0.0.4/ChatTTS.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-27 03:01:04.000000 ChatTTS-0.0.4/ChatTTS.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-27 03:01:04.000000 ChatTTS-0.0.4/ChatTTS.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 03:01:04.887869 ChatTTS-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-27 03:00:40.000000 ChatTTS-0.0.4/setup.py
```

### Comparing `ChatTTS-0.0.3/ChatTTS/core.py` & `ChatTTS-0.0.4/ChatTTS/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from omegaconf import OmegaConf
 
 import torch
 from vocos import Vocos
-from chattts.model.dvae import DVAE
-from chattts.model.gpt import GPT_warpper
-from chattts.utils.gpu_utils import select_device
-from chattts.infer.api import refine_text, infer_code
+from .model.dvae import DVAE
+from .model.gpt import GPT_warpper
+from .utils.gpu_utils import select_device
+from .infer.api import refine_text, infer_code
 
 logging.basicConfig(level = logging.INFO)
 
 
 class Chat:
     def __init__(self, ):
         self.pretrain_models = {}
```

### Comparing `ChatTTS-0.0.3/ChatTTS/experimental/llm.py` & `ChatTTS-0.0.4/ChatTTS/experimental/llm.py`

 * *Files identical despite different names*

### Comparing `ChatTTS-0.0.3/ChatTTS/infer/api.py` & `ChatTTS-0.0.4/ChatTTS/infer/api.py`

 * *Files identical despite different names*

### Comparing `ChatTTS-0.0.3/ChatTTS/model/dvae.py` & `ChatTTS-0.0.4/ChatTTS/model/dvae.py`

 * *Files identical despite different names*

### Comparing `ChatTTS-0.0.3/ChatTTS/model/gpt.py` & `ChatTTS-0.0.4/ChatTTS/model/gpt.py`

 * *Files identical despite different names*

### Comparing `ChatTTS-0.0.3/ChatTTS/utils/gpu_utils.py` & `ChatTTS-0.0.4/ChatTTS/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ChatTTS-0.0.3/ChatTTS/utils/infer_utils.py` & `ChatTTS-0.0.4/ChatTTS/utils/infer_utils.py`

 * *Files identical despite different names*

