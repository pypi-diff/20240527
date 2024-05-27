# Comparing `tmp/jsonUts-1.0.2.tar.gz` & `tmp/jsonUts-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonUts-1.0.2.tar", last modified: Mon Apr 29 13:50:15 2024, max compression
+gzip compressed data, was "jsonUts-1.0.3.tar", last modified: Mon May 27 12:34:52 2024, max compression
```

## Comparing `jsonUts-1.0.2.tar` & `jsonUts-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 13:50:15.532738 jsonUts-1.0.2/
--rw-rw-rw-   0        0        0       83 2024-04-19 21:46:49.000000 jsonUts-1.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 jsonUts-1.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 jsonUts-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1648 2024-04-29 13:50:15.530739 jsonUts-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2024-04-19 21:45:12.000000 jsonUts-1.0.2/README.md
--rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 jsonUts-1.0.2/commands.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 13:50:15.501739 jsonUts-1.0.2/jsonUts/
--rw-rw-rw-   0        0        0     2649 2024-04-29 13:49:37.000000 jsonUts-1.0.2/jsonUts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 13:50:15.528735 jsonUts-1.0.2/jsonUts.egg-info/
--rw-rw-rw-   0        0        0     1648 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 13:50:15.532738 jsonUts-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-04-19 21:31:46.000000 jsonUts-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:34:52.044492 jsonUts-1.0.3/
+-rw-rw-rw-   0        0        0       83 2024-04-19 21:46:49.000000 jsonUts-1.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 jsonUts-1.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 jsonUts-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1700 2024-05-27 12:34:52.042488 jsonUts-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2024-05-27 12:33:36.000000 jsonUts-1.0.3/README.md
+-rw-rw-rw-   0        0        0      205 2024-05-27 12:32:02.000000 jsonUts-1.0.3/commands.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 12:34:51.939489 jsonUts-1.0.3/jsonUts/
+-rw-rw-rw-   0        0        0     2037 2024-05-27 12:34:21.000000 jsonUts-1.0.3/jsonUts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:34:52.040488 jsonUts-1.0.3/jsonUts.egg-info/
+-rw-rw-rw-   0        0        0     1700 2024-05-27 12:34:51.000000 jsonUts-1.0.3/jsonUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-27 12:34:51.000000 jsonUts-1.0.3/jsonUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:34:51.000000 jsonUts-1.0.3/jsonUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-27 12:34:51.000000 jsonUts-1.0.3/jsonUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      741 2024-05-27 12:32:44.000000 jsonUts-1.0.3/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 12:34:52.045492 jsonUts-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-04-19 21:31:46.000000 jsonUts-1.0.3/setup.py
```

### Comparing `jsonUts-1.0.2/LICENCE.txt` & `jsonUts-1.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `jsonUts-1.0.2/PKG-INFO` & `jsonUts-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonUts
-Version: 1.0.2
+Version: 1.0.3
 Summary: Json package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: jsonUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,18 @@
 #
 ### Installation
 
 ```sh
 pip install jsonUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/JsonUts
+
+
 ### Usage
 #
 #### Json sample
 ```json
 my_json =  {
     "person":{
         "name":"json uts",
```

### Comparing `jsonUts-1.0.2/README.md` & `jsonUts-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 #
 ### Installation
 
 ```sh
 pip install jsonUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/JsonUts
+
+
 ### Usage
 #
 #### Json sample
 ```json
 my_json =  {
     "person":{
         "name":"json uts",
```

### Comparing `jsonUts-1.0.2/jsonUts.egg-info/PKG-INFO` & `jsonUts-1.0.3/jsonUts.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonUts
-Version: 1.0.2
+Version: 1.0.3
 Summary: Json package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: jsonUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,18 @@
 #
 ### Installation
 
 ```sh
 pip install jsonUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/JsonUts
+
+
 ### Usage
 #
 #### Json sample
 ```json
 my_json =  {
     "person":{
         "name":"json uts",
```

### Comparing `jsonUts-1.0.2/setup.py` & `jsonUts-1.0.3/setup.py`

 * *Files identical despite different names*

