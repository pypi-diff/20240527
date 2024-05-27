# Comparing `tmp/mia_vgg-0.0.8.tar.gz` & `tmp/mia_vgg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia_vgg-0.0.8.tar", last modified: Mon May 27 08:41:05 2024, max compression
+gzip compressed data, was "mia_vgg-0.0.9.tar", last modified: Mon May 27 09:05:47 2024, max compression
```

## Comparing `mia_vgg-0.0.8.tar` & `mia_vgg-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-27 08:41:01.000000 mia_vgg-0.0.8/pyproject.toml
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/setup.cfg
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/src/
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/src/mia_vgg/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.8/src/mia_vgg/__init__.py
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2714 2024-05-27 08:40:35.000000 mia_vgg-0.0.8/src/mia_vgg/train_target.py
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 08:41:05.803085 mia_vgg-0.0.8/src/mia_vgg.egg-info/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/SOURCES.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/dependency_links.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/requires.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-27 08:41:05.000000 mia_vgg-0.0.8/src/mia_vgg.egg-info/top_level.txt
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 09:05:47.136308 mia_vgg-0.0.9/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-27 09:05:47.136308 mia_vgg-0.0.9/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-27 09:05:41.000000 mia_vgg-0.0.9/pyproject.toml
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-27 09:05:47.136308 mia_vgg-0.0.9/setup.cfg
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 09:05:47.136308 mia_vgg-0.0.9/src/
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 09:05:47.136308 mia_vgg-0.0.9/src/mia_vgg/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.9/src/mia_vgg/__init__.py
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      183 2024-05-27 09:04:27.000000 mia_vgg-0.0.9/src/mia_vgg/mia.py
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2784 2024-05-27 09:05:26.000000 mia_vgg-0.0.9/src/mia_vgg/train_target.py
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-27 09:05:47.136308 mia_vgg-0.0.9/src/mia_vgg.egg-info/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-27 09:05:47.000000 mia_vgg-0.0.9/src/mia_vgg.egg-info/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      259 2024-05-27 09:05:47.000000 mia_vgg-0.0.9/src/mia_vgg.egg-info/SOURCES.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-27 09:05:47.000000 mia_vgg-0.0.9/src/mia_vgg.egg-info/dependency_links.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-27 09:05:47.000000 mia_vgg-0.0.9/src/mia_vgg.egg-info/requires.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-27 09:05:47.000000 mia_vgg-0.0.9/src/mia_vgg.egg-info/top_level.txt
```

### Comparing `mia_vgg-0.0.8/PKG-INFO` & `mia_vgg-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.8
+Version: 0.0.9
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mia_vgg-0.0.8/pyproject.toml` & `mia_vgg-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mia_vgg"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Jan Aalmoes", email="jan.aalmoes@protonmail.com" },
 ]
 description = "MIA on VGG dataset using pytorch"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mia_vgg-0.0.8/src/mia_vgg/train_target.py` & `mia_vgg-0.0.9/src/mia_vgg/train_target.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from torchvision import datasets, models
 import matplotlib.pyplot as plt
 from torch import nn
 from torch.utils.data import random_split, DataLoader
 import torch.optim as optim
 from torchvision.transforms import PILToTensor, v2
 import torch
+import numpy as np
+import os
+from pathlib import Path
 
 
 def trgtsf(t):
     """Transform a target.
     :param t: Target vector.
     :type t: Vector of size 40
     """
@@ -20,16 +23,16 @@
     """Train VGG16."""
     transform = v2.Compose([PILToTensor(),
                            v2.ToDtype(torch.float32, scale=True)])
     celeba = datasets.CelebA(root="data", download=True, target_transform=trgtsf, transform=transform)
     x = celeba[0][0]
 
     train, test = random_split(celeba, [0.8,0.2])
-    trainloader = DataLoader(train, batch_size=101)
-    testloader = DataLoader(test)
+    trainloader = DataLoader(train, batch_size=100)
+    testloader = DataLoader(test, batch_size=100)
 
     weights = models.VGG16_Weights
     model = models.vgg16(weights=weights)
 
     num_ftrs = model.classifier[len(model.classifier)-1].in_features
 
     model.classifier[len(model.classifier)-1] = nn.Linear(num_ftrs, 2)
```

### Comparing `mia_vgg-0.0.8/src/mia_vgg.egg-info/PKG-INFO` & `mia_vgg-0.0.9/src/mia_vgg.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.8
+Version: 0.0.9
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

