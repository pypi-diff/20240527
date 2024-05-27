# Comparing `tmp/chatgpt_interface-0.1.0.tar.gz` & `tmp/chatgpt_interface-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_interface-0.1.0.tar", last modified: Mon May 27 09:46:23 2024, max compression
+gzip compressed data, was "chatgpt_interface-0.1.2.tar", last modified: Mon May 27 11:43:18 2024, max compression
```

## Comparing `chatgpt_interface-0.1.0.tar` & `chatgpt_interface-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 09:46:23.859298 chatgpt_interface-0.1.0/
--rw-rw-rw-   0        0        0      956 2024-05-27 09:46:23.859298 chatgpt_interface-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-05-24 00:46:56.000000 chatgpt_interface-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 09:46:23.796804 chatgpt_interface-0.1.0/chatgpt_interface/
--rw-rw-rw-   0        0        0       62 2024-05-24 00:46:56.000000 chatgpt_interface-0.1.0/chatgpt_interface/__init__.py
--rw-rw-rw-   0        0        0     1184 2024-05-24 00:46:56.000000 chatgpt_interface-0.1.0/chatgpt_interface/chatgpt_interface.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:46:23.859298 chatgpt_interface-0.1.0/chatgpt_interface.egg-info/
--rw-rw-rw-   0        0        0      956 2024-05-27 09:46:23.000000 chatgpt_interface-0.1.0/chatgpt_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-27 09:46:23.000000 chatgpt_interface-0.1.0/chatgpt_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 09:46:23.000000 chatgpt_interface-0.1.0/chatgpt_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-27 09:46:23.000000 chatgpt_interface-0.1.0/chatgpt_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-27 09:46:23.000000 chatgpt_interface-0.1.0/chatgpt_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 09:46:23.859298 chatgpt_interface-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      697 2024-05-27 09:42:12.000000 chatgpt_interface-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-27 09:46:23.843681 chatgpt_interface-0.1.0/tests/
--rw-rw-rw-   0        0        0       52 2024-05-24 00:46:56.000000 chatgpt_interface-0.1.0/tests/test_chatgpt_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:43:18.174430 chatgpt_interface-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-27 11:43:18.174430 chatgpt_interface-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-27 11:43:08.000000 chatgpt_interface-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:43:18.170430 chatgpt_interface-0.1.2/chatgpt_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 11:43:08.000000 chatgpt_interface-0.1.2/chatgpt_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-27 11:43:08.000000 chatgpt_interface-0.1.2/chatgpt_interface/chatgpt_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:43:18.174430 chatgpt_interface-0.1.2/chatgpt_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-27 11:43:18.000000 chatgpt_interface-0.1.2/chatgpt_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 11:43:18.000000 chatgpt_interface-0.1.2/chatgpt_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:43:18.000000 chatgpt_interface-0.1.2/chatgpt_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 11:43:18.000000 chatgpt_interface-0.1.2/chatgpt_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 11:43:18.000000 chatgpt_interface-0.1.2/chatgpt_interface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:43:18.174430 chatgpt_interface-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-27 11:43:08.000000 chatgpt_interface-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:43:18.174430 chatgpt_interface-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 11:43:08.000000 chatgpt_interface-0.1.2/tests/test_chatgpt_interface.py
```

### Comparing `chatgpt_interface-0.1.0/PKG-INFO` & `chatgpt_interface-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: chatgpt_interface
-Version: 0.1.0
-Summary: A Python interface for interacting with ChatGPT via web interface using Selenium
-Home-page: https://github.com/spicanet/chatgpt_interface
-Author: SpicaNet
-Author-email: dev@spicanet.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: selenium
-Requires-Dist: webdriver-manager
-
-# ChatGPT Interface
-
-A Python interface for interacting with ChatGPT via web interface using Selenium.
-
-## Installation
-
-```
-pip install chatgpt_interface
-```
-
-## Usage
-
-```python
-from chatgpt_interface import ChatGPTInterface
-
-chatgpt = ChatGPTInterface()
-chatgpt.open_chat("URL_of_ChatGPT_Web_Interface")
-chatgpt.send_prompt("Hello, how are you?")
-response = chatgpt.get_response()
-print(response)
-chatgpt.close()
-```
+Metadata-Version: 2.1
+Name: chatgpt_interface
+Version: 0.1.2
+Summary: A Python interface for interacting with ChatGPT via web interface using Selenium
+Home-page: https://github.com/spicanet/ChatGPTInterface
+Author: SpicaNet
+Author-email: dev@spicanet.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Requires-Dist: selenium
+Requires-Dist: webdriver-manager
+
+# ChatGPT Interface
+
+A Python interface for interacting with ChatGPT via web interface using Selenium.
+
+## Installation
+
+```
+pip install chatgpt_interface
+```
+
+## Usage
+
+```python
+from chatgpt_interface import ChatGPTInterface
+
+chatgpt = ChatGPTInterface()
+chatgpt.open_chat("URL_of_ChatGPT_Web_Interface")
+chatgpt.send_prompt("Hello, how are you?")
+response = chatgpt.get_response()
+print(response)
+chatgpt.close()
+```
```

### Comparing `chatgpt_interface-0.1.0/chatgpt_interface/chatgpt_interface.py` & `chatgpt_interface-0.1.2/chatgpt_interface/chatgpt_interface.py`

 * *Files identical despite different names*

### Comparing `chatgpt_interface-0.1.0/chatgpt_interface.egg-info/PKG-INFO` & `chatgpt_interface-0.1.2/chatgpt_interface.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
-Name: chatgpt_interface
-Version: 0.1.0
-Summary: A Python interface for interacting with ChatGPT via web interface using Selenium
-Home-page: https://github.com/spicanet/chatgpt_interface
-Author: SpicaNet
-Author-email: dev@spicanet.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: selenium
-Requires-Dist: webdriver-manager
-
-# ChatGPT Interface
-
-A Python interface for interacting with ChatGPT via web interface using Selenium.
-
-## Installation
-
-```
-pip install chatgpt_interface
-```
-
-## Usage
-
-```python
-from chatgpt_interface import ChatGPTInterface
-
-chatgpt = ChatGPTInterface()
-chatgpt.open_chat("URL_of_ChatGPT_Web_Interface")
-chatgpt.send_prompt("Hello, how are you?")
-response = chatgpt.get_response()
-print(response)
-chatgpt.close()
-```
+Metadata-Version: 2.1
+Name: chatgpt_interface
+Version: 0.1.2
+Summary: A Python interface for interacting with ChatGPT via web interface using Selenium
+Home-page: https://github.com/spicanet/ChatGPTInterface
+Author: SpicaNet
+Author-email: dev@spicanet.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Requires-Dist: selenium
+Requires-Dist: webdriver-manager
+
+# ChatGPT Interface
+
+A Python interface for interacting with ChatGPT via web interface using Selenium.
+
+## Installation
+
+```
+pip install chatgpt_interface
+```
+
+## Usage
+
+```python
+from chatgpt_interface import ChatGPTInterface
+
+chatgpt = ChatGPTInterface()
+chatgpt.open_chat("URL_of_ChatGPT_Web_Interface")
+chatgpt.send_prompt("Hello, how are you?")
+response = chatgpt.get_response()
+print(response)
+chatgpt.close()
+```
```

### Comparing `chatgpt_interface-0.1.0/setup.py` & `chatgpt_interface-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chatgpt_interface',
-    version='0.1.0',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'selenium',
         'webdriver-manager',
     ],
     author='SpicaNet',
     author_email='dev@spicanet.net',
     description='A Python interface for interacting with ChatGPT via web interface using Selenium',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/spicanet/chatgpt_interface',
+    url='https://github.com/spicanet/ChatGPTInterface',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

