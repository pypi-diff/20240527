# Comparing `tmp/NameExtractor-1.0.2.tar.gz` & `tmp/NameExtractor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NameExtractor-1.0.2.tar", last modified: Mon May 27 17:21:39 2024, max compression
+gzip compressed data, was "dist/NameExtractor-1.0.3.tar", last modified: Mon May 27 17:33:29 2024, max compression
```

## Comparing `NameExtractor-1.0.2.tar` & `NameExtractor-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 WillBallantine   (501) staff       (20)        0 2024-05-27 17:21:39.310075 NameExtractor-1.0.2/
--rw-r--r--   0 WillBallantine   (501) staff       (20)     1437 2024-05-27 17:21:39.309828 NameExtractor-1.0.2/PKG-INFO
--rw-r--r--   0 WillBallantine   (501) staff       (20)      851 2024-05-27 17:20:29.000000 NameExtractor-1.0.2/README.md
--rw-r--r--   0 WillBallantine   (501) staff       (20)       38 2024-05-27 17:21:39.310210 NameExtractor-1.0.2/setup.cfg
--rw-r--r--   0 WillBallantine   (501) staff       (20)      467 2024-05-27 17:21:33.000000 NameExtractor-1.0.2/setup.py
-drwxr-xr-x   0 WillBallantine   (501) staff       (20)        0 2024-05-27 17:21:39.307161 NameExtractor-1.0.2/src/
-drwxr-xr-x   0 WillBallantine   (501) staff       (20)        0 2024-05-27 17:21:39.309397 NameExtractor-1.0.2/src/NameExtractor.egg-info/
--rw-r--r--   0 WillBallantine   (501) staff       (20)     1437 2024-05-27 17:21:39.000000 NameExtractor-1.0.2/src/NameExtractor.egg-info/PKG-INFO
--rw-r--r--   0 WillBallantine   (501) staff       (20)      182 2024-05-27 17:21:39.000000 NameExtractor-1.0.2/src/NameExtractor.egg-info/SOURCES.txt
--rw-r--r--   0 WillBallantine   (501) staff       (20)        1 2024-05-27 17:21:39.000000 NameExtractor-1.0.2/src/NameExtractor.egg-info/dependency_links.txt
--rw-r--r--   0 WillBallantine   (501) staff       (20)        1 2024-05-27 17:21:39.000000 NameExtractor-1.0.2/src/NameExtractor.egg-info/top_level.txt
+drwxr-xr-x   0 WillBallantine   (501) staff       (20)        0 2024-05-27 17:33:29.397897 NameExtractor-1.0.3/
+-rw-r--r--   0 WillBallantine   (501) staff       (20)     1437 2024-05-27 17:33:29.397433 NameExtractor-1.0.3/PKG-INFO
+-rw-r--r--   0 WillBallantine   (501) staff       (20)      851 2024-05-27 17:20:29.000000 NameExtractor-1.0.3/README.md
+-rw-r--r--   0 WillBallantine   (501) staff       (20)       38 2024-05-27 17:33:29.398066 NameExtractor-1.0.3/setup.cfg
+-rw-r--r--   0 WillBallantine   (501) staff       (20)      549 2024-05-27 17:32:51.000000 NameExtractor-1.0.3/setup.py
+drwxr-xr-x   0 WillBallantine   (501) staff       (20)        0 2024-05-27 17:33:29.391554 NameExtractor-1.0.3/src/
+drwxr-xr-x   0 WillBallantine   (501) staff       (20)        0 2024-05-27 17:33:29.394048 NameExtractor-1.0.3/src/NameExtractor/
+-rw-r--r--   0 WillBallantine   (501) staff       (20)      143 2024-05-27 17:32:46.000000 NameExtractor-1.0.3/src/NameExtractor/__init__.py
+-rw-r--r--   0 WillBallantine   (501) staff       (20)      248 2024-05-27 00:12:48.000000 NameExtractor-1.0.3/src/NameExtractor/downloaded.py
+-rw-r--r--   0 WillBallantine   (501) staff       (20)     1842 2024-05-27 16:29:11.000000 NameExtractor-1.0.3/src/NameExtractor/names.py
+-rw-r--r--   0 WillBallantine   (501) staff       (20)      304 2024-05-27 00:05:24.000000 NameExtractor-1.0.3/src/NameExtractor/sslcert.py
+drwxr-xr-x   0 WillBallantine   (501) staff       (20)        0 2024-05-27 17:33:29.396826 NameExtractor-1.0.3/src/NameExtractor.egg-info/
+-rw-r--r--   0 WillBallantine   (501) staff       (20)     1437 2024-05-27 17:33:29.000000 NameExtractor-1.0.3/src/NameExtractor.egg-info/PKG-INFO
+-rw-r--r--   0 WillBallantine   (501) staff       (20)      340 2024-05-27 17:33:29.000000 NameExtractor-1.0.3/src/NameExtractor.egg-info/SOURCES.txt
+-rw-r--r--   0 WillBallantine   (501) staff       (20)        1 2024-05-27 17:33:29.000000 NameExtractor-1.0.3/src/NameExtractor.egg-info/dependency_links.txt
+-rw-r--r--   0 WillBallantine   (501) staff       (20)       11 2024-05-27 17:33:29.000000 NameExtractor-1.0.3/src/NameExtractor.egg-info/requires.txt
+-rw-r--r--   0 WillBallantine   (501) staff       (20)       14 2024-05-27 17:33:29.000000 NameExtractor-1.0.3/src/NameExtractor.egg-info/top_level.txt
```

### Comparing `NameExtractor-1.0.2/PKG-INFO` & `NameExtractor-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NameExtractor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Name Extractor is a small AI program to extract name and gender from characters in text.
 Home-page: https://github.com/xDefyingGravity/Name-Extractor/
 Author: Defying Gravity
 License: UNKNOWN
 Description: # Name Extractor
         ## Name Extractor is a small AI program that analyzes text for characters and retrieves their full names and genders
```

### Comparing `NameExtractor-1.0.2/README.md` & `NameExtractor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `NameExtractor-1.0.2/src/NameExtractor.egg-info/PKG-INFO` & `NameExtractor-1.0.3/src/NameExtractor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NameExtractor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Name Extractor is a small AI program to extract name and gender from characters in text.
 Home-page: https://github.com/xDefyingGravity/Name-Extractor/
 Author: Defying Gravity
 License: UNKNOWN
 Description: # Name Extractor
         ## Name Extractor is a small AI program that analyzes text for characters and retrieves their full names and genders
```

