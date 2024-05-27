# Comparing `tmp/quickQrLib-0.2.22.tar.gz` & `tmp/quickQrLib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickQrLib-0.2.22.tar", last modified: Mon May 27 19:53:29 2024, max compression
+gzip compressed data, was "quickQrLib-0.2.3.tar", last modified: Mon May 27 16:06:03 2024, max compression
```

## Comparing `quickQrLib-0.2.22.tar` & `quickQrLib-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.644763 quickQrLib-0.2.22/
--rw-rw-rw-   0        0        0     1092 2024-05-27 14:41:13.000000 quickQrLib-0.2.22/LICENSE
--rw-rw-rw-   0        0        0       81 2024-05-27 19:53:29.641124 quickQrLib-0.2.22/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-27 15:15:15.000000 quickQrLib-0.2.22/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.534184 quickQrLib-0.2.22/quickQrLib/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.22/quickQrLib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.601617 quickQrLib-0.2.22/quickQrLib/auth_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.22/quickQrLib/auth_util/__init__.py
--rw-rw-rw-   0        0        0      893 2024-05-27 15:27:15.000000 quickQrLib-0.2.22/quickQrLib/auth_util/authenticate_jwt.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.609939 quickQrLib-0.2.22/quickQrLib/permissions_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.22/quickQrLib/permissions_util/__init__.py
--rw-rw-rw-   0        0        0     4264 2024-05-27 17:09:11.000000 quickQrLib-0.2.22/quickQrLib/permissions_util/permissions_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.617082 quickQrLib-0.2.22/quickQrLib/s3_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.22/quickQrLib/s3_util/__init__.py
--rw-rw-rw-   0        0        0     2790 2024-05-27 18:16:14.000000 quickQrLib-0.2.22/quickQrLib/s3_util/s3_storage_util.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.632634 quickQrLib-0.2.22/quickQrLib/test_folder_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.22/quickQrLib/test_folder_util/__init__.py
--rw-rw-rw-   0        0        0       33 2024-05-27 16:01:30.000000 quickQrLib-0.2.22/quickQrLib/test_folder_util/test.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.639112 quickQrLib-0.2.22/quickQrLib/time_util/
--rw-rw-rw-   0        0        0        0 2024-05-27 14:37:12.000000 quickQrLib-0.2.22/quickQrLib/time_util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:53:29.593227 quickQrLib-0.2.22/quickQrLib.egg-info/
--rw-rw-rw-   0        0        0       81 2024-05-27 19:53:29.000000 quickQrLib-0.2.22/quickQrLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-05-27 19:53:29.000000 quickQrLib-0.2.22/quickQrLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 19:53:29.000000 quickQrLib-0.2.22/quickQrLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-27 19:53:29.000000 quickQrLib-0.2.22/quickQrLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 19:53:29.000000 quickQrLib-0.2.22/quickQrLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 19:53:29.644763 quickQrLib-0.2.22/setup.cfg
--rw-rw-rw-   0        0        0      272 2024-05-27 19:53:28.000000 quickQrLib-0.2.22/setup.py
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

### Comparing `quickQrLib-0.2.22/LICENSE` & `quickQrLib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quickQrLib-0.2.22/quickQrLib/auth_util/authenticate_jwt.py` & `quickQrLib-0.2.3/quickQrLib/qr_auth_util.py`

 * *Files identical despite different names*

