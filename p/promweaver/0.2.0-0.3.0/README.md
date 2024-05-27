# Comparing `tmp/promweaver-0.2.0.tar.gz` & `tmp/promweaver-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promweaver-0.2.0.tar", last modified: Thu Jan 25 16:56:30 2024, max compression
+gzip compressed data, was "promweaver-0.3.0.tar", last modified: Mon May 27 19:54:07 2024, max compression
```

## Comparing `promweaver-0.2.0.tar` & `promweaver-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:56:30.239156 promweaver-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:56:30.235156 promweaver-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:56:30.235156 promweaver-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-25 16:56:17.000000 promweaver-0.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-01-25 16:56:17.000000 promweaver-0.2.0/.github/workflows/build_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-01-25 16:56:17.000000 promweaver-0.2.0/.github/workflows/build_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-25 16:56:17.000000 promweaver-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-25 16:56:30.239156 promweaver-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-01-25 16:56:17.000000 promweaver-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:56:30.235156 promweaver-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-25 16:56:17.000000 promweaver-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-01-25 16:56:17.000000 promweaver-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-01-25 16:56:17.000000 promweaver-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-25 16:56:17.000000 promweaver-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-25 16:56:17.000000 promweaver-0.2.0/docs/promweaver-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-01-25 16:56:17.000000 promweaver-0.2.0/iso_detailed_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-01-25 16:56:17.000000 promweaver-0.2.0/pctr_detailed_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-01-25 16:56:17.000000 promweaver-0.2.0/pctr_pw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-01-25 16:56:17.000000 promweaver-0.2.0/pctr_removing_lines_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:56:30.239156 promweaver-0.2.0/promweaver/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/bc_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/compute_bc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/cone_prom_bc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/iso_prom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/j_prom_bc.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/limb_darkening.py
--rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/pctr_prom.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/prom_bc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/prom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-01-25 16:56:17.000000 promweaver-0.2.0/promweaver/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-25 16:56:30.000000 promweaver-0.2.0/promweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 16:56:30.239156 promweaver-0.2.0/promweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-25 16:56:30.000000 promweaver-0.2.0/promweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-25 16:56:30.000000 promweaver-0.2.0/promweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 16:56:30.000000 promweaver-0.2.0/promweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-25 16:56:30.000000 promweaver-0.2.0/promweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-25 16:56:30.000000 promweaver-0.2.0/promweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-01-25 16:56:17.000000 promweaver-0.2.0/pw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-25 16:56:17.000000 promweaver-0.2.0/pw_test_fil.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-25 16:56:17.000000 promweaver-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 16:56:30.239156 promweaver-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-25 16:56:17.000000 promweaver-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:54:07.649166 promweaver-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:54:07.641166 promweaver-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:54:07.645166 promweaver-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-27 19:54:03.000000 promweaver-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-27 19:54:03.000000 promweaver-0.3.0/.github/workflows/build_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-27 19:54:03.000000 promweaver-0.3.0/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-27 19:54:03.000000 promweaver-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-27 19:54:07.649166 promweaver-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-27 19:54:03.000000 promweaver-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:54:07.645166 promweaver-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 19:54:03.000000 promweaver-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-27 19:54:03.000000 promweaver-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-27 19:54:03.000000 promweaver-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 19:54:03.000000 promweaver-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-27 19:54:03.000000 promweaver-0.3.0/docs/promweaver-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-27 19:54:03.000000 promweaver-0.3.0/iso_detailed_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-27 19:54:03.000000 promweaver-0.3.0/pctr_detailed_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-27 19:54:03.000000 promweaver-0.3.0/pctr_pw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-27 19:54:03.000000 promweaver-0.3.0/pctr_removing_lines_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:54:07.645166 promweaver-0.3.0/promweaver/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/bc_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/compute_bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/cone_prom_bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/iso_prom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/j_prom_bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/limb_darkening.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/pctr_prom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/prom_bc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/prom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/stratified_prom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-27 19:54:03.000000 promweaver-0.3.0/promweaver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 19:54:07.000000 promweaver-0.3.0/promweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:54:07.649166 promweaver-0.3.0/promweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-27 19:54:07.000000 promweaver-0.3.0/promweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-27 19:54:07.000000 promweaver-0.3.0/promweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:54:07.000000 promweaver-0.3.0/promweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 19:54:07.000000 promweaver-0.3.0/promweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 19:54:07.000000 promweaver-0.3.0/promweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-27 19:54:03.000000 promweaver-0.3.0/pw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-27 19:54:03.000000 promweaver-0.3.0/pw_test_fil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-27 19:54:03.000000 promweaver-0.3.0/pw_test_stratification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-27 19:54:03.000000 promweaver-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:54:07.649166 promweaver-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-27 19:54:03.000000 promweaver-0.3.0/setup.py
```

### Comparing `promweaver-0.2.0/.github/workflows/build.yml` & `promweaver-0.3.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/.github/workflows/build_deploy.yml` & `promweaver-0.3.0/.github/workflows/build_deploy.yml`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/.github/workflows/build_docs.yml` & `promweaver-0.3.0/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/LICENSE` & `promweaver-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/PKG-INFO` & `promweaver-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promweaver
-Version: 0.2.0
+Version: 0.3.0
 Summary: Prominence/Filament Radiative Transfer Modelling with Lightweaver
 Home-page: http://github.com/Goobley/Promweaver
 Author: Chris Osborne
 Author-email: christopher.osborne@glasgow.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `promweaver-0.2.0/README.md` & `promweaver-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/docs/Makefile` & `promweaver-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/docs/conf.py` & `promweaver-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/docs/index.rst` & `promweaver-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/docs/make.bat` & `promweaver-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/docs/promweaver-api.rst` & `promweaver-0.3.0/docs/promweaver-api.rst`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/iso_detailed_test.py` & `promweaver-0.3.0/iso_detailed_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import lightweaver as lw
 import matplotlib.pyplot as plt
 import numpy as np
 import promweaver as pw
 import psutil
 
 process = psutil.Process()
+
+
 def print_mem():
     print(f"Mem: {process.memory_info().rss / 1024 / 1024} MB")
 
+
 Nthreads = 8
 
-active_atoms = ['H', 'Ca', 'Mg']
+active_atoms = ["H", "Ca", "Mg"]
 
 print_mem()
 bc_ctx = pw.compute_falc_bc_ctx(active_atoms, prd=True, Nthreads=Nthreads)
 print_mem()
 bc_table = pw.tabulate_bc(bc_ctx, max_rays=10)
 print_mem()
 bc_provider = pw.TabulatedPromBcProvider(**bc_table)
 
-print('---------')
+print("---------")
 
 print_mem()
 model = pw.IsoPromModel(
-    'prominence',
+    "prominence",
     temperature=8000,
     pressure=0.05,
     thickness=0.5e6,
     vturb=5e3,
     altitude=10e6,
     active_atoms=active_atoms,
     Nthreads=Nthreads,
     Nrays=10,
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
-    prd=True
+    prd=True,
 )
 
 print_mem()
 
 model.iterate_se()
 
 detailed_atoms = ["H"]
-detailed_pops = {
-    "H": np.copy(model.eq_pops["H"])
-}
+detailed_pops = {"H": np.copy(model.eq_pops["H"])}
 model_detailed_nlte_H = pw.IsoPromModel(
-    'prominence',
+    "prominence",
     temperature=8000,
     pressure=0.05,
     thickness=0.5e6,
     vturb=5e3,
     altitude=10e6,
     active_atoms=active_atoms,
     detailed_atoms=detailed_atoms,
@@ -61,42 +62,38 @@
     bc_provider=bc_provider,
     prd=True,
 )
 print_mem()
 model_detailed_nlte_H.iterate_se()
 
 detailed_atoms = ["H"]
-detailed_pops = {
-    "H": np.copy(model.eq_pops["H"])
-}
+detailed_pops = {"H": np.copy(model.eq_pops["H"])}
 model_detailed_nlte_H_crd = pw.IsoPromModel(
-    'prominence',
+    "prominence",
     temperature=8000,
     pressure=0.05,
     thickness=0.5e6,
     vturb=5e3,
     altitude=10e6,
     active_atoms=active_atoms,
     detailed_atoms=detailed_atoms,
     detailed_pops=detailed_pops,
     Nthreads=Nthreads,
     Nrays=10,
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
     prd=True,
-    ctx_kwargs={
-        "detailedAtomPrd": False
-    },
+    ctx_kwargs={"detailedAtomPrd": False},
 )
 print_mem()
 model_detailed_nlte_H_crd.iterate_se()
 
 # NOTE(cmo): Doing detailed Mg from the start seems to need some help... it doesn't seem to start in a sensible position. Use an H and Ca only to seed it to a good NLTE start.
 model_H_Ca = pw.IsoPromModel(
-    'prominence',
+    "prominence",
     temperature=8000,
     pressure=0.05,
     thickness=0.5e6,
     vturb=5e3,
     altitude=10e6,
     active_atoms=["H", "Ca"],
     Nthreads=Nthreads,
@@ -104,19 +101,17 @@
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
     prd=True,
 )
 model_H_Ca.iterate_se()
 
 detailed_atoms = ["Mg"]
-detailed_pops = {
-    "Mg": np.copy(model.eq_pops["Mg"])
-}
+detailed_pops = {"Mg": np.copy(model.eq_pops["Mg"])}
 model_detailed_nlte_Mg = pw.IsoPromModel(
-    'prominence',
+    "prominence",
     temperature=8000,
     pressure=0.05,
     thickness=0.5e6,
     vturb=5e3,
     altitude=10e6,
     active_atoms=active_atoms,
     detailed_atoms=detailed_atoms,
@@ -132,15 +127,15 @@
 model_detailed_nlte_Mg.eq_pops["Ca"][...] = model_H_Ca.eq_pops["Ca"]
 model_detailed_nlte_Mg.atmos.ne[:] = model_H_Ca.atmos.ne
 model_detailed_nlte_Mg.atmos.nHTot[:] = model_H_Ca.atmos.nHTot
 model_detailed_nlte_Mg.iterate_se()
 
 detailed_atoms = ["H"]
 model_detailed_lte_H = pw.IsoPromModel(
-    'prominence',
+    "prominence",
     temperature=8000,
     pressure=0.05,
     thickness=0.5e6,
     vturb=5e3,
     altitude=10e6,
     active_atoms=active_atoms,
     detailed_atoms=detailed_atoms,
```

### Comparing `promweaver-0.2.0/pctr_detailed_test.py` & `promweaver-0.3.0/pctr_detailed_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import lightweaver as lw
 import matplotlib.pyplot as plt
 import numpy as np
 import promweaver as pw
 import psutil
 
 process = psutil.Process()
+
+
 def print_mem():
     print(f"Mem: {process.memory_info().rss / 1024 / 1024} MB")
 
+
 Nthreads = 8
 
-active_atoms = ['H', 'Ca', 'Mg']
+active_atoms = ["H", "Ca", "Mg"]
 
 print_mem()
 bc_ctx = pw.compute_falc_bc_ctx(active_atoms, prd=True, Nthreads=Nthreads)
 print_mem()
 bc_table = pw.tabulate_bc(bc_ctx, max_rays=10)
 print_mem()
 bc_provider = pw.TabulatedPromBcProvider(**bc_table)
 
-print('---------')
+print("---------")
 
 print_mem()
 model = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
     gamma=2,
     active_atoms=active_atoms,
     Nthreads=Nthreads,
     Nrays=10,
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
-    prd=True
+    prd=True,
 )
 
 print_mem()
 
 model.iterate_se()
 
 detailed_atoms = ["H"]
-detailed_pops = {
-    "H": np.copy(model.eq_pops["H"])
-}
+detailed_pops = {"H": np.copy(model.eq_pops["H"])}
 model_detailed_nlte_H = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
@@ -67,19 +68,17 @@
     bc_provider=bc_provider,
     prd=True,
 )
 print_mem()
 model_detailed_nlte_H.iterate_se()
 
 detailed_atoms = ["H"]
-detailed_pops = {
-    "H": np.copy(model.eq_pops["H"])
-}
+detailed_pops = {"H": np.copy(model.eq_pops["H"])}
 model_detailed_nlte_H_crd = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
@@ -88,24 +87,22 @@
     detailed_atoms=detailed_atoms,
     detailed_pops=detailed_pops,
     Nthreads=Nthreads,
     Nrays=10,
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
     prd=True,
-    ctx_kwargs={
-        "detailedAtomPrd": False
-    },
+    ctx_kwargs={"detailedAtomPrd": False},
 )
 print_mem()
 model_detailed_nlte_H_crd.iterate_se()
 
 # NOTE(cmo): Doing detailed Mg from the start seems to need some help... it doesn't seem to start in a sensible position. Use an H and Ca only to seed it to a good NLTE start.
 model_H_Ca = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
@@ -116,19 +113,17 @@
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
     prd=True,
 )
 model_H_Ca.iterate_se()
 
 detailed_atoms = ["Mg"]
-detailed_pops = {
-    "Mg": np.copy(model.eq_pops["Mg"])
-}
+detailed_pops = {"Mg": np.copy(model.eq_pops["Mg"])}
 model_detailed_nlte_Mg = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
@@ -147,15 +142,15 @@
 model_detailed_nlte_Mg.eq_pops["Ca"][...] = model_H_Ca.eq_pops["Ca"]
 model_detailed_nlte_Mg.atmos.ne[:] = model_H_Ca.atmos.ne
 model_detailed_nlte_Mg.atmos.nHTot[:] = model_H_Ca.atmos.nHTot
 model_detailed_nlte_Mg.iterate_se()
 
 detailed_atoms = ["H"]
 model_detailed_lte_H = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
```

### Comparing `promweaver-0.2.0/pctr_pw_test.py` & `promweaver-0.3.0/pctr_pw_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 import lightweaver as lw
 import matplotlib.pyplot as plt
 import numpy as np
 import promweaver as pw
 
 Nthreads = 8
 
-active_atoms = ['H', 'Ca']
+active_atoms = ["H", "Ca"]
 
 bc_ctx = pw.compute_falc_bc_ctx(active_atoms, Nthreads=Nthreads)
 bc_table = pw.tabulate_bc(bc_ctx)
 bc_provider = pw.TabulatedPromBcProvider(**bc_table)
 
-print('---------')
+print("---------")
 
-model = pw.PctrPromModel('prominence',
-                         cen_temperature=8000, tr_temperature=1e5,
-                         cen_pressure=0.05, tr_pressure=0.001,
-                         max_cmass=5e-4, vturb=5e3, altitude=10e6,
-                         gamma=2,
-                         active_atoms=active_atoms, Nthreads=Nthreads,
-                         Nrays=10, BcType=pw.ConePromBc,
-                         bc_provider=bc_provider,
-                        )
-
-modelJ = pw.PctrPromModel('prominence',
-                           cen_temperature=8000, tr_temperature=1e5,
-                           cen_pressure=0.05, tr_pressure=0.001,
-                           max_cmass=5e-4, vturb=5e3, altitude=10e6,
-                           gamma=2,
-                           active_atoms=active_atoms,
-                           Nthreads=Nthreads, bc_provider=bc_provider,
-                           BcType=pw.UniformJPromBc,
-                           Nrays=3,
-                          )
+model = pw.PctrPromModel(
+    "prominence",
+    cen_temperature=8000,
+    tr_temperature=1e5,
+    cen_pressure=0.05,
+    tr_pressure=0.001,
+    max_cmass=5e-4,
+    vturb=5e3,
+    altitude=10e6,
+    gamma=2,
+    active_atoms=active_atoms,
+    Nthreads=Nthreads,
+    Nrays=10,
+    BcType=pw.ConePromBc,
+    bc_provider=bc_provider,
+)
+
+modelJ = pw.PctrPromModel(
+    "prominence",
+    cen_temperature=8000,
+    tr_temperature=1e5,
+    cen_pressure=0.05,
+    tr_pressure=0.001,
+    max_cmass=5e-4,
+    vturb=5e3,
+    altitude=10e6,
+    gamma=2,
+    active_atoms=active_atoms,
+    Nthreads=Nthreads,
+    bc_provider=bc_provider,
+    BcType=pw.UniformJPromBc,
+    Nrays=3,
+)
 
 plt.ion()
 
 model.iterate_se()
 modelJ.iterate_se()
 Ivert = model.compute_rays(wavelengths=model.ctx.spect.wavelength, mus=1.0)
 IvertJ = modelJ.compute_rays(wavelengths=modelJ.ctx.spect.wavelength, mus=1.0)
```

### Comparing `promweaver-0.2.0/pctr_removing_lines_test.py` & `promweaver-0.3.0/pctr_removing_lines_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,65 +5,66 @@
 import promweaver as pw
 import psutil
 
 process = psutil.Process()
 
 Nthreads = 8
 
-active_atoms = ['H', 'Ca', 'Mg']
+active_atoms = ["H", "Ca", "Mg"]
 
 bc_ctx = pw.compute_falc_bc_ctx(active_atoms, prd=True, Nthreads=Nthreads)
 bc_table = pw.tabulate_bc(bc_ctx, max_rays=10)
 bc_provider = pw.TabulatedPromBcProvider(**bc_table)
 
-print('---------')
+print("---------")
 
 model = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
     gamma=2,
     active_atoms=active_atoms,
     Nthreads=Nthreads,
     Nrays=10,
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
-    prd=True
+    prd=True,
 )
 
 model.iterate_se()
 
 detailed_atoms = ["H"]
-detailed_pops = {
-    "H": np.copy(model.eq_pops["H"])
-}
+detailed_pops = {"H": np.copy(model.eq_pops["H"])}
+
+
 def H_no_lyman():
     h = H_6_atom()
     idxs_to_delete = [i for i, l in enumerate(h.lines) if l.i == 0]
     for i in reversed(idxs_to_delete):
         del h.lines[i]
 
     idxs_to_delete = [i for i, l in enumerate(h.continua) if l.i == 0]
     for i in reversed(idxs_to_delete):
         del h.continua[i]
     lw.reconfigure_atom(h)
     return h
 
+
 atomic_models = pw.default_atomic_models()
 for i, atom in enumerate(atomic_models):
     if atom.element == lw.PeriodicTable["H"]:
         atomic_models[i] = H_no_lyman()
 
 model_detailed_H_no_lyman = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
@@ -76,32 +77,34 @@
     Nrays=10,
     BcType=pw.ConePromBc,
     bc_provider=bc_provider,
     prd=True,
 )
 model_detailed_H_no_lyman.iterate_se()
 
+
 def MgII_no_resonance():
     mg = MgII_atom()
     idxs_to_delete = [i for i, l in enumerate(mg.lines) if l.i == 0]
     for i in reversed(idxs_to_delete):
         del mg.lines[i]
 
     idxs_to_delete = [i for i, l in enumerate(mg.continua) if l.i == 0]
     for i in reversed(idxs_to_delete):
         del mg.continua[i]
     lw.reconfigure_atom(mg)
     return mg
 
+
 atomic_models = pw.default_atomic_models()
 for i, atom in enumerate(atomic_models):
     if atom.element == lw.PeriodicTable["Mg"]:
         atomic_models[i] = MgII_no_resonance()
 model_detailed_Mg_no_resonance = pw.PctrPromModel(
-    'prominence',
+    "prominence",
     cen_temperature=8000,
     tr_temperature=1e5,
     cen_pressure=0.05,
     tr_pressure=0.001,
     max_cmass=5e-4,
     vturb=5e3,
     altitude=10e6,
@@ -119,11 +122,19 @@
 model_detailed_Mg_no_resonance.iterate_se()
 
 Ivert = model.compute_rays(wavelengths=model.ctx.spect.wavelength, mus=1.0)
 Ivert_detailed_H_no_lyman = model_detailed_H_no_lyman.compute_rays(mus=1.0)
 Ivert_detailed_Mg_no_resonance = model_detailed_Mg_no_resonance.compute_rays(mus=1.0)
 
 plt.ion()
-plt.plot(model.ctx.spect.wavelength, Ivert, label='Full NLTE')
-plt.plot(model_detailed_H_no_lyman.ctx.spect.wavelength, Ivert_detailed_H_no_lyman, label="No Lyman internal to prominence")
-plt.plot(model_detailed_Mg_no_resonance.ctx.spect.wavelength, Ivert_detailed_Mg_no_resonance, label="No Mg resonance internal to prominence")
+plt.plot(model.ctx.spect.wavelength, Ivert, label="Full NLTE")
+plt.plot(
+    model_detailed_H_no_lyman.ctx.spect.wavelength,
+    Ivert_detailed_H_no_lyman,
+    label="No Lyman internal to prominence",
+)
+plt.plot(
+    model_detailed_Mg_no_resonance.ctx.spect.wavelength,
+    Ivert_detailed_Mg_no_resonance,
+    label="No Mg resonance internal to prominence",
+)
 plt.legend()
```

### Comparing `promweaver-0.2.0/promweaver/bc_provider.py` & `promweaver-0.3.0/promweaver/bc_provider.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/promweaver/compute_bc.py` & `promweaver-0.3.0/promweaver/compute_bc.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/promweaver/cone_prom_bc.py` & `promweaver-0.3.0/promweaver/cone_prom_bc.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/promweaver/iso_prom.py` & `promweaver-0.3.0/promweaver/iso_prom.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         self.rad_set = lw.RadiativeSet(atomic_models)
         self.rad_set.set_active(*active_atoms)
         if detailed_atoms is not None:
             if detailed_pops is None:
                 detailed_pops = {}
             self.rad_set.set_detailed_static(*detailed_atoms)
             elements = [lw.PeriodicTable[a] for a in detailed_atoms]
-            if lw.PeriodicTable['H'] in elements:
+            if lw.PeriodicTable["H"] in elements:
                 # NOTE(cmo): Can't do charge conservation
                 self.do_pressure_updates = False
 
             # NOTE(cmo): Set ne now to correctly match pressure if "H" pops are provided
             if "H" in detailed_pops:
                 new_nHTot = np.sum(detailed_pops["H"], axis=0)
             else:
@@ -256,14 +256,15 @@
             update_model_kwargs = {}
 
         if self.prd and "prd" not in kwargs:
             kwargs["prd"] = self.prd
 
         update_model = None
         if self.do_pressure_updates:
+
             def update_model(self, printNow, **kwargs):
                 # NOTE(cmo): Fix pressure throughout the atmosphere.
                 N = (
                     lw.DefaultAtomicAbundance.totalAbundance * self.atmos.nHTot
                     + self.atmos.ne
                 )
                 NError = self.pressure / (lw.KBoltzmann * self.temperature) - N
```

### Comparing `promweaver-0.2.0/promweaver/j_prom_bc.py` & `promweaver-0.3.0/promweaver/j_prom_bc.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/promweaver/limb_darkening.py` & `promweaver-0.3.0/promweaver/limb_darkening.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/promweaver/pctr_prom.py` & `promweaver-0.3.0/promweaver/pctr_prom.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         self.rad_set = lw.RadiativeSet(atomic_models)
         self.rad_set.set_active(*active_atoms)
         if detailed_atoms is not None:
             if detailed_pops is None:
                 detailed_pops = {}
             self.rad_set.set_detailed_static(*detailed_atoms)
             elements = [lw.PeriodicTable[a] for a in detailed_atoms]
-            if lw.PeriodicTable['H'] in elements:
+            if lw.PeriodicTable["H"] in elements:
                 # NOTE(cmo): Can't do charge conservation
                 self.do_pressure_updates = False
 
             # NOTE(cmo): Set ne now to correctly match pressure if "H" pops are provided
             if "H" in detailed_pops:
                 new_nHTot = np.sum(detailed_pops["H"], axis=0)
             else:
@@ -314,14 +314,15 @@
             update_model_kwargs = {}
 
         if self.prd and "prd" not in kwargs:
             kwargs["prd"] = self.prd
 
         update_model = None
         if self.do_pressure_updates:
+
             def update_model(self, printNow, **kwargs):
                 # NOTE(cmo): Fix pressure throughout the atmosphere.
                 N = (
                     lw.DefaultAtomicAbundance.totalAbundance * self.atmos.nHTot
                     + self.atmos.ne
                 )
                 NError = self.pressure / (lw.KBoltzmann * self.temperature) - N
```

### Comparing `promweaver-0.2.0/promweaver/prom_model.py` & `promweaver-0.3.0/promweaver/prom_model.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/promweaver/utils.py` & `promweaver-0.3.0/promweaver/utils.py`

 * *Files identical despite different names*

### Comparing `promweaver-0.2.0/promweaver.egg-info/PKG-INFO` & `promweaver-0.3.0/promweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promweaver
-Version: 0.2.0
+Version: 0.3.0
 Summary: Prominence/Filament Radiative Transfer Modelling with Lightweaver
 Home-page: http://github.com/Goobley/Promweaver
 Author: Chris Osborne
 Author-email: christopher.osborne@glasgow.ac.uk
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `promweaver-0.2.0/promweaver.egg-info/SOURCES.txt` & `promweaver-0.3.0/promweaver.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 iso_detailed_test.py
 pctr_detailed_test.py
 pctr_pw_test.py
 pctr_removing_lines_test.py
 pw_test.py
 pw_test_fil.py
+pw_test_stratification.py
 pyproject.toml
 setup.py
 .github/workflows/build.yml
 .github/workflows/build_deploy.yml
 .github/workflows/build_docs.yml
 docs/Makefile
 docs/conf.py
@@ -22,14 +23,15 @@
 promweaver/cone_prom_bc.py
 promweaver/iso_prom.py
 promweaver/j_prom_bc.py
 promweaver/limb_darkening.py
 promweaver/pctr_prom.py
 promweaver/prom_bc.py
 promweaver/prom_model.py
+promweaver/stratified_prom.py
 promweaver/utils.py
 promweaver/version.py
 promweaver.egg-info/PKG-INFO
 promweaver.egg-info/SOURCES.txt
 promweaver.egg-info/dependency_links.txt
 promweaver.egg-info/requires.txt
 promweaver.egg-info/top_level.txt
```

### Comparing `promweaver-0.2.0/pw_test.py` & `promweaver-0.3.0/pw_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,48 +2,66 @@
 from os import path
 
 import lightweaver as lw
 import matplotlib.pyplot as plt
 import numpy as np
 import promweaver as pw
 
-active_atoms = ['H', 'Ca']
+active_atoms = ["H", "Ca"]
 Nthreads = 8
 # NOTE(cmo): String hashes are not stable across python runs. Huh.
 # active_atoms_hash = sum(hash(a) for a in active_atoms)
-active_atoms_hash = ''.join(sorted(active_atoms))
+active_atoms_hash = "".join(sorted(active_atoms))
 
-data_path = f'FalcTabulatedBcData_{active_atoms_hash}.pickle'
+data_path = f"FalcTabulatedBcData_{active_atoms_hash}.pickle"
 if path.isfile(data_path):
-    with open(data_path, 'rb') as pkl:
+    with open(data_path, "rb") as pkl:
         bc_table = pickle.load(pkl)
 else:
     bc_ctx = pw.compute_falc_bc_ctx(active_atoms, Nthreads=Nthreads)
     bc_table = pw.tabulate_bc(bc_ctx)
 
-    with open(data_path, 'wb') as pkl:
+    with open(data_path, "wb") as pkl:
         pickle.dump(bc_table, pkl)
 
-    print(f'Made BC data and written to {data_path}')
+    print(f"Made BC data and written to {data_path}")
 
 bc_provider = pw.TabulatedPromBcProvider(**bc_table)
 
-model = pw.IsoPromModel('prominence', 8000, 0.05, 10e6, 5e3, 1e7, active_atoms=active_atoms,
-                        Nthreads=Nthreads,
-                        Nrays=10, BcType=pw.ConePromBc,
-                        bc_provider=bc_provider,
-                        ctx_kwargs={'ngOptions': lw.NgOptions(2, 5, 10)})
-
-modelJ = pw.IsoPromModel('prominence', 8000, 0.05, 10e6, 5e3, 1e7, active_atoms=active_atoms,
-                         Nthreads=Nthreads,
-                         ctx_kwargs={'ngOptions': lw.NgOptions(2, 5, 10)}, prd=True)
+model = pw.IsoPromModel(
+    "prominence",
+    8000,
+    0.05,
+    10e6,
+    5e3,
+    1e7,
+    active_atoms=active_atoms,
+    Nthreads=Nthreads,
+    Nrays=10,
+    BcType=pw.ConePromBc,
+    bc_provider=bc_provider,
+    ctx_kwargs={"ngOptions": lw.NgOptions(2, 5, 10)},
+)
+
+modelJ = pw.IsoPromModel(
+    "prominence",
+    8000,
+    0.05,
+    10e6,
+    5e3,
+    1e7,
+    active_atoms=active_atoms,
+    Nthreads=Nthreads,
+    ctx_kwargs={"ngOptions": lw.NgOptions(2, 5, 10)},
+    prd=True,
+)
 
 plt.ion()
 
 modelJ.iterate_se()
 model.iterate_se()
 IvertJ = modelJ.compute_rays(mus=1.0)
 IvertCtx = model.compute_rays(mus=1.0)
 
 wave = model.ctx.spect.wavelength
 plt.plot(wave, IvertJ)
-plt.plot(wave, IvertCtx, '--')
+plt.plot(wave, IvertCtx, "--")
```

### Comparing `promweaver-0.2.0/pw_test_fil.py` & `promweaver-0.3.0/pw_test_fil.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,36 +2,45 @@
 from os import path
 
 import lightweaver as lw
 import matplotlib.pyplot as plt
 import numpy as np
 import promweaver as pw
 
-active_atoms = ['H', 'Ca']
+active_atoms = ["H", "Ca"]
 Nthreads = 8
 # NOTE(cmo): String hashes are not stable across python runs. Huh.
 # active_atoms_hash = sum(hash(a) for a in active_atoms)
-active_atoms_hash = ''.join(sorted(active_atoms))
+active_atoms_hash = "".join(sorted(active_atoms))
 
-data_path = f'FalcTabulatedBcData_{active_atoms_hash}.pickle'
+data_path = f"FalcTabulatedBcData_{active_atoms_hash}.pickle"
 if path.isfile(data_path):
-    with open(data_path, 'rb') as pkl:
+    with open(data_path, "rb") as pkl:
         bc_table = pickle.load(pkl)
 else:
     bc_ctx = pw.compute_falc_bc_ctx(active_atoms, Nthreads=Nthreads)
     bc_table = pw.tabulate_bc(bc_ctx)
 
-    with open(data_path, 'wb') as pkl:
+    with open(data_path, "wb") as pkl:
         pickle.dump(bc_table, pkl)
 
-    print(f'Made BC data and written to {data_path}')
+    print(f"Made BC data and written to {data_path}")
 
 bc_provider = pw.TabulatedPromBcProvider(**bc_table)
 
-model = pw.IsoPromModel('filament', 8000, 0.05, 10e6, 5e3, 1e7, active_atoms=active_atoms,
-                        Nthreads=12, bc_provider=bc_provider,
-                        ctx_kwargs={'ngOptions': lw.NgOptions(2, 5, 10)})
+model = pw.IsoPromModel(
+    "filament",
+    8000,
+    0.05,
+    10e6,
+    5e3,
+    1e7,
+    active_atoms=active_atoms,
+    Nthreads=12,
+    bc_provider=bc_provider,
+    ctx_kwargs={"ngOptions": lw.NgOptions(2, 5, 10)},
+)
 model.iterate_se()
 Is = model.compute_rays()
 wave = model.ctx.spect.wavelength
 plt.ion()
 plt.plot(wave, Is)
```

### Comparing `promweaver-0.2.0/setup.py` & `promweaver-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup
 
+
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
+
 setup(
     name="promweaver",
     setup_requires=["setuptools_scm"],
     use_scm_version=True,
     packages=["promweaver"],
     install_requires=["lightweaver>=0.8.0rc6"],
     author="Chris Osborne",
     author_email="christopher.osborne@glasgow.ac.uk",
     license="MIT",
     url="http://github.com/Goobley/Promweaver",
     description="Prominence/Filament Radiative Transfer Modelling with Lightweaver",
     long_description=readme(),
     long_description_content_type="text/markdown",
-    python_requires=">=3.8"
-)
+    python_requires=">=3.8",
+)
```

