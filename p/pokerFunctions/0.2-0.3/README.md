# Comparing `tmp/pokerfunctions-0.2.tar.gz` & `tmp/pokerfunctions-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerfunctions-0.2.tar", last modified: Sun May 26 04:40:31 2024, max compression
+gzip compressed data, was "pokerfunctions-0.3.tar", last modified: Mon May 27 07:07:44 2024, max compression
```

## Comparing `pokerfunctions-0.2.tar` & `pokerfunctions-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-26 04:40:31.899477 pokerfunctions-0.2/
--rw-r--r--   0 jonah      (501) staff       (20)     2793 2024-05-26 04:40:31.899307 pokerfunctions-0.2/PKG-INFO
--rw-r--r--   0 jonah      (501) staff       (20)     2374 2024-05-26 04:24:32.000000 pokerfunctions-0.2/README.md
-drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-26 04:40:31.899156 pokerfunctions-0.2/pokerFunctions.egg-info/
--rw-r--r--   0 jonah      (501) staff       (20)     2793 2024-05-26 04:40:31.000000 pokerfunctions-0.2/pokerFunctions.egg-info/PKG-INFO
--rw-r--r--   0 jonah      (501) staff       (20)      170 2024-05-26 04:40:31.000000 pokerfunctions-0.2/pokerFunctions.egg-info/SOURCES.txt
--rw-r--r--   0 jonah      (501) staff       (20)        1 2024-05-26 04:40:31.000000 pokerfunctions-0.2/pokerFunctions.egg-info/dependency_links.txt
--rw-r--r--   0 jonah      (501) staff       (20)        1 2024-05-26 04:40:31.000000 pokerfunctions-0.2/pokerFunctions.egg-info/top_level.txt
--rw-r--r--   0 jonah      (501) staff       (20)       38 2024-05-26 04:40:31.899509 pokerfunctions-0.2/setup.cfg
--rw-r--r--   0 jonah      (501) staff       (20)      657 2024-05-26 04:37:23.000000 pokerfunctions-0.2/setup.py
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-27 07:07:44.182997 pokerfunctions-0.3/
+-rw-r--r--   0 jonah      (501) staff       (20)     2793 2024-05-27 07:07:44.182849 pokerfunctions-0.3/PKG-INFO
+-rw-r--r--   0 jonah      (501) staff       (20)     2374 2024-05-26 04:24:32.000000 pokerfunctions-0.3/README.md
+drwxr-xr-x   0 jonah      (501) staff       (20)        0 2024-05-27 07:07:44.182708 pokerfunctions-0.3/pokerFunctions.egg-info/
+-rw-r--r--   0 jonah      (501) staff       (20)     2793 2024-05-27 07:07:44.000000 pokerfunctions-0.3/pokerFunctions.egg-info/PKG-INFO
+-rw-r--r--   0 jonah      (501) staff       (20)      170 2024-05-27 07:07:44.000000 pokerfunctions-0.3/pokerFunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 jonah      (501) staff       (20)        1 2024-05-27 07:07:44.000000 pokerfunctions-0.3/pokerFunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 jonah      (501) staff       (20)        1 2024-05-27 07:07:44.000000 pokerfunctions-0.3/pokerFunctions.egg-info/top_level.txt
+-rw-r--r--   0 jonah      (501) staff       (20)       38 2024-05-27 07:07:44.183030 pokerfunctions-0.3/setup.cfg
+-rw-r--r--   0 jonah      (501) staff       (20)      657 2024-05-27 07:02:41.000000 pokerfunctions-0.3/setup.py
```

### Comparing `pokerfunctions-0.2/PKG-INFO` & `pokerfunctions-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerFunctions
-Version: 0.2
+Version: 0.3
 Summary: A package for poker functions
 Home-page: https://github.com/yourusername/pokerFunctions
 Author: Jonah Aden
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pokerfunctions-0.2/README.md` & `pokerfunctions-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pokerfunctions-0.2/pokerFunctions.egg-info/PKG-INFO` & `pokerfunctions-0.3/pokerFunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerFunctions
-Version: 0.2
+Version: 0.3
 Summary: A package for poker functions
 Home-page: https://github.com/yourusername/pokerFunctions
 Author: Jonah Aden
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pokerfunctions-0.2/setup.py` & `pokerfunctions-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pokerFunctions',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[ ],
     include_package_data=True,
     description='A package for poker functions',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Jonah Aden',
```

