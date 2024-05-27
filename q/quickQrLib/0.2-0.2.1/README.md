# Comparing `tmp/quickQrLib-0.2.tar.gz` & `tmp/quickQrLib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickQrLib-0.2.tar", last modified: Mon May 27 15:47:08 2024, max compression
+gzip compressed data, was "quickQrLib-0.2.1.tar", last modified: Mon May 27 16:03:30 2024, max compression
```

## Comparing `quickQrLib-0.2.tar` & `quickQrLib-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 15:47:08.492067 quickQrLib-0.2/
--rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2/LICENSE
--rw-rw-rw-   0        0        0       78 2024-05-27 15:47:08.490211 quickQrLib-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 15:47:08.424342 quickQrLib-0.2/quickQrLib/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2/quickQrLib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 15:47:08.488694 quickQrLib-0.2/quickQrLib.egg-info/
--rw-rw-rw-   0        0        0       78 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 15:47:08.000000 quickQrLib-0.2/quickQrLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 15:47:08.492067 quickQrLib-0.2/setup.cfg
--rw-rw-rw-   0        0        0      217 2024-05-27 15:46:05.000000 quickQrLib-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:03:30.102751 quickQrLib-0.2.1/
+-rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       80 2024-05-27 16:03:30.098735 quickQrLib-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 16:03:30.013330 quickQrLib-0.2.1/quickQrLib/
+-rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.1/quickQrLib/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-05-27 15:54:12.000000 quickQrLib-0.2.1/quickQrLib/qr_auth_util.py
+-rw-rw-rw-   0        0        0      104 2024-05-27 16:01:43.000000 quickQrLib-0.2.1/quickQrLib/test_util.py
+-rw-rw-rw-   0        0        0        0 2024-05-27 15:54:26.000000 quickQrLib-0.2.1/quickQrLib/time_util.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:03:30.096618 quickQrLib-0.2.1/quickQrLib.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-05-27 16:03:29.000000 quickQrLib-0.2.1/quickQrLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-27 16:03:29.000000 quickQrLib-0.2.1/quickQrLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 16:03:29.000000 quickQrLib-0.2.1/quickQrLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-27 16:03:29.000000 quickQrLib-0.2.1/quickQrLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 16:03:29.000000 quickQrLib-0.2.1/quickQrLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 16:03:30.102751 quickQrLib-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      272 2024-05-27 16:03:26.000000 quickQrLib-0.2.1/setup.py
```

### Comparing `quickQrLib-0.2/LICENSE` & `quickQrLib-0.2.1/LICENSE`

 * *Files identical despite different names*

