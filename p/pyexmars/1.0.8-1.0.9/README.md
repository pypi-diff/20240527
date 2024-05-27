# Comparing `tmp/pyexmars-1.0.8.tar.gz` & `tmp/pyexmars-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyexmars-1.0.8.tar", last modified: Mon May 27 10:55:10 2024, max compression
+gzip compressed data, was "pyexmars-1.0.9.tar", last modified: Mon May 27 11:19:41 2024, max compression
```

## Comparing `pyexmars-1.0.8.tar` & `pyexmars-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 10:55:10.543564 pyexmars-1.0.8/
--rw-rw-rw-   0        0        0       55 2024-05-27 10:55:10.542411 pyexmars-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 10:55:10.523420 pyexmars-1.0.8/pyexmars/
--rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.8/pyexmars/__init__.py
--rw-rw-rw-   0        0        0      687 2024-05-27 10:51:19.000000 pyexmars-1.0.8/pyexmars/pyexmars.py
-drwxrwxrwx   0        0        0        0 2024-05-27 10:55:10.540228 pyexmars-1.0.8/pyexmars.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 10:55:10.000000 pyexmars-1.0.8/pyexmars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 10:55:10.543564 pyexmars-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      260 2024-05-27 10:54:46.000000 pyexmars-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:19:41.194340 pyexmars-1.0.9/
+-rw-rw-rw-   0        0        0       55 2024-05-27 11:19:41.192857 pyexmars-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 11:19:41.183124 pyexmars-1.0.9/pyexmars/
+-rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.9/pyexmars/__init__.py
+-rw-rw-rw-   0        0        0     6317 2024-05-27 11:17:07.000000 pyexmars-1.0.9/pyexmars/pyexmars.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:19:41.191859 pyexmars-1.0.9/pyexmars.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-27 11:19:41.000000 pyexmars-1.0.9/pyexmars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-27 11:19:41.000000 pyexmars-1.0.9/pyexmars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:19:41.000000 pyexmars-1.0.9/pyexmars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 11:19:41.000000 pyexmars-1.0.9/pyexmars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:19:41.194340 pyexmars-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      260 2024-05-27 11:19:14.000000 pyexmars-1.0.9/setup.py
```

