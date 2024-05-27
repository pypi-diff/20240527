# Comparing `tmp/nonebot_plugin_sanyao-0.2.4.tar.gz` & `tmp/nonebot_plugin_sanyao-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sanyao-0.2.4.tar", last modified: Mon Apr 22 06:46:43 2024, max compression
+gzip compressed data, was "nonebot_plugin_sanyao-0.2.6.tar", last modified: Mon May 27 06:04:32 2024, max compression
```

## Comparing `nonebot_plugin_sanyao-0.2.4.tar` & `nonebot_plugin_sanyao-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0     1064 2024-04-22 06:46:31.002159 nonebot_plugin_sanyao-0.2.4/LICENSE
--rw-r--r--   0        0        0     2287 2024-04-22 06:46:31.002159 nonebot_plugin_sanyao-0.2.4/README.md
--rw-r--r--   0        0        0      366 2024-04-22 06:46:31.006160 nonebot_plugin_sanyao-0.2.4/nonebot_plugin_sanyao/__init__.py
--rw-r--r--   0        0        0      642 2024-04-22 06:46:31.006160 nonebot_plugin_sanyao-0.2.4/nonebot_plugin_sanyao/__main__.py
--rw-r--r--   0        0        0       87 2024-04-22 06:46:31.006160 nonebot_plugin_sanyao-0.2.4/nonebot_plugin_sanyao/config.py
--rw-r--r--   0        0        0     6143 2024-04-22 06:46:31.006160 nonebot_plugin_sanyao-0.2.4/nonebot_plugin_sanyao/sanyao.py
--rw-r--r--   0        0        0      963 2024-04-22 06:46:43.630261 nonebot_plugin_sanyao-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 nonebot_plugin_sanyao-0.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-27 06:04:18.000000 nonebot_plugin_sanyao-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-27 06:04:18.000000 nonebot_plugin_sanyao-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:04:32.296195 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:04:32.000000 nonebot_plugin_sanyao-0.2.6/nonebot_plugin_sanyao/nonebot_plugin_sanyao.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-27 06:04:18.000000 nonebot_plugin_sanyao-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:04:32.300195 nonebot_plugin_sanyao-0.2.6/setup.cfg
```

### Comparing `nonebot_plugin_sanyao-0.2.4/LICENSE` & `nonebot_plugin_sanyao-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.2.4/README.md` & `nonebot_plugin_sanyao-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sanyao-0.2.4/pyproject.toml` & `nonebot_plugin_sanyao-0.2.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 [project]
 name = "nonebot-plugin-sanyao"
-dynamic = []
+version = "0.2.6"
 authors = [
-    { name = "afterow", email = "afterow@163.com" },
+    {name="afterow", email="afterow@163.com"}
 ]
 description = "三爻易数排盘"
 readme = "README.md"
-requires-python = ">=3.9"
+license = { text = "MIT License" }
+requires-python = ">=3.10, <4.0"
 dependencies = [
-    "cnlunar>=0.1.3",
-    "nonebot2>=2.2.0",
+    "cnlunar",
+    "nonebot2"
 ]
 classifiers = [
     "Framework :: Pydantic",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Natural Language :: Chinese (Simplified)",
+    "Natural Language :: Chinese (Simplified)"
 ]
-version = "0.2.4"
 
-[project.license]
-text = "MIT License"
+[tool.nonebot]
+adapters = [
+    { name = "OneBot V11", module_name = "nonebot.adapters.onebot.v11" }
+]
+plugins = ["nonebot_plugin_sanyao"]
+plugin_dirs = ["nonebot_plugin_sanyao"]
+builtin_plugins = []
 
-[project.urls]
-Homepage = "https://github.com/afterow/nonebot-plugin-sanyao"
-"Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
+[tool.setuptools.packages.find]
+where = ['nonebot_plugin_sanyao']
+include = []
 
 [build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
+requires = ["setuptools >= 65.6.3"]
+build-backend = "setuptools.build_meta"
 
-[tool.pdm.version]
-source = "file"
-path = "nonebot_plugin_sanyao/__init__.py"
+[project.urls]
+"Homepage" = "https://github.com/afterow/nonebot-plugin-sanyao"
+"Bug Tracker" = "https://github.com/afterow/nonebot-plugin-sanyao/issues"
```

### Comparing `nonebot_plugin_sanyao-0.2.4/PKG-INFO` & `nonebot_plugin_sanyao-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sanyao
-Version: 0.2.4
+Version: 0.2.6
 Summary: 三爻易数排盘
-Author-Email: afterow <afterow@163.com>
+Author-email: afterow <afterow@163.com>
 License: MIT License
+Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
+Project-URL: Bug Tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: Chinese (Simplified)
-Project-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao
-Project-URL: Bug tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues
-Requires-Python: >=3.9
-Requires-Dist: cnlunar>=0.1.3
-Requires-Dist: nonebot2>=2.2.0
+Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cnlunar
+Requires-Dist: nonebot2
 
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
-Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.4 Summary:
-ä¸ç»ææ°æç Author-Email: afterow
-163.com> License: MIT License Classifier: Framework :: Pydantic Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified) Project-
-URL: Homepage, https://github.com/afterow/nonebot-plugin-sanyao Project-URL:
-Bug tracker, https://github.com/afterow/nonebot-plugin-sanyao/issues Requires-
-Python: >=3.9 Requires-Dist: cnlunar>=0.1.3 Requires-Dist: nonebot2>=2.2.0
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot-plugin-sanyao Version: 0.2.6 Summary:
+ä¸ç»ææ°æç Author-email: afterow
+163.com> License: MIT License Project-URL: Homepage, https://github.com/
+afterow/nonebot-plugin-sanyao Project-URL: Bug Tracker, https://github.com/
+afterow/nonebot-plugin-sanyao/issues Classifier: Framework :: Pydantic
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Natural Language :: Chinese (Simplified)
+Requires-Python: <4.0,>=3.10 Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: cnlunar Requires-Dist: nonebot2
                                     _[_l_o_g_o_]
                                     [logo]
   # nonebot-plugin-sanyao _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª ä¸ç»ææ°æä»¶ ## ð ä»ç» è¿éæ¯ä¸ä¸ª
 ä¸ç»ææ°æä»¶ï¼åç»­å¢å 64å¦ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨
 nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
```

