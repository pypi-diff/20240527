# Comparing `tmp/postfinancex-0.0.4.tar.gz` & `tmp/postfinancex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfinancex-0.0.4.tar", max compression
+gzip compressed data, was "postfinancex-0.0.5.tar", max compression
```

## Comparing `postfinancex-0.0.4.tar` & `postfinancex-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,12 @@
--rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.4/LICENSE
--rw-r--r--   0        0        0      923 2024-04-16 17:38:59.033315 postfinancex-0.0.4/README.md
--rw-r--r--   0        0        0      222 2024-04-16 00:54:00.166029 postfinancex-0.0.4/postfinance/__init__.py
--rw-r--r--   0        0        0     5363 2024-04-16 18:06:26.419453 postfinancex-0.0.4/postfinance/agents.py
--rw-r--r--   0        0        0     2094 2024-04-16 16:27:34.174963 postfinancex-0.0.4/postfinance/input_parsers.py
--rw-r--r--   0        0        0        0 2024-04-15 09:30:16.578796 postfinancex-0.0.4/postfinance/langchain/__init__.py
--rw-r--r--   0        0        0     2599 2024-04-15 00:18:14.909252 postfinancex-0.0.4/postfinance/langchain/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-16 01:02:12.975627 postfinancex-0.0.4/postfinance/langchain/llms.py
--rw-r--r--   0        0        0     4731 2024-04-16 18:04:34.902752 postfinancex-0.0.4/postfinance/langchain/storage.py
--rw-r--r--   0        0        0       59 2024-04-14 14:24:09.328883 postfinancex-0.0.4/postfinance/langchain/vectorstores.py
--rw-r--r--   0        0        0     3716 2024-04-16 17:16:08.729777 postfinancex-0.0.4/postfinance/models.py
--rw-r--r--   0        0        0     6790 2024-04-16 15:55:57.740472 postfinancex-0.0.4/postfinance/output_parsers.py
--rw-r--r--   0        0        0    14430 2024-04-16 17:15:12.175360 postfinancex-0.0.4/postfinance/prompts.py
--rw-r--r--   0        0        0      667 2024-04-16 18:05:30.405907 postfinancex-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 postfinancex-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1406 2024-05-27 00:32:46.191007 postfinancex-0.0.5/README.md
+-rw-r--r--   0        0        0      144 2024-05-27 00:05:10.628112 postfinancex-0.0.5/postfinance/__init__.py
+-rw-r--r--   0        0        0     2729 2024-05-27 00:11:45.515399 postfinancex-0.0.5/postfinance/agent.py
+-rw-r--r--   0        0        0     3797 2024-05-27 00:48:22.035951 postfinancex-0.0.5/postfinance/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 22:24:54.394886 postfinancex-0.0.5/postfinance/tools/__init__.py
+-rw-r--r--   0        0        0     7272 2024-05-27 00:11:37.715437 postfinancex-0.0.5/postfinance/tools/graph_qa_tool.py
+-rw-r--r--   0        0        0     2072 2024-05-27 00:49:47.089556 postfinancex-0.0.5/postfinance/tools/summarization_tool.py
+-rw-r--r--   0        0        0     1633 2024-05-26 23:50:41.315057 postfinancex-0.0.5/postfinance/tools/translation_tool.py
+-rw-r--r--   0        0        0     2039 2024-05-27 00:50:32.615892 postfinancex-0.0.5/postfinance/tools/vector_search_tool.py
+-rw-r--r--   0        0        0      779 2024-05-27 00:41:12.031938 postfinancex-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 postfinancex-0.0.5/PKG-INFO
```

### Comparing `postfinancex-0.0.4/LICENSE` & `postfinancex-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.4/README.md` & `postfinancex-0.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 # PostFinanceX
 
 [![GitHub][github_badge]][github_link] [![PyPI][pypi_badge]][pypi_link]
 
-**PostFinanceX** is a Python library allows you to call PostFinance LLM agent powered by IBM watsonx.ai
+**PostFinanceX** is a Python library allows you to chat with PostFinance LLM agent powered by IBM watsonx.ai
 
 
 
 ## Installation
 
 ```bash
 pip install postfinancex
 ```
 
 
 
 ## Quickstart
 
 ```python
-from postfinance import Agent
+from postfinance import Settings, get_agent_executor, chat
 
-agent = Agent("your_api_key_here")
+Settings.watsonx_api_key = "watsonx_api_key"
+Settings.watsonx_url = "watsonx_url"
+Settings.watsonx_project_id = "watsonx_project_id"
+Settings.jina_api_key = "jina_api_key"
+Settings.neo4j_url = "neo4j_url"
+Settings.neo4j_username = "neo4j_username"
+Settings.neo4j_password = "neo4j_password"
+Settings.mongo_uri = "mongo_uri"
+Settings.verbose = True
+
+agent_executor = get_agent_executor()
+
+chat(agent_executor, "What is the most commonly used language in the recorded customer calls?")
 ```
 
 
 
 ## License
 
 **PostFinanceX** has a BSD-3-Clause license, as found in the [LICENSE](https://github.com/imyizhang/postfinancex/blob/main/LICENSE) file.
```

### Comparing `postfinancex-0.0.4/pyproject.toml` & `postfinancex-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [tool.poetry]
 name = "postfinancex"
-version = "0.0.4"
+version = "0.0.5"
 description = "PostFinanceX Virtual Assistant powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai"
 packages = [
     {include = "postfinance"}
 ]
 authors = ["Yi ZHANG <yizhang.dev@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://pypi.org/project/postfinancex"
 repository = "https://github.com/imyizhang/postfinancex"
 
 [tool.poetry.dependencies]
-python = "^3.12"
-ibm-watsonx-ai = "^0.2.4"
-pymongo = "^4.6.3"
+python = "^3.10"
+pymongo = "^4.7.2"
 dnspython = "^2.6.1"
-langchain-community = "^0.0.33"
-langchain-core = "^0.1.43"
+neo4j = "^5.20.0"
+llama-index = "^0.10.38"
+llama-index-embeddings-jinaai = "^0.1.5"
+llama-index-llms-watsonx = "^0.1.7"
+langchain = "^0.2.0"
+langchain-community = "^0.2.1"
+langchain-ibm = "^0.1.7"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

