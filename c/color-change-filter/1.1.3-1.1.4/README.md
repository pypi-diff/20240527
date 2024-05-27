# Comparing `tmp/color_change_filter-1.1.3.tar.gz` & `tmp/color_change_filter-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_change_filter-1.1.3.tar", last modified: Mon May 27 05:25:30 2024, max compression
+gzip compressed data, was "color_change_filter-1.1.4.tar", last modified: Mon May 27 05:30:58 2024, max compression
```

## Comparing `color_change_filter-1.1.3.tar` & `color_change_filter-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:25:30.451128 color_change_filter-1.1.3/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       24 2024-05-24 18:09:24.000000 color_change_filter-1.1.3/.gitignore
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1627 2024-05-27 05:25:30.450890 color_change_filter-1.1.3/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1097 2024-05-27 05:24:34.000000 color_change_filter-1.1.3/README.md
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       10 2024-05-24 18:09:24.000000 color_change_filter-1.1.3/requirements.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-27 05:25:30.451189 color_change_filter-1.1.3/setup.cfg
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      995 2024-05-27 05:24:55.000000 color_change_filter-1.1.3/setup.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:25:30.449250 color_change_filter-1.1.3/src/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       36 2024-05-26 10:08:09.000000 color_change_filter-1.1.3/src/__init__.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:25:30.450250 color_change_filter-1.1.3/src/color_change_filter.egg-info/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1627 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      373 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/SOURCES.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/dependency_links.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/entry_points.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/requires.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/top_level.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4799 2024-05-27 04:57:31.000000 color_change_filter-1.1.3/src/color_change_filter.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:30:58.055650 color_change_filter-1.1.4/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       24 2024-05-24 18:09:24.000000 color_change_filter-1.1.4/.gitignore
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1661 2024-05-27 05:30:58.055349 color_change_filter-1.1.4/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1131 2024-05-27 05:29:45.000000 color_change_filter-1.1.4/README.md
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       10 2024-05-24 18:09:24.000000 color_change_filter-1.1.4/requirements.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-27 05:30:58.055704 color_change_filter-1.1.4/setup.cfg
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      995 2024-05-27 05:30:49.000000 color_change_filter-1.1.4/setup.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:30:58.053938 color_change_filter-1.1.4/src/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       36 2024-05-26 10:08:09.000000 color_change_filter-1.1.4/src/__init__.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:30:58.054951 color_change_filter-1.1.4/src/color_change_filter.egg-info/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1661 2024-05-27 05:30:58.000000 color_change_filter-1.1.4/src/color_change_filter.egg-info/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      373 2024-05-27 05:30:58.000000 color_change_filter-1.1.4/src/color_change_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-27 05:30:58.000000 color_change_filter-1.1.4/src/color_change_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-27 05:30:58.000000 color_change_filter-1.1.4/src/color_change_filter.egg-info/entry_points.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:30:58.000000 color_change_filter-1.1.4/src/color_change_filter.egg-info/requires.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:30:58.000000 color_change_filter-1.1.4/src/color_change_filter.egg-info/top_level.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4799 2024-05-27 04:57:31.000000 color_change_filter-1.1.4/src/color_change_filter.py
```

### Comparing `color_change_filter-1.1.3/PKG-INFO` & `color_change_filter-1.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.1.3
+Version: 1.1.4
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,17 +38,14 @@
 from color_change_filter import *
 C = color_change_filter()
 C.color_change_GUI("IMG_3430.jpeg","output.jpg")
 
 ```
 
 1. input image
-![input image](https://drive.google.com/uc?export=view&id=1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd)
-
+<img src="https://drive.google.com/uc?export=view&id=1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd" width="200px">
 2. select color from input image
-![Choice color](https://drive.google.com/uc?export=view&id=1m5X2APSrvFFYXmA_c-vhM_IishERVuyR)
-
+<img src="https://drive.google.com/uc?export=view&id=1m5X2APSrvFFYXmA_c-vhM_IishERVuyR" width="200px">
 3. select color from color picker
-![color picker](https://drive.google.com/uc?export=view&id=12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u)
-
+<img src="https://drive.google.com/uc?export=view&id=12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u" width="200px">
 4. output image
-![output image](https://drive.google.com/uc?export=view&id=1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu)
+<img src="https://drive.google.com/uc?export=view&id=1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu" width="200px">
```

### Comparing `color_change_filter-1.1.3/setup.py` & `color_change_filter-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r",encoding="UTF-8") as fh:
     long_description = fh.read()
 setuptools.setup(
   name="color_change_filter",
-  version="1.1.3",
+  version="1.1.4",
   author="Chihiro senbonmatsu",
   author_email="s2222020@stu.musahino-u.ac.jp",
   description="Change color of image",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/senbonmatsu/color_changer",
   project_urls={
```

### Comparing `color_change_filter-1.1.3/src/color_change_filter.egg-info/PKG-INFO` & `color_change_filter-1.1.4/src/color_change_filter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.1.3
+Version: 1.1.4
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,17 +38,14 @@
 from color_change_filter import *
 C = color_change_filter()
 C.color_change_GUI("IMG_3430.jpeg","output.jpg")
 
 ```
 
 1. input image
-![input image](https://drive.google.com/uc?export=view&id=1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd)
-
+<img src="https://drive.google.com/uc?export=view&id=1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd" width="200px">
 2. select color from input image
-![Choice color](https://drive.google.com/uc?export=view&id=1m5X2APSrvFFYXmA_c-vhM_IishERVuyR)
-
+<img src="https://drive.google.com/uc?export=view&id=1m5X2APSrvFFYXmA_c-vhM_IishERVuyR" width="200px">
 3. select color from color picker
-![color picker](https://drive.google.com/uc?export=view&id=12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u)
-
+<img src="https://drive.google.com/uc?export=view&id=12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u" width="200px">
 4. output image
-![output image](https://drive.google.com/uc?export=view&id=1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu)
+<img src="https://drive.google.com/uc?export=view&id=1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu" width="200px">
```

### Comparing `color_change_filter-1.1.3/src/color_change_filter.py` & `color_change_filter-1.1.4/src/color_change_filter.py`

 * *Files identical despite different names*

