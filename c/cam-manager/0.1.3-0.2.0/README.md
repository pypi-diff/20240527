# Comparing `tmp/cam_manager-0.1.3.tar.gz` & `tmp/cam_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cam_manager-0.1.3.tar", last modified: Sun May 26 20:38:17 2024, max compression
+gzip compressed data, was "cam_manager-0.2.0.tar", last modified: Sun May 26 21:42:08 2024, max compression
```

## Comparing `cam_manager-0.1.3.tar` & `cam_manager-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:38:17.567403 cam_manager-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 20:38:13.000000 cam_manager-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-26 20:38:17.567403 cam_manager-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-26 20:38:13.000000 cam_manager-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:38:17.567403 cam_manager-0.1.3/cam_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_effects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:38:17.567403 cam_manager-0.1.3/cam_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:38:17.567403 cam_manager-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-26 20:38:13.000000 cam_manager-0.1.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)  6534387 2024-05-26 20:38:14.000000 cam_manager-0.1.3/yolov8n.pt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:08.686006 cam_manager-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-26 21:42:08.686006 cam_manager-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-26 21:42:04.000000 cam_manager-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:08.682006 cam_manager-0.2.0/cam_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-26 21:42:04.000000 cam_manager-0.2.0/cam_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-26 21:42:04.000000 cam_manager-0.2.0/cam_manager/cam_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-26 21:42:04.000000 cam_manager-0.2.0/cam_manager/cam_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-26 21:42:04.000000 cam_manager-0.2.0/cam_manager/cam_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 21:42:04.000000 cam_manager-0.2.0/cam_manager/cam_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-26 21:42:04.000000 cam_manager-0.2.0/cam_manager/cam_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:42:08.682006 cam_manager-0.2.0/cam_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-26 21:42:08.000000 cam_manager-0.2.0/cam_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-26 21:42:08.000000 cam_manager-0.2.0/cam_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:42:08.000000 cam_manager-0.2.0/cam_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-26 21:42:08.000000 cam_manager-0.2.0/cam_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 21:42:08.000000 cam_manager-0.2.0/cam_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:42:08.686006 cam_manager-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-26 21:42:04.000000 cam_manager-0.2.0/setup.py
```

### Comparing `cam_manager-0.1.3/PKG-INFO` & `cam_manager-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.1.3
+Version: 0.2.0
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: opencv-python
+Requires-Dist: pytorch==2.2.2
+Requires-Dist: torchaudio==2.2.2
+Requires-Dist: torchvision==0.17.2
+Requires-Dist: setuptools==69.5.1
+Requires-Dist: ultralytics==8.2.22
+Requires-Dist: opencv-python==4.9.0.80
 
 CamManager - Methods
 
 __init__()
 Initializes a CamManager instance.
 
 --------------------------------------------------
```

### Comparing `cam_manager-0.1.3/README.md` & `cam_manager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cam_manager-0.1.3/cam_manager/cam_control.py` & `cam_manager-0.2.0/cam_manager/cam_control.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.1.3/cam_manager/cam_effects.py` & `cam_manager-0.2.0/cam_manager/cam_effects.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.1.3/cam_manager/cam_info.py` & `cam_manager-0.2.0/cam_manager/cam_info.py`

 * *Files identical despite different names*

### Comparing `cam_manager-0.1.3/cam_manager.egg-info/PKG-INFO` & `cam_manager-0.2.0/cam_manager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.1.3
+Version: 0.2.0
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: opencv-python
+Requires-Dist: pytorch==2.2.2
+Requires-Dist: torchaudio==2.2.2
+Requires-Dist: torchvision==0.17.2
+Requires-Dist: setuptools==69.5.1
+Requires-Dist: ultralytics==8.2.22
+Requires-Dist: opencv-python==4.9.0.80
 
 CamManager - Methods
 
 __init__()
 Initializes a CamManager instance.
 
 --------------------------------------------------
```

### Comparing `cam_manager-0.1.3/setup.py` & `cam_manager-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import setup, find_packages
 
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 setup(
-    version = "0.1.3",
+    version = "0.2.0",
     name = "cam_manager",
     description = "A camera management library to easily handle cameras with OpenCV.",
 
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
 
     author = "snatev",
     author_email = "snatev@proton.me",
     url = "https://github.com/snatev/cam-manager",
 
-    include_package_data = True,
-
     packages = find_packages(),
-    install_requires = [
-        "opencv-python"
-    ],
+    install_requires = requirements,
 
     classifiers = [
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
```

