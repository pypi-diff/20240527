# Comparing `tmp/redis_cached-0.4.1.tar.gz` & `tmp/redis_cached-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_cached-0.4.1.tar", max compression
+gzip compressed data, was "redis_cached-0.4.2.tar", max compression
```

## Comparing `redis_cached-0.4.1.tar` & `redis_cached-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-12-12 12:36:44.895347 redis_cached-0.4.1/LICENSE
--rw-r--r--   0        0        0     2185 2024-04-26 07:30:19.823667 redis_cached-0.4.1/README.md
--rw-r--r--   0        0        0      623 2024-05-13 05:29:42.499211 redis_cached-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-26 07:30:19.824920 redis_cached-0.4.1/redis_cached/__init__.py
--rw-r--r--   0        0        0     3824 2024-05-13 05:25:28.120681 redis_cached-0.4.1/redis_cached/core.py
--rw-r--r--   0        0        0      368 2024-05-13 05:14:17.333310 redis_cached-0.4.1/redis_cached/utils.py
--rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 redis_cached-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-12-12 12:36:44.895347 redis_cached-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2185 2024-04-26 07:30:19.823667 redis_cached-0.4.2/README.md
+-rw-r--r--   0        0        0      623 2024-05-27 07:54:09.206622 redis_cached-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-26 07:30:19.824920 redis_cached-0.4.2/redis_cached/__init__.py
+-rw-r--r--   0        0        0     3824 2024-05-13 05:25:28.120681 redis_cached-0.4.2/redis_cached/core.py
+-rw-r--r--   0        0        0      512 2024-05-27 07:47:26.452615 redis_cached-0.4.2/redis_cached/utils.py
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 redis_cached-0.4.2/PKG-INFO
```

### Comparing `redis_cached-0.4.1/LICENSE` & `redis_cached-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_cached-0.4.1/README.md` & `redis_cached-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `redis_cached-0.4.1/pyproject.toml` & `redis_cached-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-cached"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python cache decorator and other itils with support for Redis or KeyDB"
 authors = ["Dmitry Babanov <85852989+dmitrybabanovforreal@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/dmitrybabanovforreal/redis-cached"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `redis_cached-0.4.1/redis_cached/core.py` & `redis_cached-0.4.2/redis_cached/core.py`

 * *Files identical despite different names*

### Comparing `redis_cached-0.4.1/PKG-INFO` & `redis_cached-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-cached
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python cache decorator and other itils with support for Redis or KeyDB
 Home-page: https://github.com/dmitrybabanovforreal/redis-cached
 Author: Dmitry Babanov
 Author-email: 85852989+dmitrybabanovforreal@users.noreply.github.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

