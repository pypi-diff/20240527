# Comparing `tmp/orcaz-0.1.3.4.tar.gz` & `tmp/orcaz-0.1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orcaz-0.1.3.4.tar", last modified: Mon Apr 22 15:34:51 2024, max compression
+gzip compressed data, was "orcaz-0.1.3.5.tar", last modified: Mon May 27 14:18:13 2024, max compression
```

## Comparing `orcaz-0.1.3.4.tar` & `orcaz-0.1.3.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:34:51.577054 orcaz-0.1.3.4/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-22 15:34:51.577054 orcaz-0.1.3.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     4539 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:34:51.577054 orcaz-0.1.3.4/orcaz/
--rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/NiftiDataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3383 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5801 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/discriminators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1702 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/download.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/file_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16048 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    26207 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/input_validation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/options.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7285 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/orcaz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/plot_generated_batch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15581 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/predict_single_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13140 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/showcase.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/train.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/orcaz/train_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:34:51.577054 orcaz-0.1.3.4/orcaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-22 15:34:51.000000 orcaz-0.1.3.4/orcaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-22 15:34:51.000000 orcaz-0.1.3.4/orcaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:34:51.000000 orcaz-0.1.3.4/orcaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 15:34:51.000000 orcaz-0.1.3.4/orcaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 15:34:51.000000 orcaz-0.1.3.4/orcaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 15:34:51.000000 orcaz-0.1.3.4/orcaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:34:51.577054 orcaz-0.1.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-04-22 15:34:47.000000 orcaz-0.1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4789 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:18:13.714231 orcaz-0.1.3.5/orcaz/
+-rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/NiftiDataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3431 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5801 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/discriminators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1702 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/download.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/file_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16048 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26207 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/input_validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/options.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7285 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/orcaz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3707 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/plot_generated_batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15581 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/predict_single_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13140 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/showcase.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10770 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/orcaz/train_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/orcaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 14:18:13.000000 orcaz-0.1.3.5/orcaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:18:13.718231 orcaz-0.1.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-05-27 14:18:07.000000 orcaz-0.1.3.5/setup.py
```

### Comparing `orcaz-0.1.3.4/LICENSE` & `orcaz-0.1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/PKG-INFO` & `orcaz-0.1.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orcaz
-Version: 0.1.3.4
+Version: 0.1.3.5
 Summary: ORCA (Optimized Registration through Conditional Adversarial networks) 
 Home-page: 
 Author: Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD
 Author-email: zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -106,65 +106,71 @@
 
 ### Required Directory Structure 🌳
 Please structure your dataset as follows:
 
 ```
 EXAMPLE_Data_folder/
 ├── S1
-│   ├── CT
+│   ├── S1_CT
 │   │   ├── xyz_1.dcm
 │   │   ├── xyz_2.dcm
 │   │   ├── .
 │   │   ├── .
 │   │   ├── .
 │   │   └── xyz_532.dcm
-│   └── AC_FDG_PET
+│   └── S1_FDG_NAC_PT
 │       ├── xyz_1.dcm
 │       ├── xyz_2.dcm
 │       ├── .
 │       ├── .
 │       ├── .
 │       └── xyz_532.dcm
 ├── S2
-│   ├── CT
+│   ├── S2_CT
 │   │   ├── xyz_1.dcm
 │   │   ├── xyz_2.dcm
 │   │   ├── .
 │   │   ├── .
 │   │   ├── .
 │   │   └── xyz_532.dcm
-│   └── NAC_FDG_PET
+│   └── S2_FDG_NAC_PT
 │       ├── xyz_1.dcm
 │       ├── xyz_2.dcm
 │       ├── .
 │       ├── .
 │       ├── .
 │       └── xyz_532.dcm
-├── S2
-│   ├── CT
-│   │   └── xyz_ct.nii
-│   └── AC_FDG_PET
-│       └── xyz_pt.nii
+├── S3
+│   ├── S3_CT.nii
+│   └── S3_FDG_NAC_PT.nii
+├── S4
+│   ├── S4_CT.nii.gz
+│   └── S4_FDG_NAC_PT.nii.gz
 ```
 
 In all these cases, ORCA can be executed on the directories one by one
 
 ```bash
 orcaz -d S1 -m coreg
 orcaz -d S2 -m coreg
 orcaz -d S3 -m coreg  
 ```
 
 **Note:** If the necessary naming conventions are not followed, ORCA will not process the data in the directory.
 
 
 ### Naming Conventions for files 📝
-There is none! Currently orca requires the naming of the subject subloders to be of a particular name. 
+There is none! Currently orca requires the naming of the subject subfoders inlcude particular names.
+The patient identifier can be placed in the start of each subfolder
 
-For instance, `CT` and `NAC_FDG_PET`, or  `CT` and `AC_FDG_PET`.
+For instance, `S1_CT` and `S1_FDG_NAC_PT`, or  `S1_CT` and `S1_FDG_AC_PT`.  
+`S2_CT` and `S2_PSMA_NAC_PT`.  
+`S3_CT` and `S3_FACBC_NAC_PT`.  
+`S4_CT` and `S4_DOTA_NAC_PT`.  
+`S5_CT` and `S5_AGNOSTIC_NAC_PT`.  
 
 ### Output
 After successful completion, the co-registered CT is saved as dicom data in `ORCA_CT_DICOM`.
 
 Intermediate images and warp files are stored within the `ORCA-VXX-YYYY-MM-DD-HH-MM-SS` folder
 ```
 S1
```

### Comparing `orcaz-0.1.3.4/README.md` & `orcaz-0.1.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -76,65 +76,71 @@
 
 ### Required Directory Structure 🌳
 Please structure your dataset as follows:
 
 ```
 EXAMPLE_Data_folder/
 ├── S1
-│   ├── CT
+│   ├── S1_CT
 │   │   ├── xyz_1.dcm
 │   │   ├── xyz_2.dcm
 │   │   ├── .
 │   │   ├── .
 │   │   ├── .
 │   │   └── xyz_532.dcm
-│   └── AC_FDG_PET
+│   └── S1_FDG_NAC_PT
 │       ├── xyz_1.dcm
 │       ├── xyz_2.dcm
 │       ├── .
 │       ├── .
 │       ├── .
 │       └── xyz_532.dcm
 ├── S2
-│   ├── CT
+│   ├── S2_CT
 │   │   ├── xyz_1.dcm
 │   │   ├── xyz_2.dcm
 │   │   ├── .
 │   │   ├── .
 │   │   ├── .
 │   │   └── xyz_532.dcm
-│   └── NAC_FDG_PET
+│   └── S2_FDG_NAC_PT
 │       ├── xyz_1.dcm
 │       ├── xyz_2.dcm
 │       ├── .
 │       ├── .
 │       ├── .
 │       └── xyz_532.dcm
-├── S2
-│   ├── CT
-│   │   └── xyz_ct.nii
-│   └── AC_FDG_PET
-│       └── xyz_pt.nii
+├── S3
+│   ├── S3_CT.nii
+│   └── S3_FDG_NAC_PT.nii
+├── S4
+│   ├── S4_CT.nii.gz
+│   └── S4_FDG_NAC_PT.nii.gz
 ```
 
 In all these cases, ORCA can be executed on the directories one by one
 
 ```bash
 orcaz -d S1 -m coreg
 orcaz -d S2 -m coreg
 orcaz -d S3 -m coreg  
 ```
 
 **Note:** If the necessary naming conventions are not followed, ORCA will not process the data in the directory.
 
 
 ### Naming Conventions for files 📝
-There is none! Currently orca requires the naming of the subject subloders to be of a particular name. 
+There is none! Currently orca requires the naming of the subject subfoders inlcude particular names.
+The patient identifier can be placed in the start of each subfolder
 
-For instance, `CT` and `NAC_FDG_PET`, or  `CT` and `AC_FDG_PET`.
+For instance, `S1_CT` and `S1_FDG_NAC_PT`, or  `S1_CT` and `S1_FDG_AC_PT`.  
+`S2_CT` and `S2_PSMA_NAC_PT`.  
+`S3_CT` and `S3_FACBC_NAC_PT`.  
+`S4_CT` and `S4_DOTA_NAC_PT`.  
+`S5_CT` and `S5_AGNOSTIC_NAC_PT`.  
 
 ### Output
 After successful completion, the co-registered CT is saved as dicom data in `ORCA_CT_DICOM`.
 
 Intermediate images and warp files are stored within the `ORCA-VXX-YYYY-MM-DD-HH-MM-SS` folder
 ```
 S1
```

### Comparing `orcaz-0.1.3.4/orcaz/NiftiDataset.py` & `orcaz-0.1.3.5/orcaz/NiftiDataset.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/config.py` & `orcaz-0.1.3.5/orcaz/config.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/constants.py` & `orcaz-0.1.3.5/orcaz/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
 project_root = file_utilities.get_virtual_env_root()
 BINARY_PATH = os.path.join(project_root, 'bin')
 MODEL_PATH = os.path.join(project_root, 'models')
 
 # Set the paths to the binaries based on the operating system
 if file_utilities.get_system()[0] == 'windows':
-    GREEDY_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                'greedy.exe')
-    C3D_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    C3D_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                             'c3d.exe')
     DCM2NIIX_PATH = os.path.join(BINARY_PATH,
-                                 f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+                                 f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                  'dcm2niix.exe')
 
 elif file_utilities.get_system()[0] in ['linux', 'mac']:
-    GREEDY_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    GREEDY_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                'greedy')
-    C3D_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    C3D_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                             'c3d')
-    DCM2NIIX_PATH = os.path.join(BINARY_PATH, f'falcon-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
+    DCM2NIIX_PATH = os.path.join(BINARY_PATH, f'beast-binaries-{file_utilities.get_system()[0]}-{file_utilities.get_system()[1]}',
                                     'dcm2niix')
 
 # COLOR CODES
 ANSI_ORANGE = '\033[38;5;208m'
 ANSI_GREEN = '\033[38;5;40m'
 ANSI_BLUE = '\033[1;94m'
 ANSI_RESET = '\033[0m'
```

### Comparing `orcaz-0.1.3.4/orcaz/discriminators.py` & `orcaz-0.1.3.5/orcaz/discriminators.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/display.py` & `orcaz-0.1.3.5/orcaz/display.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/download.py` & `orcaz-0.1.3.5/orcaz/download.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/file_utilities.py` & `orcaz-0.1.3.5/orcaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/generators.py` & `orcaz-0.1.3.5/orcaz/generators.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/image_conversion.py` & `orcaz-0.1.3.5/orcaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/image_processing.py` & `orcaz-0.1.3.5/orcaz/image_processing.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/input_validation.py` & `orcaz-0.1.3.5/orcaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/options.py` & `orcaz-0.1.3.5/orcaz/options.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/orcaz.py` & `orcaz-0.1.3.5/orcaz/orcaz.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/plot_generated_batch.py` & `orcaz-0.1.3.5/orcaz/plot_generated_batch.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/predict_single_image.py` & `orcaz-0.1.3.5/orcaz/predict_single_image.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/registration.py` & `orcaz-0.1.3.5/orcaz/registration.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/resources.py` & `orcaz-0.1.3.5/orcaz/resources.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/showcase.py` & `orcaz-0.1.3.5/orcaz/showcase.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/train.py` & `orcaz-0.1.3.5/orcaz/train.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz/train_utils.py` & `orcaz-0.1.3.5/orcaz/train_utils.py`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/orcaz.egg-info/PKG-INFO` & `orcaz-0.1.3.5/orcaz.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orcaz
-Version: 0.1.3.4
+Version: 0.1.3.5
 Summary: ORCA (Optimized Registration through Conditional Adversarial networks) 
 Home-page: 
 Author: Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD
 Author-email: zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -106,65 +106,71 @@
 
 ### Required Directory Structure 🌳
 Please structure your dataset as follows:
 
 ```
 EXAMPLE_Data_folder/
 ├── S1
-│   ├── CT
+│   ├── S1_CT
 │   │   ├── xyz_1.dcm
 │   │   ├── xyz_2.dcm
 │   │   ├── .
 │   │   ├── .
 │   │   ├── .
 │   │   └── xyz_532.dcm
-│   └── AC_FDG_PET
+│   └── S1_FDG_NAC_PT
 │       ├── xyz_1.dcm
 │       ├── xyz_2.dcm
 │       ├── .
 │       ├── .
 │       ├── .
 │       └── xyz_532.dcm
 ├── S2
-│   ├── CT
+│   ├── S2_CT
 │   │   ├── xyz_1.dcm
 │   │   ├── xyz_2.dcm
 │   │   ├── .
 │   │   ├── .
 │   │   ├── .
 │   │   └── xyz_532.dcm
-│   └── NAC_FDG_PET
+│   └── S2_FDG_NAC_PT
 │       ├── xyz_1.dcm
 │       ├── xyz_2.dcm
 │       ├── .
 │       ├── .
 │       ├── .
 │       └── xyz_532.dcm
-├── S2
-│   ├── CT
-│   │   └── xyz_ct.nii
-│   └── AC_FDG_PET
-│       └── xyz_pt.nii
+├── S3
+│   ├── S3_CT.nii
+│   └── S3_FDG_NAC_PT.nii
+├── S4
+│   ├── S4_CT.nii.gz
+│   └── S4_FDG_NAC_PT.nii.gz
 ```
 
 In all these cases, ORCA can be executed on the directories one by one
 
 ```bash
 orcaz -d S1 -m coreg
 orcaz -d S2 -m coreg
 orcaz -d S3 -m coreg  
 ```
 
 **Note:** If the necessary naming conventions are not followed, ORCA will not process the data in the directory.
 
 
 ### Naming Conventions for files 📝
-There is none! Currently orca requires the naming of the subject subloders to be of a particular name. 
+There is none! Currently orca requires the naming of the subject subfoders inlcude particular names.
+The patient identifier can be placed in the start of each subfolder
 
-For instance, `CT` and `NAC_FDG_PET`, or  `CT` and `AC_FDG_PET`.
+For instance, `S1_CT` and `S1_FDG_NAC_PT`, or  `S1_CT` and `S1_FDG_AC_PT`.  
+`S2_CT` and `S2_PSMA_NAC_PT`.  
+`S3_CT` and `S3_FACBC_NAC_PT`.  
+`S4_CT` and `S4_DOTA_NAC_PT`.  
+`S5_CT` and `S5_AGNOSTIC_NAC_PT`.  
 
 ### Output
 After successful completion, the co-registered CT is saved as dicom data in `ORCA_CT_DICOM`.
 
 Intermediate images and warp files are stored within the `ORCA-VXX-YYYY-MM-DD-HH-MM-SS` folder
 ```
 S1
```

### Comparing `orcaz-0.1.3.4/orcaz.egg-info/SOURCES.txt` & `orcaz-0.1.3.5/orcaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orcaz-0.1.3.4/setup.py` & `orcaz-0.1.3.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='orcaz',
-    version='0.1.3.4',
+    version='0.1.3.5',
     packages=['orcaz'],
     url='',
     license='GNU General Public License v3.0',
     author='Zacharias Chalampalakis, PhD, Lalith Kumar Shiyam Sundar, PhD',
     author_email='zacharias.chalampalakis@meduniwien.ac.at, lalith.shiyamsundar@meduniwien.ac.at',
     description='ORCA (Optimized Registration through Conditional Adversarial networks) ',
     long_description_content_type="text/markdown",
```

