# Comparing `tmp/discordreactive-0.1.tar.gz` & `tmp/discordreactive-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordreactive-0.1.tar", last modified: Mon May 27 03:19:58 2024, max compression
+gzip compressed data, was "discordreactive-0.2.tar", last modified: Mon May 27 03:22:44 2024, max compression
```

## Comparing `discordreactive-0.1.tar` & `discordreactive-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 03:19:58.643063 discordreactive-0.1/
--rw-rw-rw-   0        0        0      228 2024-05-27 03:19:58.642064 discordreactive-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 03:19:58.632070 discordreactive-0.1/discordreactive/
--rw-rw-rw-   0        0        0        0 2024-05-27 02:38:36.000000 discordreactive-0.1/discordreactive/__init__.py
--rw-rw-rw-   0        0        0      135 2024-05-27 03:10:16.000000 discordreactive-0.1/discordreactive/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 03:19:58.640065 discordreactive-0.1/discordreactive.egg-info/
--rw-rw-rw-   0        0        0      228 2024-05-27 03:19:58.000000 discordreactive-0.1/discordreactive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-27 03:19:58.000000 discordreactive-0.1/discordreactive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 03:19:58.000000 discordreactive-0.1/discordreactive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 03:19:58.000000 discordreactive-0.1/discordreactive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 03:19:58.643063 discordreactive-0.1/setup.cfg
--rw-rw-rw-   0        0        0      399 2024-05-27 03:18:28.000000 discordreactive-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:22:44.560469 discordreactive-0.2/
+-rw-rw-rw-   0        0        0      228 2024-05-27 03:22:44.559470 discordreactive-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 03:22:44.550476 discordreactive-0.2/discordreactive/
+-rw-rw-rw-   0        0        0        0 2024-05-27 02:38:36.000000 discordreactive-0.2/discordreactive/__init__.py
+-rw-rw-rw-   0        0        0      258 2024-05-27 03:22:26.000000 discordreactive-0.2/discordreactive/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:22:44.558470 discordreactive-0.2/discordreactive.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-05-27 03:22:44.000000 discordreactive-0.2/discordreactive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-27 03:22:44.000000 discordreactive-0.2/discordreactive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:22:44.000000 discordreactive-0.2/discordreactive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 03:22:44.000000 discordreactive-0.2/discordreactive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 03:22:44.561468 discordreactive-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      399 2024-05-27 03:22:40.000000 discordreactive-0.2/setup.py
```

