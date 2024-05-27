# Comparing `tmp/sqlUts-1.0.3.tar.gz` & `tmp/sqlUts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlUts-1.0.3.tar", last modified: Mon Apr 22 23:33:35 2024, max compression
+gzip compressed data, was "sqlUts-1.0.4.tar", last modified: Mon May 27 12:45:12 2024, max compression
```

## Comparing `sqlUts-1.0.3.tar` & `sqlUts-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 23:33:35.773630 sqlUts-1.0.3/
--rw-rw-rw-   0        0        0      387 2023-05-02 14:14:50.000000 sqlUts-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-05-02 14:14:50.000000 sqlUts-1.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-05-02 14:14:50.000000 sqlUts-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3658 2024-04-22 23:33:35.771629 sqlUts-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2679 2023-05-02 14:14:50.000000 sqlUts-1.0.3/README.md
--rw-rw-rw-   0        0        0      214 2024-04-22 21:38:54.000000 sqlUts-1.0.3/commands.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 23:33:35.773630 sqlUts-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      845 2024-04-22 23:33:29.000000 sqlUts-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:33:35.712632 sqlUts-1.0.3/sqlUts/
--rw-rw-rw-   0        0        0     1666 2024-04-22 23:33:05.000000 sqlUts-1.0.3/sqlUts/__init__.py
--rw-rw-rw-   0        0        0       17 2024-04-22 21:49:19.000000 sqlUts-1.0.3/sqlUts/version.py
-drwxrwxrwx   0        0        0        0 2024-04-22 23:33:35.769630 sqlUts-1.0.3/sqlUts.egg-info/
--rw-rw-rw-   0        0        0     3658 2024-04-22 23:33:35.000000 sqlUts-1.0.3/sqlUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-22 23:33:35.000000 sqlUts-1.0.3/sqlUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 23:33:35.000000 sqlUts-1.0.3/sqlUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-22 23:33:35.000000 sqlUts-1.0.3/sqlUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 23:33:35.000000 sqlUts-1.0.3/sqlUts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 12:45:12.728008 sqlUts-1.0.4/
+-rw-rw-rw-   0        0        0      387 2023-05-02 14:14:50.000000 sqlUts-1.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-05-02 14:14:50.000000 sqlUts-1.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-02 14:14:50.000000 sqlUts-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3707 2024-05-27 12:45:12.724009 sqlUts-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2728 2024-05-27 12:43:27.000000 sqlUts-1.0.4/README.md
+-rw-rw-rw-   0        0        0      206 2024-05-27 12:41:14.000000 sqlUts-1.0.4/commands.txt
+-rw-rw-rw-   0        0        0      133 2024-05-27 12:41:48.000000 sqlUts-1.0.4/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 12:45:12.728008 sqlUts-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      845 2024-05-27 12:42:32.000000 sqlUts-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:45:12.647006 sqlUts-1.0.4/sqlUts/
+-rw-rw-rw-   0        0        0     1666 2024-04-22 23:33:05.000000 sqlUts-1.0.4/sqlUts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:45:12.719008 sqlUts-1.0.4/sqlUts.egg-info/
+-rw-rw-rw-   0        0        0     3707 2024-05-27 12:45:12.000000 sqlUts-1.0.4/sqlUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-27 12:45:12.000000 sqlUts-1.0.4/sqlUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:45:12.000000 sqlUts-1.0.4/sqlUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-27 12:45:12.000000 sqlUts-1.0.4/sqlUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 12:45:12.000000 sqlUts-1.0.4/sqlUts.egg-info/top_level.txt
```

### Comparing `sqlUts-1.0.3/LICENCE.txt` & `sqlUts-1.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sqlUts-1.0.3/PKG-INFO` & `sqlUts-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlUts
-Version: 1.0.3
+Version: 1.0.4
 Summary: An orm package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: sqlUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,17 @@
 #
 ### Installation
 
 ```sh
 pip install dateUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/SqlUts
+
 ### Usage
 #
 #### sqlToDate
 ```py
 from dateUts import sqlToDate
 result = sqlToDate('1991-12-23')
 print(result)
```

### Comparing `sqlUts-1.0.3/README.md` & `sqlUts-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 #
 ### Installation
 
 ```sh
 pip install dateUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/SqlUts
+
 ### Usage
 #
 #### sqlToDate
 ```py
 from dateUts import sqlToDate
 result = sqlToDate('1991-12-23')
 print(result)
```

### Comparing `sqlUts-1.0.3/setup.py` & `sqlUts-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='sqlUts',
-  version='1.0.3',
+  version='1.0.4',
   description='An orm package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

### Comparing `sqlUts-1.0.3/sqlUts/__init__.py` & `sqlUts-1.0.4/sqlUts/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlUts-1.0.3/sqlUts.egg-info/PKG-INFO` & `sqlUts-1.0.4/sqlUts.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlUts
-Version: 1.0.3
+Version: 1.0.4
 Summary: An orm package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: sqlUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,14 +21,17 @@
 #
 ### Installation
 
 ```sh
 pip install dateUts
 ```
 
+## GitHub
+https://github.com/ZdekPyPi/SqlUts
+
 ### Usage
 #
 #### sqlToDate
 ```py
 from dateUts import sqlToDate
 result = sqlToDate('1991-12-23')
 print(result)
```

