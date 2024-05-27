# Comparing `tmp/telegram_gmail_bot-0.1.4.tar.gz` & `tmp/telegram_gmail_bot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_gmail_bot-0.1.4.tar", last modified: Mon May 27 04:33:26 2024, max compression
+gzip compressed data, was "telegram_gmail_bot-0.1.5.tar", last modified: Mon May 27 04:34:00 2024, max compression
```

## Comparing `telegram_gmail_bot-0.1.4.tar` & `telegram_gmail_bot-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:33:26.710201 telegram_gmail_bot-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 04:33:17.000000 telegram_gmail_bot-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 04:33:17.000000 telegram_gmail_bot-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 04:33:26.710201 telegram_gmail_bot-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 04:33:17.000000 telegram_gmail_bot-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 04:33:17.000000 telegram_gmail_bot-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:33:26.710201 telegram_gmail_bot-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-27 04:33:17.000000 telegram_gmail_bot-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:33:26.710201 telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 04:33:26.000000 telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 04:33:26.000000 telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:33:26.000000 telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 04:33:26.000000 telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 04:33:26.000000 telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:33:26.000000 telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/top_level.txt
```

### Comparing `telegram_gmail_bot-0.1.4/LICENSE` & `telegram_gmail_bot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.4/PKG-INFO` & `telegram_gmail_bot-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-gmail-bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: A bot that connects Telegram with Gmail
 Home-page: https://github.com/dustfeather/telegram-gmail-bot
 Author: Catalin Teodorescu
 Author-email: dustfeather@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telegram_gmail_bot-0.1.4/README.md` & `telegram_gmail_bot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.4/requirements.txt` & `telegram_gmail_bot-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.4/setup.py` & `telegram_gmail_bot-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="telegram-gmail-bot",
-    version="0.1.4",
+    version="0.1.5",
     author="Catalin Teodorescu",
     author_email="dustfeather@gmail.com",
     description="A bot that connects Telegram with Gmail",
     url="https://github.com/dustfeather/telegram-gmail-bot",
     packages=find_packages(),
     install_requires=[
         'anyio==4.4.0',
```

### Comparing `telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/PKG-INFO` & `telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-gmail-bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: A bot that connects Telegram with Gmail
 Home-page: https://github.com/dustfeather/telegram-gmail-bot
 Author: Catalin Teodorescu
 Author-email: dustfeather@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telegram_gmail_bot-0.1.4/telegram_gmail_bot.egg-info/requires.txt` & `telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/requires.txt`

 * *Files identical despite different names*

