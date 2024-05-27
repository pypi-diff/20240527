# Comparing `tmp/pygrinder-0.4.tar.gz` & `tmp/pygrinder-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrinder-0.4.tar", last modified: Sat Dec 16 05:40:39 2023, max compression
+gzip compressed data, was "pygrinder-0.5.tar", last modified: Mon May 27 16:42:49 2024, max compression
```

## Comparing `pygrinder-0.4.tar` & `pygrinder-0.5.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 05:40:39.147081 pygrinder-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-12-16 05:39:00.000000 pygrinder-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2023-12-16 05:40:39.147081 pygrinder-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2023-12-16 05:39:00.000000 pygrinder-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 05:40:39.147081 pygrinder-0.4/pygrinder/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 05:40:39.147081 pygrinder-0.4/pygrinder/missing_at_random/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_at_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_at_random/mar_logistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 05:40:39.147081 pygrinder-0.4/pygrinder/missing_completely_at_random/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_completely_at_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_completely_at_random/little_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_completely_at_random/mcar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 05:40:39.147081 pygrinder-0.4/pygrinder/missing_not_at_random/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_not_at_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_not_at_random/mnar_t.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/missing_not_at_random/mnar_x.py
--rw-r--r--   0 runner    (1001) docker     (127)     5653 2023-12-16 05:39:00.000000 pygrinder-0.4/pygrinder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 05:40:39.147081 pygrinder-0.4/pygrinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2023-12-16 05:40:39.000000 pygrinder-0.4/pygrinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-16 05:40:39.000000 pygrinder-0.4/pygrinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 05:40:39.000000 pygrinder-0.4/pygrinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-16 05:40:39.000000 pygrinder-0.4/pygrinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-16 05:40:39.000000 pygrinder-0.4/pygrinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-16 05:40:39.147081 pygrinder-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-16 05:39:00.000000 pygrinder-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:49.711243 pygrinder-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-27 16:41:11.000000 pygrinder-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-27 16:42:49.711243 pygrinder-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-05-27 16:41:11.000000 pygrinder-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:49.707243 pygrinder-0.5/pygrinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:49.711243 pygrinder-0.5/pygrinder/missing_at_random/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_at_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_at_random/mar_logistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:49.711243 pygrinder-0.5/pygrinder/missing_completely_at_random/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_completely_at_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_completely_at_random/little_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_completely_at_random/mcar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:49.711243 pygrinder-0.5/pygrinder/missing_not_at_random/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_not_at_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_not_at_random/mnar_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/missing_not_at_random/mnar_x.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:49.711243 pygrinder-0.5/pygrinder/randomly_drop_observations/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/randomly_drop_observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/randomly_drop_observations/rdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5653 2024-05-27 16:41:11.000000 pygrinder-0.5/pygrinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:42:49.711243 pygrinder-0.5/pygrinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-27 16:42:49.000000 pygrinder-0.5/pygrinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-27 16:42:49.000000 pygrinder-0.5/pygrinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:42:49.000000 pygrinder-0.5/pygrinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 16:42:49.000000 pygrinder-0.5/pygrinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 16:42:49.000000 pygrinder-0.5/pygrinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 16:42:49.711243 pygrinder-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-27 16:41:11.000000 pygrinder-0.5/setup.py
```

### Comparing `pygrinder-0.4/LICENSE` & `pygrinder-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrinder-0.4/PKG-INFO` & `pygrinder-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrinder
-Version: 0.4
+Version: 0.5
 Summary: A Python toolkit for introducing missing values into datasets
 Home-page: https://github.com/WenjieDu/PyGrinder
 Download-URL: https://github.com/WenjieDu/PyGrinder/archive/main.zip
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Keywords: data corruption,incomplete data,data mining,pypots,missingness,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values,pypots
@@ -14,17 +14,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<a href='https://github.com/WenjieDu/PyGrinder'><img src='https://pypots.com/figs/pypots_logos/PyGrinder_logo_FFBG.svg?sanitize=true' width='200' align='right' /></a>
+<a href='https://github.com/WenjieDu/PyGrinder'><img src='https://pypots.com/figs/pypots_logos/PyGrinder/logo_FFBG.svg' width='200' align='right' /></a>
 
-<h2 align="center">Welcome to PyGrinder</h2>
+<h3 align="center">Welcome to PyGrinder</h3>
 
 *<p align='center'>a Python toolkit for grinding data beans into the incomplete</p>*
 
 <p align='center'>
     <a href='https://github.com/WenjieDu/PyGrinder'>
         <img alt='Python version' src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     </a>
@@ -37,18 +37,18 @@
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README.md#-community">
         <img alt="Community" src="https://img.shields.io/badge/join_us-community!-C8A062">
     </a>
     <a href="https://github.com/WenjieDu/PyGrinder/graphs/contributors">
         <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/wenjiedu/pygrinder?color=D8E699&label=Contributors&logo=GitHub">
     </a>
     <a href="https://star-history.com/#wenjiedu/pygrinder">
-        <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/pygrinder?logo=Github&color=6BB392&label=Stars">
+        <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/pygrinder?logo=None&color=6BB392&label=%E2%98%85%20Stars">
     </a>
     <a href="https://github.com/WenjieDu/PyGrinder/network/members">
-        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=Github&color=91B821&label=Forks">
+        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=forgejo&logoColor=black&label=Forks">
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/PyGrinder">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/PyGrinder?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <a href='https://coveralls.io/github/WenjieDu/PyGrinder'>
         <img alt='Coveralls report' src='https://img.shields.io/coverallsCoverage/github/WenjieDu/PyGrinder?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
@@ -62,15 +62,15 @@
         <img alt="Conda downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/conda_pygrinder_downloads.json">
     </a>
     <a href='https://pepy.tech/project/PyGrinder'>
         <img alt='PyPI downloads' src='https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pygrinder_downloads.json'>
     </a>
 </p>
 
-<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true' width='160' align='left' /></a>
+<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg' width='160' align='left' /></a>
 PyGrinder is a part of
 <a href="https://github.com/WenjieDu/PyPOTS">
 PyPOTS <img align="center" src="https://img.shields.io/github/stars/WenjieDu/PyPOTS?style=social">
 </a>
 (a Python toolbox for data mining on
 Partially-Observed Time Series), was called PyCorruptor and separated from PyPOTS for decoupling missingness-creating functionalities from
 learning algorithms.
@@ -82,15 +82,15 @@
 
 
 ## ❖ Usage Examples
 PyGrinder now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install pygrinder`, you may need to specify the channel with option `-c conda-forge`
 
-or install from PyPI:
+or install via PyPI:
 > pip install pygrinder
 
 or install from source code:
 > pip install `https://github.com/WenjieDu/PyGrinder/archive/main.zip`
 
 ```python
 import numpy as np
@@ -108,23 +108,27 @@
 # grind the dataset with MNAR pattern
 X_with_mnar_x_data = mnar_x(ts_dataset, offset=0.1)
 X_with_mnar_t_data = mnar_t(ts_dataset, cycle=20, pos = 10, scale = 3)
 ```
 
 
 ## ❖ Citing PyGrinder/PyPOTS
-
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use PyGrinder in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
+<p align="center">
+<a href="https://github.com/WenjieDu/PyPOTS">
+    <img src="https://pypots.com/figs/pypots_logos/Ecosystem/PyPOTS_Ecosystem_Pipeline.png" width="95%"/>
+</a>
+</p>
 
 ``` bibtex
-@article{du2023PyPOTS,
+@article{du2023pypots,
 title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
 author={Wenjie Du},
 year={2023},
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
@@ -132,28 +136,12 @@
 }
 ```
 
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
-or
-
-``` bibtex
-@inproceedings{du2023PyPOTS,
-title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
-booktitle={9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)},
-author={Wenjie Du},
-year={2023},
-url={https://arxiv.org/abs/2305.18811},
-}
-```
-
-> Wenjie Du. (2023).
-> PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
-> In *9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://arxiv.org/abs/2305.18811
-
 
 <details>
 <summary>🏠 Visits</summary>
 <img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FPyCorruptor&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+May+2022&edge_flat=false'>
 </details>
```

#### html2text {}

```diff
@@ -1,67 +1,61 @@
-Metadata-Version: 2.1 Name: pygrinder Version: 0.4 Summary: A Python toolkit
+Metadata-Version: 2.1 Name: pygrinder Version: 0.5 Summary: A Python toolkit
 for introducing missing values into datasets Home-page: https://github.com/
 WenjieDu/PyGrinder Download-URL: https://github.com/WenjieDu/PyGrinder/archive/
 main.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-
 Clause Keywords: data corruption,incomplete data,data
 mining,pypots,missingness,partially observed,irregular sampled,partially-
 observed time series,incomplete time series,missing data,missing values,pypots
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Description-Content-Type: text/markdown
-License-File: LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/
-_P_y_G_r_i_n_d_e_r___l_o_g_o___F_F_B_G_._s_v_g_?_s_a_n_i_t_i_z_e_=_t_r_u_e_]
-                       ********** WWeellccoommee ttoo PPyyGGrriinnddeerr **********
+License-File: LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_G_r_i_n_d_e_r_/
+_l_o_g_o___F_F_B_G_._s_v_g_]
+                        ******** WWeellccoommee ttoo PPyyGGrriinnddeerr ********
 *
          a Python toolkit for grinding data beans into the incomplete
 *
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]_[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b
        _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e_ _C_l_i_m_a_t_e
 _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _r_e_p_o_r_t_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_a_r_X_i_v_ _D_O_I_]_[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]
                                _[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
-_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/
-_P_y_P_O_T_S___l_o_g_o___F_F_B_G_._s_v_g_?_s_a_n_i_t_i_z_e_=_t_r_u_e_]PyGrinder is a part of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/_P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a Python toolbox for
-data mining on Partially-Observed Time Series), was called PyCorruptor and
-separated from PyPOTS for decoupling missingness-creating functionalities from
-learning algorithms. In data analysis and modeling, sometimes we may need to
-corrupt the original data to achieve our goal, for instance, evaluating models'
-ability to reconstruct corrupted data or assessing the model's performance on
-only partially-observed data. PyGrinder is such a tool to help you corrupt your
-data, which provides several patterns to create missing values in the given
-data. ## â Usage Examples PyGrinder now is available on _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-_l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸
-Install it with `conda install pygrinder`, you may need to specify the channel
-with option `-c conda-forge` or install from PyPI: > pip install pygrinder or
-install from source code: > pip install `https://github.com/WenjieDu/PyGrinder/
-archive/main.zip` ```python import numpy as np from pygrinder import mcar,
-mar_logistic, mnar_x, mnar_t # given a time-series dataset with 128 samples,
-each sample with 10 time steps and 36 data features ts_dataset =
-np.random.randn(128, 10, 36) # grind the dataset with MCAR pattern, 10% missing
-probability, and using 0 to fill missing values X_with_mcar_data = mcar
-(ts_dataset, p=0.1) # grind the dataset with MAR pattern X_with_mar_data =
-mar_logistic(ts_dataset[:, 0, :], obs_rate=0.1, missing_rate=0.1) # grind the
-dataset with MNAR pattern X_with_mnar_x_data = mnar_x(ts_dataset, offset=0.1)
-X_with_mnar_t_data = mnar_t(ts_dataset, cycle=20, pos = 10, scale = 3) ``` ##
-â Citing PyGrinder/PyPOTS The paper introducing PyPOTS project is available
-on arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing
-to publish it in prestigious academic venues, e.g. JMLR (track for [Machine
-Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use
-PyGrinder in your work, please cite PyPOTS project as below and ðstar this
-repository to make others notice this library. ð¤ Thank you! ``` bibtex
-@article{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining on
-Partially-Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint=
-{2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]PyGrinder is a part
+of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/_P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a
+Python toolbox for data mining on Partially-Observed Time Series), was called
+PyCorruptor and separated from PyPOTS for decoupling missingness-creating
+functionalities from learning algorithms. In data analysis and modeling,
+sometimes we may need to corrupt the original data to achieve our goal, for
+instance, evaluating models' ability to reconstruct corrupted data or assessing
+the model's performance on only partially-observed data. PyGrinder is such a
+tool to help you corrupt your data, which provides several patterns to create
+missing values in the given data. ## â Usage Examples PyGrinder now is
+available on _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-
+_l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸ Install it with `conda install
+pygrinder`, you may need to specify the channel with option `-c conda-forge` or
+install via PyPI: > pip install pygrinder or install from source code: > pip
+install `https://github.com/WenjieDu/PyGrinder/archive/main.zip` ```python
+import numpy as np from pygrinder import mcar, mar_logistic, mnar_x, mnar_t #
+given a time-series dataset with 128 samples, each sample with 10 time steps
+and 36 data features ts_dataset = np.random.randn(128, 10, 36) # grind the
+dataset with MCAR pattern, 10% missing probability, and using 0 to fill missing
+values X_with_mcar_data = mcar(ts_dataset, p=0.1) # grind the dataset with MAR
+pattern X_with_mar_data = mar_logistic(ts_dataset[:, 0, :], obs_rate=0.1,
+missing_rate=0.1) # grind the dataset with MNAR pattern X_with_mnar_x_data =
+mnar_x(ts_dataset, offset=0.1) X_with_mnar_t_data = mnar_t(ts_dataset,
+cycle=20, pos = 10, scale = 3) ``` ## â Citing PyGrinder/PyPOTS The paper
+introducing PyPOTS project is available on arXiv at [this URL](https://
+arxiv.org/abs/2305.18811), and we are pursuing to publish it in prestigious
+academic venues, e.g. JMLR (track for [Machine Learning Open Source Software]
+(https://www.jmlr.org/mloss/)). If you use PyGrinder in your work, please cite
+PyPOTS project as below and ðstar this repository to make others notice this
+library. ð¤ Thank you!
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
+``` bibtex @article{du2023pypots, title={{PyPOTS: a Python toolbox for data
+mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
+eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
 arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du.
 (2023). > PyPOTS: a Python toolbox for data mining on Partially-Observed Time
-Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 or ``` bibtex
-@inproceedings{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining
-on Partially-Observed Time Series}}, booktitle={9th SIGKDD workshop on Mining
-and Learning from Time Series (MiLeTS'23)}, author={Wenjie Du}, year={2023},
-url={https://arxiv.org/abs/2305.18811}, } ``` > Wenjie Du. (2023). > PyPOTS: a
-Python toolbox for data mining on Partially-Observed Time Series. > In *9th
-SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://
-arxiv.org/abs/2305.18811 ð  Visits[https://hits.seeyoufarm.com/api/count/
-incr/
+Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FPyCorruptor&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+May+2022&edge_flat=false]
```

### Comparing `pygrinder-0.4/README.md` & `pygrinder-0.5/pygrinder.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,30 @@
-<a href='https://github.com/WenjieDu/PyGrinder'><img src='https://pypots.com/figs/pypots_logos/PyGrinder_logo_FFBG.svg?sanitize=true' width='200' align='right' /></a>
+Metadata-Version: 2.1
+Name: pygrinder
+Version: 0.5
+Summary: A Python toolkit for introducing missing values into datasets
+Home-page: https://github.com/WenjieDu/PyGrinder
+Download-URL: https://github.com/WenjieDu/PyGrinder/archive/main.zip
+Author: Wenjie Du
+Author-email: wenjay.du@gmail.com
+License: BSD-3-Clause
+Keywords: data corruption,incomplete data,data mining,pypots,missingness,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values,pypots
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-<h2 align="center">Welcome to PyGrinder</h2>
+<a href='https://github.com/WenjieDu/PyGrinder'><img src='https://pypots.com/figs/pypots_logos/PyGrinder/logo_FFBG.svg' width='200' align='right' /></a>
+
+<h3 align="center">Welcome to PyGrinder</h3>
 
 *<p align='center'>a Python toolkit for grinding data beans into the incomplete</p>*
 
 <p align='center'>
     <a href='https://github.com/WenjieDu/PyGrinder'>
         <img alt='Python version' src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     </a>
@@ -17,18 +37,18 @@
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README.md#-community">
         <img alt="Community" src="https://img.shields.io/badge/join_us-community!-C8A062">
     </a>
     <a href="https://github.com/WenjieDu/PyGrinder/graphs/contributors">
         <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/wenjiedu/pygrinder?color=D8E699&label=Contributors&logo=GitHub">
     </a>
     <a href="https://star-history.com/#wenjiedu/pygrinder">
-        <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/pygrinder?logo=Github&color=6BB392&label=Stars">
+        <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/pygrinder?logo=None&color=6BB392&label=%E2%98%85%20Stars">
     </a>
     <a href="https://github.com/WenjieDu/PyGrinder/network/members">
-        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=Github&color=91B821&label=Forks">
+        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=forgejo&logoColor=black&label=Forks">
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/PyGrinder">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/PyGrinder?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <a href='https://coveralls.io/github/WenjieDu/PyGrinder'>
         <img alt='Coveralls report' src='https://img.shields.io/coverallsCoverage/github/WenjieDu/PyGrinder?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
@@ -42,15 +62,15 @@
         <img alt="Conda downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/conda_pygrinder_downloads.json">
     </a>
     <a href='https://pepy.tech/project/PyGrinder'>
         <img alt='PyPI downloads' src='https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pygrinder_downloads.json'>
     </a>
 </p>
 
-<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true' width='160' align='left' /></a>
+<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg' width='160' align='left' /></a>
 PyGrinder is a part of
 <a href="https://github.com/WenjieDu/PyPOTS">
 PyPOTS <img align="center" src="https://img.shields.io/github/stars/WenjieDu/PyPOTS?style=social">
 </a>
 (a Python toolbox for data mining on
 Partially-Observed Time Series), was called PyCorruptor and separated from PyPOTS for decoupling missingness-creating functionalities from
 learning algorithms.
@@ -62,15 +82,15 @@
 
 
 ## ❖ Usage Examples
 PyGrinder now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install pygrinder`, you may need to specify the channel with option `-c conda-forge`
 
-or install from PyPI:
+or install via PyPI:
 > pip install pygrinder
 
 or install from source code:
 > pip install `https://github.com/WenjieDu/PyGrinder/archive/main.zip`
 
 ```python
 import numpy as np
@@ -88,23 +108,27 @@
 # grind the dataset with MNAR pattern
 X_with_mnar_x_data = mnar_x(ts_dataset, offset=0.1)
 X_with_mnar_t_data = mnar_t(ts_dataset, cycle=20, pos = 10, scale = 3)
 ```
 
 
 ## ❖ Citing PyGrinder/PyPOTS
-
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use PyGrinder in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
+<p align="center">
+<a href="https://github.com/WenjieDu/PyPOTS">
+    <img src="https://pypots.com/figs/pypots_logos/Ecosystem/PyPOTS_Ecosystem_Pipeline.png" width="95%"/>
+</a>
+</p>
 
 ``` bibtex
-@article{du2023PyPOTS,
+@article{du2023pypots,
 title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
 author={Wenjie Du},
 year={2023},
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
@@ -112,28 +136,12 @@
 }
 ```
 
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
-or
-
-``` bibtex
-@inproceedings{du2023PyPOTS,
-title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
-booktitle={9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)},
-author={Wenjie Du},
-year={2023},
-url={https://arxiv.org/abs/2305.18811},
-}
-```
-
-> Wenjie Du. (2023).
-> PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
-> In *9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://arxiv.org/abs/2305.18811
-
 
 <details>
 <summary>🏠 Visits</summary>
 <img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FPyCorruptor&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+May+2022&edge_flat=false'>
 </details>
```

#### html2text {}

```diff
@@ -1,54 +1,61 @@
-_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_G_r_i_n_d_e_r___l_o_g_o___F_F_B_G_._s_v_g_?_s_a_n_i_t_i_z_e_=_t_r_u_e_]
-                       ********** WWeellccoommee ttoo PPyyGGrriinnddeerr **********
+Metadata-Version: 2.1 Name: pygrinder Version: 0.5 Summary: A Python toolkit
+for introducing missing values into datasets Home-page: https://github.com/
+WenjieDu/PyGrinder Download-URL: https://github.com/WenjieDu/PyGrinder/archive/
+main.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-
+Clause Keywords: data corruption,incomplete data,data
+mining,pypots,missingness,partially observed,irregular sampled,partially-
+observed time series,incomplete time series,missing data,missing values,pypots
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Education Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+BSD License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Description-Content-Type: text/markdown
+License-File: LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_G_r_i_n_d_e_r_/
+_l_o_g_o___F_F_B_G_._s_v_g_]
+                        ******** WWeellccoommee ttoo PPyyGGrriinnddeerr ********
 *
          a Python toolkit for grinding data beans into the incomplete
 *
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]_[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b
        _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e_ _C_l_i_m_a_t_e
 _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _r_e_p_o_r_t_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_a_r_X_i_v_ _D_O_I_]_[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]
                                _[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
-_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/
-_P_y_P_O_T_S___l_o_g_o___F_F_B_G_._s_v_g_?_s_a_n_i_t_i_z_e_=_t_r_u_e_]PyGrinder is a part of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/_P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a Python toolbox for
-data mining on Partially-Observed Time Series), was called PyCorruptor and
-separated from PyPOTS for decoupling missingness-creating functionalities from
-learning algorithms. In data analysis and modeling, sometimes we may need to
-corrupt the original data to achieve our goal, for instance, evaluating models'
-ability to reconstruct corrupted data or assessing the model's performance on
-only partially-observed data. PyGrinder is such a tool to help you corrupt your
-data, which provides several patterns to create missing values in the given
-data. ## â Usage Examples PyGrinder now is available on _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-_l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸
-Install it with `conda install pygrinder`, you may need to specify the channel
-with option `-c conda-forge` or install from PyPI: > pip install pygrinder or
-install from source code: > pip install `https://github.com/WenjieDu/PyGrinder/
-archive/main.zip` ```python import numpy as np from pygrinder import mcar,
-mar_logistic, mnar_x, mnar_t # given a time-series dataset with 128 samples,
-each sample with 10 time steps and 36 data features ts_dataset =
-np.random.randn(128, 10, 36) # grind the dataset with MCAR pattern, 10% missing
-probability, and using 0 to fill missing values X_with_mcar_data = mcar
-(ts_dataset, p=0.1) # grind the dataset with MAR pattern X_with_mar_data =
-mar_logistic(ts_dataset[:, 0, :], obs_rate=0.1, missing_rate=0.1) # grind the
-dataset with MNAR pattern X_with_mnar_x_data = mnar_x(ts_dataset, offset=0.1)
-X_with_mnar_t_data = mnar_t(ts_dataset, cycle=20, pos = 10, scale = 3) ``` ##
-â Citing PyGrinder/PyPOTS The paper introducing PyPOTS project is available
-on arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing
-to publish it in prestigious academic venues, e.g. JMLR (track for [Machine
-Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use
-PyGrinder in your work, please cite PyPOTS project as below and ðstar this
-repository to make others notice this library. ð¤ Thank you! ``` bibtex
-@article{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining on
-Partially-Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint=
-{2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]PyGrinder is a part
+of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/_P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a
+Python toolbox for data mining on Partially-Observed Time Series), was called
+PyCorruptor and separated from PyPOTS for decoupling missingness-creating
+functionalities from learning algorithms. In data analysis and modeling,
+sometimes we may need to corrupt the original data to achieve our goal, for
+instance, evaluating models' ability to reconstruct corrupted data or assessing
+the model's performance on only partially-observed data. PyGrinder is such a
+tool to help you corrupt your data, which provides several patterns to create
+missing values in the given data. ## â Usage Examples PyGrinder now is
+available on _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-
+_l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸ Install it with `conda install
+pygrinder`, you may need to specify the channel with option `-c conda-forge` or
+install via PyPI: > pip install pygrinder or install from source code: > pip
+install `https://github.com/WenjieDu/PyGrinder/archive/main.zip` ```python
+import numpy as np from pygrinder import mcar, mar_logistic, mnar_x, mnar_t #
+given a time-series dataset with 128 samples, each sample with 10 time steps
+and 36 data features ts_dataset = np.random.randn(128, 10, 36) # grind the
+dataset with MCAR pattern, 10% missing probability, and using 0 to fill missing
+values X_with_mcar_data = mcar(ts_dataset, p=0.1) # grind the dataset with MAR
+pattern X_with_mar_data = mar_logistic(ts_dataset[:, 0, :], obs_rate=0.1,
+missing_rate=0.1) # grind the dataset with MNAR pattern X_with_mnar_x_data =
+mnar_x(ts_dataset, offset=0.1) X_with_mnar_t_data = mnar_t(ts_dataset,
+cycle=20, pos = 10, scale = 3) ``` ## â Citing PyGrinder/PyPOTS The paper
+introducing PyPOTS project is available on arXiv at [this URL](https://
+arxiv.org/abs/2305.18811), and we are pursuing to publish it in prestigious
+academic venues, e.g. JMLR (track for [Machine Learning Open Source Software]
+(https://www.jmlr.org/mloss/)). If you use PyGrinder in your work, please cite
+PyPOTS project as below and ðstar this repository to make others notice this
+library. ð¤ Thank you!
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
+``` bibtex @article{du2023pypots, title={{PyPOTS: a Python toolbox for data
+mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
+eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
 arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du.
 (2023). > PyPOTS: a Python toolbox for data mining on Partially-Observed Time
-Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 or ``` bibtex
-@inproceedings{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining
-on Partially-Observed Time Series}}, booktitle={9th SIGKDD workshop on Mining
-and Learning from Time Series (MiLeTS'23)}, author={Wenjie Du}, year={2023},
-url={https://arxiv.org/abs/2305.18811}, } ``` > Wenjie Du. (2023). > PyPOTS: a
-Python toolbox for data mining on Partially-Observed Time Series. > In *9th
-SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://
-arxiv.org/abs/2305.18811 ð  Visits[https://hits.seeyoufarm.com/api/count/
-incr/
+Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FPyCorruptor&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+May+2022&edge_flat=false]
```

### Comparing `pygrinder-0.4/pygrinder/__init__.py` & `pygrinder-0.5/pygrinder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-__version__ = "0.4"
+__version__ = "0.5"
 
 from .missing_at_random import mar_logistic
 from .missing_completely_at_random import mcar, mcar_little_test
 from .missing_not_at_random import mnar_x, mnar_t
+from .randomly_drop_observations import rdo
 from .utils import (
     calc_missing_rate,
     masked_fill,
     fill_and_get_mask,
     fill_and_get_mask_torch,
     fill_and_get_mask_numpy,
 )
@@ -37,13 +38,14 @@
 __all__ = [
     "__version__",
     "mcar",
     "mcar_little_test",
     "mar_logistic",
     "mnar_x",
     "mnar_t",
+    "rdo",
     "calc_missing_rate",
     "masked_fill",
     "fill_and_get_mask",
     "fill_and_get_mask_torch",
     "fill_and_get_mask_numpy",
 ]
```

### Comparing `pygrinder-0.4/pygrinder/missing_at_random/mar_logistic.py` & `pygrinder-0.5/pygrinder/missing_at_random/mar_logistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,26 +98,26 @@
     First, a subset of the variables without missing values is randomly selected.
     Missing values will be introduced into the remaining variables according to a logistic model with random weights.
     This implementation is inspired by the tutorial
     https://rmisstastic.netlify.app/how-to/python/generate_html/how%20to%20generate%20missing%20values
 
     Parameters
     ----------
-    X : shape of [n_steps, n_features]
-        A time series data vector without any missing data.
+    X :
+        A time series data vector without any missing data. Shape of [n_steps, n_features].
 
     obs_rate :
         The proportion of variables without missing values that will be used for fitting the logistic masking model.
 
     missing_rate:
         The proportion of missing values to generate for variables which will have missing values.
 
     Returns
     -------
-    corrupted_X : array-like
+    corrupted_X :
         Original X with artificial missing values.
         Both originally-missing and artificially-missing values are left as NaN.
 
     """
     if isinstance(X, list):
         X = np.asarray(X)
```

### Comparing `pygrinder-0.4/pygrinder/missing_completely_at_random/little_test.py` & `pygrinder-0.5/pygrinder/missing_completely_at_random/little_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ----------
     X:
         Time series data containing missing values that should be in shape of [n_steps, n_features],
         i.e. have 2 dimensions.
 
     Returns
     -------
-    p_value: float
+    p_value:
         The p-value of a chi-square hypothesis test.
         Null hypothesis: the time series is missing completely at random (MCAR).
 
     """
 
     if isinstance(X, np.ndarray):
         assert len(X.shape) == 2
```

### Comparing `pygrinder-0.4/pygrinder/missing_completely_at_random/mcar.py` & `pygrinder-0.5/pygrinder/missing_completely_at_random/mcar.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 import torch
 
 
 def _mcar_numpy(
     X: np.ndarray,
     p: float,
 ) -> np.ndarray:
+    assert 0 < p < 1, f"p must be in range (0, 1), but got {p}"
+
     # clone X to ensure values of X out of this function not being affected
     X = np.copy(X)
     mcar_missing_mask = np.asarray(np.random.rand(np.prod(X.shape)) < p)
     mcar_missing_mask = mcar_missing_mask.reshape(X.shape)
     X[mcar_missing_mask] = np.nan  # mask values selected by mcar_missing_mask
     return X
 
 
 def _mcar_torch(
     X: torch.Tensor,
     p: float,
 ) -> torch.Tensor:
+    assert 0 < p < 1, f"p must be in range (0, 1), but got {p}"
+
     # clone X to ensure values of X out of this function not being affected
     X = torch.clone(X)
     mcar_missing_mask = torch.rand(X.shape) < p
     X[mcar_missing_mask] = torch.nan  # mask values selected by mcar_missing_mask
     return X
 
 
@@ -41,31 +45,33 @@
     """Create completely random missing values (MCAR case).
 
     Parameters
     ----------
     X :
         Data vector. If X has any missing values, they should be numpy.nan.
 
-    p : float, in (0,1),
+    p :
         The probability that values may be masked as missing completely at random.
         Note that the values are randomly selected no matter if they are originally missing or observed.
         If the selected values are originally missing, they will be kept as missing.
         If the selected values are originally observed, they will be masked as missing.
         Therefore, if the given X already contains missing data, the final missing rate in the output X could be
         in range [original_missing_rate, original_missing_rate+rate], but not strictly equal to
         `original_missing_rate+rate`. Because the selected values to be artificially masked out may be originally
         missing, and the masking operation on the values will do nothing.
 
     Returns
     -------
-    corrupted_X : array-like
+    corrupted_X :
         Original X with artificial missing values.
         Both originally-missing and artificially-missing values are left as NaN.
 
     """
+    assert 0 < p < 1, f"p must be in range (0, 1), but got {p}"
+
     if isinstance(X, list):
         X = np.asarray(X)
 
     if isinstance(X, np.ndarray):
         corrupted_X = _mcar_numpy(X, p)
     elif isinstance(X, torch.Tensor):
         corrupted_X = _mcar_torch(X, p)
```

### Comparing `pygrinder-0.4/pygrinder/missing_not_at_random/mnar_t.py` & `pygrinder-0.5/pygrinder/missing_not_at_random/mnar_t.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,19 +74,20 @@
 
     scale :
         The scale number to control the missing rate
 
 
     Returns
     -------
-    corrupted_X : array-like
+    corrupted_X :
         Original X with artificial missing values.
         Both originally-missing and artificially-missing values are left as NaN.
 
     """
+
     if isinstance(X, list):
         X = np.asarray(X)
 
     if isinstance(X, np.ndarray):
         corrupted_X = _mnar_t_numpy(X, cycle, pos, scale)
     elif isinstance(X, torch.Tensor):
         corrupted_X = _mnar_t_torch(X, cycle, pos, scale)
```

### Comparing `pygrinder-0.4/pygrinder/missing_not_at_random/mnar_x.py` & `pygrinder-0.5/pygrinder/missing_not_at_random/mnar_x.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     offset :
         the weight of standard deviation. In MNAR-x case, for each time series,
         the values larger than the mean of each time series plus offset*standard deviation will be missing
 
     Returns
     -------
-    corrupted_X : array-like
+    corrupted_X :
         Original X with artificial missing values.
         Both originally-missing and artificially-missing values are left as NaN.
     """
     if isinstance(X, list):
         X = np.asarray(X)
 
     if isinstance(X, np.ndarray):
```

### Comparing `pygrinder-0.4/pygrinder/utils.py` & `pygrinder-0.5/pygrinder/utils.py`

 * *Files identical despite different names*

### Comparing `pygrinder-0.4/pygrinder.egg-info/PKG-INFO` & `pygrinder-0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: pygrinder
-Version: 0.4
-Summary: A Python toolkit for introducing missing values into datasets
-Home-page: https://github.com/WenjieDu/PyGrinder
-Download-URL: https://github.com/WenjieDu/PyGrinder/archive/main.zip
-Author: Wenjie Du
-Author-email: wenjay.du@gmail.com
-License: BSD-3-Clause
-Keywords: data corruption,incomplete data,data mining,pypots,missingness,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values,pypots
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<a href='https://github.com/WenjieDu/PyGrinder'><img src='https://pypots.com/figs/pypots_logos/PyGrinder/logo_FFBG.svg' width='200' align='right' /></a>
 
-<a href='https://github.com/WenjieDu/PyGrinder'><img src='https://pypots.com/figs/pypots_logos/PyGrinder_logo_FFBG.svg?sanitize=true' width='200' align='right' /></a>
-
-<h2 align="center">Welcome to PyGrinder</h2>
+<h3 align="center">Welcome to PyGrinder</h3>
 
 *<p align='center'>a Python toolkit for grinding data beans into the incomplete</p>*
 
 <p align='center'>
     <a href='https://github.com/WenjieDu/PyGrinder'>
         <img alt='Python version' src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     </a>
@@ -37,18 +17,18 @@
     <a href="https://github.com/WenjieDu/PyPOTS/blob/main/README.md#-community">
         <img alt="Community" src="https://img.shields.io/badge/join_us-community!-C8A062">
     </a>
     <a href="https://github.com/WenjieDu/PyGrinder/graphs/contributors">
         <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/wenjiedu/pygrinder?color=D8E699&label=Contributors&logo=GitHub">
     </a>
     <a href="https://star-history.com/#wenjiedu/pygrinder">
-        <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/pygrinder?logo=Github&color=6BB392&label=Stars">
+        <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/pygrinder?logo=None&color=6BB392&label=%E2%98%85%20Stars">
     </a>
     <a href="https://github.com/WenjieDu/PyGrinder/network/members">
-        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=Github&color=91B821&label=Forks">
+        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=forgejo&logoColor=black&label=Forks">
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/PyGrinder">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/PyGrinder?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <a href='https://coveralls.io/github/WenjieDu/PyGrinder'>
         <img alt='Coveralls report' src='https://img.shields.io/coverallsCoverage/github/WenjieDu/PyGrinder?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
@@ -62,15 +42,15 @@
         <img alt="Conda downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/conda_pygrinder_downloads.json">
     </a>
     <a href='https://pepy.tech/project/PyGrinder'>
         <img alt='PyPI downloads' src='https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_pygrinder_downloads.json'>
     </a>
 </p>
 
-<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS_logo_FFBG.svg?sanitize=true' width='160' align='left' /></a>
+<a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg' width='160' align='left' /></a>
 PyGrinder is a part of
 <a href="https://github.com/WenjieDu/PyPOTS">
 PyPOTS <img align="center" src="https://img.shields.io/github/stars/WenjieDu/PyPOTS?style=social">
 </a>
 (a Python toolbox for data mining on
 Partially-Observed Time Series), was called PyCorruptor and separated from PyPOTS for decoupling missingness-creating functionalities from
 learning algorithms.
@@ -82,15 +62,15 @@
 
 
 ## ❖ Usage Examples
 PyGrinder now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install pygrinder`, you may need to specify the channel with option `-c conda-forge`
 
-or install from PyPI:
+or install via PyPI:
 > pip install pygrinder
 
 or install from source code:
 > pip install `https://github.com/WenjieDu/PyGrinder/archive/main.zip`
 
 ```python
 import numpy as np
@@ -108,23 +88,27 @@
 # grind the dataset with MNAR pattern
 X_with_mnar_x_data = mnar_x(ts_dataset, offset=0.1)
 X_with_mnar_t_data = mnar_t(ts_dataset, cycle=20, pos = 10, scale = 3)
 ```
 
 
 ## ❖ Citing PyGrinder/PyPOTS
-
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use PyGrinder in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
+<p align="center">
+<a href="https://github.com/WenjieDu/PyPOTS">
+    <img src="https://pypots.com/figs/pypots_logos/Ecosystem/PyPOTS_Ecosystem_Pipeline.png" width="95%"/>
+</a>
+</p>
 
 ``` bibtex
-@article{du2023PyPOTS,
+@article{du2023pypots,
 title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
 author={Wenjie Du},
 year={2023},
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
@@ -132,28 +116,12 @@
 }
 ```
 
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
-or
-
-``` bibtex
-@inproceedings{du2023PyPOTS,
-title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
-booktitle={9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)},
-author={Wenjie Du},
-year={2023},
-url={https://arxiv.org/abs/2305.18811},
-}
-```
-
-> Wenjie Du. (2023).
-> PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
-> In *9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://arxiv.org/abs/2305.18811
-
 
 <details>
 <summary>🏠 Visits</summary>
 <img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FPyCorruptor&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+May+2022&edge_flat=false'>
 </details>
```

#### html2text {}

```diff
@@ -1,67 +1,48 @@
-Metadata-Version: 2.1 Name: pygrinder Version: 0.4 Summary: A Python toolkit
-for introducing missing values into datasets Home-page: https://github.com/
-WenjieDu/PyGrinder Download-URL: https://github.com/WenjieDu/PyGrinder/archive/
-main.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-
-Clause Keywords: data corruption,incomplete data,data
-mining,pypots,missingness,partially observed,irregular sampled,partially-
-observed time series,incomplete time series,missing data,missing values,pypots
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Education Classifier:
-Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
-BSD License Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Description-Content-Type: text/markdown
-License-File: LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/
-_P_y_G_r_i_n_d_e_r___l_o_g_o___F_F_B_G_._s_v_g_?_s_a_n_i_t_i_z_e_=_t_r_u_e_]
-                       ********** WWeellccoommee ttoo PPyyGGrriinnddeerr **********
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_G_r_i_n_d_e_r_/_l_o_g_o___F_F_B_G_._s_v_g_]
+                        ******** WWeellccoommee ttoo PPyyGGrriinnddeerr ********
 *
          a Python toolkit for grinding data beans into the incomplete
 *
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]_[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b
        _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e_ _C_l_i_m_a_t_e
 _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _r_e_p_o_r_t_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_a_r_X_i_v_ _D_O_I_]_[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]
                                _[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
-_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/
-_P_y_P_O_T_S___l_o_g_o___F_F_B_G_._s_v_g_?_s_a_n_i_t_i_z_e_=_t_r_u_e_]PyGrinder is a part of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/_P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a Python toolbox for
-data mining on Partially-Observed Time Series), was called PyCorruptor and
-separated from PyPOTS for decoupling missingness-creating functionalities from
-learning algorithms. In data analysis and modeling, sometimes we may need to
-corrupt the original data to achieve our goal, for instance, evaluating models'
-ability to reconstruct corrupted data or assessing the model's performance on
-only partially-observed data. PyGrinder is such a tool to help you corrupt your
-data, which provides several patterns to create missing values in the given
-data. ## â Usage Examples PyGrinder now is available on _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-_l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸
-Install it with `conda install pygrinder`, you may need to specify the channel
-with option `-c conda-forge` or install from PyPI: > pip install pygrinder or
-install from source code: > pip install `https://github.com/WenjieDu/PyGrinder/
-archive/main.zip` ```python import numpy as np from pygrinder import mcar,
-mar_logistic, mnar_x, mnar_t # given a time-series dataset with 128 samples,
-each sample with 10 time steps and 36 data features ts_dataset =
-np.random.randn(128, 10, 36) # grind the dataset with MCAR pattern, 10% missing
-probability, and using 0 to fill missing values X_with_mcar_data = mcar
-(ts_dataset, p=0.1) # grind the dataset with MAR pattern X_with_mar_data =
-mar_logistic(ts_dataset[:, 0, :], obs_rate=0.1, missing_rate=0.1) # grind the
-dataset with MNAR pattern X_with_mnar_x_data = mnar_x(ts_dataset, offset=0.1)
-X_with_mnar_t_data = mnar_t(ts_dataset, cycle=20, pos = 10, scale = 3) ``` ##
-â Citing PyGrinder/PyPOTS The paper introducing PyPOTS project is available
-on arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we are pursuing
-to publish it in prestigious academic venues, e.g. JMLR (track for [Machine
-Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use
-PyGrinder in your work, please cite PyPOTS project as below and ðstar this
-repository to make others notice this library. ð¤ Thank you! ``` bibtex
-@article{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining on
-Partially-Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint=
-{2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]PyGrinder is a part
+of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/_P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a
+Python toolbox for data mining on Partially-Observed Time Series), was called
+PyCorruptor and separated from PyPOTS for decoupling missingness-creating
+functionalities from learning algorithms. In data analysis and modeling,
+sometimes we may need to corrupt the original data to achieve our goal, for
+instance, evaluating models' ability to reconstruct corrupted data or assessing
+the model's performance on only partially-observed data. PyGrinder is such a
+tool to help you corrupt your data, which provides several patterns to create
+missing values in the given data. ## â Usage Examples PyGrinder now is
+available on _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-
+_l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸ Install it with `conda install
+pygrinder`, you may need to specify the channel with option `-c conda-forge` or
+install via PyPI: > pip install pygrinder or install from source code: > pip
+install `https://github.com/WenjieDu/PyGrinder/archive/main.zip` ```python
+import numpy as np from pygrinder import mcar, mar_logistic, mnar_x, mnar_t #
+given a time-series dataset with 128 samples, each sample with 10 time steps
+and 36 data features ts_dataset = np.random.randn(128, 10, 36) # grind the
+dataset with MCAR pattern, 10% missing probability, and using 0 to fill missing
+values X_with_mcar_data = mcar(ts_dataset, p=0.1) # grind the dataset with MAR
+pattern X_with_mar_data = mar_logistic(ts_dataset[:, 0, :], obs_rate=0.1,
+missing_rate=0.1) # grind the dataset with MNAR pattern X_with_mnar_x_data =
+mnar_x(ts_dataset, offset=0.1) X_with_mnar_t_data = mnar_t(ts_dataset,
+cycle=20, pos = 10, scale = 3) ``` ## â Citing PyGrinder/PyPOTS The paper
+introducing PyPOTS project is available on arXiv at [this URL](https://
+arxiv.org/abs/2305.18811), and we are pursuing to publish it in prestigious
+academic venues, e.g. JMLR (track for [Machine Learning Open Source Software]
+(https://www.jmlr.org/mloss/)). If you use PyGrinder in your work, please cite
+PyPOTS project as below and ðstar this repository to make others notice this
+library. ð¤ Thank you!
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
+``` bibtex @article{du2023pypots, title={{PyPOTS: a Python toolbox for data
+mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
+eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
 arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du.
 (2023). > PyPOTS: a Python toolbox for data mining on Partially-Observed Time
-Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 or ``` bibtex
-@inproceedings{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining
-on Partially-Observed Time Series}}, booktitle={9th SIGKDD workshop on Mining
-and Learning from Time Series (MiLeTS'23)}, author={Wenjie Du}, year={2023},
-url={https://arxiv.org/abs/2305.18811}, } ``` > Wenjie Du. (2023). > PyPOTS: a
-Python toolbox for data mining on Partially-Observed Time Series. > In *9th
-SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://
-arxiv.org/abs/2305.18811 ð  Visits[https://hits.seeyoufarm.com/api/count/
-incr/
+Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FPyCorruptor&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+May+2022&edge_flat=false]
```

### Comparing `pygrinder-0.4/setup.py` & `pygrinder-0.5/setup.py`

 * *Files identical despite different names*

