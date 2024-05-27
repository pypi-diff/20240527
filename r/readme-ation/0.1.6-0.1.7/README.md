# Comparing `tmp/readme_ation-0.1.6.tar.gz` & `tmp/readme_ation-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ation-0.1.6.tar", last modified: Mon May 27 15:19:00 2024, max compression
+gzip compressed data, was "readme_ation-0.1.7.tar", last modified: Mon May 27 15:22:02 2024, max compression
```

## Comparing `readme_ation-0.1.6.tar` & `readme_ation-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:19:00.650910 readme_ation-0.1.6/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme_ation-0.1.6/LICENSE.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1659 2024-05-27 15:19:00.650520 readme_ation-0.1.6/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1255 2024-05-27 15:16:02.000000 readme_ation-0.1.6/README.md
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme_ation-0.1.6/pyproject.toml
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:19:00.648360 readme_ation-0.1.6/readme_ation/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       46 2024-05-26 07:02:18.000000 readme_ation-0.1.6/readme_ation/__init__.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     7596 2024-05-27 15:01:45.000000 readme_ation-0.1.6/readme_ation/readme_ation.py
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:19:00.650128 readme_ation-0.1.6/readme_ation.egg-info/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1659 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      243 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/SOURCES.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/dependency_links.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       13 2024-05-27 15:19:00.000000 readme_ation-0.1.6/readme_ation.egg-info/top_level.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-27 15:19:00.651000 readme_ation-0.1.6/setup.cfg
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      906 2024-05-27 15:06:15.000000 readme_ation-0.1.6/setup.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:22:02.626156 readme_ation-0.1.7/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme_ation-0.1.7/LICENSE.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1659 2024-05-27 15:22:02.625496 readme_ation-0.1.7/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1255 2024-05-27 15:16:02.000000 readme_ation-0.1.7/README.md
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme_ation-0.1.7/pyproject.toml
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:22:02.620170 readme_ation-0.1.7/readme_ation/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       99 2024-05-27 15:21:05.000000 readme_ation-0.1.7/readme_ation/__init__.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     7596 2024-05-27 15:01:45.000000 readme_ation-0.1.7/readme_ation/readme_ation.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-27 15:22:02.624868 readme_ation-0.1.7/readme_ation.egg-info/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1659 2024-05-27 15:22:02.000000 readme_ation-0.1.7/readme_ation.egg-info/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      243 2024-05-27 15:22:02.000000 readme_ation-0.1.7/readme_ation.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-27 15:22:02.000000 readme_ation-0.1.7/readme_ation.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       13 2024-05-27 15:22:02.000000 readme_ation-0.1.7/readme_ation.egg-info/top_level.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-27 15:22:02.626345 readme_ation-0.1.7/setup.cfg
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      906 2024-05-27 15:21:45.000000 readme_ation-0.1.7/setup.py
```

### Comparing `readme_ation-0.1.6/LICENSE.txt` & `readme_ation-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `readme_ation-0.1.6/PKG-INFO` & `readme_ation-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-ation
-Version: 0.1.6
+Version: 0.1.7
 Summary: A README.md generation tool
 Home-page: https://github.com/yourusername/your-repo
 Author: Charles Feinn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `readme_ation-0.1.6/README.md` & `readme_ation-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `readme_ation-0.1.6/readme_ation/readme_ation.py` & `readme_ation-0.1.7/readme_ation/readme_ation.py`

 * *Files identical despite different names*

### Comparing `readme_ation-0.1.6/readme_ation.egg-info/PKG-INFO` & `readme_ation-0.1.7/readme_ation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-ation
-Version: 0.1.6
+Version: 0.1.7
 Summary: A README.md generation tool
 Home-page: https://github.com/yourusername/your-repo
 Author: Charles Feinn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `readme_ation-0.1.6/setup.py` & `readme_ation-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="readme-ation",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
         # List dependencies here, e.g. 'requests>=2.25.1'
     ],
     entry_points={
         # 'console_scripts': [
         #     'main = main:log_versions_to_readme_on_successful_exit',  # Assuming you have a main function in my_script.py
```

