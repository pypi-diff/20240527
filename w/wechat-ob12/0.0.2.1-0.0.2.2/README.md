# Comparing `tmp/wechat_ob12-0.0.2.1.tar.gz` & `tmp/wechat_ob12-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wechat_ob12-0.0.2.1.tar", last modified: Sat Feb 17 12:00:28 2024, max compression
+gzip compressed data, was "wechat_ob12-0.0.2.2.tar", last modified: Mon May 27 11:30:34 2024, max compression
```

## Comparing `wechat_ob12-0.0.2.1.tar` & `wechat_ob12-0.0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 12:00:28.113651 wechat_ob12-0.0.2.1/
--rw-rw-rw-   0        0        0     1091 2024-02-16 14:09:44.000000 wechat_ob12-0.0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      310 2024-02-17 12:00:28.111655 wechat_ob12-0.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       20 2024-02-16 14:10:43.000000 wechat_ob12-0.0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-02-17 12:00:28.113651 wechat_ob12-0.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      500 2024-02-17 12:00:16.000000 wechat_ob12-0.0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-17 12:00:28.096695 wechat_ob12-0.0.2.1/wechat_ob12/
--rw-rw-rw-   0        0        0      930 2024-02-17 11:55:19.000000 wechat_ob12-0.0.2.1/wechat_ob12/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-17 12:00:28.109662 wechat_ob12-0.0.2.1/wechat_ob12.egg-info/
--rw-rw-rw-   0        0        0      310 2024-02-17 12:00:27.000000 wechat_ob12-0.0.2.1/wechat_ob12.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-02-17 12:00:27.000000 wechat_ob12-0.0.2.1/wechat_ob12.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 12:00:27.000000 wechat_ob12-0.0.2.1/wechat_ob12.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-17 12:00:27.000000 wechat_ob12-0.0.2.1/wechat_ob12.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 11:30:34.843199 wechat_ob12-0.0.2.2/
+-rw-rw-rw-   0        0        0     1091 2024-02-16 14:09:44.000000 wechat_ob12-0.0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      310 2024-05-27 11:30:34.841209 wechat_ob12-0.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2024-02-16 14:10:43.000000 wechat_ob12-0.0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:30:34.844163 wechat_ob12-0.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      502 2024-05-27 11:23:44.000000 wechat_ob12-0.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:30:34.818193 wechat_ob12-0.0.2.2/wechat_ob12/
+-rw-rw-rw-   0        0        0      997 2024-05-27 11:23:44.000000 wechat_ob12-0.0.2.2/wechat_ob12/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:30:34.839176 wechat_ob12-0.0.2.2/wechat_ob12.egg-info/
+-rw-rw-rw-   0        0        0      310 2024-05-27 11:30:34.000000 wechat_ob12-0.0.2.2/wechat_ob12.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-05-27 11:30:34.000000 wechat_ob12-0.0.2.2/wechat_ob12.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:30:34.000000 wechat_ob12-0.0.2.2/wechat_ob12.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 11:30:34.000000 wechat_ob12-0.0.2.2/wechat_ob12.egg-info/top_level.txt
```

### Comparing `wechat_ob12-0.0.2.1/LICENSE.txt` & `wechat_ob12-0.0.2.2/LICENSE.txt`

 * *Files identical despite different names*

