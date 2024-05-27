# Comparing `tmp/yputils-0.6.3.tar.gz` & `tmp/yputils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yputils-0.6.3.tar", last modified: Sat Mar  9 10:13:30 2024, max compression
+gzip compressed data, was "yputils-0.7.0.tar", last modified: Mon May 27 06:09:35 2024, max compression
```

## Comparing `yputils-0.6.3.tar` & `yputils-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:13:30.227440 yputils-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-09 10:13:20.000000 yputils-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-09 10:13:30.227440 yputils-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-09 10:13:20.000000 yputils-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 10:13:30.227440 yputils-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-09 10:13:20.000000 yputils-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:13:30.227440 yputils-0.6.3/yputils/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-09 10:13:20.000000 yputils-0.6.3/yputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-09 10:13:20.000000 yputils-0.6.3/yputils/ycfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-09 10:13:20.000000 yputils-0.6.3/yputils/yfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-09 10:13:20.000000 yputils-0.6.3/yputils/yimage.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-09 10:13:20.000000 yputils-0.6.3/yputils/ypdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 10:13:30.227440 yputils-0.6.3/yputils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-09 10:13:30.000000 yputils-0.6.3/yputils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-09 10:13:30.000000 yputils-0.6.3/yputils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 10:13:30.000000 yputils-0.6.3/yputils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-09 10:13:30.000000 yputils-0.6.3/yputils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:09:35.789393 yputils-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-27 06:09:29.000000 yputils-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 06:09:35.789393 yputils-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 06:09:29.000000 yputils-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:09:35.789393 yputils-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-27 06:09:29.000000 yputils-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:09:35.789393 yputils-0.7.0/yputils/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/cfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/ycfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/yfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/yimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 06:09:29.000000 yputils-0.7.0/yputils/ypdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:09:35.789393 yputils-0.7.0/yputils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-27 06:09:35.000000 yputils-0.7.0/yputils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-27 06:09:35.000000 yputils-0.7.0/yputils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:09:35.000000 yputils-0.7.0/yputils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 06:09:35.000000 yputils-0.7.0/yputils.egg-info/top_level.txt
```

### Comparing `yputils-0.6.3/LICENSE` & `yputils-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yputils-0.6.3/PKG-INFO` & `yputils-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yputils
-Version: 0.6.3
+Version: 0.7.0
 Summary: Python code segment for myself using.
 Home-page: https://www.github.com/RyanLuDev/yputils
 Author: Ryan Lu
 Author-email: lyydev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yputils-0.6.3/setup.py` & `yputils-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `yputils-0.6.3/yputils/yfile.py` & `yputils-0.7.0/yputils/file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import pathlib
 import hashlib
+import shutil
+
 
 IMG_TYPE = ['jpg', 'jpeg', 'png']
 
 
 # def list_file(f_path: str, f_ext: list[str]) -> list[str]:
 #     files(f_path, f_ext)
 
@@ -39,15 +41,15 @@
 def imgs(f_path: str, f_ext: list[str] = IMG_TYPE) -> list[str]:
     if not os.path.exists(f_path):
         return []
     return files(f_path, f_ext)
 
 
 def img_paths(f_path: str, f_ext: list[str] = IMG_TYPE) -> list[str]:
-    file_paths(f_path, f_ext)
+    return file_paths(f_path, f_ext)
 
 
 # def i_paths(f_path: str, f_ext: list[str] = IMG_TYPE) -> list[str]:
 #     if not os.path.exists(f_path):
 #         return []
 #     return list_path(f_path, f_ext)
 
@@ -66,7 +68,16 @@
             case 'MD5':
                 md5_obj = hashlib.md5()
                 md5_obj.update(f.read())
                 hash_code = md5_obj.hexdigest()
             case _:
                 hash_code = 'Invalid Hash Type'
     return hash_code
+
+def move_files_by_ext(dir_path:str)->None
+    for filename in os.listdir(dir_path):
+        if os.path.isfile(os.path.join(dir_path, filename)):
+            file_ext = filename.split('.')[-1]
+            dest_dir = os.path.join(os.path.join(dir_path,dest_dir))
+            if not os.path.exists(dest_dir):
+                os.makedirs(dest_dir)
+                shutil.move(os.path.join(dir_path, filename),os.path.join(dest_dir,filename))
```

### Comparing `yputils-0.6.3/yputils/yimage.py` & `yputils-0.7.0/yputils/image.py`

 * *Files identical despite different names*

### Comparing `yputils-0.6.3/yputils.egg-info/PKG-INFO` & `yputils-0.7.0/yputils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yputils
-Version: 0.6.3
+Version: 0.7.0
 Summary: Python code segment for myself using.
 Home-page: https://www.github.com/RyanLuDev/yputils
 Author: Ryan Lu
 Author-email: lyydev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

