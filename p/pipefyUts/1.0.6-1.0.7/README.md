# Comparing `tmp/pipefyUts-1.0.6.tar.gz` & `tmp/pipefyUts-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipefyUts-1.0.6.tar", last modified: Mon May 27 11:37:51 2024, max compression
+gzip compressed data, was "pipefyUts-1.0.7.tar", last modified: Mon May 27 11:46:13 2024, max compression
```

## Comparing `pipefyUts-1.0.6.tar` & `pipefyUts-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.486017 pipefyUts-1.0.6/
--rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 pipefyUts-1.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 pipefyUts-1.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       55 2024-05-23 13:46:23.000000 pipefyUts-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3816 2024-05-27 11:37:51.482017 pipefyUts-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2788 2024-05-27 11:35:46.000000 pipefyUts-1.0.6/README.md
--rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 pipefyUts-1.0.6/commands.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.429017 pipefyUts-1.0.6/pipefyUts/
--rw-rw-rw-   0        0        0     4652 2024-05-26 15:36:46.000000 pipefyUts-1.0.6/pipefyUts/__init__.py
--rw-rw-rw-   0        0        0     5561 2024-05-27 11:31:02.000000 pipefyUts-1.0.6/pipefyUts/card.py
-drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.480018 pipefyUts-1.0.6/pipefyUts/graphql/
--rw-rw-rw-   0        0        0      181 2024-05-22 22:11:18.000000 pipefyUts-1.0.6/pipefyUts/graphql/createCard.gql
--rw-rw-rw-   0        0        0       72 2024-05-26 15:37:07.000000 pipefyUts-1.0.6/pipefyUts/graphql/deleteCards.gql
--rw-rw-rw-   0        0        0      336 2024-05-22 19:41:50.000000 pipefyUts-1.0.6/pipefyUts/graphql/listCardsFromPhase.gql
--rw-rw-rw-   0        0        0      137 2024-05-23 00:58:59.000000 pipefyUts-1.0.6/pipefyUts/graphql/listMembers.gql
--rw-rw-rw-   0        0        0      109 2024-05-22 19:34:03.000000 pipefyUts-1.0.6/pipefyUts/graphql/listStartFormFields.gql
--rw-rw-rw-   0        0        0      146 2024-05-22 19:24:55.000000 pipefyUts-1.0.6/pipefyUts/graphql/presignedUrl.gql
-drwxrwxrwx   0        0        0        0 2024-05-27 11:37:51.465018 pipefyUts-1.0.6/pipefyUts.egg-info/
--rw-rw-rw-   0        0        0     3816 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-27 11:37:51.000000 pipefyUts-1.0.6/pipefyUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5081 2024-05-27 11:35:46.000000 pipefyUts-1.0.6/run.py
--rw-rw-rw-   0        0        0       42 2024-05-27 11:37:51.486017 pipefyUts-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-27 11:37:29.000000 pipefyUts-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:13.206833 pipefyUts-1.0.7/
+-rw-rw-rw-   0        0        0      465 2023-04-28 18:31:34.000000 pipefyUts-1.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 pipefyUts-1.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       55 2024-05-23 13:46:23.000000 pipefyUts-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3853 2024-05-27 11:46:12.997832 pipefyUts-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2825 2024-05-27 11:44:13.000000 pipefyUts-1.0.7/README.md
+-rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 pipefyUts-1.0.7/commands.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:12.744833 pipefyUts-1.0.7/pipefyUts/
+-rw-rw-rw-   0        0        0     4652 2024-05-26 15:36:46.000000 pipefyUts-1.0.7/pipefyUts/__init__.py
+-rw-rw-rw-   0        0        0     5561 2024-05-27 11:31:02.000000 pipefyUts-1.0.7/pipefyUts/card.py
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:12.994833 pipefyUts-1.0.7/pipefyUts/graphql/
+-rw-rw-rw-   0        0        0      181 2024-05-22 22:11:18.000000 pipefyUts-1.0.7/pipefyUts/graphql/createCard.gql
+-rw-rw-rw-   0        0        0       72 2024-05-26 15:37:07.000000 pipefyUts-1.0.7/pipefyUts/graphql/deleteCards.gql
+-rw-rw-rw-   0        0        0      336 2024-05-22 19:41:50.000000 pipefyUts-1.0.7/pipefyUts/graphql/listCardsFromPhase.gql
+-rw-rw-rw-   0        0        0      137 2024-05-23 00:58:59.000000 pipefyUts-1.0.7/pipefyUts/graphql/listMembers.gql
+-rw-rw-rw-   0        0        0      109 2024-05-22 19:34:03.000000 pipefyUts-1.0.7/pipefyUts/graphql/listStartFormFields.gql
+-rw-rw-rw-   0        0        0      146 2024-05-22 19:24:55.000000 pipefyUts-1.0.7/pipefyUts/graphql/presignedUrl.gql
+drwxrwxrwx   0        0        0        0 2024-05-27 11:46:12.788830 pipefyUts-1.0.7/pipefyUts.egg-info/
+-rw-rw-rw-   0        0        0     3853 2024-05-27 11:46:12.000000 pipefyUts-1.0.7/pipefyUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-27 11:46:12.000000 pipefyUts-1.0.7/pipefyUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 11:46:12.000000 pipefyUts-1.0.7/pipefyUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 11:46:12.000000 pipefyUts-1.0.7/pipefyUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-27 11:46:12.000000 pipefyUts-1.0.7/pipefyUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5081 2024-05-27 11:35:46.000000 pipefyUts-1.0.7/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 11:46:13.206833 pipefyUts-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-27 11:45:56.000000 pipefyUts-1.0.7/setup.py
```

### Comparing `pipefyUts-1.0.6/LICENCE.txt` & `pipefyUts-1.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.6/PKG-INFO` & `pipefyUts-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefyUts
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pipefy manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: pipefyUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 ### Installation
 
 ```sh
 pip install pipefyUts
 ```
 
 ## GitHub
-
+https://github.com/ZdekPyPi/PipefyUts
 
 
 ## Usage
 
 <!-- //==================================================== -->
 ## Auth
 ##### python code
```

### Comparing `pipefyUts-1.0.6/README.md` & `pipefyUts-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ### Installation
 
 ```sh
 pip install pipefyUts
 ```
 
 ## GitHub
-
+https://github.com/ZdekPyPi/PipefyUts
 
 
 ## Usage
 
 <!-- //==================================================== -->
 ## Auth
 ##### python code
```

### Comparing `pipefyUts-1.0.6/pipefyUts/__init__.py` & `pipefyUts-1.0.7/pipefyUts/__init__.py`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.6/pipefyUts/card.py` & `pipefyUts-1.0.7/pipefyUts/card.py`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.6/pipefyUts.egg-info/PKG-INFO` & `pipefyUts-1.0.7/pipefyUts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefyUts
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pipefy manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: pipefyUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 ### Installation
 
 ```sh
 pip install pipefyUts
 ```
 
 ## GitHub
-
+https://github.com/ZdekPyPi/PipefyUts
 
 
 ## Usage
 
 <!-- //==================================================== -->
 ## Auth
 ##### python code
```

### Comparing `pipefyUts-1.0.6/run.py` & `pipefyUts-1.0.7/run.py`

 * *Files identical despite different names*

### Comparing `pipefyUts-1.0.6/setup.py` & `pipefyUts-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='pipefyUts',
-  version='1.0.6',
+  version='1.0.7',
   description='Pipefy manipulator',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

