# Comparing `tmp/telethon-client-0.0.7.tar.gz` & `tmp/telethon-client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telethon-client-0.0.7.tar", last modified: Mon May 27 17:51:29 2024, max compression
+gzip compressed data, was "telethon-client-0.0.8.tar", last modified: Mon May 27 17:54:45 2024, max compression
```

## Comparing `telethon-client-0.0.7.tar` & `telethon-client-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 17:51:29.538312 telethon-client-0.0.7/
--rw-rw-rw-   0        0        0      408 2024-05-27 17:51:29.537303 telethon-client-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 17:51:29.520061 telethon-client-0.0.7/TeleClient/
--rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.7/TeleClient/__init__.py
--rw-rw-rw-   0        0        0     1769 2024-05-27 17:50:52.000000 telethon-client-0.0.7/TeleClient/client.py
--rw-rw-rw-   0        0        0      101 2024-05-27 17:48:31.000000 telethon-client-0.0.7/TeleClient/env.py
--rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.0.7/TeleClient/errors.py
--rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 17:51:29.538312 telethon-client-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      626 2024-05-27 17:51:05.000000 telethon-client-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 17:51:29.534899 telethon-client-0.0.7/telethon_client.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 17:54:45.307614 telethon-client-0.0.8/
+-rw-rw-rw-   0        0        0      408 2024-05-27 17:54:45.306607 telethon-client-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 17:54:45.292192 telethon-client-0.0.8/TeleClient/
+-rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.8/TeleClient/__init__.py
+-rw-rw-rw-   0        0        0     1769 2024-05-27 17:50:52.000000 telethon-client-0.0.8/TeleClient/client.py
+-rw-rw-rw-   0        0        0       98 2024-05-27 17:54:19.000000 telethon-client-0.0.8/TeleClient/env.py
+-rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.0.8/TeleClient/errors.py
+-rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 17:54:45.307614 telethon-client-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-05-27 17:54:22.000000 telethon-client-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:54:45.305137 telethon-client-0.0.8/telethon_client.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-27 17:54:45.000000 telethon-client-0.0.8/telethon_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-27 17:54:45.000000 telethon-client-0.0.8/telethon_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 17:54:45.000000 telethon-client-0.0.8/telethon_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 17:54:45.000000 telethon-client-0.0.8/telethon_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 17:54:45.000000 telethon-client-0.0.8/telethon_client.egg-info/top_level.txt
```

### Comparing `telethon-client-0.0.7/TeleClient/client.py` & `telethon-client-0.0.8/TeleClient/client.py`

 * *Files identical despite different names*

### Comparing `telethon-client-0.0.7/setup.py` & `telethon-client-0.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "telethon-client",
-    version = "0.0.7",
+    version = "0.0.8",
     packages = find_packages(),
     install_requires = ["Telethon>=1.35.0"],
     author= " LEGENDX",
     author_email = "legendxcoder@gmail.com",
     description = "Custom Telethon Client for My Usage",
     long_description = open('README.md').read(),
     long_description_content_type = "text/markdown",
```

