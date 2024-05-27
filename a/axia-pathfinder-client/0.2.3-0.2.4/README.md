# Comparing `tmp/axia_pathfinder_client-0.2.3.tar.gz` & `tmp/axia_pathfinder_client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axia_pathfinder_client-0.2.3.tar", max compression
+gzip compressed data, was "axia_pathfinder_client-0.2.4.tar", max compression
```

## Comparing `axia_pathfinder_client-0.2.3.tar` & `axia_pathfinder_client-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34523 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/LICENSE
--rw-r--r--   0        0        0     1803 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/__init__.py
--rw-r--r--   0        0        0      333 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/base.py
--rw-r--r--   0        0        0      679 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/get.py
--rw-r--r--   0        0        0      683 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/gpo.py
--rw-r--r--   0        0        0      860 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/login.py
--rw-r--r--   0        0        0      388 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/sub.py
--rw-r--r--   0        0        0     1366 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/parser.py
--rw-r--r--   0        0        0     1178 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/telnet.py
--rw-r--r--   0        0        0     1075 2024-04-14 19:36:54.908888 axia_pathfinder_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 axia_pathfinder_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1803 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/operators/__init__.py
+-rw-r--r--   0        0        0      333 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/operators/base.py
+-rw-r--r--   0        0        0      679 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/operators/get.py
+-rw-r--r--   0        0        0      683 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/operators/gpo.py
+-rw-r--r--   0        0        0      860 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/operators/login.py
+-rw-r--r--   0        0        0      388 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/operators/sub.py
+-rw-r--r--   0        0        0     1366 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/parser.py
+-rw-r--r--   0        0        0     1178 2024-05-27 21:54:55.551409 axia_pathfinder_client-0.2.4/pathfinder/telnet.py
+-rw-r--r--   0        0        0     1075 2024-05-27 21:55:12.051680 axia_pathfinder_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 axia_pathfinder_client-0.2.4/PKG-INFO
```

### Comparing `axia_pathfinder_client-0.2.3/LICENSE` & `axia_pathfinder_client-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.3/README.md` & `axia_pathfinder_client-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.3/pathfinder/operators/get.py` & `axia_pathfinder_client-0.2.4/pathfinder/operators/get.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.3/pathfinder/operators/gpo.py` & `axia_pathfinder_client-0.2.4/pathfinder/operators/gpo.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.3/pathfinder/operators/login.py` & `axia_pathfinder_client-0.2.4/pathfinder/operators/login.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.3/pathfinder/parser.py` & `axia_pathfinder_client-0.2.4/pathfinder/parser.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.3/pathfinder/telnet.py` & `axia_pathfinder_client-0.2.4/pathfinder/telnet.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.3/pyproject.toml` & `axia_pathfinder_client-0.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "axia-pathfinder-client"
-version = "v0.2.3"
+version = "v0.2.4"
 description = "Proof of concept Axia Pathfinder API/SDK."
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{include = "pathfinder"}]
 
 [tool.poetry.dependencies]
@@ -13,23 +13,23 @@
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3,<25.0"
 pytest = ">=7.3.2,<9.0.0"
 pytest-cov = ">=4,<6"
 pytest-random-order = "^1.1.0"
 pytest-ruff = ">=0.1,<0.4"
-ruff = ">=0.0.272,<0.3.8"
+ruff = ">=0.0.272,<0.4.6"
 isort = "^5.12.0"
 pytest-isort = ">=3.1,<5.0"
 mkdocs = "^1.4.3"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-material = "^9.1.16"
-mkdocstrings = {extras = ["python"], version = ">=0.22,<0.25"}
+mkdocstrings = {extras = ["python"], version = ">=0.22,<0.26"}
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --random-order --cov=pathfinder --cov-fail-under=100 --ruff --isort --ignore=docs/"
```

### Comparing `axia_pathfinder_client-0.2.3/PKG-INFO` & `axia_pathfinder_client-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axia-pathfinder-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: Proof of concept Axia Pathfinder API/SDK.
 License: AGPLv3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

