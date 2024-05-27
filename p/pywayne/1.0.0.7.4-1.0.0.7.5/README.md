# Comparing `tmp/pywayne-1.0.0.7.4.tar.gz` & `tmp/pywayne-1.0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.7.4.tar", last modified: Fri May 24 03:47:58 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.7.5.tar", last modified: Mon May 27 13:03:04 2024, max compression
```

## Comparing `pywayne-1.0.0.7.4.tar` & `pywayne-1.0.0.7.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.456391 pywayne-1.0.0.7.4/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-24 03:47:58.456039 pywayne-1.0.0.7.4/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.449409 pywayne-1.0.0.7.4/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.4/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.7.4/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.451635 pywayne-1.0.0.7.4/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-05-24 03:47:39.000000 pywayne-1.0.0.7.4/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.452818 pywayne-1.0.0.7.4/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.4/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.4/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.453321 pywayne-1.0.0.7.4/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.453976 pywayne-1.0.0.7.4/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.4/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.4/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.4/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.4/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.4/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    18000 2024-05-24 03:47:33.000000 pywayne-1.0.0.7.4/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.454460 pywayne-1.0.0.7.4/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.4/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.4/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.455275 pywayne-1.0.0.7.4/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.4/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.4/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:47:58.455714 pywayne-1.0.0.7.4/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-24 03:47:58.000000 pywayne-1.0.0.7.4/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-05-24 03:47:58.000000 pywayne-1.0.0.7.4/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-05-24 03:47:58.000000 pywayne-1.0.0.7.4/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      162 2024-05-24 03:47:58.000000 pywayne-1.0.0.7.4/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-05-24 03:47:58.000000 pywayne-1.0.0.7.4/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-05-24 03:47:58.456455 pywayne-1.0.0.7.4/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.4/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.756651 pywayne-1.0.0.7.5/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-27 13:03:04.756196 pywayne-1.0.0.7.5/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.748179 pywayne-1.0.0.7.5/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.5/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     5024 2024-05-27 13:02:05.000000 pywayne-1.0.0.7.5/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.750618 pywayne-1.0.0.7.5/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-05-27 13:02:19.000000 pywayne-1.0.0.7.5/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.752631 pywayne-1.0.0.7.5/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.5/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.5/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.753187 pywayne-1.0.0.7.5/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.753978 pywayne-1.0.0.7.5/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.5/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.5/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.5/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.5/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.5/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    18000 2024-05-24 03:47:33.000000 pywayne-1.0.0.7.5/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.754612 pywayne-1.0.0.7.5/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.5/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.5/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.755300 pywayne-1.0.0.7.5/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.5/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.5/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-27 13:03:04.755707 pywayne-1.0.0.7.5/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      162 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-05-27 13:03:04.000000 pywayne-1.0.0.7.5/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-05-27 13:03:04.756729 pywayne-1.0.0.7.5/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.5/setup.py
```

### Comparing `pywayne-1.0.0.7.4/LICENSE` & `pywayne-1.0.0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/PKG-INFO` & `pywayne-1.0.0.7.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.4
+Version: 1.0.0.7.5
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.7.4/README.md` & `pywayne-1.0.0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/bin/gettool.py` & `pywayne-1.0.0.7.5/bin/gettool.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,22 +10,39 @@
 
 import argparse
 import tempfile
 import shutil
 import subprocess
 import os
 import yaml
+from pywayne.tools import wayne_print
+
+
+def sparse_clone(url: str, target_dir: str):
+    result = subprocess.run(f'git clone --sparse {url} {target_dir}', shell=True, capture_output=True, text=True)
+    if result.returncode != 0:
+        result = subprocess.run(f'git clone --no-checkout {url} {target_dir}', shell=True, capture_output=True, text=True)
+        if result.returncode == 0:
+            cwd = os.getcwd()
+            os.chdir(target_dir)
+            subprocess.run('git sparse-checkout init --cone', shell=True, capture_output=True, text=True)
+            os.chdir(cwd)
+            wayne_print(f'Cloned repository from {url} to {target_dir} with sparse-checkout initialized.', 'yellow')
+        else:
+            wayne_print(f'Failed to clone repository from {url} to {target_dir}.', 'red')
+    else:
+        wayne_print(f'Successfully cloned repository from {url} to {target_dir} with --sparse option.', 'green')
 
 
 def fetch_tool(tool_name, target_dir='', build=False, clean=False):
     print(f"Fetching tool: {tool_name}")
     cwd = os.getcwd()
     with tempfile.TemporaryDirectory() as temp_dir:
         os.chdir(temp_dir)
-        subprocess.run(["git", "clone", "--sparse", "https://github.com/wangyendt/cpp_tools", temp_dir])
+        sparse_clone("https://github.com/wangyendt/cpp_tools", temp_dir)
         name_to_path_map_yaml_file = 'name_to_path_map.yaml'
         assert name_to_path_map_yaml_file in os.listdir('.')
         with open(name_to_path_map_yaml_file, 'r') as f:
             name_to_path_map = yaml.safe_load(f)
         tool_path = name_to_path_map[tool_name]
         if not target_dir:
             target_dir = os.path.join(cwd, tool_path)
@@ -52,19 +69,15 @@
         print(f"Tool {tool_name} has been copied to {target_dir}")
     os.chdir(cwd)
 
 
 def print_supported_tools():
     with tempfile.TemporaryDirectory() as temp_dir:
         os.chdir(temp_dir)
-        subprocess.run(
-            ["git", "clone", "--sparse", "https://github.com/wangyendt/cpp_tools", temp_dir],
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL
-        )
+        sparse_clone("https://github.com/wangyendt/cpp_tools", temp_dir)
         name_to_path_map_yaml_file = 'name_to_path_map.yaml'
         assert name_to_path_map_yaml_file in os.listdir('.')
         with open(name_to_path_map_yaml_file, 'r') as f:
             name_to_path_map = yaml.safe_load(f)
             print('Currently supported tools:')
             print(', '.join(name_to_path_map.keys()))
```

### Comparing `pywayne-1.0.0.7.4/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.7.5/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/ahrs/tools.py` & `pywayne-1.0.0.7.5/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.7.5/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/data_structure.py` & `pywayne-1.0.0.7.5/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/dsp.py` & `pywayne-1.0.0.7.5/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/gui.py` & `pywayne-1.0.0.7.5/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/math.py` & `pywayne-1.0.0.7.5/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/plot.py` & `pywayne-1.0.0.7.5/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/tools.py` & `pywayne-1.0.0.7.5/pywayne/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/vio/tools.py` & `pywayne-1.0.0.7.5/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.7.5/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.7.5/pywayne.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.4
+Version: 1.0.0.7.5
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.7.4/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.7.5/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.4/setup.py` & `pywayne-1.0.0.7.5/setup.py`

 * *Files identical despite different names*

