# Comparing `tmp/lckytools-0.0.0a3.tar.gz` & `tmp/lckytools-0.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0a3.tar", max compression
+gzip compressed data, was "lckytools-0.0.0a4.tar", max compression
```

## Comparing `lckytools-0.0.0a3.tar` & `lckytools-0.0.0a4.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      294 2024-05-27 02:47:29.152194 lckytools-0.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a3/README.md
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a3/src/lckytools/__init__.py
--rw-r--r--   0        0        0       40 2024-05-27 02:47:26.695814 lckytools-0.0.0a3/src/lckytools/ai/__init__.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 lckytools-0.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0      294 2024-05-27 02:49:07.194502 lckytools-0.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a4/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a4/src/lckytools/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-27 02:47:26.695814 lckytools-0.0.0a4/src/lckytools/ai/__init__.py
+-rw-r--r--   0        0        0      144 2024-05-27 02:10:58.751794 lckytools-0.0.0a4/src/lckytools/ai/metrics/__init__.py
+-rw-r--r--   0        0        0      829 2024-05-27 02:10:59.000094 lckytools-0.0.0a4/src/lckytools/ai/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 lckytools-0.0.0a4/PKG-INFO
```

### Comparing `lckytools-0.0.0a3/README.md` & `lckytools-0.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a3/PKG-INFO` & `lckytools-0.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: 
 License: MIT
 Author: LCKYN
 Author-email: T.Pawarit@lckyn.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

