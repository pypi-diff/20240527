# Comparing `tmp/lyytkwidget-1.6.tar.gz` & `tmp/lyytkwidget-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyytkwidget-1.6.tar", last modified: Thu May  2 12:51:05 2024, max compression
+gzip compressed data, was "lyytkwidget-1.7.tar", last modified: Mon May 27 09:38:54 2024, max compression
```

## Comparing `lyytkwidget-1.6.tar` & `lyytkwidget-1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:51:05.229514 lyytkwidget-1.6/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytkwidget-1.6/LICENSE
--rw-rw-rw-   0        0        0      148 2024-05-02 12:51:05.228505 lyytkwidget-1.6/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytkwidget-1.6/README.md
--rw-rw-rw-   0        0        0     1071 2023-10-28 18:51:52.000000 lyytkwidget-1.6/lyyguifunction.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:51:05.227003 lyytkwidget-1.6/lyytkwidget.egg-info/
--rw-rw-rw-   0        0        0      148 2024-05-02 12:51:05.000000 lyytkwidget-1.6/lyytkwidget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-02 12:51:05.000000 lyytkwidget-1.6/lyytkwidget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:51:05.000000 lyytkwidget-1.6/lyytkwidget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 12:51:05.000000 lyytkwidget-1.6/lyytkwidget.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-02 12:51:05.000000 lyytkwidget-1.6/lyytkwidget.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 12:51:05.229514 lyytkwidget-1.6/setup.cfg
--rw-rw-rw-   0        0        0      273 2024-05-02 12:51:04.000000 lyytkwidget-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:38:54.929870 lyytkwidget-1.7/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytkwidget-1.7/LICENSE
+-rw-rw-rw-   0        0        0      175 2024-05-27 09:38:54.927870 lyytkwidget-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytkwidget-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 09:38:54.926870 lyytkwidget-1.7/lyytkwidget.egg-info/
+-rw-rw-rw-   0        0        0      175 2024-05-27 09:38:54.000000 lyytkwidget-1.7/lyytkwidget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-27 09:38:54.000000 lyytkwidget-1.7/lyytkwidget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 09:38:54.000000 lyytkwidget-1.7/lyytkwidget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 09:38:54.000000 lyytkwidget-1.7/lyytkwidget.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 09:38:54.000000 lyytkwidget-1.7/lyytkwidget.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22864 2024-05-27 09:37:41.000000 lyytkwidget-1.7/lyytkwidget.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 09:38:54.929870 lyytkwidget-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      273 2024-05-27 09:38:54.000000 lyytkwidget-1.7/setup.py
```

### Comparing `lyytkwidget-1.6/LICENSE` & `lyytkwidget-1.7/LICENSE`

 * *Files identical despite different names*

