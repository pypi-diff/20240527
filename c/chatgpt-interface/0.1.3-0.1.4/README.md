# Comparing `tmp/chatgpt_interface-0.1.3.tar.gz` & `tmp/chatgpt_interface-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_interface-0.1.3.tar", last modified: Mon May 27 17:42:12 2024, max compression
+gzip compressed data, was "chatgpt_interface-0.1.4.tar", last modified: Mon May 27 17:50:43 2024, max compression
```

## Comparing `chatgpt_interface-0.1.3.tar` & `chatgpt_interface-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 17:42:12.632778 chatgpt_interface-0.1.3/
--rw-rw-rw-   0        0        0      955 2024-05-27 17:42:12.632778 chatgpt_interface-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-05-24 00:46:56.000000 chatgpt_interface-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 17:42:12.570282 chatgpt_interface-0.1.3/chatgpt_interface/
--rw-rw-rw-   0        0        0       62 2024-05-27 12:09:43.000000 chatgpt_interface-0.1.3/chatgpt_interface/__init__.py
--rw-rw-rw-   0        0        0     4852 2024-05-27 17:00:36.000000 chatgpt_interface-0.1.3/chatgpt_interface/chatgpt_interface.py
-drwxrwxrwx   0        0        0        0 2024-05-27 17:42:12.632778 chatgpt_interface-0.1.3/chatgpt_interface.egg-info/
--rw-rw-rw-   0        0        0      955 2024-05-27 17:42:12.000000 chatgpt_interface-0.1.3/chatgpt_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-05-27 17:42:12.000000 chatgpt_interface-0.1.3/chatgpt_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 17:42:12.000000 chatgpt_interface-0.1.3/chatgpt_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-27 17:42:12.000000 chatgpt_interface-0.1.3/chatgpt_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-27 17:42:12.000000 chatgpt_interface-0.1.3/chatgpt_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 17:42:12.632778 chatgpt_interface-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      696 2024-05-27 17:41:15.000000 chatgpt_interface-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:50:43.188382 chatgpt_interface-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-27 17:50:43.188382 chatgpt_interface-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-27 17:50:34.000000 chatgpt_interface-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:50:43.188382 chatgpt_interface-0.1.4/chatgpt_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 17:50:34.000000 chatgpt_interface-0.1.4/chatgpt_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-27 17:50:34.000000 chatgpt_interface-0.1.4/chatgpt_interface/chatgpt_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:50:43.188382 chatgpt_interface-0.1.4/chatgpt_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-27 17:50:43.000000 chatgpt_interface-0.1.4/chatgpt_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-27 17:50:43.000000 chatgpt_interface-0.1.4/chatgpt_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:50:43.000000 chatgpt_interface-0.1.4/chatgpt_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 17:50:43.000000 chatgpt_interface-0.1.4/chatgpt_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 17:50:43.000000 chatgpt_interface-0.1.4/chatgpt_interface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:50:43.188382 chatgpt_interface-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-27 17:50:34.000000 chatgpt_interface-0.1.4/setup.py
```

### Comparing `chatgpt_interface-0.1.3/chatgpt_interface/chatgpt_interface.py` & `chatgpt_interface-0.1.4/chatgpt_interface/chatgpt_interface.py`

 * *Files identical despite different names*

### Comparing `chatgpt_interface-0.1.3/setup.py` & `chatgpt_interface-0.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='chatgpt_interface',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
-        'selenium',
-        'webdriver-manager',
+        'selenium>=3.141.0',
+        'webdriver-manager>=3.4.2',
     ],
+    python_requires='>=3.6',
     author='SpicaNet',
     author_email='dev@spicanet.net',
     description='A Python interface for interacting with ChatGPT via web interface using Selenium',
-    long_description=open('README.md').read(),
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/spicanet/ChatGPTInterface',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+    project_urls={
+        'Bug Tracker': 'https://github.com/spicanet/ChatGPTInterface/issues',
+        'Source': 'https://github.com/spicanet/ChatGPTInterface',
+    },
 )
```

