# Comparing `tmp/puepy-0.1.1.tar.gz` & `tmp/puepy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puepy-0.1.1.tar", max compression
+gzip compressed data, was "puepy-0.1.2.tar", max compression
```

## Comparing `puepy-0.1.1.tar` & `puepy-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3040 2024-05-26 17:02:46.417236 puepy-0.1.1/README.md
--rw-r--r--   0        0        0       90 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/__init__.py
--rw-r--r--   0        0        0     2756 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/application.py
--rw-r--r--   0        0        0    21358 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/core.py
--rw-r--r--   0        0        0       84 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/errors.py
--rw-r--r--   0        0        0     2659 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/reactivity.py
--rw-r--r--   0        0        0     2893 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/router.py
--rw-r--r--   0        0        0     1390 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/runtime.py
--rw-r--r--   0        0        0     2211 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/storage.py
--rw-r--r--   0        0        0     4055 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/util.py
--rw-r--r--   0        0        0      466 2024-05-26 17:02:46.417236 puepy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 puepy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3040 2024-05-27 21:19:07.414163 puepy-0.1.2/README.md
+-rw-r--r--   0        0        0       90 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/__init__.py
+-rw-r--r--   0        0        0     2756 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/application.py
+-rw-r--r--   0        0        0    21358 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/core.py
+-rw-r--r--   0        0        0       84 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/errors.py
+-rw-r--r--   0        0        0     2659 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/reactivity.py
+-rw-r--r--   0        0        0     2893 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/router.py
+-rw-r--r--   0        0        0     1390 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/runtime.py
+-rw-r--r--   0        0        0     2211 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/storage.py
+-rw-r--r--   0        0        0     4055 2024-05-27 21:19:07.414163 puepy-0.1.2/puepy/util.py
+-rw-r--r--   0        0        0      466 2024-05-27 21:19:07.414163 puepy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 puepy-0.1.2/PKG-INFO
```

### Comparing `puepy-0.1.1/README.md` & `puepy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/puepy/application.py` & `puepy-0.1.2/puepy/application.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/puepy/core.py` & `puepy-0.1.2/puepy/core.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/puepy/reactivity.py` & `puepy-0.1.2/puepy/reactivity.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/puepy/router.py` & `puepy-0.1.2/puepy/router.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/puepy/runtime.py` & `puepy-0.1.2/puepy/runtime.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/puepy/storage.py` & `puepy-0.1.2/puepy/storage.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/puepy/util.py` & `puepy-0.1.2/puepy/util.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.1/PKG-INFO` & `puepy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Frontend Framework for PyScript
 Author: Ken Kinder
 Author-email: ken+github@kkinder.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

