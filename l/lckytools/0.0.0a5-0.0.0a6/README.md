# Comparing `tmp/lckytools-0.0.0a5.tar.gz` & `tmp/lckytools-0.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.0a5.tar", max compression
+gzip compressed data, was "lckytools-0.0.0a6.tar", max compression
```

## Comparing `lckytools-0.0.0a5.tar` & `lckytools-0.0.0a6.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      294 2024-05-27 02:52:50.801135 lckytools-0.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a5/README.md
--rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a5/src/lckytools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 02:49:11.736063 lckytools-0.0.0a5/src/lckytools/ai/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 02:49:12.032838 lckytools-0.0.0a5/src/lckytools/ai/metrics/__init__.py
--rw-r--r--   0        0        0      794 2024-05-27 02:49:12.249780 lckytools-0.0.0a5/src/lckytools/ai/metrics/confusion_matrix.py
--rw-r--r--   0        0        0        0 2024-05-27 01:21:26.273683 lckytools-0.0.0a5/src/lckytools/ai/torch/__init__.py
--rw-r--r--   0        0        0       34 2024-05-27 01:45:10.349737 lckytools-0.0.0a5/src/lckytools/ai/torch/summary_model.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 lckytools-0.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-27 03:04:13.567796 lckytools-0.0.0a6/LICENSE
+-rw-r--r--   0        0        0      516 2024-05-27 04:00:52.639676 lckytools-0.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     1423 2024-05-27 01:01:39.126939 lckytools-0.0.0a6/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a6/src/lckytools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a6/src/lckytools/core/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-27 03:49:27.940843 lckytools-0.0.0a6/src/lckytools/core/hello.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:47:26.411528 lckytools-0.0.0a6/src/lckytools.ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:49:11.736063 lckytools-0.0.0a6/src/lckytools.ai/ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:49:12.032838 lckytools-0.0.0a6/src/lckytools.ai/ai/metrics/__init__.py
+-rw-r--r--   0        0        0      911 2024-05-27 03:07:44.681865 lckytools-0.0.0a6/src/lckytools.ai/ai/metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 lckytools-0.0.0a6/PKG-INFO
```

### Comparing `lckytools-0.0.0a5/README.md` & `lckytools-0.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.0a5/PKG-INFO` & `lckytools-0.0.0a6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: 
 License: MIT
 Author: LCKYN
 Author-email: T.Pawarit@lckyn.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: ai
+Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
+Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # LckyTools
 
 this sentence below I use chatGPT to generate it, it's not real, but looks like real, I will update it later.
 
 This repository contains a collection of code snippets and modules that have been developed to streamline and enhance the efficiency of multiple projects. The primary intent behind this compilation is to offer a centralized resource where commonly used code segments are readily available, thus facilitating easier and quicker integration into various projects. This approach not only ensures consistency across different applications but also significantly reduces development time by eliminating the need to repeatedly write the same code.
```

