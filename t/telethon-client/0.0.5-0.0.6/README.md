# Comparing `tmp/telethon-client-0.0.5.tar.gz` & `tmp/telethon-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telethon-client-0.0.5.tar", last modified: Mon May 27 17:24:00 2024, max compression
+gzip compressed data, was "telethon-client-0.0.6.tar", last modified: Mon May 27 17:33:45 2024, max compression
```

## Comparing `telethon-client-0.0.5.tar` & `telethon-client-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 17:24:00.815065 telethon-client-0.0.5/
--rw-rw-rw-   0        0        0      408 2024-05-27 17:24:00.814034 telethon-client-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 17:24:00.799556 telethon-client-0.0.5/TeleClient/
--rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.5/TeleClient/__init__.py
--rw-rw-rw-   0        0        0     1741 2024-05-27 17:20:49.000000 telethon-client-0.0.5/TeleClient/client.py
--rw-rw-rw-   0        0        0       67 2024-05-27 17:09:00.000000 telethon-client-0.0.5/TeleClient/env.py
--rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.0.5/TeleClient/errors.py
--rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 17:24:00.815065 telethon-client-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      626 2024-05-27 17:23:28.000000 telethon-client-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 17:24:00.812847 telethon-client-0.0.5/telethon_client.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-27 17:24:00.000000 telethon-client-0.0.5/telethon_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-27 17:24:00.000000 telethon-client-0.0.5/telethon_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 17:24:00.000000 telethon-client-0.0.5/telethon_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 17:24:00.000000 telethon-client-0.0.5/telethon_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 17:24:00.000000 telethon-client-0.0.5/telethon_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 17:33:45.305722 telethon-client-0.0.6/
+-rw-rw-rw-   0        0        0      408 2024-05-27 17:33:45.304704 telethon-client-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 17:33:45.290455 telethon-client-0.0.6/TeleClient/
+-rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.6/TeleClient/__init__.py
+-rw-rw-rw-   0        0        0     1742 2024-05-27 17:32:37.000000 telethon-client-0.0.6/TeleClient/client.py
+-rw-rw-rw-   0        0        0       67 2024-05-27 17:09:00.000000 telethon-client-0.0.6/TeleClient/env.py
+-rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.0.6/TeleClient/errors.py
+-rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 17:33:45.305722 telethon-client-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-05-27 17:33:07.000000 telethon-client-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:33:45.303760 telethon-client-0.0.6/telethon_client.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/top_level.txt
```

### Comparing `telethon-client-0.0.5/TeleClient/client.py` & `telethon-client-0.0.6/TeleClient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from telethon import TelegramClient
 from telethon.tl.functions.channels import GetFullChannelRequest
-from env import OWNERS, SUDO_USERS
+from .env import OWNERS, SUDO_USERS
 
 class MyClient(TelegramClient):
     def __init__(self, session, api_id, api_hash):
         super().__init__(session, api_id, api_hash)
         self.me = None
 
     async def getMe(self):
```

### Comparing `telethon-client-0.0.5/setup.py` & `telethon-client-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "telethon-client",
-    version = "0.0.5",
+    version = "0.0.6",
     packages = find_packages(),
     install_requires = ["Telethon>=1.35.0"],
     author= " LEGENDX",
     author_email = "legendxcoder@gmail.com",
     description = "Custom Telethon Client for My Usage",
     long_description = open('README.md').read(),
     long_description_content_type = "text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.7',
 )
```

