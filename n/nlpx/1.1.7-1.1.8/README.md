# Comparing `tmp/nlpx-1.1.7.tar.gz` & `tmp/nlpx-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.7.tar", last modified: Sun May 26 05:47:47 2024, max compression
+gzip compressed data, was "nlpx-1.1.8.tar", last modified: Sun May 26 06:16:47 2024, max compression
```

## Comparing `nlpx-1.1.7.tar` & `nlpx-1.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.962214 nlpx-1.1.7/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 05:47:47.961166 nlpx-1.1.7/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.7/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.940409 nlpx-1.1.7/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.7/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.949961 nlpx-1.1.7/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.7/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5102 2024-05-26 05:21:03.000000 nlpx-1.1.7/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.7/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.954087 nlpx-1.1.7/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.7/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.7/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.958375 nlpx-1.1.7/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.1.7/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25392 2024-05-26 05:41:52.000000 nlpx-1.1.7/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.1.7/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.7/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.944349 nlpx-1.1.7/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-26 05:47:47.962702 nlpx-1.1.7/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-26 05:47:41.000000 nlpx-1.1.7/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.959548 nlpx-1.1.7/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.7/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.641691 nlpx-1.1.8/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 06:16:47.641021 nlpx-1.1.8/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.8/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.610599 nlpx-1.1.8/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.8/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.620885 nlpx-1.1.8/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.8/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5102 2024-05-26 05:21:03.000000 nlpx-1.1.8/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.8/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.627246 nlpx-1.1.8/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.8/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.8/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.636893 nlpx-1.1.8/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.1.8/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.1.8/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.1.8/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.8/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.615407 nlpx-1.1.8/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-26 06:16:47.000000 nlpx-1.1.8/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-26 06:16:47.642005 nlpx-1.1.8/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-26 06:16:42.000000 nlpx-1.1.8/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 06:16:47.639640 nlpx-1.1.8/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.8/test/test.py
```

### Comparing `nlpx-1.1.7/PKG-INFO` & `nlpx-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.7
+Version: 1.1.8
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.7/nlpx/llm/_model_wrapper.py` & `nlpx-1.1.8/nlpx/llm/_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.7/nlpx/llm/_tokenize_vec.py` & `nlpx-1.1.8/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.7/nlpx/models/_text_cnn.py` & `nlpx-1.1.8/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.7/nlpx/text_token/_tokenizer.py` & `nlpx-1.1.8/nlpx/text_token/_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import torch
 from pathlib import Path
 from typing import Union, Iterable
+from torch.nn import Embedding
 
 from ._utils import UTF8, read_file, read_corpus_files, batch_cut, token_counter, batch_pad_mask, cut, batch_pad, pad,\
     pad_mask, load_embedding
 
 
 # -------------------------------------------------Tokenizer class-----------------------------------------------------
 class BaseTokenizer:
@@ -351,15 +353,19 @@
             raise ValueError('参数"path"为空的情况下，"vocab"和"embedding"不能为空.')
         super().__init__(vocab=vocab, reserved_token=reserved_token, language=language, cut_type=cut_type)
         reserved_token = self.reserved_token.copy()
         reserved_token.reverse()
         self.dim = len(embedding[0])
         for token in reserved_token:
             embedding = [[self.do_encode(token)] * self.dim] + embedding
-        self.embedding = embedding
+        self.embedding = Embedding.from_pretrained(torch.tensor(embedding, dtype=torch.float))
+
+    def __call__(self, sentence: Union[str, Iterable[str], Iterable[Iterable]], max_length: int = None):
+        input_ids = self.batch_encode(sentence, max_length)
+        return self.encode(torch.tensor(input_ids, dtype=torch.long))
 
     @classmethod
     def from_file(cls, file: str, func=load_embedding, is_large_file=False, reserved_token=[], language='cn', cut_type='word'):
         """
         :param file: embedding文件， 如：'./sgns.weibo.word.bz2'. 注意：必须是单一文件，不能是文件夹。
         :param func: 具体读取文件的处理函数，load_embedding，可替换。注意：其函数签名为 function_name(path: str, is_large_file: bool) -> [vocab], [[embedding]]
         :param is_large_file: 是否是大文件
```

### Comparing `nlpx-1.1.7/nlpx/text_token/_utils.py` & `nlpx-1.1.8/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.7/nlpx/training.py` & `nlpx-1.1.8/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.7/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.8/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.7
+Version: 1.1.8
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.7/setup.py` & `nlpx-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.7',
+    version='1.1.8',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

