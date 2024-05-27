# Comparing `tmp/telegram_gmail_bot-0.1.5.tar.gz` & `tmp/telegram_gmail_bot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_gmail_bot-0.1.5.tar", last modified: Mon May 27 04:34:00 2024, max compression
+gzip compressed data, was "telegram_gmail_bot-0.1.7.tar", last modified: Mon May 27 04:55:16 2024, max compression
```

## Comparing `telegram_gmail_bot-0.1.5.tar` & `telegram_gmail_bot-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-27 04:33:43.000000 telegram_gmail_bot-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:34:00.203963 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:34:00.000000 telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:55:16.612026 telegram_gmail_bot-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-27 04:55:16.612026 telegram_gmail_bot-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:55:16.612026 telegram_gmail_bot-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 04:55:02.000000 telegram_gmail_bot-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:55:16.608026 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:55:16.000000 telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/top_level.txt
```

### Comparing `telegram_gmail_bot-0.1.5/LICENSE` & `telegram_gmail_bot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.5/README.md` & `telegram_gmail_bot-0.1.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 # Python Gmail Summary Bot
 
-> [!WARNING]
-> I recommend forking the repo and using it as a GitHub Action
+[![PyPI version](https://badge.fury.io/py/telegram-gmail-bot.svg)](https://badge.fury.io/py/telegram-gmail-bot)
 
-## Creating credentials for accessing Google APIs.
+A bot to summarize your Gmail emails using the Gmail API and send summaries to Telegram.
 
-### Step 1: Create a Service Account
+## Features
+- Summarizes Gmail emails.
+- Sends email summaries to a specified Telegram chat.
+
+## Installation
+
+You can install the package via pip:
+
+```shell
+pip install telegram-gmail-bot
+```
+
+## Setup
+
+### Creating credentials for accessing Google APIs
+
+#### Step 1: Create a Service Account
 
 1. **Go to the Google Cloud Console**: [Google Cloud Console](https://console.cloud.google.com/).
 2. **Select your project** or create a new one.
 3. Search for **APIs & Services** in the search bar.
 4. Click on **Credentials** in the left sidebar.
 5. Click on **Create Credentials** and select **OAuth client ID**.
 6. Select **Desktop app** as the application type.
-7. Add the generated credentials as environment variables in your project. 
+7. Add the generated credentials as environment variables in your project.
 
-### Step 2: Enable the Gmail API
+#### Step 2: Enable the Gmail API
 
 1. **Go to the API & Services page**: [API & Services](https://console.cloud.google.com/apis/dashboard).
 2. **Enable the Gmail API**:
-    - Click on "Enable APIs and Services".
-    - Search for "Gmail API" and enable it for your project.
-
-## Local usage
+   - Click on "Enable APIs and Services".
+   - Search for "Gmail API" and enable it for your project.
 
-```shell
-cp .env.example .env
-```
+## Local Usage
 
-```shell
-python3 -m venv .
-python3 -m pip install -r requirements.txt
-python3 main.py
-```
+1. Copy the example environment file and fill in your credentials:
+    ```shell
+    cp .env.example .env
+    ```
+
+2. Create a virtual environment and install dependencies:
+    ```shell
+    python3 -m venv .
+    source venv/bin/activate
+    pip install -r requirements.txt
+    ```
+
+3. Run the bot:
+    ```shell
+    python main.py
+    ```
```

### Comparing `telegram_gmail_bot-0.1.5/requirements.txt` & `telegram_gmail_bot-0.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `telegram_gmail_bot-0.1.5/setup.py` & `telegram_gmail_bot-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="telegram-gmail-bot",
-    version="0.1.5",
+    version="0.1.7",
     author="Catalin Teodorescu",
     author_email="dustfeather@gmail.com",
     description="A bot that connects Telegram with Gmail",
+    long_description=open('README.md').read(),
     url="https://github.com/dustfeather/telegram-gmail-bot",
     packages=find_packages(),
     install_requires=[
         'anyio==4.4.0',
         'cachetools==5.3.3',
         'certifi==2024.2.2',
         'charset-normalizer==3.3.2',
```

### Comparing `telegram_gmail_bot-0.1.5/telegram_gmail_bot.egg-info/requires.txt` & `telegram_gmail_bot-0.1.7/telegram_gmail_bot.egg-info/requires.txt`

 * *Files identical despite different names*

