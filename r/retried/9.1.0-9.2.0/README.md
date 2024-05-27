# Comparing `tmp/retried-9.1.0.tar.gz` & `tmp/retried-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retried-9.1.0.tar", last modified: Sun Apr 14 03:07:24 2024, max compression
+gzip compressed data, was "retried-9.2.0.tar", last modified: Mon May 27 09:37:33 2024, max compression
```

## Comparing `retried-9.1.0.tar` & `retried-9.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      102 2024-04-14 03:07:03.555552 retried-9.1.0/README.md
--rw-r--r--   0        0        0     1061 2024-04-14 03:07:24.367655 retried-9.1.0/pyproject.toml
--rw-r--r--   0        0        0      224 2024-04-14 03:07:03.555552 retried-9.1.0/src/retried/__init__.py
--rw-r--r--   0        0        0       18 2024-04-14 03:07:03.555552 retried-9.1.0/src/retried/__version__.py
--rw-r--r--   0        0        0     2290 2024-04-14 03:07:03.555552 retried-9.1.0/src/retried/aretry.py
--rw-r--r--   0        0        0     4124 2024-04-14 03:07:03.555552 retried-9.1.0/src/retried/retry.py
--rw-r--r--   0        0        0      528 2024-04-14 03:07:03.555552 retried-9.1.0/src/retried/utils.py
--rw-r--r--   0        0        0        0 2024-04-14 03:07:03.555552 retried-9.1.0/tests/__init__.py
--rw-r--r--   0        0        0      657 2024-04-14 03:07:03.555552 retried-9.1.0/tests/test_aretry.py
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-9.1.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2024-05-27 09:37:17.523094 retried-9.2.0/README.md
+-rw-r--r--   0        0        0     1061 2024-05-27 09:37:33.123223 retried-9.2.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2024-05-27 09:37:17.523094 retried-9.2.0/src/retried/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-27 09:37:17.523094 retried-9.2.0/src/retried/__version__.py
+-rw-r--r--   0        0        0     2290 2024-05-27 09:37:17.523094 retried-9.2.0/src/retried/aretry.py
+-rw-r--r--   0        0        0     4124 2024-05-27 09:37:17.523094 retried-9.2.0/src/retried/retry.py
+-rw-r--r--   0        0        0      528 2024-05-27 09:37:17.523094 retried-9.2.0/src/retried/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:37:17.523094 retried-9.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      657 2024-05-27 09:37:17.523094 retried-9.2.0/tests/test_aretry.py
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-9.2.0/PKG-INFO
```

### Comparing `retried-9.1.0/pyproject.toml` & `retried-9.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retried"
-version = "9.1.0"
+version = "9.2.0"
 requires-python = ">=3.9"
 description = "A simple and powerful retrying library for Python"
 readme = "README.md"
 dependencies = []
 
 [build-system]
 requires = [
```

### Comparing `retried-9.1.0/src/retried/aretry.py` & `retried-9.2.0/src/retried/aretry.py`

 * *Files identical despite different names*

### Comparing `retried-9.1.0/src/retried/retry.py` & `retried-9.2.0/src/retried/retry.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,20 +117,20 @@
                 wf = wrapper.__original_wrapped__
                 i = 0
                 callback(i, e, first_delay or next(delays_), retries, wf)
                 while True:
                     try:
                         result = function_retrying()
                     except exceptions as e:
+                        i += 1
+                        callback(i, e, next(delays_), retries, wf)
                         if i == retries:
                             if chain_exception:
                                 raise
                             raise e from None
-                        i += 1
-                        callback(i, e, next(delays_), retries, wf)
                     else:
                         return result
             else:
                 return result
 
         return wrapper
```

### Comparing `retried-9.1.0/src/retried/utils.py` & `retried-9.2.0/src/retried/utils.py`

 * *Files identical despite different names*

### Comparing `retried-9.1.0/tests/test_aretry.py` & `retried-9.2.0/tests/test_aretry.py`

 * *Files identical despite different names*

