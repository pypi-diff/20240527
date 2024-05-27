# Comparing `tmp/user_context_remote-0.0.84.tar.gz` & `tmp/user_context_remote-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_context_remote-0.0.84.tar", last modified: Fri May 24 21:20:01 2024, max compression
+gzip compressed data, was "user_context_remote-0.0.85.tar", last modified: Mon May 27 17:23:26 2024, max compression
```

## Comparing `user_context_remote-0.0.84.tar` & `user_context_remote-0.0.85.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 21:19:42.000000 user_context_remote-0.0.84/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.431029 user_context_remote-0.0.84/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:23:26.159505 user_context_remote-0.0.85/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 17:23:26.159505 user_context_remote-0.0.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-27 17:23:06.000000 user_context_remote-0.0.85/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-27 17:23:11.000000 user_context_remote-0.0.85/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:23:26.159505 user_context_remote-0.0.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-27 17:23:06.000000 user_context_remote-0.0.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:23:26.155505 user_context_remote-0.0.85/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:23:26.155505 user_context_remote-0.0.85/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:23:06.000000 user_context_remote-0.0.85/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-05-27 17:23:06.000000 user_context_remote-0.0.85/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:23:26.159505 user_context_remote-0.0.85/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 17:23:26.000000 user_context_remote-0.0.85/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 17:23:26.000000 user_context_remote-0.0.85/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:23:26.000000 user_context_remote-0.0.85/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 17:23:26.000000 user_context_remote-0.0.85/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 17:23:26.000000 user_context_remote-0.0.85/user_context_remote.egg-info/top_level.txt
```

### Comparing `user_context_remote-0.0.84/PKG-INFO` & `user_context_remote-0.0.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.84
+Version: 0.0.85
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user_context_remote-0.0.84/README.md` & `user_context_remote-0.0.85/README.md`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.84/pyproject.toml` & `user_context_remote-0.0.85/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.84/setup.py` & `user_context_remote-0.0.85/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.84',  # https://pypi.org/project/user-context-remote/
+    version='0.0.85',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user_context_remote-0.0.84/user_context_remote/src/user_context.py` & `user_context_remote-0.0.85/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.84/user_context_remote.egg-info/PKG-INFO` & `user_context_remote-0.0.85/user_context_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.84
+Version: 0.0.85
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

