# Comparing `tmp/telethon-client-0.0.6.tar.gz` & `tmp/telethon-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telethon-client-0.0.6.tar", last modified: Mon May 27 17:33:45 2024, max compression
+gzip compressed data, was "telethon-client-0.0.7.tar", last modified: Mon May 27 17:51:29 2024, max compression
```

## Comparing `telethon-client-0.0.6.tar` & `telethon-client-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 17:33:45.305722 telethon-client-0.0.6/
--rw-rw-rw-   0        0        0      408 2024-05-27 17:33:45.304704 telethon-client-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 17:33:45.290455 telethon-client-0.0.6/TeleClient/
--rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.6/TeleClient/__init__.py
--rw-rw-rw-   0        0        0     1742 2024-05-27 17:32:37.000000 telethon-client-0.0.6/TeleClient/client.py
--rw-rw-rw-   0        0        0       67 2024-05-27 17:09:00.000000 telethon-client-0.0.6/TeleClient/env.py
--rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.0.6/TeleClient/errors.py
--rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 17:33:45.305722 telethon-client-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      626 2024-05-27 17:33:07.000000 telethon-client-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 17:33:45.303760 telethon-client-0.0.6/telethon_client.egg-info/
--rw-rw-rw-   0        0        0      408 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 17:33:45.000000 telethon-client-0.0.6/telethon_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 17:51:29.538312 telethon-client-0.0.7/
+-rw-rw-rw-   0        0        0      408 2024-05-27 17:51:29.537303 telethon-client-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-27 11:03:45.000000 telethon-client-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 17:51:29.520061 telethon-client-0.0.7/TeleClient/
+-rw-rw-rw-   0        0        0       30 2024-05-27 11:27:04.000000 telethon-client-0.0.7/TeleClient/__init__.py
+-rw-rw-rw-   0        0        0     1769 2024-05-27 17:50:52.000000 telethon-client-0.0.7/TeleClient/client.py
+-rw-rw-rw-   0        0        0      101 2024-05-27 17:48:31.000000 telethon-client-0.0.7/TeleClient/env.py
+-rw-rw-rw-   0        0        0       29 2024-05-27 11:34:39.000000 telethon-client-0.0.7/TeleClient/errors.py
+-rw-rw-rw-   0        0        0       97 2024-05-27 11:08:09.000000 telethon-client-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 17:51:29.538312 telethon-client-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      626 2024-05-27 17:51:05.000000 telethon-client-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 17:51:29.534899 telethon-client-0.0.7/telethon_client.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 17:51:29.000000 telethon-client-0.0.7/telethon_client.egg-info/top_level.txt
```

### Comparing `telethon-client-0.0.6/TeleClient/client.py` & `telethon-client-0.0.7/TeleClient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             return True
         else:
             return False
 
     async def checkSudo(self, event):
         if event.sender_id in OWNERS:
             return True
+        print(SUDO_USERS)
         if event.sender_id in SUDO_USERS:
             return True
         else:
             await event.respond('You are not a sudo user!')
             return False        
 
     def checkOwner(self, event):
```

### Comparing `telethon-client-0.0.6/setup.py` & `telethon-client-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "telethon-client",
-    version = "0.0.6",
+    version = "0.0.7",
     packages = find_packages(),
     install_requires = ["Telethon>=1.35.0"],
     author= " LEGENDX",
     author_email = "legendxcoder@gmail.com",
     description = "Custom Telethon Client for My Usage",
     long_description = open('README.md').read(),
     long_description_content_type = "text/markdown",
```

