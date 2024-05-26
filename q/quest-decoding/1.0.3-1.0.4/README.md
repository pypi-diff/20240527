# Comparing `tmp/quest-decoding-1.0.3.tar.gz` & `tmp/quest-decoding-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quest-decoding-1.0.3.tar", last modified: Sun May 26 23:21:03 2024, max compression
+gzip compressed data, was "quest-decoding-1.0.4.tar", last modified: Sun May 26 23:23:59 2024, max compression
```

## Comparing `quest-decoding-1.0.3.tar` & `quest-decoding-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:21:03.173425 quest-decoding-1.0.3/
--rw-rw-r--   0 graf      (1017) graf      (1017)    11427 2024-05-26 21:40:16.000000 quest-decoding-1.0.3/LICENSE
--rw-rw-r--   0 graf      (1017) graf      (1017)      266 2024-05-26 22:47:51.000000 quest-decoding-1.0.3/MANIFEST.in
--rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:21:03.173425 quest-decoding-1.0.3/PKG-INFO
--rw-rw-r--   0 graf      (1017) graf      (1017)     3542 2024-05-26 22:30:17.000000 quest-decoding-1.0.3/README.md
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:21:03.169425 quest-decoding-1.0.3/quest/
--rw-rw-r--   0 graf      (1017) graf      (1017)      243 2024-05-26 21:31:54.000000 quest-decoding-1.0.3/quest/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)    21283 2024-05-26 21:59:41.000000 quest-decoding-1.0.3/quest/decoding.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2175 2024-05-25 14:47:14.000000 quest-decoding-1.0.3/quest/index.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:21:03.169425 quest-decoding-1.0.3/quest/model/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:22:51.000000 quest-decoding-1.0.3/quest/model/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2817 2024-05-24 12:23:26.000000 quest-decoding-1.0.3/quest/model/base.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     4225 2024-05-24 12:38:57.000000 quest-decoding-1.0.3/quest/model/vllm.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:21:03.169425 quest-decoding-1.0.3/quest/reward/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:31:11.000000 quest-decoding-1.0.3/quest/reward/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      747 2024-05-24 11:17:11.000000 quest-decoding-1.0.3/quest/reward/base.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2099 2024-05-24 14:18:37.000000 quest-decoding-1.0.3/quest/reward/model.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1726 2024-05-25 14:52:55.000000 quest-decoding-1.0.3/quest/reward/qe.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:21:03.169425 quest-decoding-1.0.3/quest/utils/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-26 22:53:36.000000 quest-decoding-1.0.3/quest/utils/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      123 2024-05-23 14:15:41.000000 quest-decoding-1.0.3/quest/utils/list.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      130 2024-05-24 12:10:42.000000 quest-decoding-1.0.3/quest/utils/logger.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      443 2024-05-24 12:26:33.000000 quest-decoding-1.0.3/quest/utils/math.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:21:03.173425 quest-decoding-1.0.3/quest_decoding.egg-info/
--rw-r--r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:21:03.000000 quest-decoding-1.0.3/quest_decoding.egg-info/PKG-INFO
--rw-rw-r--   0 graf      (1017) graf      (1017)      657 2024-05-26 23:21:03.000000 quest-decoding-1.0.3/quest_decoding.egg-info/SOURCES.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)        1 2024-05-26 23:21:03.000000 quest-decoding-1.0.3/quest_decoding.egg-info/dependency_links.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)      118 2024-05-26 23:21:03.000000 quest-decoding-1.0.3/quest_decoding.egg-info/requires.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       12 2024-05-26 23:21:03.000000 quest-decoding-1.0.3/quest_decoding.egg-info/top_level.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)      130 2024-05-26 23:07:50.000000 quest-decoding-1.0.3/requirements.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       38 2024-05-26 23:21:03.173425 quest-decoding-1.0.3/setup.cfg
--rw-rw-r--   0 graf      (1017) graf      (1017)      891 2024-05-26 23:20:03.000000 quest-decoding-1.0.3/setup.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:21:03.173425 quest-decoding-1.0.3/tests/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:23:01.000000 quest-decoding-1.0.3/tests/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1372 2024-05-25 14:55:18.000000 quest-decoding-1.0.3/tests/test_decoding.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      391 2024-05-24 14:18:15.000000 quest-decoding-1.0.3/tests/test_qe.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1283 2024-05-24 14:23:10.000000 quest-decoding-1.0.3/tests/test_questqe.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      298 2024-05-24 11:15:11.000000 quest-decoding-1.0.3/tests/test_rewardmodel.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      860 2024-05-24 11:16:25.000000 quest-decoding-1.0.3/tests/test_vllm.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/
+-rw-rw-r--   0 graf      (1017) graf      (1017)    11427 2024-05-26 21:40:16.000000 quest-decoding-1.0.4/LICENSE
+-rw-rw-r--   0 graf      (1017) graf      (1017)      266 2024-05-26 22:47:51.000000 quest-decoding-1.0.4/MANIFEST.in
+-rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/PKG-INFO
+-rw-rw-r--   0 graf      (1017) graf      (1017)     3542 2024-05-26 22:30:17.000000 quest-decoding-1.0.4/README.md
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/quest/
+-rw-rw-r--   0 graf      (1017) graf      (1017)      243 2024-05-26 21:31:54.000000 quest-decoding-1.0.4/quest/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)    21283 2024-05-26 21:59:41.000000 quest-decoding-1.0.4/quest/decoding.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2175 2024-05-25 14:47:14.000000 quest-decoding-1.0.4/quest/index.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/quest/model/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:22:51.000000 quest-decoding-1.0.4/quest/model/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2817 2024-05-24 12:23:26.000000 quest-decoding-1.0.4/quest/model/base.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     4225 2024-05-24 12:38:57.000000 quest-decoding-1.0.4/quest/model/vllm.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/quest/reward/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:31:11.000000 quest-decoding-1.0.4/quest/reward/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      747 2024-05-24 11:17:11.000000 quest-decoding-1.0.4/quest/reward/base.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2099 2024-05-24 14:18:37.000000 quest-decoding-1.0.4/quest/reward/model.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1726 2024-05-25 14:52:55.000000 quest-decoding-1.0.4/quest/reward/qe.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/quest/utils/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-26 22:53:36.000000 quest-decoding-1.0.4/quest/utils/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      123 2024-05-23 14:15:41.000000 quest-decoding-1.0.4/quest/utils/list.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      130 2024-05-24 12:10:42.000000 quest-decoding-1.0.4/quest/utils/logger.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      443 2024-05-24 12:26:33.000000 quest-decoding-1.0.4/quest/utils/math.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/quest_decoding.egg-info/
+-rw-r--r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:23:59.000000 quest-decoding-1.0.4/quest_decoding.egg-info/PKG-INFO
+-rw-rw-r--   0 graf      (1017) graf      (1017)      657 2024-05-26 23:23:59.000000 quest-decoding-1.0.4/quest_decoding.egg-info/SOURCES.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)        1 2024-05-26 23:23:59.000000 quest-decoding-1.0.4/quest_decoding.egg-info/dependency_links.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)      118 2024-05-26 23:23:59.000000 quest-decoding-1.0.4/quest_decoding.egg-info/requires.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       12 2024-05-26 23:23:59.000000 quest-decoding-1.0.4/quest_decoding.egg-info/top_level.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)      130 2024-05-26 23:07:50.000000 quest-decoding-1.0.4/requirements.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       38 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/setup.cfg
+-rw-rw-r--   0 graf      (1017) graf      (1017)      891 2024-05-26 23:23:52.000000 quest-decoding-1.0.4/setup.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:23:59.237725 quest-decoding-1.0.4/tests/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:23:01.000000 quest-decoding-1.0.4/tests/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1372 2024-05-25 14:55:18.000000 quest-decoding-1.0.4/tests/test_decoding.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      391 2024-05-24 14:18:15.000000 quest-decoding-1.0.4/tests/test_qe.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1283 2024-05-24 14:23:10.000000 quest-decoding-1.0.4/tests/test_questqe.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      298 2024-05-24 11:15:11.000000 quest-decoding-1.0.4/tests/test_rewardmodel.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      860 2024-05-24 11:16:25.000000 quest-decoding-1.0.4/tests/test_vllm.py
```

### Comparing `quest-decoding-1.0.3/LICENSE` & `quest-decoding-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/PKG-INFO` & `quest-decoding-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quest-decoding
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for sampling from intractable distributions with LLMs.
 Home-page: https://github.com/goncalo-faria/quest-decoding
 Author: Goncalo Faria, Sweta Agrawal.
 Author-email: goncalofaria.research@gmail.com, swetaagrawal20@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quest-decoding-1.0.3/README.md` & `quest-decoding-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest/decoding.py` & `quest-decoding-1.0.4/quest/decoding.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest/index.py` & `quest-decoding-1.0.4/quest/index.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest/model/base.py` & `quest-decoding-1.0.4/quest/model/base.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest/model/vllm.py` & `quest-decoding-1.0.4/quest/model/vllm.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest/reward/base.py` & `quest-decoding-1.0.4/quest/reward/base.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest/reward/model.py` & `quest-decoding-1.0.4/quest/reward/model.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest/reward/qe.py` & `quest-decoding-1.0.4/quest/reward/qe.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/quest_decoding.egg-info/PKG-INFO` & `quest-decoding-1.0.4/quest_decoding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quest-decoding
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for sampling from intractable distributions with LLMs.
 Home-page: https://github.com/goncalo-faria/quest-decoding
 Author: Goncalo Faria, Sweta Agrawal.
 Author-email: goncalofaria.research@gmail.com, swetaagrawal20@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quest-decoding-1.0.3/quest_decoding.egg-info/SOURCES.txt` & `quest-decoding-1.0.4/quest_decoding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/setup.py` & `quest-decoding-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fr:
     installation_requirements = fr.readlines()
 
 setuptools.setup(
     name="quest-decoding",
-    version="1.0.3",
+    version="1.0.4",
     author="Goncalo Faria, Sweta Agrawal.",
     author_email="goncalofaria.research@gmail.com, swetaagrawal20@gmail.com",
     description="A package for sampling from intractable distributions with LLMs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/goncalo-faria/quest-decoding",
     packages=setuptools.find_packages(),
```

### Comparing `quest-decoding-1.0.3/tests/test_decoding.py` & `quest-decoding-1.0.4/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/tests/test_questqe.py` & `quest-decoding-1.0.4/tests/test_questqe.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.3/tests/test_vllm.py` & `quest-decoding-1.0.4/tests/test_vllm.py`

 * *Files identical despite different names*

