# Comparing `tmp/ctube-0.0.7.tar.gz` & `tmp/ctube-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctube-0.0.7.tar", max compression
+gzip compressed data, was "ctube-0.0.8.tar", max compression
```

## Comparing `ctube-0.0.7.tar` & `ctube-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.7/LICENSE
--rw-r--r--   0        0        0      610 2024-05-26 06:41:38.369693 ctube-0.0.7/README.md
--rw-r--r--   0        0        0       22 2024-05-26 06:41:38.369693 ctube-0.0.7/ctube/__init__.py
--rw-r--r--   0        0        0     5151 2024-05-25 21:58:13.207804 ctube-0.0.7/ctube/app.py
--rw-r--r--   0        0        0     1655 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/callbacks.py
--rw-r--r--   0        0        0      552 2024-05-25 21:58:58.300542 ctube-0.0.7/ctube/cli.py
--rw-r--r--   0        0        0     2223 2024-05-26 06:41:38.369693 ctube-0.0.7/ctube/cmds.py
--rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/colors.py
--rw-r--r--   0        0        0      353 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/containers.py
--rw-r--r--   0        0        0     4171 2024-05-25 21:59:24.906863 ctube-0.0.7/ctube/download.py
--rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/errors.py
--rw-r--r--   0        0        0     2119 2024-05-25 18:07:35.045348 ctube-0.0.7/ctube/extractors.py
--rw-r--r--   0        0        0     2327 2024-05-25 21:35:04.168284 ctube-0.0.7/ctube/helpers.py
--rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/parser.py
--rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/paths.py
--rw-r--r--   0        0        0     1682 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/printers.py
--rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.7/ctube/terminal.py
--rw-r--r--   0        0        0      641 2024-05-26 06:41:38.369693 ctube-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 ctube-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1030 2024-05-27 08:06:50.443204 ctube-0.0.8/README.md
+-rw-r--r--   0        0        0       22 2024-05-27 08:06:50.446538 ctube-0.0.8/ctube/__init__.py
+-rw-r--r--   0        0        0     5125 2024-05-27 08:06:50.446538 ctube-0.0.8/ctube/app.py
+-rw-r--r--   0        0        0     1655 2024-05-25 13:42:39.319492 ctube-0.0.8/ctube/callbacks.py
+-rw-r--r--   0        0        0      552 2024-05-25 21:58:58.300542 ctube-0.0.8/ctube/cli.py
+-rw-r--r--   0        0        0     2223 2024-05-26 06:41:38.369693 ctube-0.0.8/ctube/cmds.py
+-rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.8/ctube/colors.py
+-rw-r--r--   0        0        0      325 2024-05-27 08:06:50.446538 ctube-0.0.8/ctube/containers.py
+-rw-r--r--   0        0        0     4171 2024-05-25 21:59:24.906863 ctube-0.0.8/ctube/download.py
+-rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.8/ctube/errors.py
+-rw-r--r--   0        0        0     2119 2024-05-25 18:07:35.045348 ctube-0.0.8/ctube/extractors.py
+-rw-r--r--   0        0        0     2327 2024-05-25 21:35:04.168284 ctube-0.0.8/ctube/helpers.py
+-rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.8/ctube/parser.py
+-rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.8/ctube/paths.py
+-rw-r--r--   0        0        0     1682 2024-05-25 13:42:39.319492 ctube-0.0.8/ctube/printers.py
+-rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.8/ctube/terminal.py
+-rw-r--r--   0        0        0      641 2024-05-27 08:06:50.446538 ctube-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 ctube-0.0.8/PKG-INFO
```

### Comparing `ctube-0.0.7/LICENSE` & `ctube-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/app.py` & `ctube-0.0.8/ctube/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,34 +50,39 @@
         self._music_items: Optional[List[MusicItem]] = None
         self._artist_name: Optional[str] = None
 
     def main_loop(self) -> None:
         clear_screen()
         print_header()
         while True:
-            user_input = self.prompt.get_input()
+            user_input = self.prompt.get_input().strip()
+
             if not user_input: 
                 continue
+
             cmd_name, args = parse_user_input(user_input)
-            if cmd_name not in [cmd.value.name for cmd in Command]:
+
+            try:
+                cmd = Command.get_by_name(cmd_name)
+            except KeyError:
                 write(f"Invalid command: {cmd_name}", Color.RED)
-            elif cmd_name == Command.EXIT.value.name:
-                App._exit()
-            elif cmd_name == Command.CLEAR.value.name:
-                clear_screen()
-            elif cmd_name == Command.HELP.value.name:
-                print_help()
-            elif cmd_name == Command.SEARCH.value.name:
-                self._search(args)
-            elif cmd_name == Command.ID.value.name:
-                self._id(args)
-            elif cmd_name == Command.DOWNLOAD.value.name:
-                self._download(args)
             else:
-                write("Invalid syntax", Color.RED)
+                match cmd:
+                    case Command.EXIT:
+                        App._exit()
+                    case Command.CLEAR:
+                        clear_screen()
+                    case Command.HELP:
+                        print_help()
+                    case Command.SEARCH:
+                        self._search(args)
+                    case Command.ID:
+                        self._id(args)
+                    case Command.DOWNLOAD:
+                        self._download(args)
 
     @handle_connection_errors
     def _search(self, artist_name: str) -> None:
         if not artist_name:
             write("Missing argument: artist name", Color.RED)
         else:
             data = self.client.search(artist_name)
@@ -102,15 +107,15 @@
                 artist_music_data: Tuple[List[MusicItem], str]
                 self._music_items, self._artist_name = artist_music_data
                 write(f"Collected music for {self._artist_name}", Color.GREEN)
                 print_music_items(self._music_items)
 
     def _download(self, indexes: str):
         if not self._music_items or not self._artist_name:
-            write("You need to search for music first. ", Color.RED)
+            write("You need to search for music first.", Color.RED)
             write("Use the search/id command", Color.RED)
         elif not indexes:
             write("Missing argument: indexes", Color.RED)
         elif not connected_to_internet():
             write("No internet connection", Color.RED)
         else:
             try:
```

### Comparing `ctube-0.0.7/ctube/callbacks.py` & `ctube-0.0.8/ctube/callbacks.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/cli.py` & `ctube-0.0.8/ctube/cli.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/cmds.py` & `ctube-0.0.8/ctube/cmds.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/colors.py` & `ctube-0.0.8/ctube/colors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/download.py` & `ctube-0.0.8/ctube/download.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/extractors.py` & `ctube-0.0.8/ctube/extractors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/helpers.py` & `ctube-0.0.8/ctube/helpers.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/parser.py` & `ctube-0.0.8/ctube/parser.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/printers.py` & `ctube-0.0.8/ctube/printers.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/ctube/terminal.py` & `ctube-0.0.8/ctube/terminal.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.7/pyproject.toml` & `ctube-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctube"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Simone Gentili <gensydev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/ctube/"
 repository = "https://github.com/g3nsy/ctube"
 keywords = ["innertube", "youtube", "youtube-music", "python", "download", "music", "client"]
```

### Comparing `ctube-0.0.7/PKG-INFO` & `ctube-0.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctube
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Home-page: https://pypi.org/project/ctube/
 License: MIT
 Keywords: innertube,youtube,youtube-music,python,download,music,client
 Author: Simone Gentili
 Author-email: gensydev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -21,25 +21,42 @@
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytubefix (>=5.4.2,<6.0.0)
 Requires-Dist: requests (>=2.32.2,<3.0.0)
 Project-URL: Repository, https://github.com/g3nsy/ctube
 Description-Content-Type: text/markdown
 
 # ctube
-![Version](https://img.shields.io/badge/version-0.0.7-blue)
+![Version](https://img.shields.io/badge/version-0.0.8-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ---
 ctube is a simple program for downloading music. Written in Python, ctube has a command line interface.\
 Download in mp3 at the highest quality available. Metadata is automatically embedded in files (including cover art).\
 Type help for more information about the available commands and how they work.
 
 ### installation
 ```shell
 pip install ctube
 ```
 
+### usage
+to run ctube just type ctube in the terminal and press enter.
+
 ---
 <p align="center">
     <img src=".github/ctube.gif" alt="ctube.gif">
 </p>
 
+---
+
+The program is in a stable state, however some features are missing such as:
+- better artist search.
+- configuration via file.
+- better display of download status.
+- possibility to choose the metadata to embed.
+- possibility to choose the file format and other audio parameters.
+
+---
+Tested on Arch Linux:
+- alacritty 0.13.2
+- python 3.12.3
+
```

