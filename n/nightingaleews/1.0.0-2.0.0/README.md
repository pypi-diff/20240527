# Comparing `tmp/nightingaleews-1.0.0.tar.gz` & `tmp/nightingaleews-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingaleews-1.0.0.tar", last modified: Mon Apr 10 16:05:01 2023, max compression
+gzip compressed data, was "nightingaleews-2.0.0.tar", last modified: Mon May 27 18:47:39 2024, max compression
```

## Comparing `nightingaleews-1.0.0.tar` & `nightingaleews-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 16:05:01.393071 nightingaleews-1.0.0/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      243 2023-04-10 16:05:01.389738 nightingaleews-1.0.0/PKG-INFO
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 16:05:01.389738 nightingaleews-1.0.0/nightingaleews/
--rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-10 16:04:18.000000 nightingaleews-1.0.0/nightingaleews/__init__.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)     1770 2023-04-10 15:35:55.000000 nightingaleews-1.0.0/nightingaleews/ews_scorer.py
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2023-04-10 16:05:01.389738 nightingaleews-1.0.0/nightingaleews.egg-info/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      243 2023-04-10 16:05:01.000000 nightingaleews-1.0.0/nightingaleews.egg-info/PKG-INFO
--rw-r--r--   0 nuno      (1000) nuno      (1000)      216 2023-04-10 16:05:01.000000 nightingaleews-1.0.0/nightingaleews.egg-info/SOURCES.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2023-04-10 16:05:01.000000 nightingaleews-1.0.0/nightingaleews.egg-info/dependency_links.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       15 2023-04-10 16:05:01.000000 nightingaleews-1.0.0/nightingaleews.egg-info/top_level.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2023-04-10 16:05:01.393071 nightingaleews-1.0.0/setup.cfg
--rw-r--r--   0 nuno      (1000) nuno      (1000)      761 2023-04-10 16:04:01.000000 nightingaleews-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:47:39.414779 nightingaleews-2.0.0/
+-rw-rw-rw-   0        0        0      252 2024-05-27 18:47:39.413778 nightingaleews-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 18:47:39.402075 nightingaleews-2.0.0/nightingaleews/
+-rw-rw-rw-   0        0        0        0 2024-05-03 01:38:22.000000 nightingaleews-2.0.0/nightingaleews/__init__.py
+-rw-rw-rw-   0        0        0     1940 2024-05-27 18:33:05.000000 nightingaleews-2.0.0/nightingaleews/ews_scorer.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:47:39.412778 nightingaleews-2.0.0/nightingaleews.egg-info/
+-rw-rw-rw-   0        0        0      252 2024-05-27 18:47:39.000000 nightingaleews-2.0.0/nightingaleews.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-05-27 18:47:39.000000 nightingaleews-2.0.0/nightingaleews.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:47:39.000000 nightingaleews-2.0.0/nightingaleews.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-27 18:47:39.000000 nightingaleews-2.0.0/nightingaleews.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:47:39.414779 nightingaleews-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-05-27 18:33:17.000000 nightingaleews-2.0.0/setup.py
```

