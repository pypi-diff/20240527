# Comparing `tmp/Hypercorn-0.9.4.tar.gz` & `tmp/Hypercorn-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Hypercorn-0.9.4.tar", last modified: Tue Mar 31 14:38:48 2020, max compression
+gzip compressed data, was "dist/Hypercorn-0.9.5.tar", last modified: Sun Apr 19 18:24:57 2020, max compression
```

## Comparing `Hypercorn-0.9.4.tar` & `Hypercorn-0.9.5.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.643102 Hypercorn-0.9.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13594 2020-03-31 14:38:38.000000 Hypercorn-0.9.4/CHANGELOG.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5070 2020-03-31 14:38:48.643102 Hypercorn-0.9.4/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3321 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.631102 Hypercorn-0.9.4/artwork/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/artwork/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22901 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/artwork/logo.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18990 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/artwork/logo.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7610 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/artwork/logo_small.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5917 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/artwork/logo_small.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      487 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2020-03-31 14:38:48.643102 Hypercorn-0.9.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2078 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.631102 Hypercorn-0.9.4/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.635102 Hypercorn-0.9.4/src/Hypercorn.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5070 2020-03-31 14:38:48.000000 Hypercorn-0.9.4/src/Hypercorn.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2092 2020-03-31 14:38:48.000000 Hypercorn-0.9.4/src/Hypercorn.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2020-03-31 14:38:48.000000 Hypercorn-0.9.4/src/Hypercorn.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2020-03-31 14:38:48.000000 Hypercorn-0.9.4/src/Hypercorn.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2020-03-31 14:38:48.000000 Hypercorn-0.9.4/src/Hypercorn.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2020-03-31 14:38:48.000000 Hypercorn-0.9.4/src/Hypercorn.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.635102 Hypercorn-0.9.4/src/hypercorn/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2020-03-31 14:38:44.000000 Hypercorn-0.9.4/src/hypercorn/__about__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       99 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8275 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.635102 Hypercorn-0.9.4/src/hypercorn/asyncio/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/asyncio/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3067 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/asyncio/lifespan.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7941 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/asyncio/run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/asyncio/spawn_app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      733 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/asyncio/statsd.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4824 2020-03-31 14:38:38.000000 Hypercorn-0.9.4/src/hypercorn/asyncio/tcp_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2441 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/asyncio/udp_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11619 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      440 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/events.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6870 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/logging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2951 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/middleware.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.639102 Hypercorn-0.9.4/src/hypercorn/protocol/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     2809 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/events.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    10387 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/h11.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    13606 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/h2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4857 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/h3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6467 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/http_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4642 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/quic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13133 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/protocol/ws_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/py.typed
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2247 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/statsd.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.639102 Hypercorn-0.9.4/src/hypercorn/trio/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1318 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/trio/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2749 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/trio/lifespan.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/trio/run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1250 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/trio/spawn_app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      450 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/trio/statsd.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5243 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/trio/tcp_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/trio/udp_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1950 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/typing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6682 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/src/hypercorn/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.639102 Hypercorn-0.9.4/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.639102 Hypercorn-0.9.4/tests/assets/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1651 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/assets/cert.pem
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      104 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/assets/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/assets/config.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      173 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/assets/config_ssl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3268 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/assets/key.pem
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.643102 Hypercorn-0.9.4/tests/asyncio/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/asyncio/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1470 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/asyncio/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3476 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/asyncio/test_keep_alive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1606 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/asyncio/test_lifespan.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7485 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/asyncio/test_sanity.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/asyncio/test_tcp_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      224 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/helpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.643102 Hypercorn-0.9.4/tests/protocol/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    10710 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/protocol/test_h11.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/protocol/test_h2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7105 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/protocol/test_http_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/protocol/test_ws_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2603 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/test___main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4584 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/test_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3655 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/test_logging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4705 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/test_middleware.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2666 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/test_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-31 14:38:48.643102 Hypercorn-0.9.4/tests/trio/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/trio/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3667 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/trio/test_keep_alive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/trio/test_lifespan.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7683 2020-03-23 19:25:08.000000 Hypercorn-0.9.4/tests/trio/test_sanity.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.789571 Hypercorn-0.9.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13893 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/CHANGELOG.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5070 2020-04-19 18:24:57.789571 Hypercorn-0.9.5/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3321 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.781571 Hypercorn-0.9.5/artwork/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/artwork/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22901 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/artwork/logo.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18990 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/artwork/logo.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7610 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/artwork/logo_small.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5917 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/artwork/logo_small.svg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      487 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2020-04-19 18:24:57.789571 Hypercorn-0.9.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2078 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.777571 Hypercorn-0.9.5/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.781571 Hypercorn-0.9.5/src/Hypercorn.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5070 2020-04-19 18:24:57.000000 Hypercorn-0.9.5/src/Hypercorn.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2128 2020-04-19 18:24:57.000000 Hypercorn-0.9.5/src/Hypercorn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2020-04-19 18:24:57.000000 Hypercorn-0.9.5/src/Hypercorn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2020-04-19 18:24:57.000000 Hypercorn-0.9.5/src/Hypercorn.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2020-04-19 18:24:57.000000 Hypercorn-0.9.5/src/Hypercorn.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2020-04-19 18:24:57.000000 Hypercorn-0.9.5/src/Hypercorn.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.781571 Hypercorn-0.9.5/src/hypercorn/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2020-04-19 18:24:44.000000 Hypercorn-0.9.5/src/hypercorn/__about__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       99 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8376 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/src/hypercorn/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.785571 Hypercorn-0.9.5/src/hypercorn/asyncio/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3067 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/lifespan.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7941 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      900 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/spawn_app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      733 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/statsd.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/task_group.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4983 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/tcp_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2441 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/asyncio/udp_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11619 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      440 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/events.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6870 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2951 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/middleware.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.785571 Hypercorn-0.9.5/src/hypercorn/protocol/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     2809 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/protocol/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/protocol/events.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    10387 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/protocol/h11.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    13647 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/src/hypercorn/protocol/h2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4857 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/protocol/h3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6467 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/protocol/http_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4642 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/protocol/quic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13133 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/protocol/ws_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/py.typed
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2247 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/statsd.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.785571 Hypercorn-0.9.5/src/hypercorn/trio/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1318 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/trio/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2749 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/trio/lifespan.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/trio/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1250 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/trio/spawn_app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      450 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/trio/statsd.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5243 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/trio/tcp_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/trio/udp_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1950 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/typing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6682 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/src/hypercorn/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.785571 Hypercorn-0.9.5/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.785571 Hypercorn-0.9.5/tests/assets/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1651 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/assets/cert.pem
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      104 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/assets/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/assets/config.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      173 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/assets/config_ssl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3268 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/assets/key.pem
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.785571 Hypercorn-0.9.5/tests/asyncio/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/asyncio/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1470 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/asyncio/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3476 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/asyncio/test_keep_alive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1606 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/asyncio/test_lifespan.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7485 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/asyncio/test_sanity.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2958 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/tests/asyncio/test_tcp_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      224 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/helpers.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.785571 Hypercorn-0.9.5/tests/protocol/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    10710 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/protocol/test_h11.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2854 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/protocol/test_h2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7105 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/protocol/test_http_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/protocol/test_ws_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2603 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/test___main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4584 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/test_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3655 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/test_logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4691 2020-04-19 18:24:39.000000 Hypercorn-0.9.5/tests/test_middleware.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2666 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/test_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2020-04-19 18:24:57.789571 Hypercorn-0.9.5/tests/trio/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/trio/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3667 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/trio/test_keep_alive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/trio/test_lifespan.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7683 2020-03-23 19:25:08.000000 Hypercorn-0.9.5/tests/trio/test_sanity.py
```

### Comparing `Hypercorn-0.9.4/CHANGELOG.rst` & `Hypercorn-0.9.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+0.9.5 2020-04-19
+----------------
+
+* Bugfix also catch RuntimeError for uvloop workers.
+* Bugfix correct handling of verify-flag argument and improved error
+  message on bad values.
+* Bugfix correctly cope with TCP half closes via asyncio.
+* Bugfix handle MissingStreamError and KeyError (HTTP/2).
+
 0.9.4 2020-03-31
 ----------------
 
 * Bugfix AssertionError when draining.
 * Bugfix catch the correct timeout error.
 
 0.9.3 2020-03-23
```

### Comparing `Hypercorn-0.9.4/LICENSE` & `Hypercorn-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/PKG-INFO` & `Hypercorn-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hypercorn
-Version: 0.9.4
+Version: 0.9.5
 Summary: A ASGI Server based on Hyper libraries and inspired by Gunicorn.
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Description: Hypercorn
         =========
```

### Comparing `Hypercorn-0.9.4/README.rst` & `Hypercorn-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/artwork/LICENSE` & `Hypercorn-0.9.5/artwork/LICENSE`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/artwork/logo.png` & `Hypercorn-0.9.5/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/artwork/logo.svg` & `Hypercorn-0.9.5/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/artwork/logo_small.png` & `Hypercorn-0.9.5/artwork/logo_small.png`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/artwork/logo_small.svg` & `Hypercorn-0.9.5/artwork/logo_small.svg`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/setup.cfg` & `Hypercorn-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/setup.py` & `Hypercorn-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/Hypercorn.egg-info/PKG-INFO` & `Hypercorn-0.9.5/src/Hypercorn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hypercorn
-Version: 0.9.4
+Version: 0.9.5
 Summary: A ASGI Server based on Hyper libraries and inspired by Gunicorn.
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Description: Hypercorn
         =========
```

### Comparing `Hypercorn-0.9.4/src/Hypercorn.egg-info/SOURCES.txt` & `Hypercorn-0.9.5/src/Hypercorn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 src/hypercorn/typing.py
 src/hypercorn/utils.py
 src/hypercorn/asyncio/__init__.py
 src/hypercorn/asyncio/lifespan.py
 src/hypercorn/asyncio/run.py
 src/hypercorn/asyncio/spawn_app.py
 src/hypercorn/asyncio/statsd.py
+src/hypercorn/asyncio/task_group.py
 src/hypercorn/asyncio/tcp_server.py
 src/hypercorn/asyncio/udp_server.py
 src/hypercorn/protocol/__init__.py
 src/hypercorn/protocol/events.py
 src/hypercorn/protocol/h11.py
 src/hypercorn/protocol/h2.py
 src/hypercorn/protocol/h3.py
```

### Comparing `Hypercorn-0.9.4/src/hypercorn/__main__.py` & `Hypercorn-0.9.5/src/hypercorn/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         "-u", "--user", help="User to own any unix sockets.", default=sentinel, type=int
     )
 
     def _convert_verify_mode(value: str) -> ssl.VerifyMode:
         try:
             return ssl.VerifyMode[value]
         except KeyError:
-            raise argparse.ArgumentTypeError("Not a valid verify mode")
+            raise argparse.ArgumentTypeError(f"'{value}' is not a valid verify mode")
 
     parser.add_argument(
         "--verify-mode",
         help="SSL verify mode for peer's certificate, see ssl.VerifyMode enum for possible values.",
         type=_convert_verify_mode,
         default=sentinel,
     )
@@ -217,14 +217,16 @@
         config.statsd_prefix = args.statsd_prefix
     if args.umask is not sentinel:
         config.umask = args.umask
     if args.user is not sentinel:
         config.user = args.user
     if args.worker_class is not sentinel:
         config.worker_class = args.worker_class
+    if args.verify_mode is not sentinel:
+        config.verify_mode = args.verify_mode
     if args.workers is not sentinel:
         config.workers = args.workers
 
     if len(args.binds) > 0:
         config.bind = args.binds
     if len(args.insecure_binds) > 0:
         config.insecure_bind = args.insecure_binds
```

### Comparing `Hypercorn-0.9.4/src/hypercorn/asyncio/__init__.py` & `Hypercorn-0.9.5/src/hypercorn/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/asyncio/lifespan.py` & `Hypercorn-0.9.5/src/hypercorn/asyncio/lifespan.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/asyncio/run.py` & `Hypercorn-0.9.5/src/hypercorn/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/asyncio/spawn_app.py` & `Hypercorn-0.9.5/src/hypercorn/trio/spawn_app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-import asyncio
 from typing import Awaitable, Callable
 
+import trio
+
 from ..config import Config
 from ..typing import ASGIFramework
 from ..utils import invoke_asgi
 
 
 async def _handle(
     app: ASGIFramework, config: Config, scope: dict, receive: Callable, send: Callable
 ) -> None:
     try:
         await invoke_asgi(app, scope, receive, send)
-    except asyncio.CancelledError:
+    except trio.Cancelled:
         raise
+    except trio.MultiError as error:
+        errors = trio.MultiError.filter(
+            lambda exc: None if isinstance(exc, trio.Cancelled) else exc, root_exc=error
+        )
+        if errors is not None:
+            await config.log.exception("Error in ASGI Framework")
+            await send(None)
+        else:
+            raise
     except Exception:
         await config.log.exception("Error in ASGI Framework")
     finally:
         await send(None)
 
 
 async def spawn_app(
+    nursery: trio._core._run.Nursery,
     app: ASGIFramework,
-    loop: asyncio.AbstractEventLoop,
     config: Config,
     scope: dict,
     send: Callable[[dict], Awaitable[None]],
 ) -> Callable[[dict], Awaitable[None]]:
-    app_queue: asyncio.Queue = asyncio.Queue(config.max_app_queue_size)
-    loop.create_task(_handle(app, config, scope, app_queue.get, send))
-    return app_queue.put
+    app_send_channel, app_receive_channel = trio.open_memory_channel(config.max_app_queue_size)
+    nursery.start_soon(_handle, app, config, scope, app_receive_channel.receive, send)
+    return app_send_channel.send
```

### Comparing `Hypercorn-0.9.4/src/hypercorn/asyncio/statsd.py` & `Hypercorn-0.9.5/src/hypercorn/asyncio/statsd.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/asyncio/tcp_server.py` & `Hypercorn-0.9.5/src/hypercorn/asyncio/tcp_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 from functools import partial
 from typing import Any, Callable, Generator, Optional
 
 from .spawn_app import spawn_app
+from .task_group import TaskGroup
 from ..config import Config
 from ..events import Closed, Event, RawData, Updated
 from ..protocol import ProtocolWrapper
 from ..typing import ASGIFramework
 from ..utils import parse_socket_addr
 
 MAX_RECV = 2 ** 16
@@ -58,28 +59,29 @@
             if ssl_object is not None:
                 ssl = True
                 alpn_protocol = ssl_object.selected_alpn_protocol()
             else:
                 ssl = False
                 alpn_protocol = "http/1.1"
 
-            self.protocol = ProtocolWrapper(
-                self.config,
-                ssl,
-                client,
-                server,
-                self.protocol_send,
-                partial(spawn_app, self.app, self.loop, self.config),
-                EventWrapper,
-                alpn_protocol,
-            )
-            await self.protocol.initiate()
-            self.loop.create_task(self.protocol.send_task())
-            await self._update_keep_alive_timeout()
-            await self._read_data()
+            async with TaskGroup(self.loop) as task_group:
+                self.protocol = ProtocolWrapper(
+                    self.config,
+                    ssl,
+                    client,
+                    server,
+                    self.protocol_send,
+                    partial(spawn_app, task_group, self.app, self.config),
+                    EventWrapper,
+                    alpn_protocol,
+                )
+                await self.protocol.initiate()
+                task_group.spawn(self.protocol.send_task())
+                await self._update_keep_alive_timeout()
+                await self._read_data()
         except OSError:
             pass
         finally:
             await self._close()
 
     async def protocol_send(self, event: Event) -> None:
         if isinstance(event, RawData):
@@ -115,15 +117,15 @@
                     break
                 await self.protocol.handle(RawData(data))
                 await self._update_keep_alive_timeout()
 
     async def _close(self) -> None:
         try:
             self.writer.write_eof()
-        except (NotImplementedError, OSError):
+        except (NotImplementedError, OSError, RuntimeError):
             pass  # Likely SSL connection
 
         try:
             self.writer.close()
             await self.writer.wait_closed()
         except (BrokenPipeError, ConnectionResetError):
             pass  # Already closed
```

### Comparing `Hypercorn-0.9.4/src/hypercorn/asyncio/udp_server.py` & `Hypercorn-0.9.5/src/hypercorn/asyncio/udp_server.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/config.py` & `Hypercorn-0.9.5/src/hypercorn/config.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/logging.py` & `Hypercorn-0.9.5/src/hypercorn/logging.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/middleware.py` & `Hypercorn-0.9.5/src/hypercorn/middleware.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/__init__.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/events.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/events.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/h11.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/h11.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/h2.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/h2.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                 await self.has_data.set()
                 await self.stream_buffers[event.stream_id].drain()
             elif isinstance(event, StreamClosed):
                 await self._close_stream(event.stream_id)
                 await self.send(Updated())
             elif isinstance(event, Request):
                 await self._create_server_push(event.stream_id, event.raw_path, event.headers)
-        except h2.exceptions.ProtocolError:
+        except (KeyError, priority.MissingStreamError, h2.exceptions.ProtocolError):
             # Connection has closed whilst blocked on flow control or
             # connection has advanced ahead of the last emitted event.
             return
 
     async def _handle_events(self, events: List[h2.events.Event]) -> None:
         for event in events:
             if isinstance(event, h2.events.RequestReceived):
```

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/h3.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/h3.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/http_stream.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/http_stream.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/quic.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/protocol/ws_stream.py` & `Hypercorn-0.9.5/src/hypercorn/protocol/ws_stream.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/run.py` & `Hypercorn-0.9.5/src/hypercorn/run.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/statsd.py` & `Hypercorn-0.9.5/src/hypercorn/statsd.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/trio/__init__.py` & `Hypercorn-0.9.5/src/hypercorn/trio/__init__.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/trio/lifespan.py` & `Hypercorn-0.9.5/src/hypercorn/trio/lifespan.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/trio/run.py` & `Hypercorn-0.9.5/src/hypercorn/trio/run.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/trio/tcp_server.py` & `Hypercorn-0.9.5/src/hypercorn/trio/tcp_server.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/trio/udp_server.py` & `Hypercorn-0.9.5/src/hypercorn/trio/udp_server.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/typing.py` & `Hypercorn-0.9.5/src/hypercorn/typing.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/src/hypercorn/utils.py` & `Hypercorn-0.9.5/src/hypercorn/utils.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/assets/cert.pem` & `Hypercorn-0.9.5/tests/assets/cert.pem`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/assets/key.pem` & `Hypercorn-0.9.5/tests/assets/key.pem`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/asyncio/helpers.py` & `Hypercorn-0.9.5/tests/asyncio/helpers.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/asyncio/test_keep_alive.py` & `Hypercorn-0.9.5/tests/asyncio/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/asyncio/test_lifespan.py` & `Hypercorn-0.9.5/tests/asyncio/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/asyncio/test_sanity.py` & `Hypercorn-0.9.5/tests/asyncio/test_sanity.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/asyncio/test_tcp_server.py` & `Hypercorn-0.9.5/tests/asyncio/test_tcp_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 from typing import Callable
 
 import pytest
 
 from hypercorn.asyncio.spawn_app import spawn_app
+from hypercorn.asyncio.task_group import TaskGroup
 from hypercorn.asyncio.tcp_server import TCPServer
 from hypercorn.config import Config
 from .helpers import MemoryReader, MemoryWriter
 from ..helpers import echo_framework
 
 
 @pytest.mark.asyncio
@@ -16,42 +17,62 @@
         while True:
             message = await receive()
             if message is None:
                 return
             await send(message)
 
     app_queue: asyncio.Queue = asyncio.Queue()
-    put = await spawn_app(_echo_app, event_loop, Config(), {"asgi": {}}, app_queue.put)
-    await put({"type": "message"})
-    assert (await app_queue.get()) == {"type": "message"}
-    await put(None)
+    async with TaskGroup(event_loop) as task_group:
+        put = await spawn_app(task_group, _echo_app, Config(), {"asgi": {}}, app_queue.put)
+        await put({"type": "message"})
+        assert (await app_queue.get()) == {"type": "message"}
+        await put(None)
 
 
 @pytest.mark.asyncio
 async def test_spawn_app_error(event_loop: asyncio.AbstractEventLoop) -> None:
     async def _error_app(scope: dict, receive: Callable, send: Callable) -> None:
         raise Exception()
 
     app_queue: asyncio.Queue = asyncio.Queue()
-    await spawn_app(_error_app, event_loop, Config(), {"asgi": {}}, app_queue.put)
+    async with TaskGroup(event_loop) as task_group:
+        await spawn_app(task_group, _error_app, Config(), {"asgi": {}}, app_queue.put)
     assert (await app_queue.get()) is None
 
 
 @pytest.mark.asyncio
 async def test_spawn_app_cancelled(event_loop: asyncio.AbstractEventLoop) -> None:
     async def _error_app(scope: dict, receive: Callable, send: Callable) -> None:
         raise asyncio.CancelledError()
 
     app_queue: asyncio.Queue = asyncio.Queue()
-    await spawn_app(_error_app, event_loop, Config(), {"asgi": {}}, app_queue.put)
-    assert app_queue.empty()
+    with pytest.raises(asyncio.CancelledError):
+        async with TaskGroup(event_loop) as task_group:
+            await spawn_app(task_group, _error_app, Config(), {"asgi": {}}, app_queue.put)
+    assert (await app_queue.get()) is None
 
 
 @pytest.mark.asyncio
 async def test_completes_on_closed(event_loop: asyncio.AbstractEventLoop) -> None:
     server = TCPServer(
         echo_framework, event_loop, Config(), MemoryReader(), MemoryWriter()  # type: ignore
     )
     server.reader.close()  # type: ignore
     await server.run()
     # Key is that this line is reached, rather than the above line
     # hanging.
+
+
+@pytest.mark.asyncio
+async def test_complets_on_half_close(event_loop: asyncio.AbstractEventLoop) -> None:
+    server = TCPServer(
+        echo_framework, event_loop, Config(), MemoryReader(), MemoryWriter()  # type: ignore
+    )
+    asyncio.ensure_future(server.run())
+    await server.reader.send(b"GET / HTTP/1.1\r\nHost: hypercorn\r\n\r\n")  # type: ignore
+    server.reader.close()  # type: ignore
+    await asyncio.sleep(0)
+    data = await server.writer.receive()  # type: ignore
+    assert (
+        data
+        == b"HTTP/1.1 200 \r\ncontent-length: 317\r\ndate: Thu, 01 Jan 1970 01:23:20 GMT\r\nserver: hypercorn-h11\r\n\r\n"  # noqa: E501
+    )
```

### Comparing `Hypercorn-0.9.4/tests/helpers.py` & `Hypercorn-0.9.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/protocol/test_h11.py` & `Hypercorn-0.9.5/tests/protocol/test_h11.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/protocol/test_h2.py` & `Hypercorn-0.9.5/tests/protocol/test_h2.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/protocol/test_http_stream.py` & `Hypercorn-0.9.5/tests/protocol/test_http_stream.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/protocol/test_ws_stream.py` & `Hypercorn-0.9.5/tests/protocol/test_ws_stream.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/test___main__.py` & `Hypercorn-0.9.5/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/test_config.py` & `Hypercorn-0.9.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/test_logging.py` & `Hypercorn-0.9.5/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/test_middleware.py` & `Hypercorn-0.9.5/tests/test_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import pytest
 
 from hypercorn.middleware import DispatcherMiddleware, HTTPToHTTPSRedirectMiddleware
 from .helpers import empty_framework
 
 
 @pytest.mark.asyncio
-@pytest.mark.parametrize(
-    "raw_path", [b"/abc", b"/abc%3C"],
-)
+@pytest.mark.parametrize("raw_path", [b"/abc", b"/abc%3C"])
 async def test_http_to_https_redirect_middleware_http(raw_path: bytes) -> None:
     app = HTTPToHTTPSRedirectMiddleware(empty_framework, "localhost")
     sent_events = []
 
     async def send(message: dict) -> None:
         nonlocal sent_events
         sent_events.append(message)
@@ -28,17 +26,15 @@
             "headers": [(b"location", b"https://localhost%s?a=b" % raw_path)],
         },
         {"type": "http.response.body"},
     ]
 
 
 @pytest.mark.asyncio
-@pytest.mark.parametrize(
-    "raw_path", [b"/abc", b"/abc%3C"],
-)
+@pytest.mark.parametrize("raw_path", [b"/abc", b"/abc%3C"])
 async def test_http_to_https_redirect_middleware_websocket(raw_path: bytes) -> None:
     app = HTTPToHTTPSRedirectMiddleware(empty_framework, "localhost")
     sent_events = []
 
     async def send(message: dict) -> None:
         nonlocal sent_events
         sent_events.append(message)
```

### Comparing `Hypercorn-0.9.4/tests/test_utils.py` & `Hypercorn-0.9.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/trio/test_keep_alive.py` & `Hypercorn-0.9.5/tests/trio/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/trio/test_lifespan.py` & `Hypercorn-0.9.5/tests/trio/test_lifespan.py`

 * *Files identical despite different names*

### Comparing `Hypercorn-0.9.4/tests/trio/test_sanity.py` & `Hypercorn-0.9.5/tests/trio/test_sanity.py`

 * *Files identical despite different names*

