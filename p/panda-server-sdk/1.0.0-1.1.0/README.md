# Comparing `tmp/panda_server_sdk-1.0.0.tar.gz` & `tmp/panda_server_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\panda_server_sdk-1.0.0.tar", last modified: Thu May 23 15:47:33 2024, max compression
+gzip compressed data, was "dist\panda_server_sdk-1.1.0.tar", last modified: Mon May 27 11:15:45 2024, max compression
```

## Comparing `panda_server_sdk-1.0.0.tar` & `panda_server_sdk-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/
--rw-rw-rw-   0        0        0      220 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       58 2024-05-19 09:52:05.000000 panda_server_sdk-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/panda_server_sdk/
--rw-rw-rw-   0        0        0     4978 2024-05-23 15:24:44.000000 panda_server_sdk-1.0.0/panda_server_sdk/__init__.py
--rw-rw-rw-   0        0        0      410 2024-05-23 08:11:27.000000 panda_server_sdk-1.0.0/panda_server_sdk/panda_server_sdk_keys.py
-drwxrwxrwx   0        0        0        0 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/panda_server_sdk.egg-info/
--rw-rw-rw-   0        0        0      220 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/panda_server_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/panda_server_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/panda_server_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/panda_server_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 15:47:33.000000 panda_server_sdk-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      255 2024-05-19 09:35:50.000000 panda_server_sdk-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/
+-rw-rw-rw-   0        0        0      220 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2024-05-19 09:52:05.000000 panda_server_sdk-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/panda_server_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-27 11:14:55.000000 panda_server_sdk-1.1.0/panda_server_sdk/__init__.py
+-rw-rw-rw-   0        0        0     4959 2024-05-27 11:14:55.000000 panda_server_sdk-1.1.0/panda_server_sdk/panda_server_sdk.py
+-rw-rw-rw-   0        0        0      410 2024-05-23 08:11:27.000000 panda_server_sdk-1.1.0/panda_server_sdk/panda_server_sdk_keys.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/panda_server_sdk.egg-info/
+-rw-rw-rw-   0        0        0      220 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/panda_server_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/panda_server_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/panda_server_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/panda_server_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:15:45.000000 panda_server_sdk-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      305 2024-05-27 11:15:36.000000 panda_server_sdk-1.1.0/setup.py
```

### Comparing `panda_server_sdk-1.0.0/panda_server_sdk/__init__.py` & `panda_server_sdk-1.1.0/panda_server_sdk/panda_server_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Python SDK external package
 """
 
 # Imports
 import os
-import subprocess
 import sys
 from dotenv import load_dotenv
 from panda_server_sdk.panda_server_sdk_keys import TestingPandaPythonSDKKEYS
 
 
 class TestingPandaPythonSDK(TestingPandaPythonSDKKEYS):
     """
```

