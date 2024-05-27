# Comparing `tmp/alphaz-next-0.7.3.3.tar.gz` & `tmp/alphaz-next-0.7.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.7.3.3.tar", last modified: Thu May 23 08:36:23 2024, max compression
+gzip compressed data, was "alphaz-next-0.7.3.4.tar", last modified: Mon May 27 10:50:36 2024, max compression
```

## Comparing `alphaz-next-0.7.3.3.tar` & `alphaz-next-0.7.3.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.524413 alphaz-next-0.7.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.512413 alphaz-next-0.7.3.3/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.516413 alphaz-next-0.7.3.3/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/asyncio/async_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.516413 alphaz-next-0.7.3.3/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.516413 alphaz-next-0.7.3.3/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.516413 alphaz-next-0.7.3.3/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/core/responses/ujson_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.516413 alphaz-next-0.7.3.3/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/models/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/models/config/openapi_config_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/tests/utils/mocking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26157 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.520413 alphaz-next-0.7.3.3/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/utils/logging_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/alphaz_next/utils/loguru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:36:23.516413 alphaz-next-0.7.3.3/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-23 08:36:23.000000 alphaz-next-0.7.3.3/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-23 08:36:23.000000 alphaz-next-0.7.3.3/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:36:23.000000 alphaz-next-0.7.3.3/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 08:36:23.000000 alphaz-next-0.7.3.3/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 08:36:23.000000 alphaz-next-0.7.3.3/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-23 08:36:17.000000 alphaz-next-0.7.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:36:23.524413 alphaz-next-0.7.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 08:36:21.000000 alphaz-next-0.7.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.206736 alphaz-next-0.7.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-27 10:50:36.206736 alphaz-next-0.7.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.194736 alphaz-next-0.7.3.4/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.198737 alphaz-next-0.7.3.4/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/asyncio/async_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.198737 alphaz-next-0.7.3.4/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.198737 alphaz-next-0.7.3.4/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.198737 alphaz-next-0.7.3.4/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-27 10:50:28.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/core/responses/ujson_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/models/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/models/config/openapi_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/tests/utils/mocking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26241 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.202736 alphaz-next-0.7.3.4/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/utils/logging_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/alphaz_next/utils/loguru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 10:50:36.198737 alphaz-next-0.7.3.4/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-27 10:50:36.000000 alphaz-next-0.7.3.4/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-27 10:50:36.000000 alphaz-next-0.7.3.4/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 10:50:36.000000 alphaz-next-0.7.3.4/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-27 10:50:36.000000 alphaz-next-0.7.3.4/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 10:50:36.000000 alphaz-next-0.7.3.4/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-27 10:50:29.000000 alphaz-next-0.7.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 10:50:36.206736 alphaz-next-0.7.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-27 10:50:33.000000 alphaz-next-0.7.3.4/setup.py
```

### Comparing `alphaz-next-0.7.3.3/PKG-INFO` & `alphaz-next-0.7.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.3.3
+Version: 0.7.3.4
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.3.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.3.3/README.md` & `alphaz-next-0.7.3.4/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/asyncio/async_database.py` & `alphaz-next-0.7.3.4/alphaz_next/asyncio/async_database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/auth/auth.py` & `alphaz-next-0.7.3.4/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/_base.py` & `alphaz-next-0.7.3.4/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/_middleware.py` & `alphaz-next-0.7.3.4/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/_telemetry.py` & `alphaz-next-0.7.3.4/alphaz_next/core/_telemetry.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/application.py` & `alphaz-next-0.7.3.4/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.7.3.4/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/exceptions.py` & `alphaz-next-0.7.3.4/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.7.3.4/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/libs/httpx.py` & `alphaz-next-0.7.3.4/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/api_config.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/database_config.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.7.3.4/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.7.3.4/alphaz_next/tests/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,47 +699,47 @@
 
 
 def load_expected_data(
     saved_dir_path: _Optional[_Path] = None,
     saved_file_path: _Optional[str] = None,
     format: str = "json",
     encoding: str = "utf-8",
-) -> _Callable[[_Callable[_P, _Any]], _Callable[_P, _Any]]:
+) -> _Callable[[_Callable[_P, _T]], _Callable[_P, _T]]:
 
-    def decorator(func: _Callable[_P, _Any]) -> _Callable[_P, _Any]:
+    def decorator(func: _Callable[_P, _T]) -> _Callable[_P, _T]:
 
-        def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _Any:
+        def wrapper(*args: _P.args, **kwargs: _P.kwargs) -> _T:
             qualname = func.__qualname__
             if "." not in qualname:
                 raise ValueError("The function must be a method of a class")
 
-            if saved_dir_path is None:
-                return
+            if saved_dir_path is not None:
+                file_path = (
+                    saved_dir_path / f"{qualname.replace('.', '__')}.{format}"
+                    if saved_file_path is None
+                    else saved_dir_path / saved_file_path
+                )
+
+                expected_data: _Union[
+                    _List[_Dict[str, _Any]], _Dict[str, _Any], bytes
+                ] = {}
+                if _os.path.exists(file_path):
+                    with open(file_path, encoding=encoding) as file:
+                        match format:
+                            case "json":
+                                expected_data = _cast(
+                                    _Union[_List[_Dict[str, _Any]], _Dict[str, _Any]],
+                                    _json.load(file),
+                                )
+                            case "txt":
+                                expected_data_str = file.read()
+                                expected_data = expected_data_str.encode(encoding)
 
-            file_path = (
-                saved_dir_path / f"{qualname.replace('.', '__')}.{format}"
-                if saved_file_path is None
-                else saved_dir_path / saved_file_path
-            )
-
-            expected_data: _Union[_List[_Dict[str, _Any]], _Dict[str, _Any], bytes] = {}
-            if _os.path.exists(file_path):
-                with open(file_path, encoding=encoding) as file:
-                    match format:
-                        case "json":
-                            expected_data = _cast(
-                                _Union[_List[_Dict[str, _Any]], _Dict[str, _Any]],
-                                _json.load(file),
-                            )
-                        case "txt":
-                            expected_data_str = file.read()
-                            expected_data = expected_data_str.encode(encoding)
-
-            kwargs["expected_data"] = expected_data
-            kwargs["saved_path"] = file_path
+                kwargs["expected_data"] = expected_data
+                kwargs["saved_path"] = file_path
 
             data = func(*args, **kwargs)
 
             return data
 
         return wrapper
```

### Comparing `alphaz-next-0.7.3.3/alphaz_next/utils/database.py` & `alphaz-next-0.7.3.4/alphaz_next/utils/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/utils/format.py` & `alphaz-next-0.7.3.4/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/utils/logger.py` & `alphaz-next-0.7.3.4/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.7.3.4/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next/utils/loguru.py` & `alphaz-next-0.7.3.4/alphaz_next/utils/loguru.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.7.3.4/alphaz_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.7.3.3
+Version: 0.7.3.4
 Summary: A project to make a lib to start FastAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.3.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.7.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: Maxime MARTIN <maxime.martin02@hotmail.fr>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.7.3.3/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.7.3.4/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.7.3.3/setup.py` & `alphaz-next-0.7.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "0.7.3.3"
+version = "0.7.3.4"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

