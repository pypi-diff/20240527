# Comparing `tmp/ragoon-0.0.1.tar.gz` & `tmp/ragoon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragoon-0.0.1.tar", last modified: Sun May 26 21:54:54 2024, max compression
+gzip compressed data, was "ragoon-0.0.2.tar", last modified: Sun May 26 22:04:05 2024, max compression
```

## Comparing `ragoon-0.0.1.tar` & `ragoon-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 21:54:54.053190 ragoon-0.0.1/
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)    11357 2024-05-19 18:03:38.000000 ragoon-0.0.1/LICENSE
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     4754 2024-05-26 21:54:54.052191 ragoon-0.0.1/PKG-INFO
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     3920 2024-05-26 21:52:13.000000 ragoon-0.0.1/README.md
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     1798 2024-05-26 21:54:24.000000 ragoon-0.0.1/pyproject.toml
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)       38 2024-05-26 21:54:54.053363 ragoon-0.0.1/setup.cfg
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 21:54:54.037360 ragoon-0.0.1/src/
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 21:54:54.047086 ragoon-0.0.1/src/ragoon/
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      208 2024-05-26 21:31:34.000000 ragoon-0.0.1/src/ragoon/__init__.py
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     8080 2024-05-19 17:54:54.000000 ragoon-0.0.1/src/ragoon/_retrieval.py
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     3990 2024-04-19 22:51:33.000000 ragoon-0.0.1/src/ragoon/_scrape.py
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     2386 2024-04-20 12:11:41.000000 ragoon-0.0.1/src/ragoon/_search.py
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     4938 2024-05-26 21:34:12.000000 ragoon-0.0.1/src/ragoon/ragoon.py
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 21:54:54.050886 ragoon-0.0.1/src/ragoon.egg-info/
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     4754 2024-05-26 21:54:54.000000 ragoon-0.0.1/src/ragoon.egg-info/PKG-INFO
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      281 2024-05-26 21:54:54.000000 ragoon-0.0.1/src/ragoon.egg-info/SOURCES.txt
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        1 2024-05-26 21:54:54.000000 ragoon-0.0.1/src/ragoon.egg-info/dependency_links.txt
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        7 2024-05-26 21:54:54.000000 ragoon-0.0.1/src/ragoon.egg-info/top_level.txt
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 22:04:05.419349 ragoon-0.0.2/
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)    11357 2024-05-19 18:03:38.000000 ragoon-0.0.2/LICENSE
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     4754 2024-05-26 22:04:05.418508 ragoon-0.0.2/PKG-INFO
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     3920 2024-05-26 21:52:13.000000 ragoon-0.0.2/README.md
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     1798 2024-05-26 22:03:49.000000 ragoon-0.0.2/pyproject.toml
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)       38 2024-05-26 22:04:05.419521 ragoon-0.0.2/setup.cfg
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 22:04:05.404228 ragoon-0.0.2/src/
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 22:04:05.413901 ragoon-0.0.2/src/ragoon/
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      208 2024-05-26 21:31:34.000000 ragoon-0.0.2/src/ragoon/__init__.py
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     8080 2024-05-19 17:54:54.000000 ragoon-0.0.2/src/ragoon/_retrieval.py
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     3990 2024-04-19 22:51:33.000000 ragoon-0.0.2/src/ragoon/_scrape.py
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     2386 2024-04-20 12:11:41.000000 ragoon-0.0.2/src/ragoon/_search.py
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     4848 2024-05-26 22:03:32.000000 ragoon-0.0.2/src/ragoon/ragoon.py
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 22:04:05.417504 ragoon-0.0.2/src/ragoon.egg-info/
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     4754 2024-05-26 22:04:05.000000 ragoon-0.0.2/src/ragoon.egg-info/PKG-INFO
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      281 2024-05-26 22:04:05.000000 ragoon-0.0.2/src/ragoon.egg-info/SOURCES.txt
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        1 2024-05-26 22:04:05.000000 ragoon-0.0.2/src/ragoon.egg-info/dependency_links.txt
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        7 2024-05-26 22:04:05.000000 ragoon-0.0.2/src/ragoon.egg-info/top_level.txt
```

### Comparing `ragoon-0.0.1/LICENSE` & `ragoon-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragoon-0.0.1/PKG-INFO` & `ragoon-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragoon
-Version: 0.0.1
+Version: 0.0.2
 Summary: Improve large language models (LLM) retrieval using dynamic web-search based on blazingly fast query generation from Groq chips.
 Keywords: language-models,retrieval,web-scraping,few-shot-learning,nlp,machine-learning,retrieval-augmented-generation,RAG,groq,generative-ai,llama,Mistral
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `ragoon-0.0.1/README.md` & `ragoon-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ragoon-0.0.1/pyproject.toml` & `ragoon-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ragoon"
-version = "0.0.1"
+version = "0.0.2"
 description = "Improve large language models (LLM) retrieval using dynamic web-search based on blazingly fast query generation from Groq chips."
 readme = "README.md"
 keywords = ["language-models", "retrieval", "web-scraping", "few-shot-learning", "nlp", "machine-learning", "retrieval-augmented-generation", "RAG", "groq", "generative-ai", "llama", "Mistral"]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
@@ -29,15 +29,15 @@
     "beautifulsoup4",
     "httpx",
     "google-api-python-client"
 ]
 
 [metadata]
 name = "ragoon"
-version = "0.0.1"
+version = "0.0.2"
 license = "Apache License 2.0"
 author = "Louis Brulé Naudet"
 author_email = "louisbrulenaudet@icloud.com"
 description = "Improve large language models (LLM) retrieval using dynamic web-search based on blazingly fast query generation from Groq chips."
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 url = "https://github.com/louisbrulenaudet/ragoon"
```

### Comparing `ragoon-0.0.1/src/ragoon/_retrieval.py` & `ragoon-0.0.2/src/ragoon/_retrieval.py`

 * *Files identical despite different names*

### Comparing `ragoon-0.0.1/src/ragoon/_scrape.py` & `ragoon-0.0.2/src/ragoon/_scrape.py`

 * *Files identical despite different names*

### Comparing `ragoon-0.0.1/src/ragoon/_search.py` & `ragoon-0.0.2/src/ragoon/_search.py`

 * *Files identical despite different names*

### Comparing `ragoon-0.0.1/src/ragoon/ragoon.py` & `ragoon-0.0.2/src/ragoon/ragoon.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from dotenv import load_dotenv
 
 from groq import Groq
 from openai import OpenAI
 
 from _retrieval import Retriever
 from _scrape import WebScraper
 from _search import GoogleSearch
 
 
-# Load environment variables from .env file
-load_dotenv()
-
 class RAGoon:
     def __init__(
         self,
         google_api_key:str,
         google_cx:str,
         completion_client,
         user_agent:str="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.102 Safari/537.36"
```

### Comparing `ragoon-0.0.1/src/ragoon.egg-info/PKG-INFO` & `ragoon-0.0.2/src/ragoon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragoon
-Version: 0.0.1
+Version: 0.0.2
 Summary: Improve large language models (LLM) retrieval using dynamic web-search based on blazingly fast query generation from Groq chips.
 Keywords: language-models,retrieval,web-scraping,few-shot-learning,nlp,machine-learning,retrieval-augmented-generation,RAG,groq,generative-ai,llama,Mistral
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

