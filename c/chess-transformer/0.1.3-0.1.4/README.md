# Comparing `tmp/chess_transformer-0.1.3.tar.gz` & `tmp/chess_transformer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_transformer-0.1.3.tar", last modified: Mon May 27 06:59:02 2024, max compression
+gzip compressed data, was "chess_transformer-0.1.4.tar", last modified: Mon May 27 07:04:23 2024, max compression
```

## Comparing `chess_transformer-0.1.3.tar` & `chess_transformer-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-27 06:58:58.000000 chess_transformer-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.083722 chess_transformer-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-27 06:51:02.000000 chess_transformer-0.1.3/src/chess_transformer/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/data/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      269 2024-05-27 06:04:33.000000 chess_transformer-0.1.3/src/chess_transformer/data/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      978 2024-05-27 05:20:29.000000 chess_transformer-0.1.3/src/chess_transformer/data/collate.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      903 2024-05-27 05:21:48.000000 chess_transformer-0.1.3/src/chess_transformer/data/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1146 2024-05-27 06:44:29.000000 chess_transformer-0.1.3/src/chess_transformer/data/labs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      109 2024-05-27 05:46:01.000000 chess_transformer-0.1.3/src/chess_transformer/data/parse.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1198 2024-05-27 06:29:32.000000 chess_transformer-0.1.3/src/chess_transformer/data/pytorch.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/data/random.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/model/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-27 06:50:49.000000 chess_transformer-0.1.3/src/chess_transformer/model/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      815 2024-05-27 06:47:54.000000 chess_transformer-0.1.3/src/chess_transformer/model/bert.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-05-27 06:51:03.000000 chess_transformer-0.1.3/src/chess_transformer/model/loss.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/vocab/sans.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 07:04:23.333711 chess_transformer-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-05-27 07:04:23.333711 chess_transformer-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-27 04:49:42.000000 chess_transformer-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      566 2024-05-27 07:04:20.000000 chess_transformer-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-27 07:04:23.333711 chess_transformer-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 07:04:23.323711 chess_transformer-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 07:04:23.323711 chess_transformer-0.1.4/src/chess_transformer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-27 06:51:02.000000 chess_transformer-0.1.4/src/chess_transformer/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 07:04:23.333711 chess_transformer-0.1.4/src/chess_transformer/data/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      269 2024-05-27 06:04:33.000000 chess_transformer-0.1.4/src/chess_transformer/data/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      978 2024-05-27 05:20:29.000000 chess_transformer-0.1.4/src/chess_transformer/data/collate.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      903 2024-05-27 05:21:48.000000 chess_transformer-0.1.4/src/chess_transformer/data/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1146 2024-05-27 06:44:29.000000 chess_transformer-0.1.4/src/chess_transformer/data/labs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      109 2024-05-27 05:46:01.000000 chess_transformer-0.1.4/src/chess_transformer/data/parse.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1198 2024-05-27 06:29:32.000000 chess_transformer-0.1.4/src/chess_transformer/data/pytorch.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-27 04:49:42.000000 chess_transformer-0.1.4/src/chess_transformer/data/random.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 07:04:23.333711 chess_transformer-0.1.4/src/chess_transformer/model/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-27 06:50:49.000000 chess_transformer-0.1.4/src/chess_transformer/model/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      815 2024-05-27 06:47:54.000000 chess_transformer-0.1.4/src/chess_transformer/model/bert.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-05-27 06:51:03.000000 chess_transformer-0.1.4/src/chess_transformer/model/loss.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 07:04:23.333711 chess_transformer-0.1.4/src/chess_transformer/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-05-27 04:49:42.000000 chess_transformer-0.1.4/src/chess_transformer/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-27 04:49:42.000000 chess_transformer-0.1.4/src/chess_transformer/vocab/sans.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-27 04:49:42.000000 chess_transformer-0.1.4/src/chess_transformer/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 07:04:23.333711 chess_transformer-0.1.4/src/chess_transformer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-05-27 07:04:23.000000 chess_transformer-0.1.4/src/chess_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-27 07:04:23.000000 chess_transformer-0.1.4/src/chess_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-27 07:04:23.000000 chess_transformer-0.1.4/src/chess_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-27 07:04:23.000000 chess_transformer-0.1.4/src/chess_transformer.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-27 07:04:23.000000 chess_transformer-0.1.4/src/chess_transformer.egg-info/top_level.txt
```

### Comparing `chess_transformer-0.1.3/pyproject.toml` & `chess_transformer-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-transformer"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread goes smarter, baby"
 dependencies = [
-  "torch", "chess"
+  "torch", "chess", "jaxtyping", "haskellian"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/REPO.git"
```

### Comparing `chess_transformer-0.1.3/src/chess_transformer/data/collate.py` & `chess_transformer-0.1.4/src/chess_transformer/data/collate.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/data/dataset.py` & `chess_transformer-0.1.4/src/chess_transformer/data/dataset.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/data/labs.py` & `chess_transformer-0.1.4/src/chess_transformer/data/labs.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/data/pytorch.py` & `chess_transformer-0.1.4/src/chess_transformer/data/pytorch.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/data/random.py` & `chess_transformer-0.1.4/src/chess_transformer/data/random.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/model/bert.py` & `chess_transformer-0.1.4/src/chess_transformer/model/bert.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/model/loss.py` & `chess_transformer-0.1.4/src/chess_transformer/model/loss.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/vocab/sans.py` & `chess_transformer-0.1.4/src/chess_transformer/vocab/sans.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer/vocab/vocab.py` & `chess_transformer-0.1.4/src/chess_transformer/vocab/vocab.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.3/src/chess_transformer.egg-info/SOURCES.txt` & `chess_transformer-0.1.4/src/chess_transformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

