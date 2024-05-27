# Comparing `tmp/tablemaster-1.2.2.tar.gz` & `tmp/tablemaster-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.2.2.tar", last modified: Mon May 20 11:46:29 2024, max compression
+gzip compressed data, was "tablemaster-1.2.3.tar", last modified: Mon May 27 03:21:55 2024, max compression
```

## Comparing `tablemaster-1.2.2.tar` & `tablemaster-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-20 11:46:29.965291 tablemaster-1.2.2/
--rw-r--r--   0 livid      (501) staff       (20)    11357 2024-05-20 11:04:14.000000 tablemaster-1.2.2/LICENSE
--rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-20 11:46:29.965106 tablemaster-1.2.2/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)     2560 2024-05-20 11:04:14.000000 tablemaster-1.2.2/README.md
--rw-r--r--   0 livid      (501) staff       (20)       38 2024-05-20 11:46:29.965331 tablemaster-1.2.2/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      517 2024-05-20 11:45:52.000000 tablemaster-1.2.2/setup.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-20 11:46:29.964252 tablemaster-1.2.2/tablemaster/
--rw-r--r--   0 livid      (501) staff       (20)      632 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)     1716 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/feishu.py
--rw-r--r--   0 livid      (501) staff       (20)     1138 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/gspread.py
--rw-r--r--   0 livid      (501) staff       (20)     3334 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/local.py
--rw-r--r--   0 livid      (501) staff       (20)     5829 2024-05-20 11:45:13.000000 tablemaster-1.2.2/tablemaster/mysql.py
--rw-r--r--   0 livid      (501) staff       (20)      810 2024-05-20 11:04:14.000000 tablemaster-1.2.2/tablemaster/utils.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2024-05-20 11:46:29.964911 tablemaster-1.2.2/tablemaster.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      451 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      332 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)       77 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       12 2024-05-20 11:46:29.000000 tablemaster-1.2.2/tablemaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 03:21:55.772473 tablemaster-1.2.3/
+-rw-rw-rw-   0        0        0    11357 2024-05-20 11:04:14.000000 tablemaster-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      468 2024-05-27 03:21:55.771462 tablemaster-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2560 2024-05-20 11:04:14.000000 tablemaster-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 03:21:55.772473 tablemaster-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      517 2024-05-27 03:20:45.000000 tablemaster-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:21:55.762939 tablemaster-1.2.3/tablemaster/
+-rw-rw-rw-   0        0        0      632 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/__init__.py
+-rw-rw-rw-   0        0        0     1716 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/feishu.py
+-rw-rw-rw-   0        0        0     1265 2024-05-27 03:19:37.000000 tablemaster-1.2.3/tablemaster/gspread.py
+-rw-rw-rw-   0        0        0     3334 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/local.py
+-rw-rw-rw-   0        0        0     5829 2024-05-20 11:45:13.000000 tablemaster-1.2.3/tablemaster/mysql.py
+-rw-rw-rw-   0        0        0      810 2024-05-20 11:04:14.000000 tablemaster-1.2.3/tablemaster/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 03:21:55.770431 tablemaster-1.2.3/tablemaster.egg-info/
+-rw-rw-rw-   0        0        0      468 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 03:21:55.000000 tablemaster-1.2.3/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.2.2/LICENSE` & `tablemaster-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.2/README.md` & `tablemaster-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.2/setup.py` & `tablemaster-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.2.2',
+    version='1.2.3',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.2.2/tablemaster/__init__.py` & `tablemaster-1.2.3/tablemaster/__init__.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.2/tablemaster/feishu.py` & `tablemaster-1.2.3/tablemaster/feishu.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.2/tablemaster/local.py` & `tablemaster-1.2.3/tablemaster/local.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.2/tablemaster/mysql.py` & `tablemaster-1.2.3/tablemaster/mysql.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.2/tablemaster/utils.py` & `tablemaster-1.2.3/tablemaster/utils.py`

 * *Files identical despite different names*

