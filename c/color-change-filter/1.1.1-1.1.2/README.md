# Comparing `tmp/color_change_filter-1.1.1.tar.gz` & `tmp/color_change_filter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_change_filter-1.1.1.tar", last modified: Fri May 24 19:55:47 2024, max compression
+gzip compressed data, was "color_change_filter-1.1.2.tar", last modified: Mon May 27 05:13:52 2024, max compression
```

## Comparing `color_change_filter-1.1.1.tar` & `color_change_filter-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 19:55:47.372192 color_change_filter-1.1.1/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       24 2024-05-24 18:09:24.000000 color_change_filter-1.1.1/.gitignore
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 19:55:47.371974 color_change_filter-1.1.1/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      457 2024-05-24 16:47:02.000000 color_change_filter-1.1.1/README.md
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-24 19:55:47.372230 color_change_filter-1.1.1/setup.cfg
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      995 2024-05-24 19:55:41.000000 color_change_filter-1.1.1/setup.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 19:55:47.369770 color_change_filter-1.1.1/src/
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 19:55:47.371684 color_change_filter-1.1.1/src/color_change_filter.egg-info/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 19:55:47.000000 color_change_filter-1.1.1/src/color_change_filter.egg-info/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      340 2024-05-24 19:55:47.000000 color_change_filter-1.1.1/src/color_change_filter.egg-info/SOURCES.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-24 19:55:47.000000 color_change_filter-1.1.1/src/color_change_filter.egg-info/dependency_links.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-24 19:55:47.000000 color_change_filter-1.1.1/src/color_change_filter.egg-info/entry_points.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-24 19:55:47.000000 color_change_filter-1.1.1/src/color_change_filter.egg-info/requires.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-24 19:55:47.000000 color_change_filter-1.1.1/src/color_change_filter.egg-info/top_level.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4805 2024-05-24 19:08:10.000000 color_change_filter-1.1.1/src/color_change_filter.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:13:52.287544 color_change_filter-1.1.2/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       24 2024-05-24 18:09:24.000000 color_change_filter-1.1.2/.gitignore
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1561 2024-05-27 05:13:52.287263 color_change_filter-1.1.2/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1031 2024-05-27 05:12:47.000000 color_change_filter-1.1.2/README.md
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       10 2024-05-24 18:09:24.000000 color_change_filter-1.1.2/requirements.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-27 05:13:52.287586 color_change_filter-1.1.2/setup.cfg
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      995 2024-05-27 05:13:34.000000 color_change_filter-1.1.2/setup.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:13:52.285883 color_change_filter-1.1.2/src/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       36 2024-05-26 10:08:09.000000 color_change_filter-1.1.2/src/__init__.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-27 05:13:52.286923 color_change_filter-1.1.2/src/color_change_filter.egg-info/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     1561 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      373 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/entry_points.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/requires.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-27 05:13:52.000000 color_change_filter-1.1.2/src/color_change_filter.egg-info/top_level.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4799 2024-05-27 04:57:31.000000 color_change_filter-1.1.2/src/color_change_filter.py
```

### Comparing `color_change_filter-1.1.1/PKG-INFO` & `color_change_filter-1.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: color_change_filter
-Version: 1.1.1
-Summary: Change color of image
-Home-page: https://github.com/senbonmatsu/color_changer
-Author: Chihiro senbonmatsu
-Author-email: s2222020@stu.musahino-u.ac.jp
-Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: opencv-python
-Requires-Dist: numpy
-
+## ABOUT
 This code can apply a filter to change the selected color to any color.
 
 color_change_CUI(self, image_path,output_path,x,y,rgb)
 - image_path: str
 - output_path:str
 - x:int
 - y:int
@@ -25,7 +11,23 @@
 color_change_CUI changes the color of the specified pixel to an rgb color
 
 color_change_GUI(self, image_path,output_path)
 - image_path:str
 - output_path:str
 
 color_change_GUI selects a specified pixel by clicking on it. Also, rgb is selected from the color picker.
+
+## METHOD
+color_change_GUI method
+
+"""
+from color_change_filter import *
+"""
+
+1. input image
+![Alt text](https://drive.google.com/file/d/1_nwdDS7z2xN5Pv4276920SV-g-nFSiHd/view?usp=sharing)
+2. select color from input image
+![Choice color](https://drive.google.com/file/d/1m5X2APSrvFFYXmA_c-vhM_IishERVuyR/view?usp=sharing)
+3. select color from color picker
+![Alt text](https://drive.google.com/file/d/12mXDkKKTg0R-gP-eC_zIKIdwZOjJbZ8u/view?usp=sharing)
+4. output image
+![Alt text](https://drive.google.com/file/d/1dbJIIte8C4Hjbzau6bGbh359qXX7ZiSu/view?usp=sharing)
```

### Comparing `color_change_filter-1.1.1/setup.py` & `color_change_filter-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r",encoding="UTF-8") as fh:
     long_description = fh.read()
 setuptools.setup(
   name="color_change_filter",
-  version="1.1.1",
+  version="1.1.2",
   author="Chihiro senbonmatsu",
   author_email="s2222020@stu.musahino-u.ac.jp",
   description="Change color of image",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/senbonmatsu/color_changer",
   project_urls={
```

### Comparing `color_change_filter-1.1.1/src/color_change_filter.py` & `color_change_filter-1.1.2/src/color_change_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         while True:
             cv2.imshow('Select Color', img)
             if cv2.waitKey(20) & 0xFF == 27 or clicked:  
                 break
 
         cv2.destroyAllWindows()
         return selected_color if clicked else None
-      
+
     def get_color_at_pixel(self, img, x, y):
         # 画像の範囲外の場合はNoneを返す
         if x < 0 or y < 0 or x >= img.shape[1] or y >= img.shape[0]:
             return None
 
         selected_color = img[y, x]
         print(f"selected pixel ({x}, {y}) color: {selected_color}")
```

