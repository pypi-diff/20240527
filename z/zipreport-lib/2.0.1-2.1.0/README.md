# Comparing `tmp/zipreport-lib-2.0.1.tar.gz` & `tmp/zipreport-lib-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipreport-lib-2.0.1.tar", last modified: Sat May 25 16:26:52 2024, max compression
+gzip compressed data, was "zipreport-lib-2.1.0.tar", last modified: Mon May 27 06:43:13 2024, max compression
```

## Comparing `zipreport-lib-2.0.1.tar` & `zipreport-lib-2.1.0.tar`

### file list

```diff
@@ -1,88 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.094203 zipreport-lib-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/fileutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/basefs.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/basezip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_diskfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_pathcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/fileutils/test_zipfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/processors/test_mime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/render/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16027 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/filters/test_jinjafilters.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/test_jinjaloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/render/test_jinjarender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/report/test_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/tests/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/server/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/zipreport/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/zipreport/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.098203 zipreport-lib-2.0.1/zipreport/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/cli/debug/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/fileutils/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/fileutils/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/backend/zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/diskfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/pathcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/fileutils/zipfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/misc/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/weasyprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/processors/zipreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/report/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/report/reportfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/template/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.102203 zipreport-lib-2.0.1/zipreport/template/jinja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinja/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinjaloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/template/jinjarender.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-25 16:26:46.000000 zipreport-lib-2.0.1/zipreport/zipreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:26:52.106203 zipreport-lib-2.0.1/zipreport_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 16:26:52.000000 zipreport-lib-2.0.1/zipreport_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.711783 zipreport-lib-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-27 06:43:13.711783 zipreport-lib-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-27 06:43:13.711783 zipreport-lib-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.699783 zipreport-lib-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.699783 zipreport-lib-2.1.0/tests/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/fileutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/fileutils/basefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/fileutils/basezip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/fileutils/test_diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/fileutils/test_pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/fileutils/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/fileutils/test_zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.699783 zipreport-lib-2.1.0/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/processors/test_mime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/tests/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/render/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/tests/render/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/render/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16027 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/render/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/render/filters/test_jinjafilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/render/test_jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/render/test_jinjarender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/tests/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/report/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/report/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/report/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/server/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/zipreport/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/zipreport/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/zipreport/cli/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/command/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.703783 zipreport-lib-2.1.0/zipreport/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/debug/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.707783 zipreport-lib-2.1.0/zipreport/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/cli/utils/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.707783 zipreport-lib-2.1.0/zipreport/fileutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/fileutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.707783 zipreport-lib-2.1.0/zipreport/fileutils/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/fileutils/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/fileutils/backend/zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/fileutils/diskfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/fileutils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/fileutils/pathcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/fileutils/zipfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.707783 zipreport-lib-2.1.0/zipreport/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/misc/html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.707783 zipreport-lib-2.1.0/zipreport/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/processors/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/processors/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/processors/weasyprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/processors/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.707783 zipreport-lib-2.1.0/zipreport/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/report/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/report/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/report/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/report/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/report/reportfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.707783 zipreport-lib-2.1.0/zipreport/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.711783 zipreport-lib-2.1.0/zipreport/template/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/template/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/template/jinja/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/template/jinjaloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/template/jinjarender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-27 06:43:05.000000 zipreport-lib-2.1.0/zipreport/zipreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:43:13.711783 zipreport-lib-2.1.0/zipreport_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-27 06:43:13.000000 zipreport-lib-2.1.0/zipreport_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-27 06:43:13.000000 zipreport-lib-2.1.0/zipreport_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:43:13.000000 zipreport-lib-2.1.0/zipreport_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 06:43:13.000000 zipreport-lib-2.1.0/zipreport_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:43:13.000000 zipreport-lib-2.1.0/zipreport_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 06:43:13.000000 zipreport-lib-2.1.0/zipreport_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 06:43:13.000000 zipreport-lib-2.1.0/zipreport_lib.egg-info/top_level.txt
```

### Comparing `zipreport-lib-2.0.1/LICENSE` & `zipreport-lib-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/PKG-INFO` & `zipreport-lib-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: João Pinheiro
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zipreport-lib-2.0.1/README.md` & `zipreport-lib-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/setup.cfg` & `zipreport-lib-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/fileutils/basefs.py` & `zipreport-lib-2.1.0/tests/fileutils/basefs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/fileutils/basezip.py` & `zipreport-lib-2.1.0/tests/fileutils/basezip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/fileutils/test_diskfs.py` & `zipreport-lib-2.1.0/tests/fileutils/test_diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/fileutils/test_pathcache.py` & `zipreport-lib-2.1.0/tests/fileutils/test_pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/fileutils/test_zip.py` & `zipreport-lib-2.1.0/tests/fileutils/test_zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/fileutils/test_zipfs.py` & `zipreport-lib-2.1.0/tests/fileutils/test_zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/processors/base.py` & `zipreport-lib-2.1.0/tests/processors/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/processors/test_mime.py` & `zipreport-lib-2.1.0/tests/processors/test_mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/render/base.py` & `zipreport-lib-2.1.0/tests/render/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/render/filters/base.py` & `zipreport-lib-2.1.0/tests/render/filters/base.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/render/filters/test_jinjafilters.py` & `zipreport-lib-2.1.0/tests/render/filters/test_jinjafilters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/render/test_jinjaloader.py` & `zipreport-lib-2.1.0/tests/render/test_jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/render/test_jinjarender.py` & `zipreport-lib-2.1.0/tests/render/test_jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/report/test_builder.py` & `zipreport-lib-2.1.0/tests/report/test_builder.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/report/test_job.py` & `zipreport-lib-2.1.0/tests/report/test_job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/report/test_loader.py` & `zipreport-lib-2.1.0/tests/report/test_loader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/server/test_server.py` & `zipreport-lib-2.1.0/tests/server/test_server.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/tests/utils.py` & `zipreport-lib-2.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/cli/debug/server.py` & `zipreport-lib-2.1.0/zipreport/cli/debug/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,37 @@
         "/report.html",
         "/report.htm",
     ]
     extensions_map = {
         "": "application/octet-stream",
     }
 
-    def __init__(self, *args, report_path=None, extra_mime_types=None, **kwargs):
+    def __init__(
+        self,
+        *args,
+        report_path=None,
+        extra_mime_types=None,
+        follow_links: bool = False,
+        **kwargs
+    ):
         """
         Constructor
         :param args:
         :param report_path: path of the directory or zpt file to process
         :param extra_mime_types: optional extra mime types to register
+        :param follow_links: if True, follow symlinks
         :param kwargs:
         """
         self.bootstrap_mime_types(extra_mime_types)
         if report_path is None:
             raise RuntimeError("Debug HTTP Server must work with a generated report")
         self.report_path = Path(report_path)
         self.is_report_file = self.report_path.is_file()
         self.enc = sys.getfilesystemencoding()
+        self.follow_links = follow_links
 
         super().__init__(*args, **kwargs)
 
     def bootstrap_mime_types(self, extra_mime_types: dict = None):
         """
         Bootstrap mime types
         :param mime_types: dictionary of entries to add/replace
@@ -80,15 +89,17 @@
         try:
             # load file or build file, according to path
             if self.is_report_file:
                 sys.stdout.write("Reloading report file...\n")
                 _zpt = ReportFileLoader.load_file(self.report_path)
             else:
                 sys.stdout.write("Rebuilding report from path...\n")
-                bresult, zpt = ReportFileBuilder.build_zipfs(self.report_path)
+                bresult, zpt = ReportFileBuilder.build_zipfs(
+                    self.report_path, follow_links=self.follow_links
+                )
                 if not bresult.success():
                     return False, self.error_500(";".join(bresult.get_errors()))
                 # create ReportFile from zipfs
                 _zpt = ReportFileLoader.load_zipfs(zpt)
             # render template to REPORT_FILE_NAME
             # returns a dummy BytesIO object
             JinjaRender(_zpt).render()
@@ -247,17 +258,19 @@
 
     def set_addr(self, addr: str):
         self._addr = addr
 
     def set_port(self, port: int):
         self._port = port
 
-    def run(self, report_path: str):
+    def run(self, report_path: str, follow_links: bool = False) -> None:
         server_address = (self._addr, int(self._port))
-        handler_class = partial(ReportFileHandler, report_path=report_path)
+        handler_class = partial(
+            ReportFileHandler, report_path=report_path, follow_links=follow_links
+        )
         sys.stdout.write(
             "\nStarted debug server at http://{addr}:{port}\nServing from: {path}\nUse Ctrl+C to stop...\n\n".format(
                 addr=self._addr, port=int(self._port), path=Path(report_path).absolute()
             )
         )
         httpd = HTTPServer(server_address, handler_class)
         try:
```

### Comparing `zipreport-lib-2.0.1/zipreport/fileutils/backend/zip.py` & `zipreport-lib-2.1.0/zipreport/fileutils/backend/zip.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/fileutils/diskfs.py` & `zipreport-lib-2.1.0/zipreport/fileutils/diskfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/fileutils/interface.py` & `zipreport-lib-2.1.0/zipreport/fileutils/interface.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/fileutils/pathcache.py` & `zipreport-lib-2.1.0/zipreport/fileutils/pathcache.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/fileutils/zipfs.py` & `zipreport-lib-2.1.0/zipreport/fileutils/zipfs.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/misc/html.py` & `zipreport-lib-2.1.0/zipreport/misc/html.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/processors/mime.py` & `zipreport-lib-2.1.0/zipreport/processors/mime.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/processors/weasyprint.py` & `zipreport-lib-2.1.0/zipreport/processors/weasyprint.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/processors/zipreport.py` & `zipreport-lib-2.1.0/zipreport/processors/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/report/builder.py` & `zipreport-lib-2.1.0/zipreport/report/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,22 +36,23 @@
 class ReportFileBuilder:
     """
     Report building object
     """
 
     @staticmethod
     def build_file(
-        path: str, output_file: str, console=sys.stdout, overwrite: bool = False
+        path: str, output_file: str, console=sys.stdout, overwrite: bool = False, follow_links:bool=False
     ) -> BuildResult:
         """
         Assemble a report file from a specific path
         :param path: report dir path
         :param output_file: destination report file
         :param console: console writer
         :param overwrite: if True, overwrite destination if exists
+        :param follow_links: if True, symlinks are followed
         :return: BuildResult
         """
         status = BuildResult()
         path = Path(path)
         output_file = Path(output_file)
         if output_file.suffix != ZIPREPORT_FILE_EXTENSION:
             output_file = output_file.parent / (
@@ -81,15 +82,15 @@
         else:
             if not output_file.parent.exists():
                 return status.add_error(
                     "Invalid path for output file: '{}'".format(output_file)
                 )
 
         # build ZipFs
-        zfs_status, zfs = ReportFileBuilder.build_zipfs(path, console)
+        zfs_status, zfs = ReportFileBuilder.build_zipfs(path, console, follow_links=follow_links)
         if not zfs_status.success():
             return zfs_status
 
         try:
             # save zpt
             console.write("Generating {}...\n".format(output_file))
             if output_file.exists():
@@ -101,45 +102,49 @@
             return status.add_error("Error saving zpt file: {}".format(e))
 
         console.write("Done!\n")
         return status
 
     @staticmethod
     def build_zipfs(
-        path: str, console=sys.stdout
+        path: str, console=sys.stdout, follow_links=False
     ) -> Tuple[BuildResult, Union[ZipFs, None]]:
         """
         Assemble a ZipFs structure from a specific path
         :param path: report dir path
         :param console: console writer
+        :param follow_links: if true, follow symlinks
         :return: [BuildResult, ZipFs]
         """
         status = BuildResult()
         path = Path(path)
 
         if not path.exists():
             return status.add_error("Path '{}' not found".format(path)), None
 
         if not path.is_dir():
             return status.add_error("Path '{}' is not a directory".format(path)), None
 
+        # inform symlink status
+        console.write("Follow Symlinks: {}\n".format(follow_links))
+
         # try to load & validate manifest
         console.write("Checking manifest & index file...\n")
 
         # valid_zpt() works only on FsInterface
         dfs = DiskFs(path)
         fstatus, _ = ReportFileBuilder.valid_zpt(dfs)
         if not fstatus.success():
             return fstatus, None
 
         # build ZPT and copy files
         console.write("Building...\n")
         zfs = ZipFs(InMemoryZip())
         names = []
-        for dirname, dirs, files in os.walk(path):
+        for dirname, dirs, files in os.walk(path, followlinks=follow_links):
             dirname = Path(dirname)
             for f in files:
                 names.append(dirname / Path(f))
 
         for name in names:
             dest_name = name.relative_to(path)
             console.write("Copying {}...\n".format(dest_name))
```

### Comparing `zipreport-lib-2.0.1/zipreport/report/const.py` & `zipreport-lib-2.1.0/zipreport/report/const.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/report/job.py` & `zipreport-lib-2.1.0/zipreport/report/job.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/report/loader.py` & `zipreport-lib-2.1.0/zipreport/report/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,21 +24,22 @@
         """
         source = Path(source)
         if source.is_dir():
             return ReportFileLoader.load_dir(source)
         return ReportFileLoader.load_file(source)
 
     @staticmethod
-    def load_dir(path: str) -> ReportFile:
+    def load_dir(path: str, follow_links:bool=False) -> ReportFile:
         """
         Generate ReportFile from a directory with a valid report template
         :param path: template path
+        :follow_links: if True, symlinks are followed
         :return: ReportFile
         """
-        zstatus, zfs = ReportFileBuilder.build_zipfs(path, StringIO())
+        zstatus, zfs = ReportFileBuilder.build_zipfs(path, StringIO(), follow_links=follow_links)
         if not zstatus.success():
             error_msg = "; ".join(zstatus.get_errors())
             raise ReportFileLoaderError(
                 "Error loading report from path '{}': '{}'".format(path, error_msg)
             )
         try:
             manifest = json.loads(bytes(zfs.get(MANIFEST_FILE_NAME).getbuffer()))
```

### Comparing `zipreport-lib-2.0.1/zipreport/report/reportfile.py` & `zipreport-lib-2.1.0/zipreport/report/reportfile.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/template/jinja/filters.py` & `zipreport-lib-2.1.0/zipreport/template/jinja/filters.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/template/jinjaloader.py` & `zipreport-lib-2.1.0/zipreport/template/jinjaloader.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/template/jinjarender.py` & `zipreport-lib-2.1.0/zipreport/template/jinjarender.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport/zipreport.py` & `zipreport-lib-2.1.0/zipreport/zipreport.py`

 * *Files identical despite different names*

### Comparing `zipreport-lib-2.0.1/zipreport_lib.egg-info/PKG-INFO` & `zipreport-lib-2.1.0/zipreport_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipreport-lib
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python HTML to PDF reporting engine
 Home-page: https://github.com/zipreport/zipreport
 Author: João Pinheiro
 License: MIT
 Project-URL: Documentation, https://zipreport.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/zipreport/zipreport
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zipreport-lib-2.0.1/zipreport_lib.egg-info/SOURCES.txt` & `zipreport-lib-2.1.0/zipreport_lib.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,27 @@
 tests/server/__init__.py
 tests/server/test_server.py
 zipreport/__init__.py
 zipreport/version.py
 zipreport/zipreport.py
 zipreport/cli/__init__.py
 zipreport/cli/console.py
+zipreport/cli/command/__init__.py
+zipreport/cli/command/base.py
+zipreport/cli/command/build.py
+zipreport/cli/command/debug.py
+zipreport/cli/command/help.py
+zipreport/cli/command/info.py
+zipreport/cli/command/list.py
+zipreport/cli/command/version.py
 zipreport/cli/debug/__init__.py
 zipreport/cli/debug/server.py
+zipreport/cli/utils/__init__.py
+zipreport/cli/utils/argparse.py
+zipreport/cli/utils/console.py
 zipreport/fileutils/__init__.py
 zipreport/fileutils/diskfs.py
 zipreport/fileutils/interface.py
 zipreport/fileutils/pathcache.py
 zipreport/fileutils/zipfs.py
 zipreport/fileutils/backend/__init__.py
 zipreport/fileutils/backend/zip.py
```

