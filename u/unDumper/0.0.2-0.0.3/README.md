# Comparing `tmp/undumper-0.0.2.tar.gz` & `tmp/undumper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undumper-0.0.2.tar", max compression
+gzip compressed data, was "undumper-0.0.3.tar", max compression
```

## Comparing `undumper-0.0.2.tar` & `undumper-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1076 2024-05-22 17:59:00.480273 undumper-0.0.2/LICENSE
--rw-r--r--   0        0        0     2928 2024-05-22 17:59:00.480273 undumper-0.0.2/README.md
--rw-r--r--   0        0        0      445 2024-05-22 17:59:00.480273 undumper-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6830 2024-05-22 17:59:00.480273 undumper-0.0.2/undumper/undumper.py
--rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 undumper-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-27 16:39:55.216790 undumper-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2928 2024-05-27 16:39:55.220790 undumper-0.0.3/README.md
+-rw-r--r--   0        0        0      445 2024-05-27 16:39:55.220790 undumper-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 16:39:55.220790 undumper-0.0.3/undumper/__init__.py
+-rw-r--r--   0        0        0     6830 2024-05-27 16:39:55.220790 undumper-0.0.3/undumper/undumper.py
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 undumper-0.0.3/PKG-INFO
```

### Comparing `undumper-0.0.2/LICENSE` & `undumper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `undumper-0.0.2/README.md` & `undumper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `undumper-0.0.2/undumper/undumper.py` & `undumper-0.0.3/undumper/undumper.py`

 * *Files identical despite different names*

### Comparing `undumper-0.0.2/PKG-INFO` & `undumper-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unDumper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A fast and memory-efficient LAMMPS dump file reader with great developer experience
 License: MIT
 Author: Mohid Farooqi
 Author-email: mu2farooqi@uwaterloo.ca
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

