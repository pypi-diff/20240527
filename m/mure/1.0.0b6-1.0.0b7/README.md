# Comparing `tmp/mure-1.0.0b6.tar.gz` & `tmp/mure-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mure-1.0.0b6.tar", max compression
+gzip compressed data, was "mure-1.0.0b7.tar", max compression
```

## Comparing `mure-1.0.0b6.tar` & `mure-1.0.0b7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11345 2024-05-17 15:13:48.358748 mure-1.0.0b6/LICENSE
--rw-r--r--   0        0        0     7467 2024-05-17 15:13:48.358748 mure-1.0.0b6/README.md
--rw-r--r--   0        0        0      212 2024-05-17 15:13:48.358748 mure-1.0.0b6/mure/__init__.py
--rw-r--r--   0        0        0     3106 2024-05-17 15:13:48.358748 mure-1.0.0b6/mure/cache.py
--rw-r--r--   0        0        0     4419 2024-05-17 15:13:48.358748 mure-1.0.0b6/mure/core.py
--rw-r--r--   0        0        0     8841 2024-05-17 15:13:48.358748 mure-1.0.0b6/mure/iterator.py
--rw-r--r--   0        0        0     4272 2024-05-17 15:13:48.358748 mure-1.0.0b6/mure/logging.py
--rw-r--r--   0        0        0     3511 2024-05-17 15:13:48.358748 mure-1.0.0b6/mure/models.py
--rw-r--r--   0        0        0     2756 2024-05-17 15:13:48.362748 mure-1.0.0b6/pyproject.toml
--rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 mure-1.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-27 13:15:06.620485 mure-1.0.0b7/LICENSE
+-rw-r--r--   0        0        0     7467 2024-05-27 13:15:06.624485 mure-1.0.0b7/README.md
+-rw-r--r--   0        0        0      212 2024-05-27 13:15:06.624485 mure-1.0.0b7/mure/__init__.py
+-rw-r--r--   0        0        0     3106 2024-05-27 13:15:06.624485 mure-1.0.0b7/mure/cache.py
+-rw-r--r--   0        0        0     4419 2024-05-27 13:15:06.624485 mure-1.0.0b7/mure/core.py
+-rw-r--r--   0        0        0     9087 2024-05-27 13:15:06.624485 mure-1.0.0b7/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2024-05-27 13:15:06.624485 mure-1.0.0b7/mure/logging.py
+-rw-r--r--   0        0        0     3511 2024-05-27 13:15:06.624485 mure-1.0.0b7/mure/models.py
+-rw-r--r--   0        0        0     2756 2024-05-27 13:15:06.624485 mure-1.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 mure-1.0.0b7/PKG-INFO
```

### Comparing `mure-1.0.0b6/LICENSE` & `mure-1.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b6/README.md` & `mure-1.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b6/mure/cache.py` & `mure-1.0.0b7/mure/cache.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b6/mure/core.py` & `mure-1.0.0b7/mure/core.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b6/mure/iterator.py` & `mure-1.0.0b7/mure/iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,21 @@
         self._events = [Event() for _ in requests]
         self._tasks: set[Task] = set()
         self._responses = self._fetch_responses()
         self._agenerator = None
 
     def __del__(self):
         """Close the event loop."""
-        if not self._loop.is_closed():
-            self._loop.close()
+        try:
+            for task in {task for task in self._tasks if not task.done() or task.cancelled()}:
+                # give canceled tasks the last chance to run
+                self._loop.run_until_complete(task)
+        finally:
+            if not self._loop.is_closed():
+                self._loop.close()
 
     def __repr__(self) -> str:
         """Response iterator representation.
 
         Returns
         -------
         str
```

### Comparing `mure-1.0.0b6/mure/logging.py` & `mure-1.0.0b7/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b6/mure/models.py` & `mure-1.0.0b7/mure/models.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b6/pyproject.toml` & `mure-1.0.0b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mure"
-version = "1.0.0b6"
+version = "1.0.0b7"
 description = "Perform multiple HTTP requests concurrently – without worrying about async/await."
 authors = ["Severin Simmler <s.simmler@snapaddy.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 chardet = "^5.2.0"
```

### Comparing `mure-1.0.0b6/PKG-INFO` & `mure-1.0.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mure
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: Perform multiple HTTP requests concurrently – without worrying about async/await.
 Author: Severin Simmler
 Author-email: s.simmler@snapaddy.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

