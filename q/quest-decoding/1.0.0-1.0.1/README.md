# Comparing `tmp/quest-decoding-1.0.0.tar.gz` & `tmp/quest-decoding-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quest-decoding-1.0.0.tar", last modified: Sun May 26 22:37:50 2024, max compression
+gzip compressed data, was "quest-decoding-1.0.1.tar", last modified: Sun May 26 22:51:38 2024, max compression
```

## Comparing `quest-decoding-1.0.0.tar` & `quest-decoding-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:37:50.412559 quest-decoding-1.0.0/
--rw-rw-r--   0 graf      (1017) graf      (1017)    11427 2024-05-26 21:40:16.000000 quest-decoding-1.0.0/LICENSE
--rw-rw-r--   0 graf      (1017) graf      (1017)      293 2024-05-26 22:37:28.000000 quest-decoding-1.0.0/MANIFEST.in
--rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 22:37:50.412559 quest-decoding-1.0.0/PKG-INFO
--rw-rw-r--   0 graf      (1017) graf      (1017)     3542 2024-05-26 22:30:17.000000 quest-decoding-1.0.0/README.md
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:37:50.408559 quest-decoding-1.0.0/quest/
--rw-rw-r--   0 graf      (1017) graf      (1017)      243 2024-05-26 21:31:54.000000 quest-decoding-1.0.0/quest/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)    21283 2024-05-26 21:59:41.000000 quest-decoding-1.0.0/quest/decoding.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2175 2024-05-25 14:47:14.000000 quest-decoding-1.0.0/quest/index.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:37:50.408559 quest-decoding-1.0.0/quest/model/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:22:51.000000 quest-decoding-1.0.0/quest/model/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2817 2024-05-24 12:23:26.000000 quest-decoding-1.0.0/quest/model/base.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     4225 2024-05-24 12:38:57.000000 quest-decoding-1.0.0/quest/model/vllm.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:37:50.408559 quest-decoding-1.0.0/quest/reward/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:31:11.000000 quest-decoding-1.0.0/quest/reward/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      747 2024-05-24 11:17:11.000000 quest-decoding-1.0.0/quest/reward/base.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2099 2024-05-24 14:18:37.000000 quest-decoding-1.0.0/quest/reward/model.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1726 2024-05-25 14:52:55.000000 quest-decoding-1.0.0/quest/reward/qe.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:37:50.408559 quest-decoding-1.0.0/quest_decoding.egg-info/
--rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 22:37:50.000000 quest-decoding-1.0.0/quest_decoding.egg-info/PKG-INFO
--rw-rw-r--   0 graf      (1017) graf      (1017)      571 2024-05-26 22:37:50.000000 quest-decoding-1.0.0/quest_decoding.egg-info/SOURCES.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)        1 2024-05-26 22:37:50.000000 quest-decoding-1.0.0/quest_decoding.egg-info/dependency_links.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       54 2024-05-26 22:37:50.000000 quest-decoding-1.0.0/quest_decoding.egg-info/requires.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       12 2024-05-26 22:37:50.000000 quest-decoding-1.0.0/quest_decoding.egg-info/top_level.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       54 2024-05-24 14:10:29.000000 quest-decoding-1.0.0/requirements.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       38 2024-05-26 22:37:50.412559 quest-decoding-1.0.0/setup.cfg
--rw-rw-r--   0 graf      (1017) graf      (1017)      891 2024-05-26 22:36:45.000000 quest-decoding-1.0.0/setup.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:37:50.412559 quest-decoding-1.0.0/tests/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:23:01.000000 quest-decoding-1.0.0/tests/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1372 2024-05-25 14:55:18.000000 quest-decoding-1.0.0/tests/test_decoding.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      391 2024-05-24 14:18:15.000000 quest-decoding-1.0.0/tests/test_qe.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1283 2024-05-24 14:23:10.000000 quest-decoding-1.0.0/tests/test_questqe.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      298 2024-05-24 11:15:11.000000 quest-decoding-1.0.0/tests/test_rewardmodel.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      860 2024-05-24 11:16:25.000000 quest-decoding-1.0.0/tests/test_vllm.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:51:38.482340 quest-decoding-1.0.1/
+-rw-rw-r--   0 graf      (1017) graf      (1017)    11427 2024-05-26 21:40:16.000000 quest-decoding-1.0.1/LICENSE
+-rw-rw-r--   0 graf      (1017) graf      (1017)      266 2024-05-26 22:47:51.000000 quest-decoding-1.0.1/MANIFEST.in
+-rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 22:51:38.482340 quest-decoding-1.0.1/PKG-INFO
+-rw-rw-r--   0 graf      (1017) graf      (1017)     3542 2024-05-26 22:30:17.000000 quest-decoding-1.0.1/README.md
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:51:38.478340 quest-decoding-1.0.1/quest/
+-rw-rw-r--   0 graf      (1017) graf      (1017)      243 2024-05-26 21:31:54.000000 quest-decoding-1.0.1/quest/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)    21283 2024-05-26 21:59:41.000000 quest-decoding-1.0.1/quest/decoding.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2175 2024-05-25 14:47:14.000000 quest-decoding-1.0.1/quest/index.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:51:38.478340 quest-decoding-1.0.1/quest/model/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:22:51.000000 quest-decoding-1.0.1/quest/model/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2817 2024-05-24 12:23:26.000000 quest-decoding-1.0.1/quest/model/base.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     4225 2024-05-24 12:38:57.000000 quest-decoding-1.0.1/quest/model/vllm.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:51:38.478340 quest-decoding-1.0.1/quest/reward/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:31:11.000000 quest-decoding-1.0.1/quest/reward/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      747 2024-05-24 11:17:11.000000 quest-decoding-1.0.1/quest/reward/base.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2099 2024-05-24 14:18:37.000000 quest-decoding-1.0.1/quest/reward/model.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1726 2024-05-25 14:52:55.000000 quest-decoding-1.0.1/quest/reward/qe.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:51:38.478340 quest-decoding-1.0.1/quest/utils/
+-rw-rw-r--   0 graf      (1017) graf      (1017)      123 2024-05-23 14:15:41.000000 quest-decoding-1.0.1/quest/utils/list.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      130 2024-05-24 12:10:42.000000 quest-decoding-1.0.1/quest/utils/logger.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      443 2024-05-24 12:26:33.000000 quest-decoding-1.0.1/quest/utils/math.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:51:38.482340 quest-decoding-1.0.1/quest_decoding.egg-info/
+-rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 22:51:38.000000 quest-decoding-1.0.1/quest_decoding.egg-info/PKG-INFO
+-rw-rw-r--   0 graf      (1017) graf      (1017)      633 2024-05-26 22:51:38.000000 quest-decoding-1.0.1/quest_decoding.egg-info/SOURCES.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)        1 2024-05-26 22:51:38.000000 quest-decoding-1.0.1/quest_decoding.egg-info/dependency_links.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       54 2024-05-26 22:51:38.000000 quest-decoding-1.0.1/quest_decoding.egg-info/requires.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       12 2024-05-26 22:51:38.000000 quest-decoding-1.0.1/quest_decoding.egg-info/top_level.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       54 2024-05-24 14:10:29.000000 quest-decoding-1.0.1/requirements.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       38 2024-05-26 22:51:38.482340 quest-decoding-1.0.1/setup.cfg
+-rw-rw-r--   0 graf      (1017) graf      (1017)      891 2024-05-26 22:51:31.000000 quest-decoding-1.0.1/setup.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 22:51:38.482340 quest-decoding-1.0.1/tests/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:23:01.000000 quest-decoding-1.0.1/tests/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1372 2024-05-25 14:55:18.000000 quest-decoding-1.0.1/tests/test_decoding.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      391 2024-05-24 14:18:15.000000 quest-decoding-1.0.1/tests/test_qe.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1283 2024-05-24 14:23:10.000000 quest-decoding-1.0.1/tests/test_questqe.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      298 2024-05-24 11:15:11.000000 quest-decoding-1.0.1/tests/test_rewardmodel.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      860 2024-05-24 11:16:25.000000 quest-decoding-1.0.1/tests/test_vllm.py
```

### Comparing `quest-decoding-1.0.0/LICENSE` & `quest-decoding-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/PKG-INFO` & `quest-decoding-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quest-decoding
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for sampling from intractable distributions with LLMs.
 Home-page: https://github.com/goncalo-faria/quest-decoding
 Author: Goncalo Faria, Sweta Agrawal.
 Author-email: goncalofaria.research@gmail.com, swetaagrawal20@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quest-decoding-1.0.0/README.md` & `quest-decoding-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest/decoding.py` & `quest-decoding-1.0.1/quest/decoding.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest/index.py` & `quest-decoding-1.0.1/quest/index.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest/model/base.py` & `quest-decoding-1.0.1/quest/model/base.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest/model/vllm.py` & `quest-decoding-1.0.1/quest/model/vllm.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest/reward/base.py` & `quest-decoding-1.0.1/quest/reward/base.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest/reward/model.py` & `quest-decoding-1.0.1/quest/reward/model.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest/reward/qe.py` & `quest-decoding-1.0.1/quest/reward/qe.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/quest_decoding.egg-info/PKG-INFO` & `quest-decoding-1.0.1/quest_decoding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quest-decoding
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for sampling from intractable distributions with LLMs.
 Home-page: https://github.com/goncalo-faria/quest-decoding
 Author: Goncalo Faria, Sweta Agrawal.
 Author-email: goncalofaria.research@gmail.com, swetaagrawal20@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quest-decoding-1.0.0/setup.py` & `quest-decoding-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fr:
     installation_requirements = fr.readlines()
 
 setuptools.setup(
     name="quest-decoding",
-    version="1.0.0",
+    version="1.0.1",
     author="Goncalo Faria, Sweta Agrawal.",
     author_email="goncalofaria.research@gmail.com, swetaagrawal20@gmail.com",
     description="A package for sampling from intractable distributions with LLMs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/goncalo-faria/quest-decoding",
     packages=setuptools.find_packages(),
```

### Comparing `quest-decoding-1.0.0/tests/test_decoding.py` & `quest-decoding-1.0.1/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/tests/test_questqe.py` & `quest-decoding-1.0.1/tests/test_questqe.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.0/tests/test_vllm.py` & `quest-decoding-1.0.1/tests/test_vllm.py`

 * *Files identical despite different names*

