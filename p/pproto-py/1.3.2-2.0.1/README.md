# Comparing `tmp/pproto-py-1.3.2.tar.gz` & `tmp/pproto-py-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pproto-py-1.3.2.tar", last modified: Fri Sep  2 14:54:30 2022, max compression
+gzip compressed data, was "pproto-py-2.0.1.tar", last modified: Mon May 27 07:20:13 2024, max compression
```

## Comparing `pproto-py-1.3.2.tar` & `pproto-py-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2022-09-02 14:54:30.840547 pproto-py-1.3.2/
--rw-rw-r--   0 pi        (1000) pi        (1000)      402 2022-09-02 14:54:30.840547 pproto-py-1.3.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       98 2022-08-26 09:42:07.000000 pproto-py-1.3.2/README.md
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2022-09-02 14:54:30.836547 pproto-py-1.3.2/pproto_py/
--rw-r--r--   0 pi        (1000) pi        (1000)      347 2022-08-26 10:09:25.000000 pproto-py-1.3.2/pproto_py/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      949 2022-08-26 09:42:09.000000 pproto-py-1.3.2/pproto_py/badSituations.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5753 2022-08-26 13:21:49.000000 pproto-py-1.3.2/pproto_py/baseCommands.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3840 2022-08-26 13:21:51.000000 pproto-py-1.3.2/pproto_py/baseCommandsImpl.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1655 2022-08-26 13:21:52.000000 pproto-py-1.3.2/pproto_py/commandList.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2022-09-02 14:54:30.836547 pproto-py-1.3.2/pproto_py/commands/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2022-01-25 06:18:01.000000 pproto-py-1.3.2/pproto_py/commands/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      259 2022-01-27 10:43:18.000000 pproto-py-1.3.2/pproto_py/commands/userCommands.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     1101 2022-02-03 09:26:17.000000 pproto-py-1.3.2/pproto_py/commands/userCommandsImpl.py
--rw-r--r--   0 pi        (1000) pi        (1000)      207 2021-09-21 15:49:55.000000 pproto-py-1.3.2/pproto_py/config.py
--rw-r--r--   0 pi        (1000) pi        (1000)    17856 2022-08-26 13:22:13.000000 pproto-py-1.3.2/pproto_py/connection.py
--rw-r--r--   0 pi        (1000) pi        (1000)      688 2022-08-26 13:22:14.000000 pproto-py-1.3.2/pproto_py/connectionPool.py
--rw-r--r--   0 pi        (1000) pi        (1000)       61 2021-09-20 08:11:46.000000 pproto-py-1.3.2/pproto_py/const.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6138 2021-09-20 08:11:46.000000 pproto-py-1.3.2/pproto_py/flags.py
--rw-r--r--   0 pi        (1000) pi        (1000)      524 2022-08-26 13:22:16.000000 pproto-py-1.3.2/pproto_py/handlerPool.py
--rw-r--r--   0 pi        (1000) pi        (1000)       98 2021-09-20 08:11:46.000000 pproto-py-1.3.2/pproto_py/logger.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7889 2022-08-26 13:22:18.000000 pproto-py-1.3.2/pproto_py/message.py
--rw-r--r--   0 pi        (1000) pi        (1000)      930 2022-08-26 13:22:20.000000 pproto-py-1.3.2/pproto_py/messagePool.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2185 2022-08-26 13:40:27.000000 pproto-py-1.3.2/pproto_py/tcpServer.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2713 2022-08-26 10:08:26.000000 pproto-py-1.3.2/pproto_py/tcpSocket.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6338 2022-08-26 13:22:57.000000 pproto-py-1.3.2/pproto_py/tcpWorker.py
--rw-r--r--   0 pi        (1000) pi        (1000)      987 2021-09-20 08:11:46.000000 pproto-py-1.3.2/pproto_py/tools.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2022-09-02 14:54:30.836547 pproto-py-1.3.2/pproto_py.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      402 2022-09-02 14:54:30.000000 pproto-py-1.3.2/pproto_py.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      674 2022-09-02 14:54:30.000000 pproto-py-1.3.2/pproto_py.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2022-09-02 14:54:30.000000 pproto-py-1.3.2/pproto_py.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       10 2022-09-02 14:54:30.000000 pproto-py-1.3.2/pproto_py.egg-info/top_level.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       38 2022-09-02 14:54:30.840547 pproto-py-1.3.2/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      543 2022-09-01 09:09:01.000000 pproto-py-1.3.2/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/
+-rw-r--r--   0 pi        (1000) pi        (1000)      358 2024-05-27 07:20:13.497506 pproto-py-2.0.1/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2043 2024-05-27 06:55:08.000000 pproto-py-2.0.1/README.md
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.493506 pproto-py-2.0.1/pproto_py/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      576 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      435 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/app.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/pproto_py/base/
+-rw-rw-r--   0 pi        (1000) pi        (1000)       42 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/base/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      584 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/base/base.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/pproto_py/client/
+-rw-rw-r--   0 pi        (1000) pi        (1000)       49 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/client/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4423 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/client/client.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/pproto_py/content/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      137 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/content/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1117 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/content/content.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      922 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/content/decorators.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/pproto_py/core/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      244 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/core/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      416 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/core/commands.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      604 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/core/exceptions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)       82 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/core/logger.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/pproto_py/schemas/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      358 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/schemas/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      140 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/schemas/exceptions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3876 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/schemas/message.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/pproto_py/server/
+-rw-rw-r--   0 pi        (1000) pi        (1000)       49 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/server/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      688 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/server/router.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6498 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pproto_py/server/server.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-27 07:20:13.497506 pproto-py-2.0.1/pproto_py.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      358 2024-05-27 07:20:13.000000 pproto-py-2.0.1/pproto_py.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      683 2024-05-27 07:20:13.000000 pproto-py-2.0.1/pproto_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2024-05-27 07:20:13.000000 pproto-py-2.0.1/pproto_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       10 2024-05-27 07:20:13.000000 pproto-py-2.0.1/pproto_py.egg-info/top_level.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)      806 2024-05-27 06:55:08.000000 pproto-py-2.0.1/pyproject.toml
+-rw-rw-r--   0 pi        (1000) pi        (1000)       38 2024-05-27 07:20:13.497506 pproto-py-2.0.1/setup.cfg
+-rw-rw-r--   0 pi        (1000) pi        (1000)      470 2024-05-27 06:55:08.000000 pproto-py-2.0.1/setup.py
```

