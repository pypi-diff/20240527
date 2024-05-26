# Comparing `tmp/musicseparationyt-1.0.3.tar.gz` & `tmp/musicseparationyt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicseparationyt-1.0.3.tar", last modified: Sun May 26 23:20:45 2024, max compression
+gzip compressed data, was "musicseparationyt-1.0.4.tar", last modified: Sun May 26 23:32:00 2024, max compression
```

## Comparing `musicseparationyt-1.0.3.tar` & `musicseparationyt-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:20:45.851375 musicseparationyt-1.0.3/
--rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.3/LICENSE
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:20:45.850905 musicseparationyt-1.0.3/MusicSeparationYT.egg-info/
--rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:20:45.000000 musicseparationyt-1.0.3/MusicSeparationYT.egg-info/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)      294 2024-05-26 23:20:45.000000 musicseparationyt-1.0.3/MusicSeparationYT.egg-info/SOURCES.txt
--rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-26 23:20:45.000000 musicseparationyt-1.0.3/MusicSeparationYT.egg-info/dependency_links.txt
--rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:20:45.000000 musicseparationyt-1.0.3/MusicSeparationYT.egg-info/requires.txt
--rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:20:45.000000 musicseparationyt-1.0.3/MusicSeparationYT.egg-info/top_level.txt
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:20:45.850587 musicseparationyt-1.0.3/MusicSeparationYTMain/
--rw-r--r--   0 yrry       (501) staff       (20)       68 2024-05-24 12:29:22.000000 musicseparationyt-1.0.3/MusicSeparationYTMain/__init__.py
--rw-r--r--   0 yrry       (501) staff       (20)     1109 2024-05-26 22:56:17.000000 musicseparationyt-1.0.3/MusicSeparationYTMain/main.py
--rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:20:45.851122 musicseparationyt-1.0.3/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)      532 2024-05-26 22:54:15.000000 musicseparationyt-1.0.3/README.md
--rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-26 23:20:45.851420 musicseparationyt-1.0.3/setup.cfg
--rw-r--r--   0 yrry       (501) staff       (20)     1361 2024-05-26 23:20:43.000000 musicseparationyt-1.0.3/setup.py
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:32:00.536625 musicseparationyt-1.0.4/
+-rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.4/LICENSE
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:32:00.536124 musicseparationyt-1.0.4/MusicSeparationYT.egg-info/
+-rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:32:00.000000 musicseparationyt-1.0.4/MusicSeparationYT.egg-info/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)      294 2024-05-26 23:32:00.000000 musicseparationyt-1.0.4/MusicSeparationYT.egg-info/SOURCES.txt
+-rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-26 23:32:00.000000 musicseparationyt-1.0.4/MusicSeparationYT.egg-info/dependency_links.txt
+-rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:32:00.000000 musicseparationyt-1.0.4/MusicSeparationYT.egg-info/requires.txt
+-rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:32:00.000000 musicseparationyt-1.0.4/MusicSeparationYT.egg-info/top_level.txt
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:32:00.535833 musicseparationyt-1.0.4/MusicSeparationYTMain/
+-rw-r--r--   0 yrry       (501) staff       (20)       68 2024-05-24 12:29:22.000000 musicseparationyt-1.0.4/MusicSeparationYTMain/__init__.py
+-rw-r--r--   0 yrry       (501) staff       (20)     1109 2024-05-26 22:56:17.000000 musicseparationyt-1.0.4/MusicSeparationYTMain/main.py
+-rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:32:00.536368 musicseparationyt-1.0.4/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)      532 2024-05-26 22:54:15.000000 musicseparationyt-1.0.4/README.md
+-rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-26 23:32:00.536673 musicseparationyt-1.0.4/setup.cfg
+-rw-r--r--   0 yrry       (501) staff       (20)     1693 2024-05-26 23:31:55.000000 musicseparationyt-1.0.4/setup.py
```

### Comparing `musicseparationyt-1.0.3/LICENSE` & `musicseparationyt-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.3/MusicSeparationYTMain/main.py` & `musicseparationyt-1.0.4/MusicSeparationYTMain/main.py`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.3/README.md` & `musicseparationyt-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.3/setup.py` & `musicseparationyt-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 #!/usr/bin/env python3
 
 # from setuptools import setup, find_packages
+import os
 import setuptools
 from setuptools import find_packages
 
+current_directory = os.path.abspath(os.path.dirname(__file__))
+
+# READMEファイルを読み込む関数
+def read_readme():
+    with open(os.path.join(current_directory, 'README.md'), encoding='utf-8') as f:
+        return f.read()
+
+
 # パッケージの基本情報
 name = "MusicSeparationYT"  # パッケージ名
-version = "1.0.3"  # バージョン番号
+version = "1.0.4"  # バージョン番号
 description = "this tool music download and seprate"  # パッケージの説明
+
+long_description=read_readme(),  
+long_description_content_type='text/markdown',  
+
 # long_description_content_type="text/markdown"
-long_description = "README.md"  # 詳細な説明
+# long_description = "README.md"  # 詳細な説明
 author = "Y-Ryohei"  # 作者名
 # author_email = ""  # 作者のメールアドレス
 # url = "https://github.com/Y-Ryohei/MusicSeparationYT"  # リポジトリURL
 license = "MIT"  # ライセンス
 
 # インストールに必要な依存関係
 requirements = [
```

