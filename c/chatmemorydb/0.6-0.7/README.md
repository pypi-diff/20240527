# Comparing `tmp/chatmemorydb-0.6.tar.gz` & `tmp/chatmemorydb-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatmemorydb-0.6.tar", last modified: Sun Apr 21 21:19:56 2024, max compression
+gzip compressed data, was "chatmemorydb-0.7.tar", last modified: Mon May 27 18:31:25 2024, max compression
```

## Comparing `chatmemorydb-0.6.tar` & `chatmemorydb-0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-21 21:19:56.775592 chatmemorydb-0.6/
--rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-21 19:11:21.000000 chatmemorydb-0.6/LICENSE
--rw-r--r--   0 moro      (1000) moro      (1000)     7247 2024-04-21 21:19:56.775592 chatmemorydb-0.6/PKG-INFO
--rw-r--r--   0 moro      (1000) moro      (1000)     6768 2024-02-28 22:04:17.000000 chatmemorydb-0.6/README.md
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-21 21:19:56.775592 chatmemorydb-0.6/chatmemorydb.egg-info/
--rw-r--r--   0 moro      (1000) moro      (1000)     7247 2024-04-21 21:19:56.000000 chatmemorydb-0.6/chatmemorydb.egg-info/PKG-INFO
--rw-r--r--   0 moro      (1000) moro      (1000)      442 2024-04-21 21:19:56.000000 chatmemorydb-0.6/chatmemorydb.egg-info/SOURCES.txt
--rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-04-21 21:19:56.000000 chatmemorydb-0.6/chatmemorydb.egg-info/dependency_links.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       74 2024-04-21 21:19:56.000000 chatmemorydb-0.6/chatmemorydb.egg-info/requires.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       13 2024-04-21 21:19:56.000000 chatmemorydb-0.6/chatmemorydb.egg-info/top_level.txt
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-21 21:19:56.775592 chatmemorydb-0.6/memory/
--rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 19:11:44.000000 chatmemorydb-0.6/memory/__init__.py
--rw-r--r--   0 moro      (1000) moro      (1000)    10056 2024-02-28 23:45:55.000000 chatmemorydb-0.6/memory/brain.py
--rw-r--r--   0 moro      (1000) moro      (1000)     1185 2024-04-21 21:12:53.000000 chatmemorydb-0.6/memory/embeddings.py
--rw-r--r--   0 moro      (1000) moro      (1000)      139 2024-02-21 19:37:35.000000 chatmemorydb-0.6/memory/log_util.py
--rw-r--r--   0 moro      (1000) moro      (1000)     2086 2024-02-22 19:48:44.000000 chatmemorydb-0.6/memory/summarization.py
--rwxrwxrwx   0 moro      (1000) moro      (1000)      642 2024-04-21 21:19:23.000000 chatmemorydb-0.6/pyproject.toml
--rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-04-21 21:19:56.775592 chatmemorydb-0.6/setup.cfg
--rwxrwxrwx   0 moro      (1000) moro      (1000)      660 2024-04-21 21:19:23.000000 chatmemorydb-0.6/setup.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-21 21:19:56.775592 chatmemorydb-0.6/tests/
--rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 23:22:48.000000 chatmemorydb-0.6/tests/__init__.py
--rw-r--r--   0 moro      (1000) moro      (1000)      418 2024-04-21 21:18:33.000000 chatmemorydb-0.6/tests/test_embedding_extraction.py
--rw-r--r--   0 moro      (1000) moro      (1000)      167 2024-02-21 23:23:40.000000 chatmemorydb-0.6/tests/test_logger.py
--rw-r--r--   0 moro      (1000) moro      (1000)    10784 2024-04-21 21:17:49.000000 chatmemorydb-0.6/tests/test_memory.py
--rw-r--r--   0 moro      (1000) moro      (1000)     2611 2024-02-22 19:48:34.000000 chatmemorydb-0.6/tests/test_summarization.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-05-27 18:31:25.777928 chatmemorydb-0.7/
+-rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-21 19:11:21.000000 chatmemorydb-0.7/LICENSE
+-rw-r--r--   0 moro      (1000) moro      (1000)     7247 2024-05-27 18:31:25.777928 chatmemorydb-0.7/PKG-INFO
+-rw-r--r--   0 moro      (1000) moro      (1000)     6768 2024-02-28 22:04:17.000000 chatmemorydb-0.7/README.md
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-05-27 18:31:25.777928 chatmemorydb-0.7/chatmemorydb.egg-info/
+-rw-r--r--   0 moro      (1000) moro      (1000)     7247 2024-05-27 18:31:25.000000 chatmemorydb-0.7/chatmemorydb.egg-info/PKG-INFO
+-rw-r--r--   0 moro      (1000) moro      (1000)      442 2024-05-27 18:31:25.000000 chatmemorydb-0.7/chatmemorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-05-27 18:31:25.000000 chatmemorydb-0.7/chatmemorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       74 2024-05-27 18:31:25.000000 chatmemorydb-0.7/chatmemorydb.egg-info/requires.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       13 2024-05-27 18:31:25.000000 chatmemorydb-0.7/chatmemorydb.egg-info/top_level.txt
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-05-27 18:31:25.777928 chatmemorydb-0.7/memory/
+-rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 19:11:44.000000 chatmemorydb-0.7/memory/__init__.py
+-rw-r--r--   0 moro      (1000) moro      (1000)     9914 2024-05-27 18:29:48.000000 chatmemorydb-0.7/memory/brain.py
+-rw-r--r--   0 moro      (1000) moro      (1000)     1185 2024-04-21 21:12:53.000000 chatmemorydb-0.7/memory/embeddings.py
+-rw-r--r--   0 moro      (1000) moro      (1000)      139 2024-02-21 19:37:35.000000 chatmemorydb-0.7/memory/log_util.py
+-rw-r--r--   0 moro      (1000) moro      (1000)     2086 2024-02-22 19:48:44.000000 chatmemorydb-0.7/memory/summarization.py
+-rwxrwxrwx   0 moro      (1000) moro      (1000)      642 2024-05-27 18:30:52.000000 chatmemorydb-0.7/pyproject.toml
+-rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-05-27 18:31:25.777928 chatmemorydb-0.7/setup.cfg
+-rwxrwxrwx   0 moro      (1000) moro      (1000)      660 2024-05-27 18:30:52.000000 chatmemorydb-0.7/setup.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-05-27 18:31:25.777928 chatmemorydb-0.7/tests/
+-rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-21 23:22:48.000000 chatmemorydb-0.7/tests/__init__.py
+-rw-r--r--   0 moro      (1000) moro      (1000)      418 2024-04-21 21:18:33.000000 chatmemorydb-0.7/tests/test_embedding_extraction.py
+-rw-r--r--   0 moro      (1000) moro      (1000)      167 2024-02-21 23:23:40.000000 chatmemorydb-0.7/tests/test_logger.py
+-rw-r--r--   0 moro      (1000) moro      (1000)    10784 2024-04-21 21:17:49.000000 chatmemorydb-0.7/tests/test_memory.py
+-rw-r--r--   0 moro      (1000) moro      (1000)     2611 2024-02-22 19:48:34.000000 chatmemorydb-0.7/tests/test_summarization.py
```

### Comparing `chatmemorydb-0.6/LICENSE` & `chatmemorydb-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.6/PKG-INFO` & `chatmemorydb-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatmemorydb
-Version: 0.6
+Version: 0.7
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro/ChatMemory
 Project-URL: Bug Tracker, https://github.com/cnmoro/ChatMemory/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chatmemorydb-0.6/README.md` & `chatmemorydb-0.7/README.md`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.6/chatmemorydb.egg-info/PKG-INFO` & `chatmemorydb-0.7/chatmemorydb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatmemorydb
-Version: 0.6
+Version: 0.7
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro/ChatMemory
 Project-URL: Bug Tracker, https://github.com/cnmoro/ChatMemory/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chatmemorydb-0.6/memory/brain.py` & `chatmemorydb-0.7/memory/brain.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,14 @@
             self.DUMMY_EMBEDDING = extract_embeddings_free("Hello", self.free_embedding_model_type)
         else:
             self.DUMMY_EMBEDDING = self.extract_embeddings_wrapper("Hello")
 
         self.db_client = MongitaClientDisk(self.db_location)
         self.db_coll = self.db_client["chat_db"]["chat_sessions"]
 
-        # Ensure index creation
-        self.db_coll.create_index([("session_id", 1)])
-        self.db_coll.create_index([("timestamp", 1)])
-
     def summarize(self, text):
         """
         Summarizes the given text.
         """
         if self.summarization_function is not None:
             return self.summarization_function(text)
         else:
```

### Comparing `chatmemorydb-0.6/memory/embeddings.py` & `chatmemorydb-0.7/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.6/memory/summarization.py` & `chatmemorydb-0.7/memory/summarization.py`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.6/pyproject.toml` & `chatmemorydb-0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "mongita", "logzero", "sumy", "langdetect", "openai", "minivectordb", "text-util-en-pt", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatmemorydb"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Carlo Moro", email="cnmoro@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chatmemorydb-0.6/setup.py` & `chatmemorydb-0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chatmemorydb',
-    version='0.6',
+    version='0.7',
     author='Carlo Moro',
     author_email='cnmoro@gmail.com',
     description="Memory",
     packages=find_packages(),
     package_data={
     },
     include_package_data=True,
```

### Comparing `chatmemorydb-0.6/tests/test_memory.py` & `chatmemorydb-0.7/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `chatmemorydb-0.6/tests/test_summarization.py` & `chatmemorydb-0.7/tests/test_summarization.py`

 * *Files identical despite different names*

