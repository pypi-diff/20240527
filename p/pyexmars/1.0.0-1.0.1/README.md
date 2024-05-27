# Comparing `tmp/pyexmars-1.0.0.tar.gz` & `tmp/pyexmars-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyexmars-1.0.0.tar", last modified: Mon May 27 07:50:44 2024, max compression
+gzip compressed data, was "pyexmars-1.0.1.tar", last modified: Mon May 27 08:36:35 2024, max compression
```

## Comparing `pyexmars-1.0.0.tar` & `pyexmars-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 07:50:44.041524 pyexmars-1.0.0/
--rw-rw-rw-   0        0        0       55 2024-05-27 07:50:44.040512 pyexmars-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 07:50:44.039134 pyexmars-1.0.0/pyexmars.egg-info/
--rw-rw-rw-   0        0        0       55 2024-05-27 07:50:43.000000 pyexmars-1.0.0/pyexmars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2024-05-27 07:50:43.000000 pyexmars-1.0.0/pyexmars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 07:50:43.000000 pyexmars-1.0.0/pyexmars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 07:50:43.000000 pyexmars-1.0.0/pyexmars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 07:50:44.041524 pyexmars-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      256 2024-05-27 07:48:45.000000 pyexmars-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 08:36:35.925475 pyexmars-1.0.1/
+-rw-rw-rw-   0        0        0       55 2024-05-27 08:36:35.924969 pyexmars-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 08:36:35.922488 pyexmars-1.0.1/pyexmars.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 08:36:35.000000 pyexmars-1.0.1/pyexmars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 08:36:35.925475 pyexmars-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      256 2024-05-27 08:36:11.000000 pyexmars-1.0.1/setup.py
```

