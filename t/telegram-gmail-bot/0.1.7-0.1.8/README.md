# Comparing `tmp/telegram_gmail_bot-0.1.7.tar.gz` & `tmp/telegram_gmail_bot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_gmail_bot-0.1.7.tar", last modified: Mon May 27 04:55:16 2024, max compression
+gzip compressed data, was "telegram_gmail_bot-0.1.8.tar", last modified: Mon May 27 05:06:59 2024, max compression
```

## Comparing `telegram_gmail_bot-0.1.7.tar` & `telegram_gmail_bot-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:55:16.612026 telegram_gmail_bot-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-27 04:55:16.612026 telegram_gmail_bot-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:55:16.612026 telegram_gmail_bot-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:55:16.608026 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:06:59.309735 telegram_gmail_bot-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 05:06:49.000000 telegram_gmail_bot-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 05:06:49.000000 telegram_gmail_bot-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-27 05:06:59.309735 telegram_gmail_bot-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-27 05:06:49.000000 telegram_gmail_bot-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 05:06:49.000000 telegram_gmail_bot-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 05:06:59.309735 telegram_gmail_bot-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 05:06:49.000000 telegram_gmail_bot-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:06:59.309735 telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-27 05:06:59.000000 telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 05:06:59.000000 telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 05:06:59.000000 telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 05:06:59.000000 telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 05:06:59.000000 telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 05:06:59.000000 telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/top_level.txt
```

### Comparing `telegram_gmail_bot-0.1.7/LICENSE` & `telegram_gmail_bot-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.7/PKG-INFO` & `telegram_gmail_bot-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-gmail-bot
-Version: 0.1.7
+Version: 0.1.8
 Summary: A bot that connects Telegram with Gmail
 Home-page: https://github.com/dustfeather/telegram-gmail-bot
 Author: Catalin Teodorescu
 Author-email: dustfeather@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telegram_gmail_bot-0.1.7/README.md` & `telegram_gmail_bot-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.7/requirements.txt` & `telegram_gmail_bot-0.1.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.7/setup.py` & `telegram_gmail_bot-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="telegram-gmail-bot",
-    version="0.1.7",
+    version="0.1.8",
     author="Catalin Teodorescu",
     author_email="dustfeather@gmail.com",
     description="A bot that connects Telegram with Gmail",
     long_description=open('README.md').read(),
     url="https://github.com/dustfeather/telegram-gmail-bot",
     packages=find_packages(),
     install_requires=[
```

### Comparing `telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/PKG-INFO` & `telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-gmail-bot
-Version: 0.1.7
+Version: 0.1.8
 Summary: A bot that connects Telegram with Gmail
 Home-page: https://github.com/dustfeather/telegram-gmail-bot
 Author: Catalin Teodorescu
 Author-email: dustfeather@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/requires.txt` & `telegram_gmail_bot-0.1.8/telegram_gmail_bot.egg-info/requires.txt`

 * *Files identical despite different names*

