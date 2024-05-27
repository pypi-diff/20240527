# Comparing `tmp/spender-0.2.5.tar.gz` & `tmp/spender-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spender-0.2.5.tar", last modified: Thu May 23 21:46:20 2024, max compression
+gzip compressed data, was "spender-0.2.6.tar", last modified: Mon May 27 21:53:08 2024, max compression
```

## Comparing `spender-0.2.5.tar` & `spender-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.835485 spender-0.2.5/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1087 2024-05-23 21:38:54.000000 spender-0.2.5/LICENSE
--rw-r--r--   0 pmelchior   (501) staff       (20)     5096 2024-05-23 21:46:20.835360 spender-0.2.5/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)     4406 2024-05-23 21:38:04.000000 spender-0.2.5/README.md
--rw-r--r--   0 pmelchior   (501) staff       (20)       38 2024-05-23 21:46:20.835525 spender-0.2.5/setup.cfg
--rw-r--r--   0 pmelchior   (501) staff       (20)     1013 2024-05-23 21:44:04.000000 spender-0.2.5/setup.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.832999 spender-0.2.5/spender/
--rw-r--r--   0 pmelchior   (501) staff       (20)     3607 2024-05-23 21:32:20.000000 spender-0.2.5/spender/__init__.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.834746 spender-0.2.5/spender/data/
--rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2.5/spender/data/__init__.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    23704 2023-10-30 11:27:49.000000 spender-0.2.5/spender/data/desi.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2.5/spender/data/emission_lines.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2.5/spender/data/sdss.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)     4382 2023-11-07 15:31:14.000000 spender-0.2.5/spender/flow.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     1074 2024-05-23 21:29:57.000000 spender-0.2.5/spender/hub.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2.5/spender/instrument.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    19985 2023-10-30 13:32:40.000000 spender-0.2.5/spender/model.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3654 2023-10-30 13:32:40.000000 spender-0.2.5/spender/util.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.833695 spender-0.2.5/spender.egg-info/
--rw-r--r--   0 pmelchior   (501) staff       (20)     5096 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)      384 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/SOURCES.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        1 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/dependency_links.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)       75 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/requires.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        8 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/top_level.txt
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-27 21:53:08.646864 spender-0.2.6/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1087 2024-05-23 21:38:54.000000 spender-0.2.6/LICENSE
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4892 2024-05-27 21:53:08.646710 spender-0.2.6/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4202 2024-05-25 03:40:39.000000 spender-0.2.6/README.md
+-rw-r--r--   0 pmelchior   (501) staff       (20)       38 2024-05-27 21:53:08.646916 spender-0.2.6/setup.cfg
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1059 2024-05-25 03:58:08.000000 spender-0.2.6/setup.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-27 21:53:08.643934 spender-0.2.6/spender/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3607 2024-05-23 21:32:20.000000 spender-0.2.6/spender/__init__.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-27 21:53:08.646182 spender-0.2.6/spender/data/
+-rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2.6/spender/data/__init__.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    23704 2023-10-30 11:27:49.000000 spender-0.2.6/spender/data/desi.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2.6/spender/data/emission_lines.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2.6/spender/data/sdss.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    29320 2022-08-08 22:13:56.000000 spender-0.2.6/spender/data/sky-lines.txt
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     4382 2023-11-07 15:31:14.000000 spender-0.2.6/spender/flow.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1382 2024-05-27 21:46:48.000000 spender-0.2.6/spender/hub.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3770 2023-11-07 16:00:05.000000 spender-0.2.6/spender/hubconf.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2.6/spender/instrument.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    19985 2023-10-30 13:32:40.000000 spender-0.2.6/spender/model.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3654 2023-10-30 13:32:40.000000 spender-0.2.6/spender/util.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-27 21:53:08.644749 spender-0.2.6/spender.egg-info/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4892 2024-05-27 21:53:08.000000 spender-0.2.6/spender.egg-info/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)      430 2024-05-27 21:53:08.000000 spender-0.2.6/spender.egg-info/SOURCES.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        1 2024-05-27 21:53:08.000000 spender-0.2.6/spender.egg-info/dependency_links.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)       75 2024-05-27 21:53:08.000000 spender-0.2.6/spender.egg-info/requires.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        8 2024-05-27 21:53:08.000000 spender-0.2.6/spender.egg-info/top_level.txt
```

### Comparing `spender-0.2.5/LICENSE` & `spender-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/PKG-INFO` & `spender-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2.5
+Version: 0.2.6
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
@@ -33,16 +33,14 @@
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
 
 ## Installation
 
 The easiest way is `pip install spender`. When installing from a downloaded code repo, run `pip install -e .`.
 
-For the time being, you will have to install one dependency manually: `torchinterp1d` is available [here](https://github.com/aliutkus/torchinterp1d).
-
 ## Pretrained models
 
 We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's the workflow:
 
 ```python
 import os
 import spender
@@ -79,16 +77,15 @@
 import torch
 from accelerate import Accelerator
 
 # hardware optimization
 accelerator = Accelerator(mixed_precision='fp16')
 
 # get code, instrument, and pretrained spectrum model from the hub
-code_dir = os.path.dirname(spender.__file__)
-sdss, model = torch.hub.load(code_dir, 'sdss_II',  map_location=accelerator.device)
+sdss, model = spender.hub.load('sdss_II',  map_location=accelerator.device)
 
 # get some SDSS spectra from the ids, store locally in data_path
 data_path = "./DATA"
 ids = ((412, 52254, 308), (412, 52250, 129))
 spec, w, z, norm, zerr = sdss.make_batch(data_path, ids)
 
 # run spender end-to-end
```

### Comparing `spender-0.2.5/README.md` & `spender-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
 
 ## Installation
 
 The easiest way is `pip install spender`. When installing from a downloaded code repo, run `pip install -e .`.
 
-For the time being, you will have to install one dependency manually: `torchinterp1d` is available [here](https://github.com/aliutkus/torchinterp1d).
-
 ## Pretrained models
 
 We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's the workflow:
 
 ```python
 import os
 import spender
@@ -59,16 +57,15 @@
 import torch
 from accelerate import Accelerator
 
 # hardware optimization
 accelerator = Accelerator(mixed_precision='fp16')
 
 # get code, instrument, and pretrained spectrum model from the hub
-code_dir = os.path.dirname(spender.__file__)
-sdss, model = torch.hub.load(code_dir, 'sdss_II',  map_location=accelerator.device)
+sdss, model = spender.hub.load('sdss_II',  map_location=accelerator.device)
 
 # get some SDSS spectra from the ids, store locally in data_path
 data_path = "./DATA"
 ids = ((412, 52254, 308), (412, 52250, 129))
 spec, w, z, norm, zerr = sdss.make_batch(data_path, ids)
 
 # run spender end-to-end
```

### Comparing `spender-0.2.5/setup.py` & `spender-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 long_description = open('README.md').read()
 
 setup(
     name="spender",
     description="Spectrum encoder and decoder",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.2.5",
+    version="0.2.6",
     license="MIT",
     author="Peter Melchior",
     author_email="peter.m.melchior@gmail.com",
     url="https://github.com/pmelchior/spender",
     packages=["spender", "spender.data"],
+    package_data={"spender.data": ['*.txt']},
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
```

### Comparing `spender-0.2.5/spender/__init__.py` & `spender-0.2.6/spender/__init__.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender/data/desi.py` & `spender-0.2.6/spender/data/desi.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender/data/emission_lines.py` & `spender-0.2.6/spender/data/emission_lines.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender/data/sdss.py` & `spender-0.2.6/spender/data/sdss.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender/flow.py` & `spender-0.2.6/spender/flow.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender/hub.py` & `spender-0.2.6/spender/hub.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-# thin wrapper on top of torch.hub to provide list() and help() for local code directories
-import os
-from torch.hub import _add_to_sys_path, _import_module, _load_entry_from_hubconf, _load_local, MODULE_HUBCONF
+# Modification of torch.hub to provide list(), help(), load() for local code directories
+# hubconf.py is now a symlink to the main code dir, so that it will be copied into the package with a pip install
+# this way, code and model are always consistent, and we avoid a cached code download
+# regular torch.hub use is still possible but not encouraged because it doesn't deal with dependencies. use pip instead!
 
-repo_dir = os.path.join(os.path.dirname(__file__), "..")
+import os
+from torch.hub import _add_to_sys_path, _import_module, _load_entry_from_hubconf, _load_local, MODULE_HUBCONF, get_dir
 
+repo_dir = os.path.dirname(__file__)
 
 def list():
     # direct copy from pytorch/torch/hub.py
     with _add_to_sys_path(repo_dir):
         hubconf_path = os.path.join(repo_dir, MODULE_HUBCONF)
         hub_module = _import_module(MODULE_HUBCONF, hubconf_path)
```

### Comparing `spender-0.2.5/spender/instrument.py` & `spender-0.2.6/spender/instrument.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender/model.py` & `spender-0.2.6/spender/model.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender/util.py` & `spender-0.2.6/spender/util.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.5/spender.egg-info/PKG-INFO` & `spender-0.2.6/spender.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2.5
+Version: 0.2.6
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
@@ -33,16 +33,14 @@
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
 
 ## Installation
 
 The easiest way is `pip install spender`. When installing from a downloaded code repo, run `pip install -e .`.
 
-For the time being, you will have to install one dependency manually: `torchinterp1d` is available [here](https://github.com/aliutkus/torchinterp1d).
-
 ## Pretrained models
 
 We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's the workflow:
 
 ```python
 import os
 import spender
@@ -79,16 +77,15 @@
 import torch
 from accelerate import Accelerator
 
 # hardware optimization
 accelerator = Accelerator(mixed_precision='fp16')
 
 # get code, instrument, and pretrained spectrum model from the hub
-code_dir = os.path.dirname(spender.__file__)
-sdss, model = torch.hub.load(code_dir, 'sdss_II',  map_location=accelerator.device)
+sdss, model = spender.hub.load('sdss_II',  map_location=accelerator.device)
 
 # get some SDSS spectra from the ids, store locally in data_path
 data_path = "./DATA"
 ids = ((412, 52254, 308), (412, 52250, 129))
 spec, w, z, norm, zerr = sdss.make_batch(data_path, ids)
 
 # run spender end-to-end
```

