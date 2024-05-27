# Comparing `tmp/nonebot_plugin_plus_one-0.1.3.tar.gz` & `tmp/nonebot_plugin_plus_one-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_plus_one-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_plus_one-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_plus_one-0.1.3.tar` & `nonebot_plugin_plus_one-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      536 2024-05-24 04:48:27.158177 nonebot_plugin_plus_one-0.1.3/nonebot_plugin_plus_one/__init__.py
--rw-r--r--   0        0        0      312 2024-05-24 03:08:41.722147 nonebot_plugin_plus_one-0.1.3/nonebot_plugin_plus_one/config.py
--rw-r--r--   0        0        0     1350 2024-05-24 04:49:07.055376 nonebot_plugin_plus_one-0.1.3/nonebot_plugin_plus_one/handler.py
--rw-r--r--   0        0        0      665 2024-05-24 08:57:15.396164 nonebot_plugin_plus_one-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1391 2024-05-24 04:52:01.673109 nonebot_plugin_plus_one-0.1.3/README.md
--rw-r--r--   0        0        0     2266 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      536 2024-05-24 04:48:27.158177 nonebot_plugin_plus_one-0.1.4/nonebot_plugin_plus_one/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-24 03:08:41.722147 nonebot_plugin_plus_one-0.1.4/nonebot_plugin_plus_one/config.py
+-rw-r--r--   0        0        0     1350 2024-05-24 04:49:07.055376 nonebot_plugin_plus_one-0.1.4/nonebot_plugin_plus_one/handler.py
+-rw-r--r--   0        0        0      700 2024-05-27 03:20:17.159319 nonebot_plugin_plus_one-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1391 2024-05-24 04:52:01.673109 nonebot_plugin_plus_one-0.1.4/README.md
+-rw-r--r--   0        0        0     2317 1970-01-01 00:00:00.000000 nonebot_plugin_plus_one-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_plus_one-0.1.3/nonebot_plugin_plus_one/__init__.py` & `nonebot_plugin_plus_one-0.1.4/nonebot_plugin_plus_one/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.3/nonebot_plugin_plus_one/handler.py` & `nonebot_plugin_plus_one-0.1.4/nonebot_plugin_plus_one/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.3/pyproject.toml` & `nonebot_plugin_plus_one-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [tool.poetry]
 name = "nonebot-plugin-plus-one"
-version = "0.1.3"
+version = "0.1.4"
 description = "全新复读姬，支持文本、图片、表情甚至是转发分享卡片复读，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.0"
+nonebot2 = "^2.2"
+nonebot_plugin_session = "^0.3"
+
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
```

### Comparing `nonebot_plugin_plus_one-0.1.3/README.md` & `nonebot_plugin_plus_one-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_plus_one-0.1.3/PKG-INFO` & `nonebot_plugin_plus_one-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-plus-one
-Version: 0.1.3
+Version: 0.1.4
 Summary: 全新复读姬，支持文本、图片、表情甚至是转发分享卡片复读，任意群聊触发 +1，姬就 +1。轻巧、专注，不使用任何数据库，不使用任何文件存储
 License: MIT
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nonebot2 (>=2.0,<3.0)
+Requires-Dist: nonebot2 (>=2.2,<3.0)
+Requires-Dist: nonebot_plugin_session (>=0.3,<0.4)
 Project-URL: homepage, https://github.com/yejue/nonebot-plugin-plus-one
 Project-URL: repository, https://github.com/yejue/nonebot-plugin-plus-one
 Description-Content-Type: text/markdown
 
 
 <h1 align="center">🐣🐤只是一个复读姬 ✨</h1>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-plus-one Version: 0.1.4 Summary:
 å¨æ°å¤è¯»å§¬ï¼æ¯æææ¬ãå¾çãè¡¨æçè³æ¯è½¬ååäº«å¡çå¤è¯»ï¼ä»»æç¾¤èè§¦å
 +1ï¼å§¬å°±
 +1ãè½»å·§ãä¸æ³¨ï¼ä¸ä½¿ç¨ä»»ä½æ°æ®åºï¼ä¸ä½¿ç¨ä»»ä½æä»¶å­å¨
 License: MIT Author: yejue Author-email: 1145331931@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: nonebot2 (>=2.0,<3.0) Project-URL: homepage, https://github.com/yejue/
-nonebot-plugin-plus-one Project-URL: repository, https://github.com/yejue/
-nonebot-plugin-plus-one Description-Content-Type: text/markdown
+Dist: nonebot2 (>=2.2,<3.0) Requires-Dist: nonebot_plugin_session (>=0.3,<0.4)
+Project-URL: homepage, https://github.com/yejue/nonebot-plugin-plus-one
+Project-URL: repository, https://github.com/yejue/nonebot-plugin-plus-one
+Description-Content-Type: text/markdown
                 ************ ?ð???£?ð???¤?å??ª?æ??¯?ä?¸??ä?¸?ª?å?¤??è?¯?»?å?§?¬ ?â??¨ ************
                                      _â¨
 åªæ¯ä¸ä¸ªå¤è¯»å§¬ï¼æ¯æç¾¤èç½ååãææ¬å¤è¯»ãå¾çè¡¨æå¤è¯»
                                      â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## å¿«éå®è£ ç¬¬ä¸æ­¥ï¼å³ä¸è§ â ç¹ä¸ªä¸è¦é±ç star
 å§ï¼è¿æ¯ä¸æ­ç»´æ¤æ´æ°çå¨åã ### nb-cli ```shell nb plugin
```

