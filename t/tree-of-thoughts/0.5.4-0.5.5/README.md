# Comparing `tmp/tree_of_thoughts-0.5.4.tar.gz` & `tmp/tree_of_thoughts-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_of_thoughts-0.5.4.tar", max compression
+gzip compressed data, was "tree_of_thoughts-0.5.5.tar", max compression
```

## Comparing `tree_of_thoughts-0.5.4.tar` & `tree_of_thoughts-0.5.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11343 2024-05-22 22:37:06.476760 tree_of_thoughts-0.5.4/LICENSE
--rw-r--r--   0        0        0     9301 2024-05-23 01:01:21.809204 tree_of_thoughts-0.5.4/README.md
--rw-r--r--   0        0        0     1262 2024-05-23 01:13:47.293174 tree_of_thoughts-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      356 2024-05-23 00:55:53.906281 tree_of_thoughts-0.5.4/tree_of_thoughts/__init__.py
--rw-r--r--   0        0        0     8515 2024-05-23 01:10:34.476378 tree_of_thoughts-0.5.4/tree_of_thoughts/tot_agent.py
--rw-r--r--   0        0        0    23710 2024-05-22 22:37:06.483623 tree_of_thoughts-0.5.4/tree_of_thoughts/tree_of_thoughts.py
--rw-r--r--   0        0        0    10235 1970-01-01 00:00:00.000000 tree_of_thoughts-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-05-22 22:37:06.476760 tree_of_thoughts-0.5.5/LICENSE
+-rw-r--r--   0        0        0     9301 2024-05-23 01:01:21.809204 tree_of_thoughts-0.5.5/README.md
+-rw-r--r--   0        0        0     1262 2024-05-27 04:15:14.314267 tree_of_thoughts-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      356 2024-05-23 00:55:53.906281 tree_of_thoughts-0.5.5/tree_of_thoughts/__init__.py
+-rw-r--r--   0        0        0     8515 2024-05-23 01:10:34.476378 tree_of_thoughts-0.5.5/tree_of_thoughts/tot_agent.py
+-rw-r--r--   0        0        0    23710 2024-05-22 22:37:06.483623 tree_of_thoughts-0.5.5/tree_of_thoughts/tree_of_thoughts.py
+-rw-r--r--   0        0        0    10235 1970-01-01 00:00:00.000000 tree_of_thoughts-0.5.5/PKG-INFO
```

### Comparing `tree_of_thoughts-0.5.4/LICENSE` & `tree_of_thoughts-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.4/README.md` & `tree_of_thoughts-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.4/pyproject.toml` & `tree_of_thoughts-0.5.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tree-of-thoughts"
-version = "0.5.4"
+version = "0.5.5"
 description = "Tree of Thoughts - Pytorch"
 authors = ["Kye Gomez <kye@apac.ai>"]
 license = "MIT"
 readme = "README.md"  # Assuming you have a README.md file
 homepage = "https://github.com/kyegomez/tree-of-thoughts"
 keywords = ["artificial intelligence", "deep learning", "optimizers", "Prompt Engineering"]
 classifiers = [
```

### Comparing `tree_of_thoughts-0.5.4/tree_of_thoughts/tot_agent.py` & `tree_of_thoughts-0.5.5/tree_of_thoughts/tot_agent.py`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.4/tree_of_thoughts/tree_of_thoughts.py` & `tree_of_thoughts-0.5.5/tree_of_thoughts/tree_of_thoughts.py`

 * *Files identical despite different names*

### Comparing `tree_of_thoughts-0.5.4/PKG-INFO` & `tree_of_thoughts-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.5.4
+Version: 0.5.5
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.10,<4.0
```

