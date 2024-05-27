# Comparing `tmp/discordreactive-0.0.7.tar.gz` & `tmp/discordreactive-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordreactive-0.0.7.tar", last modified: Mon May 27 02:43:49 2024, max compression
+gzip compressed data, was "discordreactive-0.0.8.tar", last modified: Mon May 27 02:52:31 2024, max compression
```

## Comparing `discordreactive-0.0.7.tar` & `discordreactive-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 02:43:49.951460 discordreactive-0.0.7/
--rw-rw-rw-   0        0        0      230 2024-05-27 02:43:49.950461 discordreactive-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 02:43:49.941466 discordreactive-0.0.7/discordreactive/
--rw-rw-rw-   0        0        0        0 2024-05-27 02:38:36.000000 discordreactive-0.0.7/discordreactive/__init__.py
--rw-rw-rw-   0        0        0      135 2024-05-27 02:43:24.000000 discordreactive-0.0.7/discordreactive/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 02:43:49.949461 discordreactive-0.0.7/discordreactive.egg-info/
--rw-rw-rw-   0        0        0      230 2024-05-27 02:43:49.000000 discordreactive-0.0.7/discordreactive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-27 02:43:49.000000 discordreactive-0.0.7/discordreactive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 02:43:49.000000 discordreactive-0.0.7/discordreactive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 02:43:49.000000 discordreactive-0.0.7/discordreactive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 02:43:49.952459 discordreactive-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      401 2024-05-27 02:43:40.000000 discordreactive-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 02:52:31.319788 discordreactive-0.0.8/
+-rw-rw-rw-   0        0        0      230 2024-05-27 02:52:31.318789 discordreactive-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 02:52:31.305797 discordreactive-0.0.8/discordreactive/
+-rw-rw-rw-   0        0        0        0 2024-05-27 02:38:36.000000 discordreactive-0.0.8/discordreactive/__init__.py
+-rw-rw-rw-   0        0        0      643 2024-05-27 02:52:04.000000 discordreactive-0.0.8/discordreactive/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 02:52:31.316790 discordreactive-0.0.8/discordreactive.egg-info/
+-rw-rw-rw-   0        0        0      230 2024-05-27 02:52:31.000000 discordreactive-0.0.8/discordreactive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-27 02:52:31.000000 discordreactive-0.0.8/discordreactive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 02:52:31.000000 discordreactive-0.0.8/discordreactive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 02:52:31.000000 discordreactive-0.0.8/discordreactive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 02:52:31.319788 discordreactive-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      401 2024-05-27 02:52:24.000000 discordreactive-0.0.8/setup.py
```

