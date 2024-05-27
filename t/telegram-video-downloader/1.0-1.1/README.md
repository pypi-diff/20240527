# Comparing `tmp/telegram-video-downloader-1.0.tar.gz` & `tmp/telegram-video-downloader-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-video-downloader-1.0.tar", last modified: Tue Apr 23 15:28:29 2024, max compression
+gzip compressed data, was "telegram-video-downloader-1.1.tar", last modified: Mon May 27 10:35:21 2024, max compression
```

## Comparing `telegram-video-downloader-1.0.tar` & `telegram-video-downloader-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 15:28:29.091243 telegram-video-downloader-1.0/
--rw-rw-rw-   0        0        0     1086 2024-04-23 10:40:15.000000 telegram-video-downloader-1.0/LICENSE
--rw-rw-rw-   0        0        0      311 2024-04-23 15:28:29.088030 telegram-video-downloader-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2823 2024-04-23 15:24:38.000000 telegram-video-downloader-1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 15:28:29.092308 telegram-video-downloader-1.0/setup.cfg
--rw-rw-rw-   0        0        0      597 2024-04-23 15:26:59.000000 telegram-video-downloader-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 15:28:29.041527 telegram-video-downloader-1.0/telegram_video_downloader/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:46:52.000000 telegram-video-downloader-1.0/telegram_video_downloader/__init__.py
--rw-rw-rw-   0        0        0     4635 2024-04-23 15:26:28.000000 telegram-video-downloader-1.0/telegram_video_downloader/app.py
-drwxrwxrwx   0        0        0        0 2024-04-23 15:28:29.086024 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/
--rw-rw-rw-   0        0        0      311 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 10:35:21.474938 telegram-video-downloader-1.1/
+-rw-rw-rw-   0        0        0     1086 2024-04-23 10:40:15.000000 telegram-video-downloader-1.1/LICENSE
+-rw-rw-rw-   0        0        0      311 2024-05-27 10:35:21.471944 telegram-video-downloader-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2666 2024-04-23 15:39:13.000000 telegram-video-downloader-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:35:21.474938 telegram-video-downloader-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      598 2024-05-27 10:35:11.000000 telegram-video-downloader-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:35:21.421289 telegram-video-downloader-1.1/telegram_video_downloader/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:46:52.000000 telegram-video-downloader-1.1/telegram_video_downloader/__init__.py
+-rw-rw-rw-   0        0        0     4638 2024-05-27 10:33:38.000000 telegram-video-downloader-1.1/telegram_video_downloader/app.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:35:21.468109 telegram-video-downloader-1.1/telegram_video_downloader.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-05-27 10:35:21.000000 telegram-video-downloader-1.1/telegram_video_downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-27 10:35:21.000000 telegram-video-downloader-1.1/telegram_video_downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:35:21.000000 telegram-video-downloader-1.1/telegram_video_downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-27 10:35:21.000000 telegram-video-downloader-1.1/telegram_video_downloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-05-27 10:35:21.000000 telegram-video-downloader-1.1/telegram_video_downloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-27 10:35:21.000000 telegram-video-downloader-1.1/telegram_video_downloader.egg-info/top_level.txt
```

### Comparing `telegram-video-downloader-1.0/LICENSE` & `telegram-video-downloader-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram-video-downloader-1.0/README.md` & `telegram-video-downloader-1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-# telegram-video-downloader
-Command to download a video published on Telegram
-Here is an example of a README.md for your Telegram Video Downloader project using Quart and Telethon, translated into English. Modify the details as necessary for your specific project.
-
----
-
 # Telegram Video Downloader
 
 This project enables you to download videos from Telegram directly to your computer, either via an HTTP API or by running the script in direct download mode. It utilizes Quart, an asynchronous Python framework, and Telethon, a Telegram client library.
 
 ## Prerequisites
 
 Before you start, make sure you have the following:
@@ -20,14 +14,18 @@
 
 1. pip install.
    ```
    pip install telegram-video-downloader
    ```
 
 2. Set up your environment variables or pass the necessary arguments (`api_id`, `api_hash`, `session_file`) to the script.
+ENV VARS
+- API_ID
+- API_HASH
+- SESSION_FILE (.session file full path)
 
 ## Usage
 
 The script can be run in two modes: `http` (by default) and `download`.
 
 ### HTTP Mode
 
@@ -51,20 +49,20 @@
 telegram-video-downloader --api_id YOUR_API_ID --api_hash YOUR_API_HASH --session_file PATH_TO_YOUR_SESSION_FILE --mode download --url TELEGRAM_VIDEO_URL --output OUTPUT_FOLDER
 ```
 
 ## Examples of Use
 
 - Starting the HTTP server:
   ```
-  telegram-video-downloader --api_id 123456 --api_hash abcdef1234567890abcdef1234567890 --session_file session_name.session --mode http
+  telegram-video-downloader --api_id 123456 --api_hash abcdef1234567890abcdef1234567890 --session_file /media/secure/telegram/session_name.session --mode http
   ```
 
 - Directly downloading a video:
   ```
-  telegram-video-downloader --api_id 123456 --api_hash abcdef1234567890abcdef1234567890 --session_file session_name.session --mode download --url https://t.me/pokemontvcastellano/1/2016 --output /media/telegram
+  telegram-video-downloader --api_id 123456 --api_hash abcdef1234567890abcdef1234567890 --session_file /media/secure/telegram/session_name.session --mode download --url https://t.me/pokemontvcastellano/1/2016 --output /media/telegram
   ```
 
 ## Contributions
 
 Contributions are welcome. Please feel free to fork the repository and submit your pull requests.
 
 ## License
```

### Comparing `telegram-video-downloader-1.0/setup.py` & `telegram-video-downloader-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='telegram-video-downloader',
-    version='1.0',
+    version='1.01',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'quart',
         'telethon',
     ],
     author='David Grau Martínez',
```

### Comparing `telegram-video-downloader-1.0/telegram_video_downloader/app.py` & `telegram-video-downloader-1.1/telegram_video_downloader/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,28 +19,28 @@
     args = parser.parse_args()
     return args
 
 # Initialization of the Telegram client
 args = parse_args()
 client = TelegramClient(args.session_file, args.api_id, args.api_hash)
 app = Quart(__name__)
-CHUNK_SIZE = 64 * 1024  # 64 KB
+CHUNK_SIZE = 1 * 1024 * 1024  # 1MB
 
 async def download_generator(client, document, start, end):
     pos = start
     remaining = end - start + 1
     async for chunk in client.iter_download(document, offset=pos, limit=remaining):
         yield chunk
         remaining -= len(chunk)
         if remaining <= 0:
             break
 
 async def download_url(url, output):
     split_url = url.split('/')
-    channel = split_url[-3]  # Ajusta según el formato real de tu URL.
+    channel = split_url[3]  # Ajusta según el formato real de tu URL.
     message_id = int(split_url[-1])
 
     await client.start()
     message = await client.get_messages(channel, ids=int(message_id))
     if not message or not hasattr(message, 'media'):
         return "Message not found or it doesn't contain any media", 404
```

