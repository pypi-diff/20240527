# Comparing `tmp/allnc-0.1.0.tar.gz` & `tmp/allnc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allnc-0.1.0.tar", last modified: Mon May 27 08:52:39 2024, max compression
+gzip compressed data, was "allnc-0.1.1.tar", last modified: Mon May 27 10:10:55 2024, max compression
```

## Comparing `allnc-0.1.0.tar` & `allnc-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 08:52:39.748794 allnc-0.1.0/
--rw-r--r--   0 msi       (1000) msi       (1000)      880 2024-05-27 08:52:39.748794 allnc-0.1.0/PKG-INFO
--rw-rw-r--   0 msi       (1000) msi       (1000)       55 2024-05-23 14:40:22.000000 allnc-0.1.0/README.md
-drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 08:52:39.744827 allnc-0.1.0/allnc/
--rw-rw-r--   0 msi       (1000) msi       (1000)        0 2024-05-26 11:34:50.000000 allnc-0.1.0/allnc/__init__.py
--rw-rw-r--   0 msi       (1000) msi       (1000)     3749 2024-05-26 11:35:28.000000 allnc-0.1.0/allnc/app.py
--rw-rw-r--   0 msi       (1000) msi       (1000)      675 2024-05-23 14:36:01.000000 allnc-0.1.0/allnc/middleware.py
--rw-rw-r--   0 msi       (1000) msi       (1000)      944 2024-05-25 10:24:58.000000 allnc-0.1.0/allnc/response.py
-drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 08:52:39.748794 allnc-0.1.0/allnc.egg-info/
--rw-r--r--   0 msi       (1000) msi       (1000)      880 2024-05-27 08:52:39.000000 allnc-0.1.0/allnc.egg-info/PKG-INFO
--rw-rw-r--   0 msi       (1000) msi       (1000)      231 2024-05-27 08:52:39.000000 allnc-0.1.0/allnc.egg-info/SOURCES.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)        1 2024-05-27 08:52:39.000000 allnc-0.1.0/allnc.egg-info/dependency_links.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)      105 2024-05-27 08:52:39.000000 allnc-0.1.0/allnc.egg-info/requires.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)        6 2024-05-27 08:52:39.000000 allnc-0.1.0/allnc.egg-info/top_level.txt
--rw-rw-r--   0 msi       (1000) msi       (1000)       38 2024-05-27 08:52:39.748794 allnc-0.1.0/setup.cfg
--rw-rw-r--   0 msi       (1000) msi       (1000)     3914 2024-05-26 11:58:39.000000 allnc-0.1.0/setup.py
+drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:10:55.254775 allnc-0.1.1/
+-rw-r--r--   0 msi       (1000) msi       (1000)     7232 2024-05-27 10:10:55.254775 allnc-0.1.1/PKG-INFO
+-rw-rw-r--   0 msi       (1000) msi       (1000)     6400 2024-05-27 10:00:57.000000 allnc-0.1.1/README.md
+drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:10:55.254775 allnc-0.1.1/allnc/
+-rw-rw-r--   0 msi       (1000) msi       (1000)        0 2024-05-26 11:34:50.000000 allnc-0.1.1/allnc/__init__.py
+-rw-rw-r--   0 msi       (1000) msi       (1000)     3749 2024-05-26 11:35:28.000000 allnc-0.1.1/allnc/app.py
+-rw-rw-r--   0 msi       (1000) msi       (1000)      675 2024-05-23 14:36:01.000000 allnc-0.1.1/allnc/middleware.py
+-rw-rw-r--   0 msi       (1000) msi       (1000)      944 2024-05-25 10:24:58.000000 allnc-0.1.1/allnc/response.py
+drwxrwxr-x   0 msi       (1000) msi       (1000)        0 2024-05-27 10:10:55.254775 allnc-0.1.1/allnc.egg-info/
+-rw-r--r--   0 msi       (1000) msi       (1000)     7232 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/PKG-INFO
+-rw-rw-r--   0 msi       (1000) msi       (1000)      231 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/SOURCES.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)        1 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/dependency_links.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)      105 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/requires.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)        6 2024-05-27 10:10:55.000000 allnc-0.1.1/allnc.egg-info/top_level.txt
+-rw-rw-r--   0 msi       (1000) msi       (1000)       38 2024-05-27 10:10:55.254775 allnc-0.1.1/setup.cfg
+-rw-rw-r--   0 msi       (1000) msi       (1000)     3920 2024-05-27 10:10:31.000000 allnc-0.1.1/setup.py
```

### Comparing `allnc-0.1.0/allnc/app.py` & `allnc-0.1.1/allnc/app.py`

 * *Files identical despite different names*

### Comparing `allnc-0.1.0/allnc/middleware.py` & `allnc-0.1.1/allnc/middleware.py`

 * *Files identical despite different names*

### Comparing `allnc-0.1.0/allnc/response.py` & `allnc-0.1.1/allnc/response.py`

 * *Files identical despite different names*

### Comparing `allnc-0.1.0/setup.py` & `allnc-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'allnc'
 DESCRIPTION = 'Python Web Framework for building web applications'
-URL = 'https://github.com/me/myproject'
+URL = 'https://github.com/themusharraf/allnc'
 EMAIL = 'meibrohimov@gmail.com'
 AUTHOR = 'Musharraf Ibragimov'
 REQUIRES_PYTHON = '>=3.11.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'Jinja2==3.1.4',
     'parse==1.20.1',
     'requests==2.31.0',
     'requests-wsgi-adapter==0.4.1',
```

