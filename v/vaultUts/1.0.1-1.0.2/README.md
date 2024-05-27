# Comparing `tmp/vaultUts-1.0.1.tar.gz` & `tmp/vaultUts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaultUts-1.0.1.tar", last modified: Thu May  2 12:04:16 2024, max compression
+gzip compressed data, was "vaultUts-1.0.2.tar", last modified: Mon May 27 12:27:30 2024, max compression
```

## Comparing `vaultUts-1.0.1.tar` & `vaultUts-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:04:16.915479 vaultUts-1.0.1/
--rw-rw-rw-   0        0        0       83 2024-05-02 11:26:30.000000 vaultUts-1.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-05-02 14:14:50.000000 vaultUts-1.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-05-02 14:14:50.000000 vaultUts-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1024 2024-05-02 12:04:16.913478 vaultUts-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-05-02 12:01:36.000000 vaultUts-1.0.1/README.md
--rw-rw-rw-   0        0        0      214 2024-04-22 21:38:54.000000 vaultUts-1.0.1/commands.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 12:04:16.916479 vaultUts-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      750 2024-05-02 12:04:04.000000 vaultUts-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:04:16.871474 vaultUts-1.0.1/vaultUts/
--rw-rw-rw-   0        0        0     2489 2024-05-02 12:04:01.000000 vaultUts-1.0.1/vaultUts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:04:16.911478 vaultUts-1.0.1/vaultUts.egg-info/
--rw-rw-rw-   0        0        0     1024 2024-05-02 12:04:16.000000 vaultUts-1.0.1/vaultUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-02 12:04:16.000000 vaultUts-1.0.1/vaultUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:04:16.000000 vaultUts-1.0.1/vaultUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 12:04:16.000000 vaultUts-1.0.1/vaultUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 12:04:16.000000 vaultUts-1.0.1/vaultUts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 12:27:30.115886 vaultUts-1.0.2/
+-rw-rw-rw-   0        0        0       83 2024-05-02 11:26:30.000000 vaultUts-1.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-05-02 14:14:50.000000 vaultUts-1.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-02 14:14:50.000000 vaultUts-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1077 2024-05-27 12:27:30.113886 vaultUts-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-27 12:26:31.000000 vaultUts-1.0.2/README.md
+-rw-rw-rw-   0        0        0      214 2024-04-22 21:38:54.000000 vaultUts-1.0.2/commands.txt
+-rw-rw-rw-   0        0        0      149 2024-05-27 12:19:43.000000 vaultUts-1.0.2/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 12:27:30.115886 vaultUts-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-27 12:27:15.000000 vaultUts-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:27:30.069886 vaultUts-1.0.2/vaultUts/
+-rw-rw-rw-   0        0        0     2489 2024-05-02 12:04:01.000000 vaultUts-1.0.2/vaultUts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:27:30.110884 vaultUts-1.0.2/vaultUts.egg-info/
+-rw-rw-rw-   0        0        0     1077 2024-05-27 12:27:29.000000 vaultUts-1.0.2/vaultUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-27 12:27:29.000000 vaultUts-1.0.2/vaultUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:27:29.000000 vaultUts-1.0.2/vaultUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 12:27:29.000000 vaultUts-1.0.2/vaultUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 12:27:29.000000 vaultUts-1.0.2/vaultUts.egg-info/top_level.txt
```

### Comparing `vaultUts-1.0.1/LICENCE.txt` & `vaultUts-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `vaultUts-1.0.1/PKG-INFO` & `vaultUts-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaultUts
-Version: 1.0.1
+Version: 1.0.2
 Summary: An orm package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: vaultUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,18 @@
 #
 ### Installation
 
 ```sh
 pip install vaultUts
 ```
 
+
+## GitHub
+https://github.com/ZdekPyPi/VaultUts
+
 ### Usage
 #
 #### link
 ```py
 from vaultUts import VaultLib
 
 vlt = VaultLib(
```

### Comparing `vaultUts-1.0.1/setup.py` & `vaultUts-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='vaultUts',
-  version='1.0.1',
+  version='1.0.2',
   description='An orm package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

### Comparing `vaultUts-1.0.1/vaultUts/__init__.py` & `vaultUts-1.0.2/vaultUts/__init__.py`

 * *Files identical despite different names*

### Comparing `vaultUts-1.0.1/vaultUts.egg-info/PKG-INFO` & `vaultUts-1.0.2/vaultUts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaultUts
-Version: 1.0.1
+Version: 1.0.2
 Summary: An orm package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: vaultUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,18 @@
 #
 ### Installation
 
 ```sh
 pip install vaultUts
 ```
 
+
+## GitHub
+https://github.com/ZdekPyPi/VaultUts
+
 ### Usage
 #
 #### link
 ```py
 from vaultUts import VaultLib
 
 vlt = VaultLib(
```

