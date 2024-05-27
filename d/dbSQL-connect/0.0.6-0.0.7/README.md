# Comparing `tmp/dbSQL_connect-0.0.6.tar.gz` & `tmp/dbSQL_connect-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbSQL_connect-0.0.6.tar", last modified: Fri May 17 07:54:40 2024, max compression
+gzip compressed data, was "dbSQL_connect-0.0.7.tar", last modified: Mon May 27 19:29:26 2024, max compression
```

## Comparing `dbSQL_connect-0.0.6.tar` & `dbSQL_connect-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:54:40.237644 dbSQL_connect-0.0.6/
--rw-rw-rw-   0        0        0      423 2024-05-17 07:54:40.237644 dbSQL_connect-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-13 19:50:39.000000 dbSQL_connect-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 07:54:40.232658 dbSQL_connect-0.0.6/dbSQL_connect/
--rw-rw-rw-   0        0        0        0 2024-05-13 20:38:13.000000 dbSQL_connect-0.0.6/dbSQL_connect/__init__.py
--rw-rw-rw-   0        0        0     5963 2024-05-14 03:44:55.000000 dbSQL_connect-0.0.6/dbSQL_connect/_entry_points.py
--rw-rw-rw-   0        0        0    10277 2024-05-17 07:54:35.000000 dbSQL_connect-0.0.6/dbSQL_connect/_imp.py
--rw-rw-rw-   0        0        0    36807 2024-05-17 01:32:35.000000 dbSQL_connect-0.0.6/dbSQL_connect/requires.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:54:40.236647 dbSQL_connect-0.0.6/dbSQL_connect.egg-info/
--rw-rw-rw-   0        0        0      423 2024-05-17 07:54:40.000000 dbSQL_connect-0.0.6/dbSQL_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-05-17 07:54:40.000000 dbSQL_connect-0.0.6/dbSQL_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:54:40.000000 dbSQL_connect-0.0.6/dbSQL_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 07:54:40.000000 dbSQL_connect-0.0.6/dbSQL_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 07:54:40.000000 dbSQL_connect-0.0.6/dbSQL_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 07:54:40.238641 dbSQL_connect-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      685 2024-05-17 07:54:35.000000 dbSQL_connect-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:29:26.813400 dbSQL_connect-0.0.7/
+-rw-rw-rw-   0        0        0      398 2024-05-27 19:29:26.813400 dbSQL_connect-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-13 19:50:39.000000 dbSQL_connect-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 19:29:26.807415 dbSQL_connect-0.0.7/dbSQL_connect/
+-rw-rw-rw-   0        0        0        0 2024-05-13 20:38:13.000000 dbSQL_connect-0.0.7/dbSQL_connect/__init__.py
+-rw-rw-rw-   0        0        0     5963 2024-05-14 03:44:55.000000 dbSQL_connect-0.0.7/dbSQL_connect/_entry_points.py
+-rw-rw-rw-   0        0        0    10277 2024-05-17 07:54:35.000000 dbSQL_connect-0.0.7/dbSQL_connect/_imp.py
+-rw-rw-rw-   0        0        0    36807 2024-05-17 01:32:35.000000 dbSQL_connect-0.0.7/dbSQL_connect/requires.py
+drwxrwxrwx   0        0        0        0 2024-05-27 19:29:26.812403 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 19:29:26.000000 dbSQL_connect-0.0.7/dbSQL_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 19:29:26.813400 dbSQL_connect-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      656 2024-05-27 19:29:24.000000 dbSQL_connect-0.0.7/setup.py
```

### Comparing `dbSQL_connect-0.0.6/dbSQL_connect/_entry_points.py` & `dbSQL_connect-0.0.7/dbSQL_connect/_entry_points.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.6/dbSQL_connect/_imp.py` & `dbSQL_connect-0.0.7/dbSQL_connect/_imp.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.6/dbSQL_connect/requires.py` & `dbSQL_connect-0.0.7/dbSQL_connect/requires.py`

 * *Files identical despite different names*

### Comparing `dbSQL_connect-0.0.6/setup.py` & `dbSQL_connect-0.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='dbSQL_connect',
-  version='0.0.6',
+  version='0.0.7',
   author='virginxlub',
   author_email='vzlomka927@yandex.ru',
   description='This is the simplest module for quick work with files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['requests>=2.25.1'],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
-  keywords='dbSQL_connect',
 
   python_requires='>=3.6'
 )
```

