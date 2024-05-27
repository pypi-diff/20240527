# Comparing `tmp/camlab-0.0.8.6.tar.gz` & `tmp/camlab-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.0.8.6.tar", last modified: Mon Apr  8 15:34:42 2024, max compression
+gzip compressed data, was "camlab-0.1.0.tar", last modified: Mon May 27 05:28:17 2024, max compression
```

## Comparing `camlab-0.0.8.6.tar` & `camlab-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:34:42.539419 camlab-0.0.8.6/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.6/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-08 15:34:42.539256 camlab-0.0.8.6/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.6/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-08 15:34:00.000000 camlab-0.0.8.6/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-08 15:34:42.539453 camlab-0.0.8.6/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:34:42.537324 camlab-0.0.8.6/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:34:42.538241 camlab-0.0.8.6/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)     1700 2024-04-08 15:33:09.000000 camlab-0.0.8.6/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     6966 2024-04-07 15:45:31.000000 camlab-0.0.8.6/src/camlab/camera.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-08 15:34:42.539081 camlab-0.0.8.6/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-08 15:34:42.000000 camlab-0.0.8.6/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-08 15:34:42.000000 camlab-0.0.8.6/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-08 15:34:42.000000 camlab-0.0.8.6/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-08 15:34:42.000000 camlab-0.0.8.6/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:28:17.124415 camlab-0.1.0/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.1.0/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-05-27 05:28:17.124229 camlab-0.1.0/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.1.0/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      539 2024-05-27 05:27:04.000000 camlab-0.1.0/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-05-27 05:28:17.124453 camlab-0.1.0/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:28:17.121797 camlab-0.1.0/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:28:17.123079 camlab-0.1.0/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2294 2024-05-27 05:25:50.000000 camlab-0.1.0/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     7127 2024-05-27 05:25:50.000000 camlab-0.1.0/src/camlab/camera.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     3231 2024-05-27 05:25:50.000000 camlab-0.1.0/src/camlab/camera_torch.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-05-27 05:28:17.124049 camlab-0.1.0/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-05-27 05:28:17.000000 camlab-0.1.0/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      239 2024-05-27 05:28:17.000000 camlab-0.1.0/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-05-27 05:28:17.000000 camlab-0.1.0/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-05-27 05:28:17.000000 camlab-0.1.0/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.0.8.6/LICENSE` & `camlab-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.6/PKG-INFO` & `camlab-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.6
+Version: 0.1.0
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camlab-0.0.8.6/README.md` & `camlab-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.6/pyproject.toml` & `camlab-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.0.8.6"
+version = "0.1.0"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.0.8.6/src/camlab/__init__.py` & `camlab-0.1.0/src/camlab/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 import math
+import torch
 from .camera import *
+from .camera_torch import *
 
 
 def fov2focal(fov, pixels):
     return pixels / (2 * math.tan(fov / 2))
 
 
 def focal2fov(focal, pixels):
     return 2 * math.atan(pixels / (2 * focal))
 
 
-def load_3dgs_camera(cam_gs):
+def load_3dgs_camera(cam_gs, tensor_style=False):
     """
     Support 3D Gaussian Splatting Camera-Class Object
     """
-    cam = CameraObj(image_name=cam_gs.image_name)
-    cam.manual_init(focal=fov2focal(cam_gs.FoVx, cam_gs.image_width),
-                    w=cam_gs.image_width, h=cam_gs.image_height)
-
-    ext = np.eye(4)
-    ext[:3, :3] = np.transpose(cam_gs.R)
-    ext[:3, 3] = cam_gs.T
-    c2w = np.linalg.inv(ext)
-    c2w[:3, 1:3] *= -1
+    if not tensor_style:
+        cam = CameraObj(image_name=cam_gs.image_name)
+        cam.manual_init(focal=fov2focal(cam_gs.FoVx, cam_gs.image_width),
+                        w=cam_gs.image_width, h=cam_gs.image_height)
+
+        ext = np.eye(4)
+        ext[:3, :3] = np.transpose(cam_gs.R)
+        ext[:3, 3] = cam_gs.T
+        c2w = np.linalg.inv(ext)
+        c2w[:3, 1:3] *= -1
+
+        cam.R = c2w[:3, :3]
+        cam.T = c2w[:3, 3]
+    else:
+        cam = CameraObjTensor(image_name=cam_gs.image_name)
+        cam.manual_init(focal=fov2focal(cam_gs.FoVx, cam_gs.image_width),
+                        w=cam_gs.image_width, h=cam_gs.image_height)
+        ext = np.eye(4)
+        ext[:3, :3] = np.transpose(cam_gs.R)
+        ext[:3, 3] = cam_gs.T
+        c2w = np.linalg.inv(ext)
+        c2w[:3, 1:3] *= -1
+
+        cam.R = torch.FloatTensor(c2w[:3, :3])
+        cam.T = torch.FloatTensor(c2w[:3, 3])
 
-    cam.R = c2w[:3, :3]
-    cam.T = c2w[:3, 3]
     return cam
 
+
 def approximate(n, o=1e8):
     return int(n * o) / o
 
 
 def closest_points_between_lines(line1, line2, acc=8):
     # Convert points to numpy arrays for easier manipulation
     p1, p2 = np.array(line1)
```

### Comparing `camlab-0.0.8.6/src/camlab/camera.py` & `camlab-0.1.0/src/camlab/camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+
 class CameraObj:
     def __init__(self, intri_mat=None, image_name=None):
         # intrinsic
         self.focal_x = None
         self.focal_y = None
         self.o_x = None
         self.o_y = None
@@ -16,15 +17,15 @@
         # extrinsic
         self.R = None
         self.T = None
         self.is_intri_set = False
 
         # image
         self.image_name = image_name
-        
+
         self.touch = 0
 
         if intri_mat:
             self.K = intri_mat
             self.focal_x = intri_mat[0][0]
             self.focal_y = intri_mat[1][1]
             self.o_x = intri_mat[0][2]
@@ -55,14 +56,15 @@
             print("please set intri parameters !")
             raise Exception
 
     def world2cam(self, p):
         if self.R is None or self.T is None:
             print("Please init the extrinsic params!")
             return -1
+        print(np.dot(p - self.T, self.R))
         return np.dot(p - self.T, self.R)
 
     def cam2screen(self, p, to_int=False):
         """
                           x                                y
             x_im = f_x * --- + offset_x      y_im = f_y * --- + offset_y
                           z                                z
@@ -92,15 +94,15 @@
 
         x, y = screen_p
         direction = np.array([(x - self.o_x) / self.focal_x, - (y - self.o_y) / self.focal_y, -1])
         ray_d = np.sum(direction[None] * R, -1)
         ray_o = T
 
         return ray_o, ray_d
-     
+
     def quaternion2rotation(self, quater):
         self.touch += 1
         w, x, y, z = quater
         r11 = 1 - 2 * y * y - 2 * x * x
         r12 = 2 * x * y - 2 * z * w
         r13 = 2 * x * z + 2 * y * w
         r21 = 2 * x * y + 2 * z * w
@@ -123,91 +125,92 @@
         extri = np.eye(4)
         extri[:3, :3] = rot
         extri[0][-1] = trans[0]
         extri[1][-1] = trans[1]
         extri[2][-1] = trans[2]
         return extri
 
-       
 
 def _test1():
     import cv2
     intri = [[1111.0, 0.0, 400.0],
-         [0.0, 1111.0, 400.0],
-         [0.0, 0.0, 1.0]]
+             [0.0, 1111.0, 400.0],
+             [0.0, 0.0, 1.0]]
     extri = np.array(
-        [[-9.9990e-01,  4.1922e-03, -1.3346e-02, -5.3798e-02],
-        [-1.3989e-02, -2.9966e-01,  9.5394e-01,  3.8455e+00],
-        [-4.6566e-10,  9.5404e-01,  2.9969e-01,  1.2081e+00],
-        [0.0, 0.0, 0.0, 1.0]])
-    extri1 = np.array([[-3.0373e-01, -8.6047e-01,  4.0907e-01,  1.6490e+00],
-        [ 9.5276e-01, -2.7431e-01,  1.3041e-01,  5.2569e-01],
-        [-7.4506e-09,  4.2936e-01,  9.0313e-01,  3.6407e+00],
-        [0.0, 0.0, 0.0, 1.0]])
+        [[-9.9990e-01, 4.1922e-03, -1.3346e-02, -5.3798e-02],
+         [-1.3989e-02, -2.9966e-01, 9.5394e-01, 3.8455e+00],
+         [-4.6566e-10, 9.5404e-01, 2.9969e-01, 1.2081e+00],
+         [0.0, 0.0, 0.0, 1.0]])
+    extri1 = np.array([[-3.0373e-01, -8.6047e-01, 4.0907e-01, 1.6490e+00],
+                       [9.5276e-01, -2.7431e-01, 1.3041e-01, 5.2569e-01],
+                       [-7.4506e-09, 4.2936e-01, 9.0313e-01, 3.6407e+00],
+                       [0.0, 0.0, 0.0, 1.0]])
     extri2 = np.array(
         [[0.4429636299610138, 0.31377720832824707, -0.8398374915122986, -3.385493516921997],
          [-0.8965396881103516, 0.1550314873456955, -0.41494810581207275, -1.6727094650268555],
          [0.0, 0.936754584312439, 0.3499869406223297, 1.4108426570892334],
          [0.0, 0.0, 0.0, 1.0]])
 
     cam_obj = CameraObj(intri)
     cam_obj.load_extrinsic(extri)
+    print(cam_obj.world2screen([-1, -1, -1]))
+    return
 
     vertex = [[-1, -1, -1], [1, -1, -1], [1, 1, -1], [-1, 1, -1], [-1, 1, 1], [1, 1, 1], [1, -1, 1], [-1, -1, 1]]
     # vertex = [[-.5, -.5, -.5], [.5, -.5, -.5], [.5, .5, -.5], [-.5, .5, -.5], [-.5, .5, .5], [.5, .5, .5], [.5, -.5, .5], [-.5, -.5, .5]]
 
     # blank = np.zeros((800, 800, 3), np.uint8)
     blank = cv2.imread("r_0.png")
-    print(blank.shape)
+    # print(blank.shape)
 
     p_s = [cam_obj.world2screen(p_, to_int=True) for p_ in vertex]
     print(p_s)
 
     for i in range(len(p_s)):
         p1 = p_s[i]
         p2 = p_s[i + 1] if i < len(p_s) - 1 else p_s[0]
         cv2.line(blank, p1, p2, (255, 255, 0), 1)
     cv2.line(blank, p_s[3], p_s[0], (255, 255, 0), 1)
     cv2.line(blank, p_s[4], p_s[7], (255, 255, 0), 1)
     cv2.line(blank, p_s[1], p_s[6], (255, 255, 0), 1)
     cv2.line(blank, p_s[2], p_s[5], (255, 255, 0), 1)
     cv2.imwrite("demo.png", blank)
 
+
 def _test2():
     intri = [[1111.0, 0.0, 400.0],
-         [0.0, 1111.0, 400.0],
-         [0.0, 0.0, 1.0]]
+             [0.0, 1111.0, 400.0],
+             [0.0, 0.0, 1.0]]
     extri = np.array(
-        [[-9.9990e-01,  4.1922e-03, -1.3346e-02, -5.3798e-02],
-        [-1.3989e-02, -2.9966e-01,  9.5394e-01,  3.8455e+00],
-        [-4.6566e-10,  9.5404e-01,  2.9969e-01,  1.2081e+00],
-        [0.0, 0.0, 0.0, 1.0]])
-    extri1 = np.array([[-3.0373e-01, -8.6047e-01,  4.0907e-01,  1.6490e+00],
-        [ 9.5276e-01, -2.7431e-01,  1.3041e-01,  5.2569e-01],
-        [-7.4506e-09,  4.2936e-01,  9.0313e-01,  3.6407e+00],
-        [0.0, 0.0, 0.0, 1.0]])
+        [[-9.9990e-01, 4.1922e-03, -1.3346e-02, -5.3798e-02],
+         [-1.3989e-02, -2.9966e-01, 9.5394e-01, 3.8455e+00],
+         [-4.6566e-10, 9.5404e-01, 2.9969e-01, 1.2081e+00],
+         [0.0, 0.0, 0.0, 1.0]])
+    extri1 = np.array([[-3.0373e-01, -8.6047e-01, 4.0907e-01, 1.6490e+00],
+                       [9.5276e-01, -2.7431e-01, 1.3041e-01, 5.2569e-01],
+                       [-7.4506e-09, 4.2936e-01, 9.0313e-01, 3.6407e+00],
+                       [0.0, 0.0, 0.0, 1.0]])
     extri2 = np.array(
         [[0.4429636299610138, 0.31377720832824707, -0.8398374915122986, -3.385493516921997],
          [-0.8965396881103516, 0.1550314873456955, -0.41494810581207275, -1.6727094650268555],
          [0.0, 0.936754584312439, 0.3499869406223297, 1.4108426570892334],
          [0.0, 0.0, 0.0, 1.0]])
 
     cam_obj = CameraObj(intri)
     cam_obj.load_extrinsic(extri2)
 
     p = (400, 400)
     rayo, rayd = cam_obj.make_ray(p)
     ps = cam_obj.world2screen(rayd - rayo, to_int=True)
     print(rayo, rayd)
     print(ps)
-    
+
     quater = [0.980317, 0.002613, -0.19732, 0.005964]
     print(cam_obj.quaternion2rotation(quater))
 
     colmap_params = [0.980317, 0.002613, -0.19732, 0.005964, 5.91824, 0.099605, 0.691238]
     print(cam_obj.colmap2extri(colmap_params))
 
 
-
 if __name__ == "__main__":
-    # _test1()
-    _test2()
+    _test1()
+    # _test2()
```

### Comparing `camlab-0.0.8.6/src/camlab.egg-info/PKG-INFO` & `camlab-0.1.0/src/camlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.6
+Version: 0.1.0
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

