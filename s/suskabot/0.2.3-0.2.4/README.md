# Comparing `tmp/suskabot-0.2.3.tar.gz` & `tmp/suskabot-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suskabot-0.2.3.tar", max compression
+gzip compressed data, was "suskabot-0.2.4.tar", max compression
```

## Comparing `suskabot-0.2.3.tar` & `suskabot-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1072 2024-05-23 11:47:00.739677 suskabot-0.2.3/LICENSE
--rw-r--r--   0        0        0     1817 2024-05-23 11:47:00.739677 suskabot-0.2.3/README.md
--rw-r--r--   0        0        0      815 2024-05-23 11:47:00.748679 suskabot-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      510 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/__init__.py
--rw-r--r--   0        0        0      581 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/__main__.py
--rw-r--r--   0        0        0       23 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/app/__init__.py
--rw-r--r--   0        0        0     1529 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/app/app.py
--rw-r--r--   0        0        0      381 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/.env.example
--rw-r--r--   0        0        0        4 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/.gitignore
--rw-r--r--   0        0        0       26 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/__init__.py
--rw-r--r--   0        0        0     4908 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/config.py
--rw-r--r--   0        0        0       32 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/controllers/__init__.py
--rw-r--r--   0        0        0       24 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/__init__.py
--rw-r--r--   0        0        0     1486 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/bot.py
--rw-r--r--   0        0        0       67 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/__init__.py
--rw-r--r--   0        0        0     1331 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/app.py
--rw-r--r--   0        0        0     1776 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/translator.py
--rw-r--r--   0        0        0     6758 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
--rw-r--r--   0        0        0       56 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/services/__init__.py
--rw-r--r--   0        0        0     4151 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/services/translator.py
--rw-r--r--   0        0        0     5924 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/services/youtube_downloader.py
--rw-r--r--   0        0        0       25 2024-05-23 11:47:00.750679 suskabot-0.2.3/suskabot/utils/__init__.py
--rw-r--r--   0        0        0      861 2024-05-23 11:47:00.750679 suskabot-0.2.3/suskabot/utils/utils.py
--rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 suskabot-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-27 09:30:40.814144 suskabot-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1817 2024-05-27 09:30:40.814144 suskabot-0.2.4/README.md
+-rw-r--r--   0        0        0      815 2024-05-27 09:30:40.823145 suskabot-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      510 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/__main__.py
+-rw-r--r--   0        0        0       23 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/app/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/app/app.py
+-rw-r--r--   0        0        0      381 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/config/.env.example
+-rw-r--r--   0        0        0        4 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/config/.gitignore
+-rw-r--r--   0        0        0       26 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/config/__init__.py
+-rw-r--r--   0        0        0     4908 2024-05-27 09:30:40.823145 suskabot-0.2.4/suskabot/config/config.py
+-rw-r--r--   0        0        0       32 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/controllers/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/controllers/telegram_api/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/controllers/telegram_api/bot.py
+-rw-r--r--   0        0        0       67 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/controllers/telegram_api/handlers/__init__.py
+-rw-r--r--   0        0        0     1331 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/controllers/telegram_api/handlers/app.py
+-rw-r--r--   0        0        0     1776 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/controllers/telegram_api/handlers/translator.py
+-rw-r--r--   0        0        0     6975 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
+-rw-r--r--   0        0        0       56 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/services/__init__.py
+-rw-r--r--   0        0        0     4151 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/services/translator.py
+-rw-r--r--   0        0        0     5354 2024-05-27 09:30:40.824144 suskabot-0.2.4/suskabot/services/youtube_downloader.py
+-rw-r--r--   0        0        0     2148 2024-05-27 09:30:40.825145 suskabot-0.2.4/suskabot/tests/test_youtube_downloader.py
+-rw-r--r--   0        0        0       25 2024-05-27 09:30:40.825145 suskabot-0.2.4/suskabot/utils/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-27 09:30:40.825145 suskabot-0.2.4/suskabot/utils/utils.py
+-rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 suskabot-0.2.4/PKG-INFO
```

### Comparing `suskabot-0.2.3/LICENSE` & `suskabot-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/README.md` & `suskabot-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/pyproject.toml` & `suskabot-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 package-mode = true
 name = "suskabot"
-version = "0.2.3"
+version = "0.2.4"
 description = "telegram bot with various functions"
 authors = ["vinyl_summer <vinyl6428@gmail.dotcom>"]
 readme = "README.md"
 license = "LICENSE"
 
 [[tool.poetry.source]]
 name = "gitlab"
```

### Comparing `suskabot-0.2.3/suskabot/__main__.py` & `suskabot-0.2.4/suskabot/__main__.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/suskabot/app/app.py` & `suskabot-0.2.4/suskabot/app/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/suskabot/config/config.py` & `suskabot-0.2.4/suskabot/config/config.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/suskabot/controllers/telegram_api/bot.py` & `suskabot-0.2.4/suskabot/controllers/telegram_api/bot.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/app.py` & `suskabot-0.2.4/suskabot/controllers/telegram_api/handlers/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/translator.py` & `suskabot-0.2.4/suskabot/controllers/telegram_api/handlers/translator.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/youtube_downloader.py` & `suskabot-0.2.4/suskabot/controllers/telegram_api/handlers/youtube_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,18 @@
             return
         except VideoTooLarge as e:
             logger.error(f"Video too larger error, {e}")
             await update.effective_message.reply_text(f"Video too larger error, {e}")
             return
 
         progressbar: str = utils.get_formatted_progressbar(video_stream.title, 0)
-        progressbar_message: Message = await update.effective_message.reply_text(progressbar)
+        progressbar_message: Message = await update.effective_message.reply_text(
+            progressbar,
+            parse_mode=telegram.constants.ParseMode.HTML
+        )
 
         self._users_with_a_download_in_progress.add(update.effective_user.id)
         logger.debug(f"Added {update.effective_user.id} to the set of downloading user, "
                      f"current set:{self._users_with_a_download_in_progress}")
 
         async def _delete_progressbar_callback(ctx: ContextTypes.DEFAULT_TYPE) -> None:
             message_to_delete: Message = ctx.job.data
@@ -139,19 +142,22 @@
                 return
 
         complete_progressbar: str = utils.get_formatted_progressbar(video_stream.title, 100)
         complete_progressbar += "\nDownload complete! Sending the video.."
         await progressbar_message.edit_text(complete_progressbar)
         logger.info(f"{video_stream.title} download completed, sending it to {update.effective_user.full_name}")
 
+        video_caption: str = f"<a href='{video_url}'>{video_stream.title}</a>"
+
         try:
             await context.bot.send_video(
                 chat_id=update.effective_chat.id,
                 video=downloaded_video,
-                caption=video_stream.title
+                caption=video_caption,
+                parse_mode=telegram.constants.ParseMode.HTML
             )
         except telegram.error.TelegramError as e:
             logger.error(f"Couldn't send downloaded video, {e}")
             await update.effective_message.reply_text(
                 "A Telegram error occurred"
             )
         finally:
```

### Comparing `suskabot-0.2.3/suskabot/services/translator.py` & `suskabot-0.2.4/suskabot/services/translator.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/suskabot/services/youtube_downloader.py` & `suskabot-0.2.4/suskabot/services/youtube_downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,14 @@
 logger: logging.Logger = logging.getLogger()
 
 
 class VideoTooLarge(Exception):
     """Raise if a video file size exceeds set limits"""
 
 
-class YTVideoMetadata:
-    title: str
-    filesize_bytes: int
-
-    def __init__(
-            self,
-            title: str,
-            filesize_bytes: int,
-    ) -> None:
-        self.title = title
-        self.filesize_bytes = filesize_bytes
-
-
 class YTDownloaderService:
     _minimum_video_resolution: int
     _maximum_video_resolution: int
     _file_size_limit_mb: int
     _save_to_drive: bool
 
     _default_download_path = pathlib.Path(os.getcwd()).joinpath("yt_downloads/")
@@ -119,16 +106,16 @@
         2) bytes, chunk of bytes downloaded
         3) int, number of bytes remaining
 
         :return: Bytes of the downloaded video or none
 
         :raises OSError: If save_to_drive is enabled and output file couldn't be opened
         """
-        # the only way to register a callback is at the moment of YouTube object creation.
-        # since this function only has a stream object to work with,
+        # the intended way to register a callback is at the moment of YouTube object creation.
+        # since this function only has a Stream object to work with,
         # registering a callback is impossible by normal means.
         # one more reason to migrate from pytube, lol
         video_stream._monostate.on_progress = progress_callback
 
         if self._save_to_drive:
             video_path: str = video_stream.download(
                 output_path=str(self._default_download_path)
@@ -138,15 +125,7 @@
                 video_stream.stream_to_buffer(buffer)
                 logger.info(f"Successfully downloaded {video_stream.title} to RAM")
                 return buffer.getvalue()
 
         with open(video_path, "rb") as video_file:
             logger.info(f"Successfully downloaded {video_stream.url} to drive")
             return video_file.read()
-
-    # doesn't serve any purpose as of now, but I'll leave it here for a bit
-    # def __clear_download_directory(self) -> None:
-    #     try:
-    #         shutil.rmtree(self._default_download_path)
-    #     except Exception as e:
-    #         logger.warning(f"Could not clear download directory, {e}")
-    #         raise e
```

### Comparing `suskabot-0.2.3/suskabot/utils/utils.py` & `suskabot-0.2.4/suskabot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.3/PKG-INFO` & `suskabot-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suskabot
-Version: 0.2.3
+Version: 0.2.4
 Summary: telegram bot with various functions
 License: LICENSE
 Author: vinyl_summer
 Author-email: vinyl6428@gmail.dotcom
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

