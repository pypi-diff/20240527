# Comparing `tmp/abadpour-6.23.1.tar.gz` & `tmp/abadpour-6.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abadpour-6.23.1.tar", last modified: Sun May 26 17:52:09 2024, max compression
+gzip compressed data, was "abadpour-6.24.1.tar", last modified: Sun May 26 20:37:39 2024, max compression
```

## Comparing `abadpour-6.23.1.tar` & `abadpour-6.24.1.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:52:09.091318 abadpour-6.23.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 17:51:52.000000 abadpour-6.23.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-26 17:52:09.090862 abadpour-6.23.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      502 2024-05-26 17:51:52.000000 abadpour-6.23.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:52:09.087679 abadpour-6.23.1/abadpour/
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 17:52:03.000000 abadpour-6.23.1/abadpour/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      573 2024-05-26 17:51:52.000000 abadpour-6.23.1/abadpour/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      211 2024-05-26 17:51:52.000000 abadpour-6.23.1/abadpour/build.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-26 17:51:52.000000 abadpour-6.23.1/abadpour/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 17:51:52.000000 abadpour-6.23.1/abadpour/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:52:09.090338 abadpour-6.23.1/abadpour.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-26 17:52:09.000000 abadpour-6.23.1/abadpour.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      317 2024-05-26 17:52:09.000000 abadpour-6.23.1/abadpour.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 17:52:09.000000 abadpour-6.23.1/abadpour.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       79 2024-05-26 17:52:09.000000 abadpour-6.23.1/abadpour.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-26 17:52:09.000000 abadpour-6.23.1/abadpour.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 17:51:52.000000 abadpour-6.23.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)       78 2024-05-26 17:51:52.000000 abadpour-6.23.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 17:52:09.091386 abadpour-6.23.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      219 2024-05-26 17:51:52.000000 abadpour-6.23.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:37:39.284006 abadpour-6.24.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 17:51:52.000000 abadpour-6.24.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-26 20:37:39.283206 abadpour-6.24.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      502 2024-05-26 17:51:52.000000 abadpour-6.24.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:37:39.273127 abadpour-6.24.1/abadpour/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:37:39.280023 abadpour-6.24.1/abadpour/.abcli/
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      267 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/CV.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       95 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/abcli.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      134 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       56 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1315 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/build.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      353 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/clean.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:37:39.281227 abadpour-6.24.1/abadpour/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/tests/build.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      198 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 20:37:33.000000 abadpour-6.24.1/abadpour/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      573 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      211 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/build.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 17:51:52.000000 abadpour-6.24.1/abadpour/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:37:39.282137 abadpour-6.24.1/abadpour.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-26 20:37:39.000000 abadpour-6.24.1/abadpour.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      528 2024-05-26 20:37:39.000000 abadpour-6.24.1/abadpour.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 20:37:39.000000 abadpour-6.24.1/abadpour.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       79 2024-05-26 20:37:39.000000 abadpour-6.24.1/abadpour.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-26 20:37:39.000000 abadpour-6.24.1/abadpour.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 17:51:52.000000 abadpour-6.24.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)       78 2024-05-26 17:51:52.000000 abadpour-6.24.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 20:37:39.284141 abadpour-6.24.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      333 2024-05-26 20:37:26.000000 abadpour-6.24.1/setup.py
```

### Comparing `abadpour-6.23.1/PKG-INFO` & `abadpour-6.24.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abadpour
-Version: 6.23.1
+Version: 6.24.1
 Summary: 📜 Arash Abadpour's CV.
 Home-page: https://github.com/kamangir/CV
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abadpour-6.23.1/abadpour/__main__.py` & `abadpour-6.24.1/abadpour/__main__.py`

 * *Files identical despite different names*

### Comparing `abadpour-6.23.1/abadpour.egg-info/PKG-INFO` & `abadpour-6.24.1/abadpour.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abadpour
-Version: 6.23.1
+Version: 6.24.1
 Summary: 📜 Arash Abadpour's CV.
 Home-page: https://github.com/kamangir/CV
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

