# Comparing `tmp/discordreactive-0.5.tar.gz` & `tmp/discordreactive-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordreactive-0.5.tar", last modified: Mon May 27 15:06:34 2024, max compression
+gzip compressed data, was "discordreactive-0.6.tar", last modified: Mon May 27 15:19:47 2024, max compression
```

## Comparing `discordreactive-0.5.tar` & `discordreactive-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 15:06:34.931405 discordreactive-0.5/
--rw-rw-rw-   0        0        0      228 2024-05-27 15:06:34.930406 discordreactive-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 15:06:34.908418 discordreactive-0.5/discordreactive/
--rw-rw-rw-   0        0        0        0 2024-05-27 02:38:36.000000 discordreactive-0.5/discordreactive/__init__.py
--rw-rw-rw-   0        0        0      803 2024-05-27 15:04:59.000000 discordreactive-0.5/discordreactive/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 15:06:34.928407 discordreactive-0.5/discordreactive.egg-info/
--rw-rw-rw-   0        0        0      228 2024-05-27 15:06:34.000000 discordreactive-0.5/discordreactive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-27 15:06:34.000000 discordreactive-0.5/discordreactive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 15:06:34.000000 discordreactive-0.5/discordreactive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 15:06:34.000000 discordreactive-0.5/discordreactive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 15:06:34.931405 discordreactive-0.5/setup.cfg
--rw-rw-rw-   0        0        0      399 2024-05-27 15:06:31.000000 discordreactive-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 15:19:47.100006 discordreactive-0.6/
+-rw-rw-rw-   0        0        0      228 2024-05-27 15:19:47.098008 discordreactive-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 15:19:47.079018 discordreactive-0.6/discordreactive/
+-rw-rw-rw-   0        0        0        0 2024-05-27 02:38:36.000000 discordreactive-0.6/discordreactive/__init__.py
+-rw-rw-rw-   0        0        0     1142 2024-05-27 15:18:42.000000 discordreactive-0.6/discordreactive/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 15:19:47.097007 discordreactive-0.6/discordreactive.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-05-27 15:19:46.000000 discordreactive-0.6/discordreactive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-27 15:19:46.000000 discordreactive-0.6/discordreactive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 15:19:46.000000 discordreactive-0.6/discordreactive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 15:19:46.000000 discordreactive-0.6/discordreactive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 15:19:47.100006 discordreactive-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      399 2024-05-27 15:19:41.000000 discordreactive-0.6/setup.py
```

