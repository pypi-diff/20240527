# Comparing `tmp/brds-0.4.1.tar.gz` & `tmp/brds-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brds-0.4.1.tar", last modified: Fri Sep  8 17:25:53 2023, max compression
+gzip compressed data, was "brds-0.5.0.tar", last modified: Mon May 27 13:44:34 2024, max compression
```

## Comparing `brds-0.4.1.tar` & `brds-0.5.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-09-08 17:25:43.000000 brds-0.4.1/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-09-08 17:25:43.000000 brds-0.4.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-09-08 17:25:43.000000 brds-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-09-08 17:25:43.000000 brds-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-09-08 17:25:53.138266 brds-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-09-08 17:25:43.000000 brds-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.134266 brds-0.4.1/brds/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-08 17:25:43.000000 brds-0.4.1/brds/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-09-08 17:25:43.000000 brds-0.4.1/brds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-09-08 17:25:43.000000 brds-0.4.1/brds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-09-08 17:25:43.000000 brds-0.4.1/brds/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-09-08 17:25:43.000000 brds-0.4.1/brds/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-09-08 17:25:43.000000 brds-0.4.1/brds/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/core/crawler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/browser_emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/domain_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/root_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/templated_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/crawler/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/core/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/datasets/dataset_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/datasets/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/datasets/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/core/fetch/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/core/fs/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/fs/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/fs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/core/importer/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/importer/gunizp_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/importer/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-09-08 17:25:43.000000 brds-0.4.1/brds/core/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:43.000000 brds-0.4.1/brds/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-09-08 17:25:43.000000 brds-0.4.1/brds/db/init_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/humanize/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-09-08 17:25:43.000000 brds-0.4.1/brds/humanize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-09-08 17:25:43.000000 brds-0.4.1/brds/humanize/sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:43.000000 brds-0.4.1/brds/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/brds/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-09-08 17:25:43.000000 brds-0.4.1/brds/templates/dataset_files.html
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-09-08 17:25:43.000000 brds-0.4.1/brds/templates/datasets.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.134266 brds-0.4.1/brds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-09-08 17:25:53.000000 brds-0.4.1/brds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-09-08 17:25:53.000000 brds-0.4.1/brds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 17:25:53.000000 brds-0.4.1/brds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-09-08 17:25:53.000000 brds-0.4.1/brds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-09-08 17:25:53.000000 brds-0.4.1/brds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-08 17:25:53.000000 brds-0.4.1/brds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 17:25:53.138266 brds-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-09-08 17:25:43.000000 brds-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:53.138266 brds-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 17:25:43.000000 brds-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-09-08 17:25:43.000000 brds-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-08 17:25:43.000000 brds-0.4.1/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.891551 brds-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-27 13:44:25.000000 brds-0.5.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:25.000000 brds-0.5.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-27 13:44:25.000000 brds-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 13:44:25.000000 brds-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-27 13:44:34.891551 brds-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-27 13:44:25.000000 brds-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.879551 brds-0.5.0/brds/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 13:44:25.000000 brds-0.5.0/brds/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 13:44:25.000000 brds-0.5.0/brds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-27 13:44:25.000000 brds-0.5.0/brds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-27 13:44:25.000000 brds-0.5.0/brds/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-27 13:44:25.000000 brds-0.5.0/brds/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-27 13:44:25.000000 brds-0.5.0/brds/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.883551 brds-0.5.0/brds/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.883551 brds-0.5.0/brds/core/crawler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/browser_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/domain_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/pipeline_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/root_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/templated_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/crawler/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds/core/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/datasets/dataset_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/datasets/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/datasets/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds/core/fetch/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds/core/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/fs/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/fs/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds/core/importer/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/importer/gunizp_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/importer/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 13:44:25.000000 brds-0.5.0/brds/core/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:25.000000 brds-0.5.0/brds/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-27 13:44:25.000000 brds-0.5.0/brds/db/init_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds/humanize/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 13:44:25.000000 brds-0.5.0/brds/humanize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-27 13:44:25.000000 brds-0.5.0/brds/humanize/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:25.000000 brds-0.5.0/brds/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-27 13:44:25.000000 brds-0.5.0/brds/templates/dataset_files.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-27 13:44:25.000000 brds-0.5.0/brds/templates/datasets.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/brds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-27 13:44:34.000000 brds-0.5.0/brds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-27 13:44:34.000000 brds-0.5.0/brds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:44:34.000000 brds-0.5.0/brds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 13:44:34.000000 brds-0.5.0/brds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-27 13:44:34.000000 brds-0.5.0/brds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 13:44:34.000000 brds-0.5.0/brds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:44:34.891551 brds-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-27 13:44:25.000000 brds-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:34.887551 brds-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:44:25.000000 brds-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-27 13:44:25.000000 brds-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 13:44:25.000000 brds-0.5.0/tests/test_base.py
```

### Comparing `brds-0.4.1/LICENSE` & `brds-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/__init__.py` & `brds-0.5.0/brds/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/app.py` & `brds-0.5.0/brds/app.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/cli.py` & `brds-0.5.0/brds/cli.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/__init__.py` & `brds-0.5.0/brds/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/crawler/browser_emulator.py` & `brds-0.5.0/brds/core/crawler/browser_emulator.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/crawler/config.py` & `brds-0.5.0/brds/core/crawler/config.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/crawler/variables.py` & `brds-0.5.0/brds/core/crawler/variables.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/datasets/dataset_files.py` & `brds-0.5.0/brds/core/datasets/dataset_files.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/datasets/dataset_info.py` & `brds-0.5.0/brds/core/datasets/dataset_info.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/datasets/list_datasets.py` & `brds-0.5.0/brds/core/datasets/list_datasets.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/edit.py` & `brds-0.5.0/brds/core/edit.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/environment.py` & `brds-0.5.0/brds/core/environment.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/fetch/fetcher.py` & `brds-0.5.0/brds/core/fetch/fetcher.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/fs/reader.py` & `brds-0.5.0/brds/core/fs/reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             return _join(self._folder, _listdir(self._folder)[0])
         return _join(self._folder, filename)
 
     @classmethod
     def from_environment(cls: _Type[T], subfolder: str) -> T:
         return cls(_join(_reader_folder_path(), subfolder))
 
-    def load(self: "FileReader", filename: _Optional[str] = None) -> _Any:
+    def load(self: "FileReader", filename: _Optional[str] = None, *args, **kwargs) -> _Any:
         new_file_name = self.get(filename)
         if filename:
             LOGGER.debug(
                 "Latest file for folder '%s' (with filename='%s') resolved to '%s'.",
                 self._root_folder,
                 filename,
                 new_file_name,
@@ -60,20 +60,20 @@
             LOGGER.debug(
                 "Latest file for folder '%s' resolved to '%s'.",
                 self._root_folder,
                 new_file_name,
             )
         if new_file_name.endswith(".json"):
             with open(new_file_name) as input_file:
-                return _load(input_file)
+                return _load(input_file, *args, **kwargs)
         if new_file_name.endswith(".parquet"):
-            return _read_parquet(new_file_name)
+            return _read_parquet(new_file_name, *args, **kwargs)
         if new_file_name.endswith(".html"):
             try:
-                return _read_html(new_file_name)
+                return _read_html(new_file_name, *args, **kwargs)
             except ValueError as ve:
                 raise ValueError(f"Error parsing HTML from '{new_file_name}'") from ve
         raise NotImplementedError(f"Do not know how to load the file `{filename}`: `{new_file_name}`")
 
 
 def _last_folder(folder: str) -> str:
     return _join(folder, sorted(_listdir(folder), reverse=True)[0])
```

### Comparing `brds-0.4.1/brds/core/fs/writer.py` & `brds-0.5.0/brds/core/fs/writer.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/importer/gunizp_importer.py` & `brds-0.5.0/brds/core/importer/gunizp_importer.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/core/logger.py` & `brds-0.5.0/brds/core/logger.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/db/init_db.py` & `brds-0.5.0/brds/db/init_db.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/humanize/sizes.py` & `brds-0.5.0/brds/humanize/sizes.py`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/templates/dataset_files.html` & `brds-0.5.0/brds/templates/dataset_files.html`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds/templates/datasets.html` & `brds-0.5.0/brds/templates/datasets.html`

 * *Files identical despite different names*

### Comparing `brds-0.4.1/brds.egg-info/SOURCES.txt` & `brds-0.5.0/brds.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 brds/core/security.py
 brds/core/vault.py
 brds/core/crawler/__init__.py
 brds/core/crawler/browser_emulator.py
 brds/core/crawler/config.py
 brds/core/crawler/crawler.py
 brds/core/crawler/domain_rate_limiter.py
+brds/core/crawler/pipeline_crawl.py
 brds/core/crawler/root_crawler.py
 brds/core/crawler/templated_url.py
 brds/core/crawler/variables.py
 brds/core/datasets/__init__.py
 brds/core/datasets/dataset_files.py
 brds/core/datasets/dataset_info.py
 brds/core/datasets/list_datasets.py
```

### Comparing `brds-0.4.1/setup.py` & `brds-0.5.0/setup.py`

 * *Files identical despite different names*

