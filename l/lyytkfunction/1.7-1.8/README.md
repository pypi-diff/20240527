# Comparing `tmp/lyytkfunction-1.7.tar.gz` & `tmp/lyytkfunction-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyytkfunction-1.7.tar", last modified: Wed May  1 14:01:40 2024, max compression
+gzip compressed data, was "lyytkfunction-1.8.tar", last modified: Mon May 27 10:39:53 2024, max compression
```

## Comparing `lyytkfunction-1.7.tar` & `lyytkfunction-1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:01:40.521630 lyytkfunction-1.7/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytkfunction-1.7/LICENSE
--rw-rw-rw-   0        0        0      150 2024-05-01 14:01:40.521630 lyytkfunction-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytkfunction-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 14:01:40.520628 lyytkfunction-1.7/lyytkfunction.egg-info/
--rw-rw-rw-   0        0        0      150 2024-05-01 14:01:40.000000 lyytkfunction-1.7/lyytkfunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-05-01 14:01:40.000000 lyytkfunction-1.7/lyytkfunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:01:40.000000 lyytkfunction-1.7/lyytkfunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 14:01:40.000000 lyytkfunction-1.7/lyytkfunction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 14:01:40.000000 lyytkfunction-1.7/lyytkfunction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1071 2023-10-28 18:51:52.000000 lyytkfunction-1.7/lyytkfunction.py
--rw-rw-rw-   0        0        0       42 2024-05-01 14:01:40.521630 lyytkfunction-1.7/setup.cfg
--rw-rw-rw-   0        0        0      275 2024-05-01 14:01:39.000000 lyytkfunction-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:39:53.837006 lyytkfunction-1.8/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytkfunction-1.8/LICENSE
+-rw-rw-rw-   0        0        0      177 2024-05-27 10:39:53.835005 lyytkfunction-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytkfunction-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:39:53.834004 lyytkfunction-1.8/lyytkfunction.egg-info/
+-rw-rw-rw-   0        0        0      177 2024-05-27 10:39:53.000000 lyytkfunction-1.8/lyytkfunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-27 10:39:53.000000 lyytkfunction-1.8/lyytkfunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:39:53.000000 lyytkfunction-1.8/lyytkfunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 10:39:53.000000 lyytkfunction-1.8/lyytkfunction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 10:39:53.000000 lyytkfunction-1.8/lyytkfunction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14524 2024-05-27 10:39:46.000000 lyytkfunction-1.8/lyytkfunction.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:39:53.837006 lyytkfunction-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      275 2024-05-27 10:39:52.000000 lyytkfunction-1.8/setup.py
```

### Comparing `lyytkfunction-1.7/LICENSE` & `lyytkfunction-1.8/LICENSE`

 * *Files identical despite different names*

