# Comparing `tmp/timetrace-0.2.0.tar.gz` & `tmp/timetrace-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetrace-0.2.0.tar", last modified: Mon May 27 03:44:39 2024, max compression
+gzip compressed data, was "timetrace-0.2.2.tar", last modified: Mon May 27 04:09:27 2024, max compression
```

## Comparing `timetrace-0.2.0.tar` & `timetrace-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 03:44:39.256266 timetrace-0.2.0/
--rw-r--r--   0 gamouyugo   (501) staff       (20)      727 2024-05-27 03:44:39.255985 timetrace-0.2.0/PKG-INFO
--rw-r--r--   0 gamouyugo   (501) staff       (20)      289 2024-05-27 02:00:20.000000 timetrace-0.2.0/README.md
--rw-r--r--   0 gamouyugo   (501) staff       (20)       38 2024-05-27 03:44:39.256336 timetrace-0.2.0/setup.cfg
--rw-r--r--   0 gamouyugo   (501) staff       (20)      731 2024-05-27 03:44:24.000000 timetrace-0.2.0/setup.py
-drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 03:44:39.253790 timetrace-0.2.0/tests/
--rw-r--r--   0 gamouyugo   (501) staff       (20)      558 2024-05-27 01:43:22.000000 timetrace-0.2.0/tests/test_timetrace.py
-drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 03:44:39.254380 timetrace-0.2.0/timetrace/
--rw-r--r--   0 gamouyugo   (501) staff       (20)       33 2024-05-27 01:43:20.000000 timetrace-0.2.0/timetrace/__init__.py
--rw-r--r--   0 gamouyugo   (501) staff       (20)      976 2024-05-27 01:37:33.000000 timetrace-0.2.0/timetrace/timetrace.py
-drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 03:44:39.255646 timetrace-0.2.0/timetrace.egg-info/
--rw-r--r--   0 gamouyugo   (501) staff       (20)      727 2024-05-27 03:44:39.000000 timetrace-0.2.0/timetrace.egg-info/PKG-INFO
--rw-r--r--   0 gamouyugo   (501) staff       (20)      251 2024-05-27 03:44:39.000000 timetrace-0.2.0/timetrace.egg-info/SOURCES.txt
--rw-r--r--   0 gamouyugo   (501) staff       (20)        1 2024-05-27 03:44:39.000000 timetrace-0.2.0/timetrace.egg-info/dependency_links.txt
--rw-r--r--   0 gamouyugo   (501) staff       (20)       11 2024-05-27 03:44:39.000000 timetrace-0.2.0/timetrace.egg-info/requires.txt
--rw-r--r--   0 gamouyugo   (501) staff       (20)       10 2024-05-27 03:44:39.000000 timetrace-0.2.0/timetrace.egg-info/top_level.txt
+drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 04:09:27.732830 timetrace-0.2.2/
+-rw-r--r--   0 gamouyugo   (501) staff       (20)      727 2024-05-27 04:09:27.732518 timetrace-0.2.2/PKG-INFO
+-rw-r--r--   0 gamouyugo   (501) staff       (20)      289 2024-05-27 02:00:20.000000 timetrace-0.2.2/README.md
+-rw-r--r--   0 gamouyugo   (501) staff       (20)       38 2024-05-27 04:09:27.732904 timetrace-0.2.2/setup.cfg
+-rw-r--r--   0 gamouyugo   (501) staff       (20)      731 2024-05-27 04:08:55.000000 timetrace-0.2.2/setup.py
+drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 04:09:27.730178 timetrace-0.2.2/tests/
+-rw-r--r--   0 gamouyugo   (501) staff       (20)      558 2024-05-27 01:43:22.000000 timetrace-0.2.2/tests/test_timetrace.py
+drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 04:09:27.730872 timetrace-0.2.2/timetrace/
+-rw-r--r--   0 gamouyugo   (501) staff       (20)       33 2024-05-27 01:43:20.000000 timetrace-0.2.2/timetrace/__init__.py
+-rw-r--r--   0 gamouyugo   (501) staff       (20)     1002 2024-05-27 04:08:51.000000 timetrace-0.2.2/timetrace/timetrace.py
+drwxr-xr-x   0 gamouyugo   (501) staff       (20)        0 2024-05-27 04:09:27.732191 timetrace-0.2.2/timetrace.egg-info/
+-rw-r--r--   0 gamouyugo   (501) staff       (20)      727 2024-05-27 04:09:27.000000 timetrace-0.2.2/timetrace.egg-info/PKG-INFO
+-rw-r--r--   0 gamouyugo   (501) staff       (20)      251 2024-05-27 04:09:27.000000 timetrace-0.2.2/timetrace.egg-info/SOURCES.txt
+-rw-r--r--   0 gamouyugo   (501) staff       (20)        1 2024-05-27 04:09:27.000000 timetrace-0.2.2/timetrace.egg-info/dependency_links.txt
+-rw-r--r--   0 gamouyugo   (501) staff       (20)       11 2024-05-27 04:09:27.000000 timetrace-0.2.2/timetrace.egg-info/requires.txt
+-rw-r--r--   0 gamouyugo   (501) staff       (20)       10 2024-05-27 04:09:27.000000 timetrace-0.2.2/timetrace.egg-info/top_level.txt
```

### Comparing `timetrace-0.2.0/PKG-INFO` & `timetrace-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetrace
-Version: 0.2.0
+Version: 0.2.2
 Summary: A simple performance tracing and visualization library for Python
 Author: namake
 Author-email: s2222102@stu.musashino-u.ac.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `timetrace-0.2.0/setup.py` & `timetrace-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='timetrace',
     packages=['timetrace'],
     
-    version='0.2.0',
+    version='0.2.2',
     
     license='MIT',
     
     install_requires=['matplotlib'],
     
     author='namake',
     author_email='s2222102@stu.musashino-u.ac.jp',
```

### Comparing `timetrace-0.2.0/tests/test_timetrace.py` & `timetrace-0.2.2/tests/test_timetrace.py`

 * *Files identical despite different names*

### Comparing `timetrace-0.2.0/timetrace/timetrace.py` & `timetrace-0.2.2/timetrace/timetrace.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,7 +27,9 @@
         
         plt.figure(figsize=(10, 5))
         plt.bar(func_names, times, color='skyblue')
         plt.xlabel('Function Name')
         plt.ylabel('Execution Time (s)')
         plt.title('Function Execution Time')
         plt.show()
+
+        self.records = []
```

### Comparing `timetrace-0.2.0/timetrace.egg-info/PKG-INFO` & `timetrace-0.2.2/timetrace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetrace
-Version: 0.2.0
+Version: 0.2.2
 Summary: A simple performance tracing and visualization library for Python
 Author: namake
 Author-email: s2222102@stu.musashino-u.ac.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

