# Comparing `tmp/bstblue-0.1.0.tar.gz` & `tmp/bstblue-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstblue-0.1.0.tar", last modified: Fri May 24 10:16:11 2024, max compression
+gzip compressed data, was "bstblue-0.1.1.tar", last modified: Mon May 27 10:58:48 2024, max compression
```

## Comparing `bstblue-0.1.0.tar` & `bstblue-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 10:16:11.809100 bstblue-0.1.0/
--rw-rw-rw-   0        0        0        0 2024-05-23 13:29:33.000000 bstblue-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1297 2024-05-24 10:16:11.808102 bstblue-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      804 2024-05-24 10:10:49.000000 bstblue-0.1.0/README.md
--rw-rw-rw-   0        0        0      103 2024-05-23 13:32:24.000000 bstblue-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      632 2024-05-24 10:16:11.813089 bstblue-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-24 10:16:11.732304 bstblue-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-24 10:16:11.774222 bstblue-0.1.0/src/bstblue/
--rw-rw-rw-   0        0        0        0 2024-05-23 13:48:24.000000 bstblue-0.1.0/src/bstblue/__init__.py
--rw-rw-rw-   0        0        0      115 2024-05-24 10:14:56.000000 bstblue-0.1.0/src/bstblue/wbdev.py
--rw-rw-rw-   0        0        0      121 2024-05-24 10:15:34.000000 bstblue-0.1.0/src/bstblue/wbdevtz.py
--rw-rw-rw-   0        0        0      108 2024-05-24 10:15:20.000000 bstblue-0.1.0/src/bstblue/wbyt.py
-drwxrwxrwx   0        0        0        0 2024-05-24 10:16:11.805108 bstblue-0.1.0/src/bstblue.egg-info/
--rw-rw-rw-   0        0        0     1297 2024-05-24 10:16:11.000000 bstblue-0.1.0/src/bstblue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-24 10:16:11.000000 bstblue-0.1.0/src/bstblue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 10:16:11.000000 bstblue-0.1.0/src/bstblue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-24 10:16:11.000000 bstblue-0.1.0/src/bstblue.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 10:58:48.410346 bstblue-0.1.1/
+-rw-rw-rw-   0        0        0        0 2024-05-23 13:29:33.000000 bstblue-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1297 2024-05-27 10:58:48.409345 bstblue-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      804 2024-05-24 10:10:49.000000 bstblue-0.1.1/README.md
+-rw-rw-rw-   0        0        0      103 2024-05-23 13:32:24.000000 bstblue-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      632 2024-05-27 10:58:48.412393 bstblue-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 10:58:48.348646 bstblue-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 10:58:48.365157 bstblue-0.1.1/src/bstblue/
+-rw-rw-rw-   0        0        0        0 2024-05-27 07:28:41.000000 bstblue-0.1.1/src/bstblue/__init__.py
+-rw-rw-rw-   0        0        0     2065 2024-05-27 10:35:25.000000 bstblue-0.1.1/src/bstblue/install.py
+-rw-rw-rw-   0        0        0      115 2024-05-24 10:14:56.000000 bstblue-0.1.1/src/bstblue/wbdev.py
+-rw-rw-rw-   0        0        0      121 2024-05-24 10:15:34.000000 bstblue-0.1.1/src/bstblue/wbdevtz.py
+-rw-rw-rw-   0        0        0      108 2024-05-24 15:04:59.000000 bstblue-0.1.1/src/bstblue/wbyt.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:58:48.398574 bstblue-0.1.1/src/bstblue.egg-info/
+-rw-rw-rw-   0        0        0     1297 2024-05-27 10:58:48.000000 bstblue-0.1.1/src/bstblue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-27 10:58:48.000000 bstblue-0.1.1/src/bstblue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:58:48.000000 bstblue-0.1.1/src/bstblue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 10:58:48.000000 bstblue-0.1.1/src/bstblue.egg-info/top_level.txt
```

### Comparing `bstblue-0.1.0/PKG-INFO` & `bstblue-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstblue
-Version: 0.1.0
+Version: 0.1.1
 Summary: bstblue
 Home-page: https://github.com/Blueboy0999/bstblue/
 Author: Blueboy
 Author-email: contact-pypi@blueboy.dev
 Project-URL: Bug Tracker, https://github.com/Blueboy0999/bstblue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bstblue-0.1.0/README.md` & `bstblue-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bstblue-0.1.0/setup.cfg` & `bstblue-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7374 626c 7565 0d0a 7665 7273   = bstblue..vers
-00000020: 696f 6e20 3d20 302e 312e 300d 0a61 7574  ion = 0.1.0..aut
+00000020: 696f 6e20 3d20 302e 312e 310d 0a61 7574  ion = 0.1.1..aut
 00000030: 686f 7220 3d20 426c 7565 626f 790d 0a61  hor = Blueboy..a
 00000040: 7574 686f 725f 656d 6169 6c20 3d20 636f  uthor_email = co
 00000050: 6e74 6163 742d 7079 7069 4062 6c75 6562  ntact-pypi@blueb
 00000060: 6f79 2e64 6576 0d0a 6465 7363 7269 7074  oy.dev..descript
 00000070: 696f 6e20 3d20 6273 7462 6c75 650d 0a6c  ion = bstblue..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
```

### Comparing `bstblue-0.1.0/src/bstblue.egg-info/PKG-INFO` & `bstblue-0.1.1/src/bstblue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstblue
-Version: 0.1.0
+Version: 0.1.1
 Summary: bstblue
 Home-page: https://github.com/Blueboy0999/bstblue/
 Author: Blueboy
 Author-email: contact-pypi@blueboy.dev
 Project-URL: Bug Tracker, https://github.com/Blueboy0999/bstblue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

