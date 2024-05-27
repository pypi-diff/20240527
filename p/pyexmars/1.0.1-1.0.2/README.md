# Comparing `tmp/pyexmars-1.0.1.tar.gz` & `tmp/pyexmars-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyexmars-1.0.1.tar", last modified: Mon May 27 08:36:35 2024, max compression
+gzip compressed data, was "pyexmars-1.0.2.tar", last modified: Mon May 27 08:48:55 2024, max compression
```

## Comparing `pyexmars-1.0.1.tar` & `pyexmars-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 08:36:35.925475 pyexmars-1.0.1/
--rw-rw-rw-   0        0        0       55 2024-05-27 08:36:35.924969 pyexmars-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 08:36:35.922488 pyexmars-1.0.1/pyexmars.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 08:36:35.925475 pyexmars-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      256 2024-05-27 08:36:11.000000 pyexmars-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:48:55.627059 pyexmars-1.0.2/
+-rw-rw-rw-   0        0        0       55 2024-05-27 08:48:55.626060 pyexmars-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 08:48:55.594231 pyexmars-1.0.2/pyexmars/
+-rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.2/pyexmars/__init__.py
+-rw-rw-rw-   0        0        0      683 2024-05-10 06:20:11.000000 pyexmars-1.0.2/pyexmars/pyexmars.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:48:55.624044 pyexmars-1.0.2/pyexmars.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 08:48:55.000000 pyexmars-1.0.2/pyexmars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 08:48:55.627059 pyexmars-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      261 2024-05-27 08:44:32.000000 pyexmars-1.0.2/setup.py
```

