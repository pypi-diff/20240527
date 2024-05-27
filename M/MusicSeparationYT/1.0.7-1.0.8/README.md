# Comparing `tmp/musicseparationyt-1.0.7.tar.gz` & `tmp/musicseparationyt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicseparationyt-1.0.7.tar", last modified: Sun May 26 23:36:48 2024, max compression
+gzip compressed data, was "musicseparationyt-1.0.8.tar", last modified: Sun May 26 23:46:02 2024, max compression
```

## Comparing `musicseparationyt-1.0.7.tar` & `musicseparationyt-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:36:48.616765 musicseparationyt-1.0.7/
--rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.7/LICENSE
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:36:48.616309 musicseparationyt-1.0.7/MusicSeparationYT.egg-info/
--rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:36:48.000000 musicseparationyt-1.0.7/MusicSeparationYT.egg-info/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)      294 2024-05-26 23:36:48.000000 musicseparationyt-1.0.7/MusicSeparationYT.egg-info/SOURCES.txt
--rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-26 23:36:48.000000 musicseparationyt-1.0.7/MusicSeparationYT.egg-info/dependency_links.txt
--rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:36:48.000000 musicseparationyt-1.0.7/MusicSeparationYT.egg-info/requires.txt
--rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:36:48.000000 musicseparationyt-1.0.7/MusicSeparationYT.egg-info/top_level.txt
-drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:36:48.616123 musicseparationyt-1.0.7/MusicSeparationYTMain/
--rw-r--r--   0 yrry       (501) staff       (20)       68 2024-05-24 12:29:22.000000 musicseparationyt-1.0.7/MusicSeparationYTMain/__init__.py
--rw-r--r--   0 yrry       (501) staff       (20)     1109 2024-05-26 22:56:17.000000 musicseparationyt-1.0.7/MusicSeparationYTMain/main.py
--rw-r--r--   0 yrry       (501) staff       (20)      226 2024-05-26 23:36:48.616533 musicseparationyt-1.0.7/PKG-INFO
--rw-r--r--   0 yrry       (501) staff       (20)      532 2024-05-26 22:54:15.000000 musicseparationyt-1.0.7/README.md
--rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-26 23:36:48.616810 musicseparationyt-1.0.7/setup.cfg
--rw-r--r--   0 yrry       (501) staff       (20)     1744 2024-05-26 23:36:40.000000 musicseparationyt-1.0.7/setup.py
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:46:02.085616 musicseparationyt-1.0.8/
+-rw-r--r--   0 yrry       (501) staff       (20)     1051 2024-05-24 09:16:34.000000 musicseparationyt-1.0.8/LICENSE
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:46:02.085188 musicseparationyt-1.0.8/MusicSeparationYT.egg-info/
+-rw-r--r--   0 yrry       (501) staff       (20)      733 2024-05-26 23:46:02.000000 musicseparationyt-1.0.8/MusicSeparationYT.egg-info/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)      254 2024-05-26 23:46:02.000000 musicseparationyt-1.0.8/MusicSeparationYT.egg-info/SOURCES.txt
+-rw-r--r--   0 yrry       (501) staff       (20)        1 2024-05-26 23:46:02.000000 musicseparationyt-1.0.8/MusicSeparationYT.egg-info/dependency_links.txt
+-rw-r--r--   0 yrry       (501) staff       (20)       22 2024-05-26 23:46:02.000000 musicseparationyt-1.0.8/MusicSeparationYT.egg-info/top_level.txt
+drwxr-xr-x   0 yrry       (501) staff       (20)        0 2024-05-26 23:46:02.085013 musicseparationyt-1.0.8/MusicSeparationYTMain/
+-rw-r--r--   0 yrry       (501) staff       (20)       68 2024-05-24 12:29:22.000000 musicseparationyt-1.0.8/MusicSeparationYTMain/__init__.py
+-rw-r--r--   0 yrry       (501) staff       (20)     1109 2024-05-26 22:56:17.000000 musicseparationyt-1.0.8/MusicSeparationYTMain/main.py
+-rw-r--r--   0 yrry       (501) staff       (20)      733 2024-05-26 23:46:02.085393 musicseparationyt-1.0.8/PKG-INFO
+-rw-r--r--   0 yrry       (501) staff       (20)      532 2024-05-26 22:54:15.000000 musicseparationyt-1.0.8/README.md
+-rw-r--r--   0 yrry       (501) staff       (20)       38 2024-05-26 23:46:02.085660 musicseparationyt-1.0.8/setup.cfg
+-rw-r--r--   0 yrry       (501) staff       (20)     2544 2024-05-26 23:45:55.000000 musicseparationyt-1.0.8/setup.py
```

### Comparing `musicseparationyt-1.0.7/LICENSE` & `musicseparationyt-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.7/MusicSeparationYTMain/main.py` & `musicseparationyt-1.0.8/MusicSeparationYTMain/main.py`

 * *Files identical despite different names*

### Comparing `musicseparationyt-1.0.7/README.md` & `musicseparationyt-1.0.8/README.md`

 * *Files identical despite different names*

