# Comparing `tmp/mdsubsampler-0.0.4.tar.gz` & `tmp/mdsubsampler-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdsubsampler-0.0.4.tar", max compression
+gzip compressed data, was "mdsubsampler-0.0.5.tar", max compression
```

## Comparing `mdsubsampler-0.0.4.tar` & `mdsubsampler-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-09-25 10:47:35.528482 mdsubsampler-0.0.4/LICENSE
--rw-r--r--   0        0        0     5618 2023-09-25 10:47:35.528780 mdsubsampler-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-09-25 10:47:35.579816 mdsubsampler-0.0.4/mdss/__init__.py
--rw-r--r--   0        0        0     9833 2023-09-25 10:47:35.580022 mdsubsampler-0.0.4/mdss/dissimilarity.py
--rw-r--r--   0        0        0    15299 2023-09-25 10:47:35.580216 mdsubsampler-0.0.4/mdss/geometrical_property.py
--rw-r--r--   0        0        0     5268 2023-09-25 10:47:35.580370 mdsubsampler-0.0.4/mdss/graph.py
--rw-r--r--   0        0        0     1472 2023-10-16 14:21:46.792521 mdsubsampler-0.0.4/mdss/log_setup.py
--rw-r--r--   0        0        0     7258 2023-09-25 10:47:35.580702 mdsubsampler-0.0.4/mdss/parser.py
--rw-r--r--   0        0        0     5385 2023-09-25 10:47:35.580882 mdsubsampler-0.0.4/mdss/pca_property.py
--rw-r--r--   0        0        0    13148 2023-09-25 10:47:35.581207 mdsubsampler-0.0.4/mdss/property.py
--rw-r--r--   0        0        0    13055 2024-01-22 12:12:53.386598 mdsubsampler-0.0.4/mdss/protein_data.py
--rw-r--r--   0        0        0     7164 2023-10-16 12:43:27.352443 mdsubsampler-0.0.4/mdss/run.py
--rw-r--r--   0        0        0    29630 2023-09-25 10:47:35.582459 mdsubsampler-0.0.4/mdss/sampler.py
--rw-r--r--   0        0        0        0 2023-09-25 10:47:35.583260 mdsubsampler-0.0.4/mdss/scenarios/__init__.py
--rw-r--r--   0        0        0   191104 2023-09-25 10:47:35.585384 mdsubsampler-0.0.4/mdss/scenarios/scenario_1.ipynb
--rw-r--r--   0        0        0     3467 2023-12-31 13:42:17.878072 mdsubsampler-0.0.4/mdss/scenarios/scenario_1.py
--rw-r--r--   0        0        0    43744 2023-09-25 10:47:35.586336 mdsubsampler-0.0.4/mdss/scenarios/scenario_2.ipynb
--rw-r--r--   0        0        0     3379 2023-09-25 10:47:35.586728 mdsubsampler-0.0.4/mdss/scenarios/scenario_2.py
--rw-r--r--   0        0        0    41937 2023-12-31 14:21:52.487371 mdsubsampler-0.0.4/mdss/scenarios/scenario_3.ipynb
--rw-r--r--   0        0        0     3051 2023-09-25 10:47:35.587801 mdsubsampler-0.0.4/mdss/scenarios/scenario_3.py
--rw-r--r--   0        0        0     9159 2023-09-25 10:47:35.588218 mdsubsampler-0.0.4/mdss/utilities.py
--rw-r--r--   0        0        0      817 2024-01-22 12:15:44.552365 mdsubsampler-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6521 1970-01-01 00:00:00.000000 mdsubsampler-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-25 10:47:35.528482 mdsubsampler-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5618 2023-09-25 10:47:35.528780 mdsubsampler-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-09-25 10:47:35.579816 mdsubsampler-0.0.5/mdss/__init__.py
+-rw-r--r--   0        0        0     9833 2023-09-25 10:47:35.580022 mdsubsampler-0.0.5/mdss/dissimilarity.py
+-rw-r--r--   0        0        0    15299 2024-01-25 14:27:33.129065 mdsubsampler-0.0.5/mdss/geometrical_property.py
+-rw-r--r--   0        0        0     5268 2023-09-25 10:47:35.580370 mdsubsampler-0.0.5/mdss/graph.py
+-rw-r--r--   0        0        0     1472 2023-10-16 14:21:46.792521 mdsubsampler-0.0.5/mdss/log_setup.py
+-rw-r--r--   0        0        0     7224 2024-01-25 14:27:56.585334 mdsubsampler-0.0.5/mdss/parser.py
+-rw-r--r--   0        0        0     5385 2023-09-25 10:47:35.580882 mdsubsampler-0.0.5/mdss/pca_property.py
+-rw-r--r--   0        0        0    13148 2023-09-25 10:47:35.581207 mdsubsampler-0.0.5/mdss/property.py
+-rw-r--r--   0        0        0    13020 2024-01-25 14:24:10.354202 mdsubsampler-0.0.5/mdss/protein_data.py
+-rw-r--r--   0        0        0     7164 2024-01-22 16:49:07.374120 mdsubsampler-0.0.5/mdss/run.py
+-rw-r--r--   0        0        0    29630 2023-09-25 10:47:35.582459 mdsubsampler-0.0.5/mdss/sampler.py
+-rw-r--r--   0        0        0        0 2023-09-25 10:47:35.583260 mdsubsampler-0.0.5/mdss/scenarios/__init__.py
+-rw-r--r--   0        0        0   191104 2023-09-25 10:47:35.585384 mdsubsampler-0.0.5/mdss/scenarios/scenario_1.ipynb
+-rw-r--r--   0        0        0     3467 2023-12-31 13:42:17.878072 mdsubsampler-0.0.5/mdss/scenarios/scenario_1.py
+-rw-r--r--   0        0        0    43744 2023-09-25 10:47:35.586336 mdsubsampler-0.0.5/mdss/scenarios/scenario_2.ipynb
+-rw-r--r--   0        0        0     3379 2023-09-25 10:47:35.586728 mdsubsampler-0.0.5/mdss/scenarios/scenario_2.py
+-rw-r--r--   0        0        0    41937 2023-12-31 14:21:52.487371 mdsubsampler-0.0.5/mdss/scenarios/scenario_3.ipynb
+-rw-r--r--   0        0        0     3051 2023-09-25 10:47:35.587801 mdsubsampler-0.0.5/mdss/scenarios/scenario_3.py
+-rw-r--r--   0        0        0     9159 2023-09-25 10:47:35.588218 mdsubsampler-0.0.5/mdss/utilities.py
+-rw-r--r--   0        0        0      840 2024-01-25 14:31:22.863865 mdsubsampler-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6566 1970-01-01 00:00:00.000000 mdsubsampler-0.0.5/PKG-INFO
```

### Comparing `mdsubsampler-0.0.4/LICENSE` & `mdsubsampler-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/README.md` & `mdsubsampler-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/dissimilarity.py` & `mdsubsampler-0.0.5/mdss/dissimilarity.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/geometrical_property.py` & `mdsubsampler-0.0.5/mdss/geometrical_property.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/graph.py` & `mdsubsampler-0.0.5/mdss/graph.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/log_setup.py` & `mdsubsampler-0.0.5/mdss/log_setup.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/parser.py` & `mdsubsampler-0.0.5/mdss/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     d.KullbackLeibler,
     d.Pearson,
 ]
 DISSIMILARITY_CLASS_MAPPING = dict(
     (dissimilarity.__name__, dissimilarity) for dissimilarity in DISSIMILARITY_CLASSES
 )
 
-# Function that creates the parser
+
 def parse_args(arg_list):
     parser = argparse.ArgumentParser(description="Subsampler tool")
     parser.add_argument(
         "--traj",
         dest="trajectory_file",
         required=False,
         help="the path to the trajectory file",
```

### Comparing `mdsubsampler-0.0.4/mdss/pca_property.py` & `mdsubsampler-0.0.5/mdss/pca_property.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/property.py` & `mdsubsampler-0.0.5/mdss/property.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/protein_data.py` & `mdsubsampler-0.0.5/mdss/protein_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,14 @@
         mda.Universe
             An instance of the MDAnalysis Universe representing the loaded trajectory.
         """
         trajectory_data = mda.Universe(
             topology_filename,
             trajectory_filename,
             permissive=False,
-            topology_format="PDB",
         )
         return trajectory_data
 
     def _select_CA_atoms(self):
         """
         Select C-alpha atoms from the first frame of the trajectory.
```

### Comparing `mdsubsampler-0.0.4/mdss/run.py` & `mdsubsampler-0.0.5/mdss/run.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/sampler.py` & `mdsubsampler-0.0.5/mdss/sampler.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/scenarios/scenario_1.ipynb` & `mdsubsampler-0.0.5/mdss/scenarios/scenario_1.ipynb`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/scenarios/scenario_1.py` & `mdsubsampler-0.0.5/mdss/scenarios/scenario_1.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/scenarios/scenario_2.ipynb` & `mdsubsampler-0.0.5/mdss/scenarios/scenario_2.ipynb`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/scenarios/scenario_2.py` & `mdsubsampler-0.0.5/mdss/scenarios/scenario_2.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/scenarios/scenario_3.ipynb` & `mdsubsampler-0.0.5/mdss/scenarios/scenario_3.ipynb`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/scenarios/scenario_3.py` & `mdsubsampler-0.0.5/mdss/scenarios/scenario_3.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/mdss/utilities.py` & `mdsubsampler-0.0.5/mdss/utilities.py`

 * *Files identical despite different names*

### Comparing `mdsubsampler-0.0.4/pyproject.toml` & `mdsubsampler-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdsubsampler"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Namir Oues <namir.oues@brunel.ac.uk>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "mdss" },
 ]
@@ -16,14 +16,15 @@
 MDAnalysis = "2.1.0"
 numpy = "^1.23.5"
 pandas = "^1.5.2"
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 psutil = "^5.9.4"
 scikit-learn = "^1.2.2"
+setuptools = "^69.0.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 ipykernel = "^6.23.1"
 jupyter = "^1.0.0"
 
 [build-system]
```

### Comparing `mdsubsampler-0.0.4/PKG-INFO` & `mdsubsampler-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdsubsampler
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 License: GPL-3.0-only
 Author: Namir Oues
 Author-email: namir.oues@brunel.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -17,14 +17,15 @@
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0)
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Description-Content-Type: text/markdown
 
 # MDSubSampler: Molecular Dynamics SubSampler
 
 [![PyPI version](https://badge.fury.io/py/mdsubsampler.svg)](https://badge.fury.io/py/mdsubsampler)
 
 MDSubSampler is a Python library and toolkit for a posteriori subsampling of multiple trajectory data for further analysis. This toolkit implements uniform, random, stratified sampling, bootstrapping and targeted sampling to preserve the original distribution of relevant geometrical properties.
```

