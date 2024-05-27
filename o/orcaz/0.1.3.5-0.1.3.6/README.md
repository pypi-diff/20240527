# Comparing `tmp/orcaz-0.1.3.5.tar.gz` & `tmp/orcaz-0.1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orcaz-0.1.3.5.tar", last modified: Mon May 27 14:18:13 2024, max compression
+gzip compressed data, was "orcaz-0.1.3.6.tar", last modified: Mon May 27 15:00:30 2024, max compression
```

## Comparing `orcaz-0.1.3.5.tar` & `orcaz-0.1.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4789 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:18:13.714231 orcaz-0.1.3.5/orcaz/
--rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/NiftiDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3431 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5801 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/discriminators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1702 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/download.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/file_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16048 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    26207 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/input_validation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/options.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7285 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/orcaz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/plot_generated_batch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15581 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/predict_single_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13140 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/showcase.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/train.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/train_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/orcaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:00:30.132936 orcaz-0.1.3.6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 15:00:30.132936 orcaz-0.1.3.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4789 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:00:30.128936 orcaz-0.1.3.6/orcaz/
+-rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/NiftiDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3431 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5801 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/discriminators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1702 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/download.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/file_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16048 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26207 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/input_validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/options.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7285 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/orcaz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/plot_generated_batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15581 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/predict_single_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13140 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/showcase.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/orcaz/train_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:00:30.128936 orcaz-0.1.3.6/orcaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 15:00:30.000000 orcaz-0.1.3.6/orcaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 15:00:30.000000 orcaz-0.1.3.6/orcaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:00:30.000000 orcaz-0.1.3.6/orcaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 15:00:30.000000 orcaz-0.1.3.6/orcaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-27 15:00:30.000000 orcaz-0.1.3.6/orcaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 15:00:30.000000 orcaz-0.1.3.6/orcaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:00:30.132936 orcaz-0.1.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-05-27 15:00:20.000000 orcaz-0.1.3.6/setup.py
```

### Comparing `orcaz-0.1.3.5/LICENSE` & `orcaz-0.1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/PKG-INFO` & `orcaz-0.1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orcaz
-Version: 0.1.3.5
+Version: 0.1.3.6
 Summary: ORCA (Optimized Registration through Conditional Adversarial networks) 
 Home-page: 
 Author: Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD
 Author-email: zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `orcaz-0.1.3.5/README.md` & `orcaz-0.1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/NiftiDataset.py` & `orcaz-0.1.3.6/orcaz/NiftiDataset.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/config.py` & `orcaz-0.1.3.6/orcaz/config.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/constants.py` & `orcaz-0.1.3.6/orcaz/constants.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/discriminators.py` & `orcaz-0.1.3.6/orcaz/discriminators.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/display.py` & `orcaz-0.1.3.6/orcaz/display.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/download.py` & `orcaz-0.1.3.6/orcaz/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     print('')
     binary_path = constants.BINARY_PATH
     file_utilities.create_directory(binary_path)
     system_os, system_arch = file_utilities.get_system()
     print(f'{constants.ANSI_ORANGE} Detected system: {system_os} | Detected architecture: {system_arch}'
           f'{constants.ANSI_RESET}')
-    download(item_name=f'falcon-{system_os}-{system_arch}', item_path=binary_path,
+    download(item_name=f'beast-binaries-{system_os}-{system_arch}', item_path=binary_path,
                       item_dict=falcon_resources.FALCON_BINARIES)
     file_utilities.set_permissions(constants.GREEDY_PATH, system_os)
     file_utilities.set_permissions(constants.DCM2NIIX_PATH, system_os)
     file_utilities.set_permissions(constants.C3D_PATH, system_os)
 
 
 def download(item_name, item_path, item_dict):
```

### Comparing `orcaz-0.1.3.5/orcaz/file_utilities.py` & `orcaz-0.1.3.6/orcaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/generators.py` & `orcaz-0.1.3.6/orcaz/generators.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/image_conversion.py` & `orcaz-0.1.3.6/orcaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/image_processing.py` & `orcaz-0.1.3.6/orcaz/image_processing.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/input_validation.py` & `orcaz-0.1.3.6/orcaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/options.py` & `orcaz-0.1.3.6/orcaz/options.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/orcaz.py` & `orcaz-0.1.3.6/orcaz/orcaz.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/plot_generated_batch.py` & `orcaz-0.1.3.6/orcaz/plot_generated_batch.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/predict_single_image.py` & `orcaz-0.1.3.6/orcaz/predict_single_image.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/registration.py` & `orcaz-0.1.3.6/orcaz/registration.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/resources.py` & `orcaz-0.1.3.6/orcaz/resources.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/showcase.py` & `orcaz-0.1.3.6/orcaz/showcase.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/train.py` & `orcaz-0.1.3.6/orcaz/train.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz/train_utils.py` & `orcaz-0.1.3.6/orcaz/train_utils.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/orcaz.egg-info/PKG-INFO` & `orcaz-0.1.3.6/orcaz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orcaz
-Version: 0.1.3.5
+Version: 0.1.3.6
 Summary: ORCA (Optimized Registration through Conditional Adversarial networks) 
 Home-page: 
 Author: Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD
 Author-email: zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `orcaz-0.1.3.5/orcaz.egg-info/SOURCES.txt` & `orcaz-0.1.3.6/orcaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.5/setup.py` & `orcaz-0.1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='orcaz',
-    version='0.1.3.5',
+    version='0.1.3.6',
     packages=['orcaz'],
     url='',
     license='GNU General Public License v3.0',
     author='Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD',
     author_email='zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at',
     description='ORCA (Optimized Registration through Conditional Adversarial networks) ',
     long_description_content_type="text/markdown",
```

