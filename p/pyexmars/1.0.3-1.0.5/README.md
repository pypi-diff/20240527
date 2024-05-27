# Comparing `tmp/pyexmars-1.0.3.tar.gz` & `tmp/pyexmars-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyexmars-1.0.3.tar", last modified: Mon May 27 08:59:09 2024, max compression
+gzip compressed data, was "pyexmars-1.0.5.tar", last modified: Mon May 27 09:11:26 2024, max compression
```

## Comparing `pyexmars-1.0.3.tar` & `pyexmars-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 08:59:09.348026 pyexmars-1.0.3/
--rw-rw-rw-   0        0        0       55 2024-05-27 08:59:09.347030 pyexmars-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 08:59:09.316024 pyexmars-1.0.3/pyexmars/
--rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.3/pyexmars/__init__.py
--rw-rw-rw-   0        0        0      683 2024-05-27 08:57:25.000000 pyexmars-1.0.3/pyexmars/pyexmars.py
-drwxrwxrwx   0        0        0        0 2024-05-27 08:59:09.345018 pyexmars-1.0.3/pyexmars.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 08:59:09.000000 pyexmars-1.0.3/pyexmars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 08:59:09.348026 pyexmars-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      261 2024-05-27 08:58:57.000000 pyexmars-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 09:11:26.446076 pyexmars-1.0.5/
+-rw-rw-rw-   0        0        0       55 2024-05-27 09:11:26.445079 pyexmars-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 09:11:26.427282 pyexmars-1.0.5/pyexmars/
+-rw-rw-rw-   0        0        0        0 2024-05-27 08:43:52.000000 pyexmars-1.0.5/pyexmars/__init__.py
+-rw-rw-rw-   0        0        0     1006 2024-05-27 09:08:59.000000 pyexmars-1.0.5/pyexmars/pyexmars.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-05-27 09:11:26.444080 pyexmars-1.0.5/pyexmars.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-27 09:11:26.000000 pyexmars-1.0.5/pyexmars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-27 09:11:26.000000 pyexmars-1.0.5/pyexmars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 09:11:26.000000 pyexmars-1.0.5/pyexmars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 09:11:26.000000 pyexmars-1.0.5/pyexmars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 09:11:26.446076 pyexmars-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      261 2024-05-27 09:11:01.000000 pyexmars-1.0.5/setup.py
```

