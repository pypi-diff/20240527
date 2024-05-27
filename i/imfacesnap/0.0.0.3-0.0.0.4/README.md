# Comparing `tmp/imfacesnap-0.0.0.3.tar.gz` & `tmp/imfacesnap-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imfacesnap-0.0.0.3.tar", last modified: Thu May 23 13:54:43 2024, max compression
+gzip compressed data, was "imfacesnap-0.0.0.4.tar", last modified: Mon May 27 05:24:14 2024, max compression
```

## Comparing `imfacesnap-0.0.0.3.tar` & `imfacesnap-0.0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:54:43.467640 imfacesnap-0.0.0.3/
--rw-r--r--   0 kevin-personal   (501) staff       (20)     1065 2024-05-22 10:14:39.000000 imfacesnap-0.0.0.3/LICENSE
--rw-r--r--   0 kevin-personal   (501) staff       (20)       29 2024-05-22 11:08:26.000000 imfacesnap-0.0.0.3/MANIFEST.in
--rw-r--r--   0 kevin-personal   (501) staff       (20)      826 2024-05-23 13:54:43.467178 imfacesnap-0.0.0.3/PKG-INFO
--rw-r--r--   0 kevin-personal   (501) staff       (20)      537 2024-05-22 11:08:33.000000 imfacesnap-0.0.0.3/README.md
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:54:43.460930 imfacesnap-0.0.0.3/imfacesnap/
--rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.3/imfacesnap/__init__.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)       61 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.3/imfacesnap/__main__.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)     3402 2024-05-23 13:53:39.000000 imfacesnap-0.0.0.3/imfacesnap/main.py
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:54:43.466279 imfacesnap-0.0.0.3/imfacesnap/utils/
--rw-r--r--   0 kevin-personal   (501) staff       (20)    10838 2024-03-25 12:38:00.000000 imfacesnap-0.0.0.3/imfacesnap/utils/BlurDetector.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.3/imfacesnap/utils/__init__.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)     2187 2024-04-16 13:27:52.000000 imfacesnap-0.0.0.3/imfacesnap/utils/deepface_util.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)      196 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.3/imfacesnap/utils/tools.py
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:54:43.463186 imfacesnap-0.0.0.3/imfacesnap.egg-info/
--rw-r--r--   0 kevin-personal   (501) staff       (20)      826 2024-05-23 13:54:43.000000 imfacesnap-0.0.0.3/imfacesnap.egg-info/PKG-INFO
--rw-r--r--   0 kevin-personal   (501) staff       (20)      431 2024-05-23 13:54:43.000000 imfacesnap-0.0.0.3/imfacesnap.egg-info/SOURCES.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)        1 2024-05-23 13:54:43.000000 imfacesnap-0.0.0.3/imfacesnap.egg-info/dependency_links.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       52 2024-05-23 13:54:43.000000 imfacesnap-0.0.0.3/imfacesnap.egg-info/entry_points.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       20 2024-05-23 13:54:43.000000 imfacesnap-0.0.0.3/imfacesnap.egg-info/requires.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       11 2024-05-23 13:54:43.000000 imfacesnap-0.0.0.3/imfacesnap.egg-info/top_level.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       38 2024-05-23 13:54:43.467739 imfacesnap-0.0.0.3/setup.cfg
--rw-r--r--   0 kevin-personal   (501) staff       (20)     2795 2024-05-23 13:53:43.000000 imfacesnap-0.0.0.3/setup.py
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-27 05:24:14.343571 imfacesnap-0.0.0.4/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     1065 2024-05-22 10:14:39.000000 imfacesnap-0.0.0.4/LICENSE
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       29 2024-05-22 11:08:26.000000 imfacesnap-0.0.0.4/MANIFEST.in
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      826 2024-05-27 05:24:14.343003 imfacesnap-0.0.0.4/PKG-INFO
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      537 2024-05-22 11:08:33.000000 imfacesnap-0.0.0.4/README.md
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-27 05:24:14.337994 imfacesnap-0.0.0.4/imfacesnap/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.4/imfacesnap/__init__.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       61 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.4/imfacesnap/__main__.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     3400 2024-05-27 05:23:45.000000 imfacesnap-0.0.0.4/imfacesnap/main.py
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-27 05:24:14.342171 imfacesnap-0.0.0.4/imfacesnap/utils/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)    10838 2024-03-25 12:38:00.000000 imfacesnap-0.0.0.4/imfacesnap/utils/BlurDetector.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.4/imfacesnap/utils/__init__.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     2190 2024-05-27 05:23:57.000000 imfacesnap-0.0.0.4/imfacesnap/utils/deepface_util.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      196 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.4/imfacesnap/utils/tools.py
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-27 05:24:14.340487 imfacesnap-0.0.0.4/imfacesnap.egg-info/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      826 2024-05-27 05:24:14.000000 imfacesnap-0.0.0.4/imfacesnap.egg-info/PKG-INFO
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      431 2024-05-27 05:24:14.000000 imfacesnap-0.0.0.4/imfacesnap.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)        1 2024-05-27 05:24:14.000000 imfacesnap-0.0.0.4/imfacesnap.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       52 2024-05-27 05:24:14.000000 imfacesnap-0.0.0.4/imfacesnap.egg-info/entry_points.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       20 2024-05-27 05:24:14.000000 imfacesnap-0.0.0.4/imfacesnap.egg-info/requires.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       11 2024-05-27 05:24:14.000000 imfacesnap-0.0.0.4/imfacesnap.egg-info/top_level.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       38 2024-05-27 05:24:14.343666 imfacesnap-0.0.0.4/setup.cfg
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     2795 2024-05-27 05:23:34.000000 imfacesnap-0.0.0.4/setup.py
```

### Comparing `imfacesnap-0.0.0.3/LICENSE` & `imfacesnap-0.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.3/PKG-INFO` & `imfacesnap-0.0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imfacesnap
-Version: 0.0.0.3
+Version: 0.0.0.4
 Author: Kevin Snap
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deepfacesnap==0.0.2
```

### Comparing `imfacesnap-0.0.0.3/README.md` & `imfacesnap-0.0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.3/imfacesnap/main.py` & `imfacesnap-0.0.0.4/imfacesnap/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     generate_parser.add_argument("-o", "--output", help="directory to save image", required=True)
     generate_parser.add_argument("-d", "--detector", help="face detector", required=True)
     generate_parser.add_argument("-t", "--threshold", help="Face Detector Threshold", required=False, default=0.75)
     generate_parser.add_argument('-check_blurry', action='store_true')
 
     args = parser.parse_args()
 
-    version =  "0.0.0.4.2"
+    version =  "0.0.0.4"
     if args.version:
         os.environ.setdefault("DEEPFACE_HOME", "/app")
         print(version + str(os.getenv("DEEPFACE_HOME", default=str(Path.home()))))
         exit(0)
 
     elif args.command == "represent":
         try:
```

### Comparing `imfacesnap-0.0.0.3/imfacesnap/utils/BlurDetector.py` & `imfacesnap-0.0.0.4/imfacesnap/utils/BlurDetector.py`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.3/imfacesnap/utils/deepface_util.py` & `imfacesnap-0.0.0.4/imfacesnap/utils/deepface_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from deepfacey import DeepFace
+from deepfacesnap import DeepFace
 import uuid
 import cv2
 from imface.utils.tools import get_blurry_score
 
 models = [
   "VGG-Face", 
   "Facenet",
```

### Comparing `imfacesnap-0.0.0.3/imfacesnap.egg-info/PKG-INFO` & `imfacesnap-0.0.0.4/imfacesnap.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imfacesnap
-Version: 0.0.0.3
+Version: 0.0.0.4
 Author: Kevin Snap
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deepfacesnap==0.0.2
```

### Comparing `imfacesnap-0.0.0.3/setup.py` & `imfacesnap-0.0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 with open("README.md", "r") as file:
     description = file.read()
 
 requirements = ["deepfacesnap==0.0.2"]
 
 setup(
     name='imfacesnap',
-    version='0.0.0.3',
+    version='0.0.0.4',
     install_requires=requirements,
     packages=find_packages(),
     include_package_data=True,
     entry_points={"console_scripts": ["imfacesnap=imfacesnap.main:main"]},
     author="Kevin Snap",
     license="License :: OSI Approved :: MIT License",
     classifiers=[
```

