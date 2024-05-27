# Comparing `tmp/powerpathfinder_models-2.0.0.tar.gz` & `tmp/powerpathfinder_models-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpathfinder_models-2.0.0.tar", last modified: Sat May 25 22:12:48 2024, max compression
+gzip compressed data, was "powerpathfinder_models-2.1.0.tar", last modified: Mon May 27 14:26:04 2024, max compression
```

## Comparing `powerpathfinder_models-2.0.0.tar` & `powerpathfinder_models-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/common/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/charger.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/fcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/route.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/common/models/valuation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 22:12:48.000000 powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-25 22:12:43.000000 powerpathfinder_models-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:12:48.044024 powerpathfinder_models-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:04.809458 powerpathfinder_models-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-27 14:26:04.809458 powerpathfinder_models-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:04.809458 powerpathfinder_models-2.1.0/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:04.809458 powerpathfinder_models-2.1.0/common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:04.809458 powerpathfinder_models-2.1.0/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/charger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/fcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/common/models/valuation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:26:04.809458 powerpathfinder_models-2.1.0/powerpathfinder_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-27 14:26:04.000000 powerpathfinder_models-2.1.0/powerpathfinder_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-27 14:26:04.000000 powerpathfinder_models-2.1.0/powerpathfinder_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:26:04.000000 powerpathfinder_models-2.1.0/powerpathfinder_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 14:26:04.000000 powerpathfinder_models-2.1.0/powerpathfinder_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 14:26:04.000000 powerpathfinder_models-2.1.0/powerpathfinder_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-27 14:26:00.000000 powerpathfinder_models-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:26:04.809458 powerpathfinder_models-2.1.0/setup.cfg
```

### Comparing `powerpathfinder_models-2.0.0/common/models/achievement.py` & `powerpathfinder_models-2.1.0/common/models/achievement.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-2.0.0/common/models/charger.py` & `powerpathfinder_models-2.1.0/common/models/charger.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-2.0.0/common/models/payment.py` & `powerpathfinder_models-2.1.0/common/models/payment.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-2.0.0/common/models/route.py` & `powerpathfinder_models-2.1.0/common/models/route.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-2.0.0/common/models/user.py` & `powerpathfinder_models-2.1.0/common/models/user.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-2.0.0/common/models/valuation.py` & `powerpathfinder_models-2.1.0/common/models/valuation.py`

 * *Files identical despite different names*

### Comparing `powerpathfinder_models-2.0.0/powerpathfinder_models.egg-info/SOURCES.txt` & `powerpathfinder_models-2.1.0/powerpathfinder_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*
