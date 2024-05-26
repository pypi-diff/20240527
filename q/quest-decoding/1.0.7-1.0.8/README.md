# Comparing `tmp/quest-decoding-1.0.7.tar.gz` & `tmp/quest-decoding-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quest-decoding-1.0.7.tar", last modified: Sun May 26 23:34:38 2024, max compression
+gzip compressed data, was "quest-decoding-1.0.8.tar", last modified: Sun May 26 23:40:08 2024, max compression
```

## Comparing `quest-decoding-1.0.7.tar` & `quest-decoding-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:34:38.506812 quest-decoding-1.0.7/
--rw-rw-r--   0 graf      (1017) graf      (1017)    11427 2024-05-26 21:40:16.000000 quest-decoding-1.0.7/LICENSE
--rw-rw-r--   0 graf      (1017) graf      (1017)      266 2024-05-26 22:47:51.000000 quest-decoding-1.0.7/MANIFEST.in
--rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:34:38.506812 quest-decoding-1.0.7/PKG-INFO
--rw-rw-r--   0 graf      (1017) graf      (1017)     3542 2024-05-26 22:30:17.000000 quest-decoding-1.0.7/README.md
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:34:38.502812 quest-decoding-1.0.7/quest/
--rw-rw-r--   0 graf      (1017) graf      (1017)      243 2024-05-26 21:31:54.000000 quest-decoding-1.0.7/quest/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)    21283 2024-05-26 21:59:41.000000 quest-decoding-1.0.7/quest/decoding.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1397 2024-05-26 23:34:15.000000 quest-decoding-1.0.7/quest/index.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:34:38.502812 quest-decoding-1.0.7/quest/model/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:22:51.000000 quest-decoding-1.0.7/quest/model/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2817 2024-05-24 12:23:26.000000 quest-decoding-1.0.7/quest/model/base.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     4225 2024-05-24 12:38:57.000000 quest-decoding-1.0.7/quest/model/vllm.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:34:38.502812 quest-decoding-1.0.7/quest/reward/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:31:11.000000 quest-decoding-1.0.7/quest/reward/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      747 2024-05-24 11:17:11.000000 quest-decoding-1.0.7/quest/reward/base.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     2099 2024-05-24 14:18:37.000000 quest-decoding-1.0.7/quest/reward/model.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1726 2024-05-25 14:52:55.000000 quest-decoding-1.0.7/quest/reward/qe.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:34:38.502812 quest-decoding-1.0.7/quest/utils/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-26 22:53:36.000000 quest-decoding-1.0.7/quest/utils/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      123 2024-05-23 14:15:41.000000 quest-decoding-1.0.7/quest/utils/list.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      130 2024-05-24 12:10:42.000000 quest-decoding-1.0.7/quest/utils/logger.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      443 2024-05-24 12:26:33.000000 quest-decoding-1.0.7/quest/utils/math.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:34:38.502812 quest-decoding-1.0.7/quest_decoding.egg-info/
--rw-r--r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:34:38.000000 quest-decoding-1.0.7/quest_decoding.egg-info/PKG-INFO
--rw-rw-r--   0 graf      (1017) graf      (1017)      657 2024-05-26 23:34:38.000000 quest-decoding-1.0.7/quest_decoding.egg-info/SOURCES.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)        1 2024-05-26 23:34:38.000000 quest-decoding-1.0.7/quest_decoding.egg-info/dependency_links.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       85 2024-05-26 23:34:38.000000 quest-decoding-1.0.7/quest_decoding.egg-info/requires.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       12 2024-05-26 23:34:38.000000 quest-decoding-1.0.7/quest_decoding.egg-info/top_level.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)      134 2024-05-26 23:26:46.000000 quest-decoding-1.0.7/requirements.txt
--rw-rw-r--   0 graf      (1017) graf      (1017)       38 2024-05-26 23:34:38.506812 quest-decoding-1.0.7/setup.cfg
--rw-rw-r--   0 graf      (1017) graf      (1017)      891 2024-05-26 23:34:33.000000 quest-decoding-1.0.7/setup.py
-drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:34:38.502812 quest-decoding-1.0.7/tests/
--rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:23:01.000000 quest-decoding-1.0.7/tests/__init__.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1372 2024-05-25 14:55:18.000000 quest-decoding-1.0.7/tests/test_decoding.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      391 2024-05-24 14:18:15.000000 quest-decoding-1.0.7/tests/test_qe.py
--rw-rw-r--   0 graf      (1017) graf      (1017)     1283 2024-05-24 14:23:10.000000 quest-decoding-1.0.7/tests/test_questqe.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      298 2024-05-24 11:15:11.000000 quest-decoding-1.0.7/tests/test_rewardmodel.py
--rw-rw-r--   0 graf      (1017) graf      (1017)      860 2024-05-24 11:16:25.000000 quest-decoding-1.0.7/tests/test_vllm.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:40:08.699372 quest-decoding-1.0.8/
+-rw-rw-r--   0 graf      (1017) graf      (1017)    11427 2024-05-26 21:40:16.000000 quest-decoding-1.0.8/LICENSE
+-rw-rw-r--   0 graf      (1017) graf      (1017)      266 2024-05-26 22:47:51.000000 quest-decoding-1.0.8/MANIFEST.in
+-rw-rw-r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:40:08.699372 quest-decoding-1.0.8/PKG-INFO
+-rw-rw-r--   0 graf      (1017) graf      (1017)     3542 2024-05-26 22:30:17.000000 quest-decoding-1.0.8/README.md
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:40:08.695372 quest-decoding-1.0.8/quest/
+-rw-rw-r--   0 graf      (1017) graf      (1017)      243 2024-05-26 21:31:54.000000 quest-decoding-1.0.8/quest/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)    21273 2024-05-26 23:39:30.000000 quest-decoding-1.0.8/quest/decoding.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1397 2024-05-26 23:39:49.000000 quest-decoding-1.0.8/quest/index.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:40:08.695372 quest-decoding-1.0.8/quest/model/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:22:51.000000 quest-decoding-1.0.8/quest/model/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2817 2024-05-24 12:23:26.000000 quest-decoding-1.0.8/quest/model/base.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     4225 2024-05-24 12:38:57.000000 quest-decoding-1.0.8/quest/model/vllm.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:40:08.695372 quest-decoding-1.0.8/quest/reward/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:31:11.000000 quest-decoding-1.0.8/quest/reward/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      747 2024-05-24 11:17:11.000000 quest-decoding-1.0.8/quest/reward/base.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     2099 2024-05-24 14:18:37.000000 quest-decoding-1.0.8/quest/reward/model.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1726 2024-05-25 14:52:55.000000 quest-decoding-1.0.8/quest/reward/qe.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:40:08.695372 quest-decoding-1.0.8/quest/utils/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-26 22:53:36.000000 quest-decoding-1.0.8/quest/utils/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      123 2024-05-23 14:15:41.000000 quest-decoding-1.0.8/quest/utils/list.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      130 2024-05-24 12:10:42.000000 quest-decoding-1.0.8/quest/utils/logger.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      443 2024-05-24 12:26:33.000000 quest-decoding-1.0.8/quest/utils/math.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:40:08.695372 quest-decoding-1.0.8/quest_decoding.egg-info/
+-rw-r--r--   0 graf      (1017) graf      (1017)     4080 2024-05-26 23:40:08.000000 quest-decoding-1.0.8/quest_decoding.egg-info/PKG-INFO
+-rw-rw-r--   0 graf      (1017) graf      (1017)      657 2024-05-26 23:40:08.000000 quest-decoding-1.0.8/quest_decoding.egg-info/SOURCES.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)        1 2024-05-26 23:40:08.000000 quest-decoding-1.0.8/quest_decoding.egg-info/dependency_links.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       85 2024-05-26 23:40:08.000000 quest-decoding-1.0.8/quest_decoding.egg-info/requires.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       12 2024-05-26 23:40:08.000000 quest-decoding-1.0.8/quest_decoding.egg-info/top_level.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)      134 2024-05-26 23:26:46.000000 quest-decoding-1.0.8/requirements.txt
+-rw-rw-r--   0 graf      (1017) graf      (1017)       38 2024-05-26 23:40:08.699372 quest-decoding-1.0.8/setup.cfg
+-rw-rw-r--   0 graf      (1017) graf      (1017)      891 2024-05-26 23:39:59.000000 quest-decoding-1.0.8/setup.py
+drwxrwxr-x   0 graf      (1017) graf      (1017)        0 2024-05-26 23:40:08.695372 quest-decoding-1.0.8/tests/
+-rw-rw-r--   0 graf      (1017) graf      (1017)        0 2024-05-23 13:23:01.000000 quest-decoding-1.0.8/tests/__init__.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1372 2024-05-25 14:55:18.000000 quest-decoding-1.0.8/tests/test_decoding.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      391 2024-05-24 14:18:15.000000 quest-decoding-1.0.8/tests/test_qe.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)     1283 2024-05-24 14:23:10.000000 quest-decoding-1.0.8/tests/test_questqe.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      298 2024-05-24 11:15:11.000000 quest-decoding-1.0.8/tests/test_rewardmodel.py
+-rw-rw-r--   0 graf      (1017) graf      (1017)      860 2024-05-24 11:16:25.000000 quest-decoding-1.0.8/tests/test_vllm.py
```

### Comparing `quest-decoding-1.0.7/LICENSE` & `quest-decoding-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/PKG-INFO` & `quest-decoding-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quest-decoding
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for sampling from intractable distributions with LLMs.
 Home-page: https://github.com/goncalo-faria/quest-decoding
 Author: Goncalo Faria, Sweta Agrawal.
 Author-email: goncalofaria.research@gmail.com, swetaagrawal20@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quest-decoding-1.0.7/README.md` & `quest-decoding-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/quest/decoding.py` & `quest-decoding-1.0.8/quest/decoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,28 +258,28 @@
         """
         previous_length = list(map(len, previous_state.completion))
         proposal_length = list(map(len, proposal_state.completion))
 
         # Calculate the log likelihood ratios for the indices
         index_log_likelihood_backward = np.array(
             [
-                self.dist.log_prob(
+                self.log_prob(
                     index=index,
                     truncation=n,
                 )
                 for index, n in zip(
                     indeces,
                     previous_length,
                 )
             ]
         )
 
         index_log_likelihood_forward = np.array(
             [
-                self.dist.log_prob(
+                self.log_prob(
                     index=index,
                     truncation=n,
                 )
                 for index, n in zip(indeces, proposal_length)
             ],
         )
```

### Comparing `quest-decoding-1.0.7/quest/index.py` & `quest-decoding-1.0.8/quest/index.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/quest/model/base.py` & `quest-decoding-1.0.8/quest/model/base.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/quest/model/vllm.py` & `quest-decoding-1.0.8/quest/model/vllm.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/quest/reward/base.py` & `quest-decoding-1.0.8/quest/reward/base.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/quest/reward/model.py` & `quest-decoding-1.0.8/quest/reward/model.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/quest/reward/qe.py` & `quest-decoding-1.0.8/quest/reward/qe.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/quest_decoding.egg-info/PKG-INFO` & `quest-decoding-1.0.8/quest_decoding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quest-decoding
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for sampling from intractable distributions with LLMs.
 Home-page: https://github.com/goncalo-faria/quest-decoding
 Author: Goncalo Faria, Sweta Agrawal.
 Author-email: goncalofaria.research@gmail.com, swetaagrawal20@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quest-decoding-1.0.7/quest_decoding.egg-info/SOURCES.txt` & `quest-decoding-1.0.8/quest_decoding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/setup.py` & `quest-decoding-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fr:
     installation_requirements = fr.readlines()
 
 setuptools.setup(
     name="quest-decoding",
-    version="1.0.7",
+    version="1.0.8",
     author="Goncalo Faria, Sweta Agrawal.",
     author_email="goncalofaria.research@gmail.com, swetaagrawal20@gmail.com",
     description="A package for sampling from intractable distributions with LLMs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/goncalo-faria/quest-decoding",
     packages=setuptools.find_packages(),
```

### Comparing `quest-decoding-1.0.7/tests/test_decoding.py` & `quest-decoding-1.0.8/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/tests/test_questqe.py` & `quest-decoding-1.0.8/tests/test_questqe.py`

 * *Files identical despite different names*

### Comparing `quest-decoding-1.0.7/tests/test_vllm.py` & `quest-decoding-1.0.8/tests/test_vllm.py`

 * *Files identical despite different names*

