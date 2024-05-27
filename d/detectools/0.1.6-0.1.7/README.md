# Comparing `tmp/detectools-0.1.6.tar.gz` & `tmp/detectools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detectools-0.1.6.tar", last modified: Wed May 15 08:27:59 2024, max compression
+gzip compressed data, was "detectools-0.1.7.tar", last modified: Mon May 27 13:50:49 2024, max compression
```

## Comparing `detectools-0.1.6.tar` & `detectools-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)       67 2024-05-14 07:30:49.000000 detectools-0.1.6/LICENSE.txt
--rw-r--r--   0 lucas     (1002) lucas     (1002)     2086 2024-05-15 08:27:59.012578 detectools-0.1.6/PKG-INFO
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1637 2024-03-21 11:28:28.000000 detectools-0.1.6/README.md
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      599 2024-04-17 13:45:59.000000 detectools-0.1.6/README_deployment.md
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1582 2024-05-14 07:30:49.000000 detectools-0.1.6/pyproject.toml
--rw-rw-r--   0 lucas     (1002) lucas     (1002)       38 2024-05-15 08:27:59.012578 detectools-0.1.6/setup.cfg
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      145 2024-03-21 13:29:41.000000 detectools-0.1.6/setup.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.008578 detectools-0.1.6/src/
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.008578 detectools-0.1.6/src/detectools/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1460 2024-05-15 08:26:07.000000 detectools-0.1.6/src/detectools/__init__.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.008578 detectools-0.1.6/src/detectools/data/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      174 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2585 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data/augmentation.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    13633 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data/dataset.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     3354 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/data_management.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/formats/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      678 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    16146 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/base.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     8238 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/detect_mask.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     9274 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/formats/detection_format.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     5788 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/formats/interfaces.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     2936 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/mask_utils.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    12611 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/formats/segmentation_format.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/inference/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      111 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/inference/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     6742 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/inference/engine.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     9141 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/inference/predictor.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/metrics/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      277 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     4389 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/available_metrics.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    13368 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/base.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     3128 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/metrics/functionnals.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/models/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      350 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/models/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     3156 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/models/base.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    12308 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/models/mask2former.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    13114 2024-05-14 07:30:49.000000 detectools-0.1.6/src/detectools/models/yolo.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    18835 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/models/yolov8_seg.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/train/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      138 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/train/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1580 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/train/loss_aggregator.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)    10960 2024-05-15 08:25:33.000000 detectools-0.1.6/src/detectools/train/trainer.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools/utils/
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      233 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/__init__.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      241 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/data.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      320 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/display.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      751 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/utils/load_and_write.py
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     5043 2024-05-14 14:35:51.000000 detectools-0.1.6/src/detectools/visualisation.py
-drwxrwxr-x   0 lucas     (1002) lucas     (1002)        0 2024-05-15 08:27:59.012578 detectools-0.1.6/src/detectools.egg-info/
--rw-r--r--   0 lucas     (1002) lucas     (1002)     2086 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1002) lucas     (1002)     1378 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)        1 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)      218 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1002) lucas     (1002)       11 2024-05-15 08:27:59.000000 detectools-0.1.6/src/detectools.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       67 2024-05-15 09:08:23.000000 detectools-0.1.7/LICENSE.txt
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     2086 2024-05-27 13:50:49.225475 detectools-0.1.7/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1637 2024-05-15 09:08:23.000000 detectools-0.1.7/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      599 2024-05-15 09:08:23.000000 detectools-0.1.7/README_deployment.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1582 2024-05-15 09:08:23.000000 detectools-0.1.7/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2024-05-27 13:50:49.225475 detectools-0.1.7/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      145 2024-05-15 09:08:23.000000 detectools-0.1.7/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.221475 detectools-0.1.7/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.221475 detectools-0.1.7/src/detectools/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1460 2024-05-27 13:49:19.000000 detectools-0.1.7/src/detectools/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools/data/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      174 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/data/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2585 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/data/augmentation.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    13633 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/data/dataset.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3354 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/data_management.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools/formats/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      678 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/formats/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    16146 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/formats/base.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8238 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/formats/detect_mask.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     9396 2024-05-27 13:05:33.000000 detectools-0.1.7/src/detectools/formats/detection_format.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     5788 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/formats/interfaces.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2936 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/formats/mask_utils.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12785 2024-05-27 13:06:06.000000 detectools-0.1.7/src/detectools/formats/segmentation_format.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools/inference/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      111 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/inference/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6852 2024-05-27 13:36:29.000000 detectools-0.1.7/src/detectools/inference/engine.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     9141 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/inference/predictor.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools/metrics/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      277 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/metrics/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     4389 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/metrics/available_metrics.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    13368 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/metrics/base.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3128 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/metrics/functionnals.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools/models/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      350 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/models/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3156 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/models/base.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12379 2024-05-27 13:29:58.000000 detectools-0.1.7/src/detectools/models/mask2former.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    13170 2024-05-27 13:08:31.000000 detectools-0.1.7/src/detectools/models/yolo.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    18880 2024-05-27 13:08:05.000000 detectools-0.1.7/src/detectools/models/yolov8_seg.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools/train/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      138 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/train/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1580 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/train/loss_aggregator.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11066 2024-05-27 13:02:53.000000 detectools-0.1.7/src/detectools/train/trainer.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools/utils/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      233 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/utils/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      241 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/utils/data.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      320 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/utils/display.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      751 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/utils/load_and_write.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     5043 2024-05-15 09:08:23.000000 detectools-0.1.7/src/detectools/visualisation.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-27 13:50:49.225475 detectools-0.1.7/src/detectools.egg-info/
+-rw-r--r--   0 lucas     (1000) lucas     (1000)     2086 2024-05-27 13:50:49.000000 detectools-0.1.7/src/detectools.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1378 2024-05-27 13:50:49.000000 detectools-0.1.7/src/detectools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2024-05-27 13:50:49.000000 detectools-0.1.7/src/detectools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      218 2024-05-27 13:50:49.000000 detectools-0.1.7/src/detectools.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       11 2024-05-27 13:50:49.000000 detectools-0.1.7/src/detectools.egg-info/top_level.txt
```

### Comparing `detectools-0.1.6/PKG-INFO` & `detectools-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detectools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Overlay of PyTorch to generalize trainning and inference processes for detection & instance segmentation tasks.
 Author-email: Lucas Bernigaud Samatan <lucas.bernigaud-samatan@inrae.fr>, Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 Maintainer-email: Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 License: GNU Affero General Public License v3 or later (AGPLv3+) (AGPL-3.0).
 Project-URL: Homepage, https://forgemia.inra.fr/ue-apc/librairies/python/detectools
 Project-URL: Issues, https://forgemia.inra.fr/ue-apc/librairies/python/detectools/-/issues
 Project-URL: Documentation, https://detectools.readthedocs.io/en/latest/
```

### Comparing `detectools-0.1.6/README.md` & `detectools-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/README_deployment.md` & `detectools-0.1.7/README_deployment.md`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/pyproject.toml` & `detectools-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/__init__.py` & `detectools-0.1.7/src/detectools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Torch prebuild functions to train, evaluate and use models in production."""
 import json
 import os
 import sys
 from pathlib import Path
 from typing import Any, Dict, Literal, Union
 
-__version__ = "0.1.6" # change detectools version here
+__version__ = "0.1.7" # change detectools version here
 
 IMAGE_FOLDER = "images"
 ANNOTATION_FILE = "coco_annotations.json"
 
 COLORS = [
     (0, 102, 204),
     (51, 255, 51),
```

### Comparing `detectools-0.1.6/src/detectools/data/augmentation.py` & `detectools-0.1.7/src/detectools/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/data/dataset.py` & `detectools-0.1.7/src/detectools/data/dataset.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/data_management.py` & `detectools-0.1.7/src/detectools/data_management.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/formats/__init__.py` & `detectools-0.1.7/src/detectools/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/formats/base.py` & `detectools-0.1.7/src/detectools/formats/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/formats/detect_mask.py` & `detectools-0.1.7/src/detectools/formats/detect_mask.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/formats/detection_format.py` & `detectools-0.1.7/src/detectools/formats/detection_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     Attributes:
     -----------
 
     Attributes:
         boxe (``BoundingBoxes``): Boxe coordinates in XYWH format.
         label (``Tensor``): Class label of object.
         spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
-        score (``Tensor``): Confidence score of the object (for prediction). 
-    
+        score (``Tensor``): Confidence score of the object (for prediction).
+
     Methods:
     -----------
     """
 
-    boxe : BoundingBoxes
-    label : Tensor
+    boxe: BoundingBoxes
+    label: Tensor
     spatial_size: Tuple[int, int]
     score: Tensor
 
     def __init__(
         self,
         spatial_size: Tuple[int],
         label: Tensor,
@@ -74,51 +74,53 @@
 
     Args:
         spatial_size (``Tensor``): Spatial size (H, W) of corresponding images.
         labels (``Tensor``): Tensor of shape (N,) with class labels for each object.
         boxes (``Tensor``): Tensor of shape (N, 4). N for N objects and 4 for boxes coordinates.
         scores (``Tensor``, **optional**): Tensor of shape (N,) with objects confidence score. Defaults to None.
         box_format (``Literal['XYWH', 'XYXY', 'CXCYWH']``, **optional**): Format of bounding boxes. Defaults to 'XYWH'.
-        
-    
+
+
     Attributes:
     -----------
 
     Attributes:
         box_format (``Literal["XYWH", "XYXY", "CXCYWH"]``): Format of bounding boxes.
         spatial_size (``Tuple[int, int]``): Size of corresponding image (H, W)
         size (``int``): Number of objects in BaseFormat.
         data: (``Dict[str, Tensor]``): Data dict that contains objects informations in it's keys (labels, boxes, scores).
-    
+
     Methods:
     -----------
-    
+
     """
+
     spatial_size: Tuple[
         int, int
     ]  # Store the H, W image size corresponding to objects boxes/masks stored in BaseFormat.
     data: Dict[
         str, Tensor
     ]  # Store all values (labels, boxes/masks at least) corresponding to objects in an image.
     size: int  # Number of objects in image.
     box_format: Literal["XYWH", "XYXY", "CXCYWH"]  # format for bounding boxes.
 
     # override
-    def empty(spatial_size: Tuple[int]) -> DetectionFormat:
+    def empty(spatial_size: Tuple[int], device: Literal["cpu", "cuda"] = "cpu") -> DetectionFormat:
         """Return an empty instance DetectionFormat.
 
         Args:
             spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
+            device (``Literal["cpu", "cuda"]``): Device to define format on. Default to "cpu".
 
         Returns:
             ``DetectionFormat``:
                 - DetectionFormat instance.
         """
-        boxes = BoundingBoxes([[]], canvas_size=spatial_size, format="XYWH")
-        labels = torch.tensor([])
+        boxes = BoundingBoxes([[]], canvas_size=spatial_size, format="XYWH").to(device)
+        labels = torch.tensor([]).to(device)
         detection_format = DetectionFormat(
             spatial_size=spatial_size,
             labels=labels,
             boxes=boxes,
         )
         return detection_format
 
@@ -145,15 +147,15 @@
         self,
         spatial_size: Tensor,
         labels: Tensor,
         boxes: Tensor,
         scores: Tensor = None,
         box_format: Literal["XYWH", "XYXY", "CXCYWH"] = "XYWH",
     ):
-        
+
         # assert Task mode is "instance_segmentation"
         assert (
             Task.mode == "detection"
         ), f"Task mode should be 'detection' to construct DetectionFormat object, got {Task.mode}."
 
         self.spatial_size = spatial_size
         self.size = labels.nelement()
@@ -164,15 +166,15 @@
         )
         # store all data in data dict
         self.data: Dict[str, Tensor] = {"boxes": boxes, "labels": labels}
         if scores != None:
             self.data["scores"] = scores
 
     def __getitem__(self, indexes: Union[int, Tensor]) -> DetectionFormat:
-        """ Return a subset DetectionFormat by keeping only elements of data dict values (tensors) at positions of indexes.
+        """Return a subset DetectionFormat by keeping only elements of data dict values (tensors) at positions of indexes.
 
         Args:
             indexes (``Union[int, Sequence[int]]``): Indexes to slice objects data.
 
         Returns:
             ``DetectionFormat``:
                 - DetectionFormat with n objects for n indexes in indexes.
```

### Comparing `detectools-0.1.6/src/detectools/formats/interfaces.py` & `detectools-0.1.7/src/detectools/formats/interfaces.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/formats/mask_utils.py` & `detectools-0.1.7/src/detectools/formats/mask_utils.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/formats/segmentation_format.py` & `detectools-0.1.7/src/detectools/formats/segmentation_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,31 +112,32 @@
     data: Dict[
         str, Tensor
     ]  # Store all values (labels, boxes/masks at least) corresponding to objects in an image.
     size: int  # Number of objects in image.
     box_format: Literal["XYWH", "XYXY", "CXCYWH"]  # format for bounding boxes.
 
     # override
-    def empty(spatial_size: Tuple[int]) -> SegmentationFormat:
+    def empty(spatial_size: Tuple[int], device: Literal["cpu", "cuda"] = "cpu") -> SegmentationFormat:
         """Return an empty instance SegmentationFormat.
 
         Args:
             spatial_size (``Tuple[int]``): Size (H, W) of the corresponding image.
+            device (``Literal["cpu", "cuda"]``): Device to define format on. Default to "cpu".
 
         Returns:
             ``SegmentationFormat``:
                 - SegmentationFormat instance.
         """
-        boxes = torch.tensor([[]])
-        labels = torch.tensor([])
-        masks = Mask(torch.zeros((spatial_size)).int())  # mask full of 0
-        detection_format = SegmentationFormat(
+        boxes = torch.tensor([[]]).to(device)
+        labels = torch.tensor([]).to(device)
+        masks = Mask(torch.zeros((spatial_size)).int()).to(device)  # mask full of 0
+        segmentation_format = SegmentationFormat(
             spatial_size=spatial_size, labels=labels, boxes=boxes, masks=masks
         )
-        return detection_format
+        return segmentation_format
 
     # override
     def from_coco(
         coco_annotations: List[Dict[str, Any]], spatial_size: Tuple[int]
     ) -> SegmentationFormat:
         """Return SegmentationFormat from an image COCO data dictionnary.
```

### Comparing `detectools-0.1.6/src/detectools/inference/engine.py` & `detectools-0.1.7/src/detectools/inference/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,27 +162,27 @@
 
     Returns:
         ``BaseFormat``:
             -  BaseFormat of whole image.
     """
     h, w = spatial_size
     # remove 0 size patchs
+    non_empty_index = [i for i,p in enumerate(predictions) if p.size > 0]
     non_empty_predictions = [p for p in predictions if p.size > 0]
+    coordinates = torch.tensor(coordinates)[non_empty_index].tolist()
     if len(non_empty_predictions) == 0:
         return Format.empty(spatial_size=spatial_size)
 
-    merged_patch = predictions[0]
+    merged_patch = non_empty_predictions[0]
     patch_h, patch_w = merged_patch.spatial_size
     merged_patch.pad(0, 0, w - patch_w, h - patch_h)
     # for each patch / coordinates
     for i, (y, x) in enumerate(coordinates[1:]):
         # pad patch target to fit spatial size
-        patch_pred = predictions[i + 1]
-        if patch_pred.size == 0:
-            continue
+        patch_pred = non_empty_predictions[i + 1]
         patch_h, patch_w = patch_pred.spatial_size
         patch_pred.pad(x, y, w - patch_w - x, h - (patch_h + y))
         boxes = torch.cat([merged_patch.get("boxes"), patch_pred.get("boxes")])
         scores = torch.cat([merged_patch.get("scores"), patch_pred.get("scores")])
         labels = torch.cat([merged_patch.get("labels"), patch_pred.get("labels")])
         values = [labels, boxes, scores]
```

### Comparing `detectools-0.1.6/src/detectools/inference/predictor.py` & `detectools-0.1.7/src/detectools/inference/predictor.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/metrics/available_metrics.py` & `detectools-0.1.7/src/detectools/metrics/available_metrics.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/metrics/base.py` & `detectools-0.1.7/src/detectools/metrics/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/metrics/functionnals.py` & `detectools-0.1.7/src/detectools/metrics/functionnals.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/models/base.py` & `detectools-0.1.7/src/detectools/models/base.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/models/mask2former.py` & `detectools-0.1.7/src/detectools/models/mask2former.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,23 +196,23 @@
         batch_size = raw_outputs.masks_queries_logits.shape[0]
         predictions = self.processor.post_process_instance_segmentation(
             raw_outputs,
             overlap_mask_area_threshold=self.overlap_mask_thr,
             threshold=self.confidence_thr,
             target_sizes=[spatial_size] * batch_size,
         )
-
+        device = raw_outputs.masks_queries_logits.device
         results = []
         # iter on predictions
         for prediction in predictions:
             spatial_size = prediction["segmentation"].shape[-2:]
             boxes = self.build_boxes(prediction["segmentation"])
             # if no objects return empty Format
             if not boxes.nelement():
-                results.append(SegmentationFormat.empty(spatial_size))
+                results.append(SegmentationFormat.empty(spatial_size), device=device)
                 continue
             # remove empty segmentation objects (objects with no mask pixels)
             non_empty_segmentation = torch.unique(prediction["segmentation"])
             non_empty_segmentation = (
                 non_empty_segmentation[non_empty_segmentation != -1].int().tolist()
             )
             segments = prediction["segments_info"]
```

### Comparing `detectools-0.1.6/src/detectools/models/yolo.py` & `detectools-0.1.7/src/detectools/models/yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
 
         Returns:
             ``BatchedFormats``:
                 - Batched predictions.
         """
 
         prebuild_outputs = prebuild_outputs.unbind()
+        device = prebuild_outputs.device
         h, w = self.retrieve_spatial_size(raw_outputs)
         # create empty Format to merge batch results
         results = []
         # for each prediction
         for prediction in prebuild_outputs:
             # send pred in good pshape
             prediction = prediction.permute(1, 0)
@@ -254,15 +255,15 @@
             result = result.confidence(self.confidence_thr)
             result = result.nms(self.nms_threshold)
             result = result.max_detections(self.max_detection)
             # stack batch results
             results.append(result)
 
         if len(results) == 0:
-            results = DetectionFormat.empty((h, w))
+            results = DetectionFormat.empty((h, w), device=device)
 
         results = BatchedFormats(results)
         return results
 
     def compute_loss(
         self, raw_outputs: Tensor, targets: Dict[str, Tensor]
     ) -> Dict[str, Tensor]:
```

### Comparing `detectools-0.1.6/src/detectools/models/yolov8_seg.py` & `detectools-0.1.7/src/detectools/models/yolov8_seg.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
             ``BatchedFormats``:
                 - Batched predictions.
         """
 
         # TODO reduce size of this function by splitting in smaller ones
         # extract informations from raw_results
         boxes, cls_scores, mask_weights, protos = self.prebuild_output(raw_output)
+        device = boxes.device
         # gather device & spatila_size
         spatial_size = self.retrieve_spatial_size(raw_output)
         # init converter for nms
         box_converter = ConvertBoundingBoxFormat("XYXY")
 
         results = []
         # iter over image results
@@ -159,15 +160,15 @@
             # apply confidence to all values
             image_boxes = image_boxes[confidence_indexes]
             image_cls_scores = image_cls_scores[confidence_indexes]
             image_mask_weights = image_mask_weights[confidence_indexes]
             image_labels = best_class[confidence_indexes]
             # if no objects with good confidence return empty DetectionFormat
             if image_labels.nelement() == 0:
-                result = SegmentationFormat.empty(spatial_size)
+                result = SegmentationFormat.empty(spatial_size, device=device)
                 results.append(result)
                 continue
 
             # apply NMS on boxes to retrieve non overlapped objects
             image_boxes = BoundingBoxes(
                 image_boxes,
                 canvas_size=spatial_size,
```

### Comparing `detectools-0.1.6/src/detectools/train/loss_aggregator.py` & `detectools-0.1.7/src/detectools/train/loss_aggregator.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/train/trainer.py` & `detectools-0.1.7/src/detectools/train/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         device: Literal["cpu", "cuda"] = "cpu",
         nms_threshold: float = 0.45,
         confidence_threshold: float = 0.5,
     ):
 
         self.model = model
         self.model.to_device(device)
+        self.model.confidence_thr = confidence_threshold
+        self.model.nms_threshold = nms_threshold
         self.optimizer = otpimizer
         metrics = [metric.to(device) for metric in metrics]
         self.metrics = metrics
         self.log_dir = log_dir
         self.device = device
         self.nms_threshold = nms_threshold
         self.confidence_threshold = confidence_threshold
```

### Comparing `detectools-0.1.6/src/detectools/utils/load_and_write.py` & `detectools-0.1.7/src/detectools/utils/load_and_write.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools/visualisation.py` & `detectools-0.1.7/src/detectools/visualisation.py`

 * *Files identical despite different names*

### Comparing `detectools-0.1.6/src/detectools.egg-info/PKG-INFO` & `detectools-0.1.7/src/detectools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detectools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Overlay of PyTorch to generalize trainning and inference processes for detection & instance segmentation tasks.
 Author-email: Lucas Bernigaud Samatan <lucas.bernigaud-samatan@inrae.fr>, Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 Maintainer-email: Jordan Bernigaud Samatan <jordan.bernigaud-samatan@inrae.fr>
 License: GNU Affero General Public License v3 or later (AGPLv3+) (AGPL-3.0).
 Project-URL: Homepage, https://forgemia.inra.fr/ue-apc/librairies/python/detectools
 Project-URL: Issues, https://forgemia.inra.fr/ue-apc/librairies/python/detectools/-/issues
 Project-URL: Documentation, https://detectools.readthedocs.io/en/latest/
```

### Comparing `detectools-0.1.6/src/detectools.egg-info/SOURCES.txt` & `detectools-0.1.7/src/detectools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

