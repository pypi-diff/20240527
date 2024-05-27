# Comparing `tmp/discordreactive-0.0.5.tar.gz` & `tmp/discordreactive-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordreactive-0.0.5.tar", last modified: Mon May 27 02:27:59 2024, max compression
+gzip compressed data, was "discordreactive-0.0.6.tar", last modified: Mon May 27 02:39:13 2024, max compression
```

## Comparing `discordreactive-0.0.5.tar` & `discordreactive-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 02:27:59.559556 discordreactive-0.0.5/
--rw-rw-rw-   0        0        0      230 2024-05-27 02:27:59.558557 discordreactive-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 02:27:59.549563 discordreactive-0.0.5/discordreactive/
--rw-rw-rw-   0        0        0      643 2024-05-27 02:27:17.000000 discordreactive-0.0.5/discordreactive/__init__.py
--rw-rw-rw-   0        0        0       65 2024-05-27 01:04:42.000000 discordreactive-0.0.5/discordreactive/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 02:27:59.557558 discordreactive-0.0.5/discordreactive.egg-info/
--rw-rw-rw-   0        0        0      230 2024-05-27 02:27:59.000000 discordreactive-0.0.5/discordreactive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-27 02:27:59.000000 discordreactive-0.0.5/discordreactive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 02:27:59.000000 discordreactive-0.0.5/discordreactive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 02:27:59.000000 discordreactive-0.0.5/discordreactive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 02:27:59.559556 discordreactive-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      401 2024-05-27 02:27:46.000000 discordreactive-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 02:39:13.633777 discordreactive-0.0.6/
+-rw-rw-rw-   0        0        0      230 2024-05-27 02:39:13.631779 discordreactive-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 02:39:13.622783 discordreactive-0.0.6/discordreactive/
+-rw-rw-rw-   0        0        0        0 2024-05-27 02:38:36.000000 discordreactive-0.0.6/discordreactive/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-05-27 01:04:42.000000 discordreactive-0.0.6/discordreactive/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 02:39:13.630779 discordreactive-0.0.6/discordreactive.egg-info/
+-rw-rw-rw-   0        0        0      230 2024-05-27 02:39:13.000000 discordreactive-0.0.6/discordreactive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-27 02:39:13.000000 discordreactive-0.0.6/discordreactive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 02:39:13.000000 discordreactive-0.0.6/discordreactive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 02:39:13.000000 discordreactive-0.0.6/discordreactive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 02:39:13.634777 discordreactive-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      401 2024-05-27 02:38:52.000000 discordreactive-0.0.6/setup.py
```
