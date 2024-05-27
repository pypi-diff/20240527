# Comparing `tmp/lckytools-0.0.0a1.tar.gz` & `tmp/lckytools-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0a1.tar", max compression
+gzip compressed data, was "lckytools-0.0.0a2.tar", max compression
```

## Comparing `lckytools-0.0.0a1.tar` & `lckytools-0.0.0a2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      294 2024-05-27 02:40:37.378404 lckytools-0.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a1/README.md
--rw-r--r--   0        0        0       49 2024-05-27 02:40:26.047315 lckytools-0.0.0a1/src/lckytools/__init__.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 lckytools-0.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      294 2024-05-27 02:43:29.672870 lckytools-0.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a2/README.md
+-rw-r--r--   0        0        0       49 2024-05-27 02:43:19.334223 lckytools-0.0.0a2/src/lckytools/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-27 02:43:18.742205 lckytools-0.0.0a2/src/lckytools/hello.py
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 lckytools-0.0.0a2/PKG-INFO
```

### Comparing `lckytools-0.0.0a1/README.md` & `lckytools-0.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a1/PKG-INFO` & `lckytools-0.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: 
 License: MIT
 Author: LCKYN
 Author-email: T.Pawarit@lckyn.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

