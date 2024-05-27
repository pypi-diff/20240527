# Comparing `tmp/civitdl-2.0.9.tar.gz` & `tmp/civitdl-2.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civitdl-2.0.9.tar", last modified: Fri Jan 26 13:26:13 2024, max compression
+gzip compressed data, was "civitdl-2.1.0.dev1.tar", last modified: Mon May 27 19:49:05 2024, max compression
```

## Comparing `civitdl-2.0.9.tar` & `civitdl-2.1.0.dev1.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.577771 civitdl-2.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-01-26 13:26:05.000000 civitdl-2.0.9/License
--rw-r--r--   0 runner    (1001) docker     (127)    19322 2024-01-26 13:26:13.577771 civitdl-2.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-01-26 13:26:05.000000 civitdl-2.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-26 13:26:05.000000 civitdl-2.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-26 13:26:05.000000 civitdl-2.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 13:26:13.577771 civitdl-2.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-26 13:26:05.000000 civitdl-2.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.569771 civitdl-2.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.569771 civitdl-2.0.9/src/civitconfig/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.569771 civitdl-2.0.9/src/civitconfig/args/
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/args/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.569771 civitdl-2.0.9/src/civitconfig/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.573771 civitdl-2.0.9/src/civitconfig/data/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/data/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/data/config/aliasconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/data/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/data/config/defaultconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/data/config/sorterconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitconfig/data/configmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.573771 civitdl-2.0.9/src/civitdl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitdl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.573771 civitdl-2.0.9/src/civitdl/api/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitdl/api/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.573771 civitdl-2.0.9/src/civitdl/args/
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitdl/args/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.573771 civitdl-2.0.9/src/civitdl/batch/
--rw-r--r--   0 runner    (1001) docker     (127)    13836 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitdl/batch/_get_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/civitdl/batch/batch_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.577771 civitdl-2.0.9/src/civitdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19322 2024-01-26 13:26:13.000000 civitdl-2.0.9/src/civitdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-01-26 13:26:13.000000 civitdl-2.0.9/src/civitdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 13:26:13.000000 civitdl-2.0.9/src/civitdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-26 13:26:13.000000 civitdl-2.0.9/src/civitdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-26 13:26:13.000000 civitdl-2.0.9/src/civitdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-26 13:26:13.000000 civitdl-2.0.9/src/civitdl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.577771 civitdl-2.0.9/src/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/hashmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.577771 civitdl-2.0.9/src/helpers/sorter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/sorter/__Init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/sorter/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/sorter/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/sorter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/sourcemanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/styler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:13.577771 civitdl-2.0.9/src/helpers/vars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/vars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-26 13:26:05.000000 civitdl-2.0.9/src/helpers/vars/program_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/License
+-rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/args/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.425564 civitdl-2.1.0.dev1/src/civitconfig/data/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/aliasconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/defaultconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/config/sorterconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitconfig/data/configmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/api/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/args/
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/args/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/civitdl/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/batch/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/batch/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/civitdl/batch/batch_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/civitdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19335 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 19:49:05.000000 civitdl-2.1.0.dev1/src/civitdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.429564 civitdl-2.1.0.dev1/src/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/helpers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/__Init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/helpers/core/_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/_ui/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/_ui/styler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/iohelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/hashmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:05.433564 civitdl-2.1.0.dev1/src/helpers/sorter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/__Init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sorter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-27 19:49:01.000000 civitdl-2.1.0.dev1/src/helpers/sourcemanager.py
```

### Comparing `civitdl-2.0.9/License` & `civitdl-2.1.0.dev1/License`

 * *Files identical despite different names*

### Comparing `civitdl-2.0.9/PKG-INFO` & `civitdl-2.1.0.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civitdl
-Version: 2.0.9
+Version: 2.1.0.dev1
 Summary: Package for batch downloading models from civitai.com
 Author: Owen Truong
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,18 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Repository, https://github.com/OwenTruong/civitdl
 Project-URL: Bug Tracker, https://github.com/OwenTruong/civitdl/issues
 Keywords: civitai,batch download
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: tqdm<5,>=4.66.1
 Requires-Dist: appdirs<2,>=1.4.4
 Requires-Dist: argparse<2,>=1.4
 
 # civitdl (civitai-batch-download)
@@ -223,16 +223,14 @@
 (QUICK NOTE: CivitAI seems to have changed their API so that it will require an API key for all model downloads, please see [API Key Page](/doc/api_key.md) for instructions)
 
 **Note v2 has some changes regarding the cli args of the program. Please read the README below or run `civitdl --help` for the new arguments!**
 - To see changes to v2, go to [Changes in v2](#changes-in-v2-from-v1) section.
 
 Uses CLI to batch download Stable Diffusion models, metadata (including description of model, author, base model, example prompts and etc.) and example images (default is 3) of checkpoints, loras, and TI models from civitai!
 
-One thing to note is that for sfw models, currently, the program is set to only download sfw images. Please note that there may be sfw models that are rated as nsfw by CivitAI (and vice versa).
-
 <br/>
 
 ## Navigate
 - [README Page](/README.md)
 - [Alias Page](/doc/alias.md)
 - [API Key Page](/doc/api_key.md)
 - [Civitconfig / Configuration Page](/doc/civitconfig.md)
@@ -245,60 +243,77 @@
 - [civitdl (civitai-batch-download)](#civitdl-civitai-batch-download)
   - [Navigate](#navigate)
   - [Table Of Contents](#table-of-contents)
   - [Getting Started](#getting-started)
     - [Dependencies](#dependencies)
     - [Installing](#installing)
       - [Install using PIP](#install-using-pip)
-      - [Build from source](#build-from-source)
+      - [Build from source 1](#build-from-source-1)
+      - [Build from source 2 (if the instruction above fails with UNKNOWN package installed, else ignore this section)](#build-from-source-2-if-the-instruction-above-fails-with-unknown-package-installed-else-ignore-this-section)
     - [Quick Start](#quick-start)
       - [Configuration Program Options - civitconfig](#configuration-program-options---civitconfig)
   - [Changes in v2 from v1](#changes-in-v2-from-v1)
   - [Troubleshooting](#troubleshooting)
   - [Contributing](#contributing)
   - [License](#license)
 
 <br/>
 
 ## Getting Started
 
 ### Dependencies
-* Python3
+* Python3.8 or above
 * `requirements.txt`
 
 <br/>
 
 ### Installing
 
 #### Install using PIP
 ```bash
-pip3 install civitdl
+pip3 install civitdl 
+# pip install civitdl # if pip3 is not found
 ```
-- Use `pip install civitdl` if `pip3` is not found.
 
 <br/>
 
-#### Build from source
+#### Build from source 1
 ```bash
 git clone https://github.com/OwenTruong/civitdl.git # Clone the project
 cd civitdl # CD into project directory
-make install # Now program is installed globally unless you are using a virtual env
-# make install2 # Run this if make install fails
+pip3 install . # Use pip if pip3 is not found
+```
+
+<br />
+
+#### Build from source 2 (if the instruction above fails with UNKNOWN package installed, else ignore this section)
+```bash
+# Make sure you are in project directory # use pip if pip3 is not found
+python3 -m build
+pip3 install -r ./requirements.txt
+pip3 install --upgrade dist/*.whl
 ```
+<br />
+
 
 ### Quick Start
 To get started quickly, copy the command below.
 - See [civitdl doc](/doc/civitdl.md) for more info.
 
 ``` bash
 civitdl 123456 ./models
 ```
-- Replace `123456` your model of choice (it can be a civitai.com url or model id).
+- Replace `123456` with your model of choice (it can be a civitai.com url or model id).
 - Replace `./models` with the directory you wish to download the model to.
 
+Example with url:
+```bash
+civitdl https://civitai.com/models/123456 ./models
+```
+
 <br/>
 
 #### Configuration Program Options - civitconfig
 - Configuring the program might make your life easier. You would be able to set default sorter, max images, and api key to use without running any of those options in the main program!
   - You would also be able to add and delete sorters and aliases from the program.
   - Check [civitconfig doc](/doc/civitconfig.md).
 - Run `civitconfig --help` to check what options are available!
@@ -340,18 +355,14 @@
 
 For Windows, this may help: https://www.computerhope.com/issues/ch000549.htm
 
 If you are building from source and the following packages are not available `setuptools, wheel, build`, please install them with `pip install setuptools wheel build`
 
 ------
 
-If you are building the project and python unsuccessfully installs the program with `make install`, and displays the package's name as `UNKNOWN`, it is likely because you are trying to install the package globally. Either run `make install2` or use virtual env `python -m venv venv && source ./venv/bin/activate && make install`.
-
-------
-
 <br/>
 
 
 
 ## Contributing
 
 Thanks for the interest in the project!
```

### Comparing `civitdl-2.0.9/README.md` & `civitdl-2.1.0.dev1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 (QUICK NOTE: CivitAI seems to have changed their API so that it will require an API key for all model downloads, please see [API Key Page](/doc/api_key.md) for instructions)
 
 **Note v2 has some changes regarding the cli args of the program. Please read the README below or run `civitdl --help` for the new arguments!**
 - To see changes to v2, go to [Changes in v2](#changes-in-v2-from-v1) section.
 
 Uses CLI to batch download Stable Diffusion models, metadata (including description of model, author, base model, example prompts and etc.) and example images (default is 3) of checkpoints, loras, and TI models from civitai!
 
-One thing to note is that for sfw models, currently, the program is set to only download sfw images. Please note that there may be sfw models that are rated as nsfw by CivitAI (and vice versa).
-
 <br/>
 
 ## Navigate
 - [README Page](/README.md)
 - [Alias Page](/doc/alias.md)
 - [API Key Page](/doc/api_key.md)
 - [Civitconfig / Configuration Page](/doc/civitconfig.md)
@@ -25,60 +23,77 @@
 - [civitdl (civitai-batch-download)](#civitdl-civitai-batch-download)
   - [Navigate](#navigate)
   - [Table Of Contents](#table-of-contents)
   - [Getting Started](#getting-started)
     - [Dependencies](#dependencies)
     - [Installing](#installing)
       - [Install using PIP](#install-using-pip)
-      - [Build from source](#build-from-source)
+      - [Build from source 1](#build-from-source-1)
+      - [Build from source 2 (if the instruction above fails with UNKNOWN package installed, else ignore this section)](#build-from-source-2-if-the-instruction-above-fails-with-unknown-package-installed-else-ignore-this-section)
     - [Quick Start](#quick-start)
       - [Configuration Program Options - civitconfig](#configuration-program-options---civitconfig)
   - [Changes in v2 from v1](#changes-in-v2-from-v1)
   - [Troubleshooting](#troubleshooting)
   - [Contributing](#contributing)
   - [License](#license)
 
 <br/>
 
 ## Getting Started
 
 ### Dependencies
-* Python3
+* Python3.8 or above
 * `requirements.txt`
 
 <br/>
 
 ### Installing
 
 #### Install using PIP
 ```bash
-pip3 install civitdl
+pip3 install civitdl 
+# pip install civitdl # if pip3 is not found
 ```
-- Use `pip install civitdl` if `pip3` is not found.
 
 <br/>
 
-#### Build from source
+#### Build from source 1
 ```bash
 git clone https://github.com/OwenTruong/civitdl.git # Clone the project
 cd civitdl # CD into project directory
-make install # Now program is installed globally unless you are using a virtual env
-# make install2 # Run this if make install fails
+pip3 install . # Use pip if pip3 is not found
+```
+
+<br />
+
+#### Build from source 2 (if the instruction above fails with UNKNOWN package installed, else ignore this section)
+```bash
+# Make sure you are in project directory # use pip if pip3 is not found
+python3 -m build
+pip3 install -r ./requirements.txt
+pip3 install --upgrade dist/*.whl
 ```
+<br />
+
 
 ### Quick Start
 To get started quickly, copy the command below.
 - See [civitdl doc](/doc/civitdl.md) for more info.
 
 ``` bash
 civitdl 123456 ./models
 ```
-- Replace `123456` your model of choice (it can be a civitai.com url or model id).
+- Replace `123456` with your model of choice (it can be a civitai.com url or model id).
 - Replace `./models` with the directory you wish to download the model to.
 
+Example with url:
+```bash
+civitdl https://civitai.com/models/123456 ./models
+```
+
 <br/>
 
 #### Configuration Program Options - civitconfig
 - Configuring the program might make your life easier. You would be able to set default sorter, max images, and api key to use without running any of those options in the main program!
   - You would also be able to add and delete sorters and aliases from the program.
   - Check [civitconfig doc](/doc/civitconfig.md).
 - Run `civitconfig --help` to check what options are available!
@@ -120,18 +135,14 @@
 
 For Windows, this may help: https://www.computerhope.com/issues/ch000549.htm
 
 If you are building from source and the following packages are not available `setuptools, wheel, build`, please install them with `pip install setuptools wheel build`
 
 ------
 
-If you are building the project and python unsuccessfully installs the program with `make install`, and displays the package's name as `UNKNOWN`, it is likely because you are trying to install the package globally. Either run `make install2` or use virtual env `python -m venv venv && source ./venv/bin/activate && make install`.
-
-------
-
 <br/>
 
 
 
 ## Contributing
 
 Thanks for the interest in the project!
```

### Comparing `civitdl-2.0.9/pyproject.toml` & `civitdl-2.1.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 
 requires = [ "setuptools", "wheel", "build" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "civitdl"
-version = "2.0.9"
+version = "2.1.0.dev1"
 authors = [ 
    { name = "Owen Truong" } 
 ]
 description = "Package for batch downloading models from civitai.com"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "License"}
 keywords = ["civitai", "batch download"]
 classifiers = [
-   "Programming Language :: Python :: 3.7",
+   "Programming Language :: Python :: 3.8",
    "License :: OSI Approved :: MIT License",
    "Operating System :: OS Independent"
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

### Comparing `civitdl-2.0.9/src/civitconfig/__main__.py` & `civitdl-2.1.0.dev1/src/civitconfig/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 #!/usr/bin/env python3
 
-import sys
 import traceback
-from operator import itemgetter
 
-from helpers.styler import Styler
-from helpers.exceptions import UnexpectedException
-from helpers.utils import set_verbose, run_verbose, print_verbose, print_exc, DefaultOptions
+from helpers.core.utils import disable_style, UnexpectedException, set_verbose, run_verbose, print_verbose, print_exc, sprint
+from helpers.options import DefaultOptions
 from civitconfig.args.argparser import get_args
 from civitconfig.data.configmanager import ConfigManager
 
+# TODO: Make verbose and no_style similar to each other
+
 
 def main():
     try:
         args = get_args()
         if args['verbose']:
             set_verbose(True)
         else:
             set_verbose(False)
 
+        if args['with_color'] == False:
+            disable_style()
+
         config_manager = ConfigManager()
         subcommand = args['subcommand']
         print_verbose(args)
 
         if subcommand == 'default':
             args.pop('subcommand')
             config_manager.setDefault(DefaultOptions(
                 sorter=args['sorter'],
                 max_images=args['max_images'],
+                nsfw_mode=args['nsfw_mode'],
                 api_key=args['api_key'],
                 with_prompt=args['with_prompt'],
                 without_model=args['without_model'],
                 limit_rate=args['limit_rate'],
                 retry_count=args['retry_count'],
                 pause_time=args['pause_time'],
                 cache_mode=args['cache_mode'],
-                model_overwrite=args['model_overwrite']
+                model_overwrite=args['model_overwrite'],
+                with_color=args['with_color']
             ))
             config_manager.print_defaults()
         elif subcommand == 'sorter':
             if args['add'] != None:
                 add_name, add_path = args['add']
                 config_manager.addSorter(add_name, add_path)
             elif args['delete'] != None:
@@ -58,11 +62,11 @@
             elif args['download'] != None:
                 config_manager.download(args['download'])
         else:
             raise UnexpectedException(
                 'Unknown subcommand not caught by argparse')
 
     except Exception as e:
-        print('---------')
+        sprint('---------')
         run_verbose(traceback.print_exc)
         print_exc(e)
-        print('---------')
+        sprint('---------')
```

### Comparing `civitdl-2.0.9/src/civitconfig/args/argparser.py` & `civitdl-2.1.0.dev1/src/civitconfig/args/argparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import re
 from typing import Dict, List, Union
 
 import argparse
 
-from helpers.styler import Styler
-from helpers.exceptions import InputException, UnexpectedException
-from helpers.argparse import PwdAction, ConfirmAction, ColoredArgParser
-from helpers.utils import get_version, print_verbose
+from helpers.core.utils import get_version
+from helpers.argparse import PwdAction, ConfirmAction, ColoredArgParser, BooleanOptionalAction
 
 __all__ = ['get_args']
 
 
 def add_shared_option(par):
     par.add_argument(
-        '--verbose', action=argparse.BooleanOptionalAction, help='Prints out traceback and other useful information.')
+        '--with-color', action=BooleanOptionalAction, help='Enable styles like colors, background colors and bold/italized texts.'
+    )
+    par.add_argument(
+        '--verbose', action=BooleanOptionalAction, help='Prints out traceback and other useful information.')
     par.add_argument(
         '-v', '--version', action='version', version=f'civitdl v{get_version()}', help='Prints out the version of the program.'
     )
 
 
 parser = ColoredArgParser(
     prog='civitconfig',
@@ -34,24 +35,27 @@
 
 default_parser = subparsers.add_parser(
     'default', help='Set a default value for one of the options below.\nIf no options are provided, default will print the current default.')
 
 default_parser.add_argument('-i', '--max-images', metavar='INT', type=int,
                             help='Set the default max number of images to download per model.')
 
+default_parser.add_argument('--nsfw-mode', type=str,
+                            help='Set the default nsfw mode when downloading images. Setting to 0 means the program will only download sfw. Setting to 1 means the program will download sfw, and nsfw images depending on the nsfw rating of the model. Setting to 2 means the program will download both sfw and nsfw.')
+
 default_parser.add_argument('-s', '--sorter', metavar='NAME', type=str,
                             help='Set the default sorter given name of sorter (filepath not accepted).')
 
 default_parser.add_argument('-k', '--api-key', action=PwdAction, type=str, required=False, nargs='?',
                             help='Prompts the user for their api key to use for model downloads that require users to log in.')
 
-default_parser.add_argument('--with-prompt', action=argparse.BooleanOptionalAction,
+default_parser.add_argument('--with-prompt', action=BooleanOptionalAction,
                             help='Toggles default behavior on whether to download prompt alongside images.')
 
-default_parser.add_argument('--without-model', action=argparse.BooleanOptionalAction,
+default_parser.add_argument('--without-model', action=BooleanOptionalAction,
                             help='Toggles default behavior on whether to download model or not.')
 
 default_parser.add_argument('--limit-rate', type=str,
                             help='Set the default limit for the download speed/rate of resources downloaded from CivitAI. Set it to 0 to disable limit.'
                             )
 
 default_parser.add_argument('--retry-count', type=int,
@@ -59,15 +63,15 @@
                             )
 
 default_parser.add_argument('--pause-time', type=float,
                             help='Set the default number of seconds to pause between each model\'s download'
                             )
 default_parser.add_argument('--cache-mode', type=str,
                             help='Set the default cache mode. Valid modes are 0 and 1 for now. 2 is not implemented yet.')
-default_parser.add_argument('--model-overwrite', action=argparse.BooleanOptionalAction,
+default_parser.add_argument('--model-overwrite', action=BooleanOptionalAction,
                             help='Set the default behavior on whether to overwrite or skip models that are already downloaded at path. model=overwrite to overwrite model. no-model-overwrite to skip model.')
 add_shared_option(default_parser)
 
 
 sorter_parser = subparsers.add_parser(
     'sorter', help='Sorter-related subcommand.\nCurrently supports listing, adding and deleting sorters.\nIf no options are provided, sorter will list all available sorters.\nExample usage: civitdl 123456 ./lora --sorter mysorter.',
     formatter_class=argparse.RawTextHelpFormatter
```

### Comparing `civitdl-2.0.9/src/civitconfig/data/config/aliasconfig.py` & `civitdl-2.1.0.dev1/src/civitconfig/data/config/aliasconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from helpers.exceptions import InputException
+from helpers.core.utils import InputException
 from .config import Config
 
 
 class AliasConfig(Config):
 
     def __init__(self, *args):
         super(AliasConfig, self).__init__(*args)
```

### Comparing `civitdl-2.0.9/src/civitconfig/data/config/config.py` & `civitdl-2.1.0.dev1/src/civitconfig/data/config/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 import os
 import json
 from datetime import datetime
 import shutil
 from typing import Dict, List, Union
 
 from helpers.sorter import basic, tags
-from helpers.exceptions import UnexpectedException
-from helpers.styler import Styler
-from helpers.utils import getDate
-from helpers.validation import Validation
+from helpers.core.utils import Styler, UnexpectedException, getDate, sprint
+from helpers.core._validation import Validation
 
 DEFAULT_CONFIG = {
     "version": "1",
     "default": {
         "sorter": "basic",
         "max_images": 3,
+        "nsfw_mode": "2",
         "api_key": "",
 
         "with_prompt": True,
         "without_model": False,
         "limit_rate": '0',
         "retry_count": 3,
         "pause_time": 3.0,
 
         "cache_mode": '1',
-        "model_overwrite": False
+        "model_overwrite": False,
+
+        "with_color": True
     },
     "sorters": [["basic", basic.sort_model.__doc__, 'basic'], ["tags", tags.sort_model.__doc__, 'tags']],
     "aliases": [["@example", "~/.models"]]
 }
 
 
 CURRENT_VERSION = "1"
@@ -92,29 +93,29 @@
         return self._getConfig()['sorters']
 
     def getAliasesList(self) -> List:
         return self._getConfig()['aliases']
 
     def print_defaults(self):
         blacklisted_keys = ['api_key']
-        print(Styler.stylize('Default:', color='main'))
+        sprint(Styler.stylize('Default:', color='main'))
         for key, value in self.getDefault().items():
             if key in blacklisted_keys:
                 continue
             key = key.replace('_', ' ').title()
-            print(Styler.stylize(
-                f'     {key}:  { "N/A" if str(value) == "" else value }', color='main'))
+            sprint(Styler.stylize(
+                f'     {key}:  {"N/A" if str(value) == "" else value}', color='main'))
 
     def print_sorters(self):
         for i, [name, docstr, _] in enumerate(self.getSortersList()):
-            print(
+            sprint(
                 Styler.stylize(
                     f'Sorter #{i + 1}, "{name}":  {f"{docstr[:300 - 3]}..." if len(docstr) > 300 else docstr}', color='main')
             )
 
     def print_aliases(self):
         for i, [alias_name, path] in enumerate(self.getAliasesList()):
-            print(
+            sprint(
                 Styler.stylize(
                     f'Alias #{i + 1}, "{alias_name}":  {path}', color='main'
                 )
             )
```

### Comparing `civitdl-2.0.9/src/civitconfig/data/config/defaultconfig.py` & `civitdl-2.1.0.dev1/src/civitconfig/data/config/defaultconfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from helpers.exceptions import InputException, UnexpectedException
-from helpers.utils import BatchOptions, DefaultOptions
+from helpers.core.utils import InputException, UnexpectedException
+from helpers.options import DefaultOptions
 from .config import Config
 
 
 class DefaultConfig(Config):
 
     def __init__(self, *args):
         super(DefaultConfig, self).__init__(*args)
```

### Comparing `civitdl-2.0.9/src/civitconfig/data/config/sorterconfig.py` & `civitdl-2.1.0.dev1/src/civitconfig/data/config/sorterconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import os
 import shutil
-from helpers.exceptions import InputException, ResourcesException
-from helpers.utils import getDate, print_exc
+import sys
+from helpers.core.utils import InputException, ResourcesException, getDate, print_exc, sprint
 from helpers.sorter.utils import import_sort_model
 from .config import Config
 
 
 class SorterConfig(Config):
 
     def __init__(self, *args):
         super(SorterConfig, self).__init__(*args)
 
     def _copyPyFile(self, filepath) -> str:
         dst_filename = f'{getDate()}.py'
         dstpath = os.path.join(
             self._sorters_dir_path, dst_filename)
-        shutil.copy2(filepath, dstpath)
-        return dstpath
+        try:
+            shutil.copy2(filepath, dstpath)
+            return dstpath
+        except Exception as e:
+            sprint('Source: ', filepath, file=sys.stderr)
+            sprint('Destination: ', dstpath, file=sys.stderr)
+            raise e
 
     def _uncopyPyFile(self, filepath):
         if os.path.exists(filepath):
             os.remove(filepath)
         else:
             raise ResourcesException(
                 'Unable to uncopy python file (or delete it from program) because it does not exist')
```

### Comparing `civitdl-2.0.9/src/civitconfig/data/configmanager.py` & `civitdl-2.1.0.dev1/src/civitconfig/data/configmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
 import shutil
 
-from appdirs import AppDirs
-
-from helpers.styler import Styler
-from helpers.exceptions import InputException, UnexpectedException
-from helpers.utils import DefaultOptions, createDirsIfNotExist, getDate, print_verbose
-from helpers.vars.program_constants import app_dirs
+from helpers.core.utils import Styler, UnexpectedException, getDate, print_verbose, sprint
+from helpers.options import DefaultOptions
+from helpers.core.iohelper import IOHelper
+from helpers.core.constants import app_dirs
 
 from .config.config import Config, DEFAULT_CONFIG
 from .config.aliasconfig import AliasConfig
 from .config.defaultconfig import DefaultConfig
 from .config.sorterconfig import SorterConfig
 
 # Check alias -> current dir -> default
@@ -36,15 +34,15 @@
 
         super(ConfigManager, self).__init__(*args)
         self._aliasConfig = AliasConfig(*args)
         self._defaultConfig = DefaultConfig(*args)
         self._sorterConfig = SorterConfig(*args)
 
         # Make sure all directories exist
-        createDirsIfNotExist(args[1:])
+        IOHelper.createDirsIfNotExist(args[1:])
 
         # make sure config file exist
         if not self._configExists():
             self._setFallback()
 
     def _trashConfig(self):
         dst_filename = f'{getDate()}.json'
@@ -84,22 +82,23 @@
 
     def addSorter(self, name, filepath):
         self._sorterConfig.addSorter(name, filepath)
 
     def deleteSorter(self, name):
         self._sorterConfig.deleteSorter(name)
         default_sorter_name = self.getDefault('sorter')
+        sprint(default_sorter_name, name)
         if (default_sorter_name == name):
-            self._defaultConfig.setDefault(sorter='basic')
+            self._defaultConfig.setDefault(DefaultOptions(sorter='basic'))
 
     def reset(self):
         self._setFallback()
-        print(Styler.stylize('Successfully resetted config.', color='success'))
+        sprint(Styler.stylize('Successfully resetted config.', color='success'))
 
     def download(self, dst_path):
         if os.path.isdir(dst_path):
             dst_path = os.path.join(dst_path, 'civitdl_config')
 
-        print(Styler.stylize(
+        sprint(Styler.stylize(
             f'Downloading zipped config to {dst_path}.zip', color='main'))
         shutil.make_archive(dst_path, 'zip',
                             self._config_dir_path)
```

### Comparing `civitdl-2.0.9/src/civitdl/__main__.py` & `civitdl-2.1.0.dev1/src/civitdl/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#!/usr/bin/env python3
 import traceback
-from operator import itemgetter
 
 from .batch.batch_download import batch_download, BatchOptions
 from .args.argparser import get_args
 
-from helpers.exceptions import UnexpectedException
-from helpers.sourcemanager import SourceManager
-from helpers.utils import print_verbose, run_verbose, print_exc, set_verbose
+from helpers.core.utils import print_verbose, run_verbose, print_exc, set_verbose, sprint
 
 
 def main():
     try:
         args = get_args()
 
         if args['verbose']:
             set_verbose(True)
         else:
             set_verbose(False)
 
-        print_verbose('Arguments: ', str(args))
+        tempargs = args.copy()
+        tempargs.pop('api_key')
+        print_verbose('Arguments: ', str(tempargs))
 
         batchOptions = BatchOptions(
             sorter=args['sorter'],
             max_images=args['max_images'],
+            nsfw_mode=args['nsfw_mode'],
             api_key=args['api_key'],
 
             with_prompt=args['with_prompt'],
             without_model=args['without_model'],
             limit_rate=args['limit_rate'],
             retry_count=args['retry_count'],
             pause_time=args['pause_time'],
 
             cache_mode=args['cache_mode'],
             model_overwrite=args['model_overwrite'],
 
+            with_color=args['with_color'],
             verbose=args['verbose']
         )
 
         batch_download(
             source_strings=args['source_strings'],
             rootdir=args['rootdir'],
             batchOptions=batchOptions
         )
 
     except Exception as e:
-        print('---------')
+        sprint('---------')
         run_verbose(traceback.print_exc)
         print_exc(e)
-        print('---------')
+        sprint('---------')
```

### Comparing `civitdl-2.0.9/src/civitdl/args/argparser.py` & `civitdl-2.1.0.dev1/src/civitdl/args/argparser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import argparse
 import os
 
 
 from civitconfig.data.configmanager import ConfigManager
-from helpers.argparse import PwdAction, ColoredArgParser
-from helpers.utils import get_version
+from helpers.argparse import PwdAction, ColoredArgParser, BooleanOptionalAction
+from helpers.core.utils import get_version
 
 
 def parse_sorter(sorters, sorter_str):
     for sorter in sorters:
         if sorter_str == sorter[0]:
             return sorter[2]
 
@@ -48,23 +48,27 @@
 
 
 parser.add_argument('-s', '--sorter', type=str,
                     help='Specify which sorter function to use.\nDefault is "basic" sorter.\nProvide file path to sorter function if you wish to use a custom sorter.')
 parser.add_argument('-i', '--max-images', metavar='INT', type=int,
                     help='Specify max images to download for each model.')
 
+parser.add_argument(
+    '--nsfw-mode', metavar='MODE', type=str, help='Specify the nsfw mode when downloading images. Setting to 0 means the program will only download sfw. Setting to 1 means the program will download sfw, and nsfw images depending on the nsfw rating of the model. Setting to 2 means the program will download both sfw and nsfw.'
+)
+
 parser.add_argument('-k', '--api-key', action=PwdAction, type=str, required=False, nargs='?',
                     help='Prompt user for api key to download models that require users to log in.')
 
 parser.add_argument(
-    '--with-prompt', action=argparse.BooleanOptionalAction, help='Download images with prompt.'
+    '--with-prompt', action=BooleanOptionalAction, help='Download images with prompt.'
 )
 
 parser.add_argument(
-    '--without-model', action=argparse.BooleanOptionalAction, help='Download only extra details like metadata, images and hashes.'
+    '--without-model', action=BooleanOptionalAction, help='Download only extra details like metadata, images and hashes.'
 )
 
 parser.add_argument(
     '--limit-rate', metavar='BYTE', type=str, help='Limit the download speed/rate of resources downloaded from CivitAI.'
 )
 
 parser.add_argument(
@@ -76,20 +80,23 @@
 )
 
 parser.add_argument(
     '--cache-mode', metavar='MODE', type=str, help='Specify the cache mode. 0 to not use cache. 1 to use cache and copy existant models based on file path. 2 to use cache and copy existant models based on file path + hashes of model. Note that mode 2 has not been implemented yet. See documentation on github for more info.'
 )
 
 parser.add_argument(
-    '--model-overwrite', action=argparse.BooleanOptionalAction, help='Determine whether to overwrite or skip model download if model is already in path. model=overwrite to overwrite model. no-model-overwrite to skip model.'
+    '--model-overwrite', action=BooleanOptionalAction, help='Determine whether to overwrite or skip model download if model is already in path. model=overwrite to overwrite model. no-model-overwrite to skip model.'
 )
 
+parser.add_argument(
+    '--with-color', action=BooleanOptionalAction, help='Enable styles like colors, background colors and bold/italized texts.'
+)
 
 parser.add_argument(
-    '--verbose', action=argparse.BooleanOptionalAction, help='Prints out traceback and other useful information.'
+    '--verbose', action=BooleanOptionalAction, help='Prints out traceback and other useful information.'
 )
 
 parser.add_argument(
     '-v', '--version', action='version', version=f'civitdl v{get_version()}', help='Prints out the version of the program.'
 )
 
 
@@ -102,20 +109,23 @@
 
     return {
         "source_strings": parser_result.srcmodels,
         "rootdir": parse_rootdir(aliases, parser_result.rootdir),
 
         "sorter": parse_sorter(sorters, parser_result.sorter or config_defaults.get('sorter', None)),
         "max_images": parser_result.max_images or config_defaults.get('max_images', None),
+        "nsfw_mode": parser_result.nsfw_mode or config_defaults.get('nsfw_mode', None),
         "api_key": parser_result.api_key or config_defaults.get('api_key', None),
 
         "with_prompt": parser_result.with_prompt if parser_result.with_prompt is not None else config_defaults.get('with_prompt', None),
         "without_model": parser_result.without_model if parser_result.without_model is not None else config_defaults.get('without_model', None),
         "limit_rate": parser_result.limit_rate or config_defaults.get('limit_rate', None),
         "retry_count": parser_result.retry_count or config_defaults.get('retry_count', None),
         "pause_time": parser_result.pause_time or config_defaults.get('pause_time', None),
 
         "cache_mode": parser_result.cache_mode or config_defaults.get('cache_mode', None),
         "model_overwrite": parser_result.model_overwrite if parser_result.model_overwrite is not None else config_defaults.get('model_overwrite', None),
 
+        "with_color": parser_result.with_color if parser_result.with_color is not None else config_defaults.get('with_color', None),
+
         "verbose": False if parser_result.verbose == None else parser_result.verbose
     }
```

### Comparing `civitdl-2.0.9/src/civitdl.egg-info/PKG-INFO` & `civitdl-2.1.0.dev1/src/civitdl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civitdl
-Version: 2.0.9
+Version: 2.1.0.dev1
 Summary: Package for batch downloading models from civitai.com
 Author: Owen Truong
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,18 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Repository, https://github.com/OwenTruong/civitdl
 Project-URL: Bug Tracker, https://github.com/OwenTruong/civitdl/issues
 Keywords: civitai,batch download
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: tqdm<5,>=4.66.1
 Requires-Dist: appdirs<2,>=1.4.4
 Requires-Dist: argparse<2,>=1.4
 
 # civitdl (civitai-batch-download)
@@ -223,16 +223,14 @@
 (QUICK NOTE: CivitAI seems to have changed their API so that it will require an API key for all model downloads, please see [API Key Page](/doc/api_key.md) for instructions)
 
 **Note v2 has some changes regarding the cli args of the program. Please read the README below or run `civitdl --help` for the new arguments!**
 - To see changes to v2, go to [Changes in v2](#changes-in-v2-from-v1) section.
 
 Uses CLI to batch download Stable Diffusion models, metadata (including description of model, author, base model, example prompts and etc.) and example images (default is 3) of checkpoints, loras, and TI models from civitai!
 
-One thing to note is that for sfw models, currently, the program is set to only download sfw images. Please note that there may be sfw models that are rated as nsfw by CivitAI (and vice versa).
-
 <br/>
 
 ## Navigate
 - [README Page](/README.md)
 - [Alias Page](/doc/alias.md)
 - [API Key Page](/doc/api_key.md)
 - [Civitconfig / Configuration Page](/doc/civitconfig.md)
@@ -245,60 +243,77 @@
 - [civitdl (civitai-batch-download)](#civitdl-civitai-batch-download)
   - [Navigate](#navigate)
   - [Table Of Contents](#table-of-contents)
   - [Getting Started](#getting-started)
     - [Dependencies](#dependencies)
     - [Installing](#installing)
       - [Install using PIP](#install-using-pip)
-      - [Build from source](#build-from-source)
+      - [Build from source 1](#build-from-source-1)
+      - [Build from source 2 (if the instruction above fails with UNKNOWN package installed, else ignore this section)](#build-from-source-2-if-the-instruction-above-fails-with-unknown-package-installed-else-ignore-this-section)
     - [Quick Start](#quick-start)
       - [Configuration Program Options - civitconfig](#configuration-program-options---civitconfig)
   - [Changes in v2 from v1](#changes-in-v2-from-v1)
   - [Troubleshooting](#troubleshooting)
   - [Contributing](#contributing)
   - [License](#license)
 
 <br/>
 
 ## Getting Started
 
 ### Dependencies
-* Python3
+* Python3.8 or above
 * `requirements.txt`
 
 <br/>
 
 ### Installing
 
 #### Install using PIP
 ```bash
-pip3 install civitdl
+pip3 install civitdl 
+# pip install civitdl # if pip3 is not found
 ```
-- Use `pip install civitdl` if `pip3` is not found.
 
 <br/>
 
-#### Build from source
+#### Build from source 1
 ```bash
 git clone https://github.com/OwenTruong/civitdl.git # Clone the project
 cd civitdl # CD into project directory
-make install # Now program is installed globally unless you are using a virtual env
-# make install2 # Run this if make install fails
+pip3 install . # Use pip if pip3 is not found
+```
+
+<br />
+
+#### Build from source 2 (if the instruction above fails with UNKNOWN package installed, else ignore this section)
+```bash
+# Make sure you are in project directory # use pip if pip3 is not found
+python3 -m build
+pip3 install -r ./requirements.txt
+pip3 install --upgrade dist/*.whl
 ```
+<br />
+
 
 ### Quick Start
 To get started quickly, copy the command below.
 - See [civitdl doc](/doc/civitdl.md) for more info.
 
 ``` bash
 civitdl 123456 ./models
 ```
-- Replace `123456` your model of choice (it can be a civitai.com url or model id).
+- Replace `123456` with your model of choice (it can be a civitai.com url or model id).
 - Replace `./models` with the directory you wish to download the model to.
 
+Example with url:
+```bash
+civitdl https://civitai.com/models/123456 ./models
+```
+
 <br/>
 
 #### Configuration Program Options - civitconfig
 - Configuring the program might make your life easier. You would be able to set default sorter, max images, and api key to use without running any of those options in the main program!
   - You would also be able to add and delete sorters and aliases from the program.
   - Check [civitconfig doc](/doc/civitconfig.md).
 - Run `civitconfig --help` to check what options are available!
@@ -340,18 +355,14 @@
 
 For Windows, this may help: https://www.computerhope.com/issues/ch000549.htm
 
 If you are building from source and the following packages are not available `setuptools, wheel, build`, please install them with `pip install setuptools wheel build`
 
 ------
 
-If you are building the project and python unsuccessfully installs the program with `make install`, and displays the package's name as `UNKNOWN`, it is likely because you are trying to install the package globally. Either run `make install2` or use virtual env `python -m venv venv && source ./venv/bin/activate && make install`.
-
-------
-
 <br/>
 
 
 
 ## Contributing
 
 Thanks for the interest in the project!
```

### Comparing `civitdl-2.0.9/src/civitdl.egg-info/SOURCES.txt` & `civitdl-2.1.0.dev1/src/civitdl.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 src/civitdl.egg-info/SOURCES.txt
 src/civitdl.egg-info/dependency_links.txt
 src/civitdl.egg-info/entry_points.txt
 src/civitdl.egg-info/requires.txt
 src/civitdl.egg-info/top_level.txt
 src/civitdl/api/sorter.py
 src/civitdl/args/argparser.py
-src/civitdl/batch/_get_model.py
+src/civitdl/batch/_metadata.py
+src/civitdl/batch/_model.py
 src/civitdl/batch/batch_download.py
 src/helpers/__init__.py
 src/helpers/argparse.py
-src/helpers/constants.py
-src/helpers/exceptions.py
 src/helpers/hashmanager.py
+src/helpers/options.py
 src/helpers/sourcemanager.py
-src/helpers/styler.py
-src/helpers/utils.py
-src/helpers/validation.py
+src/helpers/core/__Init__.py
+src/helpers/core/_validation.py
+src/helpers/core/constants.py
+src/helpers/core/iohelper.py
+src/helpers/core/utils.py
+src/helpers/core/_ui/__Init__.py
+src/helpers/core/_ui/styler.py
 src/helpers/sorter/__Init__.py
 src/helpers/sorter/basic.py
 src/helpers/sorter/tags.py
-src/helpers/sorter/utils.py
-src/helpers/vars/__init__.py
-src/helpers/vars/program_constants.py
+src/helpers/sorter/utils.py
```

### Comparing `civitdl-2.0.9/src/helpers/hashmanager.py` & `civitdl-2.1.0.dev1/src/helpers/hashmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 
 import os
 import math
 import csv
 from typing import Dict, Union
 
-from appdirs import AppDirs
-
-from helpers.styler import Styler
-from helpers.exceptions import ResourcesException
-from helpers.utils import print_verbose
-from helpers.vars.program_constants import app_dirs
+from helpers.core.utils import Styler, print_verbose, sprint
+from helpers.core.constants import app_dirs
 
 # TODO: Watch out for edge cases where one of the hash is empty.
 # { '123456': { 'model_filepath': 'path', 'SHA256': 'hash1', 'BLAKE3': 'hash2' } }
 
 
 class HashManager:
     __CACHE_COLUMNS = ['volume_id', 'model_filepath', 'SHA256', 'BLAKE3']
@@ -68,23 +64,23 @@
                 ])
 
     def __get_hash_dict(self) -> Dict:
         return self.__hashes_dict.get(self.__version_id)
 
     def set_local_model_cache(self, model_filepath: str, hashes: Dict[str, str]) -> None:
         self.__hashes_dict[self.__version_id] = {
-            'model_filepath': model_filepath,
+            'model_filepath': os.path.abspath(model_filepath),
             'SHA256': hashes.get('SHA256', ''),
             'BLAKE3': hashes.get('BLAKE3', '')
         }
         self.__write_to_csv()
 
     def get_local_model_path(self) -> Union[None, str]:
         hash_dict = self.__get_hash_dict()
 
         if hash_dict is None:
-            print(Styler.stylize(
+            sprint(Styler.stylize(
                 f'Cache of model with version id {self.__version_id} not found.', color='info'))
             return None
         else:
             filepath = hash_dict['model_filepath']
             return None if not os.path.isfile(filepath) else filepath
```

### Comparing `civitdl-2.0.9/src/helpers/sorter/basic.py` & `civitdl-2.1.0.dev1/src/helpers/sorter/basic.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.0.9/src/helpers/sorter/tags.py` & `civitdl-2.1.0.dev1/src/helpers/sorter/tags.py`

 * *Files identical despite different names*

### Comparing `civitdl-2.0.9/src/helpers/sorter/utils.py` & `civitdl-2.1.0.dev1/src/helpers/sorter/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Dict, List
 import importlib.util
 import re
 from dataclasses import dataclass
 
-from helpers.validation import Validation
-from helpers.constants import BLACKLISTED_DIR_CHARS
+from helpers.core.utils import Validation
+from helpers.core.constants import BLACKLISTED_DIR_CHARS
 
 
 def import_sort_model(path: str) -> Callable[[Dict, Dict, str, str], List[str]]:
     spec = importlib.util.spec_from_file_location('sorter', path)
     sorter = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(sorter)
     return sorter.sort_model
```

### Comparing `civitdl-2.0.9/src/helpers/sourcemanager.py` & `civitdl-2.1.0.dev1/src/helpers/sourcemanager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,105 @@
 from dataclasses import dataclass
-from datetime import datetime
-import json
 import os
 import re
-import sys
-from typing import Callable, Dict, Iterable, List, Literal, Union
-import importlib.util
-import concurrent.futures
-import requests
-from tqdm import tqdm
+from typing import List, Literal, Union, Optional
 
-from helpers.styler import Styler
-from helpers.exceptions import CustomException, InputException, UnexpectedException
+from helpers.core.utils import print_verbose, InputException, UnexpectedException
+
+# modify id class to use getters and setters so that I can control how the data is being accessed
+# modify id class to not use type.
 
 
-@dataclass
 class Id:
-    type: Literal['id', 'site', 'api']
-    data: List[str]
+    """
+    Id class may only be used externally for type hint and type checking
+    """
     original: str
+    model_id: Optional[str]
+    version_id: Optional[str]
 
-    def __init__(self, type, data: List[str], original: str):
-        if type != 'id' and type != 'site' and type != 'api':
-            raise UnexpectedException(
-                f'Unknown type provided for Id class: {type}')
-
-        self.type = type
-        self.data = data
-        self.original = original
+    def __init__(self):
+        if type(self) == Id:
+            raise UnexpectedException(f"only subclass of Id may be instantiated")  # nopep8
 
-    def __post_init__(self):
-        if self.type != 'id' and self.type != 'site' and self.type != 'api':
-            raise UnexpectedException(
-                f'Unknown type provided for Id class: {self.type}')
-        for el in self.data:
-            if not isinstance(el, str):
-                raise UnexpectedException(
-                    f'Wrong data type for {el} in {self.data}')
 
+@dataclass
+class _Id(Id):
+    original: str
+    model_id: Optional[str] = None
+    version_id: Optional[str] = None
+
+    def __post_init__(self):
         if not isinstance(self.original, str):
             raise UnexpectedException(f'Wrong data type for {self.original}')
 
+        if self.model_id and not self.model_id.isdigit():
+            raise UnexpectedException(f'Model id passed for {self.original} is not a valid model id. The model id passed: {self.model_id}')  # nopep8
+
+        if self.version_id and not self.version_id.isdigit():
+            raise UnexpectedException(f'Model id passed for {self.original} is not a valid model id. The version id passed: {self.version_id}')  # nopep8
+
 
 class SourceManager:
     def __init__(self) -> None:
         pass
 
     def __get_comma_list(self, string: str) -> List[str]:
         return [input_str for input_str in string.replace(
             '\n', '').split(',') if input_str.strip() != '']
 
     def __use_parent_dir_if_exist(self, src: str, parent: Union[str, None]) -> str:
         return os.path.normpath(os.path.join(os.path.dirname(parent), src)) if parent else src
 
-    def parse_src(self, str_li: List[str], parent: Union[str, None] = None) -> List[Id]:
-        res: List[Id] = []
+    def parse_src(self, str_li: List[str], parent: Union[str, None] = None) -> List[_Id]:
+        res: List[_Id] = []
         for string in str_li:
             string = string.strip()
 
             if string.isdigit() and abs(int(string)) == int(string):
-                res.append(Id('id', [string], string))
+                model_id = string
+                res.append(_Id(original=string, model_id=model_id))
             elif len(self.__get_comma_list(string)) > 1:
                 arg_str_li = self.__get_comma_list(string)
                 res.extend(self.parse_src(arg_str_li))
             elif 'civitai.com/api' in string:
                 version_id_regex = r'(?<=models\/)\d+'
                 version_id = re.search(version_id_regex, string)
                 if version_id == None:
                     err = 'Incorrect format for the url provided' + \
                         (f' in {parent}: ' if parent else ': ') + string
                     raise InputException(err)
                 version_id = version_id.group(0)
-                res.append(Id('api', [version_id], string))
+                res.append(_Id(original=string, version_id=version_id))
             elif 'civitai.com/models' in string:
                 model_id = re.search(r'(?<=models\/)\d+', string)
                 version_id = re.search(r'(?<=modelVersionId=)\d+', string)
 
                 if model_id == None:
                     err = 'Incorrect format for the url/id provided' + \
                         (f' in {parent}: ' if parent else ': ') + string
                     raise InputException(err)
                 model_id = model_id.group(0)
 
                 if version_id:
                     version_id = version_id.group(0)
                     res.append(
-                        Id('site', [model_id, version_id], string))
+                        _Id(original=string, model_id=model_id, version_id=version_id))
                 else:
-                    res.append(Id('site', [model_id], string))
+                    res.append(_Id(original=string, model_id=model_id))
             elif os.path.exists(self.__use_parent_dir_if_exist(string, parent)):
                 string = self.__use_parent_dir_if_exist(string, parent)
-                print(f'after: {string}')
                 file_str = None
 
                 with open(string, 'r', encoding='UTF-8') as file:
                     file_str = file.read().strip()
                 if file_str == None:
                     raise UnexpectedException(
                         'Unknown exception while reading batchfile path.')
                 str_li_res = self.__get_comma_list(file_str)
+                print_verbose(str_li_res)
                 res.extend(self.parse_src(str_li_res, parent=string))
             else:
                 raise InputException(
-                    f'Bad source provided: {string}', f'   Batchfile Path: {parent}' if parent else None)
+                    f'Bad source provided: {string}', f'   Parent Batchfile Path: {parent}' if parent else None)
 
         return res
```

### Comparing `civitdl-2.0.9/src/helpers/validation.py` & `civitdl-2.1.0.dev1/src/helpers/core/_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from .styler import Styler
-from .exceptions import CustomException, InputException, UnexpectedException
+from ._ui.styler import Styler, InputException, UnexpectedException
 from .constants import BLACKLISTED_DIR_CHARS
 import sys
 import os
 from typing import Iterable, Union
 
 
 class Validation:
     @staticmethod
     def __validate_arg_name(arg_name):
         if not isinstance(arg_name, str):
             raise UnexpectedException(
-                f'Name/title of validator is not a string (arg_name: {arg_name})'
-            )
+                f'Name/title of validator is not a string (arg_name: {arg_name})')
 
         if len(arg_name) == 0:
             raise UnexpectedException(
                 f'Name/title of validator is not defined (arg_name: {arg_name}, length of arg_name: {len(arg_name)})')
 
     @staticmethod
     def __validate_range(min, max):
@@ -36,65 +34,57 @@
     def validate_string(cls, value, arg_name: str, min_len: Union[int, None] = None, max_len: Union[int, None] = None, whitelist: Iterable[str] = [], blacklist: Iterable[str] = []) -> str:
         # Validate keyword arguments
 
         cls.__validate_arg_name(arg_name)
         cls.__validate_range(min_len, max_len)
         if min_len is not None and min_len < 0:
             raise UnexpectedException(
-                f'Minimum length provided with value "{value}" is below 0 (min_len: {min_len}).'
-            )
+                f'Minimum length provided with value "{value}" is below 0 (min_len: {min_len}).')
         if max_len is not None and max_len < 0:
             raise UnexpectedException(
-                f'Maximum length provided with value "{value}" is below 0 (max_len: {max_len}).'
-            )
+                f'Maximum length provided with value "{value}" is below 0 (max_len: {max_len}).')
 
         if not isinstance(whitelist, Iterable):
             raise UnexpectedException(
                 f'Whitelist provided with value "{value}" is not a list (whitelist: {whitelist}).')
         if not all(isinstance(item, str) for item in whitelist):
             raise UnexpectedException(
-                f'Whitelist provided with value "{value}" contains non-string elements (whitelist: {whitelist}).'
-            )
+                f'Whitelist provided with value "{value}" contains non-string elements (whitelist: {whitelist}).')
 
         if not isinstance(blacklist, Iterable):
             raise UnexpectedException(
                 f'Blacklist provided with value "{value}" is not a list (blacklist: {blacklist}).')
         if not all(isinstance(item, str) for item in blacklist):
             raise UnexpectedException(
-                f'Blacklist provided with value "{value}" contains non-string elements (blacklist: {blacklist}).'
-            )
+                f'Blacklist provided with value "{value}" contains non-string elements (blacklist: {blacklist}).')
         if len(whitelist) > 0 and len(blacklist) > 0:
             raise UnexpectedException(
-                f'Both whitelist and blacklist provided with value "{value}" is not empty. You can not have both whitelist and blacklist (whitelist: {whitelist}, blacklist: {blacklist}).'
-            )
+                f'Both whitelist and blacklist provided with value "{value}" is not empty. You can not have both whitelist and blacklist (whitelist: {whitelist}, blacklist: {blacklist}).')
 
         # Validate value
 
         if not isinstance(value, str):
             raise InputException(
                 f'Value provided for {arg_name} is not a string (value: {value}, type: {type(value)}).')
 
         if value == '':
             raise InputException(
                 f'Value provided for {arg_name} is empty.')
 
         if min_len is not None and len(value) < min_len:
             raise InputException(
-                f'Value provided for {arg_name} is below minimum length allowed (value: {value}, min_len: {min_len}).'
-            )
+                f'Value provided for {arg_name} is below minimum length allowed (value: {value}, min_len: {min_len}).')
 
         if max_len is not None and len(value) > max_len:
             raise InputException(
-                f'Value provided for {arg_name} is above maximum length allowed (value: {value}, min_len: {min_len}).'
-            )
+                f'Value provided for {arg_name} is above maximum length allowed (value: {value}, min_len: {min_len}).')
 
         if whitelist != [] and value not in whitelist:
             raise InputException(
-                f'Value provided for {arg_name} is not in whitelist (value: {value}, whitelist: {whitelist}).'
-            )
+                f'Value provided for {arg_name} is not in whitelist (value: {value}, whitelist: {whitelist}).')
 
         if blacklist != [] and value in blacklist:
             raise InputException(
                 f'Value provided for {arg_name} is in blacklist (value: {value}, blacklist: {blacklist}).')
 
         return value
 
@@ -180,23 +170,23 @@
 
         if len(value) == 0:
             raise InputException(
                 f'Directory name provided by {arg_name} is empty.')
 
         if len(value.strip()) is not len(value):
             print(Styler.stylize(
-                f'Directory name provided by {arg_name} contains leading and trailing space. Proceeding to trim the following "{value}"', color='WARNING'))
+                f'Directory name provided by {arg_name} contains leading and trailing space. Proceeding to trim the following "{value}"', color='WARNING').encode())
             value = value.trim()
 
         for el in value:
             if el in BLACKLISTED_DIR_CHARS:
                 raise InputException(
-                    f'Directory name provided by {arg_name} is invalid. It may not contain the illegal character, "{el}".',
+                    f'Directory name provided by {arg_name} is invalid. It may not contain the illegal character, "{el}".',  # nopep8
                     f'The provided directory name is "{value}".',
-                    f'The list of blacklisted characters are {BLACKLISTED_DIR_CHARS}.',
+                    f'The list of blacklisted characters are {BLACKLISTED_DIR_CHARS}.',  # nopep8
                     f'If this directory path is generated from a sorter, please report or change to a different sorter.'
                 )
 
         return value
 
     @classmethod
     def validate_dir_path(cls, value, arg_name):
@@ -207,19 +197,21 @@
 
         if len(value) == 0:
             raise InputException(
                 f'Directory path provided by {arg_name} is empty.')
 
         if len(value.strip()) is not len(value):
             print(Styler.stylize(
-                f'Directory path provided by {arg_name} contains leading and trailing space. Proceeding to trim the following "{value}"', color='WARNING'))
+                f'Directory path provided by {arg_name} contains leading and trailing space. Proceeding to trim the following "{value}"', color='WARNING')).encode()
             value = value.trim()
 
         modified_value = value.replace('/', '\\') if os.name == 'nt' else value
-        dir_names = modified_value.split(os.path.sep)
+        if os.name == 'nt' and os.path.isabs(modified_value):
+            modified_value = modified_value[2:]
+        dir_names = [s for s in modified_value.split(os.path.sep) if s != ""]
         for dir_name in dir_names:
             try:
                 cls.validate_dir_name(dir_name, arg_name)
             except InputException as e:
                 raise InputException(
                     e, f'The invalid directory path is {value}')
```

