# Comparing `tmp/telegram_gmail_bot-0.1.0.tar.gz` & `tmp/telegram_gmail_bot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_gmail_bot-0.1.0.tar", last modified: Mon May 27 03:42:38 2024, max compression
+gzip compressed data, was "telegram_gmail_bot-0.1.1.tar", last modified: Mon May 27 03:53:57 2024, max compression
```

## Comparing `telegram_gmail_bot-0.1.0.tar` & `telegram_gmail_bot-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:42:38.269458 telegram_gmail_bot-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 03:42:27.000000 telegram_gmail_bot-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 03:42:27.000000 telegram_gmail_bot-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-27 03:42:38.269458 telegram_gmail_bot-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 03:42:27.000000 telegram_gmail_bot-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 03:42:27.000000 telegram_gmail_bot-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 03:42:38.269458 telegram_gmail_bot-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-27 03:42:27.000000 telegram_gmail_bot-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:42:38.269458 telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-27 03:42:38.000000 telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 03:42:38.000000 telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 03:42:38.000000 telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 03:42:38.000000 telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 03:42:38.000000 telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 03:42:38.000000 telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:53:57.122171 telegram_gmail_bot-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 03:53:47.000000 telegram_gmail_bot-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 03:53:47.000000 telegram_gmail_bot-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-27 03:53:57.122171 telegram_gmail_bot-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 03:53:47.000000 telegram_gmail_bot-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 03:53:47.000000 telegram_gmail_bot-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 03:53:57.122171 telegram_gmail_bot-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-27 03:53:47.000000 telegram_gmail_bot-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 03:53:57.122171 telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-27 03:53:57.000000 telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 03:53:57.000000 telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 03:53:57.000000 telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 03:53:57.000000 telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 03:53:57.000000 telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 03:53:57.000000 telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/top_level.txt
```

### Comparing `telegram_gmail_bot-0.1.0/LICENSE` & `telegram_gmail_bot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.0/PKG-INFO` & `telegram_gmail_bot-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-gmail-bot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A bot that connects Telegram with Gmail
 Home-page: https://github.com/dustfeather/telegram-gmail-bot
 Author: Catalin Teodorescu
 Author-email: dustfeather@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telegram_gmail_bot-0.1.0/README.md` & `telegram_gmail_bot-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.0/requirements.txt` & `telegram_gmail_bot-0.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.0/setup.py` & `telegram_gmail_bot-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="telegram-gmail-bot",
-    version="0.1.0",
+    version="0.1.1",
     author="Catalin Teodorescu",
     author_email="dustfeather@gmail.com",
     description="A bot that connects Telegram with Gmail",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/dustfeather/telegram-gmail-bot",
     packages=find_packages(),
```

### Comparing `telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/PKG-INFO` & `telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-gmail-bot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A bot that connects Telegram with Gmail
 Home-page: https://github.com/dustfeather/telegram-gmail-bot
 Author: Catalin Teodorescu
 Author-email: dustfeather@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telegram_gmail_bot-0.1.0/telegram_gmail_bot.egg-info/requires.txt` & `telegram_gmail_bot-0.1.1/telegram_gmail_bot.egg-info/requires.txt`

 * *Files identical despite different names*

