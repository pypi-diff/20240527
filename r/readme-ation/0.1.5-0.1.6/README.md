# Comparing `tmp/readme_ation-0.1.5.tar.gz` & `tmp/readme_ation-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ation-0.1.5.tar", last modified: Sun May 26 10:53:04 2024, max compression
+gzip compressed data, was "readme_ation-0.1.6.tar", last modified: Mon May 27 15:19:00 2024, max compression
```

## Comparing `readme_ation-0.1.5.tar` & `readme_ation-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-26 10:53:04.936212 readme_ation-0.1.5/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme_ation-0.1.5/LICENSE.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      432 2024-05-26 10:53:04.935652 readme_ation-0.1.5/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       27 2024-05-25 07:22:55.000000 readme_ation-0.1.5/README.md
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme_ation-0.1.5/pyproject.toml
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-26 10:53:04.933259 readme_ation-0.1.5/readme_ation/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       46 2024-05-26 07:02:18.000000 readme_ation-0.1.5/readme_ation/__init__.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     5010 2024-05-26 06:50:52.000000 readme_ation-0.1.5/readme_ation/readme_ation.py
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-26 10:53:04.935039 readme_ation-0.1.5/readme_ation.egg-info/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      432 2024-05-26 10:53:04.000000 readme_ation-0.1.5/readme_ation.egg-info/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      243 2024-05-26 10:53:04.000000 readme_ation-0.1.5/readme_ation.egg-info/SOURCES.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-26 10:53:04.000000 readme_ation-0.1.5/readme_ation.egg-info/dependency_links.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       13 2024-05-26 10:53:04.000000 readme_ation-0.1.5/readme_ation.egg-info/top_level.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-26 10:53:04.936406 readme_ation-0.1.5/setup.cfg
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      941 2024-05-26 10:52:46.000000 readme_ation-0.1.5/setup.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:19:00.650910 readme_ation-0.1.6/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme_ation-0.1.6/LICENSE.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1659 2024-05-27 15:19:00.650520 readme_ation-0.1.6/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1255 2024-05-27 15:16:02.000000 readme_ation-0.1.6/README.md
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme_ation-0.1.6/pyproject.toml
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:19:00.648360 readme_ation-0.1.6/readme_ation/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       46 2024-05-26 07:02:18.000000 readme_ation-0.1.6/readme_ation/__init__.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     7596 2024-05-27 15:01:45.000000 readme_ation-0.1.6/readme_ation/readme_ation.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:19:00.650128 readme_ation-0.1.6/readme_ation.egg-info/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1659 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      243 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       13 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/top_level.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-27 15:19:00.651000 readme_ation-0.1.6/setup.cfg
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      906 2024-05-27 15:06:15.000000 readme_ation-0.1.6/setup.py
```

### Comparing `readme_ation-0.1.5/LICENSE.txt` & `readme_ation-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `readme_ation-0.1.5/setup.py` & `readme_ation-0.1.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="readme-ation",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
-    # py_modules=['readme_ation'],
     install_requires=[
         # List dependencies here, e.g. 'requests>=2.25.1'
     ],
     entry_points={
         # 'console_scripts': [
         #     'main = main:log_versions_to_readme_on_successful_exit',  # Assuming you have a main function in my_script.py
         # ],
```

