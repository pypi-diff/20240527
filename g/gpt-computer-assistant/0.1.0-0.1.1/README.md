# Comparing `tmp/gpt_computer_assistant-0.1.0.tar.gz` & `tmp/gpt_computer_assistant-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_computer_assistant-0.1.0.tar", last modified: Mon May 27 11:50:53 2024, max compression
+gzip compressed data, was "gpt_computer_assistant-0.1.1.tar", last modified: Mon May 27 12:13:04 2024, max compression
```

## Comparing `gpt_computer_assistant-0.1.0.tar` & `gpt_computer_assistant-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.860532 gpt_computer_assistant-0.1.0/gpt_computer_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/background.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/proccess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/gpt_computer_assistant/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/audio/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/audio/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/gpt_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/gpt_computer_assistant/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/gui/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/gui/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/gpt_computer_assistant/screen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/screen/shot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/gpt_computer_assistant/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant/utils/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:50:53.860532 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-27 11:50:53.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-27 11:50:53.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:50:53.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 11:50:53.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:50:53.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 11:50:53.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 11:50:53.000000 gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:50:53.864532 gpt_computer_assistant-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-27 11:50:42.000000 gpt_computer_assistant-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.178418 gpt_computer_assistant-0.1.1/gpt_computer_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/proccess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/gpt_computer_assistant/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/audio/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/audio/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/gpt_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/gpt_computer_assistant/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/gui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/gui/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/gpt_computer_assistant/screen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/screen/shot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/gpt_computer_assistant/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant/utils/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-27 12:13:03.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-27 12:13:04.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:13:03.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 12:13:03.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:13:03.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 12:13:03.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 12:13:03.000000 gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:13:04.182419 gpt_computer_assistant-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-27 12:12:52.000000 gpt_computer_assistant-0.1.1/setup.py
```

### Comparing `gpt_computer_assistant-0.1.0/LICENSE` & `gpt_computer_assistant-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/PKG-INFO` & `gpt_computer_assistant-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_computer_assistant
-Version: 0.1.0
+Version: 0.1.1
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
```

### Comparing `gpt_computer_assistant-0.1.0/README.md` & `gpt_computer_assistant-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/agent.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/agent.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/assistant.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/background.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/background.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/agent/proccess.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/agent/proccess.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/audio/record.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/audio/record.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/audio/tts.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/audio/tts.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/gpt_assistant.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/gpt_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/gui/button.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/gui/button.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant/utils/db.py` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant/utils/db.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/PKG-INFO` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-computer-assistant
-Version: 0.1.0
+Version: 0.1.1
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
```

### Comparing `gpt_computer_assistant-0.1.0/gpt_computer_assistant.egg-info/SOURCES.txt` & `gpt_computer_assistant-0.1.1/gpt_computer_assistant.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
+./requirements.txt
 gpt_computer_assistant/__init__.py
 gpt_computer_assistant/gpt_assistant.py
 gpt_computer_assistant/llm.py
 gpt_computer_assistant.egg-info/PKG-INFO
 gpt_computer_assistant.egg-info/SOURCES.txt
 gpt_computer_assistant.egg-info/dependency_links.txt
 gpt_computer_assistant.egg-info/entry_points.txt
```

### Comparing `gpt_computer_assistant-0.1.0/setup.py` & `gpt_computer_assistant-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="gpt_computer_assistant",
-    version="0.1.0",
+    version="0.1.1",
     description="""GPT""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/onuratakan/gpt-computer-assistant",
     author="Onur Atakan ULUSOY",
     author_email="atadogan06@gmail.com",
     license="MIT",
```

