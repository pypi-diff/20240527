# Comparing `tmp/color_change_filter-1.1.2.tar.gz` & `tmp/color_change_filter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_change_filter-1.1.2.tar", last modified: Mon May 27 05:13:52 2024, max compression
+gzip compressed data, was "color_change_filter-1.1.3.tar", last modified: Mon May 27 05:25:30 2024, max compression
```

## Comparing `color_change_filter-1.1.2.tar` & `color_change_filter-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:13:52.287544 color_change_filter-1.1.2/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       24 2024-05-24 18:09:24.000000 color_change_filter-1.1.2/.gitignore
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1561 2024-05-27 05:13:52.287263 color_change_filter-1.1.2/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1031 2024-05-27 05:12:47.000000 color_change_filter-1.1.2/README.md
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       10 2024-05-24 18:09:24.000000 color_change_filter-1.1.2/requirements.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-27 05:13:52.287586 color_change_filter-1.1.2/setup.cfg
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      995 2024-05-27 05:13:34.000000 color_change_filter-1.1.2/setup.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:13:52.285883 color_change_filter-1.1.2/src/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       36 2024-05-26 10:08:09.000000 color_change_filter-1.1.2/src/__init__.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:13:52.286923 color_change_filter-1.1.2/src/color_change_filter.egg-info/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1561 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      373 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/SOURCES.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/dependency_links.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/entry_points.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/requires.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/top_level.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4799 2024-05-27 04:57:31.000000 color_change_filter-1.1.2/src/color_change_filter.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:25:30.451128 color_change_filter-1.1.3/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       24 2024-05-24 18:09:24.000000 color_change_filter-1.1.3/.gitignore
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1627 2024-05-27 05:25:30.450890 color_change_filter-1.1.3/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1097 2024-05-27 05:24:34.000000 color_change_filter-1.1.3/README.md
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       10 2024-05-24 18:09:24.000000 color_change_filter-1.1.3/requirements.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-27 05:25:30.451189 color_change_filter-1.1.3/setup.cfg
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      995 2024-05-27 05:24:55.000000 color_change_filter-1.1.3/setup.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:25:30.449250 color_change_filter-1.1.3/src/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       36 2024-05-26 10:08:09.000000 color_change_filter-1.1.3/src/__init__.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:25:30.450250 color_change_filter-1.1.3/src/color_change_filter.egg-info/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1627 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      373 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/entry_points.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/requires.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:25:30.000000 color_change_filter-1.1.3/src/color_change_filter.egg-info/top_level.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4799 2024-05-27 04:57:31.000000 color_change_filter-1.1.3/src/color_change_filter.py
```

### Comparing `color_change_filter-1.1.2/PKG-INFO` & `color_change_filter-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.1.2
+Version: 1.1.3
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,19 +30,25 @@
 - output_path:str
 
 color_change_GUI selects a specified pixel by clicking on it. Also, rgb is selected from the color picker.
 
 ## METHOD
 color_change_GUI method
 
-"""
+```
 from color_change_filter import *
-"""
+C = color_change_filter()
+C.color_change_GUI("IMG_3430.jpeg","output.jpg")
+
+```
 
 1. input image
-![Alt text](https://drive.google.com/file/d/1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd/view?usp=sharing)
+![input image](https://drive.google.com/uc?export=view&id=1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd)
+
 2. select color from input image
-![Choice color](https://drive.google.com/file/d/1m5X2APSrvFFYXmA_c-vhM_IishERVuyR/view?usp=sharing)
+![Choice color](https://drive.google.com/uc?export=view&id=1m5X2APSrvFFYXmA_c-vhM_IishERVuyR)
+
 3. select color from color picker
-![Alt text](https://drive.google.com/file/d/12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u/view?usp=sharing)
+![color picker](https://drive.google.com/uc?export=view&id=12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u)
+
 4. output image
-![Alt text](https://drive.google.com/file/d/1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu/view?usp=sharing)
+![output image](https://drive.google.com/uc?export=view&id=1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu)
```

### Comparing `color_change_filter-1.1.2/setup.py` & `color_change_filter-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r",encoding="UTF-8") as fh:
     long_description = fh.read()
 setuptools.setup(
   name="color_change_filter",
-  version="1.1.2",
+  version="1.1.3",
   author="Chihiro senbonmatsu",
   author_email="s2222020@stu.musahino-u.ac.jp",
   description="Change color of image",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/senbonmatsu/color_changer",
   project_urls={
```

### Comparing `color_change_filter-1.1.2/src/color_change_filter.egg-info/PKG-INFO` & `color_change_filter-1.1.3/src/color_change_filter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.1.2
+Version: 1.1.3
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,19 +30,25 @@
 - output_path:str
 
 color_change_GUI selects a specified pixel by clicking on it. Also, rgb is selected from the color picker.
 
 ## METHOD
 color_change_GUI method
 
-"""
+```
 from color_change_filter import *
-"""
+C = color_change_filter()
+C.color_change_GUI("IMG_3430.jpeg","output.jpg")
+
+```
 
 1. input image
-![Alt text](https://drive.google.com/file/d/1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd/view?usp=sharing)
+![input image](https://drive.google.com/uc?export=view&id=1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd)
+
 2. select color from input image
-![Choice color](https://drive.google.com/file/d/1m5X2APSrvFFYXmA_c-vhM_IishERVuyR/view?usp=sharing)
+![Choice color](https://drive.google.com/uc?export=view&id=1m5X2APSrvFFYXmA_c-vhM_IishERVuyR)
+
 3. select color from color picker
-![Alt text](https://drive.google.com/file/d/12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u/view?usp=sharing)
+![color picker](https://drive.google.com/uc?export=view&id=12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u)
+
 4. output image
-![Alt text](https://drive.google.com/file/d/1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu/view?usp=sharing)
+![output image](https://drive.google.com/uc?export=view&id=1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu)
```

### Comparing `color_change_filter-1.1.2/src/color_change_filter.py` & `color_change_filter-1.1.3/src/color_change_filter.py`

 * *Files identical despite different names*

