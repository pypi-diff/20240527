# Comparing `tmp/user_external_local-0.0.44.tar.gz` & `tmp/user_external_local-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_external_local-0.0.44.tar", last modified: Thu May 23 18:52:42 2024, max compression
+gzip compressed data, was "user_external_local-0.0.45.tar", last modified: Mon May 27 21:12:04 2024, max compression
```

## Comparing `user_external_local-0.0.44.tar` & `user_external_local-0.0.45.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.418931 user_external_local-0.0.44/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-23 18:52:42.418931 user_external_local-0.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-23 18:52:21.000000 user_external_local-0.0.44/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 18:52:21.000000 user_external_local-0.0.44/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:52:42.418931 user_external_local-0.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 18:52:21.000000 user_external_local-0.0.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.414931 user_external_local-0.0.44/user_external_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.418931 user_external_local-0.0.44/user_external_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:21.000000 user_external_local-0.0.44/user_external_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-23 18:52:21.000000 user_external_local-0.0.44/user_external_local/src/user_externals_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:52:42.418931 user_external_local-0.0.44/user_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 18:52:42.000000 user_external_local-0.0.44/user_external_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:12:04.823404 user_external_local-0.0.45/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 21:12:04.823404 user_external_local-0.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-27 21:11:43.000000 user_external_local-0.0.45/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-27 21:11:50.000000 user_external_local-0.0.45/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:12:04.823404 user_external_local-0.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-27 21:11:43.000000 user_external_local-0.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:12:04.819404 user_external_local-0.0.45/user_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:12:04.823404 user_external_local-0.0.45/user_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 21:11:43.000000 user_external_local-0.0.45/user_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-27 21:11:43.000000 user_external_local-0.0.45/user_external_local/src/user_externals_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:12:04.823404 user_external_local-0.0.45/user_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 21:12:04.000000 user_external_local-0.0.45/user_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-27 21:12:04.000000 user_external_local-0.0.45/user_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:12:04.000000 user_external_local-0.0.45/user_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 21:12:04.000000 user_external_local-0.0.45/user_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 21:12:04.000000 user_external_local-0.0.45/user_external_local.egg-info/top_level.txt
```

### Comparing `user_external_local-0.0.44/PKG-INFO` & `user_external_local-0.0.45/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.44
+Version: 0.0.45
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `user_external_local-0.0.44/README.md` & `user_external_local-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `user_external_local-0.0.44/setup.py` & `user_external_local-0.0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-external-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/user-external-local
-    version='0.0.44',
+    version='0.0.45',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="user-external-local",
```

### Comparing `user_external_local-0.0.44/user_external_local/src/user_externals_local.py` & `user_external_local-0.0.45/user_external_local/src/user_externals_local.py`

 * *Files identical despite different names*

### Comparing `user_external_local-0.0.44/user_external_local.egg-info/PKG-INFO` & `user_external_local-0.0.45/user_external_local.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-external-local
-Version: 0.0.44
+Version: 0.0.45
 Home-page: https://github.com/circles-zone/user-external-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

