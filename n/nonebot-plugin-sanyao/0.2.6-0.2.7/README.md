# Comparing `tmp/nonebot_plugin_sanyao-0.2.6.tar.gz` & `tmp/nonebot_plugin_sanyao-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.2.6.tar", last modified: Mon May 27 06:04:32 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.2.7.tar", last modified: Mon May 27 09:01:54 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.2.6.tar` & `nonebot_plugin_sanyao-0.2.7.tar`

### file list

```diff
@@ -1,13 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-27 06:04:18.000000 nonebot_plugin_sanyao-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-27 06:04:18.000000 nonebot_plugin_sanyao-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:04:32.296195 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-27 06:04:18.000000 nonebot_plugin_sanyao-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/setup.cfg
+-rw-r--r--   0        0        0     1064 2024-05-27 09:01:42.434974 nonebot_plugin_sanyao-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2287 2024-05-27 09:01:42.434974 nonebot_plugin_sanyao-0.2.7/README.md
+-rw-r--r--   0        0        0      366 2024-05-27 09:01:42.434974 nonebot_plugin_sanyao-0.2.7/nonebot_plugin_sanyao/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-27 09:01:42.434974 nonebot_plugin_sanyao-0.2.7/nonebot_plugin_sanyao/__main__.py
+-rw-r--r--   0        0        0       87 2024-05-27 09:01:42.434974 nonebot_plugin_sanyao-0.2.7/nonebot_plugin_sanyao/config.py
+-rw-r--r--   0        0        0     6199 2024-05-27 09:01:42.434974 nonebot_plugin_sanyao-0.2.7/nonebot_plugin_sanyao/sanyao.py
+-rw-r--r--   0        0        0     1180 2024-05-27 09:01:54.883001 nonebot_plugin_sanyao-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3056 1970-01-01 00:00:00.000000 nonebot_plugin_sanyao-0.2.7/PKG-INFO
```

### Comparing `nonebot_plugin_sanyao-0.2.6/LICENSE` & `nonebot_plugin_sanyao-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.2.6/PKG-INFO` & `nonebot_plugin_sanyao-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.2.6
+Version: 0.2.7
 Summary: 三爻易数排盘
-Author-email: afterow <afterow@163.com>
+Author-Email: afterow <afterow@163.com>
 License: MIT License
-Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
-Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: Chinese (Simplified)
+Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
+Project-URL: Bug tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Requires-Python: <4.0,>=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: cnlunar
 Requires-Dist: nonebot2
+Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store">
     <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="logo">
   </a>
   <br>
   <p>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.6 Summary:
-ä¸ç»ææ°æç Author-email: afterow
-163.com> License: MIT License Project-URL: Homepage, https://github.com/
-afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
-afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified)
-Requires-Python: <4.0,>=3.10 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: cnlunar Requires-Dist: nonebot2
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.7 Summary:
+ä¸ç»ææ°æç Author-Email: afterow
+163.com> License: MIT License Classifier: Framework :: Pydantic Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified) Project-
+URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao Project-URL:
+Bug tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues Requires-
+Python: <4.0,>=3.10 Requires-Dist: cnlunar Requires-Dist: nonebot2 Description-
+Content-Type: text/markdown
                                     _[_l_o_g_o_]
                                     [logo]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
```

### Comparing `nonebot_plugin_sanyao-0.2.6/README.md` & `nonebot_plugin_sanyao-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.2.6/pyproject.toml` & `nonebot_plugin_sanyao-0.2.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 [project]
 name = "nonebot-plugin-sanyao"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
-    {name="afterow", email="afterow@163.com"}
+    { name = "afterow", email = "afterow@163.com" },
 ]
 description = "三爻易数排盘"
 readme = "README.md"
-license = { text = "MIT License" }
 requires-python = ">=3.10, <4.0"
 dependencies = [
     "cnlunar",
-    "nonebot2"
+    "nonebot2",
 ]
 classifiers = [
     "Framework :: Pydantic",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Natural Language :: Chinese (Simplified)"
+    "Natural Language :: Chinese (Simplified)",
 ]
 
+[project.license]
+text = "MIT License"
+
+[project.urls]
+Homepage = "https://github.com/afterow/nonebot-plugin-sanyao"
+"Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
+
 [tool.nonebot]
 adapters = [
-    { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" }
+    { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" },
+]
+plugins = [
+    "nonebot_plugin_sanyao",
+]
+plugin_dirs = [
+    "nonebot_plugin_sanyao",
+]
+builtin_plugins = [
+    "echo",
 ]
-plugins = ["nonebot_plugin_sanyao"]
-plugin_dirs = ["nonebot_plugin_sanyao"]
-builtin_plugins = []
 
 [tool.setuptools.packages.find]
-where = ['nonebot_plugin_sanyao']
+where = [
+    "nonebot_plugin_sanyao",
+]
 include = []
 
 [build-system]
-requires = ["setuptools >= 65.6.3"]
-build-backend = "setuptools.build_meta"
-
-[project.urls]
-"Homepage" = "https://github.com/afterow/nonebot-plugin-sanyao"
-"Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
```

