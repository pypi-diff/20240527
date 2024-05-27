# Comparing `tmp/pyexmars-1.0.6.tar.gz` & `tmp/pyexmars-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyexmars-1.0.6.tar", last modified: Mon May 27 09:23:24 2024, max compression
+gzip compressed data, was "pyexmars-1.0.7.tar", last modified: Mon May 27 09:30:00 2024, max compression
```

## Comparing `pyexmars-1.0.6.tar` & `pyexmars-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 09:23:24.334752 pyexmars-1.0.6/
--rw-rw-rw-   0        0        0       55 2024-05-27 09:23:24.333740 pyexmars-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 09:23:24.311862 pyexmars-1.0.6/pyexmars/
--rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.6/pyexmars/__init__.py
--rw-rw-rw-   0        0        0      621 2024-05-27 09:22:28.000000 pyexmars-1.0.6/pyexmars/pyexmars.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-05-27 09:23:24.332248 pyexmars-1.0.6/pyexmars.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-27 09:23:24.000000 pyexmars-1.0.6/pyexmars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-05-27 09:23:24.000000 pyexmars-1.0.6/pyexmars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 09:23:24.000000 pyexmars-1.0.6/pyexmars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 09:23:24.000000 pyexmars-1.0.6/pyexmars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 09:23:24.335748 pyexmars-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      261 2024-05-27 09:23:17.000000 pyexmars-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:30:00.601238 pyexmars-1.0.7/
+-rw-rw-rw-   0        0        0       55 2024-05-27 09:30:00.601238 pyexmars-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 09:30:00.585137 pyexmars-1.0.7/pyexmars/
+-rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.7/pyexmars/__init__.py
+-rw-rw-rw-   0        0        0     1006 2024-05-27 09:28:54.000000 pyexmars-1.0.7/pyexmars/pyexmars.cpython-310.pyc
+-rw-rw-rw-   0        0        0      683 2024-05-27 09:27:47.000000 pyexmars-1.0.7/pyexmars/pyexmars.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:30:00.599729 pyexmars-1.0.7/pyexmars.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 09:30:00.000000 pyexmars-1.0.7/pyexmars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 09:30:00.601238 pyexmars-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      261 2024-05-27 09:29:54.000000 pyexmars-1.0.7/setup.py
```

