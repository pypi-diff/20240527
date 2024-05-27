# Comparing `tmp/climetlab_maelstrom_downscaling-0.3.1.tar.gz` & `tmp/climetlab_maelstrom_downscaling-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climetlab_maelstrom_downscaling-0.3.1.tar", last modified: Thu Oct 19 16:02:37 2023, max compression
+gzip compressed data, was "/home/michael/climetlab-maelstrom-downscaling-0.4.0/dist/.tmp-0u9_mgg0/climetlab_maelstrom_downscaling-0.4.0.tar", last modified: Mon May 27 12:16:31 2024, max compression
```

## Comparing `climetlab_maelstrom_downscaling-0.3.1.tar` & `climetlab_maelstrom_downscaling-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxr-xr-x   0 michael   (1000) users      (100)        0 2023-10-19 16:02:37.767707 climetlab_maelstrom_downscaling-0.3.1/
--rwxr-x---   0 michael   (1000) users      (100)     1491 2022-03-30 09:16:32.000000 climetlab_maelstrom_downscaling-0.3.1/.gitignore
--rwxr-x---   0 michael   (1000) users      (100)    11357 2023-10-19 14:08:27.000000 climetlab_maelstrom_downscaling-0.3.1/LICENSE
--rw-r--r--   0 michael   (1000) users      (100)     9107 2023-10-19 16:02:37.767707 climetlab_maelstrom_downscaling-0.3.1/PKG-INFO
--rwxr-x---   0 michael   (1000) users      (100)     8107 2023-10-19 14:08:19.000000 climetlab_maelstrom_downscaling-0.3.1/README.md
-drwxr-xr-x   0 michael   (1000) users      (100)        0 2023-10-19 16:02:37.727707 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling/
--rw-r--r--   0 michael   (1000) users      (100)       22 2023-10-19 14:14:46.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling/__init__.py
--rw-r--r--   0 michael   (1000) users      (100)     5943 2023-10-19 14:18:51.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling/downscaling.py
--rw-r--r--   0 michael   (1000) users      (100)     5230 2023-10-19 15:36:20.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling/downscaling_tier2.py
-drwxr-xr-x   0 michael   (1000) users      (100)        0 2023-10-19 16:02:37.727707 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/
--rw-r--r--   0 michael   (1000) users      (100)     9107 2023-10-19 16:02:37.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/PKG-INFO
--rwxr-x---   0 michael   (1000) users      (100)      697 2023-10-19 16:02:37.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/SOURCES.txt
--rwxr-x---   0 michael   (1000) users      (100)        1 2023-10-19 16:02:37.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/dependency_links.txt
--rwxr-x---   0 michael   (1000) users      (100)      199 2023-10-19 16:02:37.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/entry_points.txt
--rwxr-x---   0 michael   (1000) users      (100)       17 2023-10-19 16:02:37.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/requires.txt
--rwxr-x---   0 michael   (1000) users      (100)       32 2023-10-19 16:02:37.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/top_level.txt
--rwxr-x---   0 michael   (1000) users      (100)        1 2023-10-19 15:17:21.000000 climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/zip-safe
-drwxr-xr-x   0 michael   (1000) users      (100)        0 2023-10-19 16:02:37.727707 climetlab_maelstrom_downscaling-0.3.1/notebooks/
--rwxr--r--   0 michael   (1000) users      (100)   117465 2023-10-19 15:47:41.000000 climetlab_maelstrom_downscaling-0.3.1/notebooks/demo_downscaling_dataset.ipynb
--rwxr-x---   0 michael   (1000) users      (100)       12 2023-10-19 14:07:57.000000 climetlab_maelstrom_downscaling-0.3.1/requirements.txt
--rw-r--r--   0 michael   (1000) users      (100)       38 2023-10-19 16:02:37.771707 climetlab_maelstrom_downscaling-0.3.1/setup.cfg
--rw-r--r--   0 michael   (1000) users      (100)     2490 2023-10-19 14:12:47.000000 climetlab_maelstrom_downscaling-0.3.1/setup.py
-drwxr-xr-x   0 michael   (1000) users      (100)        0 2023-10-19 16:02:37.767707 climetlab_maelstrom_downscaling-0.3.1/tests/
--rwxr-x---   0 michael   (1000) users      (100)      618 2023-10-19 15:18:55.000000 climetlab_maelstrom_downscaling-0.3.1/tests/test_downscaling_dataset.py
--rwxr-x---   0 michael   (1000) users      (100)     1573 2023-10-19 15:18:55.000000 climetlab_maelstrom_downscaling-0.3.1/tests/test_notebooks.py
--rw-r--r--   0 michael   (1000) users      (100)      190 2023-10-19 14:08:07.000000 climetlab_maelstrom_downscaling-0.3.1/tox.ini
+drwxr-xr-x   0 michael   (1000) users      (100)        0 2024-05-27 12:16:31.097115 climetlab_maelstrom_downscaling-0.4.0/
+-rwxr-x---   0 michael   (1000) users      (100)    11357 2024-05-14 11:11:12.000000 climetlab_maelstrom_downscaling-0.4.0/LICENSE
+-rw-r--r--   0 michael   (1000) users      (100)    10067 2024-05-27 12:16:31.097115 climetlab_maelstrom_downscaling-0.4.0/PKG-INFO
+-rwxr-x---   0 michael   (1000) users      (100)     9015 2024-05-26 19:40:48.000000 climetlab_maelstrom_downscaling-0.4.0/README.md
+drwxr-xr-x   0 michael   (1000) users      (100)        0 2024-05-27 12:16:31.093114 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling/
+-rwxr-x---   0 michael   (1000) users      (100)       22 2024-05-14 11:11:12.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling/__init__.py
+-rwxrwx---   0 michael   (1000) users      (100)     6761 2024-05-26 19:43:22.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling/downscaling_tier1.py
+-rwxr-x---   0 michael   (1000) users      (100)     6346 2024-05-26 19:46:59.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling/downscaling_tier2.py
+drwxr-xr-x   0 michael   (1000) users      (100)        0 2024-05-27 12:16:31.093114 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/
+-rw-r--r--   0 michael   (1000) users      (100)    10067 2024-05-27 12:16:31.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) users      (100)      616 2024-05-27 12:16:31.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) users      (100)        1 2024-05-27 12:16:31.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) users      (100)      205 2024-05-27 12:16:31.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) users      (100)       17 2024-05-27 12:16:31.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) users      (100)       32 2024-05-27 12:16:31.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) users      (100)        1 2024-05-15 06:10:59.000000 climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) users      (100)       38 2024-05-27 12:16:31.097115 climetlab_maelstrom_downscaling-0.4.0/setup.cfg
+-rwxr-x---   0 michael   (1000) users      (100)     2547 2024-05-15 06:04:50.000000 climetlab_maelstrom_downscaling-0.4.0/setup.py
+drwxr-xr-x   0 michael   (1000) users      (100)        0 2024-05-27 12:16:31.093114 climetlab_maelstrom_downscaling-0.4.0/tests/
+-rwxr-x---   0 michael   (1000) users      (100)      618 2024-05-14 11:11:12.000000 climetlab_maelstrom_downscaling-0.4.0/tests/test_downscaling_dataset.py
+-rwxr-x---   0 michael   (1000) users      (100)     1573 2024-05-14 11:11:12.000000 climetlab_maelstrom_downscaling-0.4.0/tests/test_notebooks.py
```

### Comparing `climetlab_maelstrom_downscaling-0.3.1/LICENSE` & `climetlab_maelstrom_downscaling-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climetlab_maelstrom_downscaling-0.3.1/PKG-INFO` & `climetlab_maelstrom_downscaling-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: climetlab_maelstrom_downscaling
-Version: 0.3.1
+Version: 0.4.0
 Summary: A dataset plugin for climetlab for the dataset maelstrom-downscaling.
 Home-page: https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-ap5/
 Author: Michael Langguth, Bing Gong
 Author-email: m.langguth@fz-juelich.de
 License: Apache License Version 2.0
 Keywords: meteorology
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: climetlab>=0.9.0
 
@@ -53,19 +54,29 @@
 ```
 By changing the `dataset`-argument to `"validation"` and `"testing"`, the validation and testing data can be retrieved.
 Furthermore, an augmented variant of the dataset is available which can be downloaded by adding 
 a `_augmented`-suffix to the `dataset`-arguments.
 
 ### Download the Tier-2 data
 The Tier-2 dataset can be downloaded by replacing the value of the first argument of `cml.load_dataset`. 
-The following code-snippet exemplary downloads the training dataset (about 45 GB!):
+The following code-snippet exemplary downloads the training dataset:
 ```commandline
 ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
 ```
-Note that no augmented variant of the Tier-2 dataset is provided.
+Note that the training dataset comprises about 250 GB of data and thus downloading can require several minutes or hours depending on the Internet connection.
+Due to the comprehensive size of the dataset, no augmented variant is provided.
+
+### Saving the data on disk
+By default, `CliMetLab` only caches the data. To save the data persistently onto disk/in the user's filesystem,
+`persist=True` must be added, when running the `to_xarray`-method. Furthermore, a directory-path under which the file(-s) will be saved must be parsed via `data_dir`.
+The following command exemplifies saving the large-scale Tier-2 dataset.
+```
+ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
+ds.to_xarray(persist=True, data_dir="/my/local/path")
+```
 
 ### Tutorial for the Tier-1 dataset
 
 A tutorial is available in form of a <a href="https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-ap5/browse/notebooks/demo_downscaling_dataset.ipynb">Jupyter Notebook</a>.
 In this Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net for downscaling adapted from [1].
 
 ## Dataset description
@@ -107,15 +118,16 @@
 are downscaled onto the high-resolved grid of the COSMO REA6 dataset [4]. 
 Since data from two different models are now used, where COSMO REA6 provides added value
 over complex terrain due to its higher spatial resolution, the downscaling task is now twofold:
 The data has to be super-resolved and bias-corrected.
 
 Here, we still target the 2m temperature as with the Tier-1 dataset, but include more predictor variables:
 - 2m temperature
-- 850 hPa- and 925 hPa temperature
+- temperature from model levels 137, 135, 131, 127, 122 and 115
+- surface pressure
 - surface latent and sensible heat fluxes
 - 10m horizontal wind (u,v)
 - boundary layer height
 
 The surface topography from the ERA5 and the COSMO REA6 datasets are also included as static predictor variables.
 
 As a necessary prerequisite, the underlying grid of both reanalysis datasets needed to be merged.
@@ -123,17 +135,19 @@
 With a grid spacing of 0.275° in rotated coordinates, the spatial resolution of the ERA 5 data is 
 five times coarser than the target data, the COSMO REA6-data (dx=0.055°). 
 Similar to the Tier-1 dataset, the ERA5-data is bi-linearly interpolated onto the high resolved target 
 grid to serve as input for the neural networks for downscaling.
 
 Currently, the target domain of the Tier-2 dataset comprises 120x96 grid points (with dx=0.055°) 
 covering large parts of Central Europe to include complex terrain of the Alps and the German low mountain range.
-Hourly data is provided for the years between 2006 and 2018. By default, the years 2006-2016 constitute the 
+Hourly data is provided for the years between 1995 and 2018. By default, the years 1995-2016 constitute the 
 training dataset, while 2017 and 2018 are used for validation and testing, respectively.
 
+This dataset constitutes the final dataset used in Application 5 of the MAELSTROM project as described in this [report](https://www.maelstrom-eurohpc.eu/content/docs/uploads/doc50.pdf).
+
 ## References
 **[1]** Sha, Yingkai, et al. "Deep-learning-based gridded downscaling of surface meteorological variables in complex
 terrain. Part I: Daily maximum and minimum 2-m temperature."
 Journal of Applied Meteorology and Climatology 59.12 (2020): 2057-2073. 
 <a href="https://doi.org/10.1175/JAMC-D-20-0057.1"> DOI</a>.<br>
 **[2]** Leinonen, Jussi et al., "Stochastic Super-Resolution for Downscaling Time-Evolving Atmospheric Fields
 With a Generative Adversarial Network." IEEE Transactions on Geoscience and Remote Sensing 59.9 (2021): 7211-7223
```

#### html2text {}

```diff
@@ -1,47 +1,56 @@
-Metadata-Version: 2.1 Name: climetlab_maelstrom_downscaling Version: 0.3.1
+Metadata-Version: 2.1 Name: climetlab_maelstrom_downscaling Version: 0.4.0
 Summary: A dataset plugin for climetlab for the dataset maelstrom-downscaling.
 Home-page: https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-
 ap5/ Author: Michael Langguth, Bing Gong Author-email: m.langguth@fz-juelich.de
 License: Apache License Version 2.0 Keywords: meteorology Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-climetlab>=0.9.0 ï»¿# maelstrom-downscaling-ap5 A _C_l_i_M_e_t_L_a_b_ dataset plugin for
-the datasets used in application of the _M_A_E_L_S_T_R_O_M_ _p_r_o_j_e_c_t. Features -------
-- This README provides a brief description of the provided datasets for
-statistical downscaling of meteorological fields, the target of _a_p_p_l_i_c_a_t_i_o_n_ _5_ 
-_(_A_P_5_)_ _i_n_ _s_c_o_p_e_ _o_f_ _M_A_E_L_S_T_R_O_M. Two different datasets, named Tier-1 and Tier-2 in
-the following, can be downloaded from the _A_W_S_ _s_3_-_b_u_c_k_e_t, provided by ECMWF,
-with this `CliMetLab` plugin. Both datasets are distributed under the _A_p_a_c_h_e
-_L_i_c_e_n_s_e_,_ _v_e_r_s_i_o_n_ _2_._0_ and thus are open-access. ## Using climetlab to access the
-data The `CliMetLab` python package allows easy access to the data with a few
-lines of code.
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: climetlab>=0.9.0 ï»¿# maelstrom-
+downscaling-ap5 A _C_l_i_M_e_t_L_a_b_ dataset plugin for the datasets used in application
+of the _M_A_E_L_S_T_R_O_M_ _p_r_o_j_e_c_t. Features -------- This README provides a brief
+description of the provided datasets for statistical downscaling of
+meteorological fields, the target of _a_p_p_l_i_c_a_t_i_o_n_ _5_ _(_A_P_5_)_ _i_n_ _s_c_o_p_e_ _o_f_ _M_A_E_L_S_T_R_O_M.
+Two different datasets, named Tier-1 and Tier-2 in the following, can be
+downloaded from the _A_W_S_ _s_3_-_b_u_c_k_e_t, provided by ECMWF, with this `CliMetLab`
+plugin. Both datasets are distributed under the _A_p_a_c_h_e_ _L_i_c_e_n_s_e_,_ _v_e_r_s_i_o_n_ _2_._0_ and
+thus are open-access. ## Using climetlab to access the data The `CliMetLab`
+python package allows easy access to the data with a few lines of code.
 The following examples demonstrate how to obtain the two provided datasets. A
 more detailed description of both datasets is provided afterwards. ### Download
 the Tier-1 data The training data of the Tier-1 dataset can be downloaded as
 follows: ``` !pip install climetlab climetlab_maelstrom_downscaling import
 climetlab as cml ds = cml.load_dataset("maelstrom-downscaling",
 dataset="training") ds.to_xarray() ``` By changing the `dataset`-argument to
 `"validation"` and `"testing"`, the validation and testing data can be
 retrieved. Furthermore, an augmented variant of the dataset is available which
 can be downloaded by adding a `_augmented`-suffix to the `dataset`-arguments.
 ### Download the Tier-2 data The Tier-2 dataset can be downloaded by replacing
 the value of the first argument of `cml.load_dataset`. The following code-
-snippet exemplary downloads the training dataset (about 45 GB!): ```commandline
-ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training") ```
-Note that no augmented variant of the Tier-2 dataset is provided. ### Tutorial
-for the Tier-1 dataset A tutorial is available in form of a _J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k.
-In this Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net
-for downscaling adapted from [1]. ## Dataset description Within the _M_A_E_L_S_T_R_O_M
+snippet exemplary downloads the training dataset: ```commandline ds =
+cml.load_dataset("maelstrom-downscaling-tier2", dataset="training") ``` Note
+that the training dataset comprises about 250 GB of data and thus downloading
+can require several minutes or hours depending on the Internet connection. Due
+to the comprehensive size of the dataset, no augmented variant is provided. ###
+Saving the data on disk By default, `CliMetLab` only caches the data. To save
+the data persistently onto disk/in the user's filesystem, `persist=True` must
+be added, when running the `to_xarray`-method. Furthermore, a directory-path
+under which the file(-s) will be saved must be parsed via `data_dir`. The
+following command exemplifies saving the large-scale Tier-2 dataset. ``` ds =
+cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
+ds.to_xarray(persist=True, data_dir="/my/local/path") ``` ### Tutorial for the
+Tier-1 dataset A tutorial is available in form of a _J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k. In this
+Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net for
+downscaling adapted from [1]. ## Dataset description Within the _M_A_E_L_S_T_R_O_M
 project, two different datasets are provided that are used to construct
 statistical downscaling tasks with deep neural networks. The first dataset, the
 Tier-1 dataset, serves as the starting point and provides the data for a pure
 downscaling task similar to the super-resolution task in computer vision.
 The Tier-2 dataset provides the data for a real downscaling task in meteorology
 where the super-resolution task is complemented by bias correction.
 Both datasets will be described in more detail in the following. ### The Tier-
@@ -78,31 +87,34 @@
 2 dataset provides data for a real downscaling task where coarse-grained ERA5
 reanalysis data [3] are downscaled onto the high-resolved grid of the COSMO
 REA6 dataset [4]. Since data from two different models are now used, where
 COSMO REA6 provides added value over complex terrain due to its higher spatial
 resolution, the downscaling task is now twofold: The data has to be super-
 resolved and bias-corrected. Here, we still target the 2m temperature as with
 the Tier-1 dataset, but include more predictor variables: - 2m temperature -
-850 hPa- and 925 hPa temperature - surface latent and sensible heat fluxes -
-10m horizontal wind (u,v) - boundary layer height The surface topography from
-the ERA5 and the COSMO REA6 datasets are also included as static predictor
-variables. As a necessary prerequisite, the underlying grid of both reanalysis
-datasets needed to be merged. Here, we have remapped the ERA5 data onto the
-rotated pole grid deployed by the COSMO model [5]. With a grid spacing of
-0.275Â° in rotated coordinates, the spatial resolution of the ERA 5 data is
-five times coarser than the target data, the COSMO REA6-data (dx=0.055Â°).
-Similar to the Tier-1 dataset, the ERA5-data is bi-linearly interpolated onto
-the high resolved target grid to serve as input for the neural networks for
-downscaling. Currently, the target domain of the Tier-2 dataset comprises
-120x96 grid points (with dx=0.055Â°) covering large parts of Central Europe to
-include complex terrain of the Alps and the German low mountain range. Hourly
-data is provided for the years between 2006 and 2018. By default, the years
-2006-2016 constitute the training dataset, while 2017 and 2018 are used for
-validation and testing, respectively. ## References **[1]** Sha, Yingkai, et
-al. "Deep-learning-based gridded downscaling of surface meteorological
+temperature from model levels 137, 135, 131, 127, 122 and 115 - surface
+pressure - surface latent and sensible heat fluxes - 10m horizontal wind (u,v)
+- boundary layer height The surface topography from the ERA5 and the COSMO REA6
+datasets are also included as static predictor variables. As a necessary
+prerequisite, the underlying grid of both reanalysis datasets needed to be
+merged. Here, we have remapped the ERA5 data onto the rotated pole grid
+deployed by the COSMO model [5]. With a grid spacing of 0.275Â° in rotated
+coordinates, the spatial resolution of the ERA 5 data is five times coarser
+than the target data, the COSMO REA6-data (dx=0.055Â°). Similar to the Tier-
+1 dataset, the ERA5-data is bi-linearly interpolated onto the high resolved
+target grid to serve as input for the neural networks for downscaling.
+Currently, the target domain of the Tier-2 dataset comprises 120x96 grid points
+(with dx=0.055Â°) covering large parts of Central Europe to include complex
+terrain of the Alps and the German low mountain range. Hourly data is provided
+for the years between 1995 and 2018. By default, the years 1995-2016 constitute
+the training dataset, while 2017 and 2018 are used for validation and testing,
+respectively. This dataset constitutes the final dataset used in Application 5
+of the MAELSTROM project as described in this [report](https://www.maelstrom-
+eurohpc.eu/content/docs/uploads/doc50.pdf). ## References **[1]** Sha, Yingkai,
+et al. "Deep-learning-based gridded downscaling of surface meteorological
 variables in complex terrain. Part I: Daily maximum and minimum 2-
 m temperature." Journal of Applied Meteorology and Climatology 59.12 (2020):
 2057-2073. _D_O_I.
 **[2]** Leinonen, Jussi et al., "Stochastic Super-Resolution for Downscaling
 Time-Evolving Atmospheric Fields With a Generative Adversarial Network." IEEE
 Transactions on Geoscience and Remote Sensing 59.9 (2021): 7211-7223 _D_O_I.
 **[3]** Hersbach, Hans, et al. "The ERA5 global reanalysis." Quarterly Journal
```

### Comparing `climetlab_maelstrom_downscaling-0.3.1/README.md` & `climetlab_maelstrom_downscaling-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,19 +30,29 @@
 ```
 By changing the `dataset`-argument to `"validation"` and `"testing"`, the validation and testing data can be retrieved.
 Furthermore, an augmented variant of the dataset is available which can be downloaded by adding 
 a `_augmented`-suffix to the `dataset`-arguments.
 
 ### Download the Tier-2 data
 The Tier-2 dataset can be downloaded by replacing the value of the first argument of `cml.load_dataset`. 
-The following code-snippet exemplary downloads the training dataset (about 45 GB!):
+The following code-snippet exemplary downloads the training dataset:
 ```commandline
 ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
 ```
-Note that no augmented variant of the Tier-2 dataset is provided.
+Note that the training dataset comprises about 250 GB of data and thus downloading can require several minutes or hours depending on the Internet connection.
+Due to the comprehensive size of the dataset, no augmented variant is provided.
+
+### Saving the data on disk
+By default, `CliMetLab` only caches the data. To save the data persistently onto disk/in the user's filesystem,
+`persist=True` must be added, when running the `to_xarray`-method. Furthermore, a directory-path under which the file(-s) will be saved must be parsed via `data_dir`.
+The following command exemplifies saving the large-scale Tier-2 dataset.
+```
+ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
+ds.to_xarray(persist=True, data_dir="/my/local/path")
+```
 
 ### Tutorial for the Tier-1 dataset
 
 A tutorial is available in form of a <a href="https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-ap5/browse/notebooks/demo_downscaling_dataset.ipynb">Jupyter Notebook</a>.
 In this Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net for downscaling adapted from [1].
 
 ## Dataset description
@@ -84,15 +94,16 @@
 are downscaled onto the high-resolved grid of the COSMO REA6 dataset [4]. 
 Since data from two different models are now used, where COSMO REA6 provides added value
 over complex terrain due to its higher spatial resolution, the downscaling task is now twofold:
 The data has to be super-resolved and bias-corrected.
 
 Here, we still target the 2m temperature as with the Tier-1 dataset, but include more predictor variables:
 - 2m temperature
-- 850 hPa- and 925 hPa temperature
+- temperature from model levels 137, 135, 131, 127, 122 and 115
+- surface pressure
 - surface latent and sensible heat fluxes
 - 10m horizontal wind (u,v)
 - boundary layer height
 
 The surface topography from the ERA5 and the COSMO REA6 datasets are also included as static predictor variables.
 
 As a necessary prerequisite, the underlying grid of both reanalysis datasets needed to be merged.
@@ -100,17 +111,19 @@
 With a grid spacing of 0.275° in rotated coordinates, the spatial resolution of the ERA 5 data is 
 five times coarser than the target data, the COSMO REA6-data (dx=0.055°). 
 Similar to the Tier-1 dataset, the ERA5-data is bi-linearly interpolated onto the high resolved target 
 grid to serve as input for the neural networks for downscaling.
 
 Currently, the target domain of the Tier-2 dataset comprises 120x96 grid points (with dx=0.055°) 
 covering large parts of Central Europe to include complex terrain of the Alps and the German low mountain range.
-Hourly data is provided for the years between 2006 and 2018. By default, the years 2006-2016 constitute the 
+Hourly data is provided for the years between 1995 and 2018. By default, the years 1995-2016 constitute the 
 training dataset, while 2017 and 2018 are used for validation and testing, respectively.
 
+This dataset constitutes the final dataset used in Application 5 of the MAELSTROM project as described in this [report](https://www.maelstrom-eurohpc.eu/content/docs/uploads/doc50.pdf).
+
 ## References
 **[1]** Sha, Yingkai, et al. "Deep-learning-based gridded downscaling of surface meteorological variables in complex
 terrain. Part I: Daily maximum and minimum 2-m temperature."
 Journal of Applied Meteorology and Climatology 59.12 (2020): 2057-2073. 
 <a href="https://doi.org/10.1175/JAMC-D-20-0057.1"> DOI</a>.<br>
 **[2]** Leinonen, Jussi et al., "Stochastic Super-Resolution for Downscaling Time-Evolving Atmospheric Fields
 With a Generative Adversarial Network." IEEE Transactions on Geoscience and Remote Sensing 59.9 (2021): 7211-7223
```

#### html2text {}

```diff
@@ -14,20 +14,29 @@
 climetlab as cml ds = cml.load_dataset("maelstrom-downscaling",
 dataset="training") ds.to_xarray() ``` By changing the `dataset`-argument to
 `"validation"` and `"testing"`, the validation and testing data can be
 retrieved. Furthermore, an augmented variant of the dataset is available which
 can be downloaded by adding a `_augmented`-suffix to the `dataset`-arguments.
 ### Download the Tier-2 data The Tier-2 dataset can be downloaded by replacing
 the value of the first argument of `cml.load_dataset`. The following code-
-snippet exemplary downloads the training dataset (about 45 GB!): ```commandline
-ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training") ```
-Note that no augmented variant of the Tier-2 dataset is provided. ### Tutorial
-for the Tier-1 dataset A tutorial is available in form of a _J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k.
-In this Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net
-for downscaling adapted from [1]. ## Dataset description Within the _M_A_E_L_S_T_R_O_M
+snippet exemplary downloads the training dataset: ```commandline ds =
+cml.load_dataset("maelstrom-downscaling-tier2", dataset="training") ``` Note
+that the training dataset comprises about 250 GB of data and thus downloading
+can require several minutes or hours depending on the Internet connection. Due
+to the comprehensive size of the dataset, no augmented variant is provided. ###
+Saving the data on disk By default, `CliMetLab` only caches the data. To save
+the data persistently onto disk/in the user's filesystem, `persist=True` must
+be added, when running the `to_xarray`-method. Furthermore, a directory-path
+under which the file(-s) will be saved must be parsed via `data_dir`. The
+following command exemplifies saving the large-scale Tier-2 dataset. ``` ds =
+cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
+ds.to_xarray(persist=True, data_dir="/my/local/path") ``` ### Tutorial for the
+Tier-1 dataset A tutorial is available in form of a _J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k. In this
+Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net for
+downscaling adapted from [1]. ## Dataset description Within the _M_A_E_L_S_T_R_O_M
 project, two different datasets are provided that are used to construct
 statistical downscaling tasks with deep neural networks. The first dataset, the
 Tier-1 dataset, serves as the starting point and provides the data for a pure
 downscaling task similar to the super-resolution task in computer vision.
 The Tier-2 dataset provides the data for a real downscaling task in meteorology
 where the super-resolution task is complemented by bias correction.
 Both datasets will be described in more detail in the following. ### The Tier-
@@ -64,33 +73,37 @@
 2 dataset provides data for a real downscaling task where coarse-grained ERA5
 reanalysis data [3] are downscaled onto the high-resolved grid of the COSMO
 REA6 dataset [4]. Since data from two different models are now used, where
 COSMO REA6 provides added value over complex terrain due to its higher spatial
 resolution, the downscaling task is now twofold: The data has to be super-
 resolved and bias-corrected. Here, we still target the 2m temperature as with
 the Tier-1 dataset, but include more predictor variables: - 2m temperature -
-850 hPa- and 925 hPa temperature - surface latent and sensible heat fluxes -
-10m horizontal wind (u,v) - boundary layer height The surface topography from
-the ERA5 and the COSMO REA6 datasets are also included as static predictor
-variables. As a necessary prerequisite, the underlying grid of both reanalysis
-datasets needed to be merged. Here, we have remapped the ERA5 data onto the
-rotated pole grid deployed by the COSMO model [5]. With a grid spacing of
-0.275° in rotated coordinates, the spatial resolution of the ERA 5 data is five
-times coarser than the target data, the COSMO REA6-data (dx=0.055°). Similar to
-the Tier-1 dataset, the ERA5-data is bi-linearly interpolated onto the high
-resolved target grid to serve as input for the neural networks for downscaling.
+temperature from model levels 137, 135, 131, 127, 122 and 115 - surface
+pressure - surface latent and sensible heat fluxes - 10m horizontal wind (u,v)
+- boundary layer height The surface topography from the ERA5 and the COSMO REA6
+datasets are also included as static predictor variables. As a necessary
+prerequisite, the underlying grid of both reanalysis datasets needed to be
+merged. Here, we have remapped the ERA5 data onto the rotated pole grid
+deployed by the COSMO model [5]. With a grid spacing of 0.275° in rotated
+coordinates, the spatial resolution of the ERA 5 data is five times coarser
+than the target data, the COSMO REA6-data (dx=0.055°). Similar to the Tier-
+1 dataset, the ERA5-data is bi-linearly interpolated onto the high resolved
+target grid to serve as input for the neural networks for downscaling.
 Currently, the target domain of the Tier-2 dataset comprises 120x96 grid points
 (with dx=0.055°) covering large parts of Central Europe to include complex
 terrain of the Alps and the German low mountain range. Hourly data is provided
-for the years between 2006 and 2018. By default, the years 2006-2016 constitute
+for the years between 1995 and 2018. By default, the years 1995-2016 constitute
 the training dataset, while 2017 and 2018 are used for validation and testing,
-respectively. ## References **[1]** Sha, Yingkai, et al. "Deep-learning-based
-gridded downscaling of surface meteorological variables in complex terrain.
-Part I: Daily maximum and minimum 2-m temperature." Journal of Applied
-Meteorology and Climatology 59.12 (2020): 2057-2073. _D_O_I.
+respectively. This dataset constitutes the final dataset used in Application 5
+of the MAELSTROM project as described in this [report](https://www.maelstrom-
+eurohpc.eu/content/docs/uploads/doc50.pdf). ## References **[1]** Sha, Yingkai,
+et al. "Deep-learning-based gridded downscaling of surface meteorological
+variables in complex terrain. Part I: Daily maximum and minimum 2-
+m temperature." Journal of Applied Meteorology and Climatology 59.12 (2020):
+2057-2073. _D_O_I.
 **[2]** Leinonen, Jussi et al., "Stochastic Super-Resolution for Downscaling
 Time-Evolving Atmospheric Fields With a Generative Adversarial Network." IEEE
 Transactions on Geoscience and Remote Sensing 59.9 (2021): 7211-7223 _D_O_I.
 **[3]** Hersbach, Hans, et al. "The ERA5 global reanalysis." Quarterly Journal
 of the Royal Meteorological Society 146.730 (2020): 1999-2049. _D_O_I.
 **[4]** Bollmeyer, Christoph, et al. "Towards a high‐resolution regional
 reanalysis for the European CORDEX domain." Quarterly Journal of the Royal
```

### Comparing `climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling/downscaling.py` & `climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling/downscaling_tier1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-#!/usr/bin/env python3# (C) Copyright 2021 ECMWF and JSC
+#!/usr/bin/env python3# (C) Copyright 2024 ECMWF and JSC
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF and JSC do not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 from __future__ import annotations
 
 import os
 from typing import Union, List
+import shutil
 import numpy as np
 import pandas as pd
 import xarray as xr
 import climetlab as cml
 from climetlab import Dataset
 from climetlab.decorators import normalize
 
 List_or_string = Union[List, str]
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 URL = "https://object-store.os-api.cci1.ecmwf.int"
-PATTERN = "{url}/maelstrom-ap5/unet_ds_t2m_{date}.nc"
+PATTERN = "{url}/maelstrom-ap5/tier-1/downscaling_tier1_{date}.nc"
 
-@normalize("x","date-list(%Y%m)")
+@normalize("x", "date-list(%Y-%m)")
 def DateListNormaliser(x):
     return x
 
 
 class Downscaling(Dataset):
     class_name = "Downsclaing_Dataset"
     name = "IFS t2m dataset"
@@ -51,17 +52,17 @@
 
     dataset_types = {"training": dates_all[dates_all.year.isin(list(np.arange(2016, 2020)))],
                      "validation": dates_all[np.logical_and(dates_all.year.isin([2020]),
                                                             dates_all.month.isin([5, 7, 8]))],
                      "testing": dates_all[np.logical_and(dates_all.year.isin([2020]),
                                                          dates_all.month.isin([4, 6, 9]))],
                      # augmenetd datasets are stored in individual files
-                     "training_aug": "maelstrom-downscaling_train_aug.nc",
-                     "validation_aug": "maelstrom-downscaling_val_aug.nc",
-                     "testing_aug": "maelstrom-downscaling_test_aug.nc"}
+                     "training_aug": "downscaling_tier1_train_aug.nc",
+                     "validation_aug": "downscaling_tier1_val_aug.nc",
+                     "testing_aug": "downscaling_tier1_test_aug.nc"}
 
     default_datelist = dataset_types["training"]
 
     def __init__(self, months: List = None, dataset: str = None):
         """
         Initialize data loader instance
         :param months: list of months for which downscaling data is requested
@@ -96,16 +97,16 @@
         if self.date is None:       # in case, no date is specified, a sngle URL-request is created
             data_url = os.path.join(*os.path.normpath(PATTERN).split(os.path.sep)[:-1],
                                     self.dataset_types[self.dataset])
             data_url = data_url.replace("{url}", URL)
             self.source = cml.load_source("url", data_url)
         else:
             request_dict = dict(url=URL, date=self.date)
-            self.source = cml.load_source("url-pattern", PATTERN, request_dict, merger=Merger())
-
+            self.source = cml.load_source("url-pattern", PATTERN, request_dict, merger=Merger(self.dataset))
+            
     def parse_date(self, dates: List_or_string):
         """
         Parse individual date or list of dates for downscaling dataset
         :param dates: list of dates (months) or individual month
         :return: normalized date string suitable for requiring downscaling data
         """
         if dates is None:
@@ -118,28 +119,44 @@
                 print("* {0}".format(dates[index]))
             raise ValueError("Unavailable months requested. Check your input.")
 
         return dates
 
 
 class Merger:
-    def __init__(self, engine: str = "netcdf4", options=None):
+    def __init__(self, dataset: str, engine: str = "netcdf4", options=None):
         """Initializes merger based on xarray's open_mfdataset.
         :param engine: Engine to read netCDF-files (see open_mfdataset-documentation for more details).
         :param options: Additional options passed to open_mfdataset.
         :return: -
         """
+        self.dataset = dataset
         self.engine = engine
         self.options = options if options is not None else {}
 
-    def to_xarray(self, paths: List):
+    def to_xarray(self, paths: List, persist: bool=False, data_dir: str=None):
         """
         Merger to read data from multiple netCDF-files
         :param paths: list containing paths to netCDF-data files to be read
-        :return: -
-        """
-        return xr.open_mfdataset(
-            paths,
-            engine=self.engine,
-            parallel=True,
-            **self.options
-        )
+        :param persist: boolean to save data persistently to disk (in addition to caching)
+        :param data_dir: directory under which data will be saved persistently
+        :return: the data as xarray.Dataset
+        """
+        ds = xr.open_mfdataset(paths, engine=self.engine, parallel=True, **self.options)
+        
+        # save data to disk if desired
+        if persist:
+            try:
+                os.makedirs(data_dir, exist_ok=True)
+            except TypeError as e:
+                print(f"Please parse a proper directory-path data_dir")
+                raise
+
+            
+            fname_tar = os.path.join(data_dir, f"downscaling_tier1_{self.dataset.replace('ing', '').replace('idation', '')}.nc")
+
+            ds.to_netcdf(fname_tar, engine=self.engine)
+            print(f"Saved data for persistently under {fname_tar}")
+
+        return ds
+
+
```

### Comparing `climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling/downscaling_tier2.py` & `climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling/downscaling_tier2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿#!/usr/bin/env python3# (C) Copyright 2023 ECMWF and JSC
+﻿#!/usr/bin/env python3# (C) Copyright 2024 ECMWF and JSC
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF and JSC do not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
@@ -14,19 +14,19 @@
 import xarray as xr
 import climetlab as cml
 from climetlab import Dataset
 from climetlab.decorators import normalize
 
 List_or_string = Union[List, str]
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 
 URL = "https://object-store.os-api.cci1.ecmwf.int"
-PATTERN = "{url}/maelstrom-ap5/maelstrom-downscaling-tier2_{date}.nc"
+PATTERN = "{url}/maelstrom-ap5/tier-2/downscaling_tier2_{date}.nc"
 
 @normalize("x","date-list(%Y-%m)")
 def DateListNormaliser(x):
     return x
 
 class Downscaling(Dataset):
     class_name = "Downsclaing_Dataset"
@@ -39,94 +39,117 @@
         "By downloading data from this dataset, you agree to the terms and conditions defined at "
         "https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-ap5/browse/climetlab-maelstrom-downscaling-ap5/LICENSE"
         "If you do not agree with such terms, do not download the data. "
     )
 
     dataset = None
 
-    dates_all = pd.date_range("2006-01-01", "2018-12-01", freq="MS")
+    dates_all = pd.date_range("1995-01-01", "2018-12-01", freq="MS")
 
     all_datelist = DateListNormaliser(dates_all)    
 
-    dataset_types = {"training": dates_all[dates_all.year.isin(list(np.arange(2006, 2017)))],
+    dataset_types = {"training": dates_all[dates_all.year.isin(list(np.arange(1995, 2017)))],
                      "validation": dates_all[dates_all.year.isin([2017])],
                      "testing": dates_all[dates_all.year.isin([2018])]}
 
     default_datelist = dataset_types["training"]
 
     def __init__(self, months: List = None, dataset: str = None):
         """
         Initialize data loader instance
         :param months: list of months for which downscaling data is requested
         :param dataset: name of dataset (see dataset_types-dictionary)
         """
-        method = "{0}->{1}".format(Downscaling.class_name, Downscaling.__init__.__name__)
+        self.dataset = dataset
+
+        assert not (months is None and dataset is None), "Either list of months or dataset-name must be passed."
 
-        assert not (months is None and dataset is None), "%{0}: Either list of months or dataset-name must be passed."\
-                                                         .format(method)
         if (not dataset is None) and (not months is None):
-            print("%{0}: List of months and dataset-name cannot be processed simultaneously. months will be ignored."
-                  .format(method))
+            print("List of months and dataset-name cannot be processed simultaneously. months will be ignored.")
 
         if dataset is None:
             self.date = self.parse_date(months)
         else:
             if not dataset in self.dataset_types.keys():
-                raise ValueError("%{0}: Unknown dataset type {1} passed. Valid choices are [{2}]"
-                                 .format(method, dataset, ",".join(self.dataset_types.keys())))
+                raise ValueError("Unknown dataset type {0} passed. Valid choices are [{1}]"
+                                 .format(dataset, ",".join(self.dataset_types.keys())))
             self.date = self.parse_date(self.dataset_types[dataset])
         
         # get the requested data
         self._load()
 
     def _load(self):
         """
         Builds the URL-request and retrieves the data
         :return: -
         """
         request_dict = dict(url=URL, date=self.date)
-        self.source = cml.load_source("url-pattern", PATTERN, request_dict, merger=Merger())
+        self.source = cml.load_source("url-pattern", PATTERN, request_dict, merger=Merger(self.dataset))
 
     def parse_date(self, dates: List_or_string):
         """
         Parse individual date or list of dates for downscaling dataset
         :param dates: list of dates (months) or individual month
         :return: normalized date string suitable for requiring downscaling data
         """
-        method = "{0}->{1}".format(Downscaling.class_name, Downscaling.__init__.__name__)
-
         if dates is None:
             dates = self.default_datelist
         
         dates = DateListNormaliser(dates)
         
         check_date = [d for d, date in enumerate(dates) if date not in self.all_datelist]
         if check_date:
-            print("%{0}: The following passed months are not available in the dataset:".format(method))
+            print("The following passed months are not available in the dataset:")
             for index in check_date:
                 print("* {0}".format(dates[index]))
-            raise ValueError("%{0}: Unavailable months requested. Check your input.".format(method))
+            raise ValueError("Unavailable months requested. Check your input.")
 
         return dates
 
 class Merger:
-    def __init__(self, engine: str = "netcdf4", options=None):
+    def __init__(self, dataset: str, engine: str = "netcdf4", options=None):
         """Initializes merger based on xarray's open_mfdataset.
         :param engine: Engine to read netCDF-files (see open_mfdataset-documentation for more details).
         :param options: Additional options passed to open_mfdataset.
         :return: -
         """
+        self.dataset = dataset
         self.engine = engine
         self.options = options if options is not None else {}
 
-    def to_xarray(self, paths: List):
+    def to_xarray(self, paths: List, persist: bool=False, data_dir: str=None):
         """
         Merger to read data from multiple netCDF-files
         :param paths: list containing paths to netCDF-data files to be read
-        :return: -
+        :param persist: boolean to save data persistently to disk (in addition to caching)
+        :param data_dir: directory under which data will be saved persistently
+        :return: the data as xarray.Dataset
         """
-        return xr.open_mfdataset(
-            paths,
-            engine=self.engine,
-            parallel=True,
-            **self.options
-       )
+        # read all files to provide xarray dataset
+        ds_all = xr.open_mfdataset(paths, engine=self.engine, parallel=True, **self.options)
+        
+        # save data to disk if desired
+        if persist:
+            try:
+                os.makedirs(data_dir, exist_ok=True)
+            except TypeError as e:
+                print(f"Please parse a proper directory-path data_dir")
+                raise
+            
+            if self.dataset == "training":
+                nfiles = len(paths)
+                
+                for i, path in enumerate(paths):
+                    ds = xr.open_dataset(path, chunks=-1)
+                    time0 = pd.to_datetime(ds["time"][0].values)
+
+                    fname_tar = os.path.join(data_dir, f"downscaling_tier2_train_{time0.strftime('%Y-%m')}.nc")
+
+                    shutil.copy(path, fname_tar)
+                    print(f"Persistently saved file for {self.dataset} under {fname_tar} ({i}/{nfiles})")
+            else:
+                fname_tar = os.path.join(data_dir, f"downscaling_tier1_{self.dataset.replace('ing', '').replace('idation', '')}.nc")
+
+                ds_all.to_netcdf(fname_tar, engine=self.engine)
+                print(f"Persistently saved data for {self.dataset} under {fname_tar}")
+            
+        return ds_all
```

### Comparing `climetlab_maelstrom_downscaling-0.3.1/climetlab_maelstrom_downscaling.egg-info/PKG-INFO` & `climetlab_maelstrom_downscaling-0.4.0/climetlab_maelstrom_downscaling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
-Name: climetlab-maelstrom-downscaling
-Version: 0.3.1
+Name: climetlab_maelstrom_downscaling
+Version: 0.4.0
 Summary: A dataset plugin for climetlab for the dataset maelstrom-downscaling.
 Home-page: https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-ap5/
 Author: Michael Langguth, Bing Gong
 Author-email: m.langguth@fz-juelich.de
 License: Apache License Version 2.0
 Keywords: meteorology
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: climetlab>=0.9.0
 
@@ -53,19 +54,29 @@
 ```
 By changing the `dataset`-argument to `"validation"` and `"testing"`, the validation and testing data can be retrieved.
 Furthermore, an augmented variant of the dataset is available which can be downloaded by adding 
 a `_augmented`-suffix to the `dataset`-arguments.
 
 ### Download the Tier-2 data
 The Tier-2 dataset can be downloaded by replacing the value of the first argument of `cml.load_dataset`. 
-The following code-snippet exemplary downloads the training dataset (about 45 GB!):
+The following code-snippet exemplary downloads the training dataset:
 ```commandline
 ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
 ```
-Note that no augmented variant of the Tier-2 dataset is provided.
+Note that the training dataset comprises about 250 GB of data and thus downloading can require several minutes or hours depending on the Internet connection.
+Due to the comprehensive size of the dataset, no augmented variant is provided.
+
+### Saving the data on disk
+By default, `CliMetLab` only caches the data. To save the data persistently onto disk/in the user's filesystem,
+`persist=True` must be added, when running the `to_xarray`-method. Furthermore, a directory-path under which the file(-s) will be saved must be parsed via `data_dir`.
+The following command exemplifies saving the large-scale Tier-2 dataset.
+```
+ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
+ds.to_xarray(persist=True, data_dir="/my/local/path")
+```
 
 ### Tutorial for the Tier-1 dataset
 
 A tutorial is available in form of a <a href="https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-ap5/browse/notebooks/demo_downscaling_dataset.ipynb">Jupyter Notebook</a>.
 In this Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net for downscaling adapted from [1].
 
 ## Dataset description
@@ -107,15 +118,16 @@
 are downscaled onto the high-resolved grid of the COSMO REA6 dataset [4]. 
 Since data from two different models are now used, where COSMO REA6 provides added value
 over complex terrain due to its higher spatial resolution, the downscaling task is now twofold:
 The data has to be super-resolved and bias-corrected.
 
 Here, we still target the 2m temperature as with the Tier-1 dataset, but include more predictor variables:
 - 2m temperature
-- 850 hPa- and 925 hPa temperature
+- temperature from model levels 137, 135, 131, 127, 122 and 115
+- surface pressure
 - surface latent and sensible heat fluxes
 - 10m horizontal wind (u,v)
 - boundary layer height
 
 The surface topography from the ERA5 and the COSMO REA6 datasets are also included as static predictor variables.
 
 As a necessary prerequisite, the underlying grid of both reanalysis datasets needed to be merged.
@@ -123,17 +135,19 @@
 With a grid spacing of 0.275° in rotated coordinates, the spatial resolution of the ERA 5 data is 
 five times coarser than the target data, the COSMO REA6-data (dx=0.055°). 
 Similar to the Tier-1 dataset, the ERA5-data is bi-linearly interpolated onto the high resolved target 
 grid to serve as input for the neural networks for downscaling.
 
 Currently, the target domain of the Tier-2 dataset comprises 120x96 grid points (with dx=0.055°) 
 covering large parts of Central Europe to include complex terrain of the Alps and the German low mountain range.
-Hourly data is provided for the years between 2006 and 2018. By default, the years 2006-2016 constitute the 
+Hourly data is provided for the years between 1995 and 2018. By default, the years 1995-2016 constitute the 
 training dataset, while 2017 and 2018 are used for validation and testing, respectively.
 
+This dataset constitutes the final dataset used in Application 5 of the MAELSTROM project as described in this [report](https://www.maelstrom-eurohpc.eu/content/docs/uploads/doc50.pdf).
+
 ## References
 **[1]** Sha, Yingkai, et al. "Deep-learning-based gridded downscaling of surface meteorological variables in complex
 terrain. Part I: Daily maximum and minimum 2-m temperature."
 Journal of Applied Meteorology and Climatology 59.12 (2020): 2057-2073. 
 <a href="https://doi.org/10.1175/JAMC-D-20-0057.1"> DOI</a>.<br>
 **[2]** Leinonen, Jussi et al., "Stochastic Super-Resolution for Downscaling Time-Evolving Atmospheric Fields
 With a Generative Adversarial Network." IEEE Transactions on Geoscience and Remote Sensing 59.9 (2021): 7211-7223
```

#### html2text {}

```diff
@@ -1,47 +1,56 @@
-Metadata-Version: 2.1 Name: climetlab-maelstrom-downscaling Version: 0.3.1
+Metadata-Version: 2.1 Name: climetlab_maelstrom_downscaling Version: 0.4.0
 Summary: A dataset plugin for climetlab for the dataset maelstrom-downscaling.
 Home-page: https://git.ecmwf.int/projects/MLFET/repos/maelstrom-downscaling-
 ap5/ Author: Michael Langguth, Bing Gong Author-email: m.langguth@fz-juelich.de
 License: Apache License Version 2.0 Keywords: meteorology Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-climetlab>=0.9.0 ï»¿# maelstrom-downscaling-ap5 A _C_l_i_M_e_t_L_a_b_ dataset plugin for
-the datasets used in application of the _M_A_E_L_S_T_R_O_M_ _p_r_o_j_e_c_t. Features -------
-- This README provides a brief description of the provided datasets for
-statistical downscaling of meteorological fields, the target of _a_p_p_l_i_c_a_t_i_o_n_ _5_ 
-_(_A_P_5_)_ _i_n_ _s_c_o_p_e_ _o_f_ _M_A_E_L_S_T_R_O_M. Two different datasets, named Tier-1 and Tier-2 in
-the following, can be downloaded from the _A_W_S_ _s_3_-_b_u_c_k_e_t, provided by ECMWF,
-with this `CliMetLab` plugin. Both datasets are distributed under the _A_p_a_c_h_e
-_L_i_c_e_n_s_e_,_ _v_e_r_s_i_o_n_ _2_._0_ and thus are open-access. ## Using climetlab to access the
-data The `CliMetLab` python package allows easy access to the data with a few
-lines of code.
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: climetlab>=0.9.0 ï»¿# maelstrom-
+downscaling-ap5 A _C_l_i_M_e_t_L_a_b_ dataset plugin for the datasets used in application
+of the _M_A_E_L_S_T_R_O_M_ _p_r_o_j_e_c_t. Features -------- This README provides a brief
+description of the provided datasets for statistical downscaling of
+meteorological fields, the target of _a_p_p_l_i_c_a_t_i_o_n_ _5_ _(_A_P_5_)_ _i_n_ _s_c_o_p_e_ _o_f_ _M_A_E_L_S_T_R_O_M.
+Two different datasets, named Tier-1 and Tier-2 in the following, can be
+downloaded from the _A_W_S_ _s_3_-_b_u_c_k_e_t, provided by ECMWF, with this `CliMetLab`
+plugin. Both datasets are distributed under the _A_p_a_c_h_e_ _L_i_c_e_n_s_e_,_ _v_e_r_s_i_o_n_ _2_._0_ and
+thus are open-access. ## Using climetlab to access the data The `CliMetLab`
+python package allows easy access to the data with a few lines of code.
 The following examples demonstrate how to obtain the two provided datasets. A
 more detailed description of both datasets is provided afterwards. ### Download
 the Tier-1 data The training data of the Tier-1 dataset can be downloaded as
 follows: ``` !pip install climetlab climetlab_maelstrom_downscaling import
 climetlab as cml ds = cml.load_dataset("maelstrom-downscaling",
 dataset="training") ds.to_xarray() ``` By changing the `dataset`-argument to
 `"validation"` and `"testing"`, the validation and testing data can be
 retrieved. Furthermore, an augmented variant of the dataset is available which
 can be downloaded by adding a `_augmented`-suffix to the `dataset`-arguments.
 ### Download the Tier-2 data The Tier-2 dataset can be downloaded by replacing
 the value of the first argument of `cml.load_dataset`. The following code-
-snippet exemplary downloads the training dataset (about 45 GB!): ```commandline
-ds = cml.load_dataset("maelstrom-downscaling-tier2", dataset="training") ```
-Note that no augmented variant of the Tier-2 dataset is provided. ### Tutorial
-for the Tier-1 dataset A tutorial is available in form of a _J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k.
-In this Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net
-for downscaling adapted from [1]. ## Dataset description Within the _M_A_E_L_S_T_R_O_M
+snippet exemplary downloads the training dataset: ```commandline ds =
+cml.load_dataset("maelstrom-downscaling-tier2", dataset="training") ``` Note
+that the training dataset comprises about 250 GB of data and thus downloading
+can require several minutes or hours depending on the Internet connection. Due
+to the comprehensive size of the dataset, no augmented variant is provided. ###
+Saving the data on disk By default, `CliMetLab` only caches the data. To save
+the data persistently onto disk/in the user's filesystem, `persist=True` must
+be added, when running the `to_xarray`-method. Furthermore, a directory-path
+under which the file(-s) will be saved must be parsed via `data_dir`. The
+following command exemplifies saving the large-scale Tier-2 dataset. ``` ds =
+cml.load_dataset("maelstrom-downscaling-tier2", dataset="training")
+ds.to_xarray(persist=True, data_dir="/my/local/path") ``` ### Tutorial for the
+Tier-1 dataset A tutorial is available in form of a _J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k. In this
+Jupyter Notebook, the Tier-1 dataset is used to train a simple U-Net for
+downscaling adapted from [1]. ## Dataset description Within the _M_A_E_L_S_T_R_O_M
 project, two different datasets are provided that are used to construct
 statistical downscaling tasks with deep neural networks. The first dataset, the
 Tier-1 dataset, serves as the starting point and provides the data for a pure
 downscaling task similar to the super-resolution task in computer vision.
 The Tier-2 dataset provides the data for a real downscaling task in meteorology
 where the super-resolution task is complemented by bias correction.
 Both datasets will be described in more detail in the following. ### The Tier-
@@ -78,31 +87,34 @@
 2 dataset provides data for a real downscaling task where coarse-grained ERA5
 reanalysis data [3] are downscaled onto the high-resolved grid of the COSMO
 REA6 dataset [4]. Since data from two different models are now used, where
 COSMO REA6 provides added value over complex terrain due to its higher spatial
 resolution, the downscaling task is now twofold: The data has to be super-
 resolved and bias-corrected. Here, we still target the 2m temperature as with
 the Tier-1 dataset, but include more predictor variables: - 2m temperature -
-850 hPa- and 925 hPa temperature - surface latent and sensible heat fluxes -
-10m horizontal wind (u,v) - boundary layer height The surface topography from
-the ERA5 and the COSMO REA6 datasets are also included as static predictor
-variables. As a necessary prerequisite, the underlying grid of both reanalysis
-datasets needed to be merged. Here, we have remapped the ERA5 data onto the
-rotated pole grid deployed by the COSMO model [5]. With a grid spacing of
-0.275Â° in rotated coordinates, the spatial resolution of the ERA 5 data is
-five times coarser than the target data, the COSMO REA6-data (dx=0.055Â°).
-Similar to the Tier-1 dataset, the ERA5-data is bi-linearly interpolated onto
-the high resolved target grid to serve as input for the neural networks for
-downscaling. Currently, the target domain of the Tier-2 dataset comprises
-120x96 grid points (with dx=0.055Â°) covering large parts of Central Europe to
-include complex terrain of the Alps and the German low mountain range. Hourly
-data is provided for the years between 2006 and 2018. By default, the years
-2006-2016 constitute the training dataset, while 2017 and 2018 are used for
-validation and testing, respectively. ## References **[1]** Sha, Yingkai, et
-al. "Deep-learning-based gridded downscaling of surface meteorological
+temperature from model levels 137, 135, 131, 127, 122 and 115 - surface
+pressure - surface latent and sensible heat fluxes - 10m horizontal wind (u,v)
+- boundary layer height The surface topography from the ERA5 and the COSMO REA6
+datasets are also included as static predictor variables. As a necessary
+prerequisite, the underlying grid of both reanalysis datasets needed to be
+merged. Here, we have remapped the ERA5 data onto the rotated pole grid
+deployed by the COSMO model [5]. With a grid spacing of 0.275Â° in rotated
+coordinates, the spatial resolution of the ERA 5 data is five times coarser
+than the target data, the COSMO REA6-data (dx=0.055Â°). Similar to the Tier-
+1 dataset, the ERA5-data is bi-linearly interpolated onto the high resolved
+target grid to serve as input for the neural networks for downscaling.
+Currently, the target domain of the Tier-2 dataset comprises 120x96 grid points
+(with dx=0.055Â°) covering large parts of Central Europe to include complex
+terrain of the Alps and the German low mountain range. Hourly data is provided
+for the years between 1995 and 2018. By default, the years 1995-2016 constitute
+the training dataset, while 2017 and 2018 are used for validation and testing,
+respectively. This dataset constitutes the final dataset used in Application 5
+of the MAELSTROM project as described in this [report](https://www.maelstrom-
+eurohpc.eu/content/docs/uploads/doc50.pdf). ## References **[1]** Sha, Yingkai,
+et al. "Deep-learning-based gridded downscaling of surface meteorological
 variables in complex terrain. Part I: Daily maximum and minimum 2-
 m temperature." Journal of Applied Meteorology and Climatology 59.12 (2020):
 2057-2073. _D_O_I.
 **[2]** Leinonen, Jussi et al., "Stochastic Super-Resolution for Downscaling
 Time-Evolving Atmospheric Fields With a Generative Adversarial Network." IEEE
 Transactions on Geoscience and Remote Sensing 59.9 (2021): 7211-7223 _D_O_I.
 **[3]** Hersbach, Hans, et al. "The ERA5 global reanalysis." Quarterly Journal
```

### Comparing `climetlab_maelstrom_downscaling-0.3.1/setup.py` & `climetlab_maelstrom_downscaling-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,26 +45,27 @@
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=["climetlab>=0.9.0"],
     extras_require=extras_require,
     zip_safe=True,
     entry_points={
         "climetlab.datasets": [
-            "maelstrom-downscaling-tier1 = climetlab_maelstrom_downscaling.downscaling:Downscaling",
+            "maelstrom-downscaling-tier1 = climetlab_maelstrom_downscaling.downscaling_tier1:Downscaling",
             "maelstrom-downscaling-tier2 = climetlab_maelstrom_downscaling.downscaling_tier2:Downscaling",
             # "maelstrom-downscaling-ap5-other-dataset = climetlab_maelstrom_downscaling_ap5.other_dataset:OtherDatasetClass",
         ]
     },
     keywords="meteorology",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `climetlab_maelstrom_downscaling-0.3.1/tests/test_downscaling_dataset.py` & `climetlab_maelstrom_downscaling-0.4.0/tests/test_downscaling_dataset.py`

 * *Files identical despite different names*

### Comparing `climetlab_maelstrom_downscaling-0.3.1/tests/test_notebooks.py` & `climetlab_maelstrom_downscaling-0.4.0/tests/test_notebooks.py`

 * *Files identical despite different names*

