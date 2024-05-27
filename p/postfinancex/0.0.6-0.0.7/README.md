# Comparing `tmp/postfinancex-0.0.6.tar.gz` & `tmp/postfinancex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfinancex-0.0.6.tar", max compression
+gzip compressed data, was "postfinancex-0.0.7.tar", max compression
```

## Comparing `postfinancex-0.0.6.tar` & `postfinancex-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.6/LICENSE
--rw-r--r--   0        0        0     1406 2024-05-27 00:32:46.191007 postfinancex-0.0.6/README.md
--rw-r--r--   0        0        0      315 2024-05-27 02:03:46.094859 postfinancex-0.0.6/postfinance/__init__.py
--rw-r--r--   0        0        0     2729 2024-05-27 00:11:45.515399 postfinancex-0.0.6/postfinance/agent.py
--rw-r--r--   0        0        0    10494 2024-05-27 02:20:15.219075 postfinancex-0.0.6/postfinance/annotate.py
--rw-r--r--   0        0        0     3797 2024-05-27 00:48:22.035951 postfinancex-0.0.6/postfinance/settings.py
--rw-r--r--   0        0        0        0 2024-05-26 22:24:54.394886 postfinancex-0.0.6/postfinance/tools/__init__.py
--rw-r--r--   0        0        0     7272 2024-05-27 00:11:37.715437 postfinancex-0.0.6/postfinance/tools/graph_qa_tool.py
--rw-r--r--   0        0        0     2072 2024-05-27 00:49:47.089556 postfinancex-0.0.6/postfinance/tools/summarization_tool.py
--rw-r--r--   0        0        0     1633 2024-05-26 23:50:41.315057 postfinancex-0.0.6/postfinance/tools/translation_tool.py
--rw-r--r--   0        0        0     2039 2024-05-27 00:50:32.615892 postfinancex-0.0.6/postfinance/tools/vector_search_tool.py
--rw-r--r--   0        0        0    11121 2024-05-27 02:08:04.198793 postfinancex-0.0.6/postfinance/translate.py
--rw-r--r--   0        0        0      805 2024-05-27 02:27:15.646532 postfinancex-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 postfinancex-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1406 2024-05-27 00:32:46.191007 postfinancex-0.0.7/README.md
+-rw-r--r--   0        0        0      389 2024-05-27 04:37:44.026260 postfinancex-0.0.7/postfinance/__init__.py
+-rw-r--r--   0        0        0     2729 2024-05-27 00:11:45.515399 postfinancex-0.0.7/postfinance/agent.py
+-rw-r--r--   0        0        0    10494 2024-05-27 02:20:15.219075 postfinancex-0.0.7/postfinance/annotate.py
+-rw-r--r--   0        0        0     3797 2024-05-27 04:24:51.735184 postfinancex-0.0.7/postfinance/settings.py
+-rw-r--r--   0        0        0     1446 2024-05-27 04:36:04.514673 postfinancex-0.0.7/postfinance/storage.py
+-rw-r--r--   0        0        0        0 2024-05-26 22:24:54.394886 postfinancex-0.0.7/postfinance/tools/__init__.py
+-rw-r--r--   0        0        0     7272 2024-05-27 04:24:45.593360 postfinancex-0.0.7/postfinance/tools/graph_qa_tool.py
+-rw-r--r--   0        0        0     2062 2024-05-27 04:37:05.783729 postfinancex-0.0.7/postfinance/tools/summarization_tool.py
+-rw-r--r--   0        0        0     1633 2024-05-26 23:50:41.315057 postfinancex-0.0.7/postfinance/tools/translation_tool.py
+-rw-r--r--   0        0        0     2030 2024-05-27 04:37:02.264590 postfinancex-0.0.7/postfinance/tools/vector_search_tool.py
+-rw-r--r--   0        0        0    11121 2024-05-27 02:08:04.198793 postfinancex-0.0.7/postfinance/translate.py
+-rw-r--r--   0        0        0      805 2024-05-27 04:38:38.833363 postfinancex-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 postfinancex-0.0.7/PKG-INFO
```

### Comparing `postfinancex-0.0.6/LICENSE` & `postfinancex-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.6/README.md` & `postfinancex-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.6/postfinance/agent.py` & `postfinancex-0.0.7/postfinance/agent.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.6/postfinance/annotate.py` & `postfinancex-0.0.7/postfinance/annotate.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.6/postfinance/settings.py` & `postfinancex-0.0.7/postfinance/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         temperature=0.5,
         random_seed=0,
         repetition_penalty=1.0,
         min_new_tokens=0,
         max_new_tokens=1024,
     )
     _jina_api_key: str = ""
-    _neo4j_url: str = ""
+    _neo4j_uri: str = ""
     _neo4j_username: str = ""
     _neo4j_password: str = ""
     _mongo_uri: str = ""
     _persist_dir: str = "./storage"
     _verbose: bool = False
 
     # llm, IBM watsonx
@@ -93,20 +93,20 @@
 
     @jina_api_key.setter
     def jina_api_key(self, value: str) -> None:
         self._jina_api_key = value
 
     # graph, Neo4j Aura
     @property
-    def neo4j_url(self) -> str:
-        return self._neo4j_url
+    def neo4j_uri(self) -> str:
+        return self._neo4j_uri
 
-    @neo4j_url.setter
-    def neo4j_url(self, value: str) -> None:
-        self._neo4j_url = value
+    @neo4j_uri.setter
+    def neo4j_uri(self, value: str) -> None:
+        self._neo4j_uri = value
 
     @property
     def neo4j_username(self) -> str:
         return self._neo4j_username
 
     @neo4j_username.setter
     def neo4j_username(self, value: str) -> None:
```

### Comparing `postfinancex-0.0.6/postfinance/tools/graph_qa_tool.py` & `postfinancex-0.0.7/postfinance/tools/graph_qa_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         url=settings.watsonx_url,
         project_id=settings.watsonx_project_id,
         params=settings.watsonx_model_params.to_dict(),
     )
 
     # graph
     graph = Neo4jGraph(
-        url=settings.neo4j_url,
+        url=settings.neo4j_uri,
         username=settings.neo4j_username,
         password=settings.neo4j_password,
     )
 
     # prompts
     query_prompt = PromptTemplate.from_template(
         CYPHER_GENERATION_PROMPT_TEMPLATE
```

### Comparing `postfinancex-0.0.6/postfinance/tools/summarization_tool.py` & `postfinancex-0.0.7/postfinance/tools/summarization_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,22 +35,21 @@
     try:
         storage_context = StorageContext.from_defaults(
             persist_dir=str(pathlib.Path(settings.persist_dir) / "summary"),
         )
         summary_index = load_index_from_storage(storage_context)
     except Exception as e:
 
-        import pymongo
+        from ..storage import mongo_storage_from_uri
 
-        client = pymongo.MongoClient(settings.mongo_uri)
-        collection = client["postfinance"]["calls"]
+        mongo_storage = mongo_storage_from_uri(settings.mongo_uri)
 
         nodes = [
             TextNode(id_=c["id"], text=c["translation"])
-            for c in collection.find()
+            for c in mongo_storage.calls
         ]
 
         summary_index = SummaryIndex(nodes, embed_model=embed_model)
         summary_index.storage_context.persist(
             persist_dir=str(pathlib.Path(settings.persist_dir) / "summary"),
         )
```

### Comparing `postfinancex-0.0.6/postfinance/tools/translation_tool.py` & `postfinancex-0.0.7/postfinance/tools/translation_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.6/postfinance/tools/vector_search_tool.py` & `postfinancex-0.0.7/postfinance/tools/vector_search_tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     # index
     try:
         storage_context = StorageContext.from_defaults(
             persist_dir=str(pathlib.Path(settings.persist_dir) / "vector"),
         )
         vector_index = load_index_from_storage(storage_context)
     except Exception as e:
-        import pymongo
 
-        client = pymongo.MongoClient(settings.mongo_uri)
-        collection = client["postfinance"]["calls"]
+        from ..storage import mongo_storage_from_uri
+
+        mongo_storage = mongo_storage_from_uri(settings.mongo_uri)
 
         nodes = [
             TextNode(id_=c["id"], text=c["translation"])
-            for c in collection.find()
+            for c in mongo_storage.calls
         ]
 
         vector_index = VectorStoreIndex(nodes, embed_model=embed_model)
         vector_index.storage_context.persist(
             persist_dir=str(pathlib.Path(settings.persist_dir) / "vector"),
         )
```

### Comparing `postfinancex-0.0.6/postfinance/translate.py` & `postfinancex-0.0.7/postfinance/translate.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.6/pyproject.toml` & `postfinancex-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postfinancex"
-version = "0.0.6"
+version = "0.0.7"
 description = "PostFinanceX Virtual Assistant powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai"
 packages = [
     {include = "postfinance"}
 ]
 authors = ["Yi ZHANG <yizhang.dev@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `postfinancex-0.0.6/PKG-INFO` & `postfinancex-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfinancex
-Version: 0.0.6
+Version: 0.0.7
 Summary: PostFinanceX Virtual Assistant powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai
 Home-page: https://pypi.org/project/postfinancex
 License: BSD-3-Clause
 Author: Yi ZHANG
 Author-email: yizhang.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

