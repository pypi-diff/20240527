# Comparing `tmp/pypdf2htmlex-1.1.tar.gz` & `tmp/pypdf2htmlex-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdf2htmlex-1.1.tar", last modified: Fri May 24 22:38:44 2024, max compression
+gzip compressed data, was "pypdf2htmlex-1.3.tar", last modified: Mon May 27 13:24:12 2024, max compression
```

## Comparing `pypdf2htmlex-1.1.tar` & `pypdf2htmlex-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/pypdf2htmlEX/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/pypdf2htmlEX/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/pypdf2htmlEX/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 22:38:44.000000 pypdf2htmlex-1.1/pypdf2htmlex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:38:44.621617 pypdf2htmlex-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-24 22:38:38.000000 pypdf2htmlex-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:24:12.273858 pypdf2htmlex-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 13:24:08.000000 pypdf2htmlex-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-27 13:24:12.273858 pypdf2htmlex-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-27 13:24:08.000000 pypdf2htmlex-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:24:12.269858 pypdf2htmlex-1.3/pypdf2htmlEX/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 13:24:08.000000 pypdf2htmlex-1.3/pypdf2htmlEX/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-27 13:24:08.000000 pypdf2htmlex-1.3/pypdf2htmlEX/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:24:12.273858 pypdf2htmlex-1.3/pypdf2htmlex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-27 13:24:12.000000 pypdf2htmlex-1.3/pypdf2htmlex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-27 13:24:12.000000 pypdf2htmlex-1.3/pypdf2htmlex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:24:12.000000 pypdf2htmlex-1.3/pypdf2htmlex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 13:24:12.000000 pypdf2htmlex-1.3/pypdf2htmlex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:24:12.273858 pypdf2htmlex-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-27 13:24:08.000000 pypdf2htmlex-1.3/setup.py
```

### Comparing `pypdf2htmlex-1.1/LICENSE` & `pypdf2htmlex-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdf2htmlex-1.1/PKG-INFO` & `pypdf2htmlex-1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pypdf2htmlex
-Version: 1.1
+Version: 1.3
 Summary: Wrapper não oficial do pdf2htmlEX
+Home-page: https://github.com/gabriel-batistuta/pypdf2htmlEX
 Author: Gabriel Batistuta
 Author-email: batistutag190@gmail.com
 License: MIT License
+Project-URL: Repository, https://github.com/gabriel-batistuta/pypdf2htmlEX
 Keywords: pdf2htmlEX pdf-to-html pdf html wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDF2HTMLEX
 pypdf2htmlex is a Python wrapper for the PDF2HTMLEX
```

### Comparing `pypdf2htmlex-1.1/README.md` & `pypdf2htmlex-1.3/README.md`

 * *Files identical despite different names*

### Comparing `pypdf2htmlex-1.1/pypdf2htmlEX/core.py` & `pypdf2htmlex-1.3/pypdf2htmlEX/core.py`

 * *Files identical despite different names*

### Comparing `pypdf2htmlex-1.1/pypdf2htmlex.egg-info/PKG-INFO` & `pypdf2htmlex-1.3/pypdf2htmlex.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: pypdf2htmlex
-Version: 1.1
+Version: 1.3
 Summary: Wrapper não oficial do pdf2htmlEX
+Home-page: https://github.com/gabriel-batistuta/pypdf2htmlEX
 Author: Gabriel Batistuta
 Author-email: batistutag190@gmail.com
 License: MIT License
+Project-URL: Repository, https://github.com/gabriel-batistuta/pypdf2htmlEX
 Keywords: pdf2htmlEX pdf-to-html pdf html wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDF2HTMLEX
 pypdf2htmlex is a Python wrapper for the PDF2HTMLEX
```

