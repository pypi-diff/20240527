# Comparing `tmp/online_scheduler-1.5.tar.gz` & `tmp/online_scheduler-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "online_scheduler-1.5.tar", last modified: Sat May 25 13:56:22 2024, max compression
+gzip compressed data, was "online_scheduler-1.6.tar", last modified: Mon May 27 04:55:24 2024, max compression
```

## Comparing `online_scheduler-1.5.tar` & `online_scheduler-1.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 13:56:22.720499 online_scheduler-1.5/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 13:56:22.720288 online_scheduler-1.5/PKG-INFO
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 13:56:22.719468 online_scheduler-1.5/online_scheduler/
--rw-r--r--   0 endo       (501) staff       (20)       54 2024-05-25 08:32:49.000000 online_scheduler-1.5/online_scheduler/__init__.py
--rw-r--r--   0 endo       (501) staff       (20)     2812 2024-05-25 13:45:43.000000 online_scheduler-1.5/online_scheduler/online_scheduler.py
-drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-25 13:56:22.720073 online_scheduler-1.5/online_scheduler.egg-info/
--rw-r--r--   0 endo       (501) staff       (20)      317 2024-05-25 13:56:22.000000 online_scheduler-1.5/online_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 endo       (501) staff       (20)      273 2024-05-25 13:56:22.000000 online_scheduler-1.5/online_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-25 13:56:22.000000 online_scheduler-1.5/online_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 13:56:22.000000 online_scheduler-1.5/online_scheduler.egg-info/requires.txt
--rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-25 13:56:22.000000 online_scheduler-1.5/online_scheduler.egg-info/top_level.txt
--rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-25 13:56:22.720548 online_scheduler-1.5/setup.cfg
--rw-r--r--   0 endo       (501) staff       (20)      529 2024-05-25 13:55:36.000000 online_scheduler-1.5/setup.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-27 04:55:24.851538 online_scheduler-1.6/
+-rw-r--r--   0 endo       (501) staff       (20)      334 2024-05-27 04:55:24.851271 online_scheduler-1.6/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      661 2024-05-27 04:48:56.000000 online_scheduler-1.6/README.md
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-27 04:55:24.850477 online_scheduler-1.6/online_scheduler/
+-rw-r--r--   0 endo       (501) staff       (20)       54 2024-05-25 08:32:49.000000 online_scheduler-1.6/online_scheduler/__init__.py
+-rw-r--r--   0 endo       (501) staff       (20)     2812 2024-05-25 13:45:43.000000 online_scheduler-1.6/online_scheduler/online_scheduler.py
+drwxr-xr-x   0 endo       (501) staff       (20)        0 2024-05-27 04:55:24.851035 online_scheduler-1.6/online_scheduler.egg-info/
+-rw-r--r--   0 endo       (501) staff       (20)      334 2024-05-27 04:55:24.000000 online_scheduler-1.6/online_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 endo       (501) staff       (20)      283 2024-05-27 04:55:24.000000 online_scheduler-1.6/online_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 endo       (501) staff       (20)        1 2024-05-27 04:55:24.000000 online_scheduler-1.6/online_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-27 04:55:24.000000 online_scheduler-1.6/online_scheduler.egg-info/requires.txt
+-rw-r--r--   0 endo       (501) staff       (20)       17 2024-05-27 04:55:24.000000 online_scheduler-1.6/online_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 endo       (501) staff       (20)       38 2024-05-27 04:55:24.851602 online_scheduler-1.6/setup.cfg
+-rw-r--r--   0 endo       (501) staff       (20)      546 2024-05-27 04:54:42.000000 online_scheduler-1.6/setup.py
```

### Comparing `online_scheduler-1.5/online_scheduler/online_scheduler.py` & `online_scheduler-1.6/online_scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `online_scheduler-1.5/setup.py` & `online_scheduler-1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 
 requires = ["requests>=2.14.2"]
 
 
 setup(
     name='online_scheduler',
-    version='1.5',
+    version='1.6',
     description='Awesome library',
-    url='https://github.com/2222041',
+    url='https://github.com/2222041/Online_Scheduler',
     author='2222041',
     author_email='s2222041@stu.musashino-u.ac.jp',
     license='MIT',
     keywords='sample setuptools development',
     packages=[
         "online_scheduler"#,
         #"online_scheduler.subpackage",
```

