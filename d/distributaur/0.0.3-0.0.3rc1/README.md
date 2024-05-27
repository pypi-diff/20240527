# Comparing `tmp/distributaur-0.0.3.tar.gz` & `tmp/distributaur-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributaur-0.0.3.tar", last modified: Mon May 27 20:55:52 2024, max compression
+gzip compressed data, was "distributaur-0.0.3rc1.tar", last modified: Mon May 27 21:03:45 2024, max compression
```

## Comparing `distributaur-0.0.3.tar` & `distributaur-0.0.3rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:55:52.655589 distributaur-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 20:55:45.000000 distributaur-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:55:45.000000 distributaur-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-27 20:55:52.655589 distributaur-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-27 20:55:45.000000 distributaur-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:55:52.655589 distributaur-0.0.3/distributaur/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 20:55:45.000000 distributaur-0.0.3/distributaur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-27 20:55:45.000000 distributaur-0.0.3/distributaur/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-05-27 20:55:45.000000 distributaur-0.0.3/distributaur/vast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:55:52.655589 distributaur-0.0.3/distributaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 20:55:45.000000 distributaur-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:55:52.655589 distributaur-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-27 20:55:45.000000 distributaur-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 20:55:50.000000 distributaur-0.0.3/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:03:45.538653 distributaur-0.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-27 21:03:45.538653 distributaur-0.0.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:03:45.538653 distributaur-0.0.3rc1/distributaur/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/distributaur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/distributaur/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/distributaur/vast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:03:45.538653 distributaur-0.0.3rc1/distributaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-27 21:03:45.000000 distributaur-0.0.3rc1/distributaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 21:03:45.000000 distributaur-0.0.3rc1/distributaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:03:45.000000 distributaur-0.0.3rc1/distributaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 21:03:45.000000 distributaur-0.0.3rc1/distributaur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 21:03:45.000000 distributaur-0.0.3rc1/distributaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:03:45.538653 distributaur-0.0.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-27 21:03:41.000000 distributaur-0.0.3rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 21:03:43.000000 distributaur-0.0.3rc1/version.txt
```

### Comparing `distributaur-0.0.3/LICENSE` & `distributaur-0.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `distributaur-0.0.3/PKG-INFO` & `distributaur-0.0.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distributaur
-Version: 0.0.3
+Version: 0.0.3rc1
 Summary: Simple task manager and job queue for distributed rendering. Built on celery and redis.
 Home-page: https://github.com/RaccoonResearch/distributaur
 Author: Raccoon Research
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `distributaur-0.0.3/README.md` & `distributaur-0.0.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `distributaur-0.0.3/distributaur/core.py` & `distributaur-0.0.3rc1/distributaur/core.py`

 * *Files identical despite different names*

### Comparing `distributaur-0.0.3/distributaur/vast.py` & `distributaur-0.0.3rc1/distributaur/vast.py`

 * *Files identical despite different names*

### Comparing `distributaur-0.0.3/distributaur.egg-info/PKG-INFO` & `distributaur-0.0.3rc1/distributaur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distributaur
-Version: 0.0.3
+Version: 0.0.3rc1
 Summary: Simple task manager and job queue for distributed rendering. Built on celery and redis.
 Home-page: https://github.com/RaccoonResearch/distributaur
 Author: Raccoon Research
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `distributaur-0.0.3/setup.py` & `distributaur-0.0.3rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,23 @@
     long_description = fh.read()
     long_description = long_description.split("\n")
     long_description = [line for line in long_description if not "<img" in line]
     long_description = "\n".join(long_description)
 
 with open(os.path.join(file_path, "version.txt"), "r") as fh:
     version_content = fh.read()
-    print("Content from version.txt:", version_content)
     version = version_content.split("\n")[0].strip()
 
 with open(os.path.join(file_path, "requirements.txt"), "r") as fh:
     install_requires = fh.read()
     install_requires = install_requires.split("\n")
     install_requires = [
         line.split("=")[0].split(">")[0].split("<")[0] for line in install_requires
     ]
 
-print("version:", version)
-
 setup(
     name="distributaur",
     version=version,
     description="Simple task manager and job queue for distributed rendering. Built on celery and redis.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RaccoonResearch/distributaur",
```

