# Comparing `tmp/impyrialtest-0.1.3.tar.gz` & `tmp/impyrialtest-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/impyrialtest-0.1.3.tar", last modified: Sun May 26 18:30:05 2024, max compression
+gzip compressed data, was "dist/impyrialtest-0.1.5.tar", last modified: Mon May 27 18:24:57 2024, max compression
```

## Comparing `impyrialtest-0.1.3.tar` & `impyrialtest-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.849838 impyrialtest-0.1.3/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      311 2024-05-26 18:30:05.849402 impyrialtest-0.1.3/PKG-INFO
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.842185 impyrialtest-0.1.3/impyrialTest/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      247 2024-05-26 18:03:46.000000 impyrialtest-0.1.3/impyrialTest/__init__.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.845952 impyrialtest-0.1.3/impyrialTest/length/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 impyrialtest-0.1.3/impyrialTest/length/__init__.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1221 2024-05-26 16:39:16.000000 impyrialtest-0.1.3/impyrialTest/length/api.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1387 2024-05-26 16:13:45.000000 impyrialtest-0.1.3/impyrialTest/length/core.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)      457 2024-05-26 16:13:45.000000 impyrialtest-0.1.3/impyrialTest/utils.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.848034 impyrialtest-0.1.3/impyrialTest/weight/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 impyrialtest-0.1.3/impyrialTest/weight/__init__.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1226 2024-05-26 16:40:48.000000 impyrialtest-0.1.3/impyrialTest/weight/api.py
--rw-r--r--   0 aelkhodary   (501) staff       (20)     1410 2024-05-26 18:03:13.000000 impyrialtest-0.1.3/impyrialTest/weight/core.py
-drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-26 18:30:05.848912 impyrialtest-0.1.3/impyrialTest.egg-info/
--rw-r--r--   0 aelkhodary   (501) staff       (20)      311 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/PKG-INFO
--rw-r--r--   0 aelkhodary   (501) staff       (20)      408 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/SOURCES.txt
--rw-r--r--   0 aelkhodary   (501) staff       (20)        1 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/dependency_links.txt
--rw-r--r--   0 aelkhodary   (501) staff       (20)        6 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/requires.txt
--rw-r--r--   0 aelkhodary   (501) staff       (20)       13 2024-05-26 18:30:05.000000 impyrialtest-0.1.3/impyrialTest.egg-info/top_level.txt
--rw-r--r--   0 aelkhodary   (501) staff       (20)       38 2024-05-26 18:30:05.849960 impyrialtest-0.1.3/setup.cfg
--rw-r--r--   0 aelkhodary   (501) staff       (20)      525 2024-05-26 18:29:57.000000 impyrialtest-0.1.3/setup.py
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-27 18:24:57.608941 impyrialtest-0.1.5/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1069 2024-05-27 18:06:11.000000 impyrialtest-0.1.5/LICENSE
+-rw-r--r--   0 aelkhodary   (501) staff       (20)       33 2024-05-27 18:07:31.000000 impyrialtest-0.1.5/MANIFEST.in
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      333 2024-05-27 18:24:57.608425 impyrialtest-0.1.5/PKG-INFO
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      585 2024-05-27 18:06:57.000000 impyrialtest-0.1.5/README.md
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-27 18:24:57.602214 impyrialtest-0.1.5/impyrialTest/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      247 2024-05-26 18:03:46.000000 impyrialtest-0.1.5/impyrialTest/__init__.py
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-27 18:24:57.606058 impyrialtest-0.1.5/impyrialTest/length/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 impyrialtest-0.1.5/impyrialTest/length/__init__.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1221 2024-05-26 16:39:16.000000 impyrialtest-0.1.5/impyrialTest/length/api.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1387 2024-05-26 16:13:45.000000 impyrialtest-0.1.5/impyrialTest/length/core.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      457 2024-05-26 16:13:45.000000 impyrialtest-0.1.5/impyrialTest/utils.py
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-27 18:24:57.607428 impyrialtest-0.1.5/impyrialTest/weight/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      140 2024-05-26 16:25:56.000000 impyrialtest-0.1.5/impyrialTest/weight/__init__.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1226 2024-05-26 16:40:48.000000 impyrialtest-0.1.5/impyrialTest/weight/api.py
+-rw-r--r--   0 aelkhodary   (501) staff       (20)     1410 2024-05-26 18:03:13.000000 impyrialtest-0.1.5/impyrialTest/weight/core.py
+drwxr-xr-x   0 aelkhodary   (501) staff       (20)        0 2024-05-27 18:24:57.607922 impyrialtest-0.1.5/impyrialTest.egg-info/
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      333 2024-05-27 18:24:57.000000 impyrialtest-0.1.5/impyrialTest.egg-info/PKG-INFO
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      438 2024-05-27 18:24:57.000000 impyrialtest-0.1.5/impyrialTest.egg-info/SOURCES.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)        1 2024-05-27 18:24:57.000000 impyrialtest-0.1.5/impyrialTest.egg-info/dependency_links.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)        6 2024-05-27 18:24:57.000000 impyrialtest-0.1.5/impyrialTest.egg-info/requires.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)       13 2024-05-27 18:24:57.000000 impyrialtest-0.1.5/impyrialTest.egg-info/top_level.txt
+-rw-r--r--   0 aelkhodary   (501) staff       (20)       38 2024-05-27 18:24:57.609037 impyrialtest-0.1.5/setup.cfg
+-rw-r--r--   0 aelkhodary   (501) staff       (20)      525 2024-05-27 18:24:38.000000 impyrialtest-0.1.5/setup.py
```

### Comparing `impyrialtest-0.1.3/impyrialTest/length/api.py` & `impyrialtest-0.1.5/impyrialTest/length/api.py`

 * *Files identical despite different names*

### Comparing `impyrialtest-0.1.3/impyrialTest/length/core.py` & `impyrialtest-0.1.5/impyrialTest/length/core.py`

 * *Files identical despite different names*

### Comparing `impyrialtest-0.1.3/impyrialTest/weight/api.py` & `impyrialtest-0.1.5/impyrialTest/weight/api.py`

 * *Files identical despite different names*

### Comparing `impyrialtest-0.1.3/impyrialTest/weight/core.py` & `impyrialtest-0.1.5/impyrialTest/weight/core.py`

 * *Files identical despite different names*

### Comparing `impyrialtest-0.1.3/setup.py` & `impyrialtest-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 # Call setup function
 setup(
     author="Ahmed Elkhodary",
     description="A package for converting imperial lengths and weights.",
     name="impyrialTest",
     packages=find_packages(include=["impyrialTest", "impyrialTest.*"]),
     install_requires=['numpy'],
-    version="0.1.3",
+    version="0.1.5",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

