# Comparing `tmp/proof_of_train-0.1.0.tar.gz` & `tmp/proof_of_train-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proof_of_train-0.1.0.tar", max compression
+gzip compressed data, was "proof_of_train-0.2.0.tar", max compression
```

## Comparing `proof_of_train-0.1.0.tar` & `proof_of_train-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3621 2024-05-23 09:19:26.093380 proof_of_train-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-20 03:16:12.219328 proof_of_train-0.1.0/proof_of_train/__init__.py
--rw-r--r--   0        0        0     1460 2024-05-22 11:02:00.944128 proof_of_train-0.1.0/proof_of_train/abi.json
--rw-r--r--   0        0        0     2649 2024-05-22 11:02:17.998383 proof_of_train-0.1.0/proof_of_train/model_metadata.py
--rw-r--r--   0        0        0     4418 2024-05-23 09:19:26.090913 proof_of_train-0.1.0/proof_of_train/proof_of_train.py
--rw-r--r--   0        0        0     1724 2024-05-23 09:17:38.791252 proof_of_train-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 proof_of_train-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3621 2024-05-23 09:19:26.093380 proof_of_train-0.2.0/README.md
+-rw-r--r--   0        0        0      127 2024-05-27 02:01:43.425888 proof_of_train-0.2.0/proof_of_train/__init__.py
+-rw-r--r--   0        0        0     1460 2024-05-22 11:02:00.944128 proof_of_train-0.2.0/proof_of_train/abi.json
+-rw-r--r--   0        0        0     2649 2024-05-22 11:02:17.998383 proof_of_train-0.2.0/proof_of_train/model_metadata.py
+-rw-r--r--   0        0        0     4418 2024-05-23 09:19:26.090913 proof_of_train-0.2.0/proof_of_train/proof_of_train.py
+-rw-r--r--   0        0        0     1724 2024-05-27 02:01:43.422373 proof_of_train-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 proof_of_train-0.2.0/PKG-INFO
```

### Comparing `proof_of_train-0.1.0/README.md` & `proof_of_train-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `proof_of_train-0.1.0/proof_of_train/abi.json` & `proof_of_train-0.2.0/proof_of_train/abi.json`

 * *Files identical despite different names*

### Comparing `proof_of_train-0.1.0/proof_of_train/model_metadata.py` & `proof_of_train-0.2.0/proof_of_train/model_metadata.py`

 * *Files identical despite different names*

### Comparing `proof_of_train-0.1.0/proof_of_train/proof_of_train.py` & `proof_of_train-0.2.0/proof_of_train/proof_of_train.py`

 * *Files identical despite different names*

### Comparing `proof_of_train-0.1.0/pyproject.toml` & `proof_of_train-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proof-of-train"
-version = "0.1.0"
+version = "0.2.0"
 description = "Proof of Train SDK for submitting and verifying model training metadata on blockchain."
 authors = ["Thomas <wxy_000000@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 web3 = "^6.19.0"
```

### Comparing `proof_of_train-0.1.0/PKG-INFO` & `proof_of_train-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proof-of-train
-Version: 0.1.0
+Version: 0.2.0
 Summary: Proof of Train SDK for submitting and verifying model training metadata on blockchain.
 Author: Thomas
 Author-email: wxy_000000@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=8.2.1,<9.0.0)
```

