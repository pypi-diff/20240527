# Comparing `tmp/quickQrLib-0.2.2.tar.gz` & `tmp/quickQrLib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickQrLib-0.2.2.tar", last modified: Mon May 27 16:04:43 2024, max compression
+gzip compressed data, was "quickQrLib-0.2.3.tar", last modified: Mon May 27 16:06:03 2024, max compression
```

## Comparing `quickQrLib-0.2.2.tar` & `quickQrLib-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 16:04:43.210474 quickQrLib-0.2.2/
--rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       80 2024-05-27 16:04:43.210474 quickQrLib-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 16:04:43.174731 quickQrLib-0.2.2/quickQrLib/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.2/quickQrLib/__init__.py
--rw-rw-rw-   0        0        0      893 2024-05-27 15:54:12.000000 quickQrLib-0.2.2/quickQrLib/qr_auth_util.py
--rw-rw-rw-   0        0        0      104 2024-05-27 16:01:43.000000 quickQrLib-0.2.2/quickQrLib/test_util.py
--rw-rw-rw-   0        0        0        0 2024-05-27 15:54:26.000000 quickQrLib-0.2.2/quickQrLib/time_util.py
-drwxrwxrwx   0        0        0        0 2024-05-27 16:04:43.198495 quickQrLib-0.2.2/quickQrLib.egg-info/
--rw-rw-rw-   0        0        0       80 2024-05-27 16:04:43.000000 quickQrLib-0.2.2/quickQrLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-05-27 16:04:43.000000 quickQrLib-0.2.2/quickQrLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 16:04:43.000000 quickQrLib-0.2.2/quickQrLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-27 16:04:43.000000 quickQrLib-0.2.2/quickQrLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 16:04:43.000000 quickQrLib-0.2.2/quickQrLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 16:04:43.210474 quickQrLib-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      272 2024-05-27 16:04:40.000000 quickQrLib-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:06:03.153874 quickQrLib-0.2.3/
+-rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       80 2024-05-27 16:06:03.150865 quickQrLib-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 16:06:02.894496 quickQrLib-0.2.3/quickQrLib/
+-rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.3/quickQrLib/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-05-27 15:54:12.000000 quickQrLib-0.2.3/quickQrLib/qr_auth_util.py
+-rw-rw-rw-   0        0        0      104 2024-05-27 16:01:43.000000 quickQrLib-0.2.3/quickQrLib/test_util.py
+-rw-rw-rw-   0        0        0        0 2024-05-27 15:54:26.000000 quickQrLib-0.2.3/quickQrLib/time_util.py
+drwxrwxrwx   0        0        0        0 2024-05-27 16:06:03.144201 quickQrLib-0.2.3/quickQrLib.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 16:06:02.000000 quickQrLib-0.2.3/quickQrLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 16:06:03.154828 quickQrLib-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      272 2024-05-27 16:05:56.000000 quickQrLib-0.2.3/setup.py
```

### Comparing `quickQrLib-0.2.2/LICENSE` & `quickQrLib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickQrLib-0.2.2/quickQrLib/qr_auth_util.py` & `quickQrLib-0.2.3/quickQrLib/qr_auth_util.py`

 * *Files identical despite different names*

