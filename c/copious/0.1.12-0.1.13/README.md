# Comparing `tmp/copious-0.1.12.tar.gz` & `tmp/copious-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copious-0.1.12.tar", last modified: Thu May 23 11:04:29 2024, max compression
+gzip compressed data, was "copious-0.1.13.tar", last modified: Mon May 27 10:42:59 2024, max compression
```

## Comparing `copious-0.1.12.tar` & `copious-0.1.13.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.340757 copious-0.1.12/
--rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-23 11:04:29.340612 copious-0.1.12/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      124 2024-05-07 10:00:56.000000 copious-0.1.12/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.337159 copious-0.1.12/copious/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.338414 copious-0.1.12/copious/cv/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     4271 2024-05-23 11:02:14.000000 copious-0.1.12/copious/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-05-07 09:54:59.000000 copious-0.1.12/copious/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.338851 copious-0.1.12/copious/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-05-07 09:54:59.000000 copious-0.1.12/copious/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.340049 copious-0.1.12/copious/io/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      671 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/args.py
--rw-r--r--   0 rlan       (501) staff       (20)     1763 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.340390 copious-0.1.12/copious/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-05-07 09:54:59.000000 copious-0.1.12/copious/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-05-07 09:54:59.000000 copious-0.1.12/copious/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.337898 copious-0.1.12/copious.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      502 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       42 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)        8 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-05-23 11:04:29.340826 copious-0.1.12/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      553 2024-05-23 11:04:00.000000 copious-0.1.12/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 10:42:59.772076 copious-0.1.13/
+-rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-27 10:42:59.771914 copious-0.1.13/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      124 2024-05-07 10:00:56.000000 copious-0.1.13/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 10:42:59.766865 copious-0.1.13/copious/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.13/copious/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 10:42:59.768044 copious-0.1.13/copious/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.13/copious/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     4451 2024-05-27 10:42:50.000000 copious-0.1.13/copious/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-05-07 09:54:59.000000 copious-0.1.13/copious/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 10:42:59.768522 copious-0.1.13/copious/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.13/copious/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-05-07 09:54:59.000000 copious-0.1.13/copious/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 10:42:59.771258 copious-0.1.13/copious/io/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.13/copious/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      671 2024-05-07 09:54:59.000000 copious-0.1.13/copious/io/args.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1763 2024-05-07 09:54:59.000000 copious-0.1.13/copious/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-05-07 09:54:59.000000 copious-0.1.13/copious/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-05-07 09:54:59.000000 copious-0.1.13/copious/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-05-07 09:54:59.000000 copious-0.1.13/copious/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 10:42:59.771657 copious-0.1.13/copious/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-05-07 09:54:59.000000 copious-0.1.13/copious/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-05-07 09:54:59.000000 copious-0.1.13/copious/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-27 10:42:59.767465 copious-0.1.13/copious.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-27 10:42:59.000000 copious-0.1.13/copious.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      502 2024-05-27 10:42:59.000000 copious-0.1.13/copious.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-05-27 10:42:59.000000 copious-0.1.13/copious.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       42 2024-05-27 10:42:59.000000 copious-0.1.13/copious.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        8 2024-05-27 10:42:59.000000 copious-0.1.13/copious.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-05-27 10:42:59.772121 copious-0.1.13/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      553 2024-05-27 10:42:50.000000 copious-0.1.13/setup.py
```

### Comparing `copious-0.1.12/copious/cv/geometry.py` & `copious-0.1.13/copious/cv/geometry.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
 def homo_to_points3d(points_homo: np.ndarray) -> np.ndarray:
     return points_homo[:, :3]
 
 
 class Box3d:
-    def __init__(self, position: np.ndarray, scale: np.ndarray, rotation: Rotation) -> None:
+    def __init__(self, position: np.ndarray, scale: np.ndarray, rotation: Rotation, corners_template: np.ndarray = None) -> None:
         """_summary_
 
         Parameters
         ----------
         position : np.ndarray
             of shape (3, )
         scale : np.ndarray
@@ -93,14 +93,25 @@
         _type_
             _description_
         """
         self.position = position
         self.scale = scale
         self.rotation = rotation
         self._corners = None
+        if self.corners_template is None:
+            self.corners_template = np.array([
+                [0.5, -0.5, -0.5],
+                [0.5, 0.5, -0.5],
+                [0.5, 0.5, 0.5],
+                [0.5, -0.5, 0.5],
+                [-0.5, -0.5, -0.5],
+                [-0.5, 0.5, -0.5],
+                [-0.5, 0.5, 0.5],
+                [-0.5, -0.5, 0.5],
+            ])
     
     @property
     def corners(self) -> np.ndarray:
         """
         Returns
         -------
         np.ndarray
@@ -113,24 +124,15 @@
     def calc_box_corners(self) -> np.ndarray:
         """
         Parameters
         -------
         np.ndarray
             of shape (8, 3)
         """
-        corners = np.array([
-            [0.5, -0.5, -0.5],
-            [0.5, 0.5, -0.5],
-            [0.5, 0.5, 0.5],
-            [0.5, -0.5, 0.5],
-            [-0.5, -0.5, -0.5],
-            [-0.5, 0.5, -0.5],
-            [-0.5, 0.5, 0.5],
-            [-0.5, -0.5, 0.5],
-        ])
+        corners = self.corners_template.copy()
         corners = corners * self.scale[None]
         corners = corners @ self.rotation.as_matrix().T
         corners = corners + self.position
         return corners
 
     @classmethod
     def from_pos_scale_euler(cls, pos_x: float, pos_y: float, pos_z: float, scale_x: float, scale_y: float, scale_z: float, rot_euler_x: float, rot_euler_y: float, rot_euler_z: float, degrees: bool = False):
```

### Comparing `copious-0.1.12/copious/cv/graphics.py` & `copious-0.1.13/copious/cv/graphics.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/copious/data_structure/set.py` & `copious-0.1.13/copious/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/copious/io/args.py` & `copious-0.1.13/copious/io/args.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/copious/io/fs.py` & `copious-0.1.13/copious/io/fs.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/copious/io/indices.py` & `copious-0.1.13/copious/io/indices.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/copious/io/network.py` & `copious-0.1.13/copious/io/network.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/copious/io/parallelism.py` & `copious-0.1.13/copious/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/copious/plot/color.py` & `copious-0.1.13/copious/plot/color.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.12/setup.py` & `copious-0.1.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='copious',
-    version='0.1.12',
+    version='0.1.13',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/copious',
```

