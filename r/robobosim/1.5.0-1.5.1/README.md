# Comparing `tmp/robobosim-1.5.0.tar.gz` & `tmp/robobosim-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robobosim-1.5.0.tar", last modified: Wed May 22 14:38:36 2024, max compression
+gzip compressed data, was "robobosim-1.5.1.tar", last modified: Mon May 27 13:14:18 2024, max compression
```

## Comparing `robobosim-1.5.0.tar` & `robobosim-1.5.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.036396 robobosim-1.5.0/
--rw-rw-rw-   0        0        0     7817 2024-05-22 14:36:21.000000 robobosim-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     1465 2024-05-22 14:38:36.033966 robobosim-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-05-22 14:36:21.000000 robobosim-1.5.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 14:38:36.036396 robobosim-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1487 2024-05-22 14:36:21.000000 robobosim-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:38:35.971011 robobosim-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 14:38:35.985525 robobosim-1.5.0/src/robobosim/
--rw-rw-rw-   0        0        0     5217 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/RoboboSim.py
--rw-rw-rw-   0        0        0      246 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/State.py
--rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.024919 robobosim-1.5.0/src/robobosim/processors/
--rw-rw-rw-   0        0        0     1313 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/AGVProcessor.py
--rw-rw-rw-   0        0        0     1012 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/AbstractProcessor.py
--rw-rw-rw-   0        0        0      482 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/ControlProcessor.py
--rw-rw-rw-   0        0        0     1934 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/LocationProcessor.py
--rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/__init__.py
--rw-rw-rw-   0        0        0     5458 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/remotelib.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.032961 robobosim-1.5.0/src/robobosim/utils/
--rw-rw-rw-   0        0        0      138 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/utils/ConnectionState.py
--rw-rw-rw-   0        0        0      919 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/utils/Message.py
--rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.016580 robobosim-1.5.0/src/robobosim.egg-info/
--rw-rw-rw-   0        0        0     1465 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:18.329989 robobosim-1.5.1/
+-rw-rw-rw-   0        0        0     7817 2024-05-22 14:36:21.000000 robobosim-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     1465 2024-05-27 13:14:18.329479 robobosim-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-05-22 14:36:21.000000 robobosim-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:14:18.329989 robobosim-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1487 2024-05-27 13:13:56.000000 robobosim-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:18.272929 robobosim-1.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:18.289946 robobosim-1.5.1/src/robobosim/
+-rw-rw-rw-   0        0        0     5217 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/RoboboSim.py
+-rw-rw-rw-   0        0        0      246 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/State.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:18.325475 robobosim-1.5.1/src/robobosim/processors/
+-rw-rw-rw-   0        0        0     1313 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/processors/AGVProcessor.py
+-rw-rw-rw-   0        0        0     1012 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/processors/AbstractProcessor.py
+-rw-rw-rw-   0        0        0      482 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/processors/ControlProcessor.py
+-rw-rw-rw-   0        0        0     1934 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/processors/LocationProcessor.py
+-rw-rw-rw-   0        0        0     2025 2024-05-27 13:13:18.000000 robobosim-1.5.1/src/robobosim/processors/ObjectLocationProcessor.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/processors/__init__.py
+-rw-rw-rw-   0        0        0     5458 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/remotelib.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:18.328477 robobosim-1.5.1/src/robobosim/utils/
+-rw-rw-rw-   0        0        0      138 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/utils/ConnectionState.py
+-rw-rw-rw-   0        0        0      919 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/utils/Message.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.1/src/robobosim/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:14:18.316957 robobosim-1.5.1/src/robobosim.egg-info/
+-rw-rw-rw-   0        0        0     1465 2024-05-27 13:14:18.000000 robobosim-1.5.1/src/robobosim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2024-05-27 13:14:18.000000 robobosim-1.5.1/src/robobosim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:14:18.000000 robobosim-1.5.1/src/robobosim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 13:14:18.000000 robobosim-1.5.1/src/robobosim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-27 13:14:18.000000 robobosim-1.5.1/src/robobosim.egg-info/top_level.txt
```

### Comparing `robobosim-1.5.0/LICENSE` & `robobosim-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/PKG-INFO` & `robobosim-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robobosim
-Version: 1.5.0
+Version: 1.5.1
 Summary: Robobo Sim remote control library
 Author: The Robobo Project
 Author-email: info@theroboboproject.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `robobosim-1.5.0/README.md` & `robobosim-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/setup.py` & `robobosim-1.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="robobosim",                     # This is the name of the package
-    version="1.5.0",                        # The initial release version
+    version="1.5.1",                        # The initial release version
     author="The Robobo Project",                     # Full name of the author
     author_email='info@theroboboproject.com',
     description="Robobo Sim remote control library",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     #repository_url="https://github.com/mintforpeople/robobosim.py",
     #packages=setuptools.find_packages(),    # List of all python modules to be installed
```

### Comparing `robobosim-1.5.0/src/robobosim/RoboboSim.py` & `robobosim-1.5.1/src/robobosim/RoboboSim.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/src/robobosim/processors/AGVProcessor.py` & `robobosim-1.5.1/src/robobosim/processors/AGVProcessor.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/src/robobosim/processors/AbstractProcessor.py` & `robobosim-1.5.1/src/robobosim/processors/AbstractProcessor.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/src/robobosim/processors/LocationProcessor.py` & `robobosim-1.5.1/src/robobosim/processors/LocationProcessor.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/src/robobosim/remotelib.py` & `robobosim-1.5.1/src/robobosim/remotelib.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/src/robobosim/utils/Message.py` & `robobosim-1.5.1/src/robobosim/utils/Message.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.5.0/src/robobosim.egg-info/PKG-INFO` & `robobosim-1.5.1/src/robobosim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robobosim
-Version: 1.5.0
+Version: 1.5.1
 Summary: Robobo Sim remote control library
 Author: The Robobo Project
 Author-email: info@theroboboproject.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `robobosim-1.5.0/src/robobosim.egg-info/SOURCES.txt` & `robobosim-1.5.1/src/robobosim.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 src/robobosim.egg-info/dependency_links.txt
 src/robobosim.egg-info/requires.txt
 src/robobosim.egg-info/top_level.txt
 src/robobosim/processors/AGVProcessor.py
 src/robobosim/processors/AbstractProcessor.py
 src/robobosim/processors/ControlProcessor.py
 src/robobosim/processors/LocationProcessor.py
+src/robobosim/processors/ObjectLocationProcessor.py
 src/robobosim/processors/__init__.py
 src/robobosim/utils/ConnectionState.py
 src/robobosim/utils/Message.py
 src/robobosim/utils/__init__.py
```

