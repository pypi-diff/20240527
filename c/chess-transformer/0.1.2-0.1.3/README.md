# Comparing `tmp/chess_transformer-0.1.2.tar.gz` & `tmp/chess_transformer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_transformer-0.1.2.tar", last modified: Sun May 26 18:34:54 2024, max compression
+gzip compressed data, was "chess_transformer-0.1.3.tar", last modified: Mon May 27 06:59:02 2024, max compression
```

## Comparing `chess_transformer-0.1.2.tar` & `chess_transformer-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:34:54.276925 chess_transformer-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-05-26 18:34:54.276925 chess_transformer-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-26 16:42:39.000000 chess_transformer-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-26 18:34:52.000000 chess_transformer-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-26 18:34:54.276925 chess_transformer-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:34:54.266925 chess_transformer-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:34:54.266925 chess_transformer-0.1.2/src/chess_transformer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-26 17:06:39.000000 chess_transformer-0.1.2/src/chess_transformer/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:34:54.266925 chess_transformer-0.1.2/src/chess_transformer/data/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      173 2024-05-26 18:29:19.000000 chess_transformer-0.1.2/src/chess_transformer/data/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      787 2024-05-26 18:16:42.000000 chess_transformer-0.1.2/src/chess_transformer/data/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2559 2024-05-26 18:29:11.000000 chess_transformer-0.1.2/src/chess_transformer/data/mask.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-26 18:34:48.000000 chess_transformer-0.1.2/src/chess_transformer/data/random.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:34:54.276925 chess_transformer-0.1.2/src/chess_transformer/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-05-26 18:05:22.000000 chess_transformer-0.1.2/src/chess_transformer/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-26 16:57:10.000000 chess_transformer-0.1.2/src/chess_transformer/vocab/sans.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-26 18:06:59.000000 chess_transformer-0.1.2/src/chess_transformer/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:34:54.276925 chess_transformer-0.1.2/src/chess_transformer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-05-26 18:34:54.000000 chess_transformer-0.1.2/src/chess_transformer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      544 2024-05-26 18:34:54.000000 chess_transformer-0.1.2/src/chess_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-26 18:34:54.000000 chess_transformer-0.1.2/src/chess_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-26 18:34:54.000000 chess_transformer-0.1.2/src/chess_transformer.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-26 18:34:54.000000 chess_transformer-0.1.2/src/chess_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      539 2024-05-27 06:58:58.000000 chess_transformer-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.083722 chess_transformer-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      123 2024-05-27 06:51:02.000000 chess_transformer-0.1.3/src/chess_transformer/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/data/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      269 2024-05-27 06:04:33.000000 chess_transformer-0.1.3/src/chess_transformer/data/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      978 2024-05-27 05:20:29.000000 chess_transformer-0.1.3/src/chess_transformer/data/collate.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      903 2024-05-27 05:21:48.000000 chess_transformer-0.1.3/src/chess_transformer/data/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1146 2024-05-27 06:44:29.000000 chess_transformer-0.1.3/src/chess_transformer/data/labs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      109 2024-05-27 05:46:01.000000 chess_transformer-0.1.3/src/chess_transformer/data/parse.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1198 2024-05-27 06:29:32.000000 chess_transformer-0.1.3/src/chess_transformer/data/pytorch.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      696 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/data/random.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/model/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-27 06:50:49.000000 chess_transformer-0.1.3/src/chess_transformer/model/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      815 2024-05-27 06:47:54.000000 chess_transformer-0.1.3/src/chess_transformer/model/bert.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-05-27 06:51:03.000000 chess_transformer-0.1.3/src/chess_transformer/model/loss.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/vocab/sans.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-27 04:49:42.000000 chess_transformer-0.1.3/src/chess_transformer/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-27 06:59:02.093722 chess_transformer-0.1.3/src/chess_transformer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      365 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-27 06:59:02.000000 chess_transformer-0.1.3/src/chess_transformer.egg-info/top_level.txt
```

### Comparing `chess_transformer-0.1.2/pyproject.toml` & `chess_transformer-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-transformer"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread goes smarter, baby"
 dependencies = [
   "torch", "chess"
 ]
```

### Comparing `chess_transformer-0.1.2/src/chess_transformer/data/dataset.py` & `chess_transformer-0.1.3/src/chess_transformer/data/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,23 @@
 
   def __getitem__(self, idx: int) -> T:
     game = self.games[idx]
     return self.sample(game)
 
 class LazyDataset(Dataset, Generic[T]):
   def __init__(
-    self, sample: Callable[[int], T], num_games: int
+    self, sample: Callable[[int], T], num_samples: int
   ):
-    from functools import cache
-    self.sample = cache(sample)
-    self.num_games = num_games
+    self.samples: dict[int, T] = {}
+    self.sample = sample
+    self.num_samples = num_samples
 
   def __len__(self) -> int:
-    return self.num_games
+    return self.num_samples
 
   def __getitem__(self, idx: int) -> T:
-    return self.sample(idx)
+    if idx in self.samples:
+      return self.samples[idx]
+    else:
+      x = self.sample(idx)
+      self.samples[idx] = x
+      return x
```

### Comparing `chess_transformer-0.1.2/src/chess_transformer/data/random.py` & `chess_transformer-0.1.3/src/chess_transformer/data/random.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.2/src/chess_transformer/vocab/sans.py` & `chess_transformer-0.1.3/src/chess_transformer/vocab/sans.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.2/src/chess_transformer/vocab/vocab.py` & `chess_transformer-0.1.3/src/chess_transformer/vocab/vocab.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.2/src/chess_transformer.egg-info/SOURCES.txt` & `chess_transformer-0.1.3/src/chess_transformer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,13 +3,19 @@
 src/chess_transformer/__init__.py
 src/chess_transformer.egg-info/PKG-INFO
 src/chess_transformer.egg-info/SOURCES.txt
 src/chess_transformer.egg-info/dependency_links.txt
 src/chess_transformer.egg-info/requires.txt
 src/chess_transformer.egg-info/top_level.txt
 src/chess_transformer/data/__init__.py
+src/chess_transformer/data/collate.py
 src/chess_transformer/data/dataset.py
-src/chess_transformer/data/mask.py
+src/chess_transformer/data/labs.py
+src/chess_transformer/data/parse.py
+src/chess_transformer/data/pytorch.py
 src/chess_transformer/data/random.py
+src/chess_transformer/model/__init__.py
+src/chess_transformer/model/bert.py
+src/chess_transformer/model/loss.py
 src/chess_transformer/vocab/__init__.py
 src/chess_transformer/vocab/sans.py
 src/chess_transformer/vocab/vocab.py
```

