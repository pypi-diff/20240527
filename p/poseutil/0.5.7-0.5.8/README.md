# Comparing `tmp/poseutil-0.5.7.tar.gz` & `tmp/poseutil-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.5.7.tar", last modified: Mon May 13 00:34:38 2024, max compression
+gzip compressed data, was "poseutil-0.5.8.tar", last modified: Mon May 27 00:43:36 2024, max compression
```

## Comparing `poseutil-0.5.7.tar` & `poseutil-0.5.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-13 00:34:38.705937 poseutil-0.5.7/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-13 00:34:38.705674 poseutil-0.5.7/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-13 00:34:38.701094 poseutil-0.5.7/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      470 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2024-05-13 00:34:38.000000 poseutil-0.5.7/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2024-05-13 00:34:38.705991 poseutil-0.5.7/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      610 2024-05-13 00:30:52.000000 poseutil-0.5.7/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-13 00:34:38.705287 poseutil-0.5.7/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17120 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/canvas_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19162 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/common_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    25586 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2884 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/cv_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8313 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6483 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    21797 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    82667 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17710 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    10107 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     5875 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/qt_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2276 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/qt_model.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19250 2024-05-13 00:31:27.000000 poseutil-0.5.7/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:43:36.110698 poseutil-0.5.8/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-27 00:43:36.110489 poseutil-0.5.8/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:43:36.105641 poseutil-0.5.8/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      458 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      470 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2024-05-27 00:43:36.000000 poseutil-0.5.8/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2024-05-27 00:43:36.110741 poseutil-0.5.8/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      610 2024-05-27 00:43:31.000000 poseutil-0.5.8/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2024-05-27 00:43:36.110215 poseutil-0.5.8/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17120 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/canvas_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19162 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    25586 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2884 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/cv_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8313 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6483 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    21797 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    88459 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    17710 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    10107 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     5875 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2276 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/qt_model.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    19250 2024-05-27 00:42:51.000000 poseutil-0.5.8/utils/version.py
```

### Comparing `poseutil-0.5.7/setup.py` & `poseutil-0.5.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.5.7',
+    version='0.5.8',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle', 'pyqt6'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.5.7/utils/ReadFrameData.py` & `poseutil-0.5.8/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/canvas_model.py` & `poseutil-0.5.8/utils/canvas_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/common_component.py` & `poseutil-0.5.8/utils/common_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/const.py` & `poseutil-0.5.8/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/csvHelper.py` & `poseutil-0.5.8/utils/csvHelper.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/cv_model.py` & `poseutil-0.5.8/utils/cv_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/cv_util.py` & `poseutil-0.5.8/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/math_util.py` & `poseutil-0.5.8/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/normarlize.py` & `poseutil-0.5.8/utils/normarlize.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/poseMeasure.py` & `poseutil-0.5.8/utils/poseMeasure.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,139 @@
         self.rightHandPinkyMcp = hand[RIGHT_HAND_PINKY_MCP]
         self.leftHandPinkyPip = hand[LEFT_HAND_PINKY_PIP]
         self.rightHandPinkyPip = hand[RIGHT_HAND_PINKY_PIP]
         self.leftHandPinkyDip = hand[LEFT_HAND_PINKY_DIP]
         self.rightHandPinkyDip = hand[RIGHT_HAND_PINKY_DIP]
         self.leftHandPinkyTip = hand[LEFT_HAND_PINKY_TIP]
         self.righHandPinkyTip = hand[RIGHT_HAND_PINKY_TIP]
+
+    def getData(self, selector: str):
+        func, *inputs = selector.split(",")
+        dimension = inputs[0].strip().lower()
+        direction = inputs[-1].strip()
+        if inputs[-4].strip().isdigit():
+            target = int(inputs[-4].strip())
+        if inputs[-3].strip().isdigit():
+            second = int(inputs[-3].strip())
+        if inputs[-2].strip().isdigit():
+            thrid = int(inputs[-2].strip())
+
+        if func == "Point":
+            return self.getCoordWithDirection(target, dimension, direction)
+        elif func == "Distance":
+            return self.getDistanceWithDirection(target, second, dimension, direction)
+        elif func == "Angle":
+            return self.getAngleWithDirection(target, second, thrid, dimension, direction)
+        elif func == "Plane":
+            return self.getPlaneWithDirection(target, second, dimension, direction)
+        elif func == "Line":
+            return self.getLineWithDirection(target, second, dimension, direction, 'x')
+    
+    def getCoordWithDirection(self, target, dimension, direction):
+        left = self.getCoord(self.pose[target], dimension)
+        right = self.getCoord(self.pose[target+1], dimension)
+        if target == 0:
+            return self.getCoord(self.pose[target], dimension)
+        if direction == 'AVG':
+            return (left + right)/2
+        elif direction == 'LEFT':
+            return left
+        elif direction == 'RIGHT':
+            return right
+        elif direction == 'MINUS':
+            return right
+        elif direction == 'PLUS':
+            return right
+    
+    def getDistanceWithDirection(self, target, second, dimension, direction):
+        if target == 0:
+            left = self.getDistance(self.pose[target], self.pose[second], dimension)
+            right = self.getDistance(self.pose[target], self.pose[second+1], dimension)
+        elif second == 0:
+            left = self.getDistance(self.pose[target], self.pose[second], dimension)
+            right = self.getDistance(self.pose[target+1], self.pose[second], dimension)
+        else:
+            left = self.getDistance(self.pose[target], self.pose[second], dimension)
+            right = self.getDistance(self.pose[target+1], self.pose[second+1], dimension)
+        if direction == 'AVG':
+            return (left + right)/2
+        elif direction == 'LEFT':
+            return left
+        elif direction == 'RIGHT':
+            return right
+        elif direction == 'MINUS':
+            return right
+        elif direction == 'PLUS':
+            return right
+    
+    def getAngleWithDirection(self, target, second, thrid, dimension, direction):
+        if target == 0:
+            left = self.getAngle(self.pose[target], self.pose[second], self.pose[thrid], dimension)
+            right = self.getAngle(self.pose[target], self.pose[second+1], self.pose[thrid+1], dimension)
+        elif second == 0:
+            left = self.getAngle(self.pose[target], self.pose[second], self.pose[thrid], dimension)
+            right = self.getAngle(self.pose[target+1], self.pose[second], self.pose[thrid+1], dimension)
+        elif thrid == 0:
+            left = self.getAngle(self.pose[target], self.pose[second], self.pose[thrid], dimension)
+            right = self.getAngle(self.pose[target+1], self.pose[second+1], self.pose[thrid], dimension)
+        else:
+            left = self.getAngle(self.pose[target], self.pose[second], self.pose[thrid], dimension)
+            right = self.getAngle(self.pose[target+1], self.pose[second+1], self.pose[thrid+1], dimension)
+        if direction == 'AVG':
+            return (left + right)/2
+        elif direction == 'LEFT':
+            return left
+        elif direction == 'RIGHT':
+            return right
+        elif direction == 'MINUS':
+            return right
+        elif direction == 'PLUS':
+            return right
+    
+    def getPlaneWithDirection(self, target, second, dimension, direction):
+        if target == 0:
+            left = self.getPlane(self.pose[target], self.pose[second], dimension)
+            right = self.getPlane(self.pose[target], self.pose[second+1], dimension)
+        elif second == 0:
+            left = self.getPlane(self.pose[target], self.pose[second], dimension)
+            right = self.getPlane(self.pose[target+1], self.pose[second], dimension)
+        else:
+            left = self.getPlane(self.pose[target], self.pose[second], dimension)
+            right = self.getPlane(self.pose[target+1], self.pose[second+1], dimension)
+        if direction == 'AVG':
+            return (left + right)/2
+        elif direction == 'LEFT':
+            return left
+        elif direction == 'RIGHT':
+            return right
+        elif direction == 'MINUS':
+            return right
+        elif direction == 'PLUS':
+            return right
         
+    def getLineWithDirection(self, target, second, dimension, direction, line):
+        if target == 0:
+            left = self.getLine(self.pose[target], self.pose[second], dimension, line)
+            right = self.getLine(self.pose[target], self.pose[second+1], dimension, line)
+        elif second == 0:
+            left = self.getLine(self.pose[target], self.pose[second], dimension, line)
+            right = self.getLine(self.pose[target+1], self.pose[second], dimension, line)
+        else:
+            left = self.getLine(self.pose[target], self.pose[second], dimension, line)
+            right = self.getLine(self.pose[target+1], self.pose[second+1], dimension, line)
+        if direction == 'AVG':
+            return (left + right)/2
+        elif direction == 'LEFT':
+            return left
+        elif direction == 'RIGHT':
+            return right
+        elif direction == 'MINUS':
+            return right
+        elif direction == 'PLUS':
+            return right
 
     def getAngleFromString(self, angleSelect: str):
         if "/" not in angleSelect:
             func, *inputs = angleSelect.split(",")
             angle = round(getattr(self, func)(*inputs), 2)
         else:
             numerator, denominator = angleSelect.split("/")
```

### Comparing `poseutil-0.5.7/utils/poseMeasureFormat.py` & `poseutil-0.5.8/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/pose_util.py` & `poseutil-0.5.8/utils/pose_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/qt_component.py` & `poseutil-0.5.8/utils/qt_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/qt_model.py` & `poseutil-0.5.8/utils/qt_model.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.5.7/utils/version.py` & `poseutil-0.5.8/utils/version.py`

 * *Files identical despite different names*

