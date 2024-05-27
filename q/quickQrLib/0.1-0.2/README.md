# Comparing `tmp/quickQrLib-0.1.tar.gz` & `tmp/quickQrLib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickQrLib-0.1.tar", last modified: Mon May 27 14:42:42 2024, max compression
+gzip compressed data, was "quickQrLib-0.2.tar", last modified: Mon May 27 15:47:08 2024, max compression
```

## Comparing `quickQrLib-0.1.tar` & `quickQrLib-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:42.090212 quickQrLib-0.1/
--rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.1/LICENSE
--rw-rw-rw-   0        0        0       78 2024-05-27 14:42:42.084627 quickQrLib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       35 2024-05-27 14:28:22.000000 quickQrLib-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:42.009831 quickQrLib-0.1/quickQrLib/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.1/quickQrLib/__init__.py
--rw-rw-rw-   0        0        0       52 2024-05-27 14:37:44.000000 quickQrLib-0.1/quickQrLib/test.py
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:42.082625 quickQrLib-0.1/quickQrLib.egg-info/
--rw-rw-rw-   0        0        0       78 2024-05-27 14:42:41.000000 quickQrLib-0.1/quickQrLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-05-27 14:42:41.000000 quickQrLib-0.1/quickQrLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 14:42:41.000000 quickQrLib-0.1/quickQrLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 14:42:41.000000 quickQrLib-0.1/quickQrLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 14:42:42.090212 quickQrLib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      115 2024-05-27 14:38:37.000000 quickQrLib-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 15:47:08.492067 quickQrLib-0.2/
+-rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2/LICENSE
+-rw-rw-rw-   0        0        0       78 2024-05-27 15:47:08.490211 quickQrLib-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 15:47:08.424342 quickQrLib-0.2/quickQrLib/
+-rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2/quickQrLib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 15:47:08.488694 quickQrLib-0.2/quickQrLib.egg-info/
+-rw-rw-rw-   0        0        0       78 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 15:47:08.492067 quickQrLib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      217 2024-05-27 15:46:05.000000 quickQrLib-0.2/setup.py
```

### Comparing `quickQrLib-0.1/LICENSE` & `quickQrLib-0.2/LICENSE`

 * *Files identical despite different names*

