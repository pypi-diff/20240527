# Comparing `tmp/lyyinit-1.2.tar.gz` & `tmp/lyyinit-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyinit-1.2.tar", last modified: Sun Apr 14 06:29:17 2024, max compression
+gzip compressed data, was "lyyinit-1.4.tar", last modified: Mon May 27 10:35:51 2024, max compression
```

## Comparing `lyyinit-1.2.tar` & `lyyinit-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 06:29:17.556602 lyyinit-1.2/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyinit-1.2/LICENSE
--rw-rw-rw-   0        0        0      158 2024-04-14 06:29:17.555098 lyyinit-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyinit-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 06:29:17.555098 lyyinit-1.2/lyyinit.egg-info/
--rw-rw-rw-   0        0        0      158 2024-04-14 06:29:17.000000 lyyinit-1.2/lyyinit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-04-14 06:29:17.000000 lyyinit-1.2/lyyinit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 06:29:17.000000 lyyinit-1.2/lyyinit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 06:29:17.000000 lyyinit-1.2/lyyinit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1118 2024-04-14 06:28:13.000000 lyyinit-1.2/lyyinit.py
--rw-rw-rw-   0        0        0       42 2024-04-14 06:29:17.556602 lyyinit-1.2/setup.cfg
--rw-rw-rw-   0        0        0      261 2024-04-14 06:29:16.000000 lyyinit-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:35:51.510910 lyyinit-1.4/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyinit-1.4/LICENSE
+-rw-rw-rw-   0        0        0      158 2024-05-27 10:35:51.507910 lyyinit-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyinit-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:35:51.504911 lyyinit-1.4/lyyinit.egg-info/
+-rw-rw-rw-   0        0        0      158 2024-05-27 10:35:51.000000 lyyinit-1.4/lyyinit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-27 10:35:51.000000 lyyinit-1.4/lyyinit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:35:51.000000 lyyinit-1.4/lyyinit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 10:35:51.000000 lyyinit-1.4/lyyinit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12760 2024-05-27 10:35:44.000000 lyyinit-1.4/lyyinit.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:35:51.510910 lyyinit-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      261 2024-05-27 10:35:50.000000 lyyinit-1.4/setup.py
```

### Comparing `lyyinit-1.2/LICENSE` & `lyyinit-1.4/LICENSE`

 * *Files identical despite different names*

