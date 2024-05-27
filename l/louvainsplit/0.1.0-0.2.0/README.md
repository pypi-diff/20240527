# Comparing `tmp/louvainsplit-0.1.0.tar.gz` & `tmp/louvainsplit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "louvainsplit-0.1.0.tar", last modified: Sun May 26 15:21:56 2024, max compression
+gzip compressed data, was "louvainsplit-0.2.0.tar", last modified: Sun May 26 23:59:29 2024, max compression
```

## Comparing `louvainsplit-0.1.0.tar` & `louvainsplit-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:21:56.866048 louvainsplit-0.1.0/
--rw-rw-rw-   0        0        0     1119 2024-05-26 14:11:51.000000 louvainsplit-0.1.0/LICENCE
--rw-rw-rw-   0        0        0      848 2024-05-26 15:21:56.865048 louvainsplit-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2297 2024-05-26 14:11:20.000000 louvainsplit-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 15:21:56.804050 louvainsplit-0.1.0/louvainsplit/
--rw-rw-rw-   0        0        0      160 2024-05-26 14:22:35.000000 louvainsplit-0.1.0/louvainsplit/__init__.py
--rw-rw-rw-   0        0        0     1347 2024-05-26 14:22:48.000000 louvainsplit-0.1.0/louvainsplit/feature_extraction.py
--rw-rw-rw-   0        0        0      819 2024-05-26 14:22:59.000000 louvainsplit-0.1.0/louvainsplit/louvain_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:21:56.854049 louvainsplit-0.1.0/louvainsplit/tests/
--rw-rw-rw-   0        0        0        0 2024-05-26 14:21:04.000000 louvainsplit-0.1.0/louvainsplit/tests/__init__.py
--rw-rw-rw-   0        0        0      555 2024-05-26 14:23:19.000000 louvainsplit-0.1.0/louvainsplit/tests/test_louvain_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:21:56.864052 louvainsplit-0.1.0/louvainsplit.egg-info/
--rw-rw-rw-   0        0        0      848 2024-05-26 15:21:56.000000 louvainsplit-0.1.0/louvainsplit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-05-26 15:21:56.000000 louvainsplit-0.1.0/louvainsplit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:21:56.000000 louvainsplit-0.1.0/louvainsplit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-26 15:21:56.000000 louvainsplit-0.1.0/louvainsplit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-26 15:21:56.000000 louvainsplit-0.1.0/louvainsplit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 15:21:56.866048 louvainsplit-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      965 2024-05-26 14:10:30.000000 louvainsplit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:59:29.303366 louvainsplit-0.2.0/
+-rw-rw-rw-   0        0        0     1119 2024-05-26 14:11:51.000000 louvainsplit-0.2.0/LICENCE
+-rw-rw-rw-   0        0        0     5205 2024-05-26 23:59:29.301367 louvainsplit-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4314 2024-05-26 23:57:01.000000 louvainsplit-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 23:59:29.283367 louvainsplit-0.2.0/louvainsplit/
+-rw-rw-rw-   0        0        0      160 2024-05-26 14:22:35.000000 louvainsplit-0.2.0/louvainsplit/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-05-26 14:22:48.000000 louvainsplit-0.2.0/louvainsplit/feature_extraction.py
+-rw-rw-rw-   0        0        0      819 2024-05-26 14:22:59.000000 louvainsplit-0.2.0/louvainsplit/louvain_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:59:29.299366 louvainsplit-0.2.0/louvainsplit/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-26 14:21:04.000000 louvainsplit-0.2.0/louvainsplit/tests/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-05-26 14:23:19.000000 louvainsplit-0.2.0/louvainsplit/tests/test_louvain_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:59:29.300365 louvainsplit-0.2.0/louvainsplit.egg-info/
+-rw-rw-rw-   0        0        0     5205 2024-05-26 23:59:29.000000 louvainsplit-0.2.0/louvainsplit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-05-26 23:59:29.000000 louvainsplit-0.2.0/louvainsplit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 23:59:29.000000 louvainsplit-0.2.0/louvainsplit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-26 23:59:29.000000 louvainsplit-0.2.0/louvainsplit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-26 23:59:29.000000 louvainsplit-0.2.0/louvainsplit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 23:59:29.303366 louvainsplit-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-05-26 23:58:07.000000 louvainsplit-0.2.0/setup.py
```

### Comparing `louvainsplit-0.1.0/LICENCE` & `louvainsplit-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.1.0/louvainsplit/feature_extraction.py` & `louvainsplit-0.2.0/louvainsplit/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.1.0/louvainsplit/louvain_algorithm.py` & `louvainsplit-0.2.0/louvainsplit/louvain_algorithm.py`

 * *Files identical despite different names*

### Comparing `louvainsplit-0.1.0/louvainsplit/tests/test_louvain_algorithm.py` & `louvainsplit-0.2.0/louvainsplit/tests/test_louvain_algorithm.py`

 * *Files identical despite different names*

