# Comparing `tmp/Pharokka-1.7.1.tar.gz` & `tmp/pharokka-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pharokka-1.7.1.tar", last modified: Wed Mar 13 00:34:27 2024, max compression
+gzip compressed data, was "pharokka-1.7.2.tar", last modified: Mon May 27 16:48:07 2024, max compression
```

## Comparing `Pharokka-1.7.1.tar` & `pharokka-1.7.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 00:34:27.685051 Pharokka-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-13 00:33:18.000000 Pharokka-1.7.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-13 00:33:18.000000 Pharokka-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35844 2024-03-13 00:34:27.681051 Pharokka-1.7.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 00:34:27.681051 Pharokka-1.7.1/Pharokka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35844 2024-03-13 00:34:27.000000 Pharokka-1.7.1/Pharokka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-13 00:34:27.000000 Pharokka-1.7.1/Pharokka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 00:34:27.000000 Pharokka-1.7.1/Pharokka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-13 00:34:27.000000 Pharokka-1.7.1/Pharokka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-13 00:34:27.000000 Pharokka-1.7.1/Pharokka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34368 2024-03-13 00:33:18.000000 Pharokka-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 00:34:27.681051 Pharokka-1.7.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/citation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/create_custom_hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/custom_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/external_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/input_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1285 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/install_databases.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17687 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/pharokka.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8546 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/pharokka_multiplotter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10560 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/pharokka_plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7087 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/pharokka_proteins.py
--rw-r--r--   0 runner    (1001) docker     (127)    43611 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    98888 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    34700 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)    21794 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/proteins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/run_pyrodigal_gv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 00:33:18.000000 Pharokka-1.7.1/bin/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 00:34:27.685051 Pharokka-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-13 00:33:18.000000 Pharokka-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 00:34:27.681051 Pharokka-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-13 00:33:18.000000 Pharokka-1.7.1/tests/test_external_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5426 2024-03-13 00:33:18.000000 Pharokka-1.7.1/tests/test_input_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14900 2024-03-13 00:33:18.000000 Pharokka-1.7.1/tests/test_overall.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3156 2024-03-13 00:33:18.000000 Pharokka-1.7.1/tests/test_proteins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:48:07.349389 pharokka-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-27 16:46:54.000000 pharokka-1.7.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 16:46:54.000000 pharokka-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    36378 2024-05-27 16:48:07.349389 pharokka-1.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:48:07.349389 pharokka-1.7.2/Pharokka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    36378 2024-05-27 16:48:07.000000 pharokka-1.7.2/Pharokka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 16:48:07.000000 pharokka-1.7.2/Pharokka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:48:07.000000 pharokka-1.7.2/Pharokka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 16:48:07.000000 pharokka-1.7.2/Pharokka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 16:48:07.000000 pharokka-1.7.2/Pharokka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34902 2024-05-27 16:46:54.000000 pharokka-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:48:07.349389 pharokka-1.7.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/citation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/create_custom_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/custom_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/external_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/input_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1285 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/install_databases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17687 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/pharokka.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8546 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/pharokka_multiplotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10560 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/pharokka_plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7087 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/pharokka_proteins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43611 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98888 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34698 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21794 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/proteins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/run_pyrodigal_gv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 16:46:54.000000 pharokka-1.7.2/bin/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:48:07.349389 pharokka-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-27 16:46:54.000000 pharokka-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:48:07.349389 pharokka-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-27 16:46:54.000000 pharokka-1.7.2/tests/test_external_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5426 2024-05-27 16:46:54.000000 pharokka-1.7.2/tests/test_input_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15262 2024-05-27 16:46:54.000000 pharokka-1.7.2/tests/test_overall.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3156 2024-05-27 16:46:54.000000 pharokka-1.7.2/tests/test_proteins.py
```

### Comparing `Pharokka-1.7.1/LICENSE` & `pharokka-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/PKG-INFO` & `pharokka-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pharokka
-Version: 1.7.1
+Version: 1.7.2
 Summary: Fast phage annotation tool
 Home-page: https://github.com/gbouras13/pharokka
 Author: George Bouras
 Author-email: george.bouras@adelaide.edu.au
 License: MIT License
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,15 +36,15 @@
 Requires-Dist: pytest-cov>=3.0.0
 Requires-Dist: alive-progress>=3.0.1
 Requires-Dist: requests>=2.25.1
 Requires-Dist: bcbio-gff>=0.7.0
 Requires-Dist: pyrodigal>=3.0.0
 Requires-Dist: pyrodigal_gv>=0.1.0
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold_and_phynteny.ipynb)
 
 [![Paper](https://img.shields.io/badge/paper-Bioinformatics-teal.svg?style=flat-square&maxAge=3600)](https://doi.org/10.1093/bioinformatics/btac776)
 [![CI](https://github.com/gbouras13/pharokka/actions/workflows/ci.yaml/badge.svg)](https://github.com/gbouras13/pharokka/actions/workflows/ci.yaml)
 [![BioConda Install](https://img.shields.io/conda/dn/bioconda/pharokka.svg?style=flag&label=BioConda%20install)](https://anaconda.org/bioconda/pharokka)
 [![codecov](https://codecov.io/gh/gbouras13/pharokka/branch/master/graph/badge.svg?token=4B1T2PGM9V)](https://codecov.io/gh/gbouras13/pharokka)
 
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/pharokka/badges/version.svg)](https://anaconda.org/bioconda/pharokka)
@@ -67,22 +67,26 @@
 
 If you are looking for rapid standardised annotation of bacterial genomes, please use [Bakta](https://github.com/oschwengers/bakta). [Prokka](https://github.com/tseemann/prokka), which inspired the creation and naming of `pharokka`, is another good option, but Bakta is [Prokka's worthy successor](https://twitter.com/torstenseemann/status/1565471892840259585).
 
 # phold
 
 If you like `pharokka`, you will probably love [phold](https://github.com/gbouras13/phold). `phold` uses structural homology to improve phage annotation. Benchmarking is ongoing but `phold` strongly outperforms `pharokka` in terms of annotation, particularly for less characterised phages such as those from metagenomic datasets.
 
-`pharokka` still has features `phold` lacks for now (identifying tRNA, tmRNA, CRISPR repeats, and INPHARED taxonomy search), so it it recommended to run `phold` after running `pharokka`. 
+`pharokka` still has features `phold` lacks for now (identifying tRNA, tmRNA, CRISPR repeats, and INPHARED taxonomy search), so it is recommended to run `phold` after running `pharokka`. 
 
 `phold` takes the Genbank output of Pharokka as input. Therefore, if you have already annotated your phage(s) with Pharokka, you can easily update the annotation with more functional predictions with [phold](https://github.com/gbouras13/phold).
 
 # Google Colab Notebooks
 
-If you don't want to install `pharokka` or `phold` locally, you can run `pharokka` and `phold`, or only `pharokka`, without any code using the Google Colab notebook [https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb)
+If you don't want to install `pharokka` or `phold` locally, you can run `pharokka` and `phold` (and [`phynteny`](https://github.com/susiegriggo/Phynteny)), or only `pharokka`, without any code using the [Google Colab notebook](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold_and_phynteny.ipynb).
 
+* [`phynteny`](https://github.com/susiegriggo/Phynteny) uses a long-short term memory model trained on phage synteny (the conserved gene order across phages) to assign hypothetical phage proteins to a PHROG category - it might help you add extra PHROG category annotations to hypothetical genes remaining after you run `phold`. 
+* Note: Phynteny will work only if your phage has fewer than 120 predicted proteins
+* You can still use this notebook to run `pharokka` and/or `phold` if your phage(s) are too big - just don't run the Phynteny step!
+  
 
 # Table of Contents
 
 - [pharokka](#pharokka)
   - [Fast Phage Annotation Tool](#fast-phage-annotation-tool)
 - [phold](#phold)
 - [Google Colab Notebooks](#google-colab-notebooks)
```

### Comparing `Pharokka-1.7.1/Pharokka.egg-info/PKG-INFO` & `pharokka-1.7.2/Pharokka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pharokka
-Version: 1.7.1
+Version: 1.7.2
 Summary: Fast phage annotation tool
 Home-page: https://github.com/gbouras13/pharokka
 Author: George Bouras
 Author-email: george.bouras@adelaide.edu.au
 License: MIT License
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,15 +36,15 @@
 Requires-Dist: pytest-cov>=3.0.0
 Requires-Dist: alive-progress>=3.0.1
 Requires-Dist: requests>=2.25.1
 Requires-Dist: bcbio-gff>=0.7.0
 Requires-Dist: pyrodigal>=3.0.0
 Requires-Dist: pyrodigal_gv>=0.1.0
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold_and_phynteny.ipynb)
 
 [![Paper](https://img.shields.io/badge/paper-Bioinformatics-teal.svg?style=flat-square&maxAge=3600)](https://doi.org/10.1093/bioinformatics/btac776)
 [![CI](https://github.com/gbouras13/pharokka/actions/workflows/ci.yaml/badge.svg)](https://github.com/gbouras13/pharokka/actions/workflows/ci.yaml)
 [![BioConda Install](https://img.shields.io/conda/dn/bioconda/pharokka.svg?style=flag&label=BioConda%20install)](https://anaconda.org/bioconda/pharokka)
 [![codecov](https://codecov.io/gh/gbouras13/pharokka/branch/master/graph/badge.svg?token=4B1T2PGM9V)](https://codecov.io/gh/gbouras13/pharokka)
 
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/pharokka/badges/version.svg)](https://anaconda.org/bioconda/pharokka)
@@ -67,22 +67,26 @@
 
 If you are looking for rapid standardised annotation of bacterial genomes, please use [Bakta](https://github.com/oschwengers/bakta). [Prokka](https://github.com/tseemann/prokka), which inspired the creation and naming of `pharokka`, is another good option, but Bakta is [Prokka's worthy successor](https://twitter.com/torstenseemann/status/1565471892840259585).
 
 # phold
 
 If you like `pharokka`, you will probably love [phold](https://github.com/gbouras13/phold). `phold` uses structural homology to improve phage annotation. Benchmarking is ongoing but `phold` strongly outperforms `pharokka` in terms of annotation, particularly for less characterised phages such as those from metagenomic datasets.
 
-`pharokka` still has features `phold` lacks for now (identifying tRNA, tmRNA, CRISPR repeats, and INPHARED taxonomy search), so it it recommended to run `phold` after running `pharokka`. 
+`pharokka` still has features `phold` lacks for now (identifying tRNA, tmRNA, CRISPR repeats, and INPHARED taxonomy search), so it is recommended to run `phold` after running `pharokka`. 
 
 `phold` takes the Genbank output of Pharokka as input. Therefore, if you have already annotated your phage(s) with Pharokka, you can easily update the annotation with more functional predictions with [phold](https://github.com/gbouras13/phold).
 
 # Google Colab Notebooks
 
-If you don't want to install `pharokka` or `phold` locally, you can run `pharokka` and `phold`, or only `pharokka`, without any code using the Google Colab notebook [https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb)
+If you don't want to install `pharokka` or `phold` locally, you can run `pharokka` and `phold` (and [`phynteny`](https://github.com/susiegriggo/Phynteny)), or only `pharokka`, without any code using the [Google Colab notebook](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold_and_phynteny.ipynb).
 
+* [`phynteny`](https://github.com/susiegriggo/Phynteny) uses a long-short term memory model trained on phage synteny (the conserved gene order across phages) to assign hypothetical phage proteins to a PHROG category - it might help you add extra PHROG category annotations to hypothetical genes remaining after you run `phold`. 
+* Note: Phynteny will work only if your phage has fewer than 120 predicted proteins
+* You can still use this notebook to run `pharokka` and/or `phold` if your phage(s) are too big - just don't run the Phynteny step!
+  
 
 # Table of Contents
 
 - [pharokka](#pharokka)
   - [Fast Phage Annotation Tool](#fast-phage-annotation-tool)
 - [phold](#phold)
 - [Google Colab Notebooks](#google-colab-notebooks)
```

### Comparing `Pharokka-1.7.1/Pharokka.egg-info/SOURCES.txt` & `pharokka-1.7.2/Pharokka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/README.md` & `pharokka-1.7.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold_and_phynteny.ipynb)
 
 [![Paper](https://img.shields.io/badge/paper-Bioinformatics-teal.svg?style=flat-square&maxAge=3600)](https://doi.org/10.1093/bioinformatics/btac776)
 [![CI](https://github.com/gbouras13/pharokka/actions/workflows/ci.yaml/badge.svg)](https://github.com/gbouras13/pharokka/actions/workflows/ci.yaml)
 [![BioConda Install](https://img.shields.io/conda/dn/bioconda/pharokka.svg?style=flag&label=BioConda%20install)](https://anaconda.org/bioconda/pharokka)
 [![codecov](https://codecov.io/gh/gbouras13/pharokka/branch/master/graph/badge.svg?token=4B1T2PGM9V)](https://codecov.io/gh/gbouras13/pharokka)
 
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/pharokka/badges/version.svg)](https://anaconda.org/bioconda/pharokka)
@@ -25,22 +25,26 @@
 
 If you are looking for rapid standardised annotation of bacterial genomes, please use [Bakta](https://github.com/oschwengers/bakta). [Prokka](https://github.com/tseemann/prokka), which inspired the creation and naming of `pharokka`, is another good option, but Bakta is [Prokka's worthy successor](https://twitter.com/torstenseemann/status/1565471892840259585).
 
 # phold
 
 If you like `pharokka`, you will probably love [phold](https://github.com/gbouras13/phold). `phold` uses structural homology to improve phage annotation. Benchmarking is ongoing but `phold` strongly outperforms `pharokka` in terms of annotation, particularly for less characterised phages such as those from metagenomic datasets.
 
-`pharokka` still has features `phold` lacks for now (identifying tRNA, tmRNA, CRISPR repeats, and INPHARED taxonomy search), so it it recommended to run `phold` after running `pharokka`. 
+`pharokka` still has features `phold` lacks for now (identifying tRNA, tmRNA, CRISPR repeats, and INPHARED taxonomy search), so it is recommended to run `phold` after running `pharokka`. 
 
 `phold` takes the Genbank output of Pharokka as input. Therefore, if you have already annotated your phage(s) with Pharokka, you can easily update the annotation with more functional predictions with [phold](https://github.com/gbouras13/phold).
 
 # Google Colab Notebooks
 
-If you don't want to install `pharokka` or `phold` locally, you can run `pharokka` and `phold`, or only `pharokka`, without any code using the Google Colab notebook [https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold.ipynb)
+If you don't want to install `pharokka` or `phold` locally, you can run `pharokka` and `phold` (and [`phynteny`](https://github.com/susiegriggo/Phynteny)), or only `pharokka`, without any code using the [Google Colab notebook](https://colab.research.google.com/github/gbouras13/pharokka/blob/master/run_pharokka_and_phold_and_phynteny.ipynb).
 
+* [`phynteny`](https://github.com/susiegriggo/Phynteny) uses a long-short term memory model trained on phage synteny (the conserved gene order across phages) to assign hypothetical phage proteins to a PHROG category - it might help you add extra PHROG category annotations to hypothetical genes remaining after you run `phold`. 
+* Note: Phynteny will work only if your phage has fewer than 120 predicted proteins
+* You can still use this notebook to run `pharokka` and/or `phold` if your phage(s) are too big - just don't run the Phynteny step!
+  
 
 # Table of Contents
 
 - [pharokka](#pharokka)
   - [Fast Phage Annotation Tool](#fast-phage-annotation-tool)
 - [phold](#phold)
 - [Google Colab Notebooks](#google-colab-notebooks)
```

### Comparing `Pharokka-1.7.1/bin/create_custom_hmm.py` & `pharokka-1.7.2/bin/create_custom_hmm.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/custom_db.py` & `pharokka-1.7.2/bin/custom_db.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/databases.py` & `pharokka-1.7.2/bin/databases.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/external_tools.py` & `pharokka-1.7.2/bin/external_tools.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/hmm.py` & `pharokka-1.7.2/bin/hmm.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/input_commands.py` & `pharokka-1.7.2/bin/input_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,20 @@
     header_set = set()
 
     # Iterate through the FASTA file and check for duplicate headers
     for record in SeqIO.parse(fasta_file, "fasta"):
         header = record.description
         if header in header_set:
             logger.error(
-                f"Duplicate header found: {header}"
+                f"Duplicate contig header found: {header}"
             )  # errors if duplicate header found
+        if "#" in header:
+            logger.error(
+                f"# character found in contig: {header} - please remove all '#' from your contig headers"
+            )  # errors if duplicate header found   
         else:
             header_set.add(header)
     # if it finished it will be fine
 
 
 def validate_gene_predictor(gene_predictor, genbank_flag):
     if gene_predictor == "phanotate":
```

### Comparing `Pharokka-1.7.1/bin/install_databases.py` & `pharokka-1.7.2/bin/install_databases.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/pharokka.py` & `pharokka-1.7.2/bin/pharokka.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/pharokka_multiplotter.py` & `pharokka-1.7.2/bin/pharokka_multiplotter.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/pharokka_plotter.py` & `pharokka-1.7.2/bin/pharokka_plotter.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/pharokka_proteins.py` & `pharokka-1.7.2/bin/pharokka_proteins.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/plot.py` & `pharokka-1.7.2/bin/plot.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/post_processing.py` & `pharokka-1.7.2/bin/post_processing.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/processes.py` & `pharokka-1.7.2/bin/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,17 +373,17 @@
     }
 
     phan_df = pd.read_csv(
         phan_file,
         delimiter="\t",
         index_col=False,
         names=col_list,
-        skiprows=2,
+        skiprows=2, # to skip the headers
         dtype=dtype_dict,
-        comment="#",  # to skip the headers
+        comment="#"
     )
     # get rid of the headers and reset the index
     phan_df = phan_df[phan_df["start"] != "#id:"]
     phan_df = phan_df[phan_df["start"] != "#START"].reset_index(drop=True)
     phan_df["gene"] = (
         phan_df["contig"].astype(str)
         + phan_df.index.astype(str)
```

### Comparing `Pharokka-1.7.1/bin/proteins.py` & `pharokka-1.7.2/bin/proteins.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/run_pyrodigal_gv.py` & `pharokka-1.7.2/bin/run_pyrodigal_gv.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/bin/util.py` & `pharokka-1.7.2/bin/util.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/setup.py` & `pharokka-1.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # read long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Pharokka",
-    version="1.7.1",
+    version="1.7.2",
     author="George Bouras",
     author_email="george.bouras@adelaide.edu.au",
     description="Fast phage annotation tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gbouras13/pharokka",
     scripts=[
```

### Comparing `Pharokka-1.7.1/tests/test_external_commands.py` & `pharokka-1.7.2/tests/test_external_commands.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/tests/test_input_commands.py` & `pharokka-1.7.2/tests/test_input_commands.py`

 * *Files identical despite different names*

### Comparing `Pharokka-1.7.1/tests/test_overall.py` & `pharokka-1.7.2/tests/test_overall.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
 def test_overall(tmp_dir):
     """test pharokka overall"""
     input_fasta: Path = f"{standard_data}/SAOMS1.fasta"
     cmd = f"pharokka.py -i {input_fasta} -d {database_dir} -o {tmp_dir} -t {threads} -f"
     exec_command(cmd)
 
-
 def test_overall_mash_distance(tmp_dir):
     """test pharokka overall with stricter mash distance"""
     input_fasta: Path = f"{standard_data}/SAOMS1.fasta"
     cmd = f"pharokka.py -i {input_fasta} -d {database_dir} -o {tmp_dir} -t {threads} -f --mash_distance 0.05"
     exec_command(cmd)
 
 
@@ -285,14 +284,21 @@
     def test_dupe_header(self):
         """tests that pharokka exits if a duplicate header is passed"""
         with self.assertRaises(RuntimeError):
             input_fasta: Path = f"{standard_data}/dupe_header.fasta"
             cmd = f"pharokka.py -i {input_fasta} -d {database_dir} -o {temp_dir} -t 1 -f -m"
             exec_command(cmd)
 
+    def test_overall_hash_header(self):
+        """test pharokka overall with # in header - should error out"""
+        with self.assertRaises(RuntimeError):
+            input_fasta: Path = f"{standard_data}/SAOMS1_hash_header.fasta"
+            cmd = f"pharokka.py -i {input_fasta} -d {database_dir} -o {temp_dir} -t {threads} -f"
+            exec_command(cmd)
+
     def test_meta_with_single_contig(self):
         """tests that pharokka exits if single contig is passed to meta"""
         with self.assertRaises(RuntimeError):
             input_fasta: Path = f"{standard_data}/SAOMS1.fasta"
             cmd = f"pharokka.py -i {input_fasta} -d {database_dir} -o {temp_dir} -t 1 -f -m"
             exec_command(cmd)
```

### Comparing `Pharokka-1.7.1/tests/test_proteins.py` & `pharokka-1.7.2/tests/test_proteins.py`

 * *Files identical despite different names*

