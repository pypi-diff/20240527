# Comparing `tmp/fastdev-0.0.6.tar.gz` & `tmp/fastdev-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdev-0.0.6.tar", last modified: Wed May 22 22:44:45 2024, max compression
+gzip compressed data, was "fastdev-0.0.7.tar", last modified: Mon May 27 00:05:57 2024, max compression
```

## Comparing `fastdev-0.0.6.tar` & `fastdev-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.742223 fastdev-0.0.6/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)     1956 2024-05-22 22:44:45.741223 fastdev-0.0.6/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      751 2024-05-22 14:25:21.000000 fastdev-0.0.6/README.md
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1075 2024-05-22 22:44:03.000000 fastdev-0.0.6/pyproject.toml
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-22 22:44:45.742223 fastdev-0.0.6/setup.cfg
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.739223 fastdev-0.0.6/src/
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.739223 fastdev-0.0.6/src/fastdev/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:08:07.000000 fastdev-0.0.6/src/fastdev/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-14 01:25:51.000000 fastdev-0.0.6/src/fastdev/constants.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.740223 fastdev-0.0.6/src/fastdev/datasets/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.6/src/fastdev/datasets/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17965 2024-05-22 22:07:35.000000 fastdev-0.0.6/src/fastdev/datasets/dexycb.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.740223 fastdev-0.0.6/src/fastdev/io/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      101 2024-05-22 22:08:01.000000 fastdev-0.0.6/src/fastdev/io/__init__.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.740223 fastdev-0.0.6/src/fastdev/io/handlers/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.6/src/fastdev/io/handlers/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      501 2024-05-22 08:08:06.000000 fastdev-0.0.6/src/fastdev/io/handlers/base_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      723 2024-05-22 22:07:46.000000 fastdev-0.0.6/src/fastdev/io/handlers/json_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1761 2024-05-22 22:07:41.000000 fastdev-0.0.6/src/fastdev/io/handlers/yaml_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3661 2024-05-22 22:07:57.000000 fastdev-0.0.6/src/fastdev/io/io.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 07:27:36.000000 fastdev-0.0.6/src/fastdev/py.typed
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.740223 fastdev-0.0.6/src/fastdev/robo/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      111 2024-05-22 22:09:23.000000 fastdev-0.0.6/src/fastdev/robo/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1335 2024-05-22 14:15:16.000000 fastdev-0.0.6/src/fastdev/robo/urdf.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.740223 fastdev-0.0.6/src/fastdev/smplx/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      275 2024-05-22 08:08:06.000000 fastdev-0.0.6/src/fastdev/smplx/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     4099 2024-05-22 13:54:52.000000 fastdev-0.0.6/src/fastdev/smplx/smplx.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.740223 fastdev-0.0.6/src/fastdev/transforms/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1421 2024-05-18 00:55:47.000000 fastdev-0.0.6/src/fastdev/transforms/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    18016 2024-05-22 22:43:44.000000 fastdev-0.0.6/src/fastdev/transforms/rotation.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     6624 2024-05-22 11:21:07.000000 fastdev-0.0.6/src/fastdev/transforms/transforms.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3017 2024-05-22 11:21:53.000000 fastdev-0.0.6/src/fastdev/transforms/utils.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.740223 fastdev-0.0.6/src/fastdev/utils/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      123 2024-05-22 07:54:17.000000 fastdev-0.0.6/src/fastdev/utils/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      795 2024-05-22 11:22:28.000000 fastdev-0.0.6/src/fastdev/utils/dispatch.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1215 2024-05-22 11:31:18.000000 fastdev-0.0.6/src/fastdev/utils/geometry.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1361 2024-05-22 11:22:49.000000 fastdev-0.0.6/src/fastdev/utils/timer.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.741223 fastdev-0.0.6/src/fastdev/visualization/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.6/src/fastdev/visualization/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1831 2024-05-22 11:23:08.000000 fastdev-0.0.6/src/fastdev/visualization/image.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.741223 fastdev-0.0.6/src/fastdev.egg-info/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)     1956 2024-05-22 22:44:45.000000 fastdev-0.0.6/src/fastdev.egg-info/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1018 2024-05-22 22:44:45.000000 fastdev-0.0.6/src/fastdev.egg-info/SOURCES.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-22 22:44:45.000000 fastdev-0.0.6/src/fastdev.egg-info/dependency_links.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      235 2024-05-22 22:44:45.000000 fastdev-0.0.6/src/fastdev.egg-info/requires.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-22 22:44:45.000000 fastdev-0.0.6/src/fastdev.egg-info/top_level.txt
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:44:45.741223 fastdev-0.0.6/tests/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1189 2024-05-22 22:10:20.000000 fastdev-0.0.6/tests/test_io.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1185 2024-05-22 09:27:21.000000 fastdev-0.0.6/tests/test_transforms.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.452247 fastdev-0.0.7/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)     2317 2024-05-27 00:05:57.451247 fastdev-0.0.7/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      839 2024-05-26 23:27:22.000000 fastdev-0.0.7/README.md
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1311 2024-05-27 00:02:42.000000 fastdev-0.0.7/pyproject.toml
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-27 00:05:57.452247 fastdev-0.0.7/setup.cfg
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.449247 fastdev-0.0.7/src/
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.449247 fastdev-0.0.7/src/fastdev/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 22:08:07.000000 fastdev-0.0.7/src/fastdev/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-14 01:25:51.000000 fastdev-0.0.7/src/fastdev/constants.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/datasets/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.7/src/fastdev/datasets/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    19697 2024-05-26 23:56:30.000000 fastdev-0.0.7/src/fastdev/datasets/dexycb.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/io/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      101 2024-05-23 02:52:37.000000 fastdev-0.0.7/src/fastdev/io/__init__.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/io/handlers/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.7/src/fastdev/io/handlers/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      501 2024-05-22 08:08:06.000000 fastdev-0.0.7/src/fastdev/io/handlers/base_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      723 2024-05-22 22:07:46.000000 fastdev-0.0.7/src/fastdev/io/handlers/json_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1761 2024-05-22 22:07:41.000000 fastdev-0.0.7/src/fastdev/io/handlers/yaml_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3657 2024-05-23 03:38:46.000000 fastdev-0.0.7/src/fastdev/io/io.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 07:27:36.000000 fastdev-0.0.7/src/fastdev/py.typed
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/robo/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      111 2024-05-22 22:09:23.000000 fastdev-0.0.7/src/fastdev/robo/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1335 2024-05-22 14:15:16.000000 fastdev-0.0.7/src/fastdev/robo/urdf.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/smplx/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      275 2024-05-22 08:08:06.000000 fastdev-0.0.7/src/fastdev/smplx/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     4099 2024-05-22 13:54:52.000000 fastdev-0.0.7/src/fastdev/smplx/smplx.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/transforms/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1421 2024-05-18 00:55:47.000000 fastdev-0.0.7/src/fastdev/transforms/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    18016 2024-05-22 22:43:44.000000 fastdev-0.0.7/src/fastdev/transforms/rotation.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     6624 2024-05-23 23:59:14.000000 fastdev-0.0.7/src/fastdev/transforms/transforms.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3031 2024-05-24 09:21:26.000000 fastdev-0.0.7/src/fastdev/transforms/utils.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/utils/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      125 2024-05-26 23:59:28.000000 fastdev-0.0.7/src/fastdev/utils/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      822 2024-05-24 09:21:26.000000 fastdev-0.0.7/src/fastdev/utils/dispatch.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1215 2024-05-22 11:31:18.000000 fastdev-0.0.7/src/fastdev/utils/geometry.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      778 2024-05-26 23:57:33.000000 fastdev-0.0.7/src/fastdev/utils/timer.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.450247 fastdev-0.0.7/src/fastdev/visualization/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.7/src/fastdev/visualization/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1831 2024-05-22 11:23:08.000000 fastdev-0.0.7/src/fastdev/visualization/image.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.451247 fastdev-0.0.7/src/fastdev.egg-info/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)     2317 2024-05-27 00:05:57.000000 fastdev-0.0.7/src/fastdev.egg-info/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1018 2024-05-27 00:05:57.000000 fastdev-0.0.7/src/fastdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-27 00:05:57.000000 fastdev-0.0.7/src/fastdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      224 2024-05-27 00:05:57.000000 fastdev-0.0.7/src/fastdev.egg-info/requires.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-27 00:05:57.000000 fastdev-0.0.7/src/fastdev.egg-info/top_level.txt
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-27 00:05:57.451247 fastdev-0.0.7/tests/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1189 2024-05-22 22:10:20.000000 fastdev-0.0.7/tests/test_io.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1057 2024-05-24 09:21:26.000000 fastdev-0.0.7/tests/test_transforms.py
```

### Comparing `fastdev-0.0.6/PKG-INFO` & `fastdev-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 Metadata-Version: 2.1
 Name: fastdev
-Version: 0.0.6
+Version: 0.0.7
 Summary: Type less, code more
 Author-email: Jianglong Ye <jianglong.yeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/jianglongye/fastdev
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: typing-extensions
 Requires-Dist: fastcore
 Requires-Dist: msgspec[toml,yaml]
 Requires-Dist: rich
 Requires-Dist: fsspec
 Requires-Dist: universal_pathlib
-Requires-Dist: huggingface_hub[cli,hf_transfer]
+Requires-Dist: huggingface_hub
 Requires-Dist: GitPython
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: xdoctest; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: streamlit; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: docutils; extra == "doc"
 Requires-Dist: sphinx-autoapi; extra == "doc"
 Requires-Dist: m2r2; extra == "doc"
-Requires-Dist: setuptools; extra == "doc"
 
-![](https://fastdev.jianglongye.com/_static/logo.svg)
+<p align="center">
+    <img alt="logo" src="https://fastdev.jianglongye.com/_static/logo.svg" style="max-width:600px;width:100%" />
+</p>
 
 <p align="center">
     <em><a href="https://fastdev.jianglongye.com">Documentation</a></em>
     &nbsp;&nbsp;&bull;&nbsp;&nbsp;
     <em><code>pip install fastdev</code></em>
 </p>
 
 ---
 
 > Type Less, Code More
 
-## Features
+## Features 🌟
 
 - **Reasearch oriented**, provide a set of tools for vision and robotics research
 - **User friendly**, provide simple-yet-flexible APIs to reduce boilerplate code
 - **Strong typed**, provide type checking and code completion
 
 ## Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,26 +1,29 @@
-Metadata-Version: 2.1 Name: fastdev Version: 0.0.6 Summary: Type less, code
+Metadata-Version: 2.1 Name: fastdev Version: 0.0.7 Summary: Type less, code
 more Author-email: Jianglong Ye
 gmail.com> License: MIT Project-URL: Repository, https://github.com/
 jianglongye/fastdev Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Requires-Dist: typing-extensions Requires-Dist: fastcore Requires-Dist: msgspec
-[toml,yaml] Requires-Dist: rich Requires-Dist: fsspec Requires-Dist:
-universal_pathlib Requires-Dist: huggingface_hub[cli,hf_transfer] Requires-
-Dist: GitPython Provides-Extra: dev Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev" Requires-Dist: ipython; extra == "dev"
-Requires-Dist: ruff; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: mypy; extra == "dev" Requires-Dist: types-PyYAML; extra == "dev"
-Provides-Extra: doc Requires-Dist: sphinx; extra == "doc" Requires-Dist: furo;
-extra == "doc" Requires-Dist: docutils; extra == "doc" Requires-Dist: sphinx-
-autoapi; extra == "doc" Requires-Dist: m2r2; extra == "doc" Requires-Dist:
-setuptools; extra == "doc" ![](https://fastdev.jianglongye.com/_static/
-logo.svg)
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Requires-Dist: typing-extensions Requires-Dist: fastcore
+Requires-Dist: msgspec[toml,yaml] Requires-Dist: rich Requires-Dist: fsspec
+Requires-Dist: universal_pathlib Requires-Dist: huggingface_hub Requires-Dist:
+GitPython Provides-Extra: dev Requires-Dist: build; extra == "dev" Requires-
+Dist: twine; extra == "dev" Requires-Dist: ipython; extra == "dev" Requires-
+Dist: ruff; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
+xdoctest; extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+pre-commit; extra == "dev" Requires-Dist: streamlit; extra == "dev" Provides-
+Extra: doc Requires-Dist: sphinx; extra == "doc" Requires-Dist: furo; extra ==
+"doc" Requires-Dist: docutils; extra == "doc" Requires-Dist: sphinx-autoapi;
+extra == "doc" Requires-Dist: m2r2; extra == "doc"
+                                    [logo]
                     _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn   •   ppiipp iinnssttaallll ffaassttddeevv
---- > Type Less, Code More ## Features - **Reasearch oriented**, provide a set
-of tools for vision and robotics research - **User friendly**, provide simple-
-yet-flexible APIs to reduce boilerplate code - **Strong typed**, provide type
-checking and code completion ## Installation The package is available on PyPI,
-you can install it via pip: ```shell pip install fastdev ``` Or you can install
-the latest version from the source code: ```shell pip install "git+https://
-github.com/jianglongye/fastdev.git" ```
+--- > Type Less, Code More ## Features ð - **Reasearch oriented**, provide a
+set of tools for vision and robotics research - **User friendly**, provide
+simple-yet-flexible APIs to reduce boilerplate code - **Strong typed**, provide
+type checking and code completion ## Installation The package is available on
+PyPI, you can install it via pip: ```shell pip install fastdev ``` Or you can
+install the latest version from the source code: ```shell pip install
+"git+https://github.com/jianglongye/fastdev.git" ```
```

### Comparing `fastdev-0.0.6/pyproject.toml` & `fastdev-0.0.7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastdev"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "Jianglong Ye", email = "jianglong.yeh@gmail.com" }]
 description = "Type less, code more"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "typing-extensions",
     "fastcore",
     "msgspec[toml,yaml]",
     "rich",
     "fsspec",
     "universal_pathlib",
-    "huggingface_hub[cli,hf_transfer]",
+    "huggingface_hub",
     "GitPython",
 ]
 
 [project.optional-dependencies]
-dev = ["build", "twine", "ipython", "ruff", "pytest", "mypy", "types-PyYAML"]
-doc = ["sphinx", "furo", "docutils", "sphinx-autoapi", "m2r2", "setuptools"]
+dev = [
+    "build",
+    "twine",
+    "ipython",
+    "ruff",
+    "pytest",
+    "xdoctest",
+    "mypy",
+    "pre-commit",
+    "streamlit",
+]
+doc = ["sphinx", "furo", "docutils", "sphinx-autoapi", "m2r2"]
 
 [project.urls]
 Repository = "https://github.com/jianglongye/fastdev"
 
 [tool.ruff]
-exclude = ["playground", "tests"]
 line-length = 120
 
 [tool.mypy]
-exclude = ["playground", "tests", "dexycb.py"]
+exclude = ["playground", "tests", "src/fastdev/datasets"]
 ignore_missing_imports = true
```

### Comparing `fastdev-0.0.6/src/fastdev/constants.py` & `fastdev-0.0.7/src/fastdev/constants.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/datasets/dexycb.py` & `fastdev-0.0.7/src/fastdev/datasets/dexycb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import dataclasses
 import os
 import pickle
 from glob import glob
-from typing import Literal, Optional
+from typing import Dict, Literal, Optional
 
 import cv2
 import numpy as np
 import torch
+import trimesh
 from rich.progress import track
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset, default_collate
 from torchvision.io import read_image
 
 from fastdev.constants import FDEV_DATASET_ROOT, FDEV_PROCESSED_ROOT
 from fastdev.io import load
-from fastdev.utils import Timer
+from fastdev.utils import timeit
 
 _SUBJECTS = [
     "20200709-subject-01",
     "20200813-subject-02",
     "20200820-subject-03",
     "20200903-subject-04",
     "20200908-subject-05",
@@ -63,14 +64,16 @@
     20: "052_extra_large_clamp",
     21: "061_foam_brick",
 }
 
 
 @dataclasses.dataclass
 class DexYCBDatasetConfig:
+    """Configuration for DexYCBDataset."""
+
     data_root: str = os.path.join(FDEV_DATASET_ROOT, "dexycb")
 
     split: Literal["train", "val", "test", "all"] = "train"
     hand_side: Literal["left", "right", "both"] = "left"
     setup: Literal["s0", "s1", "s2", "s3"] = "s0"
     """
 
@@ -79,31 +82,44 @@
     - [s2] Unseen camera views
     - [s3] Unseen grasped objects
 
     Reference_
 
     .. _Reference: https://github.com/NVlabs/dex-ycb-toolkit/blob/64551b001d360ad83bc383157a559ec248fb9100/dex_ycb_toolkit/dex_ycb.py#L126
     """
+    serials: Optional[list[str]] = None  # specify serials to load
 
     return_color: bool = True
     return_depth: bool = False
+    return_object_mesh: bool = False  # return object mesh vertices and faces in the object space
     return_as_sequence: bool = False  # return the whole sequence instead of a single frame
     return_no_hand_frames: bool = True
-    # if False, filter out frames where the hand is not visible (mano pose all zeros)
+    # if False, filter out frames where the hand is not fully visible on image (i.e., mano pose non-zero and all joints inside the frame)
 
     metadata_cache_path: str = os.path.join(FDEV_PROCESSED_ROOT, "dexycb", "metadata_cache.pkl")
     # pkl is faster than npz, suitable for caching
     force_rebuild_cache: bool = False
 
     def __post_init__(self) -> None:
         assert os.path.exists(self.data_root), f"Data root {self.data_root} does not exist."
+        if self.serials is not None:
+            assert all(s in _SERIALS for s in self.serials), f"Serials {self.serials} invalid."
 
 
 class DexYCBDataset(Dataset):
-    """DexYCBDataset."""
+    """DexYCBDataset.
+
+    Args:
+        config (DexYCBDatasetConfig): configuration for the dataset.
+
+    Examples:
+        >>> # doctest: +SKIP
+        >>> from fastdev.datasets.dexycb import DexYCBDataset, DexYCBDatasetConfig
+        >>> dataset = DexYCBDataset(DexYCBDatasetConfig())
+    """
 
     ycb_classes = _YCB_CLASSES
 
     def __init__(self, config: DexYCBDatasetConfig) -> None:
         super().__init__()
 
         self.config = config
@@ -113,14 +129,15 @@
         self._model_dir = os.path.join(self._data_dir, "models")
         self._color_format = "color_{:06d}.jpg"
         self._depth_format = "aligned_depth_to_color_{:06d}.png"
         self._label_format = "labels_{:06d}.npz"
         self._h = 480
         self._w = 640
         self._obj_file = {k: os.path.join(self._model_dir, v, "textured_simple.obj") for k, v in _YCB_CLASSES.items()}
+        self._obj_mesh_cache = {}
 
         # ----------- Cache Metadata -----------
         if (not os.path.exists(self.config.metadata_cache_path)) or self.config.force_rebuild_cache:
             intrinsics = {}
             for serial in _SERIALS:
                 intr_file = os.path.join(
                     self._calib_dir,
@@ -193,15 +210,15 @@
                         "intrinsics": intrinsics,
                         "extrinsics": extrinsics,
                         "mano_calibs": mano_calibs,
                         "seq_metas": seq_metas,
                     },
                     f,
                 )
-        with Timer(print_tmpl="Loading metadata cache: {:.4f}s"):
+        with timeit(print_tmpl="Loading metadata cache: {:.4f}s"):
             with open(self.config.metadata_cache_path, "rb") as f:
                 metadata_cache = pickle.load(f)
                 self._intrinsics = metadata_cache["intrinsics"]
                 self._extrinsics = metadata_cache["extrinsics"]
                 self._mano_calibs = metadata_cache["mano_calibs"]
                 cached_seq_metas = metadata_cache["seq_metas"]
 
@@ -264,15 +281,15 @@
                 sequence_ind = [i for i in range(100) if i // 5 in (7, 11, 15)]
         if self.config.split == "all":
             subject_ind = list(range(10))
             serial_ind = list(range(8))
             sequence_ind = list(range(100))
 
         self._subjects = [_SUBJECTS[i] for i in subject_ind]  # type: ignore
-        self._serials = [_SERIALS[i] for i in serial_ind]  # type: ignore
+        self._serials = [_SERIALS[i] for i in serial_ind] if self.config.serials is None else self.config.serials  # type: ignore
         self._sequences, self._seq_metas = [], []
 
         for subject in self._subjects:
             seqs = sorted([seq for seq in cached_seq_metas.keys() if subject in seq])
             seqs = [seqs[i] for i in sequence_ind]  # type: ignore
             for seq in seqs:
                 meta = cached_seq_metas[seq]
@@ -318,14 +335,23 @@
             frame_data["color"] = read_image(color_file)
         if self.config.return_depth:
             depth_file = os.path.join(data_dir, self._depth_format.format(frame_idx))
             depth = cv2.imread(depth_file, cv2.IMREAD_ANYDEPTH)
             frame_data["depth"] = torch.from_numpy(depth.astype(np.float32) / 1000)
         return frame_data
 
+    def _load_object_mesh(self, ycb_id: int) -> Dict[Literal["vertices", "faces"], torch.Tensor]:
+        if ycb_id not in self._obj_mesh_cache:
+            obj_file = self._obj_file[ycb_id]
+            obj_mesh = trimesh.load(obj_file)
+            vertices = torch.tensor(obj_mesh.vertices, dtype=torch.float32)  # type: ignore
+            faces = torch.tensor(obj_mesh.faces, dtype=torch.int32)  # type: ignore
+            self._obj_mesh_cache[ycb_id] = {"vertices": vertices, "faces": faces}
+        return self._obj_mesh_cache[ycb_id]
+
     def __getitem__(self, idx):
         if not self.config.return_as_sequence:
             seq_idx, serial_idx, frame_idx = self._mapping[idx]
             # range is always half-open
             frame_range = (frame_idx, frame_idx + 1)
         else:
             seq_idx, serial_idx = self._mapping[idx]
@@ -348,29 +374,39 @@
             "mano_side": seq_meta["mano_sides"][0],
             "mano_betas": torch.tensor(
                 self._mano_calibs[seq_meta["mano_calib"][0]]["betas"],
                 dtype=torch.float32,
             ),
         }
 
+        pose_y = torch.from_numpy(
+            seq_meta["pose_y"][self._serials[serial_idx]][frame_range[0] : frame_range[1]]
+        ).float()
+        sample["object_pose"] = pose_y
+        object_mesh = self._load_object_mesh(sample["ycb_grasp_id"])
+        sample["object_vertices"] = object_mesh["vertices"]
+        sample["object_faces"] = object_mesh["faces"]
+
         frames_data = [self._load_frame_data(data_dir, frame_idx) for frame_idx in range(*frame_range)]
         for key in frames_data[0].keys():
             sample[key] = torch.stack([frame_data[key] for frame_data in frames_data], dim=0)
             if not self.config.return_as_sequence:
                 sample[key].squeeze_(0)
         pose_m = torch.from_numpy(
             seq_meta["pose_m"][self._serials[serial_idx]][frame_range[0] : frame_range[1]]
         ).float()
         sample["mano_global_orient"] = pose_m[..., :3]
         sample["mano_hand_pose"] = pose_m[..., 3:48]
         sample["mano_transl"] = pose_m[..., 48:51]
+
         if not self.config.return_as_sequence:
             sample["mano_global_orient"].squeeze_(0)
             sample["mano_hand_pose"].squeeze_(0)
             sample["mano_transl"].squeeze_(0)
+            sample["object_pose"].squeeze_(0)
         return sample
 
     @property
     def h(self):
         return self._h
 
     @property
```

### Comparing `fastdev-0.0.6/src/fastdev/io/handlers/json_handler.py` & `fastdev-0.0.7/src/fastdev/io/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/io/handlers/yaml_handler.py` & `fastdev-0.0.7/src/fastdev/io/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/io/io.py` & `fastdev-0.0.7/src/fastdev/io/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from functools import lru_cache
 from pathlib import Path
-from typing import IO, Any, Dict, Literal, Mapping, Optional, Type, Union, cast
-
-from typing_extensions import TypeAlias
+from typing import IO, Any, Dict, Literal, Optional, Type, Union, cast
 
 import fsspec  # type: ignore
+from typing_extensions import TypeAlias
 
 from fastdev.io.handlers.base_handler import BaseFileHandler
 from fastdev.io.handlers.json_handler import JSONHandler
 from fastdev.io.handlers.yaml_handler import YAMLHandler
 
-FILE_HANDLER_CLASSES: Mapping[str, Type[BaseFileHandler]] = {
+FILE_HANDLER_CLASSES: Dict[str, Type[BaseFileHandler]] = {
     "json": JSONHandler,
     "yaml": YAMLHandler,
     "yml": YAMLHandler,
 }
 FILE_EXTENSIONS: TypeAlias = Literal["json", "yaml", "yml"]
 FILE_HANDLERS: Dict[str, BaseFileHandler] = {}
 
@@ -82,16 +81,16 @@
     Args:
         obj (Any): Python object to dump.
         file (Union[str, Path, IO]): File path or IO object.
         file_format (Optional[FILE_EXTENSIONS], optional): File format. Defaults to None.
 
     Examples:
         >>> import tempfile
-        >>> with tempfile.NamedTemporaryFile(suffix=".json") as f:
-        ...     dump({"hello": "world"}, f.name)
+        >>> with tempfile.TemporaryDirectory() as tmpdir:
+        ...     dump({"hello": "world"}, f"{tmpdir}/example.json")
     """
     # Parameters validation
     if isinstance(file, Path):
         file = str(file)
     if file_format is None:
         if isinstance(file, str):
             file_format = cast(FILE_EXTENSIONS, file.split(".")[-1])
```

### Comparing `fastdev-0.0.6/src/fastdev/robo/urdf.py` & `fastdev-0.0.7/src/fastdev/robo/urdf.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/smplx/smplx.py` & `fastdev-0.0.7/src/fastdev/smplx/smplx.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/transforms/__init__.py` & `fastdev-0.0.7/src/fastdev/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/transforms/rotation.py` & `fastdev-0.0.7/src/fastdev/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/transforms/transforms.py` & `fastdev-0.0.7/src/fastdev/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/transforms/utils.py` & `fastdev-0.0.7/src/fastdev/transforms/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     if check_handness:
         if np.linalg.det(rot_mat) < 0:
             raise RuntimeWarning("The rotation matrix is not right-hand.")
 
     return rot_mat
 
 
-def compose_intr_mat(fu: float, fv: float, cu: float, cv: float, skew: float = 0.0):
+def compose_intr_mat(fu: float, fv: float, cu: float, cv: float, skew: float = 0.0) -> np.ndarray:
     """
     Args:
         fu: horizontal focal length (width)
         fv: vertical focal length (height)
         cu: horizontal principal point (width)
         cv: vertical principal point (height)
         skew: skew coefficient, default to 0
```

### Comparing `fastdev-0.0.6/src/fastdev/utils/dispatch.py` & `fastdev-0.0.7/src/fastdev/utils/dispatch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from collections import defaultdict
 from typing import Callable, DefaultDict, TypeVar
 
 from fastcore.dispatch import TypeDispatch
 
 T = TypeVar("T")
 
-REGISTRY: DefaultDict[str, TypeDispatch] = defaultdict(TypeDispatch)
+DSIPATCH_REGISTRY: DefaultDict[str, TypeDispatch] = defaultdict(TypeDispatch)
 
 
 def typedispatch(is_impl: bool = True) -> Callable[[T], T]:
     def _inner(f: T) -> T:
         if isinstance(f, (classmethod, staticmethod)):
             name = f"{f.__func__.__qualname__}"
         elif hasattr(f, "__qualname__"):
             name = f"{f.__qualname__}"
         else:
             raise TypeError(f"Unsupported type: {type(f)}")
 
         if isinstance(f, classmethod):
             f = f.__func__  # type: ignore
         if is_impl:
-            REGISTRY[name].add(f)
-        return REGISTRY[name]  # type: ignore
+            DSIPATCH_REGISTRY[name].add(f)
+        return DSIPATCH_REGISTRY[name]  # type: ignore
 
     return _inner
 
 
 __all__ = ["typedispatch"]
```

### Comparing `fastdev-0.0.6/src/fastdev/utils/geometry.py` & `fastdev-0.0.7/src/fastdev/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev/visualization/image.py` & `fastdev-0.0.7/src/fastdev/visualization/image.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/src/fastdev.egg-info/PKG-INFO` & `fastdev-0.0.7/src/fastdev.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 Metadata-Version: 2.1
 Name: fastdev
-Version: 0.0.6
+Version: 0.0.7
 Summary: Type less, code more
 Author-email: Jianglong Ye <jianglong.yeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/jianglongye/fastdev
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: typing-extensions
 Requires-Dist: fastcore
 Requires-Dist: msgspec[toml,yaml]
 Requires-Dist: rich
 Requires-Dist: fsspec
 Requires-Dist: universal_pathlib
-Requires-Dist: huggingface_hub[cli,hf_transfer]
+Requires-Dist: huggingface_hub
 Requires-Dist: GitPython
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: xdoctest; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: streamlit; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: furo; extra == "doc"
 Requires-Dist: docutils; extra == "doc"
 Requires-Dist: sphinx-autoapi; extra == "doc"
 Requires-Dist: m2r2; extra == "doc"
-Requires-Dist: setuptools; extra == "doc"
 
-![](https://fastdev.jianglongye.com/_static/logo.svg)
+<p align="center">
+    <img alt="logo" src="https://fastdev.jianglongye.com/_static/logo.svg" style="max-width:600px;width:100%" />
+</p>
 
 <p align="center">
     <em><a href="https://fastdev.jianglongye.com">Documentation</a></em>
     &nbsp;&nbsp;&bull;&nbsp;&nbsp;
     <em><code>pip install fastdev</code></em>
 </p>
 
 ---
 
 > Type Less, Code More
 
-## Features
+## Features 🌟
 
 - **Reasearch oriented**, provide a set of tools for vision and robotics research
 - **User friendly**, provide simple-yet-flexible APIs to reduce boilerplate code
 - **Strong typed**, provide type checking and code completion
 
 ## Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,26 +1,29 @@
-Metadata-Version: 2.1 Name: fastdev Version: 0.0.6 Summary: Type less, code
+Metadata-Version: 2.1 Name: fastdev Version: 0.0.7 Summary: Type less, code
 more Author-email: Jianglong Ye
 gmail.com> License: MIT Project-URL: Repository, https://github.com/
 jianglongye/fastdev Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Requires-Dist: typing-extensions Requires-Dist: fastcore Requires-Dist: msgspec
-[toml,yaml] Requires-Dist: rich Requires-Dist: fsspec Requires-Dist:
-universal_pathlib Requires-Dist: huggingface_hub[cli,hf_transfer] Requires-
-Dist: GitPython Provides-Extra: dev Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev" Requires-Dist: ipython; extra == "dev"
-Requires-Dist: ruff; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: mypy; extra == "dev" Requires-Dist: types-PyYAML; extra == "dev"
-Provides-Extra: doc Requires-Dist: sphinx; extra == "doc" Requires-Dist: furo;
-extra == "doc" Requires-Dist: docutils; extra == "doc" Requires-Dist: sphinx-
-autoapi; extra == "doc" Requires-Dist: m2r2; extra == "doc" Requires-Dist:
-setuptools; extra == "doc" ![](https://fastdev.jianglongye.com/_static/
-logo.svg)
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Requires-Dist: typing-extensions Requires-Dist: fastcore
+Requires-Dist: msgspec[toml,yaml] Requires-Dist: rich Requires-Dist: fsspec
+Requires-Dist: universal_pathlib Requires-Dist: huggingface_hub Requires-Dist:
+GitPython Provides-Extra: dev Requires-Dist: build; extra == "dev" Requires-
+Dist: twine; extra == "dev" Requires-Dist: ipython; extra == "dev" Requires-
+Dist: ruff; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
+xdoctest; extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
+pre-commit; extra == "dev" Requires-Dist: streamlit; extra == "dev" Provides-
+Extra: doc Requires-Dist: sphinx; extra == "doc" Requires-Dist: furo; extra ==
+"doc" Requires-Dist: docutils; extra == "doc" Requires-Dist: sphinx-autoapi;
+extra == "doc" Requires-Dist: m2r2; extra == "doc"
+                                    [logo]
                     _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn   •   ppiipp iinnssttaallll ffaassttddeevv
---- > Type Less, Code More ## Features - **Reasearch oriented**, provide a set
-of tools for vision and robotics research - **User friendly**, provide simple-
-yet-flexible APIs to reduce boilerplate code - **Strong typed**, provide type
-checking and code completion ## Installation The package is available on PyPI,
-you can install it via pip: ```shell pip install fastdev ``` Or you can install
-the latest version from the source code: ```shell pip install "git+https://
-github.com/jianglongye/fastdev.git" ```
+--- > Type Less, Code More ## Features ð - **Reasearch oriented**, provide a
+set of tools for vision and robotics research - **User friendly**, provide
+simple-yet-flexible APIs to reduce boilerplate code - **Strong typed**, provide
+type checking and code completion ## Installation The package is available on
+PyPI, you can install it via pip: ```shell pip install fastdev ``` Or you can
+install the latest version from the source code: ```shell pip install
+"git+https://github.com/jianglongye/fastdev.git" ```
```

### Comparing `fastdev-0.0.6/src/fastdev.egg-info/SOURCES.txt` & `fastdev-0.0.7/src/fastdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.6/tests/test_io.py` & `fastdev-0.0.7/tests/test_io.py`

 * *Files identical despite different names*

