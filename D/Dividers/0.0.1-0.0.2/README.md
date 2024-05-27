# Comparing `tmp/dividers-0.0.1.tar.gz` & `tmp/dividers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dividers-0.0.1.tar", last modified: Sun May 26 23:26:57 2024, max compression
+gzip compressed data, was "dividers-0.0.2.tar", last modified: Sun May 26 23:45:22 2024, max compression
```

## Comparing `dividers-0.0.1.tar` & `dividers-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 23:26:57.655534 dividers-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-26 23:26:57.641031 dividers-0.0.1/Dividers/
--rw-rw-rw-   0        0        0       22 2024-05-26 23:26:47.000000 dividers-0.0.1/Dividers/__init__.py
--rw-rw-rw-   0        0        0       75 2024-05-26 22:52:58.000000 dividers-0.0.1/Dividers/div.py
-drwxrwxrwx   0        0        0        0 2024-05-26 23:26:57.654034 dividers-0.0.1/Dividers.egg-info/
--rw-rw-rw-   0        0        0      202 2024-05-26 23:26:57.000000 dividers-0.0.1/Dividers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-26 23:26:57.000000 dividers-0.0.1/Dividers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 23:26:57.000000 dividers-0.0.1/Dividers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-26 23:26:57.000000 dividers-0.0.1/Dividers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35802 2024-04-28 03:38:43.000000 dividers-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      202 2024-05-26 23:26:57.654534 dividers-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-29 02:12:58.000000 dividers-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 23:26:57.655534 dividers-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      377 2024-05-26 23:18:48.000000 dividers-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 23:26:57.653033 dividers-0.0.1/tests/
--rw-rw-rw-   0        0        0       48 2024-05-26 23:23:46.000000 dividers-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:45:22.394465 dividers-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-26 23:45:22.381728 dividers-0.0.2/Dividers/
+-rw-rw-rw-   0        0        0       22 2024-05-26 23:26:47.000000 dividers-0.0.2/Dividers/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-26 22:52:58.000000 dividers-0.0.2/Dividers/div.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:45:22.392464 dividers-0.0.2/Dividers.egg-info/
+-rw-rw-rw-   0        0        0      563 2024-05-26 23:45:22.000000 dividers-0.0.2/Dividers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-26 23:45:22.000000 dividers-0.0.2/Dividers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 23:45:22.000000 dividers-0.0.2/Dividers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 23:45:22.000000 dividers-0.0.2/Dividers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35802 2024-04-28 03:38:43.000000 dividers-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      563 2024-05-26 23:45:22.393465 dividers-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-29 02:12:58.000000 dividers-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 23:45:22.394465 dividers-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-05-26 23:43:14.000000 dividers-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 23:45:22.391464 dividers-0.0.2/tests/
+-rw-rw-rw-   0        0        0      186 2024-05-26 23:32:23.000000 dividers-0.0.2/tests/test.py
```

### Comparing `dividers-0.0.1/LICENSE` & `dividers-0.0.2/LICENSE`

 * *Files identical despite different names*

