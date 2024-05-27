# Comparing `tmp/TraceUts-0.0.4.tar.gz` & `tmp/traceUts-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceUts-0.0.4.tar", last modified: Tue May  2 14:41:28 2023, max compression
+gzip compressed data, was "traceUts-0.0.5.tar", last modified: Mon May 27 13:13:56 2024, max compression
```

## Comparing `TraceUts-0.0.4.tar` & `traceUts-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 14:41:28.745673 traceUts-0.0.4/
--rw-rw-rw-   0        0        0      156 2023-05-02 14:40:12.000000 traceUts-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-05-02 14:40:12.000000 traceUts-0.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-05-02 14:40:12.000000 traceUts-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      710 2023-05-02 14:41:28.744675 traceUts-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-02 14:40:12.000000 traceUts-0.0.4/README.md
--rw-rw-rw-   0        0        0      122 2023-05-02 14:40:12.000000 traceUts-0.0.4/commands.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 14:41:28.745673 traceUts-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      750 2023-05-02 14:41:10.000000 traceUts-0.0.4/setup.py
--rw-rw-rw-   0        0        0      181 2023-05-02 14:40:12.000000 traceUts-0.0.4/test.py
-drwxrwxrwx   0        0        0        0 2023-05-02 14:41:28.716750 traceUts-0.0.4/traceUts/
--rw-rw-rw-   0        0        0     6766 2023-05-02 14:41:04.000000 traceUts-0.0.4/traceUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 14:41:28.742681 traceUts-0.0.4/traceUts.egg-info/
--rw-rw-rw-   0        0        0      710 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:56.948274 traceUts-0.0.5/
+-rw-rw-rw-   0        0        0      156 2023-05-02 14:40:12.000000 traceUts-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-05-02 14:40:12.000000 traceUts-0.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-02 14:40:12.000000 traceUts-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      710 2024-05-27 13:13:56.944274 traceUts-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-02 14:40:12.000000 traceUts-0.0.5/README.md
+-rw-rw-rw-   0        0        0      209 2024-05-27 13:13:15.000000 traceUts-0.0.5/commands.txt
+-rw-rw-rw-   0        0        0      248 2024-05-27 13:11:35.000000 traceUts-0.0.5/run.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:13:56.949274 traceUts-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-27 13:13:48.000000 traceUts-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:56.878276 traceUts-0.0.5/traceUts/
+-rw-rw-rw-   0        0        0     6766 2023-05-02 14:41:04.000000 traceUts-0.0.5/traceUts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:13:56.934274 traceUts-0.0.5/traceUts.egg-info/
+-rw-rw-rw-   0        0        0      710 2024-05-27 13:13:56.000000 traceUts-0.0.5/traceUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-27 13:13:56.000000 traceUts-0.0.5/traceUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:13:56.000000 traceUts-0.0.5/traceUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 13:13:56.000000 traceUts-0.0.5/traceUts.egg-info/top_level.txt
```

### Comparing `traceUts-0.0.4/LICENCE.txt` & `traceUts-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `traceUts-0.0.4/PKG-INFO` & `traceUts-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceUts
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trace Functions package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: traceUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `traceUts-0.0.4/setup.py` & `traceUts-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='traceUts',
-  version='0.0.4',
+  version='0.0.5',
   description='Trace Functions package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

### Comparing `traceUts-0.0.4/traceUts/__init__.py` & `traceUts-0.0.5/traceUts/__init__.py`

 * *Files identical despite different names*

### Comparing `traceUts-0.0.4/traceUts.egg-info/PKG-INFO` & `traceUts-0.0.5/traceUts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceUts
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trace Functions package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: traceUts
 Classifier: Development Status :: 5 - Production/Stable
```

