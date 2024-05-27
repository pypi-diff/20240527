# Comparing `tmp/lckytools-0.0.8.tar.gz` & `tmp/lckytools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lckytools-0.0.8.tar", last modified: Tue Jan 30 05:58:59 2024, max compression
+gzip compressed data, was "lckytools-0.0.9.tar", last modified: Tue Jan 30 06:05:28 2024, max compression
```

## Comparing `lckytools-0.0.8.tar` & `lckytools-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:59.270924 lckytools-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-30 05:58:47.000000 lckytools-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:47.000000 lckytools-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-30 05:58:59.270924 lckytools-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 05:58:47.000000 lckytools-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:59.270924 lckytools-0.0.8/lckytools/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:59.270924 lckytools-0.0.8/lckytools/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/airflow/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:59.270924 lckytools-0.0.8/lckytools/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/sql/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/sql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-30 05:58:47.000000 lckytools-0.0.8/lckytools/sql/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 05:58:59.270924 lckytools-0.0.8/lckytools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-30 05:58:59.000000 lckytools-0.0.8/lckytools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-30 05:58:59.000000 lckytools-0.0.8/lckytools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 05:58:59.000000 lckytools-0.0.8/lckytools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-30 05:58:59.000000 lckytools-0.0.8/lckytools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-30 05:58:59.000000 lckytools-0.0.8/lckytools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-30 05:58:47.000000 lckytools-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 05:58:59.270924 lckytools-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 05:58:47.000000 lckytools-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:28.422935 lckytools-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-30 06:05:15.000000 lckytools-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:15.000000 lckytools-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-30 06:05:28.422935 lckytools-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 06:05:15.000000 lckytools-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:28.418935 lckytools-0.0.9/lckytools/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:28.422935 lckytools-0.0.9/lckytools/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/airflow/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:28.422935 lckytools-0.0.9/lckytools/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/sql/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/sql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-30 06:05:15.000000 lckytools-0.0.9/lckytools/sql/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 06:05:28.418935 lckytools-0.0.9/lckytools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-30 06:05:28.000000 lckytools-0.0.9/lckytools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-30 06:05:28.000000 lckytools-0.0.9/lckytools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 06:05:28.000000 lckytools-0.0.9/lckytools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-30 06:05:28.000000 lckytools-0.0.9/lckytools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-30 06:05:28.000000 lckytools-0.0.9/lckytools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-30 06:05:15.000000 lckytools-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 06:05:28.422935 lckytools-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 06:05:15.000000 lckytools-0.0.9/setup.py
```

### Comparing `lckytools-0.0.8/LICENSE` & `lckytools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.8/PKG-INFO` & `lckytools-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.8
+Version: 0.0.9
 Author-email: LCKYN <t.pwawrit@lckyn.com>
 License: MIT License
         
         Copyright (c) 2024 pawarit thareechan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `lckytools-0.0.8/lckytools/airflow/const.py` & `lckytools-0.0.9/lckytools/airflow/const.py`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.8/lckytools/sql/fetch.py` & `lckytools-0.0.9/lckytools/sql/fetch.py`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.8/lckytools/sql/schema.py` & `lckytools-0.0.9/lckytools/sql/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,7 +13,11 @@
 
     if cascade:
         sql += " CASCADE"
     else:
         sql += " RESTRICT"
 
     return f"{sql};"
+
+
+def show_schemas(catalog_name):
+    return f"SHOW SCHEMAS FROM '{catalog_name}';"
```

### Comparing `lckytools-0.0.8/lckytools/sql/table.py` & `lckytools-0.0.9/lckytools/sql/table.py`

 * *Files identical despite different names*

### Comparing `lckytools-0.0.8/lckytools.egg-info/PKG-INFO` & `lckytools-0.0.9/lckytools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lckytools
-Version: 0.0.8
+Version: 0.0.9
 Author-email: LCKYN <t.pwawrit@lckyn.com>
 License: MIT License
         
         Copyright (c) 2024 pawarit thareechan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `lckytools-0.0.8/pyproject.toml` & `lckytools-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lckytools"
-version = "0.0.8"
+version = "0.0.9"
 readme = "README.md"
 authors = [{"name"="LCKYN", "email"="t.pwawrit@lckyn.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

