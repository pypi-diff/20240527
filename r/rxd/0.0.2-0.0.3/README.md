# Comparing `tmp/rxd-0.0.2.tar.gz` & `tmp/rxd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxd-0.0.2.tar", last modified: Sat May 25 06:29:53 2024, max compression
+gzip compressed data, was "rxd-0.0.3.tar", last modified: Sun May 26 23:34:46 2024, max compression
```

## Comparing `rxd-0.0.2.tar` & `rxd-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-25 06:29:53.299436 rxd-0.0.2/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-25 06:29:53.299055 rxd-0.0.2/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.2/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-25 06:29:53.295640 rxd-0.0.2/rxd/
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.2/rxd/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)      123 2024-05-25 05:10:15.000000 rxd-0.0.2/rxd/daemon.py
--rw-r--r--   0 huy        (501) staff       (20)      330 2024-05-25 06:28:45.000000 rxd-0.0.2/rxd/install.py
--rw-r--r--   0 huy        (501) staff       (20)     2896 2024-05-24 19:56:24.000000 rxd-0.0.2/rxd/webui.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-25 06:29:53.298508 rxd-0.0.2/rxd.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-25 06:29:53.000000 rxd-0.0.2/rxd.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      236 2024-05-25 06:29:53.000000 rxd-0.0.2/rxd.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 06:29:53.000000 rxd-0.0.2/rxd.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.2/rxd.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-25 06:29:53.000000 rxd-0.0.2/rxd.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-25 06:29:53.000000 rxd-0.0.2/rxd.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-25 06:29:53.299634 rxd-0.0.2/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)      669 2024-05-25 06:29:09.000000 rxd-0.0.2/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:34:46.373052 rxd-0.0.3/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-26 23:34:46.372737 rxd-0.0.3/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.3/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:34:46.368097 rxd-0.0.3/rxd/
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.3/rxd/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     5733 2024-05-26 21:17:07.000000 rxd-0.0.3/rxd/app_manager.py
+-rwxr-xr-x   0 huy        (501) staff       (20)      410 2024-05-25 23:57:42.000000 rxd-0.0.3/rxd/ask.py
+-rw-r--r--   0 huy        (501) staff       (20)      939 2024-05-26 23:27:05.000000 rxd-0.0.3/rxd/cmd.py
+-rw-r--r--   0 huy        (501) staff       (20)     1815 2024-05-26 20:22:11.000000 rxd-0.0.3/rxd/cmd_app.py
+-rw-r--r--   0 huy        (501) staff       (20)     1148 2024-05-26 20:16:36.000000 rxd-0.0.3/rxd/cmd_responder.py
+-rw-r--r--   0 huy        (501) staff       (20)      358 2024-05-25 12:54:20.000000 rxd-0.0.3/rxd/cmd_setup.py
+-rw-r--r--   0 huy        (501) staff       (20)      111 2024-05-26 20:17:01.000000 rxd-0.0.3/rxd/cmd_worker_daemon.py
+-rw-r--r--   0 huy        (501) staff       (20)     2794 2024-05-25 22:31:16.000000 rxd-0.0.3/rxd/codex.py
+-rw-r--r--   0 huy        (501) staff       (20)      143 2024-05-26 16:11:09.000000 rxd-0.0.3/rxd/messages.py
+-rw-r--r--   0 huy        (501) staff       (20)      113 2024-05-25 23:36:37.000000 rxd-0.0.3/rxd/worker.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:34:46.372058 rxd-0.0.3/rxd.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      386 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.3/rxd.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)       12 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-26 23:34:46.373252 rxd-0.0.3/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)      788 2024-05-26 22:11:27.000000 rxd-0.0.3/setup.py
```

