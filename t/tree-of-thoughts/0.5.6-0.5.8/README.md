# Comparing `tmp/tree_of_thoughts-0.5.6.tar.gz` & `tmp/tree_of_thoughts-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_of_thoughts-0.5.6.tar", max compression
+gzip compressed data, was "tree_of_thoughts-0.5.8.tar", max compression
```

## Comparing `tree_of_thoughts-0.5.6.tar` & `tree_of_thoughts-0.5.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11343 2024-05-22 22:37:06.476760 tree_of_thoughts-0.5.6/LICENSE
--rw-r--r--   0        0        0     9301 2024-05-23 01:01:21.809204 tree_of_thoughts-0.5.6/README.md
--rw-r--r--   0        0        0     1262 2024-05-27 04:20:07.064838 tree_of_thoughts-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      357 2024-05-27 04:20:02.856585 tree_of_thoughts-0.5.6/tree_of_thoughts/__init__.py
--rw-r--r--   0        0        0    23710 2024-05-22 22:37:06.483623 tree_of_thoughts-0.5.6/tree_of_thoughts/search_algorithms.py
--rw-r--r--   0        0        0     8515 2024-05-23 01:10:34.476378 tree_of_thoughts-0.5.6/tree_of_thoughts/tot_agent.py
--rw-r--r--   0        0        0    10235 1970-01-01 00:00:00.000000 tree_of_thoughts-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-05-22 22:37:06.476760 tree_of_thoughts-0.5.8/LICENSE
+-rw-r--r--   0        0        0     9301 2024-05-23 01:01:21.809204 tree_of_thoughts-0.5.8/README.md
+-rw-r--r--   0        0        0     1262 2024-05-27 04:25:48.653707 tree_of_thoughts-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      329 2024-05-27 04:25:44.360559 tree_of_thoughts-0.5.8/tree_of_thoughts/__init__.py
+-rw-r--r--   0        0        0    23710 2024-05-22 22:37:06.483623 tree_of_thoughts-0.5.8/tree_of_thoughts/search_algorithms.py
+-rw-r--r--   0        0        0     8515 2024-05-23 01:10:34.476378 tree_of_thoughts-0.5.8/tree_of_thoughts/tot_agent.py
+-rw-r--r--   0        0        0    10235 1970-01-01 00:00:00.000000 tree_of_thoughts-0.5.8/PKG-INFO
```

### Comparing `tree_of_thoughts-0.5.6/LICENSE` & `tree_of_thoughts-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.6/README.md` & `tree_of_thoughts-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.6/pyproject.toml` & `tree_of_thoughts-0.5.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tree-of-thoughts"
-version = "0.5.6"
+version = "0.5.8"
 description = "Tree of Thoughts - Pytorch"
 authors = ["Kye Gomez <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"  # Assuming you have a README.md file
 homepage = "https://github.com/kyegomez/tree-of-thoughts"
 keywords = ["artificial intelligence", "deep learning", "optimizers", "Prompt Engineering"]
 classifiers = [
```

### Comparing `tree_of_thoughts-0.5.6/tree_of_thoughts/search_algorithms.py` & `tree_of_thoughts-0.5.8/tree_of_thoughts/search_algorithms.py`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.6/tree_of_thoughts/tot_agent.py` & `tree_of_thoughts-0.5.8/tree_of_thoughts/tot_agent.py`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.6/PKG-INFO` & `tree_of_thoughts-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.5.6
+Version: 0.5.8
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
```

