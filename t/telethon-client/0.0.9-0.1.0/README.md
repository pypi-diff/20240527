# Comparing `tmp/telethon-client-0.0.9.tar.gz` & `tmp/telethon-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telethon-client-0.0.9.tar", last modified: Mon May 27 18:06:28 2024, max compression
+gzip compressed data, was "telethon-client-0.1.0.tar", last modified: Mon May 27 18:28:26 2024, max compression
```

## Comparing `telethon-client-0.0.9.tar` & `telethon-client-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 18:06:28.362896 telethon-client-0.0.9/
--rw-rw-rw-   0        0        0      408 2024-05-27 18:06:28.361889 telethon-client-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 18:06:28.341190 telethon-client-0.0.9/TeleClient/
--rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.9/TeleClient/__init__.py
--rw-rw-rw-   0        0        0     1833 2024-05-27 18:05:35.000000 telethon-client-0.0.9/TeleClient/client.py
--rw-rw-rw-   0        0        0       98 2024-05-27 17:54:19.000000 telethon-client-0.0.9/TeleClient/env.py
--rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.0.9/TeleClient/errors.py
--rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 18:06:28.362896 telethon-client-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      733 2024-05-27 18:05:52.000000 telethon-client-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 18:06:28.360432 telethon-client-0.0.9/telethon_client.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-27 18:06:28.000000 telethon-client-0.0.9/telethon_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-27 18:06:28.000000 telethon-client-0.0.9/telethon_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 18:06:28.000000 telethon-client-0.0.9/telethon_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 18:06:28.000000 telethon-client-0.0.9/telethon_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 18:06:28.000000 telethon-client-0.0.9/telethon_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 18:28:26.889655 telethon-client-0.1.0/
+-rw-rw-rw-   0        0        0      408 2024-05-27 18:28:26.888652 telethon-client-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 18:28:26.874339 telethon-client-0.1.0/TeleClient/
+-rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.1.0/TeleClient/__init__.py
+-rw-rw-rw-   0        0        0     1447 2024-05-27 18:27:10.000000 telethon-client-0.1.0/TeleClient/client.py
+-rw-rw-rw-   0        0        0       59 2024-05-27 18:26:29.000000 telethon-client-0.1.0/TeleClient/env.py
+-rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.1.0/TeleClient/errors.py
+-rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:28:26.889655 telethon-client-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-27 18:27:39.000000 telethon-client-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:28:26.887651 telethon-client-0.1.0/telethon_client.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-27 18:28:26.000000 telethon-client-0.1.0/telethon_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-27 18:28:26.000000 telethon-client-0.1.0/telethon_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:28:26.000000 telethon-client-0.1.0/telethon_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 18:28:26.000000 telethon-client-0.1.0/telethon_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 18:28:26.000000 telethon-client-0.1.0/telethon_client.egg-info/top_level.txt
```

### Comparing `telethon-client-0.0.9/TeleClient/client.py` & `telethon-client-0.1.0/TeleClient/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from telethon import TelegramClient
 from telethon.tl.functions.channels import GetFullChannelRequest
-from .env import OWNERS, SUDO_USERS
+from .env import OWNERS
 
 class MyClient(TelegramClient):
     def __init__(self, session, api_id, api_hash):
         super().__init__(session, api_id, api_hash)
         self.me = None
 
     async def getMe(self):
@@ -32,24 +32,13 @@
     async def checkCancel(self, event):
         if event.text == "/cancel":
             await event.respond("Cancelled The Command.")
             return True
         else:
             return False
 
-    async def checkSudo(self, event):
-        if event.sender_id in OWNERS:
-            return True
-        SUDO_USERS.update(SUDO_USERS)
-        print("inside client -", SUDO_USERS)
-        if event.sender_id in list(SUDO_USERS):
-            return True
-        else:
-            await event.respond('You are not a sudo user!')
-            return False        
-
     def checkOwner(self, event):
         if event.sender_id in OWNERS:
             return True
         else:
             return False
```

### Comparing `telethon-client-0.0.9/setup.py` & `telethon-client-0.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
-import os, shutil
+import shutil
 shutil.rmtree('build')
 shutil.rmtree('dist')
 shutil.rmtree('Telethon_Client.egg-info')
 setup(
     name = "telethon-client",
-    version = "0.0.9",
+    version = "0.1.0",
     packages = find_packages(),
     install_requires = ["Telethon>=1.35.0"],
     author= " LEGENDX",
     author_email = "legendxcoder@gmail.com",
     description = "Custom Telethon Client for My Usage",
     long_description = open('README.md').read(),
     long_description_content_type = "text/markdown",
```

