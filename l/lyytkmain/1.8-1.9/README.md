# Comparing `tmp/lyytkmain-1.8.tar.gz` & `tmp/lyytkmain-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyytkmain-1.8.tar", last modified: Wed May  1 14:06:31 2024, max compression
+gzip compressed data, was "lyytkmain-1.9.tar", last modified: Mon May 27 10:31:33 2024, max compression
```

## Comparing `lyytkmain-1.8.tar` & `lyytkmain-1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 14:06:31.895051 lyytkmain-1.8/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytkmain-1.8/LICENSE
--rw-rw-rw-   0        0        0      146 2024-05-01 14:06:31.894051 lyytkmain-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytkmain-1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 14:06:31.893051 lyytkmain-1.8/lyytkmain.egg-info/
--rw-rw-rw-   0        0        0      146 2024-05-01 14:06:31.000000 lyytkmain-1.8/lyytkmain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-05-01 14:06:31.000000 lyytkmain-1.8/lyytkmain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 14:06:31.000000 lyytkmain-1.8/lyytkmain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 14:06:31.000000 lyytkmain-1.8/lyytkmain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 14:06:31.000000 lyytkmain-1.8/lyytkmain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1071 2023-10-28 18:51:52.000000 lyytkmain-1.8/lyytkmain.py
--rw-rw-rw-   0        0        0       42 2024-05-01 14:06:31.895051 lyytkmain-1.8/setup.cfg
--rw-rw-rw-   0        0        0      271 2024-05-01 14:06:30.000000 lyytkmain-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:31:33.193514 lyytkmain-1.9/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyytkmain-1.9/LICENSE
+-rw-rw-rw-   0        0        0      173 2024-05-27 10:31:33.191515 lyytkmain-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyytkmain-1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:31:33.190514 lyytkmain-1.9/lyytkmain.egg-info/
+-rw-rw-rw-   0        0        0      173 2024-05-27 10:31:33.000000 lyytkmain-1.9/lyytkmain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-27 10:31:33.000000 lyytkmain-1.9/lyytkmain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:31:33.000000 lyytkmain-1.9/lyytkmain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 10:31:33.000000 lyytkmain-1.9/lyytkmain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-27 10:31:33.000000 lyytkmain-1.9/lyytkmain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12191 2024-05-27 10:31:26.000000 lyytkmain-1.9/lyytkmain.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:31:33.193514 lyytkmain-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      271 2024-05-27 10:31:32.000000 lyytkmain-1.9/setup.py
```

### Comparing `lyytkmain-1.8/LICENSE` & `lyytkmain-1.9/LICENSE`

 * *Files identical despite different names*

