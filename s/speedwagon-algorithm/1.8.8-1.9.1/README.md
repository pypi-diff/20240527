# Comparing `tmp/speedwagon_algorithm-1.8.8.tar.gz` & `tmp/speedwagon_algorithm-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedwagon_algorithm-1.8.8.tar", last modified: Sat Mar 30 13:07:31 2024, max compression
+gzip compressed data, was "speedwagon_algorithm-1.9.1.tar", last modified: Mon May 27 12:47:28 2024, max compression
```

## Comparing `speedwagon_algorithm-1.8.8.tar` & `speedwagon_algorithm-1.9.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 ruchan    (1000) ruchan    (1000)        0 2024-03-30 13:07:31.580435 speedwagon_algorithm-1.8.8/
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)    35149 2024-03-24 11:33:14.000000 speedwagon_algorithm-1.8.8/LICENSE
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)      329 2024-03-30 13:07:31.580435 speedwagon_algorithm-1.8.8/PKG-INFO
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)     2789 2024-03-24 11:33:14.000000 speedwagon_algorithm-1.8.8/README.md
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)       38 2024-03-30 13:07:31.580435 speedwagon_algorithm-1.8.8/setup.cfg
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)      402 2024-03-30 13:07:19.000000 speedwagon_algorithm-1.8.8/setup.py
-drwxr-xr-x   0 ruchan    (1000) ruchan    (1000)        0 2024-03-30 13:07:31.580435 speedwagon_algorithm-1.8.8/speedwagon_algorithm.egg-info/
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)      329 2024-03-30 13:07:31.000000 speedwagon_algorithm-1.8.8/speedwagon_algorithm.egg-info/PKG-INFO
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)      202 2024-03-30 13:07:31.000000 speedwagon_algorithm-1.8.8/speedwagon_algorithm.egg-info/SOURCES.txt
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)        1 2024-03-30 13:07:31.000000 speedwagon_algorithm-1.8.8/speedwagon_algorithm.egg-info/dependency_links.txt
--rw-r--r--   0 ruchan    (1000) ruchan    (1000)        1 2024-03-30 13:07:31.000000 speedwagon_algorithm-1.8.8/speedwagon_algorithm.egg-info/top_level.txt
+drwxr-xr-x   0 ruchan    (1000) ruchan    (1000)        0 2024-05-27 12:47:28.783540 speedwagon_algorithm-1.9.1/
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)      307 2024-05-27 12:47:28.783540 speedwagon_algorithm-1.9.1/PKG-INFO
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)       38 2024-05-27 12:47:28.783540 speedwagon_algorithm-1.9.1/setup.cfg
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)      402 2024-05-27 12:43:27.000000 speedwagon_algorithm-1.9.1/setup.py
+drwxr-xr-x   0 ruchan    (1000) ruchan    (1000)        0 2024-05-27 12:47:28.782540 speedwagon_algorithm-1.9.1/speedwagon_algorithm/
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)       49 2024-05-27 12:37:49.000000 speedwagon_algorithm-1.9.1/speedwagon_algorithm/__init__.py
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)    23854 2024-05-27 12:37:27.000000 speedwagon_algorithm-1.9.1/speedwagon_algorithm/modules.py
+drwxr-xr-x   0 ruchan    (1000) ruchan    (1000)        0 2024-05-27 12:47:28.782540 speedwagon_algorithm-1.9.1/speedwagon_algorithm.egg-info/
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)      307 2024-05-27 12:47:28.000000 speedwagon_algorithm-1.9.1/speedwagon_algorithm.egg-info/PKG-INFO
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)      249 2024-05-27 12:47:28.000000 speedwagon_algorithm-1.9.1/speedwagon_algorithm.egg-info/SOURCES.txt
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)        1 2024-05-27 12:47:28.000000 speedwagon_algorithm-1.9.1/speedwagon_algorithm.egg-info/dependency_links.txt
+-rw-r--r--   0 ruchan    (1000) ruchan    (1000)       21 2024-05-27 12:47:28.000000 speedwagon_algorithm-1.9.1/speedwagon_algorithm.egg-info/top_level.txt
```

