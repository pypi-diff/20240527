# Comparing `tmp/sevenapps_py_easy-0.0.8.tar.gz` & `tmp/sevenapps_py_easy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenapps_py_easy-0.0.8.tar", last modified: Sun May 26 10:27:52 2024, max compression
+gzip compressed data, was "sevenapps_py_easy-0.0.9.tar", last modified: Sun May 26 10:56:35 2024, max compression
```

## Comparing `sevenapps_py_easy-0.0.8.tar` & `sevenapps_py_easy-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.399908 sevenapps_py_easy-0.0.8/
--rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.8/LICENSE
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-26 10:27:52.399846 sevenapps_py_easy-0.0.8/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      205 2024-05-24 22:50:51.000000 sevenapps_py_easy-0.0.8/README.md
--rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-26 10:27:52.400098 sevenapps_py_easy-0.0.8/setup.cfg
--rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-26 10:27:44.000000 sevenapps_py_easy-0.0.8/setup.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.398117 sevenapps_py_easy-0.0.8/sevenapps/
--rw-r--r--   0 jjimenez   (502) staff       (20)       42 2024-05-24 21:42:35.000000 sevenapps_py_easy-0.0.8/sevenapps/__init__.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.398577 sevenapps_py_easy-0.0.8/sevenapps/services/
--rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:01.000000 sevenapps_py_easy-0.0.8/sevenapps/services/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     8576 2024-05-26 10:26:51.000000 sevenapps_py_easy-0.0.8/sevenapps/services/google_firestore_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     2658 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.8/sevenapps/services/google_services_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     3211 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.8/sevenapps/services/selenium_connector.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.398797 sevenapps_py_easy-0.0.8/sevenapps/utils/
--rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:09.000000 sevenapps_py_easy-0.0.8/sevenapps/utils/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.8/sevenapps/utils/file_manager.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:27:52.399562 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      491 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/SOURCES.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/dependency_links.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/requires.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       10 2024-05-26 10:27:52.000000 sevenapps_py_easy-0.0.8/sevenapps_py_easy.egg-info/top_level.txt
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:56:35.859654 sevenapps_py_easy-0.0.9/
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.9/LICENSE
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-26 10:56:35.859594 sevenapps_py_easy-0.0.9/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      205 2024-05-24 22:50:51.000000 sevenapps_py_easy-0.0.9/README.md
+-rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-26 10:56:35.859847 sevenapps_py_easy-0.0.9/setup.cfg
+-rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-26 10:56:12.000000 sevenapps_py_easy-0.0.9/setup.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:56:35.857241 sevenapps_py_easy-0.0.9/sevenapps/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       42 2024-05-24 21:42:35.000000 sevenapps_py_easy-0.0.9/sevenapps/__init__.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:56:35.858057 sevenapps_py_easy-0.0.9/sevenapps/services/
+-rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:01.000000 sevenapps_py_easy-0.0.9/sevenapps/services/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     8576 2024-05-26 10:26:51.000000 sevenapps_py_easy-0.0.9/sevenapps/services/google_firestore_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     2658 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.9/sevenapps/services/google_services_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     3211 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.9/sevenapps/services/selenium_connector.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:56:35.858520 sevenapps_py_easy-0.0.9/sevenapps/utils/
+-rw-r--r--   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:51:09.000000 sevenapps_py_easy-0.0.9/sevenapps/utils/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1249 2024-05-26 10:56:02.000000 sevenapps_py_easy-0.0.9/sevenapps/utils/data_manager.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.9/sevenapps/utils/file_manager.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-26 10:56:35.859334 sevenapps_py_easy-0.0.9/sevenapps_py_easy.egg-info/
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-26 10:56:35.000000 sevenapps_py_easy-0.0.9/sevenapps_py_easy.egg-info/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      523 2024-05-26 10:56:35.000000 sevenapps_py_easy-0.0.9/sevenapps_py_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-26 10:56:35.000000 sevenapps_py_easy-0.0.9/sevenapps_py_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-26 10:56:35.000000 sevenapps_py_easy-0.0.9/sevenapps_py_easy.egg-info/requires.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       10 2024-05-26 10:56:35.000000 sevenapps_py_easy-0.0.9/sevenapps_py_easy.egg-info/top_level.txt
```

### Comparing `sevenapps_py_easy-0.0.8/LICENSE` & `sevenapps_py_easy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.8/sevenapps/services/google_firestore_connector.py` & `sevenapps_py_easy-0.0.9/sevenapps/services/google_firestore_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.8/sevenapps/services/google_services_connector.py` & `sevenapps_py_easy-0.0.9/sevenapps/services/google_services_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.8/sevenapps/services/selenium_connector.py` & `sevenapps_py_easy-0.0.9/sevenapps/services/selenium_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.8/sevenapps/utils/file_manager.py` & `sevenapps_py_easy-0.0.9/sevenapps/utils/file_manager.py`

 * *Files identical despite different names*

