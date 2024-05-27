# Comparing `tmp/xray_disease_detector-0.1.0.tar.gz` & `tmp/xray_disease_detector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xray_disease_detector-0.1.0.tar", last modified: Wed May 22 13:11:44 2024, max compression
+gzip compressed data, was "xray_disease_detector-0.1.1.tar", last modified: Mon May 27 04:21:13 2024, max compression
```

## Comparing `xray_disease_detector-0.1.0.tar` & `xray_disease_detector-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 13:11:44.351762 xray_disease_detector-0.1.0/
--rw-r--r--   0 k-on       (501) staff       (20)     1131 2024-05-22 13:11:44.351632 xray_disease_detector-0.1.0/PKG-INFO
--rw-r--r--   0 k-on       (501) staff       (20)      565 2024-05-22 13:01:46.000000 xray_disease_detector-0.1.0/README.md
--rw-r--r--   0 k-on       (501) staff       (20)       38 2024-05-22 13:11:44.351799 xray_disease_detector-0.1.0/setup.cfg
--rw-r--r--   0 k-on       (501) staff       (20)     1165 2024-05-22 13:11:40.000000 xray_disease_detector-0.1.0/setup.py
-drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 13:11:44.350798 xray_disease_detector-0.1.0/src/
-drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 13:11:44.351443 xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/
--rw-r--r--   0 k-on       (501) staff       (20)     1131 2024-05-22 13:11:44.000000 xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/PKG-INFO
--rw-r--r--   0 k-on       (501) staff       (20)      343 2024-05-22 13:11:44.000000 xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/SOURCES.txt
--rw-r--r--   0 k-on       (501) staff       (20)        1 2024-05-22 13:11:44.000000 xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/dependency_links.txt
--rw-r--r--   0 k-on       (501) staff       (20)       69 2024-05-22 13:11:44.000000 xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/entry_points.txt
--rw-r--r--   0 k-on       (501) staff       (20)       25 2024-05-22 13:11:44.000000 xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/requires.txt
--rw-r--r--   0 k-on       (501) staff       (20)       22 2024-05-22 13:11:44.000000 xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/top_level.txt
--rw-r--r--   0 k-on       (501) staff       (20)     1712 2024-05-22 13:05:42.000000 xray_disease_detector-0.1.0/src/xray_disease_detector.py
+drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-27 04:21:13.797901 xray_disease_detector-0.1.1/
+-rw-r--r--   0 k-on       (501) staff       (20)     1131 2024-05-27 04:21:13.797717 xray_disease_detector-0.1.1/PKG-INFO
+-rw-r--r--   0 k-on       (501) staff       (20)      565 2024-05-22 13:01:46.000000 xray_disease_detector-0.1.1/README.md
+-rw-r--r--   0 k-on       (501) staff       (20)       38 2024-05-27 04:21:13.798024 xray_disease_detector-0.1.1/setup.cfg
+-rw-r--r--   0 k-on       (501) staff       (20)     1165 2024-05-27 04:20:29.000000 xray_disease_detector-0.1.1/setup.py
+drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-27 04:21:13.796278 xray_disease_detector-0.1.1/src/
+drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-27 04:21:13.797475 xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/
+-rw-r--r--   0 k-on       (501) staff       (20)     1131 2024-05-27 04:21:13.000000 xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/PKG-INFO
+-rw-r--r--   0 k-on       (501) staff       (20)      343 2024-05-27 04:21:13.000000 xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 k-on       (501) staff       (20)        1 2024-05-27 04:21:13.000000 xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 k-on       (501) staff       (20)       69 2024-05-27 04:21:13.000000 xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/entry_points.txt
+-rw-r--r--   0 k-on       (501) staff       (20)       25 2024-05-27 04:21:13.000000 xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/requires.txt
+-rw-r--r--   0 k-on       (501) staff       (20)       22 2024-05-27 04:21:13.000000 xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/top_level.txt
+-rw-r--r--   0 k-on       (501) staff       (20)     1712 2024-05-22 13:05:42.000000 xray_disease_detector-0.1.1/src/xray_disease_detector.py
```

### Comparing `xray_disease_detector-0.1.0/PKG-INFO` & `xray_disease_detector-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xray_disease_detector
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for detecting diseases in X-ray images using a pre-trained PyTorch model
 Home-page: https://github.com/KONMIO34/xray_disease_detector
 Author: Gong Zhan
 Author-email: gongzhan34@yahoo.co.jp
 Project-URL: Bug Tracker, https://github.com/KONMIO34/xray_disease_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xray_disease_detector-0.1.0/README.md` & `xray_disease_detector-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xray_disease_detector-0.1.0/setup.py` & `xray_disease_detector-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xray_disease_detector",
-    version="0.1.0",
+    version="0.1.1",
     author="Gong Zhan",
     author_email="gongzhan34@yahoo.co.jp",
     description="A package for detecting diseases in X-ray images using a pre-trained PyTorch model",
     long_description=long_description,      
     long_description_content_type="text/markdown",
     url="https://github.com/KONMIO34/xray_disease_detector",
     project_urls={
```

### Comparing `xray_disease_detector-0.1.0/src/xray_disease_detector.egg-info/PKG-INFO` & `xray_disease_detector-0.1.1/src/xray_disease_detector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xray-disease-detector
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for detecting diseases in X-ray images using a pre-trained PyTorch model
 Home-page: https://github.com/KONMIO34/xray_disease_detector
 Author: Gong Zhan
 Author-email: gongzhan34@yahoo.co.jp
 Project-URL: Bug Tracker, https://github.com/KONMIO34/xray_disease_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xray_disease_detector-0.1.0/src/xray_disease_detector.py` & `xray_disease_detector-0.1.1/src/xray_disease_detector.py`

 * *Files identical despite different names*

