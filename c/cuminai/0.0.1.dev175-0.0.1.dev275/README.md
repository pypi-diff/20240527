# Comparing `tmp/cuminai-0.0.1.dev175.tar.gz` & `tmp/cuminai-0.0.1.dev275.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuminai-0.0.1.dev175.tar", max compression
+gzip compressed data, was "cuminai-0.0.1.dev275.tar", max compression
```

## Comparing `cuminai-0.0.1.dev175.tar` & `cuminai-0.0.1.dev275.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       75 2024-05-12 07:46:46.527637 cuminai-0.0.1.dev175/cuminai/__init__.py
--rw-r--r--   0        0        0      691 2024-05-15 18:12:16.655249 cuminai-0.0.1.dev175/cuminai/constants.py
--rw-r--r--   0        0        0     2466 2024-05-15 10:54:39.551320 cuminai-0.0.1.dev175/cuminai/contextstores.py
--rw-r--r--   0        0        0    12718 2024-05-16 19:49:15.267475 cuminai-0.0.1.dev175/cuminai/creator.py
--rw-r--r--   0        0        0      575 2024-05-16 19:30:39.564649 cuminai-0.0.1.dev175/cuminai/validator.py
--rw-r--r--   0        0        0    11558 2024-05-11 18:16:30.219425 cuminai-0.0.1.dev175/LICENSE
--rw-r--r--   0        0        0      569 2024-05-16 19:34:50.032171 cuminai-0.0.1.dev175/pyproject.toml
--rw-r--r--   0        0        0     3135 2024-05-16 19:58:36.161593 cuminai-0.0.1.dev175/README.md
--rw-r--r--   0        0        0     3754 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev175/PKG-INFO
+-rw-r--r--   0        0        0       75 2024-05-12 07:46:46.527637 cuminai-0.0.1.dev275/cuminai/__init__.py
+-rw-r--r--   0        0        0      613 2024-05-27 13:46:42.872184 cuminai-0.0.1.dev275/cuminai/constants.py
+-rw-r--r--   0        0        0     2576 2024-05-27 20:06:10.643890 cuminai-0.0.1.dev275/cuminai/contextstores.py
+-rw-r--r--   0        0        0    13607 2024-05-27 18:14:01.118580 cuminai-0.0.1.dev275/cuminai/creator.py
+-rw-r--r--   0        0        0      575 2024-05-16 19:30:39.564649 cuminai-0.0.1.dev275/cuminai/validator.py
+-rw-r--r--   0        0        0    11558 2024-05-11 18:16:30.219425 cuminai-0.0.1.dev275/LICENSE
+-rw-r--r--   0        0        0      558 2024-05-27 13:45:37.883875 cuminai-0.0.1.dev275/pyproject.toml
+-rw-r--r--   0        0        0     3135 2024-05-16 19:58:36.161593 cuminai-0.0.1.dev275/README.md
+-rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev275/PKG-INFO
```

### Comparing `cuminai-0.0.1.dev175/cuminai/constants.py` & `cuminai-0.0.1.dev275/cuminai/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Creator constants
 _CUMINAI_CONFIG_DIR = ".cuminai"
 _CUMINAI_CONFIG_FILE = "config.yaml"
 _CUMIN_FILE_NAME = "CUMINFILE.yaml"
 _CUMINAI_CREATOR_HOST = "https://api.creator.cuminai.com"
 
 # Client constants
-_CUMINAI_DUMMY_TENANT_NAME = "dummy"
-_CUMINAI_DUMMY_DATABASE_NAME = "dummy"
 _CUMINAI_DUMMY_COLLECTION_NAME = "dummy"
 _CUMINAI_API_KEY_ENV = "CUMINAI_API_KEY"
 _CUMINAI_HOST = "https://api.cuminai.com"
 
 # Knowledge Kinds
 _LINK_KIND = 'LINK'
```

### Comparing `cuminai-0.0.1.dev175/cuminai/creator.py` & `cuminai-0.0.1.dev275/cuminai/creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 import http.client
 import yaml
 from cuminai.constants import (
     _CUMINAI_CONFIG_DIR,
     _CUMINAI_CONFIG_FILE,
     _CUMINAI_CREATOR_HOST,
     _CUMIN_FILE_NAME,
-    _CUMINAI_DUMMY_TENANT_NAME,
-    _CUMINAI_DUMMY_DATABASE_NAME,
     _LINK_KIND,
     _PUBLIC_VISIBILITY,
     _PRIVATE_VISIBILITY,
     _GLOBAL_TAGGING,
     _LOCAL_TAGGING,
     _DEFAULT_CHUNK_SIZE,
-    _DEFAULT_CHUNK_OVERLAP
+    _DEFAULT_CHUNK_OVERLAP,
+    _CUMINAI_DUMMY_COLLECTION_NAME,
 )
 
 import cuminai.validator as validator
 
 from langchain_community.embeddings import OllamaEmbeddings
 from langchain_community.document_loaders import WebBaseLoader
 from langchain_text_splitters import CharacterTextSplitter
-from langchain_chroma import Chroma
-import chromadb
+import qdrant_client
+from langchain_qdrant import Qdrant
 
 @click.group()
 def executor():
     pass
 
 @executor.command(help='Log in to a Cumin AI managed knowledge store')
 @click.option('-u', '--username',  help='username', required=True)
@@ -44,15 +43,15 @@
 
     if apikey == "":
         click.echo("apikey can't be empty")
         return
 
     # validate the client credentials from Cumin AI
     connection = http.client.HTTPSConnection("api.creator.cuminai.com", timeout=10)
-    connection.request("GET", "/v1/creator/auth/verify", headers={
+    connection.request("GET", "/v1/login/verify", headers={
         "CUMINAI-API-KEY": apikey,
         "CUMINAI-CLIENT-ID": username
     })
     response = connection.getresponse()
     if response.status != 200:
         click.echo("Login failed: invalid client credentials. please try again with correct username and apikey combination.")
         return
@@ -174,63 +173,88 @@
         tags[source['link']] = source['metadata']['tags']
 
     tag_type = cuminfile['tag']['type']
 
     if tag_type == _GLOBAL_TAGGING:
         for doc in doc_splits:
             for tag in tags[doc.metadata['source']]:
-                doc.metadata[f'tag-{tag}'] = True
+                processed_tag = tag.lower().replace("-","_").replace(" ", "_")
+                doc.metadata[f'tag-{processed_tag}'] = True
     elif tag_type == _LOCAL_TAGGING:
         tag_min_occur_th = cuminfile['tag']['minoccurances']
         for doc in doc_splits:
             for tag in tags[doc.metadata['source']]:
-                if doc.page_content.count(tag) >= tag_min_occur_th:
-                     doc.metadata[f'tag:{tag.lower()}'] = True
+                processed_tag = tag.lower().replace("-","_").replace(" ", "_")
+                if doc.page_content.lower().count(tag.lower()) >= tag_min_occur_th:
+                     doc.metadata[f'tag-{processed_tag}'] = True
 
     click.echo("knowledge metadata enriched")
 
     match = validator.OllamaEmbeddingFetcher.match(cuminfile['embedding'])
     ollama_embedding_name = match.groups(1)[0]
     embedding_function = OllamaEmbeddings(model=ollama_embedding_name)
 
     is_public_header = "false"
     if cuminfile['type'] == _PUBLIC_VISIBILITY:
         is_public_header = "true"
 
     click.echo("Deploying knowledge to Cumin AI...")
 
-    chroma_client = None
+    chroma_client = qdrant_client.QdrantClient(
+        url=_CUMINAI_CREATOR_HOST, 
+        port=443,
+        https=True,
+        metadata={
+            "CUMINAI-API-KEY": creds['apikey'],
+            "CUMINAI-KB-NAME": cuminfile['name'],
+            "CUMINAI-IS-PUBLIC": is_public_header,
+        }
+    )
+
     try:
-        chroma_client = chromadb.HttpClient(host=_CUMINAI_CREATOR_HOST, 
-                                            port=443, 
-                                            tenant=_CUMINAI_DUMMY_TENANT_NAME, 
-                                            database=_CUMINAI_DUMMY_DATABASE_NAME, 
-                                            ssl=True, 
-                                            headers={
-                                                "CUMINAI-API-KEY": creds['apikey'],
-                                                "CUMINAI-KB-NAME": cuminfile['name'],
-                                                "CUMINAI-IS-PUBLIC": is_public_header,
-                                            }
+        store = Qdrant(
+            client=chroma_client,
+            collection_name=_CUMINAI_DUMMY_COLLECTION_NAME,
+            embeddings=embedding_function,
         )
+
+        store.add_documents(documents=doc_splits)
+        click.echo(f"knowledge deployed and is available at @{creds['username']}/{cuminfile['name']}")
+        return
+    except qdrant_client.http.exceptions.UnexpectedResponse as e:
+        if e.status_code != 404:
+            click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
+            return
+        click.echo(f"knowledge source {cuminfile['name']} doesn't exist.")
     except ValueError as e:
-        click.echo("Failed to connect to Cumin AI. Please try again after sometime")
+        click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
         return
-
+    
     try:
-        Chroma.from_documents(
-            client=chroma_client,
+        click.echo(f"creating knowledge source {cuminfile['name']} and uploading knowledge...")
+        _ = Qdrant.from_documents(
             documents=doc_splits,
-            collection_name=cuminfile['name'],
+            collection_name=_CUMINAI_DUMMY_COLLECTION_NAME,
             embedding=embedding_function,
+            url=_CUMINAI_CREATOR_HOST, 
+            port=443,
+            https=True,
+            metadata={
+                "CUMINAI-API-KEY": creds['apikey'],
+                "CUMINAI-KB-NAME": cuminfile['name'],
+                "CUMINAI-IS-PUBLIC": is_public_header,
+            }
         )
+        click.echo(f"knowledge deployed and is available at @{creds['username']}/{cuminfile['name']}")
+    except qdrant_client.http.exceptions.UnexpectedResponse as e:
+        click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
+        return
     except ValueError as e:
         click.echo("Oops... something went wrong. Failed to deploy to Cumin AI")
         return
-    
-    click.echo(f"knowledge deployed and is available at @{creds['username']}/{cuminfile['name']}")
 
 def _validate(projectdir, get_parsed=False):
     data = {}
     with open(os.path.join(projectdir, _CUMIN_FILE_NAME), 'r') as f:
         try:
             data = yaml.safe_load(f)
         except:
```

### Comparing `cuminai-0.0.1.dev175/cuminai/validator.py` & `cuminai-0.0.1.dev275/cuminai/validator.py`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev175/LICENSE` & `cuminai-0.0.1.dev275/LICENSE`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev175/pyproject.toml` & `cuminai-0.0.1.dev275/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "cuminai"
-version = "0.0.1dev175"
+version = "0.0.1dev275"
 description = ""
 authors = ["Harshal Priyadarshi <harshal@cuminai.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-numpy = "^1"
-langchain-chroma = ">=0.1.1"
-chromadb = { version = ">=0.4.0,<0.6.0" }
+langchain_qdrant = ">=0.1.0"
+qdrant-client = ">=1.0.0"
 langchain-community = ">=0.0.10"
 langchain_text_splitters = ">=0.0.1"
 beautifulsoup4 = ">=4.10.0"
 tiktoken = ">=0.4.0"
+click = ">=8.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 cuminai = "cuminai.creator:executor"
```

### Comparing `cuminai-0.0.1.dev175/README.md` & `cuminai-0.0.1.dev275/README.md`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev175/PKG-INFO` & `cuminai-0.0.1.dev275/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cuminai
-Version: 0.0.1.dev175
+Version: 0.0.1.dev275
 Summary: 
 Author: Harshal Priyadarshi
 Author-email: harshal@cuminai.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.10.0)
-Requires-Dist: chromadb (>=0.4.0,<0.6.0)
-Requires-Dist: langchain-chroma (>=0.1.1)
+Requires-Dist: click (>=8.1.0)
 Requires-Dist: langchain-community (>=0.0.10)
+Requires-Dist: langchain_qdrant (>=0.1.0)
 Requires-Dist: langchain_text_splitters (>=0.0.1)
-Requires-Dist: numpy (>=1,<2)
+Requires-Dist: qdrant-client (>=1.0.0)
 Requires-Dist: tiktoken (>=0.4.0)
 Description-Content-Type: text/markdown
 
 # cuminai
 
 This package contains the Cumin AI Python SDK. Cumin AI is a Managed LLM Context Service. This package provides integration with Langchain.
```

