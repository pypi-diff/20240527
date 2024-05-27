# Comparing `tmp/telethon-client-0.0.2.tar.gz` & `tmp/telethon-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telethon-client-0.0.2.tar", last modified: Mon May 27 11:22:15 2024, max compression
+gzip compressed data, was "telethon-client-0.0.3.tar", last modified: Mon May 27 11:27:49 2024, max compression
```

## Comparing `telethon-client-0.0.2.tar` & `telethon-client-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 11:22:15.429394 telethon-client-0.0.2/
--rw-rw-rw-   0        0        0      408 2024-05-27 11:22:15.429394 telethon-client-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 11:22:15.414675 telethon-client-0.0.2/TeleClient/
--rw-rw-rw-   0        0        0       29 2024-05-27 11:18:59.000000 telethon-client-0.0.2/TeleClient/__init__.py
--rw-rw-rw-   0        0        0     1757 2024-05-27 11:19:48.000000 telethon-client-0.0.2/TeleClient/client.py
--rw-rw-rw-   0        0        0       35 2024-05-27 11:19:43.000000 telethon-client-0.0.2/TeleClient/env.py
--rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 11:22:15.429394 telethon-client-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      626 2024-05-27 11:21:52.000000 telethon-client-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 11:22:15.428394 telethon-client-0.0.2/telethon_client.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-27 11:22:15.000000 telethon-client-0.0.2/telethon_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-05-27 11:22:15.000000 telethon-client-0.0.2/telethon_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 11:22:15.000000 telethon-client-0.0.2/telethon_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 11:22:15.000000 telethon-client-0.0.2/telethon_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 11:22:15.000000 telethon-client-0.0.2/telethon_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 11:27:49.259638 telethon-client-0.0.3/
+-rw-rw-rw-   0        0        0      408 2024-05-27 11:27:49.259638 telethon-client-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 11:27:49.244883 telethon-client-0.0.3/TeleClient/
+-rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.3/TeleClient/__init__.py
+-rw-rw-rw-   0        0        0     1757 2024-05-27 11:19:48.000000 telethon-client-0.0.3/TeleClient/client.py
+-rw-rw-rw-   0        0        0       35 2024-05-27 11:19:43.000000 telethon-client-0.0.3/TeleClient/env.py
+-rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:27:49.259638 telethon-client-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-05-27 11:27:28.000000 telethon-client-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:27:49.258633 telethon-client-0.0.3/telethon_client.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-27 11:27:49.000000 telethon-client-0.0.3/telethon_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-05-27 11:27:49.000000 telethon-client-0.0.3/telethon_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:27:49.000000 telethon-client-0.0.3/telethon_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 11:27:49.000000 telethon-client-0.0.3/telethon_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 11:27:49.000000 telethon-client-0.0.3/telethon_client.egg-info/top_level.txt
```

### Comparing `telethon-client-0.0.2/TeleClient/client.py` & `telethon-client-0.0.3/TeleClient/client.py`

 * *Files identical despite different names*

### Comparing `telethon-client-0.0.2/setup.py` & `telethon-client-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "telethon-client",
-    version = "0.0.2",
+    version = "0.0.3",
     packages = find_packages(),
     install_requires = ["Telethon>=1.35.0"],
     author= " LEGENDX",
     author_email = "legendxcoder@gmail.com",
     description = "Custom Telethon Client for My Usage",
     long_description = open('README.md').read(),
     long_description_content_type = "text/markdown",
```

