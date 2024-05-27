# Comparing `tmp/distributaur-0.0.1.tar.gz` & `tmp/distributaur-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributaur-0.0.1.tar", last modified: Sat May 25 03:45:01 2024, max compression
+gzip compressed data, was "distributaur-0.0.3.tar", last modified: Mon May 27 20:55:52 2024, max compression
```

## Comparing `distributaur-0.0.1.tar` & `distributaur-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:45:01.426971 distributaur-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-25 03:44:55.000000 distributaur-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-25 03:44:55.000000 distributaur-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-25 03:45:01.426971 distributaur-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-25 03:44:55.000000 distributaur-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:45:01.422971 distributaur-0.0.1/distributaur/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 03:44:55.000000 distributaur-0.0.1/distributaur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-25 03:44:55.000000 distributaur-0.0.1/distributaur/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-05-25 03:44:55.000000 distributaur-0.0.1/distributaur/vast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 03:45:01.426971 distributaur-0.0.1/distributaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-25 03:45:01.000000 distributaur-0.0.1/distributaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-25 03:45:01.000000 distributaur-0.0.1/distributaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 03:45:01.000000 distributaur-0.0.1/distributaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-25 03:45:01.000000 distributaur-0.0.1/distributaur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 03:45:01.000000 distributaur-0.0.1/distributaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-25 03:44:55.000000 distributaur-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 03:45:01.426971 distributaur-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-25 03:44:55.000000 distributaur-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 03:44:59.000000 distributaur-0.0.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:55:52.655589 distributaur-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 20:55:45.000000 distributaur-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:55:45.000000 distributaur-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-27 20:55:52.655589 distributaur-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-27 20:55:45.000000 distributaur-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:55:52.655589 distributaur-0.0.3/distributaur/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 20:55:45.000000 distributaur-0.0.3/distributaur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-27 20:55:45.000000 distributaur-0.0.3/distributaur/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-05-27 20:55:45.000000 distributaur-0.0.3/distributaur/vast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:55:52.655589 distributaur-0.0.3/distributaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 20:55:52.000000 distributaur-0.0.3/distributaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 20:55:45.000000 distributaur-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:55:52.655589 distributaur-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-27 20:55:45.000000 distributaur-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 20:55:50.000000 distributaur-0.0.3/version.txt
```

### Comparing `distributaur-0.0.1/LICENSE` & `distributaur-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `distributaur-0.0.1/setup.py` & `distributaur-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 with open(os.path.join(file_path, "README.md"), "r") as fh:
     long_description = fh.read()
     long_description = long_description.split("\n")
     long_description = [line for line in long_description if not "<img" in line]
     long_description = "\n".join(long_description)
 
 with open(os.path.join(file_path, "version.txt"), "r") as fh:
-    print(fh.read())
-    version = fh.read()
+    version_content = fh.read()
+    print("Content from version.txt:", version_content)
+    version = version_content.split("\n")[0].strip()
 
 with open(os.path.join(file_path, "requirements.txt"), "r") as fh:
     install_requires = fh.read()
     install_requires = install_requires.split("\n")
     install_requires = [
         line.split("=")[0].split(">")[0].split("<")[0] for line in install_requires
     ]
 
+print("version:", version)
+
 setup(
     name="distributaur",
-    version="0.0.1",
+    version=version,
     description="Simple task manager and job queue for distributed rendering. Built on celery and redis.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RaccoonResearch/distributaur",
     author="Raccoon Research",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

