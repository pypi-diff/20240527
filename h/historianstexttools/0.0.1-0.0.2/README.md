# Comparing `tmp/historianstexttools-0.0.1.tar.gz` & `tmp/historianstexttools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "historianstexttools-0.0.1.tar", last modified: Wed Apr 24 02:55:57 2024, max compression
+gzip compressed data, was "historianstexttools-0.0.2.tar", last modified: Mon May 27 04:49:03 2024, max compression
```

## Comparing `historianstexttools-0.0.1.tar` & `historianstexttools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 cgoodwin  (1000) cgoodwin  (1000)        0 2024-04-24 02:55:57.369351 historianstexttools-0.0.1/
--rw-r--r--   0 cgoodwin  (1000) cgoodwin  (1000)      544 2024-04-24 02:55:57.369351 historianstexttools-0.0.1/PKG-INFO
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)       79 2024-04-24 02:40:28.000000 historianstexttools-0.0.1/README.md
-drwxrwxr-x   0 cgoodwin  (1000) cgoodwin  (1000)        0 2024-04-24 02:55:57.369351 historianstexttools-0.0.1/historianstexttools.egg-info/
--rw-r--r--   0 cgoodwin  (1000) cgoodwin  (1000)      544 2024-04-24 02:55:57.000000 historianstexttools-0.0.1/historianstexttools.egg-info/PKG-INFO
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)      275 2024-04-24 02:55:57.000000 historianstexttools-0.0.1/historianstexttools.egg-info/SOURCES.txt
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)        1 2024-04-24 02:55:57.000000 historianstexttools-0.0.1/historianstexttools.egg-info/dependency_links.txt
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)        4 2024-04-24 02:55:57.000000 historianstexttools-0.0.1/historianstexttools.egg-info/top_level.txt
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)       38 2024-04-24 02:55:57.369351 historianstexttools-0.0.1/setup.cfg
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)      847 2024-04-24 02:55:49.000000 historianstexttools-0.0.1/setup.py
-drwxrwxr-x   0 cgoodwin  (1000) cgoodwin  (1000)        0 2024-04-24 02:55:57.369351 historianstexttools-0.0.1/src/
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)        0 2024-04-24 02:37:25.000000 historianstexttools-0.0.1/src/__init__.py
-drwxrwxr-x   0 cgoodwin  (1000) cgoodwin  (1000)        0 2024-04-24 02:55:57.369351 historianstexttools-0.0.1/src/historianstexttools/
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)        0 2024-04-24 02:41:00.000000 historianstexttools-0.0.1/src/historianstexttools/__init__.py
--rw-rw-r--   0 cgoodwin  (1000) cgoodwin  (1000)       73 2024-04-24 02:35:31.000000 historianstexttools-0.0.1/src/historianstexttools/chunk.py
+drwxr-xr-x   0 cgoodwin   (501) staff       (20)        0 2024-05-27 04:49:03.930288 historianstexttools-0.0.2/
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      599 2024-05-27 04:49:03.930180 historianstexttools-0.0.2/PKG-INFO
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      117 2024-04-24 03:34:25.000000 historianstexttools-0.0.2/README.md
+drwxr-xr-x   0 cgoodwin   (501) staff       (20)        0 2024-05-27 04:49:03.929040 historianstexttools-0.0.2/historianstexttools.egg-info/
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      599 2024-05-27 04:49:03.000000 historianstexttools-0.0.2/historianstexttools.egg-info/PKG-INFO
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      474 2024-05-27 04:49:03.000000 historianstexttools-0.0.2/historianstexttools.egg-info/SOURCES.txt
+-rw-r--r--   0 cgoodwin   (501) staff       (20)        1 2024-05-27 04:49:03.000000 historianstexttools-0.0.2/historianstexttools.egg-info/dependency_links.txt
+-rw-r--r--   0 cgoodwin   (501) staff       (20)       25 2024-05-27 04:49:03.000000 historianstexttools-0.0.2/historianstexttools.egg-info/requires.txt
+-rw-r--r--   0 cgoodwin   (501) staff       (20)        4 2024-05-27 04:49:03.000000 historianstexttools-0.0.2/historianstexttools.egg-info/top_level.txt
+-rw-r--r--   0 cgoodwin   (501) staff       (20)       38 2024-05-27 04:49:03.930327 historianstexttools-0.0.2/setup.cfg
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      993 2024-05-27 04:48:45.000000 historianstexttools-0.0.2/setup.py
+drwxr-xr-x   0 cgoodwin   (501) staff       (20)        0 2024-05-27 04:49:03.929161 historianstexttools-0.0.2/src/
+-rw-r--r--   0 cgoodwin   (501) staff       (20)        0 2024-04-24 03:34:25.000000 historianstexttools-0.0.2/src/__init__.py
+drwxr-xr-x   0 cgoodwin   (501) staff       (20)        0 2024-05-27 04:49:03.930034 historianstexttools-0.0.2/src/historianstexttools/
+-rw-r--r--   0 cgoodwin   (501) staff       (20)        0 2024-04-24 03:34:25.000000 historianstexttools-0.0.2/src/historianstexttools/__init__.py
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      998 2024-05-27 04:41:29.000000 historianstexttools-0.0.2/src/historianstexttools/chunking.py
+-rw-r--r--   0 cgoodwin   (501) staff       (20)     2590 2024-05-27 04:48:22.000000 historianstexttools-0.0.2/src/historianstexttools/cleantext.py
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      150 2024-05-27 04:17:28.000000 historianstexttools-0.0.2/src/historianstexttools/dataloaders.py
+-rw-r--r--   0 cgoodwin   (501) staff       (20)      172 2024-04-26 17:27:33.000000 historianstexttools-0.0.2/src/historianstexttools/filemanipulation.py
+-rw-r--r--   0 cgoodwin   (501) staff       (20)     1053 2024-05-27 04:47:09.000000 historianstexttools-0.0.2/src/historianstexttools/tester.py
```

