# Comparing `tmp/copent-0.5.3.tar.gz` & `tmp/copent-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copent-0.5.3.tar", last modified: Mon May 27 20:59:17 2024, max compression
+gzip compressed data, was "copent-0.5.4.tar", last modified: Mon May 27 21:01:20 2024, max compression
```

## Comparing `copent-0.5.3.tar` & `copent-0.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 20:59:17.250081 copent-0.5.3/
--rw-rw-r--   0 majian    (1000) majian    (1000)    35149 2022-09-11 06:39:52.000000 copent-0.5.3/LICENSE
--rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 20:59:17.250081 copent-0.5.3/PKG-INFO
--rw-rw-r--   0 majian    (1000) majian    (1000)     5889 2024-03-14 23:57:08.000000 copent-0.5.3/README.md
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 20:59:17.250081 copent-0.5.3/copent/
--rw-rw-r--   0 majian    (1000) majian    (1000)       97 2024-02-12 06:43:57.000000 copent-0.5.3/copent/__init__.py
--rw-rw-r--   0 majian    (1000) majian    (1000)     5230 2024-05-27 20:58:51.000000 copent-0.5.3/copent/copent.py
-drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 20:59:17.250081 copent-0.5.3/copent.egg-info/
--rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 20:59:17.000000 copent-0.5.3/copent.egg-info/PKG-INFO
--rw-rw-r--   0 majian    (1000) majian    (1000)      211 2024-05-27 20:59:17.000000 copent-0.5.3/copent.egg-info/SOURCES.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)        1 2024-05-27 20:59:17.000000 copent-0.5.3/copent.egg-info/dependency_links.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)       12 2024-05-27 20:59:17.000000 copent-0.5.3/copent.egg-info/requires.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)        7 2024-05-27 20:59:17.000000 copent-0.5.3/copent.egg-info/top_level.txt
--rw-rw-r--   0 majian    (1000) majian    (1000)       38 2024-05-27 20:59:17.250081 copent-0.5.3/setup.cfg
--rw-rw-r--   0 majian    (1000) majian    (1000)      555 2024-05-27 20:57:59.000000 copent-0.5.3/setup.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:01:20.225587 copent-0.5.4/
+-rw-rw-r--   0 majian    (1000) majian    (1000)    35149 2022-09-11 06:39:52.000000 copent-0.5.4/LICENSE
+-rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 21:01:20.225587 copent-0.5.4/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)     5889 2024-03-14 23:57:08.000000 copent-0.5.4/README.md
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:01:20.225587 copent-0.5.4/copent/
+-rw-rw-r--   0 majian    (1000) majian    (1000)       97 2024-02-12 06:43:57.000000 copent-0.5.4/copent/__init__.py
+-rw-rw-r--   0 majian    (1000) majian    (1000)     5230 2024-05-27 20:58:51.000000 copent-0.5.4/copent/copent.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2024-05-27 21:01:20.225587 copent-0.5.4/copent.egg-info/
+-rw-rw-r--   0 majian    (1000) majian    (1000)     6220 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)      211 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/SOURCES.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        1 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/dependency_links.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       12 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/requires.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        7 2024-05-27 21:01:20.000000 copent-0.5.4/copent.egg-info/top_level.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       38 2024-05-27 21:01:20.225587 copent-0.5.4/setup.cfg
+-rw-rw-r--   0 majian    (1000) majian    (1000)      555 2024-05-27 21:01:04.000000 copent-0.5.4/setup.py
```

### Comparing `copent-0.5.3/LICENSE` & `copent-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `copent-0.5.3/PKG-INFO` & `copent-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copent
-Version: 0.5.3
+Version: 0.5.4
 Summary: Estimating Copula Entropy and Transfer Entropy
 Home-page: https://github.com/majianthu/pycopent
 Author: MA Jian
 Author-email: majian03@gmail.com
 License: GPL License
 Platform: UNKNOWN
 Requires-Python: >=2.7
```

### Comparing `copent-0.5.3/README.md` & `copent-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `copent-0.5.3/copent/copent.py` & `copent-0.5.4/copent/copent.py`

 * *Files identical despite different names*

### Comparing `copent-0.5.3/copent.egg-info/PKG-INFO` & `copent-0.5.4/copent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copent
-Version: 0.5.3
+Version: 0.5.4
 Summary: Estimating Copula Entropy and Transfer Entropy
 Home-page: https://github.com/majianthu/pycopent
 Author: MA Jian
 Author-email: majian03@gmail.com
 License: GPL License
 Platform: UNKNOWN
 Requires-Python: >=2.7
```

### Comparing `copent-0.5.3/setup.py` & `copent-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="copent",
-    version="0.5.3",
+    version="0.5.4",
     author="MA Jian",
     author_email="majian03@gmail.com",
     description="Estimating Copula Entropy and Transfer Entropy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPL License',
     url="https://github.com/majianthu/pycopent",
```

