# Comparing `tmp/lyytktextbox-1.1.tar.gz` & `tmp/lyytktextbox-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyytktextbox-1.1.tar", last modified: Wed May  1 15:08:49 2024, max compression
+gzip compressed data, was "lyytktextbox-1.2.tar", last modified: Mon May 27 10:41:51 2024, max compression
```

## Comparing `lyytktextbox-1.1.tar` & `lyytktextbox-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:08:49.556685 lyytktextbox-1.1/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytktextbox-1.1/LICENSE
--rw-rw-rw-   0        0        0      149 2024-05-01 15:08:49.555685 lyytktextbox-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytktextbox-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 15:08:49.554683 lyytktextbox-1.1/lyytktextbox.egg-info/
--rw-rw-rw-   0        0        0      149 2024-05-01 15:08:49.000000 lyytktextbox-1.1/lyytktextbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-01 15:08:49.000000 lyytktextbox-1.1/lyytktextbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:08:49.000000 lyytktextbox-1.1/lyytktextbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 15:08:49.000000 lyytktextbox-1.1/lyytktextbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-01 15:08:49.000000 lyytktextbox-1.1/lyytktextbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6241 2024-05-01 15:08:22.000000 lyytktextbox-1.1/lyytktextbox.py
--rw-rw-rw-   0        0        0       42 2024-05-01 15:08:49.556685 lyytktextbox-1.1/setup.cfg
--rw-rw-rw-   0        0        0      274 2024-05-01 15:08:48.000000 lyytktextbox-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:51.983678 lyytktextbox-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytktextbox-1.2/LICENSE
+-rw-rw-rw-   0        0        0      176 2024-05-27 10:41:51.981680 lyytktextbox-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytktextbox-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:41:51.979679 lyytktextbox-1.2/lyytktextbox.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-27 10:41:51.000000 lyytktextbox-1.2/lyytktextbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-05-27 10:41:51.000000 lyytktextbox-1.2/lyytktextbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:41:51.000000 lyytktextbox-1.2/lyytktextbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 10:41:51.000000 lyytktextbox-1.2/lyytktextbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-27 10:41:51.000000 lyytktextbox-1.2/lyytktextbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    30836 2024-05-27 10:41:46.000000 lyytktextbox-1.2/lyytktextbox.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:41:51.983678 lyytktextbox-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      274 2024-05-27 10:41:51.000000 lyytktextbox-1.2/setup.py
```

### Comparing `lyytktextbox-1.1/LICENSE` & `lyytktextbox-1.2/LICENSE`

 * *Files identical despite different names*

