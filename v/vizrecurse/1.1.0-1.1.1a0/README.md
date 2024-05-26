# Comparing `tmp/vizrecurse-1.1.0.tar.gz` & `tmp/vizrecurse-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizrecurse-1.1.0.tar", last modified: Sun May 26 20:08:15 2024, max compression
+gzip compressed data, was "vizrecurse-1.1.1a0.tar", last modified: Sun May 26 21:53:24 2024, max compression
```

## Comparing `vizrecurse-1.1.0.tar` & `vizrecurse-1.1.1a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 20:08:15.293039 vizrecurse-1.1.0/
--rw-r--r--   0 enso       (501) staff       (20)      359 2024-05-26 20:08:15.292856 vizrecurse-1.1.0/PKG-INFO
--rw-r--r--   0 enso       (501) staff       (20)     3036 2024-05-25 16:27:06.000000 vizrecurse-1.1.0/README.md
--rw-r--r--   0 enso       (501) staff       (20)       38 2024-05-26 20:08:15.293084 vizrecurse-1.1.0/setup.cfg
--rw-r--r--   0 enso       (501) staff       (20)     1173 2024-05-26 20:08:01.000000 vizrecurse-1.1.0/setup.py
-drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 20:08:15.291872 vizrecurse-1.1.0/vizrecurse/
--rw-r--r--   0 enso       (501) staff       (20)      229 2024-05-24 21:05:55.000000 vizrecurse-1.1.0/vizrecurse/__init__.py
--rw-r--r--   0 enso       (501) staff       (20)      433 2024-05-25 22:59:24.000000 vizrecurse-1.1.0/vizrecurse/debug.py
--rw-r--r--   0 enso       (501) staff       (20)     1573 2024-05-25 21:07:35.000000 vizrecurse-1.1.0/vizrecurse/display.py
--rw-r--r--   0 enso       (501) staff       (20)     2393 2024-05-25 23:18:42.000000 vizrecurse-1.1.0/vizrecurse/vizzy.py
-drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 20:08:15.292676 vizrecurse-1.1.0/vizrecurse.egg-info/
--rw-r--r--   0 enso       (501) staff       (20)      359 2024-05-26 20:08:15.000000 vizrecurse-1.1.0/vizrecurse.egg-info/PKG-INFO
--rw-r--r--   0 enso       (501) staff       (20)      272 2024-05-26 20:08:15.000000 vizrecurse-1.1.0/vizrecurse.egg-info/SOURCES.txt
--rw-r--r--   0 enso       (501) staff       (20)        1 2024-05-26 20:08:15.000000 vizrecurse-1.1.0/vizrecurse.egg-info/dependency_links.txt
--rw-r--r--   0 enso       (501) staff       (20)      394 2024-05-26 20:08:15.000000 vizrecurse-1.1.0/vizrecurse.egg-info/requires.txt
--rw-r--r--   0 enso       (501) staff       (20)       11 2024-05-26 20:08:15.000000 vizrecurse-1.1.0/vizrecurse.egg-info/top_level.txt
+drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 21:53:24.870842 vizrecurse-1.1.1a0/
+-rw-r--r--   0 enso       (501) staff       (20)      361 2024-05-26 21:53:24.870674 vizrecurse-1.1.1a0/PKG-INFO
+-rw-r--r--   0 enso       (501) staff       (20)     3118 2024-05-26 20:10:38.000000 vizrecurse-1.1.1a0/README.md
+-rw-r--r--   0 enso       (501) staff       (20)       38 2024-05-26 21:53:24.870888 vizrecurse-1.1.1a0/setup.cfg
+-rw-r--r--   0 enso       (501) staff       (20)     1174 2024-05-26 21:53:21.000000 vizrecurse-1.1.1a0/setup.py
+drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 21:53:24.869515 vizrecurse-1.1.1a0/vizrecurse/
+-rw-r--r--   0 enso       (501) staff       (20)      229 2024-05-24 21:05:55.000000 vizrecurse-1.1.1a0/vizrecurse/__init__.py
+-rw-r--r--   0 enso       (501) staff       (20)      433 2024-05-25 22:59:24.000000 vizrecurse-1.1.1a0/vizrecurse/debug.py
+-rw-r--r--   0 enso       (501) staff       (20)     1573 2024-05-25 21:07:35.000000 vizrecurse-1.1.1a0/vizrecurse/display.py
+-rw-r--r--   0 enso       (501) staff       (20)     2393 2024-05-25 23:18:42.000000 vizrecurse-1.1.1a0/vizrecurse/vizzy.py
+drwxr-xr-x   0 enso       (501) staff       (20)        0 2024-05-26 21:53:24.870426 vizrecurse-1.1.1a0/vizrecurse.egg-info/
+-rw-r--r--   0 enso       (501) staff       (20)      361 2024-05-26 21:53:24.000000 vizrecurse-1.1.1a0/vizrecurse.egg-info/PKG-INFO
+-rw-r--r--   0 enso       (501) staff       (20)      272 2024-05-26 21:53:24.000000 vizrecurse-1.1.1a0/vizrecurse.egg-info/SOURCES.txt
+-rw-r--r--   0 enso       (501) staff       (20)        1 2024-05-26 21:53:24.000000 vizrecurse-1.1.1a0/vizrecurse.egg-info/dependency_links.txt
+-rw-r--r--   0 enso       (501) staff       (20)      394 2024-05-26 21:53:24.000000 vizrecurse-1.1.1a0/vizrecurse.egg-info/requires.txt
+-rw-r--r--   0 enso       (501) staff       (20)       11 2024-05-26 21:53:24.000000 vizrecurse-1.1.1a0/vizrecurse.egg-info/top_level.txt
```

### Comparing `vizrecurse-1.1.0/README.md` & `vizrecurse-1.1.1a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 ### About viz.recurse
 viz.recurse is a bare-bones library to easily visualize recursion without any significant overhead on the part of the user. This library utilizes common graph and visualization libraries (networkx, matplotlib, pygraphviz).
 
+### Latest PyPi release [1.1.0]
+Visit https://pypi.org/project/vizrecurse/1.1.0/
+
 ### Requirements
 `Python 3.10.13`\
 `pip 23.0.1` (graphviz compatibility)\
 `brew install graphviz` (MacOS)\
 `pip3 install -r requirements.txt`
 
 If running into problems installing `pygraphviz`:
```

### Comparing `vizrecurse-1.1.0/setup.py` & `vizrecurse-1.1.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """PyPi vizrecurse setup"""
 from setuptools import setup, find_packages
 setup(
     name='vizrecurse',
-    version='1.1.0',
+    version='1.1.1a0',
     author='Cody Pedersen',
     description='Bare bones library to vizualize recursion with one line of code.',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3.10',
     'Operating System :: OS Independent',
     'Intended Audience :: Developers',
@@ -36,8 +36,7 @@
         "python-dateutil==2.9.0.post0",
         "six==1.16.0",
         "tomli==2.0.1",
         "tomlkit==0.12.5",
         "typing_extensions==4.12.0"
     ]
 )
-
```

### Comparing `vizrecurse-1.1.0/vizrecurse/display.py` & `vizrecurse-1.1.1a0/vizrecurse/display.py`

 * *Files identical despite different names*

### Comparing `vizrecurse-1.1.0/vizrecurse/vizzy.py` & `vizrecurse-1.1.1a0/vizrecurse/vizzy.py`

 * *Files identical despite different names*

