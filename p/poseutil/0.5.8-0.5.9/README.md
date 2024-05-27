# Comparing `tmp/poseutil-0.5.8.tar.gz` & `tmp/poseutil-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.5.8.tar", last modified: Mon May 27 00:43:36 2024, max compression
+gzip compressed data, was "poseutil-0.5.9.tar", last modified: Mon May 27 00:49:26 2024, max compression
```

## Comparing `poseutil-0.5.8.tar` & `poseutil-0.5.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:43:36.110698 poseutil-0.5.8/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-27 00:43:36.110489 poseutil-0.5.8/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:43:36.105641 poseutil-0.5.8/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      470 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2024-05-27 00:43:36.110741 poseutil-0.5.8/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      610 2024-05-27 00:43:31.000000 poseutil-0.5.8/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:43:36.110215 poseutil-0.5.8/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17120 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/canvas_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19162 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/common_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    25586 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2884 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/cv_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8313 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6483 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    21797 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    88459 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17710 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    10107 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     5875 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/qt_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2276 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/qt_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19250 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:49:26.413554 poseutil-0.5.9/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-27 00:49:26.413341 poseutil-0.5.9/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:49:26.409241 poseutil-0.5.9/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-27 00:49:26.000000 poseutil-0.5.9/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      470 2024-05-27 00:49:26.000000 poseutil-0.5.9/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-27 00:49:26.000000 poseutil-0.5.9/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-27 00:49:26.000000 poseutil-0.5.9/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2024-05-27 00:49:26.000000 poseutil-0.5.9/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2024-05-27 00:49:26.413602 poseutil-0.5.9/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      610 2024-05-27 00:49:24.000000 poseutil-0.5.9/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:49:26.413046 poseutil-0.5.9/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17120 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/canvas_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19162 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    25586 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2884 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/cv_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8313 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6483 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    21797 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    88459 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17710 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    10107 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     5875 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2276 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/qt_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19250 2024-05-27 00:48:48.000000 poseutil-0.5.9/utils/version.py
```

### Comparing `poseutil-0.5.8/setup.py` & `poseutil-0.5.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.5.8',
+    version='0.5.9',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle', 'pyqt6'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.5.8/utils/ReadFrameData.py` & `poseutil-0.5.9/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/canvas_model.py` & `poseutil-0.5.9/utils/canvas_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/common_component.py` & `poseutil-0.5.9/utils/common_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/const.py` & `poseutil-0.5.9/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/csvHelper.py` & `poseutil-0.5.9/utils/csvHelper.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/cv_model.py` & `poseutil-0.5.9/utils/cv_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/cv_util.py` & `poseutil-0.5.9/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/math_util.py` & `poseutil-0.5.9/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/normarlize.py` & `poseutil-0.5.9/utils/normarlize.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/poseMeasure.py` & `poseutil-0.5.9/utils/poseMeasure.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/poseMeasureFormat.py` & `poseutil-0.5.9/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/pose_util.py` & `poseutil-0.5.9/utils/pose_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/qt_component.py` & `poseutil-0.5.9/utils/qt_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/qt_model.py` & `poseutil-0.5.9/utils/qt_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.8/utils/version.py` & `poseutil-0.5.9/utils/version.py`

 * *Files identical despite different names*

