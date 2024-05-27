# Comparing `tmp/postfinancex-0.0.5.tar.gz` & `tmp/postfinancex-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfinancex-0.0.5.tar", max compression
+gzip compressed data, was "postfinancex-0.0.6.tar", max compression
```

## Comparing `postfinancex-0.0.5.tar` & `postfinancex-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.5/LICENSE
--rw-r--r--   0        0        0     1406 2024-05-27 00:32:46.191007 postfinancex-0.0.5/README.md
--rw-r--r--   0        0        0      144 2024-05-27 00:05:10.628112 postfinancex-0.0.5/postfinance/__init__.py
--rw-r--r--   0        0        0     2729 2024-05-27 00:11:45.515399 postfinancex-0.0.5/postfinance/agent.py
--rw-r--r--   0        0        0     3797 2024-05-27 00:48:22.035951 postfinancex-0.0.5/postfinance/settings.py
--rw-r--r--   0        0        0        0 2024-05-26 22:24:54.394886 postfinancex-0.0.5/postfinance/tools/__init__.py
--rw-r--r--   0        0        0     7272 2024-05-27 00:11:37.715437 postfinancex-0.0.5/postfinance/tools/graph_qa_tool.py
--rw-r--r--   0        0        0     2072 2024-05-27 00:49:47.089556 postfinancex-0.0.5/postfinance/tools/summarization_tool.py
--rw-r--r--   0        0        0     1633 2024-05-26 23:50:41.315057 postfinancex-0.0.5/postfinance/tools/translation_tool.py
--rw-r--r--   0        0        0     2039 2024-05-27 00:50:32.615892 postfinancex-0.0.5/postfinance/tools/vector_search_tool.py
--rw-r--r--   0        0        0      779 2024-05-27 00:41:12.031938 postfinancex-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 postfinancex-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1406 2024-05-27 00:32:46.191007 postfinancex-0.0.6/README.md
+-rw-r--r--   0        0        0      315 2024-05-27 02:03:46.094859 postfinancex-0.0.6/postfinance/__init__.py
+-rw-r--r--   0        0        0     2729 2024-05-27 00:11:45.515399 postfinancex-0.0.6/postfinance/agent.py
+-rw-r--r--   0        0        0    10494 2024-05-27 02:20:15.219075 postfinancex-0.0.6/postfinance/annotate.py
+-rw-r--r--   0        0        0     3797 2024-05-27 00:48:22.035951 postfinancex-0.0.6/postfinance/settings.py
+-rw-r--r--   0        0        0        0 2024-05-26 22:24:54.394886 postfinancex-0.0.6/postfinance/tools/__init__.py
+-rw-r--r--   0        0        0     7272 2024-05-27 00:11:37.715437 postfinancex-0.0.6/postfinance/tools/graph_qa_tool.py
+-rw-r--r--   0        0        0     2072 2024-05-27 00:49:47.089556 postfinancex-0.0.6/postfinance/tools/summarization_tool.py
+-rw-r--r--   0        0        0     1633 2024-05-26 23:50:41.315057 postfinancex-0.0.6/postfinance/tools/translation_tool.py
+-rw-r--r--   0        0        0     2039 2024-05-27 00:50:32.615892 postfinancex-0.0.6/postfinance/tools/vector_search_tool.py
+-rw-r--r--   0        0        0    11121 2024-05-27 02:08:04.198793 postfinancex-0.0.6/postfinance/translate.py
+-rw-r--r--   0        0        0      805 2024-05-27 02:27:15.646532 postfinancex-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 postfinancex-0.0.6/PKG-INFO
```

### Comparing `postfinancex-0.0.5/LICENSE` & `postfinancex-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/README.md` & `postfinancex-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/postfinance/agent.py` & `postfinancex-0.0.6/postfinance/agent.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/postfinance/settings.py` & `postfinancex-0.0.6/postfinance/settings.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/postfinance/tools/graph_qa_tool.py` & `postfinancex-0.0.6/postfinance/tools/graph_qa_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/postfinance/tools/summarization_tool.py` & `postfinancex-0.0.6/postfinance/tools/summarization_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/postfinance/tools/translation_tool.py` & `postfinancex-0.0.6/postfinance/tools/translation_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/postfinance/tools/vector_search_tool.py` & `postfinancex-0.0.6/postfinance/tools/vector_search_tool.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.5/PKG-INFO` & `postfinancex-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: postfinancex
-Version: 0.0.5
+Version: 0.0.6
 Summary: PostFinanceX Virtual Assistant powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai
 Home-page: https://pypi.org/project/postfinancex
 License: BSD-3-Clause
 Author: Yi ZHANG
 Author-email: yizhang.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dnspython (>=2.6.1,<3.0.0)
+Requires-Dist: ibm_watsonx_ai (>=1.0.4,<2.0.0)
 Requires-Dist: langchain (>=0.2.0,<0.3.0)
 Requires-Dist: langchain-community (>=0.2.1,<0.3.0)
 Requires-Dist: langchain-ibm (>=0.1.7,<0.2.0)
 Requires-Dist: llama-index (>=0.10.38,<0.11.0)
 Requires-Dist: llama-index-embeddings-jinaai (>=0.1.5,<0.2.0)
 Requires-Dist: llama-index-llms-watsonx (>=0.1.7,<0.2.0)
 Requires-Dist: neo4j (>=5.20.0,<6.0.0)
```

