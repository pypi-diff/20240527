# Comparing `tmp/musicseparationyt-1.0.1.tar.gz` & `tmp/musicseparationyt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicseparationyt-1.0.1.tar", last modified: Fri May 24 12:29:45 2024, max compression
+gzip compressed data, was "musicseparationyt-1.0.2.tar", last modified: Sun May 26 23:16:11 2024, max compression
```

## Comparing `musicseparationyt-1.0.1.tar` & `musicseparationyt-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 12:29:45.997928 musicseparationyt-1.0.1/
--rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.1/LICENSE
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 12:29:45.997366 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/
--rw-r--r--   0 yrry       (501) staff       (20)      563 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)      294 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/SOURCES.txt
--rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/dependency_links.txt
--rw-r--r--   0 yrry       (501) staff       (20)       44 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/requires.txt
--rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-24 12:29:45.000000 musicseparationyt-1.0.1/MusicSeparationYT.egg-info/top_level.txt
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-24 12:29:45.997177 musicseparationyt-1.0.1/MusicSeparationYTMain/
--rw-r--r--   0 yrry       (501) staff       (20)       68 2024-05-24 12:29:22.000000 musicseparationyt-1.0.1/MusicSeparationYTMain/__init__.py
--rw-r--r--   0 yrry       (501) staff       (20)     1109 2024-05-24 12:25:08.000000 musicseparationyt-1.0.1/MusicSeparationYTMain/main.py
--rw-r--r--   0 yrry       (501) staff       (20)      563 2024-05-24 12:29:45.997706 musicseparationyt-1.0.1/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)       86 2024-05-24 11:51:34.000000 musicseparationyt-1.0.1/README.md
--rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-24 12:29:45.997975 musicseparationyt-1.0.1/setup.cfg
--rw-r--r--   0 yrry       (501) staff       (20)     1321 2024-05-24 12:29:37.000000 musicseparationyt-1.0.1/setup.py
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:16:11.523553 musicseparationyt-1.0.2/
+-rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.2/LICENSE
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:16:11.523118 musicseparationyt-1.0.2/MusicSeparationYT.egg-info/
+-rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:16:11.000000 musicseparationyt-1.0.2/MusicSeparationYT.egg-info/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)      294 2024-05-26 23:16:11.000000 musicseparationyt-1.0.2/MusicSeparationYT.egg-info/SOURCES.txt
+-rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-26 23:16:11.000000 musicseparationyt-1.0.2/MusicSeparationYT.egg-info/dependency_links.txt
+-rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:16:11.000000 musicseparationyt-1.0.2/MusicSeparationYT.egg-info/requires.txt
+-rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:16:11.000000 musicseparationyt-1.0.2/MusicSeparationYT.egg-info/top_level.txt
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:16:11.522779 musicseparationyt-1.0.2/MusicSeparationYTMain/
+-rw-r--r--   0 yrry       (501) staff       (20)       68 2024-05-24 12:29:22.000000 musicseparationyt-1.0.2/MusicSeparationYTMain/__init__.py
+-rw-r--r--   0 yrry       (501) staff       (20)     1109 2024-05-26 22:56:17.000000 musicseparationyt-1.0.2/MusicSeparationYTMain/main.py
+-rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:16:11.523337 musicseparationyt-1.0.2/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)      532 2024-05-26 22:54:15.000000 musicseparationyt-1.0.2/README.md
+-rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-26 23:16:11.523603 musicseparationyt-1.0.2/setup.cfg
+-rw-r--r--   0 yrry       (501) staff       (20)     1309 2024-05-26 23:16:07.000000 musicseparationyt-1.0.2/setup.py
```

### Comparing `musicseparationyt-1.0.1/LICENSE` & `musicseparationyt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.1/MusicSeparationYTMain/main.py` & `musicseparationyt-1.0.2/MusicSeparationYTMain/main.py`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.1/setup.py` & `musicseparationyt-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python3
 
 # from setuptools import setup, find_packages
 import setuptools
-# from setuptools import find_packages
+from setuptools import find_packages
 
 # パッケージの基本情報
 name = "MusicSeparationYT"  # パッケージ名
-version = "1.0.1"  # バージョン番号
+version = "1.0.2"  # バージョン番号
 description = "this tool music download and seprate"  # パッケージの説明
-long_description_content_type="text/markdown",
+long_description_content_type="text/markdown"
 author = "Y-Ryohei"  # 作者名
-author_email = ""  # 作者のメールアドレス
-url = "https://github.com/Y-Ryohei/MusicSeparationYT"  # リポジトリURL
+# author_email = ""  # 作者のメールアドレス
+# url = "https://github.com/Y-Ryohei/MusicSeparationYT"  # リポジトリURL
 license = "MIT"  # ライセンス
 
 # インストールに必要な依存関係
 requirements = [
-  'pytube==15.0.0',
-  'moviepy==1.0.3',
-  'demucs==4.0.3',
+  'pytube',
+  'moviepy',
+  'demucs',
 ]
 
 # パッケージに含めるモジュール
-# packages = find_packages(),
+packages = find_packages()
 
 # その他の情報
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.6",
-    "Topic :: Software Development :: Libraries",
+    # "Development Status :: 4 - Beta",
+    # "Intended Audience :: Developers",
+    # "License :: OSI Approved :: MIT License",
+    # "Programming Language :: Python :: 3.6",
+    # "Topic :: Software Development :: Libraries",
 ]
 
 # セットアップ処理
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     author=author,
-    author_email=author_email,
-    url=url,
+    # author_email=author_email,
+    # url=url,
     license=license,
     install_requires=requirements,
-    # packages=packages,
+    packages=packages,
     classifiers=classifiers,
 )
```

