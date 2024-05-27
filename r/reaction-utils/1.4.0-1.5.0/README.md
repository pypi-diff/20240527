# Comparing `tmp/reaction_utils-1.4.0.tar.gz` & `tmp/reaction_utils-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaction_utils-1.4.0.tar", max compression
+gzip compressed data, was "reaction_utils-1.5.0.tar", max compression
```

## Comparing `reaction_utils-1.4.0.tar` & `reaction_utils-1.5.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0    11365 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/LICENSE
--rw-r--r--   0        0        0     4389 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/README.md
--rw-r--r--   0        0        0     1443 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/__init__.py
--rw-r--r--   0        0        0     5542 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/cgr.py
--rw-r--r--   0        0        0    25245 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/reaction.py
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/rinchi/__init__.py
--rw-r--r--   0        0        0     3185 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/rinchi/download_rinchi.py
--rw-r--r--   0        0        0     3048 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/rinchi/rinchi_api.py
--rw-r--r--   0        0        0    15259 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/template.py
--rw-r--r--   0        0        0    24318 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/chem/utils.py
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/data/__init__.py
--rw-r--r--   0        0        0     2492 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/data/base_pipeline.py
--rw-r--r--   0        0        0     4113 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/data/batch_utils.py
--rw-r--r--   0        0        0      581 2024-03-14 09:54:39.225433 reaction_utils-1.4.0/rxnutils/data/clean_pipeline.yml
--rw-r--r--   0        0        0     2466 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/mapping.py
--rw-r--r--   0        0        0     2043 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/mapping_pipeline.py
--rw-r--r--   0        0        0     1626 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/ord/README.md
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/ord/__init__.py
--rw-r--r--   0        0        0     2608 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/ord/import_ord_dataset.py
--rw-r--r--   0        0        0     1764 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/ord/preparation_pipeline.py
--rw-r--r--   0        0        0     1260 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/uspto/README.md
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/uspto/__init__.py
--rw-r--r--   0        0        0     1657 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/uspto/combine.py
--rw-r--r--   0        0        0     1932 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/uspto/download.py
--rw-r--r--   0        0        0     1691 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/data/uspto/preparation_pipeline.py
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/actions/__init__.py
--rw-r--r--   0        0        0     5970 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/actions/dataframe_mod.py
--rw-r--r--   0        0        0    19289 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/actions/reaction_mod.py
--rw-r--r--   0        0        0    33239 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/actions/reaction_props.py
--rw-r--r--   0        0        0     4758 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/actions/templates.py
--rw-r--r--   0        0        0     5368 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/base.py
--rw-r--r--   0        0        0     3151 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/pipeline/runner.py
--rw-r--r--   0        0        0        0 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/routes/__init__.py
--rw-r--r--   0        0        0    23023 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/routes/base.py
--rw-r--r--   0        0        0    10740 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/routes/image.py
--rw-r--r--   0        0        0     7252 2024-03-14 09:54:39.229433 reaction_utils-1.4.0/rxnutils/routes/readers.py
--rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 reaction_utils-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11365 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4389 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/README.md
+-rw-r--r--   0        0        0     1443 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/rxnutils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/rxnutils/chem/__init__.py
+-rw-r--r--   0        0        0     5542 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/rxnutils/chem/cgr.py
+-rw-r--r--   0        0        0     4608 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/rxnutils/chem/disconnection_sites/atom_map_tagging.py
+-rw-r--r--   0        0        0     6340 2024-05-27 11:34:58.150877 reaction_utils-1.5.0/rxnutils/chem/disconnection_sites/tag_converting.py
+-rw-r--r--   0        0        0    25245 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/chem/reaction.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/chem/rinchi/__init__.py
+-rw-r--r--   0        0        0     3190 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/chem/rinchi/download_rinchi.py
+-rw-r--r--   0        0        0     3048 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/chem/rinchi/rinchi_api.py
+-rw-r--r--   0        0        0    15259 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/chem/template.py
+-rw-r--r--   0        0        0    24317 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/chem/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/__init__.py
+-rw-r--r--   0        0        0     2492 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/base_pipeline.py
+-rw-r--r--   0        0        0     4223 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/batch_utils.py
+-rw-r--r--   0        0        0      581 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/clean_pipeline.yml
+-rw-r--r--   0        0        0     2466 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/mapping.py
+-rw-r--r--   0        0        0     2043 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/mapping_pipeline.py
+-rw-r--r--   0        0        0     1626 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/ord/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/ord/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/ord/import_ord_dataset.py
+-rw-r--r--   0        0        0     1764 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/ord/preparation_pipeline.py
+-rw-r--r--   0        0        0     1260 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/uspto/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/uspto/__init__.py
+-rw-r--r--   0        0        0     1657 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/uspto/combine.py
+-rw-r--r--   0        0        0     1932 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/uspto/download.py
+-rw-r--r--   0        0        0     1691 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/data/uspto/preparation_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/actions/__init__.py
+-rw-r--r--   0        0        0     5970 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/actions/dataframe_mod.py
+-rw-r--r--   0        0        0    21438 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/actions/reaction_mod.py
+-rw-r--r--   0        0        0    33239 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/actions/reaction_props.py
+-rw-r--r--   0        0        0     4758 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/actions/templates.py
+-rw-r--r--   0        0        0     5368 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/base.py
+-rw-r--r--   0        0        0     3151 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/pipeline/runner.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/routes/__init__.py
+-rw-r--r--   0        0        0    23442 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/routes/base.py
+-rw-r--r--   0        0        0    10740 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/routes/image.py
+-rw-r--r--   0        0        0     7252 2024-05-27 11:34:58.154877 reaction_utils-1.5.0/rxnutils/routes/readers.py
+-rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 reaction_utils-1.5.0/PKG-INFO
```

### Comparing `reaction_utils-1.4.0/LICENSE` & `reaction_utils-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/README.md` & `reaction_utils-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/pyproject.toml` & `reaction_utils-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reaction_utils"
-version = "1.4.0"
+version = "1.5.0"
 description = "Utilities for working with reactions, reaction templates and template extraction"
 authors = ["Genheden, Samuel <samuel.genheden@astrazeneca.com>", "Kannas, Christos <christos.kannas@astrazeneca.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/MolecularAI/reaction_utils/"
 repository = "https://github.com/MolecularAI/reaction_utils/"
 documentation = "https://molecularai.github.io/reaction_utils/"
```

### Comparing `reaction_utils-1.4.0/rxnutils/chem/cgr.py` & `reaction_utils-1.5.0/rxnutils/chem/cgr.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/chem/reaction.py` & `reaction_utils-1.5.0/rxnutils/chem/reaction.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/chem/rinchi/download_rinchi.py` & `reaction_utils-1.5.0/rxnutils/chem/rinchi/download_rinchi.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "win32": "windows",
 }
 
 PLATFORM2EXTENSION = {"linux": "", "win32": ".exe"}
 
 CONFIG = {
     "download_folder": ".",
-    "download_url": "http://www.inchi-trust.org/download/RInChI/RInChI-V1-00.zip",
+    "download_url": "https://www.inchi-trust.org/wp/download/RInChI/RInChI-V1-00.zip",
 }
 PATH = os.path.dirname(__file__)
 
 
 class RInChIError(Exception):
     """Exception raised by RInChI API"""
 
@@ -31,41 +31,41 @@
 
     :return: Path of the folder containing the appropriate
              command line executable based on system type.
     """
     if sys.platform not in PLATFORM2FOLDER:
         raise RInChIError("RInChI software not supported on this platform")
 
-    rinchi_url = CONFIG.get("download_url")
+    rinchi_url = CONFIG.get("download_url", "")
     rinchi_fn = rinchi_url.split("/")[-1]
-    download_loc = CONFIG.get("download_folder")
+    download_loc = CONFIG.get("download_folder", "")
     download_loc = os.path.join(PATH, download_loc)
     rinchi_fn = os.path.join(download_loc, rinchi_fn)
     if not os.path.exists(rinchi_fn):
         if not os.path.exists(download_loc):
             logging.info(f"Creating: {download_loc}")
             os.makedirs(download_loc)
         logging.info(f"Downloading: {rinchi_url}")
         req = requests.get(rinchi_url)
         logging.debug(f"{req.status_code}")
         logging.debug(f"{req.headers}")
         req.raise_for_status()
         logging.info(f"Creating: {rinchi_fn}")
-        with open(rinchi_fn, "wb") as fileobj:
-            fileobj.write(req.content)
+        with open(rinchi_fn, "wb") as in_fp:
+            in_fp.write(req.content)
         logging.info("Download completed...")
         logging.info(f"Unziping: {rinchi_fn}")
-        with ZipFile(rinchi_fn, "r") as fileobj:
+        with ZipFile(rinchi_fn, "r") as out_fp:
             bin_path = [
                 x
-                for x in fileobj.namelist()
+                for x in out_fp.namelist()
                 if x.endswith(_exec_folder_ending(os_sep=False) + "/")
             ]
             logging.debug(bin_path)
-            fileobj.extractall(download_loc)
+            out_fp.extractall(download_loc)
         logging.info("Completed...")
         rinchi_cli_path = os.path.join(download_loc, bin_path[0])
         logging.info(f"RInChI CLI: {rinchi_cli_path}")
         if sys.platform == "linux":
             os.chmod(os.path.join(rinchi_cli_path, "rinchi_cmdline"), stat.S_IEXEC)
     else:
         logging.info(f"RInChI exists at: {rinchi_fn}")
```

### Comparing `reaction_utils-1.4.0/rxnutils/chem/rinchi/rinchi_api.py` & `reaction_utils-1.5.0/rxnutils/chem/rinchi/rinchi_api.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/chem/template.py` & `reaction_utils-1.5.0/rxnutils/chem/template.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/chem/utils.py` & `reaction_utils-1.5.0/rxnutils/chem/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module containing various chemical utility routines"""
+
 import logging
 import functools
 from typing import List, Tuple
 
 
 import rdchiral.template_extractor
 
@@ -287,15 +288,15 @@
             "[#6]-[#6]-[#7](-[#6]-[#6])-[#6](=O)-[#16]-[#6]",
         ),  # N,N-ethyl thiocarbamate
         (range(7), "[#6]-[#16]-[#6](=O)-[#7](-[#6])-[#6]"),  # N,N-methyl thiocarbamate
     ]
 
     # Build list
     groups = []
-    for (add_if_match, template) in group_templates:
+    for add_if_match, template in group_templates:
         matches = mol.GetSubstructMatches(
             Chem.MolFromSmarts(template), useChirality=True
         )
         for match in matches:
             add_if = []
             for pattern_idx, atom_idx in enumerate(match):
                 if pattern_idx in add_if_match:
```

### Comparing `reaction_utils-1.4.0/rxnutils/data/base_pipeline.py` & `reaction_utils-1.5.0/rxnutils/data/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/batch_utils.py` & `reaction_utils-1.5.0/rxnutils/data/batch_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,17 @@
     """
     if output_filename and Path(output_filename).exists():
         return [(-1, None, None)]
 
     file_size = (
         nlines(filename) - 1
     )  # Header should not be counted for batch size calculations
+    nbatches = min(
+        file_size, nbatches
+    )  # Adjust the number of batches to the size of the file
     batch_size, remainder = divmod(file_size, nbatches)
     stop = 1  # 1-indexed to account for header in the .csv file
     batches = []
     for partition_idx in range(1, nbatches + 1):
         start = stop
         stop += batch_size + 1 if partition_idx <= remainder else batch_size
         batches.append((partition_idx - 1, start, stop))
```

### Comparing `reaction_utils-1.4.0/rxnutils/data/clean_pipeline.yml` & `reaction_utils-1.5.0/rxnutils/data/clean_pipeline.yml`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/mapping.py` & `reaction_utils-1.5.0/rxnutils/data/mapping.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/mapping_pipeline.py` & `reaction_utils-1.5.0/rxnutils/data/mapping_pipeline.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/ord/README.md` & `reaction_utils-1.5.0/rxnutils/data/ord/README.md`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/ord/import_ord_dataset.py` & `reaction_utils-1.5.0/rxnutils/data/ord/import_ord_dataset.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/ord/preparation_pipeline.py` & `reaction_utils-1.5.0/rxnutils/data/ord/preparation_pipeline.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/uspto/README.md` & `reaction_utils-1.5.0/rxnutils/data/uspto/README.md`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/uspto/combine.py` & `reaction_utils-1.5.0/rxnutils/data/uspto/combine.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/uspto/download.py` & `reaction_utils-1.5.0/rxnutils/data/uspto/download.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/data/uspto/preparation_pipeline.py` & `reaction_utils-1.5.0/rxnutils/data/uspto/preparation_pipeline.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/pipeline/actions/dataframe_mod.py` & `reaction_utils-1.5.0/rxnutils/pipeline/actions/dataframe_mod.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/pipeline/actions/reaction_mod.py` & `reaction_utils-1.5.0/rxnutils/pipeline/actions/reaction_mod.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Module containing actions on reactions that modify the reaction in some way"""
+
 from __future__ import annotations
 
 import os
-import re
 import subprocess
 import sys
 import tempfile
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from pathlib import Path
 from typing import ClassVar, List, Tuple
 
 import pandas as pd
 from rdkit import Chem, RDLogger
 from rdkit.Chem import RDConfig
 
+from rxnutils.chem.disconnection_sites.atom_map_tagging import atom_map_tag_products
+from rxnutils.chem.disconnection_sites.tag_converting import convert_atom_map_tag
 from rxnutils.chem.utils import (
     atom_mapping_numbers,
     neutralize_molecules,
     remove_atom_mapping,
     desalt_molecules,
-    split_smiles_from_reaction,
-    join_smiles_from_reaction,
 )
 from rxnutils.pipeline.base import ReactionActionMixIn, action, global_apply
 
 CONTRIB_INSTALLED = os.path.exists(RDConfig.RDContribDir)
 if CONTRIB_INSTALLED:
     # RDKit contrib is not default part of PYTHONPATH
     sys.path.append(RDConfig.RDContribDir)
@@ -541,14 +541,72 @@
         return pd.Series(
             {"reactants": reactants, "reagents": reagents, "products": products}
         )
 
 
 @action
 @dataclass
+class AtomMapTagDisconnectionSite(ReactionActionMixIn):
+    """Action for tagging disconnection site in products with atom-map '[<atom>:1]'."""
+
+    pretty_name: ClassVar[str] = "atom_map_tag_disconnection_site"
+    in_column: str = "RxnSmilesClean"
+    out_column: str = "products_atom_map_tagged"
+
+    def __call__(self, data: pd.DataFrame) -> pd.DataFrame:
+        smiles_col = global_apply(data, self._row_action, axis=1)
+        return data.assign(**{self.out_column: smiles_col})
+
+    def __str__(self) -> str:
+        return f"{self.pretty_name} (tag disconnection sites in products with '[<atom>:1]')"
+
+    def _row_action(self, row: pd.Series) -> str:
+        return atom_map_tag_products(row[self.in_column])
+
+
+@action
+@dataclass
+class ConvertAtomMapDisconnectionTag(ReactionActionMixIn):
+    """Action for converting atom-map tagging to exclamation mark tagging.
+
+    yaml example:
+
+    convert_atom_map_disconnection_tag:
+        in_column_tagged: products_atom_map_tagged
+        in_column_untagged: products
+        out_column_tagged: products_tagged
+        out_column_reconstructed: products_reconstructed
+    """
+
+    pretty_name: ClassVar[str] = "convert_atom_map_disconnection_tag"
+    in_column: str = "products_atom_map_tagged"
+    out_column_tagged: str = "products_tagged"
+    out_column_reconstructed: str = "products_reconstructed"
+
+    def __call__(self, data: pd.DataFrame) -> pd.DataFrame:
+        smiles_tagged_col = global_apply(data, self._row_action, axis=1)
+        smiles_reconstructed_col = smiles_tagged_col.str.replace("!", "")
+
+        return data.assign(
+            **{
+                self.out_column_tagged: smiles_tagged_col,
+                self.out_column_reconstructed: smiles_reconstructed_col,
+            }
+        )
+
+    def __str__(self) -> str:
+        return f"{self.pretty_name} (convert disconnection tagging '[<atom>:1]' to '<atom>!')"
+
+    def _row_action(self, row: pd.Series) -> str:
+        product_tagged = convert_atom_map_tag(row[self.in_column])
+        return product_tagged
+
+
+@action
+@dataclass
 class TrimRxnSmiles:
     """Action from trimming reaction SMILES"""
 
     pretty_name: ClassVar[str] = "trim_rxn_smiles"
     in_column: str
     out_column: str = "RxnSmiles"
     smiles_column_index: int = 0
```

### Comparing `reaction_utils-1.4.0/rxnutils/pipeline/actions/reaction_props.py` & `reaction_utils-1.5.0/rxnutils/pipeline/actions/reaction_props.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/pipeline/actions/templates.py` & `reaction_utils-1.5.0/rxnutils/pipeline/actions/templates.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/pipeline/base.py` & `reaction_utils-1.5.0/rxnutils/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/pipeline/runner.py` & `reaction_utils-1.5.0/rxnutils/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/routes/base.py` & `reaction_utils-1.5.0/rxnutils/routes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Contains a class encapsulating a synthesis route,
 as well as routines for assigning proper atom-mapping
 and drawing the route
 """
 
-from typing import Dict, Any, List, Callable
+from typing import Dict, Any, List, Callable, Union
 from copy import deepcopy
 from operator import itemgetter
 
 import pandas as pd
 from PIL.Image import Image as PilImage
 from rdkit import Chem
 
@@ -20,15 +20,15 @@
     join_smiles_from_reaction,
 )
 
 
 class SynthesisRoute:
     """
     This encapsulates a synthesis route or a reaction tree.
-    It provides convenient methods for assigning atom-mapping
+    It provide convenient methods for assigning atom-mapping
     to the reactions, and for providing reaction-level data
     of the route
 
     It is typically initiallized by one of the readers in the
     `rxnutils.routes.readers` module.
 
     The tree depth and the forward step are automatically assigned
@@ -64,19 +64,21 @@
     def atom_mapped_reaction_smiles(self) -> List[str]:
         """Returns a list of the atom-mapped reaction SMILES in the route"""
         smiles = []
         _collect_atom_mapped_smiles(self.reaction_tree, smiles)
         return smiles
 
     def assign_atom_mapping(
-        self, overwrite: bool = False, only_rxnmapper: bool = False
+        self,
+        overwrite: bool = False,
+        only_rxnmapper: bool = False,
     ) -> None:
         """
         Assign atom-mapping to each reaction in the route and
-        ensure that is consistent from root compound and throughout
+        ensure that it is consistent from root compound and throughout
         the route.
 
         It will use NameRxn to assign classification and possiblty atom-mapping,
         as well as rxnmapper to assign atom-mapping in case NameRxn cannot classify
         a reaction.
 
         :param overwrite: if True will overwrite existing mapping
@@ -88,15 +90,15 @@
 
     def chains(
         self, complexity_func: Callable[[str], float]
     ) -> List[List[Dict[str, Any]]]:
         """
         Returns linear sequences or chains extracted from the route.
 
-        Each chain is a list of dictionaries representing the molecules, only the most
+        Each chain is a list of a dictionary representing the molecules, only the most
         complex molecule is kept for each reaction - making the chain a sequence of molecule
         to molecule transformation.
 
         The first chain will be the longest linear sequence (LLS), and the second chain
         will be longest branch if this is a convergent route. This branch will be processed
         further, but the other branches can probably be discarded as they have not been
         investigated thoroughly.
@@ -164,27 +166,33 @@
         smiles = []
         _collect_reaction_smiles(self.reaction_tree, smiles)
         return smiles
 
     def remap(self, other: "SynthesisRoute") -> None:
         """
         Remap the reaction so that it follows the mapping of a
-        root compound in a reference routes
+        1) root compound in a reference route, 2) a ref compound given
+        as a SMILES, or 3) using a raw mapping
 
-        :param other: the reference route
+        :param other: the reference for re-mapping
         """
-        try:
-            ref = other.mapped_root_smiles
-            other = self.mapped_root_smiles
-        except ValueError as err:
-            # For single-compound routes, we can just ignore this
-            if str(err).startswith("Single"):
+        if isinstance(other, SynthesisRoute):
+            if len(self.reaction_smiles()) == 0 or len(other.reaction_smiles()) == 0:
+                return
+            mapping_dict = _find_remapping(
+                other.mapped_root_smiles, self.mapped_root_smiles
+            )
+        elif isinstance(other, str):
+            if len(self.reaction_smiles()) == 0:
                 return
-            raise
-        mapping_dict = _find_remapping(ref, other)
+            mapping_dict = _find_remapping(other, self.mapped_root_smiles)
+        elif isinstance(other, dict):
+            mapping_dict = other
+        else:
+            raise ValueError(f"Cannot perform re-mapping using a {type(other)}")
         _remap_reactions(self.reaction_tree, mapping_dict)
 
     def _assign_mapping(
         self, overwrite: bool = False, only_rxnmapper: bool = False
     ) -> None:
         if not overwrite:
             try:
@@ -192,19 +200,22 @@
             except KeyError:
                 # We will just create the mapping
                 pass
             else:
                 return
 
         df = pd.DataFrame({"smiles": list(set(self.reaction_smiles()))})
-        nextmove_action = NameRxn(in_column="smiles")
+        nextmove_action = NameRxn(in_column="smiles", nm_rxn_column="mapped_smiles")
         rxnmapper_action = RxnMapper(in_column="smiles")
         df = rxnmapper_action(nextmove_action(df))
         if only_rxnmapper:
-            df["NextMoveRxnSmiles"] = df["RxnmapperRxnSmiles"]
+            df["mapped_smiles"] = df["RxnmapperRxnSmiles"]
+        else:
+            sel = df["NMC"] == "0.0"
+            df["mapped_smiles"].mask(sel, df["RxnmapperRxnSmiles"], inplace=True)
         datamap = df.set_index("smiles").to_dict("index")
         _copy_mapping_from_datamap(self.reaction_tree, datamap)
 
     def _create_atom_mapping_tree(self) -> Dict[str, Any]:
         dict_ = deepcopy(self.reaction_tree)
         _assign_atom_mapped_smiles(dict_)
         return dict_
@@ -485,18 +496,15 @@
     grandchildren = children[0]["children"]
     reactants = join_smiles_from_reaction(
         [grandchild["smiles"] for grandchild in grandchildren]
     )
     rxnsmi = f"{reactants}>>{tree_dict['smiles']}"
     metadata = children[0].get("metadata", {})
     metadata["classification"] = datamap[rxnsmi]["NMC"]
-    if datamap[rxnsmi]["NMC"] == "0.0":
-        metadata["mapped_reaction_smiles"] = datamap[rxnsmi]["RxnmapperRxnSmiles"]
-    else:
-        metadata["mapped_reaction_smiles"] = datamap[rxnsmi]["NextMoveRxnSmiles"]
+    metadata["mapped_reaction_smiles"] = datamap[rxnsmi]["mapped_smiles"]
     metadata = children[0]["metadata"] = metadata
     for grandchild in grandchildren:
         _copy_mapping_from_datamap(grandchild, datamap)
 
 
 def _extract_chain_molecules(
     tree_dict: Dict[str, Any],
```

### Comparing `reaction_utils-1.4.0/rxnutils/routes/image.py` & `reaction_utils-1.5.0/rxnutils/routes/image.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/rxnutils/routes/readers.py` & `reaction_utils-1.5.0/rxnutils/routes/readers.py`

 * *Files identical despite different names*

### Comparing `reaction_utils-1.4.0/PKG-INFO` & `reaction_utils-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaction_utils
-Version: 1.4.0
+Version: 1.5.0
 Summary: Utilities for working with reactions, reaction templates and template extraction
 Home-page: https://github.com/MolecularAI/reaction_utils/
 License: Apache-2.0
 Author: Genheden, Samuel
 Author-email: samuel.genheden@astrazeneca.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

