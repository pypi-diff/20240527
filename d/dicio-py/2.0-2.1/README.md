# Comparing `tmp/dicio_py-2.0.tar.gz` & `tmp/dicio_py-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-2.0.tar", last modified: Mon May 27 14:10:05 2024, max compression
+gzip compressed data, was "dicio_py-2.1.tar", last modified: Mon May 27 14:26:34 2024, max compression
```

## Comparing `dicio_py-2.0.tar` & `dicio_py-2.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:10:05.150871 dicio_py-2.0/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-2.0/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:10:05.146871 dicio_py-2.0/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-2.0/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:10:05.146871 dicio_py-2.0/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      154 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:10:05.000000 dicio_py-2.0/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 14:10:05.150871 dicio_py-2.0/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      647 2024-05-27 14:09:53.000000 dicio_py-2.0/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:26:34.178108 dicio_py-2.1/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-2.1/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:26:34.178108 dicio_py-2.1/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-2.1/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:26:34.170108 dicio_py-2.1/dicio/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:18:42.000000 dicio_py-2.1/dicio/__init__.py
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     3877 2024-05-27 13:57:27.000000 dicio_py-2.1/dicio/dicio.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-27 14:26:34.174108 dicio_py-2.1/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1667 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      222 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       49 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/entry_points.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        6 2024-05-27 14:26:34.000000 dicio_py-2.1/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-27 14:26:34.178108 dicio_py-2.1/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      708 2024-05-27 14:25:33.000000 dicio_py-2.1/setup.py
```

### Comparing `dicio_py-2.0/LICENSE` & `dicio_py-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-2.0/PKG-INFO` & `dicio_py-2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 2.0
+Version: 2.1
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dicio_py-2.0/README.md` & `dicio_py-2.1/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-2.0/dicio_py.egg-info/PKG-INFO` & `dicio_py-2.1/dicio_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 2.0
+Version: 2.1
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

