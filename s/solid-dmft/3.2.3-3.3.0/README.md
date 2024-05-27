# Comparing `tmp/solid_dmft-3.2.3.tar.gz` & `tmp/solid_dmft-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solid_dmft-3.2.3.tar", last modified: Wed May 15 17:31:50 2024, max compression
+gzip compressed data, was "solid_dmft-3.3.0.tar", last modified: Mon May 27 14:47:43 2024, max compression
```

## Comparing `solid_dmft-3.2.3.tar` & `solid_dmft-3.3.0.tar`

### file list

```diff
@@ -1,56 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.298572 solid_dmft-3.2.3/
--rw-r--r--   0 root         (0) root         (0)    35147 2024-05-15 17:31:44.000000 solid_dmft-3.2.3/COPYING.txt
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-15 17:31:44.000000 solid_dmft-3.2.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-15 17:31:47.000000 solid_dmft-3.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3591 2024-05-15 17:31:50.298572 solid_dmft-3.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2796 2024-05-15 17:31:44.000000 solid_dmft-3.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)      937 2024-05-15 17:31:47.000000 solid_dmft-3.2.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.290572 solid_dmft-3.2.3/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.290572 solid_dmft-3.2.3/python/solid_dmft/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14897 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/csc_flow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.294572 solid_dmft-3.2.3/python/solid_dmft/dft_managers/
--rw-r--r--   0 root         (0) root         (0)     1146 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dft_managers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5494 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dft_managers/mpi_helpers.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dft_managers/qe_manager.py
--rw-r--r--   0 root         (0) root         (0)     7980 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dft_managers/vasp_manager.py
--rwxr-xr-x   0 root         (0) root         (0)    36937 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_cycle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.298572 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/
--rw-r--r--   0 root         (0) root         (0)     1179 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6014 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/afm_mapping.py
--rw-r--r--   0 root         (0) root         (0)    12110 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/convergence.py
--rw-r--r--   0 root         (0) root         (0)     8953 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/formatter.py
--rw-r--r--   0 root         (0) root         (0)    10088 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/greens_functions_mixer.py
--rwxr-xr-x   0 root         (0) root         (0)    22700 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/initial_self_energies.py
--rw-r--r--   0 root         (0) root         (0)    24491 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/interaction_hamiltonian.py
--rw-r--r--   0 root         (0) root         (0)     2068 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/legendre_filter.py
--rwxr-xr-x   0 root         (0) root         (0)    18548 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
--rw-r--r--   0 root         (0) root         (0)     1316 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/matheval.py
--rw-r--r--   0 root         (0) root         (0)    24521 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/observables.py
--rw-r--r--   0 root         (0) root         (0)     7298 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/results_to_archive.py
--rwxr-xr-x   0 root         (0) root         (0)    57627 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/dmft_tools/solver.py
--rw-r--r--   0 root         (0) root         (0)     5064 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.298572 solid_dmft-3.2.3/python/solid_dmft/postprocessing/
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/postprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9176 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py
--rw-r--r--   0 root         (0) root         (0)    16115 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
--rw-r--r--   0 root         (0) root         (0)    11337 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/postprocessing/maxent_gf_imp.py
--rw-r--r--   0 root         (0) root         (0)    12338 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/postprocessing/maxent_gf_latt.py
--rw-r--r--   0 root         (0) root         (0)    17196 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/postprocessing/maxent_sigma.py
--rw-r--r--   0 root         (0) root         (0)    38834 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/postprocessing/plot_correlated_bands.py
--rwxr-xr-x   0 root         (0) root         (0)    71594 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/read_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.298572 solid_dmft-3.2.3/python/solid_dmft/util/
--rw-r--r--   0 root         (0) root         (0)     1178 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6808 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/util/symmetrize_gamma_file.py
--rw-r--r--   0 root         (0) root         (0)     4940 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/util/update_dmft_config.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/util/update_results_h5.py
--rw-r--r--   0 root         (0) root         (0)     4727 2024-05-15 17:31:45.000000 solid_dmft-3.2.3/python/solid_dmft/util/write_kslice_to_h5.py
--rw-r--r--   0 root         (0) root         (0)     1472 2024-05-15 17:31:47.000000 solid_dmft-3.2.3/python/solid_dmft/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 17:31:50.298572 solid_dmft-3.2.3/python/solid_dmft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3591 2024-05-15 17:31:50.000000 solid_dmft-3.2.3/python/solid_dmft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1869 2024-05-15 17:31:50.000000 solid_dmft-3.2.3/python/solid_dmft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 17:31:50.000000 solid_dmft-3.2.3/python/solid_dmft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-15 17:31:50.000000 solid_dmft-3.2.3/python/solid_dmft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-15 17:31:50.000000 solid_dmft-3.2.3/python/solid_dmft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-15 17:31:50.000000 solid_dmft-3.2.3/python/solid_dmft.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 17:31:50.302572 solid_dmft-3.2.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.706831 solid_dmft-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)    35147 2024-05-27 14:47:37.000000 solid_dmft-3.3.0/COPYING.txt
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-27 14:47:37.000000 solid_dmft-3.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-27 14:47:42.000000 solid_dmft-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3597 2024-05-27 14:47:43.706831 solid_dmft-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-27 14:47:37.000000 solid_dmft-3.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      943 2024-05-27 14:47:42.000000 solid_dmft-3.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.694831 solid_dmft-3.3.0/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.698831 solid_dmft-3.3.0/python/solid_dmft/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14909 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/csc_flow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.698831 solid_dmft-3.3.0/python/solid_dmft/dft_managers/
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dft_managers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5494 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dft_managers/mpi_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dft_managers/qe_manager.py
+-rw-r--r--   0 root         (0) root         (0)     7980 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dft_managers/vasp_manager.py
+-rwxr-xr-x   0 root         (0) root         (0)    41642 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_cycle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.702831 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6110 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/afm_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    12069 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/convergence.py
+-rw-r--r--   0 root         (0) root         (0)     8807 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/formatter.py
+-rw-r--r--   0 root         (0) root         (0)     9129 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/greens_functions_mixer.py
+-rwxr-xr-x   0 root         (0) root         (0)    29436 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/initial_self_energies.py
+-rw-r--r--   0 root         (0) root         (0)    27174 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/interaction_hamiltonian.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/legendre_filter.py
+-rwxr-xr-x   0 root         (0) root         (0)    17953 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/matheval.py
+-rw-r--r--   0 root         (0) root         (0)    24102 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/observables.py
+-rw-r--r--   0 root         (0) root         (0)     8713 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/results_to_archive.py
+-rwxr-xr-x   0 root         (0) root         (0)    72986 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/dmft_tools/solver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.702831 solid_dmft-3.3.0/python/solid_dmft/gw_embedding/
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/gw_embedding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17156 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/gw_embedding/bdft_converter.py
+-rw-r--r--   0 root         (0) root         (0)    23578 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/gw_embedding/gw_flow.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/gw_embedding/iaft.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/gw_embedding/qp_evs_to_eig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.702831 solid_dmft-3.3.0/python/solid_dmft/io_tools/
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/io_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/io_tools/dict_to_h5.py
+-rw-r--r--   0 root         (0) root         (0)     9056 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/io_tools/postproc_toml_dict.py
+-rw-r--r--   0 root         (0) root         (0)     7064 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/io_tools/verify_input_params.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.706831 solid_dmft-3.3.0/python/solid_dmft/postprocessing/
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9246 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py
+-rw-r--r--   0 root         (0) root         (0)    16115 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/maxent_gf_imp.py
+-rw-r--r--   0 root         (0) root         (0)    12338 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/maxent_gf_latt.py
+-rw-r--r--   0 root         (0) root         (0)    17783 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/maxent_sigma.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/pade_sigma.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/postprocessing/plot_correlated_bands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.706831 solid_dmft-3.3.0/python/solid_dmft/util/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/util/symmetrize_gamma_file.py
+-rw-r--r--   0 root         (0) root         (0)     4727 2024-05-27 14:47:38.000000 solid_dmft-3.3.0/python/solid_dmft/util/write_kslice_to_h5.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-05-27 14:47:42.000000 solid_dmft-3.3.0/python/solid_dmft/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:47:43.706831 solid_dmft-3.3.0/python/solid_dmft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3597 2024-05-27 14:47:43.000000 solid_dmft-3.3.0/python/solid_dmft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-05-27 14:47:43.000000 solid_dmft-3.3.0/python/solid_dmft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 14:47:43.000000 solid_dmft-3.3.0/python/solid_dmft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-27 14:47:43.000000 solid_dmft-3.3.0/python/solid_dmft.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-27 14:47:43.000000 solid_dmft-3.3.0/python/solid_dmft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-27 14:47:43.000000 solid_dmft-3.3.0/python/solid_dmft.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 14:47:43.706831 solid_dmft-3.3.0/setup.cfg
```

### Comparing `solid_dmft-3.2.3/COPYING.txt` & `solid_dmft-3.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/LICENSE.txt` & `solid_dmft-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/PKG-INFO` & `solid_dmft-3.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solid_dmft
-Version: 3.2.3
+Version: 3.3.0
 Summary: solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library
 Author-email: Alexander Hampel <ahampel@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/solid_dmft
 Project-URL: Bug Tracker, https://github.com/triqs/solid_dmft/issues
 Project-URL: Paper, https://doi.org/10.21105/joss.04623
 Keywords: DMFT,DFT,triqs
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: COPYING.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: pytest
+Requires-Dist: scikit-image
 
 ![logo_soliDMFT](https://raw.githubusercontent.com/triqs/solid_dmft/unstable/doc/logos/logo_solid_dmft.png)
 
 ![CI](https://github.com/triqs/solid_dmft/actions/workflows/build.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/solid_dmft.svg)](https://badge.fury.io/py/solid_dmft)
 [![status](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922/status.svg)](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922)
```

### Comparing `solid_dmft-3.2.3/README.md` & `solid_dmft-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/pyproject.toml` & `solid_dmft-3.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 
 [project]
 name = "solid_dmft"
-version = "3.2.3"
+version = "3.3.0"
 authors = [
   { name="Alexander Hampel", email="ahampel@flatironinstitute.org" }
 ]
 description = "solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library"
 readme = "README.md"
 keywords = ["DMFT", "DFT", "triqs"]
 requires-python = ">=3.7"
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
     "scipy",
-    "pytest"
+    "scikit-image"
 ]
 
 [project.urls]
 "Homepage" = "https://triqs.github.io/solid_dmft"
 "Bug Tracker" = "https://github.com/triqs/solid_dmft/issues"
 "Paper" = "https://doi.org/10.21105/joss.04623"
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/__init__.py` & `solid_dmft-3.3.0/python/solid_dmft/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/csc_flow.py` & `solid_dmft-3.3.0/python/solid_dmft/csc_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,26 +40,26 @@
 from triqs_dft_tools.converters.plovasp.vaspio import VaspData
 import triqs_dft_tools.converters.plovasp.converter as plo_converter
 
 from solid_dmft.dmft_cycle import dmft_cycle
 from solid_dmft.dft_managers import vasp_manager as vasp
 from solid_dmft.dft_managers import qe_manager as qe
 
-def _run_plo_converter(general_params):
+def _run_plo_converter(general_params, dft_params):
     if not mpi.is_master_node():
         return
 
     # Checks for plo file for projectors
-    if not os.path.exists(general_params['plo_cfg']):
+    if not os.path.exists(dft_params['plo_cfg']):
         print('*** Input PLO config file not found! '
-              + 'I was looking for {} ***'.format(general_params['plo_cfg']))
+              + 'I was looking for {} ***'.format(dft_params['plo_cfg']))
         mpi.MPI.COMM_WORLD.Abort(1)
 
     # Runs plo converter
-    plo_converter.generate_and_output_as_text(general_params['plo_cfg'], vasp_dir='./')
+    plo_converter.generate_and_output_as_text(dft_params['plo_cfg'], vasp_dir='./')
     # Writes new H(k) to h5 archive
     converter = VaspConverter(filename=general_params['seedname'])
     converter.convert_dft_input()
 
 def _run_wannier90(general_params, dft_params):
     if not mpi.is_master_node():
         return
@@ -186,15 +186,15 @@
             vasp_process_id = vasp.run_initial_scf(dft_params['n_cores'], dft_params['dft_exec'],
                                                    dft_params['mpi_env'])
         else:
             vasp_process_id = None
             vasp.run_charge_update()
 
         if dft_params['projector_type'] == 'plo':
-            _run_plo_converter(general_params)
+            _run_plo_converter(general_params, dft_params)
             irred_indices = None
         elif dft_params['projector_type'] == 'w90':
             _run_wannier90(general_params, dft_params)
             mpi.barrier()
             _run_w90converter(general_params['seedname'], dft_params['w90_tolerance'])
             mpi.barrier()
             kpts = None
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dft_managers/__init__.py` & `solid_dmft-3.3.0/python/solid_dmft/dft_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dft_managers/mpi_helpers.py` & `solid_dmft-3.3.0/python/solid_dmft/dft_managers/mpi_helpers.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dft_managers/qe_manager.py` & `solid_dmft-3.3.0/python/solid_dmft/dft_managers/qe_manager.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dft_managers/vasp_manager.py` & `solid_dmft-3.3.0/python/solid_dmft/dft_managers/vasp_manager.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_cycle.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_cycle.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 ################################################################################
 """
 main DMFT cycle, DMFT step, and helper functions
 """
 
 
 # system
-import os
 from copy import deepcopy
 from timeit import default_timer as timer
 import numpy as np
 
 # triqs
 from triqs.operators.util.observables import S_op, N_op
 from triqs.version import git_hash as triqs_hash
 from triqs.version import version as triqs_version
 from h5 import HDFArchive
 import triqs.utility.mpi as mpi
-from triqs.gf import Gf, make_hermitian, MeshReFreq, MeshImFreq
-from triqs.gf.tools import inverse
+from triqs.operators import c_dag, c, Operator
+from triqs.gf import make_hermitian, fit_hermitian_tail, MeshReFreq, MeshImFreq, make_gf_from_fourier, iOmega_n
+from triqs.gf.tools import inverse, make_zero_tail
 from triqs_dft_tools.sumk_dft import SumkDFT
 
 # own modules
 from solid_dmft.version import solid_dmft_hash
 from solid_dmft.version import version as solid_dmft_version
 from solid_dmft.dmft_tools.observables import (calc_dft_kin_en, add_dmft_observables, calc_bandcorr_man, write_obs,
                                          add_dft_values_as_zeroth_iteration, write_header_to_file, prep_observables)
@@ -52,17 +52,60 @@
 from solid_dmft.dmft_tools import formatter
 from solid_dmft.dmft_tools import interaction_hamiltonian
 from solid_dmft.dmft_tools import results_to_archive
 from solid_dmft.dmft_tools import afm_mapping
 from solid_dmft.dmft_tools import manipulate_chemical_potential as manipulate_mu
 from solid_dmft.dmft_tools import initial_self_energies as initial_sigma
 from solid_dmft.dmft_tools import greens_functions_mixer as gf_mixer
+from solid_dmft.io_tools import verify_input_params, dict_to_h5
 
+def _extract_quantity_per_inequiv(param_name, n_inequiv_shells, general_params):
+    """
+    For quantities that can be different for each inequivalent shell, this
+    function checks if the quantity is a single value or a list of the correct
+    length. If just a single value is given, this value is applied to each shell.
+
+    Parameters
+    ----------
+    param_name : str
+        name of the parameter to be checked
+    n_inequiv_shells : int
+        number of inequivalent shells
+    general_params : dict
+        general parameters as a dict
+
+    Returns
+    -------
+    general_params : dict
+        updated general parameters as a dict
+
+    """
+
+
+    def formatter(value):
+        if isinstance(value, float):
+            return '{:.2f}'.format(value)
+        return str(value)
+
+    param = general_params[param_name]
+    if not isinstance(param, list):
+        mpi.report('Assuming {} = '.format(param_name)
+                + '{} for all correlated shells'.format(formatter(param)))
+        general_params[param_name] = [param] * n_inequiv_shells
+    elif len(param) == n_inequiv_shells:
+        mpi.report(f'{param_name} list for correlated shells: '
+                   + ', '.join([formatter(p) for p in param]))
+    else:
+        raise IndexError(f'{param_name} must be list of length '
+                         f'n_inequiv_shells={n_inequiv_shells} '
+                         'or single value but is ' + str(general_params[param_name]))
+
+    return general_params
 
-def _determine_block_structure(sum_k, general_params, advanced_params):
+def _determine_block_structure(sum_k, general_params, advanced_params, solver_type_per_imp, dens_mat):
     """
     Determines block structrure and degenerate deg_shells
     computes first DFT density matrix to determine block structure and changes
     the density matrix according to needs i.e. magnetic calculations, or keep
     off-diag elements
 
     Parameters
@@ -70,101 +113,90 @@
     sum_k : SumK Object instances
 
     Returns
     -------
     sum_k : SumK Object instances
         updated sum_k Object
     """
-    mpi.report('\n *** determination of block structure ***')
+    mpi.report('\n *** Determination of block structure ***')
 
-    # this returns a list of dicts (one entry for each corr shell)
-    # the dict contains one entry for up and one for down
-    # each entry is a square complex numpy matrix with dim=corr_shell['dim']
-    zero_Sigma = [sum_k.block_structure.create_gf(ish=iineq, gf_function=Gf, mesh=sum_k.mesh)
-                  for iineq in range(sum_k.n_inequiv_shells)]
-    sum_k.put_Sigma(zero_Sigma)
-    if general_params['solver_type'] in ['ftps']:
-        G_loc_all = sum_k.extract_G_loc(broadening=general_params['eta'], transform_to_solver_blocks=False)
-        dens_mat = [G_loc_all[iineq].density() for iineq in range(sum_k.n_inequiv_shells)]
-    else:
-        dens_mat = sum_k.density_matrix(method='using_gf')
-
-    original_dens_mat = deepcopy(dens_mat)
+    # Adds spin degeneracies if not spin-orbit coupled
+    if sum_k.SO == 0:
+        sum_k.block_structure.deg_shells = [[['up_0', 'down_0']] for _ in range(sum_k.n_inequiv_shells)]
+
+    # Evaluates degeneracies for ftps
+    imp_ftps = [i for i, s in enumerate(solver_type_per_imp) if s == 'ftps']
+    if imp_ftps:
+        mock_sumk = deepcopy(sum_k)
+        mock_sumk.analyse_block_structure(dm=dens_mat, threshold=general_params['block_threshold'], include_shells=imp_ftps)
+        deg_orbs_ftps = [mock_sumk.deg_shells[icrsh] if icrsh in imp_ftps else None
+                         for icrsh in range(sum_k.n_inequiv_shells)]
+        mpi.report('Block structure written to "deg_orbs_ftps":')
+        mpi.report(deg_orbs_ftps)
+    else:
+        deg_orbs_ftps = None
+
+    # Only removes the off-diagonal terms for the selected impurities
+    imp_to_analyze = [i for i, offdiag in enumerate(general_params['enforce_off_diag']) if not offdiag]
+    mpi.report('using 1-particle density matrix and Hloc (atomic levels) to determine the block structure')
+    sum_k.analyse_block_structure(dm=dens_mat, threshold=general_params['block_threshold'], include_shells=imp_to_analyze)
 
-    # for certain systems it is needed to keep off diag elements
-    # this enforces to use the full corr subspace matrix
-    solver_struct_ftps = None
-    if general_params['enforce_off_diag'] or general_params['solver_type'] in ['ftps', 'hartree']:
-        if general_params['solver_type'] in ['ftps']:
-            # first round to determine real blockstructure
-            mock_sumk = deepcopy(sum_k)
-            mock_sumk.analyse_block_structure(dm=dens_mat, threshold=general_params['block_threshold'])
-            solver_struct_ftps = [None] * sum_k.n_inequiv_shells
-            for icrsh in range(sum_k.n_inequiv_shells):
-                solver_struct_ftps[icrsh] = mock_sumk.deg_shells[icrsh]
-            mpi.report('Block structure written to "solver_struct_ftps":')
-            mpi.report(solver_struct_ftps)
-
-        mpi.report('enforcing off-diagonal elements in block structure finder')
-        for dens_mat_per_imp in dens_mat:
-            for dens_mat_per_block in dens_mat_per_imp.values():
-                dens_mat_per_block += 2 * general_params['block_threshold']
-
-    if not general_params['enforce_off_diag'] and general_params['block_suppress_orbital_symm']:
-        mpi.report('removing orbital symmetries in block structure finder')
-        for dens_mat_per_imp in dens_mat:
-            for dens_mat_per_block in dens_mat_per_imp.values():
-                dens_mat_per_block += 2*np.diag(np.arange(dens_mat_per_block.shape[0]))
-
-    mpi.report('using 1-particle density matrix and Hloc (atomic levels) to '
-               'determine the block structure')
-    sum_k.analyse_block_structure(dm=dens_mat, threshold=general_params['block_threshold'])
-
-    if advanced_params['pick_solver_struct'] != 'none':
+    # Applies manual selection of the solver struct
+    if any(s is not None for s in advanced_params['pick_solver_struct']):
         mpi.report('selecting subset of orbital space for gf_struct_solver from input:')
-        mpi.report(advanced_params['pick_solver_struct'])
+        mpi.report(advanced_params['pick_solver_struct'][icrsh])
         sum_k.block_structure.pick_gf_struct_solver(advanced_params['pick_solver_struct'])
 
     # Applies the manual mapping to each inequivalent shell
-    if advanced_params['map_solver_struct'] != 'none':
+    if any(s is not None for s in advanced_params['map_solver_struct']):
         sum_k.block_structure.map_gf_struct_solver(advanced_params['map_solver_struct'])
-        if advanced_params['mapped_solver_struct_degeneracies'] != 'none':
+        if any(s is not None for s in advanced_params['mapped_solver_struct_degeneracies']):
             sum_k.block_structure.deg_shells = advanced_params['mapped_solver_struct_degeneracies']
 
     # if we want to do a magnetic calculation we need to lift up/down degeneracy
     if general_params['magnetic'] and sum_k.SO == 0:
-        mpi.report('magnetic calculation: removing the spin degeneracy from the block structure')
-
+        mpi.report('Magnetic calculation: removing the spin degeneracy from the block structure')
         for icrsh, deg_shells_site in enumerate(sum_k.block_structure.deg_shells):
             deg_shell_mag = []
             # find degenerate orbitals that do not simply connect different spin channels
             for deg_orbs in deg_shells_site:
                 for spin in ['up', 'down']:
                     # create a list of all up / down orbitals
                     deg = [orb for orb in deg_orbs if spin in orb]
                     # if longer than one than we have two deg orbitals also in a magnetic calculation
                     if len(deg) > 1:
                         deg_shell_mag.append(deg)
             sum_k.block_structure.deg_shells[icrsh] = deg_shell_mag
-
     # for SOC we remove all degeneracies
-    elif general_params['magnetic'] and sum_k.SO == 1:
-        sum_k.block_structure.deg_shells = [[] for icrsh in range(len(sum_k.block_structure.deg_shells))]
+    elif sum_k.SO == 1:
+        sum_k.block_structure.deg_shells = [[] for _ in range(sum_k.n_inequiv_shells)]
 
-    return sum_k, original_dens_mat, solver_struct_ftps
+    return sum_k, deg_orbs_ftps
 
 
 def _calculate_rotation_matrix(general_params, sum_k):
     """
     Applies rotation matrix to make the DMFT calculations easier for the solver.
     Possible are rotations diagonalizing either the local Hamiltonian or the
     density. Diagonalizing the density has not proven really helpful but
     diagonalizing the local Hamiltonian has.
     Note that the interaction Hamiltonian has to be rotated if it is not fully
     orbital-gauge invariant (only the Kanamori fulfills that).
+
+    Parameters
+    ----------
+    general_params : dict
+        general parameters as a dict
+    sum_k : SumkDFT object
+        Sumk Object
+
+    Returns
+    -------
+    sum_k : SumkDFT Object
+        updated Sumk object with the new rotation matrices
     """
 
     # Extracts new rotation matrices from density_mat or local Hamiltonian
     if general_params['set_rot'] == 'hloc':
         q_diag = sum_k.eff_atomic_levels()
     elif general_params['set_rot'] == 'den':
         q_diag = sum_k.density_matrix(method='using_gf')
@@ -192,96 +224,93 @@
     # Prints matrices
     mpi.report('\nNew rotation matrices')
     formatter.print_rotation_matrix(sum_k)
 
     return sum_k
 
 
-def _chi_setup(sum_k, general_params, solver_params):
+def _chi_setup(sum_k, solver_params, map_imp_solver):
     """
 
     Parameters
     ----------
     sum_k : SumkDFT object
         Sumk object with the information about the correct block structure
-    general_paramters: general params dict
     solver_params: solver params dict
 
     Returns
     -------
-    solver_params :  dict
-        solver_paramters for the QMC solver
-    Op_list : list of one-particle operators to measure per impurity
+    ops_chi_measurement : list of one-particle operators to measure per impurity
     """
 
-    if general_params['measure_chi'] == 'SzSz':
-        mpi.report('\nSetting up Chi(S_z(tau),S_z(0)) measurement')
-    elif general_params['measure_chi'] == 'NN':
-        mpi.report('\nSetting up Chi(n(tau),n(0)) measurement')
-
-    Op_list = [None] * sum_k.n_inequiv_shells
+    ops_chi_measure = [None] * sum_k.n_inequiv_shells
 
     for icrsh in range(sum_k.n_inequiv_shells):
+        isolv = map_imp_solver[icrsh]
+        if 'measure_chi' not in solver_params[isolv] or solver_params[isolv]['measure_chi'] is None:
+            continue
+
         n_orb = sum_k.corr_shells[icrsh]['dim']
-        orb_names = list(range(n_orb))
+        if solver_params[isolv]['measure_chi'] == 'SzSz':
+            mpi.report(f'\nImp {icrsh} with solver #{isolv}: Setting up Chi(S_z(tau),S_z(0)) measurement')
 
-        if general_params['measure_chi'] == 'SzSz':
-            Op_list[icrsh] = S_op('z',
-                                  spin_names=sum_k.spin_block_names[sum_k.SO],
-                                  n_orb=n_orb,
-                                  map_operator_structure=sum_k.sumk_to_solver[icrsh])
-        elif general_params['measure_chi'] == 'NN':
-            Op_list[icrsh] = N_op(spin_names=sum_k.spin_block_names[sum_k.SO],
-                                  n_orb=n_orb,
-                                  map_operator_structure=sum_k.sumk_to_solver[icrsh])
+            ops_chi_measure[icrsh] = S_op('z', spin_names=sum_k.spin_block_names[sum_k.SO],
+                                          n_orb=n_orb, map_operator_structure=sum_k.sumk_to_solver[icrsh])
+        elif solver_params[isolv]['measure_chi'] == 'NN':
+            mpi.report(f'\nImp {icrsh} with solver #{isolv}: Setting up Chi(n(tau),n(0)) measurement')
 
-    solver_params['measure_O_tau_min_ins'] = general_params['measure_chi_insertions']
+            ops_chi_measure[icrsh] = N_op(spin_names=sum_k.spin_block_names[sum_k.SO],
+                                          n_orb=n_orb, map_operator_structure=sum_k.sumk_to_solver[icrsh])
 
-    return solver_params, Op_list
+    return ops_chi_measure
 
 
 def dmft_cycle(general_params, solver_params, advanced_params, dft_params,
-               n_iter, dft_irred_kpt_indices=None, dft_energy=None):
+               gw_params, n_iter, dft_irred_kpt_indices=None, dft_energy=None):
     """
     main dmft cycle that works for one shot and CSC equally
 
     Parameters
     ----------
     general_params : dict
         general parameters as a dict
     solver_params : dict
         solver parameters as a dict
     advanced_params : dict
         advanced parameters as a dict
-    observables : dict
-        current observable array for calculation
+    dft_params : dict
+        dft parameters as a dict
+    gw_params : dict
+        gw parameters as a dict
     n_iter : int
         number of iterations to be executed
     dft_irred_kpt_indices: iterable of int
         If given, writes density correction for csc calculations only for
         irreducible kpoints
 
     Returns
     ---------
     observables : dict
         updated observable array for calculation
     """
 
-    # create Sumk object
-    # TODO: use_dft_blocks=True yields inconsistent number of blocks!
-
-    # first we have to determine the mesh
-    if general_params['solver_type'] in ['ftps']:
-        sumk_mesh = MeshReFreq(window=general_params['w_range'],
-                               n_w=general_params['n_w'])
-    else:
+    # Creates real- or imaginary-frequency mesh to store Green functions on
+    if general_params['beta'] is not None:
+        mpi.report('Running solid_dmft on imag-freq grid because "general.beta" specified')
         sumk_mesh = MeshImFreq(beta=general_params['beta'],
                                S='Fermion',
                                n_iw=general_params['n_iw'])
+        broadening = None
+    else:
+        mpi.report('Running solid_dmft on real-freq grid because "general.beta" not specified')
+        sumk_mesh = MeshReFreq(window=general_params['w_range'],
+                               n_w=general_params['n_w'])
+        broadening = general_params['eta']
 
+    # Creates SumkDFT object
     sum_k = SumkDFT(hdf_file=general_params['jobname']+'/'+general_params['seedname']+'.h5',
                     mesh=sumk_mesh, use_dft_blocks=False, h_field=general_params['h_field'])
 
     iteration_offset = 0
 
     # determine chemical potential for bare DFT sum_k object
     if mpi.is_master_node():
@@ -309,211 +338,222 @@
         print('#'*80, '\n')
     else:
         archive = None
 
     iteration_offset = mpi.bcast(iteration_offset)
     sum_k.chemical_potential = mpi.bcast(sum_k.chemical_potential)
 
-    # Incompatabilities for SO coupling
-    if sum_k.SO == 1:
-        if not general_params['csc'] and general_params['magnetic'] and general_params['afm_order']:
-            raise ValueError('AFM order not supported with SO coupling')
-
-    # need to set sigma immediately here, otherwise mesh in unclear for sumK
-    # Initializes empty Sigma for calculation of DFT density even if block structure changes later
-    zero_Sigma = [sum_k.block_structure.create_gf(ish=iineq, gf_function=Gf, mesh=sum_k.mesh)
-                  for iineq in range(sum_k.n_inequiv_shells)]
-    sum_k.put_Sigma(zero_Sigma)
+    # Checks the general parameters that are impurity-dependent and ensures they are a list
+    mpi.report('Checking parameters that are impurity-dependent')
+    for key in ['U', 'J', 'U_prime', 'ratio_F4_F2', 'h_int_type', 'enforce_off_diag', 'dc_type']:
+        general_params = _extract_quantity_per_inequiv(key, sum_k.n_inequiv_shells, general_params)
+    # Same for advanced params
+    for key in ['dc_U', 'dc_J', 'dc_fixed_occ', 'map_solver_struct', 'pick_solver_struct', 'mapped_solver_struct_degeneracies']:
+        advanced_params = _extract_quantity_per_inequiv(key, sum_k.n_inequiv_shells, advanced_params)
+
+    # Checks that all impurities have an associated solver
+    # and creates a map between impurity index and solver index
+    if len(solver_params) == 1 and solver_params[0]['idx_impurities'] is None:
+        map_imp_solver = [0] * sum_k.n_inequiv_shells
+    else:
+        all_idx_imp = [i for entry in solver_params for i in entry['idx_impurities']]
+        if sorted(all_idx_imp) != list(range(sum_k.n_inequiv_shells)):
+            raise ValueError('All impurities must be listed exactly once in solver.idx_impurities'
+                             f'but instead got {all_idx_imp}')
+
+        map_imp_solver = []
+        for iineq in range(sum_k.n_inequiv_shells):
+            for isolver, entry in enumerate(solver_params):
+                if iineq in entry['idx_impurities']:
+                    map_imp_solver.append(isolver)
+                    break
+    solver_type_per_imp = [solver_params[map_imp_solver[iineq]]['type'] for iineq in range(sum_k.n_inequiv_shells)]
+    mpi.report(f'\nSolver type per impurity: {solver_type_per_imp}')
+
+    # Checks all parameters that need to be checked against info in SumkDFT object
+    verify_input_params.verify_h5_dependent(sum_k, solver_type_per_imp, general_params)
 
     # Initializes chemical potential with mu_initial_guess if this is the first iteration
-    if general_params['mu_initial_guess'] != 'none' and iteration_offset == 0:
-            sum_k.chemical_potential = general_params['mu_initial_guess']
-            mpi.report('\ninitial chemical potential set to {:.3f} eV\n'.format(sum_k.chemical_potential))
-
-    if general_params['solver_type'] in ['ftps']:
-        dft_mu = sum_k.calc_mu(precision=general_params['prec_mu'],
-                               broadening=general_params['eta'])
-    else:
-        dft_mu = sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'])
+    if general_params['mu_initial_guess'] is not None and iteration_offset == 0:
+        sum_k.chemical_potential = general_params['mu_initial_guess']
+        mpi.report('\nInitial chemical potential set to {:.3f} eV\n'.format(sum_k.chemical_potential))
+
+    dft_mu = sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'],
+                           broadening=broadening)
 
     # calculate E_kin_dft for one shot calculations
     if not general_params['csc'] and general_params['calc_energies']:
         E_kin_dft = calc_dft_kin_en(general_params, sum_k, dft_mu)
     else:
         E_kin_dft = None
 
     # check for previous broyden data oterhwise initialize it:
     if mpi.is_master_node() and  general_params['g0_mix_type'] == 'broyden':
         if not 'broyler' in archive['DMFT_results']:
             archive['DMFT_results']['broyler'] = [{'mu' : [],'V': [], 'dV': [], 'F': [], 'dF': []}
                                                   for _ in range(sum_k.n_inequiv_shells)]
 
     # Generates a rotation matrix to change the basis
-    if general_params['set_rot'] != 'none':
+    if general_params['set_rot'] is not None:
         # calculate new rotation matrices
         sum_k = _calculate_rotation_matrix(general_params, sum_k)
     # Saves rotation matrix to h5 archive:
     if mpi.is_master_node() and iteration_offset == 0:
         archive['DMFT_input']['rot_mat'] = sum_k.rot_mat
     mpi.barrier()
 
+    # Calculates density in default block structure
+    local_gf_dft_corr = sum_k.extract_G_loc(broadening=broadening, transform_to_solver_blocks=False, with_Sigma=False)
+    dens_mat_dft = [gf.density() for gf in local_gf_dft_corr]
+
+    for iineq, gf in enumerate(local_gf_dft_corr):
+        mpi.report(f'Total density for imp {iineq} from DFT: '
+                   '{:10.6f}'.format(np.real(gf.total_density())))
+
     # determine block structure for solver
     det_blocks = None
     # load previous block_structure if possible
     if mpi.is_master_node():
         det_blocks = 'block_structure' not in archive['DMFT_input']
     det_blocks = mpi.bcast(det_blocks)
 
     # Previous rot_mat only not None if the rot_mat changed from load_sigma or previous run
     previous_rot_mat = None
-    solver_struct_ftps = None
+    deg_orbs_ftps = None
     # determine block structure for GF and Hyb function
     if det_blocks and not general_params['load_sigma']:
-        sum_k, dm, solver_struct_ftps = _determine_block_structure(sum_k, general_params, advanced_params)
+        sum_k, deg_orbs_ftps = _determine_block_structure(sum_k, general_params, advanced_params, solver_type_per_imp, dens_mat_dft)
     # if load sigma we need to load everything from this h5 archive
     elif general_params['load_sigma']:
         #loading block_struc and rot_mat and deg_shells
         if mpi.is_master_node():
             with HDFArchive(general_params['path_to_sigma'], 'r') as old_calc:
                 sum_k.block_structure = old_calc['DMFT_input/block_structure']
                 sum_k.deg_shells = old_calc['DMFT_input/deg_shells']
                 previous_rot_mat = old_calc['DMFT_input/rot_mat']
-                if general_params['solver_type'] in ['ftps']:
-                    solver_struct_ftps = old_calc['DMFT_input/solver_struct_ftps']
+                if deg_orbs_ftps is not None:
+                    deg_orbs_ftps = old_calc['DMFT_input/solver_struct_ftps']
 
             if not all(np.allclose(x, y) for x, y in zip(sum_k.rot_mat, previous_rot_mat)):
                 print('WARNING: rot_mat in current run is different from loaded_sigma run.')
             else:
                 previous_rot_mat = None
 
         sum_k.block_structure = mpi.bcast(sum_k.block_structure)
         sum_k.deg_shells = mpi.bcast(sum_k.deg_shells)
         previous_rot_mat = mpi.bcast(previous_rot_mat)
-        solver_struct_ftps = mpi.bcast(solver_struct_ftps)
+        deg_orbs_ftps = mpi.bcast(deg_orbs_ftps)
 
         # In a magnetic calculation, no shells are degenerate
         if general_params['magnetic'] and sum_k.SO == 0:
             sum_k.deg_shells = [[] for _ in range(sum_k.n_inequiv_shells)]
-        dm = None
     else:
         # Master node checks if rot_mat stayed the same
         if mpi.is_master_node():
             sum_k.block_structure = archive['DMFT_input']['block_structure']
             sum_k.deg_shells = archive['DMFT_input/deg_shells']
             previous_rot_mat = archive['DMFT_input']['rot_mat']
             if not all(np.allclose(x, y) for x, y in zip(sum_k.rot_mat, previous_rot_mat)):
                 print('WARNING: rot_mat in current step is different from previous step.')
                 archive['DMFT_input']['rot_mat'] = sum_k.rot_mat
             else:
                 previous_rot_mat = None
-            if general_params['solver_type'] in ['ftps']:
-                solver_struct_ftps = archive['DMFT_input/solver_struct_ftps']
+            if 'solver_struct_ftps' in archive['DMFT_input']:
+                deg_orbs_ftps = archive['DMFT_input/solver_struct_ftps']
 
         sum_k.block_structure = mpi.bcast(sum_k.block_structure)
         sum_k.deg_shells = mpi.bcast(sum_k.deg_shells)
         previous_rot_mat = mpi.bcast(previous_rot_mat)
-        solver_struct_ftps = mpi.bcast(solver_struct_ftps)
-        dm = None
+        deg_orbs_ftps = mpi.bcast(deg_orbs_ftps)
 
     # Compatibility with h5 archives from the triqs2 version
     # Sumk doesn't hold corr_to_inequiv anymore, which is in block_structure now
     if sum_k.block_structure.corr_to_inequiv is None:
         if mpi.is_master_node():
             sum_k.block_structure.corr_to_inequiv = archive['dft_input/corr_to_inequiv']
         sum_k.block_structure = mpi.bcast(sum_k.block_structure)
 
     # Determination of shell_multiplicity
     shell_multiplicity = [sum_k.corr_to_inequiv.count(icrsh) for icrsh in range(sum_k.n_inequiv_shells)]
 
-    # Initializes new empty Sigma with new blockstructure for calculation of DFT density
-    zero_Sigma = [sum_k.block_structure.create_gf(ish=iineq, gf_function=Gf, mesh=sum_k.mesh)
-                  for iineq in range(sum_k.n_inequiv_shells)]
-    sum_k.put_Sigma(zero_Sigma)
-
     # print block structure and DFT input quantitites!
-    formatter.print_block_sym(sum_k, dm, general_params)
-
-    # extract free lattice greens function
-    if general_params['solver_type'] in ['ftps']:
-        G_loc_all_dft = sum_k.extract_G_loc(broadening=general_params['eta'], with_Sigma=False, mu=dft_mu)
-    else:
-        G_loc_all_dft = sum_k.extract_G_loc(with_Sigma=False, mu=dft_mu)
-    density_mat_dft = [G_loc_all_dft[iineq].density() for iineq in range(sum_k.n_inequiv_shells)]
-
-    for iineq in range(sum_k.n_inequiv_shells):
-        density_shell_dft = G_loc_all_dft[iineq].total_density()
-        mpi.report('total density for imp {} from DFT: {:10.6f}'.format(iineq, np.real(density_shell_dft)))
+    formatter.print_block_sym(sum_k, dens_mat_dft, general_params)
 
     if general_params['magnetic']:
         sum_k.SP = 1
-
         if general_params['afm_order']:
             general_params = afm_mapping.determine(general_params, archive, sum_k.n_inequiv_shells)
 
     # Constructs interaction Hamiltonian and writes it to the h5 archive
-    h_int = interaction_hamiltonian.construct(sum_k, general_params, advanced_params)
+    h_int, gw_params = interaction_hamiltonian.construct(sum_k, general_params, solver_type_per_imp, gw_params)
     if mpi.is_master_node():
         archive['DMFT_input']['h_int'] = h_int
 
     # If new calculation, writes input parameters and sum_k <-> solver mapping to archive
     if iteration_offset == 0:
         if mpi.is_master_node():
-            archive['DMFT_input']['general_params'] = general_params
-            archive['DMFT_input']['solver_params'] = solver_params
-            archive['DMFT_input']['advanced_params'] = advanced_params
+            archive['DMFT_input']['general_params'] = dict_to_h5.prep_params_for_h5(general_params)
+            archive['DMFT_input']['solver_params'] = dict_to_h5.prep_params_for_h5(solver_params)
+            archive['DMFT_input']['dft_params'] = dict_to_h5.prep_params_for_h5(dft_params)
+            archive['DMFT_input']['advanced_params'] = dict_to_h5.prep_params_for_h5(advanced_params)
 
             archive['DMFT_input']['block_structure'] = sum_k.block_structure
             archive['DMFT_input']['deg_shells'] = sum_k.deg_shells
             archive['DMFT_input']['shell_multiplicity'] = shell_multiplicity
-            if general_params['solver_type'] in ['ftps']:
-                archive['DMFT_input']['solver_struct_ftps'] = solver_struct_ftps
+            if deg_orbs_ftps is not None:
+                archive['DMFT_input']['solver_struct_ftps'] = deg_orbs_ftps
+    mpi.barrier()
 
     solvers = [None] * sum_k.n_inequiv_shells
     for icrsh in range(sum_k.n_inequiv_shells):
         # Construct the Solver instances
-        solvers[icrsh] = SolverStructure(general_params, solver_params, advanced_params,
-                                         sum_k, icrsh, h_int[icrsh],
-                                         iteration_offset, solver_struct_ftps)
+        solvers[icrsh] = SolverStructure(general_params, solver_params[map_imp_solver[icrsh]],
+                                         gw_params, advanced_params, sum_k, icrsh, h_int[icrsh],
+                                         iteration_offset, deg_orbs_ftps)
 
     # store solver hash to archive
     if mpi.is_master_node():
         if 'version' not in archive['DMFT_input']:
             archive['DMFT_input'].create_group('version')
-        archive['DMFT_input']['version']['solver_name'] = general_params['solver_type']
-        archive['DMFT_input']['version']['solver_hash'] = solvers[0].git_hash
-        archive['DMFT_input']['version']['solver_version'] = solvers[0].version
+        for iineq, solver in enumerate(solvers):
+            if f'solver {iineq}' not in archive['DMFT_input']['version']:
+                archive['DMFT_input']['version'].create_group(f'solver {iineq}')
+            archive['DMFT_input']['version'][f'solver {iineq}']['name'] = solver.solver_params['type']
+            archive['DMFT_input']['version'][f'solver {iineq}']['hash'] = solver.git_hash
+            archive['DMFT_input']['version'][f'solver {iineq}']['version'] = solver.version
+
+    # Extracts local GF per *inequivalent* shell
+    local_gf_dft = sum_k.extract_G_loc(broadening=broadening, with_Sigma=False, mu=dft_mu)
 
     # Determines initial Sigma and DC
-    sum_k, solvers = initial_sigma.determine_dc_and_initial_sigma(general_params, advanced_params, sum_k,
-                                                                  archive, iteration_offset, density_mat_dft, solvers)
+    sum_k, solvers = initial_sigma.determine_dc_and_initial_sigma(general_params, gw_params, advanced_params, sum_k,
+                                                                  archive, iteration_offset, local_gf_dft, solvers,
+                                                                  solver_type_per_imp)
 
-    sum_k = manipulate_mu.set_initial_mu(general_params, sum_k, iteration_offset, archive, shell_multiplicity)
+    sum_k = manipulate_mu.set_initial_mu(general_params, sum_k, iteration_offset, archive, broadening)
 
 
     # setup of measurement of chi(SzSz(tau) if requested
-    if general_params['measure_chi'] != 'none':
-        solver_params, Op_list = _chi_setup(sum_k, general_params, solver_params)
-    else:
-        Op_list = None
+    ops_chi_measure = _chi_setup(sum_k, solver_params, map_imp_solver)
 
     mpi.report('\n {} DMFT cycles requested. Starting with iteration  {}.\n'.format(n_iter, iteration_offset+1))
 
     # Prepares observable and conv dicts
     observables = None
     conv_obs = None
     if mpi.is_master_node():
         observables = prep_observables(archive, sum_k)
-        conv_obs = convergence.prep_conv_obs(archive, sum_k)
+        conv_obs = convergence.prep_conv_obs(archive)
     observables = mpi.bcast(observables)
     conv_obs = mpi.bcast(conv_obs)
 
     if mpi.is_master_node() and iteration_offset == 0:
         write_header_to_file(general_params, sum_k)
-        observables = add_dft_values_as_zeroth_iteration(observables, general_params, dft_mu, dft_energy, sum_k,
-                                                         G_loc_all_dft, density_mat_dft, shell_multiplicity)
+        observables = add_dft_values_as_zeroth_iteration(observables, general_params, solver_type_per_imp, dft_mu, dft_energy, sum_k,
+                                                         local_gf_dft, shell_multiplicity)
         write_obs(observables, sum_k, general_params)
         # write convergence file
         convergence.prep_conv_file(general_params, sum_k)
 
     # The infamous DMFT self consistency cycle
     is_converged = False
     for it in range(iteration_offset + 1, iteration_offset + n_iter + 1):
@@ -525,17 +565,17 @@
             # enforce recomputation of eff_atomic_levels
             delattr(sum_k, 'Hsumk')
 
         mpi.report('#'*80)
         mpi.report('Running iteration: {} / {}'.format(it, iteration_offset + n_iter))
         (sum_k, solvers,
          observables, is_converged) = _dmft_step(sum_k, solvers, it, general_params,
-                                                 solver_params, advanced_params, dft_params,
+                                                 solver_params, advanced_params, dft_params, map_imp_solver, solver_type_per_imp,
                                                  h_int, archive, shell_multiplicity, E_kin_dft,
-                                                 observables, conv_obs, Op_list, dft_irred_kpt_indices, dft_energy,
+                                                 observables, conv_obs, ops_chi_measure, dft_irred_kpt_indices, dft_energy, broadening,
                                                  is_converged, is_sampling=False)
 
         if is_converged:
             break
 
     if is_converged:
         mpi.report('*** Required convergence reached ***')
@@ -549,17 +589,17 @@
         iteration_offset = it
 
         for it in range(iteration_offset + 1,
                         iteration_offset + 1 + general_params['sampling_iterations']):
             mpi.report('#'*80)
             mpi.report('Running iteration: {} / {}'.format(it, iteration_offset+general_params['sampling_iterations']))
             sum_k, solvers, observables, _ = _dmft_step(sum_k, solvers, it, general_params,
-                                                        solver_params, advanced_params, dft_params,
+                                                        solver_params, advanced_params, dft_params, map_imp_solver, solver_type_per_imp,
                                                         h_int, archive, shell_multiplicity, E_kin_dft,
-                                                        observables, conv_obs, Op_list, dft_irred_kpt_indices, dft_energy,
+                                                        observables, conv_obs, ops_chi_measure, dft_irred_kpt_indices, dft_energy, broadening,
                                                         is_converged=True, is_sampling=True)
 
         mpi.report('** Sampling finished ***')
         mpi.report('#'*80)
 
     mpi.barrier()
 
@@ -567,17 +607,17 @@
     if mpi.is_master_node():
         del archive
 
     return is_converged, sum_k
 
 
 def _dmft_step(sum_k, solvers, it, general_params,
-               solver_params, advanced_params, dft_params,
+               solver_params, advanced_params, dft_params, map_imp_solver, solver_type_per_imp,
                h_int, archive, shell_multiplicity, E_kin_dft,
-               observables, conv_obs, Op_list, dft_irred_kpt_indices, dft_energy,
+               observables, conv_obs, ops_chi_measure, dft_irred_kpt_indices, dft_energy, broadening,
                is_converged, is_sampling):
     """
     Contains the actual dmft steps when all the preparation is done
     """
 
     # init local density matrices for observables
     density_tot = 0.0
@@ -591,24 +631,19 @@
 
     if sum_k.SO:
         printed = ((np.real, 'real'), (np.imag, 'imaginary'))
     else:
         printed = ((np.real, 'real'), )
 
     # Extracts G local
-    if general_params['solver_type'] in ['ftps']:
-        G_loc_all = sum_k.extract_G_loc(broadening=general_params['eta'])
-    else:
-        G_loc_all = sum_k.extract_G_loc()
+    G_loc_all = sum_k.extract_G_loc(broadening=broadening)
 
     # Copies Sigma and G0 before Solver run for mixing later
     Sigma_freq_previous = [solvers[iineq].Sigma_freq.copy() for iineq in range(sum_k.n_inequiv_shells)]
     G0_freq_previous = [solvers[iineq].G0_freq.copy() for iineq in range(sum_k.n_inequiv_shells)]
-    if general_params['dc'] and general_params['dc_type'] == 4:
-        cpa_G_loc = gf_mixer.init_cpa(sum_k, solvers, general_params)
 
     # looping over inequiv shells and solving for each site seperately
     for icrsh in range(sum_k.n_inequiv_shells):
         # copy the block of G_loc into the corresponding instance of the impurity solver
         # TODO: why do we set solvers.G_freq? Isn't that simply an output of the solver?
         solvers[icrsh].G_freq << G_loc_all[icrsh]
 
@@ -621,44 +656,84 @@
             for func, name in printed:
                 mpi.report('{}, {} part'.format(key, name))
                 mpi.report(func(value))
 
         # dyson equation to extract G0_freq, using Hermitian symmetry
         solvers[icrsh].G0_freq << inverse(solvers[icrsh].Sigma_freq + inverse(solvers[icrsh].G_freq))
 
-        # dyson equation to extract cpa_G0_freq
-        if general_params['dc'] and general_params['dc_type'] == 4:
-            cpa_G0_freq[icrsh] << inverse(solvers[icrsh].Sigma_freq + inverse(cpa_G_loc[icrsh]))
-
         # mixing of G0 if wanted from the second iteration on
         if it > 1:
             solvers[icrsh] = gf_mixer.mix_g0(solvers[icrsh], general_params, icrsh, archive,
                                              G0_freq_previous[icrsh], it, sum_k.deg_shells[icrsh])
 
-        if general_params['solver_type'] in ['cthyb', 'ctint', 'hubbardI', 'inchworm']:
+        if isinstance(sum_k.mesh, MeshImFreq):
             solvers[icrsh].G0_freq << make_hermitian(solvers[icrsh].G0_freq)
         sum_k.symm_deg_gf(solvers[icrsh].G0_freq, ish=icrsh)
 
+        if ((solver_type_per_imp[icrsh] == 'cthyb' and solver_params[icrsh]['delta_interface'])
+                or solver_type_per_imp[icrsh] == 'ctseg'):
+            mpi.report('\n Using the delta interface for passing Delta(tau) and Hloc0 directly to the solver.')
+             # prepare solver input
+            sumk_eal = sum_k.eff_atomic_levels()[icrsh]
+            solver_eal = sum_k.block_structure.convert_matrix(sumk_eal, space_from='sumk', ish_from=sum_k.inequiv_to_corr[icrsh])
+            # fill Delta_time from Delta_freq sum_k to solver
+            # for name, g0 in self.G0_freq:
+            for name, g0 in solvers[icrsh].G0_freq:
+                solvers[icrsh].Delta_freq[name] << iOmega_n - inverse(g0) - solver_eal[name]
+                known_moments = make_zero_tail(solvers[icrsh].Delta_freq[name], 1)
+                tail, err = fit_hermitian_tail(solvers[icrsh].Delta_freq[name], known_moments)
+                # without SOC delta_tau needs to be real
+                if not sum_k.SO == 1:
+                    solvers[icrsh].Delta_time[name] << make_gf_from_fourier(solvers[icrsh].Delta_freq[name],
+                                                                            solvers[icrsh].Delta_time.mesh, tail).real
+                else:
+                    solvers[icrsh].Delta_time[name] << make_gf_from_fourier(solvers[icrsh].Delta_freq[name],
+                                                                           solvers[icrsh].Delta_time.mesh, tail)
+
+                if solver_params[icrsh]['diag_delta']:
+                    for o1 in range(g0.target_shape[0]):
+                        for o2 in range(g0.target_shape[0]):
+                            if o1 != o2:
+                                solvers[icrsh].Delta_time[name].data[:, o1, o2] = 0.0 + 0.0j
+
+                # Make non-interacting operator for Hloc0
+                Hloc_0 = Operator()
+                for spin, spin_block in solver_eal.items():
+                    for o1 in range(spin_block.shape[0]):
+                        for o2 in range(spin_block.shape[1]):
+                            # check if off-diag element is larger than threshold
+                            if o1 != o2 and abs(spin_block[o1,o2]) < solver_params[icrsh]['off_diag_threshold']:
+                                continue
+                            else:
+                                # TODO: adapt for SOC calculations, which should keep the imag part
+                                Hloc_0 += spin_block[o1,o2].real/2 * (c_dag(spin,o1) * c(spin,o2) + c_dag(spin,o2) * c(spin,o1))
+                solvers[icrsh].Hloc_0 = Hloc_0
+
          # store solver to h5 archive
         if general_params['store_solver'] and mpi.is_master_node():
+            if 'solver' not in archive['DMFT_input']:
+                archive['DMFT_input'].create_group('solver')
             archive['DMFT_input/solver'].create_group('it_'+str(it))
             archive['DMFT_input/solver/it_'+str(it)]['S_'+str(icrsh)] = solvers[icrsh].triqs_solver
 
         # store DMFT input directly in last_iter
         if mpi.is_master_node():
             archive['DMFT_results/last_iter']['G0_freq_{}'.format(icrsh)] = solvers[icrsh].G0_freq
+            if solver_type_per_imp[icrsh] == 'cthyb' and solver_params[icrsh]['delta_interface']:
+                archive['DMFT_results/last_iter']['Delta_time_{}'.format(icrsh)] = solvers[icrsh].Delta_time
 
         # setup of measurement of chi(SzSz(tau) if requested
-        if general_params['measure_chi'] != 'none':
-            solvers[icrsh].solver_params['measure_O_tau'] = (Op_list[icrsh], Op_list[icrsh])
+        # TODO: move this into solver class?
+        if ops_chi_measure[icrsh] is not None:
+            solvers[icrsh].solver_params['measure_O_tau'] = (ops_chi_measure[icrsh], ops_chi_measure[icrsh])
 
         if (general_params['magnetic'] and general_params['afm_order'] and general_params['afm_mapping'][icrsh][0]):
             # If we do a AFM calculation we can use the init magnetic moments to
             # copy the self energy instead of solving it explicitly
-            solvers = afm_mapping.apply(general_params, solver_params, icrsh, sum_k.gf_struct_solver[icrsh], solvers)
+            solvers = afm_mapping.apply(general_params, icrsh, sum_k.gf_struct_solver[icrsh], solvers)
         else:
             # Solve the impurity problem for this shell
             mpi.report('\nSolving the impurity problem for shell {} ...'.format(icrsh))
             mpi.barrier()
             start_time = timer()
             solvers[icrsh].solve(it=it)
             mpi.barrier()
@@ -672,47 +747,45 @@
         formatter.print_local_density(density_shell[icrsh], density_shell_pre[icrsh],
                                       density_mat_unsym[icrsh], sum_k.SO)
 
         # update solver in h5 archive
         if general_params['store_solver'] and mpi.is_master_node():
             archive['DMFT_input/solver/it_'+str(it)]['S_'+str(icrsh)] = solvers[icrsh].triqs_solver
 
-        # add to cpa_G_time
-        if general_params['dc'] and general_params['dc_type'] == 4:
-            cpa_G_time << cpa_G_time + general_params['cpa_x'][icrsh] * solvers[icrsh].G_time
-
     # Done with loop over impurities
 
     if mpi.is_master_node():
         # Done. Now do post-processing:
         print('\n *** Post-processing the solver output ***')
         print('Total charge of all correlated shells : {:.6f}\n'.format(density_tot))
 
-    # if CPA average Sigma over impurities before mixing
-    if general_params['dc'] and general_params['dc_type'] == 4:
-        solvers = gf_mixer.mix_cpa(cpa_G0_freq, sum_k.n_inequiv_shells, solvers)
     solvers = gf_mixer.mix_sigma(general_params, sum_k.n_inequiv_shells, solvers, Sigma_freq_previous)
 
     # calculate new DC
     # for the hartree solver the DC potential will be formally set to zero as it is already present in the Sigma
     if general_params['dc'] and general_params['dc_dmft']:
         sum_k = initial_sigma.calculate_double_counting(sum_k, density_mat,
-                                                        general_params, advanced_params)
-    
+                                                        general_params, advanced_params,
+                                                        solver_type_per_imp)
+
     #The hartree solver computes the DC energy internally, set it in sum_k
-    if general_params['solver_type'] == 'hartree':
-        for icrsh in range(sum_k.n_inequiv_shells):
-            sum_k.dc_energ[icrsh] = solvers[icrsh].DC_energy
+    for icrsh in range(sum_k.n_corr_shells):
+        iineq = sum_k.corr_to_inequiv[icrsh]
+        if solver_type_per_imp[iineq] == 'hartree':
+            sum_k.dc_energ[icrsh] = solvers[iineq].DC_energy
 
+    # symmetrize Sigma over degenerate blocks
+    for icrsh in range(sum_k.n_inequiv_shells):
+        sum_k.symm_deg_gf(solvers[icrsh].Sigma_freq, ish=icrsh)
     # doing the dmft loop and set new sigma into sumk
     sum_k.put_Sigma([solvers[icrsh].Sigma_freq for icrsh in range(sum_k.n_inequiv_shells)])
 
     # saving previous mu for writing to observables file
     previous_mu = sum_k.chemical_potential
-    sum_k = manipulate_mu.update_mu(general_params, sum_k, it, archive)
+    sum_k = manipulate_mu.update_mu(general_params, sum_k, it, archive, broadening)
 
     # if we do a CSC calculation we need always an updated GAMMA file
     E_bandcorr = 0.0
     deltaN = None
     dens = None
     if general_params['csc']:
         # handling the density correction for fcsc calculations
@@ -720,25 +793,27 @@
         deltaN, dens, E_bandcorr = sum_k.calc_density_correction(dm_type=dft_params['dft_code'],
                                                                  kpts_to_write=dft_irred_kpt_indices)
     elif general_params['calc_energies']:
         # for a one shot calculation we are using our own method
         E_bandcorr = calc_bandcorr_man(general_params, sum_k, E_kin_dft)
 
     # Writes results to h5 archive
-    results_to_archive.write(archive, sum_k, general_params, solver_params, solvers, it,
+    results_to_archive.write(archive, sum_k, general_params, solver_params, solvers, map_imp_solver, solver_type_per_imp, it,
                              is_sampling, previous_mu, density_mat_pre, density_mat, deltaN, dens)
 
     mpi.barrier()
 
     # calculate observables and write them to file
     if mpi.is_master_node():
         print('\n *** calculation of observables ***')
         observables = add_dmft_observables(observables,
                                            general_params,
                                            solver_params,
+                                           map_imp_solver,
+                                           solver_type_per_imp,
                                            dft_energy,
                                            it,
                                            solvers,
                                            h_int,
                                            previous_mu,
                                            sum_k,
                                            density_mat,
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/__init__.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/afm_mapping.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/afm_mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     general_params['afm_order'] = mpi.bcast(general_params['afm_order'])
     if general_params['afm_order']:
         general_params['afm_mapping'] = mpi.bcast(afm_mapping)
 
     return general_params
 
 
-def apply(general_params, solver_params, icrsh, gf_struct_solver, solvers):
+def apply(general_params, icrsh, gf_struct_solver, solvers):
     imp_source = general_params['afm_mapping'][icrsh][1]
     invert_spin = general_params['afm_mapping'][icrsh][2]
     mpi.report('\ncopying the self-energy for shell {} from shell {}'.format(icrsh, imp_source))
     mpi.report('inverting spin channels: '+str(invert_spin))
 
     if invert_spin:
         for spin_channel in gf_struct_solver.keys():
@@ -95,32 +95,32 @@
 
             solvers[icrsh].Sigma_freq[spin_channel] << solvers[imp_source].Sigma_freq[target_channel]
             solvers[icrsh].G_freq[spin_channel] << solvers[imp_source].G_freq[target_channel]
             solvers[icrsh].G_freq_unsym[spin_channel] << solvers[imp_source].G_freq_unsym[target_channel]
             solvers[icrsh].G0_freq[spin_channel] << solvers[imp_source].G0_freq[target_channel]
             solvers[icrsh].G_time[spin_channel] << solvers[imp_source].G_time[target_channel]
 
-            if solver_params['measure_pert_order']:
+            if solvers[icrsh].solver_params['measure_pert_order']:
                 if not hasattr(solvers[icrsh], 'perturbation_order'):
                     solvers[icrsh].perturbation_order = {}
                 solvers[icrsh].perturbation_order[spin_channel] = solvers[imp_source].perturbation_order[target_channel]
                 solvers[icrsh].perturbation_order_total = solvers[imp_source].perturbation_order_total
 
     else:
         solvers[icrsh].Sigma_freq << solvers[imp_source].Sigma_freq
         solvers[icrsh].G_freq << solvers[imp_source].G_freq
         solvers[icrsh].G_freq_unsym << solvers[imp_source].G_freq_unsym
         solvers[icrsh].G0_freq << solvers[imp_source].G0_freq
         solvers[icrsh].G_time << solvers[imp_source].G_time
 
-        if solver_params['measure_pert_order']:
+        if solvers[icrsh].solver_params['measure_pert_order']:
             solvers[icrsh].perturbation_order = solvers[imp_source].perturbation_order
             solvers[icrsh].perturbation_order_total = solvers[imp_source].perturbation_order_total
 
-    if solver_params['measure_density_matrix']:
+    if solvers[icrsh].solver_params['measure_density_matrix']:
         solvers[icrsh].density_matrix = solvers[imp_source].density_matrix
         solvers[icrsh].h_loc_diagonalization = solvers[imp_source].h_loc_diagonalization
 
-    if general_params['measure_chi'] != 'none':
+    if 'measure_chi' in solvers[icrsh].solver_params and solvers[icrsh].solver_params['measure_chi'] is not None:
         solvers[icrsh].O_time = solvers[imp_source].O_time
 
     return solvers
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/convergence.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/convergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,23 +165,22 @@
         raise ValueError('MeshReTime is not implemented')
 
     if type(G1.mesh) in (MeshImFreq, MeshImTime) and norm_temp:
         norm = norm / np.sqrt(G1.mesh.beta)
 
     return norm
 
-def prep_conv_obs(h5_archive, sum_k):
+def prep_conv_obs(h5_archive):
     """
     prepares the conv arrays and files for the DMFT calculation
 
     Parameters
     ----------
     h5_archive: hdf archive instance
         hdf archive for calculation
-    sum_k : SumK Object instances
 
     __Returns:__
     conv_obs : dict
         conv array for calculation
     """
 
     # determine number of impurities
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/formatter.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 #
 # solid_dmft - A versatile python wrapper to perform DFT+DMFT calculations
 #              utilizing the TRIQS software library
 #
 # Copyright (C) 2018-2020, ETH Zurich
 # Copyright (C) 2021, The Simons Foundation
@@ -86,21 +85,18 @@
             row = np.concatenate((block_1.real, block_2.real))
             print((' '*11 + fmt + '  ' + fmt).format(*row))
     print('\n')
 
     if dm:
         # Prints dft density matrix
         print('\nDFT density matrix')
+        # Double loop to sort by impurities
         for icrsh in range(sum_k.n_inequiv_shells):
             spins = sum_k.spin_block_names[sum_k.SO]
-            # ftps dens_mat only knows inequiv_shells
-            if general_params['solver_type'] in ['ftps']:
-                shlst = [icrsh]
-            else:
-                shlst = [ish for ish, ineq_shell in enumerate(sum_k.corr_to_inequiv) if ineq_shell == icrsh]
+            shlst = [ish for ish, ineq_shell in enumerate(sum_k.corr_to_inequiv) if ineq_shell == icrsh]
             for sh in shlst:
                 n_orb = sum_k.corr_shells[sh]['dim']
                 if sum_k.SO == 0:
                     dm_blocks = {spin: dm[sh][spin] for spin in spins}
                 else:
                     dm_blocks = {'ud real': dm[sh]['ud'].real, 'ud imag': dm[sh]['ud'].imag}
                 print('rho[{0:2d}] '.format(sh)+4*' '+' '.join([sp.center(9*n_orb) for sp in dm_blocks.keys()]))
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/greens_functions_mixer.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/greens_functions_mixer.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,29 +215,7 @@
             solvers[icrsh].Sigma_freq << (general_params['sigma_mix'] * solvers[icrsh].Sigma_freq
                                         + (1-general_params['sigma_mix']) * Sigma_freq_previous[icrsh])
 
     for icrsh in range(n_inequiv_shells):
         solvers[icrsh].Sigma_freq << mpi.bcast(solvers[icrsh].Sigma_freq)
 
     return solvers
-
-
-def init_cpa(sum_k, solvers, general_params):
-    # initialize cpa_G_time, cpa_G0_freq; extract cpa_G_loc
-    cpa_G_time = sum_k.block_structure.create_gf(ish=0, gf_function=Gf, space='solver',
-                                                 mesh=MeshImTime(beta=general_params['beta'],
-                                                                 S='Fermion', n_tau=general_params['n_tau'])
-                                                 )
-    cpa_G0_freq = [solvers[iineq].G0_freq.copy() for iineq in range(sum_k.n_inequiv_shells)]
-    cpa_G_loc = sum_k.extract_G_loc(with_Sigma=True, with_dc=False)
-
-    return cpa_G_loc
-
-
-def mix_cpa(cpa_G0_freq, n_inequiv_shells, solvers):
-    cpa_G_freq = solvers[0].G_freq.copy()
-    cpa_G_freq << Fourier(cpa_G_time)
-    # replace solver Sigma with cpa Sigma
-    for icrsh in range(n_inequiv_shells):
-        solvers[icrsh].Sigma_freq << inverse(cpa_G0_freq[icrsh]) - inverse(cpa_G_freq)
-
-    return solvers
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/initial_self_energies.py` & `solid_dmft-3.3.0/python/solid_dmft/gw_embedding/gw_flow.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,473 +18,474 @@
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # solid_dmft (in the file COPYING.txt in this directory). If not, see
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
-
+# pyright: reportUnusedExpression=false
 """
-Contains all functions related to determining the double counting and the
-initial self-energy.
+Module for gw flow
 """
 
-# system
-from copy import deepcopy
+from timeit import default_timer as timer
 import numpy as np
 
-# triqs
 from h5 import HDFArchive
-import triqs.utility.mpi as mpi
-from triqs.gf import BlockGf, Gf
+from triqs.utility import mpi
+from triqs.gf.tools import inverse
+from triqs.gf import (
+    Gf,
+    BlockGf,
+    make_hermitian,
+    make_gf_dlr,
+    make_gf_imfreq,
+    make_gf_imtime,
+    make_gf_dlr_imfreq,
+)
+from triqs.version import git_hash as triqs_hash
+from triqs.version import version as triqs_version
+from triqs.gf.meshes import MeshImFreq
+from triqs.operators import c_dag, c, Operator
+from triqs_dft_tools.block_structure import BlockStructure
+
+from solid_dmft.version import solid_dmft_hash
+from solid_dmft.version import version as solid_dmft_version
+from solid_dmft.dmft_tools import formatter
+from solid_dmft.dmft_tools import results_to_archive
+from solid_dmft.dmft_tools.solver import SolverStructure
+from solid_dmft.dmft_tools import interaction_hamiltonian
+from solid_dmft.dmft_cycle import _extract_quantity_per_inequiv
+from solid_dmft.gw_embedding.bdft_converter import convert_gw_output
 
 
-def calculate_double_counting(sum_k, density_matrix, general_params, advanced_params):
+class dummy_sumk(object):
     """
-    Calculates the double counting, including all manipulations from advanced_params.
-
-    Parameters
-    ----------
-    sum_k : SumkDFT object
-    density_matrix : list of gf_struct_solver like
-        List of density matrices for all inequivalent shells
-    general_params : dict
-        general parameters as a dict
-    advanced_params : dict
-        advanced parameters as a dict
-
-    Returns
-    --------
-    sum_k : SumKDFT object
-        The SumKDFT object containing the updated double counting
+    create dummy sumk helper object
     """
 
-    mpi.report('\n*** DC determination ***')
-
-    # copy the density matrix to not change it
-    density_matrix_DC = deepcopy(density_matrix)
-
-    if general_params['solver_type'] == 'hartree':
-        mpi.report('\nSOLID_DMFT: Hartree solver detected, zeroing out the DC correction. This gets computed at the solver level')
-        for icrsh in range(sum_k.n_inequiv_shells):
-            sum_k.calc_dc(density_matrix_DC[icrsh], orb=icrsh,
-                          use_dc_value=0.0)
-        return sum_k
-
-    # Sets the DC and exits the function if advanced_params['dc_fixed_value'] is specified
-    if advanced_params['dc_fixed_value'] != 'none':
-        for icrsh in range(sum_k.n_inequiv_shells):
-            sum_k.calc_dc(density_matrix_DC[icrsh], orb=icrsh,
-                          use_dc_value=advanced_params['dc_fixed_value'])
-        return sum_k
-
-    # use DC for CPA
-    if general_params['dc'] and general_params['dc_type'] == 4:
-        zetas = general_params['cpa_zeta']
-        for icrsh in range(sum_k.n_inequiv_shells):
-            sum_k.calc_dc(density_matrix_DC[icrsh], orb=icrsh, use_dc_value=zetas[icrsh])
-
-        return sum_k
-
-
-    if advanced_params['dc_fixed_occ'] != 'none':
-        mpi.report('Fixing occupation for DC potential to provided value')
-
-        assert sum_k.n_inequiv_shells == len(advanced_params['dc_fixed_occ']), "give exactly one occupation per correlated shell"
-        for icrsh in range(sum_k.n_inequiv_shells):
-            mpi.report('fixing occupation for impurity '+str(icrsh)+' to n='+str(advanced_params['dc_fixed_occ'][icrsh]))
-            n_orb = sum_k.corr_shells[icrsh]['dim']
-            # we need to handover a matrix to calc_dc so calc occ per orb per spin channel
-            orb_occ = advanced_params['dc_fixed_occ'][icrsh]/(n_orb*2)
-            # setting occ of each diag orb element to calc value
-            for inner in density_matrix_DC[icrsh].values():
-                np.fill_diagonal(inner, orb_occ+0.0j)
-
-    # The regular way: calculates the DC based on U, J and the dc_type
-    for icrsh in range(sum_k.n_inequiv_shells):
-        if general_params['dc_type'] == 3:
-            # this is FLL for eg orbitals only as done in Seth PRB 96 205139 2017 eq 10
-            # this setting for U and J is reasonable as it is in the spirit of F0 and Javg
-            # for the 5 orb case
-            mpi.report('Doing FLL DC for eg orbitals only with Uavg=U-J and Javg=2*J')
-            Uavg = advanced_params['dc_U'][icrsh] - advanced_params['dc_J'][icrsh]
-            Javg = 2*advanced_params['dc_J'][icrsh]
-            sum_k.calc_dc(density_matrix_DC[icrsh], U_interact=Uavg, J_hund=Javg,
-                          orb=icrsh, use_dc_formula=0)
+    def __init__(self, n_inequiv_shells, n_orb_list, enforce_off_diag, use_rot, magnetic):
+        self.n_inequiv_shells = n_inequiv_shells
+        self.SO = 0
+        self.use_rotations = use_rot
+        if self.use_rotations:
+            raise ValueError('rotations not implemented yet for GW embedding')
+        self.gf_struct_solver = []
+        self.gf_struct_sumk = []
+        self.spin_block_names = []
+        self.inequiv_to_corr = []
+        self.corr_to_inequiv = []
+        self.deg_shells = []
+        self.dc_energ = [0.0 for ish in range(self.n_inequiv_shells)]
+        self.sumk_to_solver = [{} for ish in range(self.n_inequiv_shells)]
+        self.solver_to_sumk = [{} for ish in range(self.n_inequiv_shells)]
+        self.solver_to_sumk_block = [{} for ish in range(self.n_inequiv_shells)]
+        for ish in range(self.n_inequiv_shells):
+            self.inequiv_to_corr.append(ish)
+            self.corr_to_inequiv.append(ish)
+            self.spin_block_names.append(['up', 'down'])
+            self.gf_struct_sumk.append([('up', n_orb_list[ish]), ('down', n_orb_list[ish])])
+
+            # use full off-diagonal block structure in impurity solver
+            if enforce_off_diag:
+                self.gf_struct_solver.append({'up_0': n_orb_list[ish], 'down_0': n_orb_list[ish]})
+                if not magnetic:
+                    self.deg_shells.append([['up_0', 'down_0']])
+                # setup standard mapping between sumk and solver
+                for block, inner_dim in self.gf_struct_sumk[ish]:
+                    self.solver_to_sumk_block[ish][f'{block}_0'] = block
+                    for iorb in range(inner_dim):
+                        self.sumk_to_solver[ish][(block, iorb)] = (block + '_0', iorb)
+                        self.solver_to_sumk[ish][(block + '_0', iorb)] = (block, iorb)
+            else:
+                self.gf_struct_solver.append({})
+                self.deg_shells.append([])
+                for block, inner_dim in self.gf_struct_sumk[ish]:
+                    for iorb in range(inner_dim):
+                        self.gf_struct_solver[ish][f'{block}_{iorb}'] = 1
+                        if not magnetic and block == 'up':
+                            self.deg_shells[ish].append([f'up_{iorb}', f'down_{iorb}'])
+                        # setup standard mapping between sumk and solver
+                        self.solver_to_sumk_block[ish][f'{block}_{iorb}'] = block
+                        self.sumk_to_solver[ish][(block, iorb)] = (f'{block}_{iorb}', 0)
+                        self.solver_to_sumk[ish][(f'{block}_{iorb}', 0)] = (block, iorb)
+
+
+        self.gf_struct_solver_list = [sorted([(k, v) for k, v in list(gfs.items())], key=lambda x: x[0]) for gfs in self.gf_struct_solver]
+
+        # creat block_structure object for solver
+        self.block_structure = BlockStructure(
+            gf_struct_sumk=self.gf_struct_sumk,
+            gf_struct_solver=self.gf_struct_solver,
+            solver_to_sumk=self.solver_to_sumk,
+            sumk_to_solver=self.sumk_to_solver,
+            solver_to_sumk_block=self.solver_to_sumk_block,
+            deg_shells=self.deg_shells,
+            corr_to_inequiv = self.corr_to_inequiv,
+            transformation=None,
+        )
+
+    def symm_deg_gf(self, gf_to_symm, ish=0):
+        r"""
+        Averages a GF or a dict of np.ndarrays over degenerate shells.
+
+        Degenerate shells of an inequivalent correlated shell are defined by
+        `self.deg_shells`. This function enforces corresponding degeneracies
+        in the input GF.
+
+        Parameters
+        ----------
+        gf_to_symm : gf_struct_solver like
+                     Input and output GF (i.e., it gets overwritten)
+                     or dict of np.ndarrays.
+        ish : int
+              Index of an inequivalent shell. (default value 0)
+
+        """
+
+        # when reading block_structures written with older versions from
+        # an h5 file, self.deg_shells might be None
+        if self.deg_shells is None:
+            return
+
+        if not isinstance(gf_to_symm, BlockGf) and isinstance(gf_to_symm[list(gf_to_symm.keys())[0]], np.ndarray):
+            blockgf = False
+        elif isinstance(gf_to_symm, BlockGf):
+            blockgf = True
         else:
-            sum_k.calc_dc(density_matrix_DC[icrsh], U_interact=advanced_params['dc_U'][icrsh],
-                          J_hund=advanced_params['dc_J'][icrsh], orb=icrsh,
-                          use_dc_formula=general_params['dc_type'])
-
-    # for the fixed DC according to https://doi.org/10.1103/PhysRevB.90.075136
-    # dc_imp is calculated with fixed occ but dc_energ is calculated with given n
-    if advanced_params['dc_nominal']:
-        mpi.report('\ncalculating DC energy with fixed DC potential from above\n'
-                   + ' for the original density matrix doi.org/10.1103/PhysRevB.90.075136\n'
-                   + ' aka nominal DC')
-        dc_imp = deepcopy(sum_k.dc_imp)
-        dc_new_en = deepcopy(sum_k.dc_energ)
-        for ish in range(sum_k.n_corr_shells):
-            n_DC = 0.0
-            for value in density_matrix[sum_k.corr_to_inequiv[ish]].values():
-                n_DC += np.trace(value.real)
-
-            # calculate new DC_energ as n*V_DC
-            # average over blocks in case blocks have different imp
-            dc_new_en[ish] = 0.0
-            for spin, dc_per_spin in dc_imp[ish].items():
-                # assuming that the DC potential is the same for all orbitals
-                # dc_per_spin is a list for each block containing on the diag
-                # elements the DC potential for the self-energy correction
-                dc_new_en[ish] += n_DC * dc_per_spin[0][0]
-            dc_new_en[ish] = dc_new_en[ish] / len(dc_imp[ish])
-        sum_k.set_dc(dc_imp, dc_new_en)
-
-        # Print new DC values
-        mpi.report('\nFixed occ, new DC values:')
-        for icrsh, (dc_per_shell, energy_per_shell) in enumerate(zip(dc_imp, dc_new_en)):
-            for spin, dc_per_spin in dc_per_shell.items():
-                mpi.report('DC for shell {} and block {} = {}'.format(icrsh, spin, dc_per_spin[0][0]))
-            mpi.report('DC energy for shell {} = {}'.format(icrsh, energy_per_shell))
-
-    # Rescales DC if advanced_params['dc_factor'] is given
-    if advanced_params['dc_factor'] != 'none':
-        rescaled_dc_imp = [{spin: advanced_params['dc_factor'] * dc_per_spin
-                            for spin, dc_per_spin in dc_per_shell.items()}
-                          for dc_per_shell in sum_k.dc_imp]
-        rescaled_dc_energy = [advanced_params['dc_factor'] * energy_per_shell
-                              for energy_per_shell in sum_k.dc_energ]
-        sum_k.set_dc(rescaled_dc_imp, rescaled_dc_energy)
-
-        # Print new DC values
-        mpi.report('\nRescaled DC, new DC values:')
-        for icrsh, (dc_per_shell, energy_per_shell) in enumerate(zip(rescaled_dc_imp, rescaled_dc_energy)):
-            for spin, dc_per_spin in dc_per_shell.items():
-                mpi.report('DC for shell {} and block {} = {}'.format(icrsh, spin, dc_per_spin[0][0]))
-            mpi.report('DC energy for shell {} = {}'.format(icrsh, energy_per_shell))
-
-    return sum_k
-
-
-def _load_sigma_from_h5(h5_archive, iteration):
-    """
-    Reads impurity self-energy for all impurities from file and returns them as a list
+            raise ValueError("gf_to_symm should be either a BlockGf or a dict of numpy arrays")
 
-    Parameters
-    ----------
-    h5_archive : HDFArchive
-        HDFArchive to read from
-    iteration : int
-        at which iteration will sigma be loaded
-
-    Returns
-    --------
-    self_energies : list of green functions
-
-    dc_imp : numpy array
-        DC potentials
-    dc_energy : numpy array
-        DC energies per impurity
-    density_matrix : numpy arrays
-        Density matrix from the previous self-energy
-    """
-
-    internal_path = 'DMFT_results/'
-    internal_path += 'last_iter' if iteration == -1 else 'it_{}'.format(iteration)
-
-    n_inequiv_shells = h5_archive['dft_input']['n_inequiv_shells']
-
-    # Loads previous self-energies and DC
-    self_energies = [h5_archive[internal_path]['Sigma_freq_{}'.format(iineq)]
-                     for iineq in range(n_inequiv_shells)]
-    last_g0 = [h5_archive[internal_path]['G0_freq_{}'.format(iineq)]
-                     for iineq in range(n_inequiv_shells)]
-    dc_imp = h5_archive[internal_path]['DC_pot']
-    dc_energy = h5_archive[internal_path]['DC_energ']
-
-    # Loads density_matrix to recalculate DC if dc_dmft
-    density_matrix = h5_archive[internal_path]['dens_mat_post']
-
-    print('Loaded Sigma_imp0...imp{} '.format(n_inequiv_shells-1)
-          + ('at last it ' if iteration == -1 else 'at it {} '.format(iteration)))
-
-    return self_energies, dc_imp, dc_energy, last_g0, density_matrix
-
-
-def _sumk_sigma_to_solver_struct(sum_k, start_sigma):
-    """
-    Extracts the local Sigma. Copied from SumkDFT.extract_G_loc, version 2.1.x.
-
-    Parameters
-    ----------
-    sum_k : SumkDFT object
-        Sumk object with the information about the correct block structure
-    start_sigma : list of BlockGf (Green's function) objects
-        List of Sigmas in sum_k block structure that are to be converted.
-
-    Returns
-    -------
-    Sigma_inequiv : list of BlockGf (Green's function) objects
-        List of Sigmas that can be used to initialize the solver
-    """
-
-    Sigma_local = [start_sigma[icrsh].copy() for icrsh in range(sum_k.n_corr_shells)]
-    Sigma_inequiv = [BlockGf(name_block_generator=[(block, Gf(mesh=Sigma_local[0].mesh, target_shape=(dim, dim)))
-                                                   for block, dim in sum_k.gf_struct_solver[ish].items()],
-                             make_copies=False) for ish in range(sum_k.n_inequiv_shells)]
-
-    # G_loc is rotated to the local coordinate system
-    if sum_k.use_rotations:
-        for icrsh in range(sum_k.n_corr_shells):
-            for bname, gf in Sigma_local[icrsh]:
-                Sigma_local[icrsh][bname] << sum_k.rotloc(
-                    icrsh, gf, direction='toLocal')
-
-    # transform to CTQMC blocks
-    for ish in range(sum_k.n_inequiv_shells):
-        for block, dim in sum_k.gf_struct_solver[ish].items():
-            for ind1 in range(dim):
-                for ind2 in range(dim):
-                    block_sumk, ind1_sumk = sum_k.solver_to_sumk[ish][(block, ind1)]
-                    block_sumk, ind2_sumk = sum_k.solver_to_sumk[ish][(block, ind2)]
-                    Sigma_inequiv[ish][block][ind1, ind2] << Sigma_local[
-                        sum_k.inequiv_to_corr[ish]][block_sumk][ind1_sumk, ind2_sumk]
-
-    # return only the inequivalent shells
-    return Sigma_inequiv
+        for degsh in self.deg_shells[ish]:
+            # ss will hold the averaged orbitals in the basis where the
+            # blocks are all equal
+            # i.e. maybe_conjugate(v^dagger gf v)
+            ss = None
+            n_deg = len(degsh)
+            for key in degsh:
+                if ss is None:
+                    if blockgf:
+                        ss = gf_to_symm[key].copy()
+                        ss.zero()
+                        helper = ss.copy()
+                    else:
+                        ss = np.zeros_like(gf_to_symm[key])
+                        helper = np.zeros_like(gf_to_symm[key])
+
+                # get the transformation matrix
+                if isinstance(degsh, dict):
+                    v, C = degsh[key]
+                else:
+                    # for backward compatibility, allow degsh to be a list
+                    if blockgf:
+                        v = np.eye(*ss.target_shape)
+                    else:
+                        v = np.eye(*ss.shape)
+                    C = False
+                # the helper is in the basis where the blocks are all equal
+                if blockgf:
+                    helper.from_L_G_R(v.conjugate().transpose(), gf_to_symm[key], v)
+                else:
+                    helper = np.dot(v.conjugate().transpose(), np.dot(gf_to_symm[key], v))
 
+                if C:
+                    helper << helper.transpose()
+                # average over all shells
+                ss += helper / (1.0 * n_deg)
+            # now put back the averaged gf to all shells
+            for key in degsh:
+                if isinstance(degsh, dict):
+                    v, C = degsh[key]
+                else:
+                    # for backward compatibility, allow degsh to be a list
+                    if blockgf:
+                        v = np.eye(*ss.target_shape)
+                    else:
+                        v = np.eye(*ss.shape)
+                    C = False
+                if blockgf and C:
+                    gf_to_symm[key].from_L_G_R(v, ss.transpose().copy(), v.conjugate().transpose())
+                elif blockgf and not C:
+                    gf_to_symm[key].from_L_G_R(v, ss, v.conjugate().transpose())
+                elif not blockgf and C:
+                    gf_to_symm[key] = np.dot(v, np.dot(ss.transpose().copy(), v.conjugate().transpose()))
+                elif not blockgf and not C:
+                    gf_to_symm[key] = np.dot(v, np.dot(ss, v.conjugate().transpose()))
 
-def _set_loaded_sigma(sum_k, loaded_sigma, loaded_dc_imp, general_params):
+def embedding_driver(general_params, solver_params, gw_params, advanced_params):
     """
-    Adjusts for the Hartree shift when loading a self energy Sigma_freq from a
-    previous calculation that was run with a different U, J or double counting.
+    Function to run the gw embedding cycle.
 
     Parameters
     ----------
-    sum_k : SumkDFT object
-        Sumk object with the information about the correct block structure
-    loaded_sigma : list of BlockGf (Green's function) objects
-        List of Sigmas loaded from the previous calculation
-    loaded_dc_imp : list of dicts
-        List of dicts containing the loaded DC. Used to adjust the Hartree shift.
     general_params : dict
         general parameters as a dict
-
-    Raises
-    ------
-    ValueError
-        Raised if the block structure between the loaded and the Sumk DC_imp
-        does not agree.
-
-    Returns
-    -------
-    start_sigma : list of BlockGf (Green's function) objects
-        List of Sigmas, loaded Sigma adjusted for the new Hartree term
-
+    solver_params : dict
+        solver parameters as a dict
+    gw_params : dict
+        dft parameters as a dict
+    advanced_params : dict
+        advanced parameters as a dict
     """
-    # Compares loaded and new double counting
-    if len(loaded_dc_imp) != len(sum_k.dc_imp):
-        raise ValueError('Loaded double counting has a different number of '
-                         + 'correlated shells than current calculation.')
-
-    has_double_counting_changed = False
-    for loaded_dc_shell, calc_dc_shell in zip(loaded_dc_imp, sum_k.dc_imp):
-        if sorted(loaded_dc_shell.keys()) != sorted(calc_dc_shell.keys()):
-            raise ValueError('Loaded double counting has a different block '
-                             + 'structure than current calculation.')
-
-        for channel in loaded_dc_shell.keys():
-            if not np.allclose(loaded_dc_shell[channel], calc_dc_shell[channel],
-                               atol=1e-4, rtol=0):
-                has_double_counting_changed = True
-                break
-
-    # Sets initial Sigma
-    start_sigma = loaded_sigma
-
-    if not has_double_counting_changed:
-        print('DC remained the same. Using loaded Sigma as initial Sigma.')
-        return start_sigma
-
-    # Uses the SumkDFT add_dc routine to correctly substract the DC shift
-    sum_k.put_Sigma(start_sigma)
-    calculated_dc_imp = sum_k.dc_imp
-    sum_k.dc_imp = [{channel: np.array(loaded_dc_shell[channel]) - np.array(calc_dc_shell[channel])
-                     for channel in loaded_dc_shell}
-                    for calc_dc_shell, loaded_dc_shell in zip(sum_k.dc_imp, loaded_dc_imp)]
-    start_sigma = sum_k.add_dc()
-    start_sigma = _sumk_sigma_to_solver_struct(sum_k, start_sigma)
-
-    # Prints information on correction of Hartree shift
-    first_block = sorted(key for key, _ in loaded_sigma[0])[0]
-    print('DC changed, initial Sigma is the loaded Sigma with corrected Hartree shift:')
-    print('    Sigma for imp0, block "{}", orbital 0 '.format(first_block)
-          + 'shifted from {:.3f} eV '.format(loaded_sigma[0][first_block].data[0, 0, 0].real)
-          + 'to {:.3f} eV'.format(start_sigma[0][first_block].data[0, 0, 0].real))
-
-    # Cleans up
-    sum_k.dc_imp = calculated_dc_imp
-    [sigma_freq.zero() for sigma_freq in sum_k.Sigma_imp]
 
-    return start_sigma
+    assert gw_params['code'] == 'aimbes', 'Only AIMBES is currently supported as gw code'
 
+    iteration = 1
+    # prepare output h5 archive
+    if mpi.is_master_node():
+        with HDFArchive(general_params['jobname'] + '/' + general_params['seedname'] + '.h5', 'a') as ar:
+            if 'DMFT_results' not in ar:
+                ar.create_group('DMFT_results')
+            if 'last_iter' not in ar['DMFT_results']:
+                ar['DMFT_results'].create_group('last_iter')
+            if 'DMFT_input' not in ar:
+                ar.create_group('DMFT_input')
+                ar['DMFT_input']['program'] = 'solid_dmft'
+                ar['DMFT_input'].create_group('solver')
+                ar['DMFT_input'].create_group('version')
+                ar['DMFT_input']['version']['triqs_hash'] = triqs_hash
+                ar['DMFT_input']['version']['triqs_version'] = triqs_version
+                ar['DMFT_input']['version']['solid_dmft_hash'] = solid_dmft_hash
+                ar['DMFT_input']['version']['solid_dmft_version'] = solid_dmft_version
 
-def determine_dc_and_initial_sigma(general_params, advanced_params, sum_k,
-                                   archive, iteration_offset, density_mat_dft, solvers):
-    """
-    Determines the double counting (DC) and the initial Sigma. This can happen
-    in five different ways:
-    * Calculation resumed: use the previous DC and the Sigma of the last complete calculation.
-
-    * Calculation initialized with load_sigma: use the DC and Sigma from the previous file.
-      If the DC changed (and therefore the Hartree shift), the initial Sigma is adjusted by that.
-
-    * New calculation, with DC: calculate the DC, then initialize the Sigma as the DC,
-      effectively starting the calculation from the DFT Green's function.
-      Also breaks magnetic symmetry if calculation is magnetic.
-
-    * New calculation, without DC: Sigma is initialized as 0,
-      starting the calculation from the DFT Green's function.
-
-    Parameters
-    ----------
-    general_params : dict
-        general parameters as a dict
-    advanced_params : dict
-        advanced parameters as a dict
-    sum_k : SumkDFT object
-        Sumk object with the information about the correct block structure
-    archive : HDFArchive
-        the archive of the current calculation
-    iteration_offset : int
-        the iterations done before this calculation
-    density_mat_dft : numpy array
-        DFT density matrix
-    solvers : list
-        list of Solver instances
-
-    Returns
-    -------
-    sum_k : SumkDFT object
-        the SumkDFT object, updated by the initial Sigma and the DC
-    solvers : list
-        list of Solver instances, updated by the initial Sigma
+    # make sure each iteration is saved to h5 file
+    general_params['h5_save_freq'] = 1
 
-    """
-    start_sigma = None
-    last_g0 = None
+    # lad GW input from h5 file
     if mpi.is_master_node():
-        # Resumes previous calculation
-        if iteration_offset > 0:
-            print('\nFrom previous calculation:', end=' ')
-            start_sigma, sum_k.dc_imp, sum_k.dc_energ, last_g0,  _ = _load_sigma_from_h5(archive, -1)
-            if general_params['csc'] and not general_params['dc_dmft']:
-                sum_k = calculate_double_counting(sum_k, density_mat_dft, general_params, advanced_params)
-        # Loads Sigma from different calculation
-        elif general_params['load_sigma']:
-            print('\nFrom {}:'.format(general_params['path_to_sigma']), end=' ')
-            with HDFArchive(general_params['path_to_sigma'], 'r') as sigma_archive:
-                (loaded_sigma, loaded_dc_imp, _,
-                 _, loaded_density_matrix) = _load_sigma_from_h5(sigma_archive, general_params['load_sigma_iter'])
-
-            # Recalculate double counting in case U, J or DC formula changed
-            if general_params['dc']:
-                if general_params['dc_dmft']:
-                    sum_k = calculate_double_counting(sum_k, loaded_density_matrix,
-                                                       general_params, advanced_params)
-                else:
-                    sum_k = calculate_double_counting(sum_k, density_mat_dft,
-                                                       general_params, advanced_params)
-
-            start_sigma = _set_loaded_sigma(sum_k, loaded_sigma, loaded_dc_imp, general_params)
+        gw_data, ir_kernel = convert_gw_output(
+            general_params['jobname'] + '/' + general_params['seedname'] + '.h5',
+            gw_params['h5_file'],
+            it_1e = gw_params['it_1e'],
+            it_2e = gw_params['it_2e'],
+        )
+        gw_params.update(gw_data)
+    mpi.barrier()
+    gw_params = mpi.bcast(gw_params)
+    iteration = gw_params['it_1e']
+
+    # if GW calculation was performed with spin never average spin channels
+    if gw_params['number_of_spins'] == 2:
+        general_params['magnetic'] = True
+
+    # dummy helper class for sumk
+    sumk = dummy_sumk(gw_params['n_inequiv_shells'], gw_params['n_orb'],
+                      general_params['enforce_off_diag'], gw_params['use_rot'],
+                      general_params['magnetic'])
+
+    sumk.mesh = MeshImFreq(beta=gw_params['beta'], statistic='Fermion', n_iw=general_params['n_iw'])
+    sumk.chemical_potential = gw_params['mu_emb']
+    sumk.dc_imp = gw_params['Vhf_dc']
+    general_params['beta'] = gw_params['beta']
+
+    # create h_int
+    general_params = _extract_quantity_per_inequiv('h_int_type', sumk.n_inequiv_shells, general_params)
+    general_params = _extract_quantity_per_inequiv('dc_type', sumk.n_inequiv_shells, general_params)
+
+    h_int, gw_params = interaction_hamiltonian.construct(sumk, general_params, advanced_params, gw_params)
+
+    if len(solver_params) == 1 and solver_params[0]['idx_impurities'] is None:
+        map_imp_solver = [0] * sumk.n_inequiv_shells
+    else:
+        all_idx_imp = [i for entry in solver_params for i in entry['idx_impurities']]
+        if sorted(all_idx_imp) != list(range(sumk.n_inequiv_shells)):
+            raise ValueError('All impurities must be listed exactly once in solver.idx_impurities'
+                             f'but instead got {all_idx_imp}')
+
+        map_imp_solver = []
+        for iineq in range(sumk.n_inequiv_shells):
+            for isolver, entry in enumerate(solver_params):
+                if iineq in entry['idx_impurities']:
+                    map_imp_solver.append(isolver)
+                    break
+    solver_type_per_imp = [solver_params[map_imp_solver[iineq]]['type'] for iineq in range(sumk.n_inequiv_shells)]
+    mpi.report(f'\nSolver type per impurity: {solver_type_per_imp}')
 
-        # Sets DC as Sigma because no initial Sigma given
-        elif general_params['dc']:
-            sum_k = calculate_double_counting(sum_k, density_mat_dft, general_params, advanced_params)
-
-            # initialize Sigma from sum_k
-            if general_params['solver_type'] in ['ftps']:
-                start_sigma = [sum_k.block_structure.create_gf(ish=iineq, gf_function=Gf, space='solver',
-                                                               mesh=sum_k.mesh)
-                               for iineq in range(sum_k.n_inequiv_shells)]
-            else:
-                start_sigma = [sum_k.block_structure.create_gf(ish=iineq, space='solver', mesh=sum_k.mesh)
-                               for iineq in range(sum_k.n_inequiv_shells)]
-            for icrsh in range(sum_k.n_inequiv_shells):
-                dc_value = sum_k.dc_imp[sum_k.inequiv_to_corr[icrsh]][sum_k.spin_block_names[sum_k.SO][0]][0, 0]
-
-                if (general_params['magnetic'] and general_params['magmom'] and sum_k.SO == 0):
-                    # if we are doing a magnetic calculation and initial magnetic moments
-                    # are set, manipulate the initial sigma accordingly
-                    fac = general_params['magmom'][icrsh]
-
-                    # init self energy according to factors in magmoms
-                    # if magmom positive the up channel will be favored
-                    for spin_channel in sum_k.gf_struct_solver[icrsh].keys():
-                        if 'up' in spin_channel:
-                            start_sigma[icrsh][spin_channel] << -fac + dc_value
-                        else:
-                            start_sigma[icrsh][spin_channel] << fac + dc_value
+    # create solver objects
+    solvers = [None] * sumk.n_inequiv_shells
+    if mpi.is_master_node():
+        Sigma_dlr = [None] * sumk.n_inequiv_shells
+        Sigma_dlr_iw = [None] * sumk.n_inequiv_shells
+        ir_mesh_idx = ir_kernel.wn_mesh(stats='f',ir_notation=False)
+        ir_mesh = (2*ir_mesh_idx+1)*np.pi/gw_params['beta']
+        Sigma_ir = np.zeros((len(ir_mesh_idx),
+                             gw_params['number_of_spins'],
+                             sumk.n_inequiv_shells,max(gw_params['n_orb']),max(gw_params['n_orb'])),
+                            dtype=complex)
+        Vhf_imp_sIab = np.zeros((gw_params['number_of_spins'],
+                                 sumk.n_inequiv_shells,
+                                 max(gw_params['n_orb']),max(gw_params['n_orb'])),dtype=complex)
+
+    for ish in range(sumk.n_inequiv_shells):
+        # Construct the Solver instances
+        solvers[ish] = SolverStructure(general_params, solver_params[map_imp_solver[ish]],
+                                       gw_params, advanced_params, sumk, ish, h_int[ish])
+
+    # init local density matrices for observables
+    density_tot = 0.0
+    density_shell = np.zeros(sumk.n_inequiv_shells)
+    density_mat = [None] * sumk.n_inequiv_shells
+    density_mat_unsym = [None] * sumk.n_inequiv_shells
+    density_shell_pre = np.zeros(sumk.n_inequiv_shells)
+    density_mat_pre = [None] * sumk.n_inequiv_shells
+
+    if sumk.SO:
+        printed = ((np.real, 'real'), (np.imag, 'imaginary'))
+    else:
+        printed = ((np.real, 'real'),)
+
+    for ish in range(sumk.n_inequiv_shells):
+        density_shell_pre[ish] = np.real(gw_params['Gloc_dlr'][ish].total_density())
+        mpi.report(
+            '\n *** Correlated Shell type #{:3d} : '.format(ish)
+            + 'Estimated total charge of impurity problem = {:.6f}'.format(density_shell_pre[ish])
+        )
+        density_mat_pre[ish] = gw_params['Gloc_dlr'][ish].density()
+        mpi.report('Estimated density matrix:')
+        for key, value in sorted(density_mat_pre[ish].items()):
+            for func, name in printed:
+                mpi.report('{}, {} part'.format(key, name))
+                mpi.report(func(value))
+
+        if not general_params['enforce_off_diag']:
+            mpi.report('\n*** WARNING: off-diagonal elements are neglected in the impurity solver ***')
+
+        if ((solver_type_per_imp[ish] == 'cthyb' and solver_params[ish]['delta_interface'])
+                or solver_type_per_imp[ish] == 'ctseg'):
+            mpi.report('\n Using the delta interface for passing Delta(tau) and Hloc0 directly to the solver.\n')
+            Gloc_dlr = sumk.block_structure.convert_gf(gw_params['Gloc_dlr'][ish], ish_from=ish, space_from='sumk', space_to='solver')
+            # prepare solver input
+            imp_eal = sumk.block_structure.convert_matrix(gw_params['Hloc0'][ish], ish_from=ish, space_from='sumk', space_to='solver')
+            # fill Delta_time from Delta_freq sumk to solver
+            for name, g0 in Gloc_dlr:
+                G0_dlr_iw = make_gf_dlr_imfreq(g0)
+                # make non-interacting impurity Hamiltonian hermitian
+                imp_eal[name] = (imp_eal[name] + imp_eal[name].T.conj())/2
+                if mpi.is_master_node():
+                    print('H_loc0[{:2d}] block: {}'.format(ish, name))
+                    fmt = '{:11.7f}' * imp_eal[name].shape[0]
+                    for block in imp_eal[name]:
+                        print((' '*11 + fmt).format(*block.real))
+
+                Delta_dlr_iw = Gf(mesh=G0_dlr_iw.mesh, target_shape=g0.target_shape)
+                for iw in G0_dlr_iw.mesh:
+                    Delta_dlr_iw[iw] = iw.value - inverse(G0_dlr_iw[iw]) - imp_eal[name]
+
+                # without SOC delta_tau needs to be real
+                if not sumk.SO == 1:
+                    Delta_dlr = make_gf_dlr(Delta_dlr_iw)
+                    Delta_tau = make_hermitian(make_gf_imtime(Delta_dlr, n_tau=general_params['n_tau']))
+                    # create now full delta(tau)
+                    solvers[ish].Delta_time[name] << Delta_tau.real
                 else:
-                    start_sigma[icrsh] << dc_value
-        # Sets Sigma to zero because neither initial Sigma nor DC given
+                    solvers[ish].Delta_time[name] << Delta_tau
 
-        elif (not general_params['dc'] and general_params['magnetic']):
-            start_sigma = [sum_k.block_structure.create_gf(ish=iineq, gf_function=Gf, space='solver', mesh=sum_k.mesh)
-                                for iineq in range(sum_k.n_inequiv_shells)]
-            for icrsh in range(sum_k.n_inequiv_shells):
-                if (general_params['magnetic'] and general_params['magmom'] and sum_k.SO == 0):
-                    mpi.report(f'\n*** Adding magnetic bias to initial sigma for impurity {icrsh} ***')
-                    # if we are doing a magnetic calculation and initial magnetic moments
-                    # are set, manipulate the initial sigma accordingly
-                    fac = general_params['magmom'][icrsh]
-
-                    # if magmom positive the up channel will be favored
-                    for spin_channel in sum_k.gf_struct_solver[icrsh].keys():
-                        if 'up' in spin_channel:
-                            start_sigma[icrsh][spin_channel] << -fac
+                if solver_params[ish]['diag_delta']:
+                    for o1 in range(imp_eal[name].shape[0]):
+                        for o2 in range(imp_eal[name].shape[0]):
+                            if o1 != o2:
+                                solvers[ish].Delta_time[name].data[:, o1, o2] = 0.0 + 0.0j
+
+            # Make non-interacting operator for Hloc0
+            Hloc_0 = Operator()
+            for spin, spin_block in imp_eal.items():
+                for o1 in range(spin_block.shape[0]):
+                    for o2 in range(spin_block.shape[1]):
+                        # check if off-diag element is larger than threshold
+                        if o1 != o2 and abs(spin_block[o1, o2]) < solver_params[ish]['off_diag_threshold']:
+                            continue
                         else:
-                            start_sigma[icrsh][spin_channel] << fac
+                            # TODO: adapt for SOC calculations, which should keep the imag part
+                            Hloc_0 += spin_block[o1, o2].real / 2 * (c_dag(spin, o1) * c(spin, o2) + c_dag(spin, o2) * c(spin, o1))
+            solvers[ish].Hloc_0 = Hloc_0
         else:
-            if general_params['solver_type'] in ['ftps']:
-                start_sigma = [sum_k.block_structure.create_gf(ish=iineq, gf_function=Gf, space='solver',
-                                                               mesh=sum_k.mesh)
-                               for iineq in range(sum_k.n_inequiv_shells)]
-            else:
-                start_sigma = [sum_k.block_structure.create_gf(ish=iineq, space='solver', mesh=sum_k.mesh)
-                               for iineq in range(sum_k.n_inequiv_shells)]
+            # convert G0 to solver basis
+            G0_dlr = sumk.block_structure.convert_gf(gw_params['G0_dlr'][ish], ish_from=ish, space_from='sumk', space_to='solver')
+            # dyson equation to extract G0_freq, using Hermitian symmetry
+            solvers[ish].G0_freq << make_hermitian(make_gf_imfreq(G0_dlr, n_iw=general_params['n_iw']))
+
+        mpi.report('\nSolving the impurity problem for shell {} ...'.format(ish))
+        mpi.barrier()
+        start_time = timer()
+        solvers[ish].solve()
+        mpi.barrier()
+        mpi.report('Actual time for solver: {:.2f} s'.format(timer() - start_time))
+
+        # some printout of the obtained density matrices and some basic checks from the unsymmetrized solver output
+        density_shell[ish] = np.real(solvers[ish].G_freq_unsym.total_density())
+        density_tot += density_shell[ish]
+        density_mat_unsym[ish] = solvers[ish].G_freq_unsym.density()
+        density_mat[ish] = solvers[ish].G_freq.density()
+        formatter.print_local_density(density_shell[ish], density_shell_pre[ish], density_mat_unsym[ish], sumk.SO)
+        mpi.report('')
 
-    # Adds random, frequency-independent noise in zeroth iteration to break symmetries
-    if not np.isclose(general_params['noise_level_initial_sigma'], 0) and iteration_offset == 0:
+        # post-processing for GW
         if mpi.is_master_node():
-            for start_sigma_per_imp in start_sigma:
-                for _, block in start_sigma_per_imp:
-                    noise = np.random.normal(scale=general_params['noise_level_initial_sigma'],
-                                             size=block.data.shape[1:])
-                    # Makes the noise hermitian
-                    noise = np.broadcast_to(.5 * (noise + noise.T), block.data.shape)
-                    block += Gf(indices=block.indices, mesh=block.mesh, data=noise)
-
-    # bcast everything to other nodes
-    sum_k.dc_imp = mpi.bcast(sum_k.dc_imp)
-    sum_k.dc_energ = mpi.bcast(sum_k.dc_energ)
-    start_sigma = mpi.bcast(start_sigma)
-    last_g0 = mpi.bcast(last_g0)
-    # Loads everything now to the solver
-    for icrsh in range(sum_k.n_inequiv_shells):
-        solvers[icrsh].Sigma_freq = start_sigma[icrsh]
-        if last_g0:
-            solvers[icrsh].G0_freq = last_g0[icrsh]
-
-    # Updates the sum_k object with the Matsubara self-energy
-    sum_k.put_Sigma([solvers[icrsh].Sigma_freq for icrsh in range(sum_k.n_inequiv_shells)])
-    
-    # load sigma as first guess in the hartree solver if applicable
-    if general_params['solver_type'] == 'hartree':
-        # TODO:
-        # should this be moved to before the solve() call? Having it only here means there is a mismatch
-        # between the mixing at the level of the solver and the sumk (solver mixes always 100%)
-        for icrsh in range(sum_k.n_inequiv_shells):
-            mpi.report(f"SOLID_DMFT: setting first guess hartree solver for impurity {icrsh}")
-            solvers[icrsh].triqs_solver.reinitialize_sigma(start_sigma[icrsh])
+            if solver_params[ish]['type'] in ('cthyb', 'ctseg') and solver_params[ish]['crm_dyson_solver']:
+                Sigma_dlr[ish] = make_gf_dlr(solvers[ish].Sigma_dlr)
+            else:
+                Sigma_dlr_iw[ish] = sumk.block_structure.create_gf(ish=ish,
+                                                                   gf_function=Gf,
+                                                                   space='solver',
+                                                                   mesh=gw_params['mesh_dlr_iw_f'])
+                for w in Sigma_dlr_iw[ish].mesh:
+                    for block, gf in Sigma_dlr_iw[ish]:
+                        gf[w] = solvers[ish].Sigma_freq[block](w)-solvers[ish].Sigma_Hartree[block]
+
+                sumk.symm_deg_gf(Sigma_dlr_iw[ish],ish=ish)
+                Sigma_dlr[ish] = make_gf_dlr(Sigma_dlr_iw[ish])
+
+                for i, (block, gf) in enumerate(Sigma_dlr[ish]):
+                    # print Hartree shift
+                    print('Σ_HF {}'.format(block))
+                    fmt = '{:11.7f}' * solvers[ish].Sigma_Hartree[block].shape[0]
+                    for vhf in solvers[ish].Sigma_Hartree[block]:
+                        print((' '*11 + fmt).format(*vhf.real))
+
+                # average Hartree shift if not magnetic
+                if not general_params['magnetic']:
+                    if general_params['enforce_off_diag']:
+                        solvers[ish].Sigma_Hartree['up_0'] = 0.5*(solvers[ish].Sigma_Hartree['up_0']+
+                                                                  solvers[ish].Sigma_Hartree['down_0'])
+                        solvers[ish].Sigma_Hartree['down_0'] = solvers[ish].Sigma_Hartree['up_0']
+                    else:
+                        for iorb in range(gw_params['n_orb'][ish]):
+                            solvers[ish].Sigma_Hartree[f'up_{iorb}'] = 0.5*(solvers[ish].Sigma_Hartree[f'up_{iorb}']+
+                                                                          solvers[ish].Sigma_Hartree[f'down_{iorb}'])
+                            solvers[ish].Sigma_Hartree[f'down_{iorb}'] = solvers[ish].Sigma_Hartree[f'up_{iorb}']
+
+            iw_mesh = solvers[ish].Sigma_freq.mesh
+            # convert Sigma to sumk basis
+            Sigma_dlr_sumk = sumk.block_structure.convert_gf(Sigma_dlr[ish], ish_from=ish, space_from='solver', space_to='sumk')
+            Sigma_Hartree_sumk = sumk.block_structure.convert_matrix(solvers[ish].Sigma_Hartree, ish_from=ish, space_from='solver', space_to='sumk')
+            # store Sigma and V_HF in sumk basis on IR mesh
+            for i, (block, gf) in enumerate(Sigma_dlr_sumk):
+                Vhf_imp_sIab[i,ish] = Sigma_Hartree_sumk[block]
+                for iw in range(len(ir_mesh_idx)):
+                    Sigma_ir[iw,i,ish] = gf(iw_mesh(ir_mesh_idx[iw]))
+
+                if not general_params['magnetic']:
+                    break
 
-    return sum_k, solvers
+    # Writes results to h5 archive
+    if mpi.is_master_node():
+        with HDFArchive(general_params['jobname'] + '/' + general_params['seedname'] + '.h5', 'a') as ar:
+            results_to_archive.write(ar, sumk, general_params, solver_params, solvers,
+                                     map_imp_solver, solver_type_per_imp, iteration,
+                                     False, gw_params['mu_emb'], density_mat_pre, density_mat)
+
+            # store also IR / DLR Sigma
+            ar['DMFT_results/it_{}'.format(iteration)]['ir_mesh'] = ir_mesh
+            ar['DMFT_results/it_{}'.format(iteration)]['Sigma_imp_wsIab'] = Sigma_ir
+            ar['DMFT_results/it_{}'.format(iteration)]['Vhf_imp_sIab'] = Vhf_imp_sIab
+            for ish in range(sumk.n_inequiv_shells):
+                ar['DMFT_results/it_{}'.format(iteration)][f'Sigma_dlr_{ish}'] = Sigma_dlr[ish]
+
+        # write results to GW h5_file
+        with HDFArchive(gw_params['h5_file'],'a') as ar:
+            ar[f'downfold_1e/iter{iteration}']['Sigma_imp_wsIab'] = Sigma_ir
+            ar[f'downfold_1e/iter{iteration}']['Vhf_imp_sIab'] = Vhf_imp_sIab
+
+
+    mpi.report('*** iteration finished ***')
+    mpi.report('#'*80)
+    mpi.barrier()
+    return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/interaction_hamiltonian.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/interaction_hamiltonian.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,92 +31,98 @@
 import os
 import numpy as np
 from itertools import product
 
 # triqs
 from h5 import HDFArchive
 import triqs.utility.mpi as mpi
+from triqs.gf import make_gf_imfreq
 from triqs.operators import util, n, c, c_dag, Operator
 from solid_dmft.dmft_tools import solver
+
+
 try:
     import forktps as ftps
 except ImportError:
     pass
 
-
-def _extract_U_J_list(param_name, n_inequiv_shells, general_params):
-    """
-    Checks if param_name ('U', 'U_prime', or 'J') are a single value or
-    different per inequivalent shell. If just a single value is given,
-    this value is applied to each shell.
-    """
-
-    if not isinstance(param_name, str):
-        formatted_param = ['none' if p == 'none' else '{:.2f}'.format(p)
-                           for p in general_params[param_name]]
-    else:
-        formatted_param = general_params[param_name]
-
-    if len(general_params[param_name]) == 1:
-        mpi.report('Assuming {} = '.format(param_name)
-                   + '{} for all correlated shells'.format(formatted_param[0]))
-        general_params[param_name] *= n_inequiv_shells
-    elif len(general_params[param_name]) == n_inequiv_shells:
-        mpi.report('{} list for correlated shells: {}'.format(param_name, formatted_param))
-    else:
-        raise IndexError('Property list {} '.format(general_params[param_name])
-                         + 'must have length 1 or n_inequiv_shells')
-
-    return general_params
-
-
-def _load_crpa_interaction_matrix(sum_k, filename='UIJKL'):
+def _load_crpa_interaction_matrix(sum_k, general_params, gw_params, filename='UIJKL'):
     """
-    Loads VASP cRPA data to use as an interaction Hamiltonian.
+    Loads  dynamic interaction data to use as an interaction Hamiltonian.
     """
     def _round_to_int(data):
         return (np.array(data) + .5).astype(int)
 
+    if gw_params['code'] == 'Vasp':
     # Loads data from VASP cRPA file
-    print('Loading cRPA matrix from file: '+str(filename))
-    data = np.loadtxt(filename, unpack=True)
-    u_matrix_four_indices = np.zeros(_round_to_int(np.max(data[:4], axis=1)), dtype=complex)
-    for entry in data.T:
-        # VASP switches the order of the indices, ijkl -> ikjl
-        i, k, j, l = _round_to_int(entry[:4])-1
-        u_matrix_four_indices[i, j, k, l] = entry[4] + 1j * entry[5]
-
-    # Slices up the four index U-matrix, separating shells
-    u_matrix_four_indices_per_shell = [None] * sum_k.n_inequiv_shells
-    first_index_shell = 0
-    for ish in range(sum_k.n_corr_shells):
-        icrsh = sum_k.corr_to_inequiv[ish]
-        n_orb = solver.get_n_orbitals(sum_k)[icrsh]['up']
-        u_matrix_temp = u_matrix_four_indices[first_index_shell:first_index_shell+n_orb,
-                                              first_index_shell:first_index_shell+n_orb,
-                                              first_index_shell:first_index_shell+n_orb,
-                                              first_index_shell:first_index_shell+n_orb]
-        # I think for now we should stick with real interactions make real
-        u_matrix_temp.imag = 0.0
-
-        if ish == icrsh:
-            u_matrix_four_indices_per_shell[icrsh] = u_matrix_temp
-        elif not np.allclose(u_matrix_four_indices_per_shell[icrsh], u_matrix_temp, atol=1e-6, rtol=0):
-            # TODO: for some reason, some entries in the matrices differ by a sign. Check that
-            # mpi.report(np.allclose(np.abs(u_matrix_four_indices_per_shell[icrsh]), np.abs(u_matrix_temp),
-            # atol=1e-6, rtol=0))
-            mpi.report('Warning: cRPA matrix for impurity {} '.format(icrsh)
-                       + 'differs for shells {} and {}'.format(sum_k.inequiv_to_corr[icrsh], ish))
-
-        first_index_shell += n_orb
-
-    if not np.allclose(u_matrix_four_indices.shape, first_index_shell):
-        print('Warning: different number of orbitals in cRPA matrix than in calculation.')
+        print('Loading Vasp cRPA matrix from file: '+str(filename))
+        data = np.loadtxt(filename, unpack=True)
+        u_matrix_four_indices = np.zeros(_round_to_int(np.max(data[:4], axis=1)), dtype=complex)
+        for entry in data.T:
+            # VASP switches the order of the indices, ijkl -> ikjl
+            i, k, j, l = _round_to_int(entry[:4])-1
+            u_matrix_four_indices[i, j, k, l] = entry[4] + 1j * entry[5]
+
+        # Slices up the four index U-matrix, separating shells
+        u_matrix_four_indices_per_shell = [None] * sum_k.n_inequiv_shells
+        first_index_shell = 0
+        for ish in range(sum_k.n_corr_shells):
+            icrsh = sum_k.corr_to_inequiv[ish]
+            n_orb = solver.get_n_orbitals(sum_k)[icrsh]['up']
+            u_matrix_temp = u_matrix_four_indices[first_index_shell:first_index_shell+n_orb,
+                                                  first_index_shell:first_index_shell+n_orb,
+                                                  first_index_shell:first_index_shell+n_orb,
+                                                  first_index_shell:first_index_shell+n_orb]
+            # I think for now we should stick with real interactions make real
+            u_matrix_temp.imag = 0.0
+
+            if ish == icrsh:
+                u_matrix_four_indices_per_shell[icrsh] = u_matrix_temp
+            elif not np.allclose(u_matrix_four_indices_per_shell[icrsh], u_matrix_temp, atol=1e-6, rtol=0):
+                # TODO: for some reason, some entries in the matrices differ by a sign. Check that
+                # mpi.report(np.allclose(np.abs(u_matrix_four_indices_per_shell[icrsh]), np.abs(u_matrix_temp),
+                # atol=1e-6, rtol=0))
+                mpi.report('Warning: cRPA matrix for impurity {} '.format(icrsh)
+                           + 'differs for shells {} and {}'.format(sum_k.inequiv_to_corr[icrsh], ish))
+
+            first_index_shell += n_orb
+
+        if not np.allclose(u_matrix_four_indices.shape, first_index_shell):
+            print('Warning: different number of orbitals in cRPA matrix than in calculation.')
+
+    elif gw_params['code'] == 'aimbes':
+        from solid_dmft.gw_embedding.bdft_converter import convert_gw_output
+        u_matrix_four_indices_per_shell = []
+        # lad GW input from h5 file
+        if mpi.is_master_node():
+            if 'Uloc_dlr' not in gw_params:
+                gw_data, ir_kernel = convert_gw_output(
+                    general_params['jobname'] + '/' + general_params['seedname'] + '.h5',
+                    gw_params['h5_file'],
+                    it_1e = gw_params['it_1e'],
+                    it_2e = gw_params['it_2e'],
+                    ha_ev_conv = True
+                )
+                gw_params.update(gw_data)
+            for icrsh in range(sum_k.n_inequiv_shells):
+                # for now we assume that up / down are equal
+                if general_params['h_int_type'][icrsh] in  ('crpa', 'crpa_density_density'):
+                    Uloc_0 = make_gf_imfreq(gw_params['Uloc_dlr'][icrsh]['up'],1)
+                    u_matrix_four_indices_per_shell.append(Uloc_0.data[0,:,:,:,:] + gw_params['Vloc'][icrsh]['up'])
+                else:
+                    u_matrix_four_indices_per_shell.append(gw_params['Vloc'][icrsh]['up'])
+
+                u_matrix_four_indices_per_shell[icrsh] = u_matrix_four_indices_per_shell[icrsh]
+        mpi.barrier()
+        u_matrix_four_indices_per_shell = mpi.bcast(u_matrix_four_indices_per_shell)
+        gw_params = mpi.bcast(gw_params)
+    else:
+        raise ValueError('Unknown code for reading cRPA results: {}'.format(gw_params['code']))
 
-    return u_matrix_four_indices_per_shell
+    return u_matrix_four_indices_per_shell, gw_params
 
 
 # def _adapt_U_2index_for_SO(Umat, Upmat):
 #     """
 #     Changes the two-index U matrices such that for a system consisting of a
 #     single block 'ud' with the entries (1, up), (1, down), (2, up), (2, down),
 #     ... the matrices are consistent with the case without spin-orbit coupling.
@@ -169,15 +175,15 @@
     Umat_full_SO = np.zeros(np.array(Umat_full.shape)*2, dtype=Umat_full.dtype)
     for spin, spin_prime in ((0, 0), (0, 1), (1, 0), (1, 1)):
         Umat_full_SO[spin::2, spin_prime::2, spin::2, spin_prime::2] = Umat_full
 
     return Umat_full_SO
 
 
-def _construct_kanamori(sum_k, general_params, icrsh):
+def _construct_kanamori(sum_k, general_params, solver_type_per_imp, icrsh):
     """
     Constructs the Kanamori interaction Hamiltonian. Only Kanamori does not
     need the full four-index matrix. Therefore, we can construct it directly
     from the parameters U and J.
     """
 
     n_orb = solver.get_n_orbitals(sum_k)[icrsh]['up']
@@ -186,20 +192,21 @@
         n_orb = n_orb // 2
 
     if n_orb not in (2, 3):
         mpi.report('warning: are you sure you want to use the kanamori hamiltonian '
                    + 'outside the t2g or eg manifold?')
 
     # check if Uprime has been specified manually
-    if general_params['U_prime'][icrsh] == 'U-2J':
+    if general_params['U_prime'][icrsh] is None:
         U_prime = general_params['U'][icrsh] - 2.0 * general_params['J'][icrsh]
     else:
         U_prime = general_params['U_prime'][icrsh]
+    mpi.report('U = {:.2f}, U\' = {:.2f}, J = {:.2f}\n'.format(general_params['U'][icrsh], U_prime, general_params['J'][icrsh]))
 
-    if general_params['solver_type'] == 'ftps':
+    if solver_type_per_imp[icrsh] == 'ftps':
         # 1-band modell requires J and U' equals zero
         if n_orb == 1:
             up, j = 0.0, 0.0
         else:
             up = U_prime
             j = general_params['J'][icrsh]
         h_int = ftps.solver_core.HInt(u=general_params['U'][icrsh], j=j, up=up, dd=False)
@@ -208,19 +215,19 @@
         Umat, Upmat = util.U_matrix_kanamori(n_orb=n_orb, U_int=general_params['U'][icrsh],
                                              J_hund=general_params['J'][icrsh],
                                              Up_int=U_prime)
 
         h_int = util.h_int_kanamori(sum_k.spin_block_names[sum_k.SO], n_orb,
                                     map_operator_structure=sum_k.sumk_to_solver[icrsh],
                                     U=Umat, Uprime=Upmat, J_hund=general_params['J'][icrsh],
-                                    H_dump=os.path.join(general_params['jobname'], 'H.txt'))
+                                    H_dump=os.path.join(general_params['jobname'], f'H_imp{icrsh}.txt'))
     else:
         h_int = _construct_kanamori_soc(general_params['U'][icrsh], general_params['J'][icrsh],
                                         n_orb, sum_k.sumk_to_solver[icrsh],
-                                        os.path.join(general_params['jobname'], 'H.txt'))
+                                        os.path.join(general_params['jobname'], f'H_imp{icrsh}.txt'))
     return h_int
 
 
 def _construct_kanamori_soc(U_int, J_hund, n_orb, map_operator_structure, H_dump=None):
     r"""
     Adapted from triqs.operators.util.hamiltonians.h_int_kanamori. Assumes
     that spin_names == ['ud'] and that map_operator_structure is given.
@@ -324,15 +331,15 @@
         raise ValueError('dynamic U not implemented for SO!=0')
     if n_orb > 1:
         raise ValueError('dynamic U not implemented for more than one orbital')
 
     mpi.report('onsite interaction value for imp {}: {:.3f}'.format(icrsh, U_onsite[icrsh]))
     h_int = util.h_int_density(sum_k.spin_block_names[sum_k.SO], n_orb,
                                map_operator_structure=sum_k.sumk_to_solver[icrsh],
-                               U=np.array([[0]]), Uprime=np.array([[U_onsite[icrsh]]]), H_dump=os.path.join(general_params['jobname'], 'H.txt'))
+                               U=np.array([[0]]), Uprime=np.array([[U_onsite[icrsh]]]), H_dump=os.path.join(general_params['jobname'], f'H_imp{icrsh}.txt'))
 
     return h_int
 
 
 def _generate_four_index_u_matrix(sum_k, general_params, icrsh):
     """
     Generates the four-index interaction matrix per impurity with the interaction
@@ -342,69 +349,68 @@
     # ish points to the shell representative of the current group
     ish = sum_k.inequiv_to_corr[icrsh]
     n_orb = solver.get_n_orbitals(sum_k)[icrsh]['up']
     if sum_k.SO == 1:
         assert n_orb % 2 == 0
         n_orb = n_orb // 2
 
-    if sum_k.corr_shells[ish]['l'] != 2:
-        slater_integrals = util.U_J_to_radial_integrals(l=sum_k.corr_shells[ish]['l'],
-                                                        U_int=general_params['U'][icrsh],
+    l = sum_k.corr_shells[ish]['l']
+    if l != 2:
+        slater_integrals = util.U_J_to_radial_integrals(l=l, U_int=general_params['U'][icrsh],
                                                         J_hund=general_params['J'][icrsh])
     else:
         # Implements parameter R=F4/F2. For R=0.63 equivalent to util.U_J_to_radial_integrals
         U = general_params['U'][icrsh]
         J = general_params['J'][icrsh]
         R = general_params['ratio_F4_F2'][icrsh]
-        R = 0.63 if R == 'none' else R
+        R = 0.63 if R is None else R
         slater_integrals = np.array([U, 14*J/(1+R), 14*J*R/(1+R)])
 
     mpi.report('\nImpurity {}: The corresponding slater integrals are'.format(icrsh))
     formatted_slater_integrals = [y for x in list(zip([2*x for x in range(len(slater_integrals))], slater_integrals)) for y in x]
     mpi.report(('F{:d} = {:.2f}, '*len(slater_integrals)).format(*formatted_slater_integrals))
 
     # Constructs U matrix
     # construct full spherical symmetric U matrix and transform to cubic basis
     # the order for the cubic orbitals is given by the convention. The TRIQS
     # convention is as follows ("xy","yz","z^2","xz","x^2-y^2")
     # this is consistent with the order of orbitals in the VASP interface
-    # but not necessarily with wannier90, qe, and wien2k! 
+    # but not necessarily with wannier90, qe, and wien2k!
     # This is also true for the f-shell.
-    Umat_full = util.U_matrix_slater(l=sum_k.corr_shells[ish]['l'],
+    Umat_full = util.U_matrix_slater(l=l,
                               radial_integrals=slater_integrals, basis='spherical')
     Umat_full = util.transform_U_matrix(Umat_full,
-                                        util.spherical_to_cubic(l=sum_k.corr_shells[ish]['l'],
-                                                                convention=general_params['h_int_basis'])
-                                        )
+                                        util.spherical_to_cubic(l=l, convention=general_params['h_int_basis']))
 
-    if n_orb == 2:
+    if l == 2 and n_orb == 2:
         Umat_full = util.eg_submatrix(Umat_full)
         mpi.report('Using eg subspace of interaction Hamiltonian')
-    elif n_orb == 3:
+    elif l == 2 and n_orb == 3:
         Umat_full = util.t2g_submatrix(Umat_full)
         mpi.report('Using t2g subspace of interaction Hamiltonian')
-    elif n_orb not in (5, 7):
-        raise ValueError('Calculations for d shell only support 2, 3 or 5 orbitals'
-                         + 'and for the f shell only 7 orbitals')
+    elif n_orb != 2*l+1:
+        raise ValueError(f'Imp {icrsh}: for the Slater Hamiltonian, please use either '
+                         f'the full shell with 2l+1={2*l+1} orbitals '
+                         'or the t2g or eg subspace of the d shell with 3 or 2 orbitals.')
 
     return Umat_full
 
 
 def _rotate_four_index_matrix(sum_k, general_params, Umat_full, icrsh):
     """ Rotates the four index matrix into the local frame. """
 
     ish = sum_k.inequiv_to_corr[icrsh]
     # Transposes rotation matrix here because TRIQS has a slightly different definition
     Umat_full_rotated = util.transform_U_matrix(Umat_full, sum_k.rot_mat[ish].T)
 
-    if general_params['h_int_type'][icrsh] in ('density_density', 'crpa_density_density'):
+    if general_params['h_int_type'][icrsh] in ('density_density', 'crpa_density_density', 'dyn_density_density'):
         if not np.allclose(Umat_full_rotated, Umat_full):
             mpi.report('WARNING: applying a rotation matrix changes the dens-dens Hamiltonian.\n'
                        + 'This changes the definition of the ignored spin flip and pair hopping.')
-    elif general_params['h_int_type'][icrsh] in ('full_slater', 'crpa'):
+    elif general_params['h_int_type'][icrsh] in ('full_slater', 'crpa', 'dyn_full'):
         if not np.allclose(Umat_full_rotated, Umat_full):
             mpi.report('WARNING: applying a rotation matrix changes the interaction Hamiltonian.\n'
                        + 'Please ensure that the rotation is correct!')
 
     return Umat_full_rotated
 
 
@@ -416,15 +422,15 @@
 
     # Constructs Hamiltonian from Umat_full_rotated
     n_orb = solver.get_n_orbitals(sum_k)[icrsh]['up']
 
     Umat, Upmat = util.reduce_4index_to_2index(Umat_full_rotated)
     h_int = util.h_int_density(sum_k.spin_block_names[sum_k.SO], n_orb,
                                map_operator_structure=sum_k.sumk_to_solver[icrsh],
-                               U=Umat, Uprime=Upmat, H_dump=os.path.join(general_params['jobname'], 'H.txt'))
+                               U=Umat, Uprime=Upmat, H_dump=os.path.join(general_params['jobname'], f'H_imp{icrsh}.txt'))
 
     return h_int
 
 
 def _construct_slater(sum_k, general_params, Umat_full_rotated, icrsh):
     """
     Constructs the full Slater-Hamiltonian from the four-index interaction
@@ -432,20 +438,76 @@
     """
 
     n_orb = solver.get_n_orbitals(sum_k)[icrsh]['up']
 
     h_int = util.h_int_slater(sum_k.spin_block_names[sum_k.SO], n_orb,
                               map_operator_structure=sum_k.sumk_to_solver[icrsh],
                               U_matrix=Umat_full_rotated,
-                              H_dump=os.path.join(general_params['jobname'], 'H.txt'))
+                              H_dump=os.path.join(general_params['jobname'], f'H_imp{icrsh}.txt'))
 
     return h_int
 
+def h_int_simple_intra(spin_names,n_orb,U,off_diag=None,map_operator_structure=None,H_dump=None):
+    r"""
+    Create a simple intra orbital density-density Hamiltonian.
+    (no inter orbital terms)
+
+    .. math::
+        H = \frac{1}{2} \sum_{i \sigma \neq \sigma')} U_{i i}^{\sigma \sigma'} n_{i \sigma} n_{i \sigma'}.
+
+    Parameters
+    ----------
+    spin_names : list of strings
+               Names of the spins, e.g. ['up','down'].
+    n_orb : int
+               Number of orbitals.
+    U : float
+               U value
+    off_diag : boolean
+               Do we have (orbital) off-diagonal elements?
+               If yes, the operators and blocks are denoted by ('spin', 'orbital'),
+               otherwise by ('spin_orbital',0).
+    map_operator_structure : dict
+               Mapping of names of GF blocks names from one convention to another,
+               e.g. {('up', 0): ('up_0', 0), ('down', 0): ('down_0',0)}.
+               If provided, the operators and blocks are denoted by the mapping of ``('spin', 'orbital')``.
+    H_dump : string
+               Name of the file to which the Hamiltonian should be written.
+
+    Returns
+    -------
+    H : Operator
+        The Hamiltonian.
 
-def construct(sum_k, general_params, advanced_params):
+    """
+    from triqs.operators.util.op_struct import get_mkind
+
+    if H_dump:
+        H_dump_file = open(H_dump,'w')
+        H_dump_file.write("Density-density Hamiltonian:" + '\n')
+
+    H = Operator()
+    mkind = get_mkind(off_diag,map_operator_structure)
+    if H_dump: H_dump_file.write("Density-density terms:" + '\n')
+    for s1, s2 in product(spin_names,spin_names):
+        if (s1 is not s2):
+            for a1 in range(n_orb):
+                H_term = 0.5 * U * n(*mkind(s1,a1)) * n(*mkind(s2,a1))
+                H += H_term
+
+                # Dump terms of H
+                if H_dump and not H_term.is_zero():
+                    H_dump_file.write('%s'%(mkind(s1,a1),) + '\t')
+                    H_dump_file.write('%s'%(mkind(s2,a1),) + '\t')
+                    H_dump_file.write(str(U) + '\n')
+
+    return H
+
+
+def construct(sum_k, general_params, solver_type_per_imp,  gw_params=None):
     """
     Constructs the interaction Hamiltonian. Currently implemented are the
     Kanamori Hamiltonian (usually for 2 or 3 orbitals), the density-density and
     the full Slater Hamiltonian (for 2, 3, or 5 orbitals).
     If sum_k.rot_mat is non-identity, we have to consider rotating the interaction
     Hamiltonian: the Kanamori Hamiltonian does not change because it is invariant
     under orbital mixing but all the other Hamiltonians are at most invariant
@@ -462,50 +524,38 @@
     orbitals matters. The correct order is specified here:
     triqs.github.io/triqs/unstable/documentation/python_api/triqs.operators.util.U_matrix.spherical_to_cubic.html
     """
 
     # Extracts U and J
     mpi.report('*** interaction parameters ***')
 
-    general_params = _extract_U_J_list('h_int_type', sum_k.n_inequiv_shells, general_params)
-    for param_name in ('U', 'J'):
-        general_params = _extract_U_J_list(param_name, sum_k.n_inequiv_shells, general_params)
-    if 'kanamori' in general_params['h_int_type']:
-        general_params = _extract_U_J_list('U_prime', sum_k.n_inequiv_shells, general_params)
-    for param_name in ('dc_U', 'dc_J'):
-        advanced_params = _extract_U_J_list(param_name, sum_k.n_inequiv_shells, advanced_params)
-
-    # Extracts ratio_F4_F2 if any shell uses a solver supporting it
-    if 'density_density' in general_params['h_int_type'] or 'full_slater' in general_params['h_int_type']:
-        general_params = _extract_U_J_list('ratio_F4_F2', sum_k.n_inequiv_shells, general_params)
-
     # Constructs the interaction Hamiltonian. Needs to come after setting sum_k.rot_mat
     mpi.report('\nConstructing the interaction Hamiltonians')
     h_int = [None] * sum_k.n_inequiv_shells
     for icrsh in range(sum_k.n_inequiv_shells):
         mpi.report('\nImpurity {}: constructing a {} type interaction Hamiltonian'.format(icrsh, general_params['h_int_type'][icrsh]))
 
         # Kanamori
         if general_params['h_int_type'][icrsh] == 'kanamori':
-            h_int[icrsh] = _construct_kanamori(sum_k, general_params, icrsh)
+            h_int[icrsh] = _construct_kanamori(sum_k, general_params, solver_type_per_imp, icrsh)
             continue
 
         # for density density or full slater get full four-index U matrix
         if general_params['h_int_type'][icrsh] in ('density_density', 'full_slater'):
             mpi.report('\nNote: The input parameters U and J here are orbital-averaged parameters.')
             mpi.report('Note: The order of the orbitals is important. See also the doc string of this method.')
-            # Checks that all entries are l == 2 or R == 'none'
+            # Checks that all entries are l == 2 or R is None
             if (sum_k.corr_shells[sum_k.inequiv_to_corr[icrsh]]['l'] != 2
-                    and general_params['ratio_F4_F2'][icrsh] != 'none'):
+                    and general_params['ratio_F4_F2'][icrsh] is not None):
                 raise ValueError('Ratio F4/F2 only implemented for d-shells '
                                  + 'but set in impurity {}'.format(icrsh))
 
-            if general_params['h_int_type'][icrsh] == 'density_density' and general_params['solver_type'] == 'ftps':
+            if general_params['h_int_type'][icrsh] == 'density_density' and solver_type_per_imp[icrsh] == 'ftps':
                 # TODO: implement
-                raise NotImplementedError('\nNote: Density-density not implemented for ftps.')
+                raise NotImplementedError('Note: Density-density not implemented for ftps.')
 
             Umat_full = _generate_four_index_u_matrix(sum_k, general_params, icrsh)
 
             if sum_k.SO == 1:
                 Umat_full = [_adapt_U_4index_for_SO(Umat_full_per_imp)
                              for Umat_full_per_imp in Umat_full]
 
@@ -524,33 +574,39 @@
         if general_params['h_int_type'][icrsh] == 'ntot':
             n_tot_op = Operator()
             for block, n_orb in sum_k.gf_struct_solver[icrsh].items():
                 n_tot_op += sum(n(block, orb) for orb in range(n_orb))
             h_int[icrsh] = general_params['U'][icrsh]/2.0 * (n_tot_op*n_tot_op - n_tot_op)
             continue
 
+        if general_params['h_int_type'][icrsh] == 'simple_intra':
+            h_int[icrsh] = h_int_simple_intra(sum_k.spin_block_names[sum_k.SO],
+                                              solver.get_n_orbitals(sum_k)[icrsh]['up'],
+                                              map_operator_structure=sum_k.sumk_to_solver[icrsh],
+                                              U=general_params['U'][icrsh],
+                                              H_dump=os.path.join(general_params['jobname'], f'H_imp{icrsh}.txt'))
+            continue
+
+
         # read from file options
-        if general_params['h_int_type'][icrsh] in ('crpa', 'crpa_density_density'):
-            Umat_full = _load_crpa_interaction_matrix(sum_k, icrsh)
+        if general_params['h_int_type'][icrsh] in ('crpa', 'crpa_density_density', 'dyn_density_density', 'dyn_full'):
+            Umat_full, gw_params = _load_crpa_interaction_matrix(sum_k, general_params, gw_params)
 
             if sum_k.SO == 1:
-                Umat_full = [_adapt_U_4index_for_SO(Umat_full_per_imp)
-                             for Umat_full_per_imp in Umat_full]
+                Umat_full[icrsh] = _adapt_U_4index_for_SO(Umat_full[icrsh])
 
             # Rotates the interaction matrix
-            Umat_full_rotated = _rotate_four_index_matrix(sum_k, general_params, Umat_full, icrsh)
-    
+            if sum_k.use_rotations:
+                Umat_full[icrsh] = _rotate_four_index_matrix(sum_k, general_params, Umat_full[icrsh], icrsh)
+                Umat_full[icrsh][np.abs(Umat_full[icrsh]) < general_params['U_crpa_threshold']] = 0.0
+
+            gw_params['U_matrix_rot']= Umat_full
             # construct slater / density density from U tensor
-            if general_params['h_int_type'][icrsh] == 'crpa':
-                h_int[icrsh] = _construct_slater(sum_k, general_params, Umat_full_rotated, icrsh)
+            if general_params['h_int_type'][icrsh] in ('crpa', 'dyn_full'):
+                h_int[icrsh] = _construct_slater(sum_k, general_params, Umat_full[icrsh].real, icrsh)
             else:
-                h_int[icrsh] = _construct_density_density(sum_k, general_params, Umat_full_rotated, icrsh)
-            continue
-
-        # dynamic interaction from file
-        if general_params['h_int_type'][icrsh] == 'dynamic':
-            h_int[icrsh] = _construct_dynamic(sum_k, general_params, icrsh)
+                h_int[icrsh] = _construct_density_density(sum_k, general_params, Umat_full[icrsh].real, icrsh)
             continue
 
         raise NotImplementedError('Error when constructing the interaction Hamiltonian.')
 
-    return h_int
+    return h_int, gw_params
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/legendre_filter.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/legendre_filter.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 Contains all the functions related to setting the chemical potential in the
 next iteration.
 """
 
 import numpy as np
 
 import triqs.utility.mpi as mpi
-from triqs.gf import BlockGf, GfImFreq, GfImTime, Fourier
+from triqs.gf import BlockGf, GfImFreq, GfImTime, Fourier, MeshImFreq
 try:
     if mpi.is_master_node():
         from solid_dmft.postprocessing import maxent_gf_latt
     imported_maxent = True
 except ImportError:
     imported_maxent = False
 
@@ -253,15 +253,15 @@
     # Determines band edges for conduction and valence band
     edge_threshold = 0.2
     conduction_edge = _determine_band_edge(mesh, spectral_function, spectral_func_threshold, False, edge_threshold)
     valence_edge = _determine_band_edge(mesh, spectral_function, spectral_func_threshold, True, edge_threshold)
 
     return sum_k.chemical_potential + (valence_edge + conduction_edge) / 2
 
-def set_initial_mu(general_params, sum_k, iteration_offset, archive, shell_multiplicity):
+def set_initial_mu(general_params, sum_k, iteration_offset, archive, broadening):
     """
     Handles the different ways of setting the initial chemical potential mu:
     * Chemical potential set to fixed value: uses this value
 
     * New calculation: determines mu from dichotomy method
 
     * Resuming calculation and chemical potential not updated this iteration:
@@ -278,37 +278,31 @@
         general parameters as dict.
     sum_k : SumkDFT object
         contains system information necessary to determine the initial mu.
     iteration_offset : int
         the number of iterations executed in previous calculations.
     archive : HDFArchive
         needed to potentially load previous results and write MaxEnt results to.
-    shell_multiplicity : iterable of ints
-        number of equivalent shells per impurity.
 
     Returns
     -------
     sum_k : SumkDFT object
         the altered SumkDFT object with the initial mu set correctly.
     """
 
     # Uses fixed_mu_value as chemical potential if parameter is given
-    if general_params['fixed_mu_value'] != 'none':
+    if general_params['fixed_mu_value'] is not None:
         sum_k.set_mu(general_params['fixed_mu_value'])
         mpi.report('+++ Keeping the chemical potential fixed at {:.3f} eV +++'.format(general_params['fixed_mu_value']))
         return sum_k
 
     # In first iteration, determines mu and returns
     if iteration_offset == 0:
-        if general_params['dc'] and general_params['dc_type'] == 4:
-            return sum_k
-        if general_params['solver_type'] in ['ftps']:
-            sum_k.calc_mu(precision=general_params['prec_mu'], broadening=general_params['eta'])
-        else:
-            sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'])
+        sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'],
+                      broadening=broadening)
         return sum_k
 
     # If continuing calculation and not updating mu, loads sold value
     if iteration_offset % general_params['mu_update_freq'] != 0:
         if mpi.is_master_node():
             sum_k.chemical_potential = archive['DMFT_results/last_iter/chemical_potential_pre']
         sum_k.chemical_potential = mpi.bcast(sum_k.chemical_potential)
@@ -320,19 +314,18 @@
     # chemical_potential_pre from the last run
     previous_mu = None
     if mpi.is_master_node():
         previous_mu = archive['DMFT_results/last_iter/chemical_potential_pre']
     previous_mu = mpi.bcast(previous_mu)
 
     # Runs maxent if spectral weight too low and occupation is close to desired one
-    # TODO: which solvers work?
-    if general_params['solver_type'] in ['cthyb', 'ctint'] and general_params['mu_gap_gb2_threshold'] != 'none':
+    if isinstance(sum_k.mesh, MeshImFreq) and general_params['mu_gap_gb2_threshold'] is not None:
         sum_k.chemical_potential = previous_mu
         gf_lattice_iw, g_betahalf, occupation = _initialize_lattice_gf(sum_k, general_params)
-        fulfills_occupation_crit = (general_params['mu_gap_occ_deviation'] == 'none'
+        fulfills_occupation_crit = (general_params['mu_gap_occ_deviation'] is None
                                     or np.abs(occupation - sum_k.density_required) < general_params['mu_gap_occ_deviation'])
 
         if -np.real(g_betahalf) < general_params['mu_gap_gb2_threshold'] and fulfills_occupation_crit:
             new_mu = _set_mu_to_gap_middle_with_maxent(general_params, sum_k, gf_lattice_iw, archive)
             new_mu = mpi.bcast(new_mu)
             if new_mu is not None:
                 sum_k.chemical_potential = new_mu
@@ -341,27 +334,25 @@
     # Calculates occupation for mu mixing below
     elif np.isclose(general_params['mu_mix_per_occupation_offset'], 0):
         occupation = 0 # The occupation does not matter in this case
     else:
         _, _, occupation = _initialize_lattice_gf(sum_k, general_params)
 
     # If system not gapped, gets chemical potential from dichotomy method
-    if general_params['solver_type'] in ['ftps']:
-        sum_k.calc_mu(precision=general_params['prec_mu'], broadening=general_params['eta'])
-    else:
-        sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'])
+    sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'],
+                  broadening=broadening)
 
     # Applies mu mixing to dichotomy result
     sum_k.chemical_potential = _mix_chemical_potential(general_params, occupation,
                                                        sum_k.density_required,
                                                        previous_mu, sum_k.chemical_potential)
 
     return sum_k
 
-def update_mu(general_params, sum_k, it, archive):
+def update_mu(general_params, sum_k, it, archive, broadening):
     """
     Handles the different ways of updating the chemical potential mu:
     * Chemical potential set to fixed value: uses this value
 
     * Chemical potential not updated this iteration: nothing happens.
 
     * Chemical potential is updated: checks if the system is gapped and
@@ -382,30 +373,30 @@
     Returns
     -------
     sum_k : SumkDFT object
         the altered SumkDFT object with the updated mu.
     """
 
     # Uses fixed_mu_value as chemical potential if parameter is given
-    if general_params['fixed_mu_value'] != 'none':
+    if general_params['fixed_mu_value'] is not None:
         sum_k.set_mu(general_params['fixed_mu_value'])
         mpi.report('+++ Keeping the chemical potential fixed at {:.3f} eV +++'.format(general_params['fixed_mu_value']))
         return sum_k
 
     # If mu won't be updated this step, don't update it...
     if it % general_params['mu_update_freq'] != 0:
         mpi.report('Chemical potential not updated this step, '
                    + 'reusing previous one of {:.3f} eV'.format(sum_k.chemical_potential))
         return sum_k
 
     # Runs maxent if spectral weight too low and occupation is close to desired one
     # TODO: which solvers work?
-    if general_params['solver_type'] in ['cthyb', 'ctint','ctseg'] and general_params['mu_gap_gb2_threshold'] != 'none':
+    if isinstance(sum_k.mesh, MeshImFreq) and general_params['mu_gap_gb2_threshold'] is not None:
         gf_lattice_iw, g_betahalf, occupation = _initialize_lattice_gf(sum_k, general_params)
-        fulfills_occupation_crit = (general_params['mu_gap_occ_deviation'] == 'none'
+        fulfills_occupation_crit = (general_params['mu_gap_occ_deviation'] is None
                                     or np.abs(occupation - sum_k.density_required) < general_params['mu_gap_occ_deviation'])
 
         if -np.real(g_betahalf) < general_params['mu_gap_gb2_threshold'] and fulfills_occupation_crit:
             new_mu = _set_mu_to_gap_middle_with_maxent(general_params, sum_k, gf_lattice_iw, archive)
             new_mu = mpi.bcast(new_mu)
             if new_mu is not None:
                 sum_k.chemical_potential = new_mu
@@ -415,18 +406,16 @@
     elif np.isclose(general_params['mu_mix_per_occupation_offset'], 0):
         occupation = 0 # The occupation does not matter in this case
     else:
         _, _, occupation = _initialize_lattice_gf(sum_k, general_params)
 
     # If system not gapped, gets chemical potential from dichotomy method
     previous_mu = sum_k.chemical_potential
-    if general_params['solver_type'] in ['ftps']:
-        sum_k.calc_mu(precision=general_params['prec_mu'], broadening=general_params['eta'])
-    else:
-        sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'])
+    sum_k.calc_mu(precision=general_params['prec_mu'], method=general_params['calc_mu_method'],
+                  broadening=broadening)
 
     # Applies mu mixing to dichotomy result
     sum_k.chemical_potential = _mix_chemical_potential(general_params, occupation,
                                                        sum_k.density_required,
                                                        previous_mu, sum_k.chemical_potential)
     mpi.barrier()
     return sum_k
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/matheval.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/matheval.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/observables.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/observables.py`

 * *Files 13% similar despite different names*

```diff
@@ -142,41 +142,43 @@
 
     for file_name, header in headers.items():
         path = os.path.join(general_params['jobname'], file_name)
         with open(path, 'w') as obs_file:
             obs_file.write(header + '\n')
 
 
-def add_dft_values_as_zeroth_iteration(observables, general_params, dft_mu, dft_energy,
-                                       sum_k, G_loc_all_dft, density_mat_dft, shell_multiplicity):
+def add_dft_values_as_zeroth_iteration(observables, general_params, solver_type_per_imp, dft_mu, dft_energy,
+                                       sum_k, G_loc_all_dft, shell_multiplicity):
     """
     Calculates the DFT observables that should be written as the zeroth iteration.
 
     Parameters
     ----------
     observables : observable arrays/dicts
 
     general_params : general parameters as a dict
 
+    solver_type_per_imp : list of strings
+        list of solver types for each impurity
+
     dft_mu : dft chemical potential
 
     sum_k : SumK Object instances
 
     G_loc_all_dft : Gloc from DFT for G(beta/2)
 
-    density_mat_dft : occupations from DFT
-
     shell_multiplicity : degeneracy of impurities
 
     Returns
     -------
 
     observables: list of dicts
     """
     dft_energy = 0.0 if dft_energy is None else dft_energy
+    density_mat_dft = [G_loc_all_dft[iineq].density() for iineq in range(sum_k.n_inequiv_shells)]
     observables['iteration'].append(0)
     observables['mu'].append(float(dft_mu))
 
     if general_params['calc_energies']:
         observables['E_bandcorr'].append(0.0)
         observables['E_corr_en'].append(0.0)
         observables['E_dft'].append(dft_energy)
@@ -205,15 +207,15 @@
             # iterate over all spin channels and add the to up or down
             # we need only the keys of the blocks, but sorted! Otherwise
             # orbitals will be mixed up_0 to down_0 etc.
             for spin_channel in sorted(sum_k.gf_struct_solver[iineq].keys()):
                 if not spin in spin_channel:
                     continue
 
-                if general_params['solver_type'] in ['ftps']:
+                if solver_type_per_imp[iineq] == 'ftps':
                     freq_mesh = np.array([w.value for w in G_loc_all_dft[iineq][spin_channel].mesh])
                     fermi_idx = abs(freq_mesh).argmin()
                     gb2_averaged = G_loc_all_dft[iineq][spin_channel].data[fermi_idx].imag
 
                     # Z is not defined without Sigma, adding 1
                     Z_per_orbital.extend( [1.0] * G_loc_all_dft[iineq][spin_channel].target_shape[0]  )
                 else:
@@ -253,15 +255,15 @@
         observables['E_tot'].append(dft_energy - sum([dc_per_imp[0] for dc_per_imp in observables['E_DC']]))
     else:
         observables['E_tot'].append('none')
 
     return observables
 
 
-def add_dmft_observables(observables, general_params, solver_params, dft_energy, it, solvers, h_int,
+def add_dmft_observables(observables, general_params, solver_params, map_imp_solver, solver_type_per_imp, dft_energy, it, solvers, h_int,
                          previous_mu, sum_k, density_mat, shell_multiplicity, E_bandcorr):
     """
     calculates the observables for given Input, I decided to calculate the observables
     not adhoc since it should be done only once by the master_node
 
     Parameters
     ----------
@@ -299,58 +301,51 @@
 
     # now the normal output from each iteration
     observables['iteration'].append(it)
     observables['mu'].append(float(previous_mu))
     observables['E_bandcorr'].append(E_bandcorr)
     observables['E_dft'].append(dft_energy)
 
-    # if density matrix was measured store result in observables
-    if general_params['solver_type'] in ['cthyb', 'hubbardI'] and solver_params["measure_density_matrix"]:
-        mpi.report("\nextracting the impurity density matrix")
-        # Extract accumulated density matrix
-        density_matrix = [solvers[icrsh].density_matrix for icrsh in range(sum_k.n_inequiv_shells)]
-        # Object containing eigensystem of the local Hamiltonian
-        diag_local_ham = [solvers[icrsh].h_loc_diagonalization for icrsh in range(sum_k.n_inequiv_shells)]
-
     if general_params['calc_energies']:
-        # dmft interaction energy with E_int = 0.5 * Tr[Sigma * G]
-        if (general_params['solver_type'] in ['cthyb', 'hubbardI']
-            and solver_params["measure_density_matrix"]):
-            E_int = [trace_rho_op(density_matrix[icrsh], h_int[icrsh], diag_local_ham[icrsh])
-                     for icrsh in range(sum_k.n_inequiv_shells)]
-        elif general_params['solver_type'] == 'hartree':
-            E_int = [solvers[icrsh].interaction_energy for icrsh in range(sum_k.n_inequiv_shells)]
-        else:
-            warning = ( "!-------------------------------------------------------------------------------------------!\n"
-                        "! WARNING: calculating interaction energy using Migdal formula                              !\n"
-                        "! consider turning on measure density matrix to use the more stable trace_rho_op function   !\n"
-                        "!-------------------------------------------------------------------------------------------!" )
-            print(warning)
-            # calc energy for given S and G
-            E_int = [0.5 * np.real((solvers[icrsh].G_freq * solvers[icrsh].Sigma_freq).total_density())
-                     for icrsh in range(sum_k.n_inequiv_shells)]
-
+        mpi.report('\nCalculating interaction energies')
         for icrsh in range(sum_k.n_inequiv_shells):
-            observables['E_int'][icrsh].append(shell_multiplicity[icrsh]*E_int[icrsh].real)
-            E_corr_en += shell_multiplicity[icrsh] * (E_int[icrsh].real - sum_k.dc_energ[sum_k.inequiv_to_corr[icrsh]])
+            if (solver_type_per_imp[icrsh] in ['cthyb', 'hubbardI']
+                    and solver_params[map_imp_solver[icrsh]]["measure_density_matrix"]):
+                mpi.report(f'    Imp {icrsh}: from impurity density matrix')
+                # Extract accumulated density matrix
+                density_matrix = solvers[icrsh].density_matrix
+                # Object containing eigensystem of the local Hamiltonian
+                diag_local_ham = solvers[icrsh].h_loc_diagonalization
+                E_int = trace_rho_op(density_matrix, h_int[icrsh], diag_local_ham)
+            elif solver_type_per_imp[icrsh] == 'hartree':
+                mpi.report(f'    Imp {icrsh}: from Hartree')
+                E_int = solvers[icrsh].interaction_energy
+            else:
+                mpi.report(f'    Imp {icrsh}: from Migdal formula. '
+                           'WARNING: less stable than measuring density matrix and using trace_rho_op!')
+                # calc energy for given S and G
+                # dmft interaction energy with E_int = 0.5 * Tr[Sigma * G]
+                E_int = 0.5 * np.real((solvers[icrsh].G_freq * solvers[icrsh].Sigma_freq).total_density())
 
+            observables['E_int'][icrsh].append(shell_multiplicity[icrsh]*E_int.real)
+            E_corr_en += shell_multiplicity[icrsh] * (E_int.real - sum_k.dc_energ[sum_k.inequiv_to_corr[icrsh]])
 
     observables['E_corr_en'].append(E_corr_en)
 
     # calc total energy
     E_tot = dft_energy + E_bandcorr + E_corr_en
     observables['E_tot'].append(E_tot)
 
     for icrsh in range(sum_k.n_inequiv_shells):
         if general_params['dc']:
             observables['E_DC'][icrsh].append(shell_multiplicity[icrsh]*sum_k.dc_energ[sum_k.inequiv_to_corr[icrsh]])
         else:
             observables['E_DC'][icrsh].append(0.0)
 
-        if general_params['solver_type'] not in ['ftps']:
+        if solver_type_per_imp[icrsh] != 'ftps':
             if solvers[icrsh].G_time:
                 G_time = solvers[icrsh].G_time
             else:
                 G_time = solvers[icrsh].G_time_orig
 
         # Collect all occupation and G(beta/2) for spin up and down separately
         for spin in sum_k.spin_block_names[sum_k.SO]:
@@ -360,15 +355,15 @@
             occupation_per_orbital = []
             Z_per_orbital = []
 
             # iterate over all spin channels and add the to up or down
             for spin_channel in sorted(sum_k.gf_struct_solver[icrsh].keys()):
                 if not spin in spin_channel:
                     continue
-                if general_params['solver_type'] in ['ftps']:
+                if solver_type_per_imp[icrsh] == 'ftps':
                     freq_mesh = np.array([w.value for w in solvers[icrsh].G_freq[spin_channel].mesh])
                     fermi_idx = abs(freq_mesh).argmin()
                     gb2_averaged = solvers[icrsh].G_freq[spin_channel].data[fermi_idx].imag
 
                     # Z is not defined without Sigma, adding 1
                     Z_per_orbital.extend( [1.0] * solvers[icrsh].G_freq[spin_channel].target_shape[0]  )
                 else:
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/results_to_archive.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/results_to_archive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 #
 # solid_dmft - A versatile python wrapper to perform DFT+DMFT calculations
 #              utilizing the TRIQS software library
 #
 # Copyright (C) 2018-2020, ETH Zurich
 # Copyright (C) 2021, The Simons Foundation
@@ -23,15 +22,15 @@
 #
 ################################################################################
 
 import os
 import triqs.utility.mpi as mpi
 
 
-def _compile_information(sum_k, general_params, solver_params, solvers,
+def _compile_information(sum_k, general_params, solver_params, solvers, map_imp_solver, solver_type_per_imp,
                          previous_mu, density_mat_pre, density_mat, deltaN, dens):
     """ Collects all results in a dictonary. """
 
     write_to_h5 = {'chemical_potential_post': sum_k.chemical_potential,
                    'chemical_potential_pre': previous_mu,
                    'DC_pot': sum_k.dc_imp,
                    'DC_energ': sum_k.dc_energ,
@@ -40,80 +39,98 @@
                   }
 
     if deltaN is not None:
         write_to_h5['deltaN'] = deltaN
     if dens is not None:
         write_to_h5['deltaN_trace'] = dens
 
+    if any(str(entry) in ('crpa_dynamic') for entry in general_params['dc_type']):
+        write_to_h5['DC_pot_dyn'] = sum_k.dc_imp_dyn
+
     for icrsh in range(sum_k.n_inequiv_shells):
-        if general_params['solver_type'] in ['cthyb', 'hubbardI']:
+        isolvsec = map_imp_solver[icrsh]
+        if solver_type_per_imp[icrsh] in ['cthyb', 'hubbardI']:
             write_to_h5['Delta_time_{}'.format(icrsh)] = solvers[icrsh].Delta_time
 
             # Write the full density matrix to last_iter only - it is large
-            if solver_params['measure_density_matrix']:
+            if solver_params[isolvsec]['measure_density_matrix']:
                 write_to_h5['full_dens_mat_{}'.format(icrsh)] = solvers[icrsh].density_matrix
                 write_to_h5['h_loc_diag_{}'.format(icrsh)] = solvers[icrsh].h_loc_diagonalization
+                if solver_type_per_imp[icrsh] in ('cthyb','hubbardI'):
+                    write_to_h5['Sigma_moments_{}'.format(icrsh)] = solvers[icrsh].Sigma_moments
+                    write_to_h5['G_moments_{}'.format(icrsh)] = solvers[icrsh].G_moments
+                    write_to_h5['Sigma_Hartree_{}'.format(icrsh)] = solvers[icrsh].Sigma_Hartree
 
-        elif general_params['solver_type'] in ['ftps']:
+        elif solver_type_per_imp[icrsh] == 'ftps':
             write_to_h5['Delta_freq_{}'.format(icrsh)] = solvers[icrsh].Delta_freq
 
         write_to_h5['Gimp_time_{}'.format(icrsh)] = solvers[icrsh].G_time
         write_to_h5['G0_freq_{}'.format(icrsh)] = solvers[icrsh].G0_freq
         write_to_h5['Gimp_freq_{}'.format(icrsh)] = solvers[icrsh].G_freq
         write_to_h5['Sigma_freq_{}'.format(icrsh)] = solvers[icrsh].Sigma_freq
 
-        if general_params['solver_type'] == 'cthyb':
-            if solver_params['measure_pert_order']:
+        if solver_type_per_imp[icrsh] == 'cthyb':
+            if solver_params[isolvsec]['measure_pert_order']:
                 write_to_h5['pert_order_imp_{}'.format(icrsh)] = solvers[icrsh].perturbation_order
                 write_to_h5['pert_order_total_imp_{}'.format(icrsh)] = solvers[icrsh].perturbation_order_total
 
-            if general_params['measure_chi'] != 'none':
-                write_to_h5['O_{}_time_{}'.format(general_params['measure_chi'], icrsh)] = solvers[icrsh].O_time
+            if solver_params[isolvsec]['measure_chi'] is not None:
+                write_to_h5['O_{}_time_{}'.format(solver_params[isolvsec]['measure_chi'], icrsh)] = solvers[icrsh].O_time
 
             # if legendre was set, that we have both now!
-            if (solver_params['measure_G_l']
-                or not solver_params['perform_tail_fit'] and general_params['legendre_fit']):
+            if (solver_params[isolvsec]['measure_G_l']
+                or not solver_params[isolvsec]['perform_tail_fit'] and solver_params[isolvsec]['legendre_fit']):
                 write_to_h5['G_time_orig_{}'.format(icrsh)] = solvers[icrsh].G_time_orig
                 write_to_h5['Gimp_l_{}'.format(icrsh)] = solvers[icrsh].G_l
 
-        if general_params['solver_type'] == 'ctint' and solver_params['measure_histogram']:
+            if solver_params[isolvsec]['crm_dyson_solver']:
+                write_to_h5['G_time_dlr_{}'.format(icrsh)] = solvers[icrsh].G_time_dlr
+                write_to_h5['Sigma_dlr_{}'.format(icrsh)] = solvers[icrsh].Sigma_dlr
+
+        if solver_type_per_imp[icrsh] == 'ctint' and solver_params[isolvsec]['measure_histogram']:
             write_to_h5['pert_order_imp_{}'.format(icrsh)] = solvers[icrsh].perturbation_order
 
-        if general_params['solver_type'] == 'hubbardI':
+        if solver_type_per_imp[icrsh] == 'hubbardI':
             write_to_h5['G0_Refreq_{}'.format(icrsh)] = solvers[icrsh].G0_Refreq
             write_to_h5['Gimp_Refreq_{}'.format(icrsh)] = solvers[icrsh].G_Refreq
             write_to_h5['Sigma_Refreq_{}'.format(icrsh)] = solvers[icrsh].Sigma_Refreq
 
-            if solver_params['measure_G_l']:
+            if solver_params[isolvsec]['measure_G_l']:
                 write_to_h5['Gimp_l_{}'.format(icrsh)] = solvers[icrsh].G_l
 
-        if general_params['solver_type'] == 'hartree':
+        if solver_type_per_imp[icrsh] == 'hartree':
             write_to_h5['Sigma_Refreq_{}'.format(icrsh)] = solvers[icrsh].Sigma_Refreq
 
-        if general_params['solver_type'] == 'ctseg':
+        if solver_type_per_imp[icrsh] == 'ctseg':
             # if legendre was set, that we have both now!
-            if (solver_params['measure_gl'] or general_params['legendre_fit']):
+            if (solver_params[isolvsec]['legendre_fit']):
                 write_to_h5['G_time_orig_{}'.format(icrsh)] = solvers[icrsh].G_time_orig
                 write_to_h5['Gimp_l_{}'.format(icrsh)] = solvers[icrsh].G_l
-            if solver_params['measure_ft']:
+            if solver_params[isolvsec]['improved_estimator']:
                 write_to_h5['F_freq_{}'.format(icrsh)] = solvers[icrsh].F_freq
                 write_to_h5['F_time_{}'.format(icrsh)] = solvers[icrsh].F_time
+            if solver_params[isolvsec]['crm_dyson_solver']:
+                write_to_h5['G_time_dlr_{}'.format(icrsh)] = solvers[icrsh].G_time_dlr
+                write_to_h5['Sigma_dlr_{}'.format(icrsh)] = solvers[icrsh].Sigma_dlr
+            if general_params['h_int_type'][icrsh] == 'dyn_density_density':
+                write_to_h5['D0_time_{}'.format(icrsh)] = solvers[icrsh].triqs_solver.D0_tau
+                write_to_h5['Jperp_time_{}'.format(icrsh)] = solvers[icrsh].triqs_solver.Jperp_tau
 
     return write_to_h5
 
-def write(archive, sum_k, general_params, solver_params, solvers, it, is_sampling,
+def write(archive, sum_k, general_params, solver_params, solvers, map_imp_solver, solver_type_per_imp, it, is_sampling,
           previous_mu, density_mat_pre, density_mat, deltaN=None, dens=None):
     """
     Collects and writes results to archive.
     """
 
     if not mpi.is_master_node():
         return
 
-    write_to_h5 = _compile_information(sum_k, general_params, solver_params, solvers,
+    write_to_h5 = _compile_information(sum_k, general_params, solver_params, solvers, map_imp_solver, solver_type_per_imp,
                                        previous_mu, density_mat_pre, density_mat, deltaN, dens)
 
     # Saves the results to last_iter
     archive['DMFT_results']['iteration_count'] = it
     for key, value in write_to_h5.items():
         archive['DMFT_results/last_iter'][key] = value
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/dmft_tools/solver.py` & `solid_dmft-3.3.0/python/solid_dmft/dmft_tools/solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,24 +17,30 @@
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # solid_dmft (in the file COPYING.txt in this directory). If not, see
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
+# pyright: reportUnusedExpression=false
 import numpy as np
 from itertools import product
 
-from triqs.gf import MeshImTime, MeshReTime, MeshReFreq, MeshLegendre, Gf, BlockGf, make_hermitian, Omega, iOmega_n, make_gf_from_fourier, fit_hermitian_tail
+from triqs.gf import MeshImTime, MeshReTime, MeshDLRImFreq, MeshReFreq, MeshLegendre, Gf, BlockGf, make_gf_imfreq, make_hermitian, Omega, iOmega_n, make_gf_from_fourier, make_gf_dlr, fit_gf_dlr, make_gf_dlr_imtime, make_gf_imtime
 from triqs.gf.tools import inverse, make_zero_tail
 from triqs.gf.descriptors import Fourier
-from triqs.operators import c_dag, c, Operator
+from triqs.operators import c_dag, c, Operator, util
+from triqs.operators.util.U_matrix import reduce_4index_to_2index
+from triqs.operators.util.extractors import block_matrix_from_op
 import triqs.utility.mpi as mpi
+import itertools
 from h5 import HDFArchive
 
+from solid_dmft.io_tools.dict_to_h5 import prep_params_for_h5
+
 from . import legendre_filter
 from .matheval import MathExpr
 
 def get_n_orbitals(sum_k):
     """
     determines the number of orbitals within the
     solver block structure.
@@ -55,15 +61,15 @@
             if 'down' in block:
                 n_orbitals[icrsh]['down'] += sum_k.gf_struct_solver[icrsh][block]
             else:
                 n_orbitals[icrsh]['up'] += sum_k.gf_struct_solver[icrsh][block]
 
     return n_orbitals
 
-def _gf_fit_tail_fraction(Gf, fraction=0.4, replace=None, known_moments=None):
+def _gf_fit_tail_fraction(Gf, fraction=0.4, replace=None, known_moments=[]):
     """
     fits the tail of Gf object by making a polynomial
     fit of the Gf on the given fraction of the Gf mesh
     and replacing that part of the Gf by the fit
 
     0.4 fits the last 40% of the Gf and replaces the
     part with the tail
@@ -86,18 +92,18 @@
     Gf_fit = Gf.copy()
     # if no replace factor is given use the same fraction
     if not replace:
         replace = fraction
 
     for i, bl in enumerate(Gf_fit.indices):
         Gf_fit[bl].mesh.set_tail_fit_parameters(tail_fraction=fraction)
-        if known_moments:
-            tail = Gf_fit[bl].fit_hermitian_tail(known_moments[i])
-        else:
+        if known_moments == []:
             tail = Gf_fit[bl].fit_hermitian_tail()
+        else:
+            tail = Gf_fit[bl].fit_hermitian_tail(known_moments[i])
         nmax_frac = int(len(Gf_fit[bl].mesh)/2 * (1-replace))
         Gf_fit[bl].replace_by_tail(tail[0],n_min=nmax_frac)
 
     return Gf_fit
 
 class SolverStructure:
 
@@ -109,15 +115,16 @@
 
     Methods
     -------
     solve(self, **kwargs)
         solve impurity problem
     '''
 
-    def __init__(self, general_params, solver_params, advanced_params, sum_k, icrsh, h_int, iteration_offset, solver_struct_ftps):
+    def __init__(self, general_params, solver_params, gw_params, advanced_params, sum_k,
+                 icrsh, h_int, iteration_offset=None, deg_orbs_ftps=None):
         r'''
         Initialisation of the solver instance with h_int for impurity "icrsh" based on soliDMFT parameters.
 
         Parameters
         ----------
         general_paramuters: dict
                            general parameters as dict
@@ -131,71 +138,74 @@
                interaction Hamiltonian of correlated shell
         iteration_offset: int
                number of iterations this run is based on
         '''
 
         self.general_params = general_params
         self.solver_params = solver_params
+        self.gw_params = gw_params
         self.advanced_params = advanced_params
         self.sum_k = sum_k
         self.icrsh = icrsh
         self.h_int = h_int
         self.iteration_offset = iteration_offset
-        self.solver_struct_ftps = solver_struct_ftps
-        if solver_params.get("random_seed") is None:
+        self.deg_orbs_ftps = deg_orbs_ftps
+
+        # Stores random_seed as MathExpr object to evaluate it at runtime
+        if self.solver_params.get('random_seed') is None:
             self.random_seed_generator = None
         else:
-            self.random_seed_generator = MathExpr(solver_params["random_seed"])
+            self.random_seed_generator = MathExpr(self.solver_params['random_seed'])
 
         # initialize solver object, options are cthyb
-        if self.general_params['solver_type'] == 'cthyb':
+        if self.solver_params['type'] == 'cthyb':
             from triqs_cthyb.version import triqs_cthyb_hash, version
 
             # sets up necessary GF objects on ImFreq
             self._init_ImFreq_objects()
             # sets up solver
             self.triqs_solver = self._create_cthyb_solver()
             self.git_hash = triqs_cthyb_hash
             self.version = version
 
-        elif self.general_params['solver_type'] == 'ctint':
+        elif self.solver_params['type'] == 'ctint':
             from triqs_ctint.version import triqs_ctint_hash, version
 
             # sets up necessary GF objects on ImFreq
             self._init_ImFreq_objects()
             # sets up solver
             self.triqs_solver = self._create_ctint_solver()
             self.solver_params['measure_histogram'] = self.solver_params.pop('measure_pert_order')
             self.solver_params['use_double_insertion'] = self.solver_params.pop('move_double')
             self.git_hash = triqs_ctint_hash
             self.version = version
 
-        elif self.general_params['solver_type'] == 'hubbardI':
+        elif self.solver_params['type'] == 'hubbardI':
             from triqs_hubbardI.version import triqs_hubbardI_hash, version
 
             # sets up necessary GF objects on ImFreq
             self._init_ImFreq_objects()
             self._init_ReFreq_hubbardI()
             # sets up solver
             self.triqs_solver = self._create_hubbardI_solver()
             self.git_hash = triqs_hubbardI_hash
             self.version = version
 
-        elif self.general_params['solver_type'] == 'hartree':
+        elif self.solver_params['type'] == 'hartree':
             from triqs_hartree_fock.version import triqs_hartree_fock_hash, version
 
             # sets up necessary GF objects on ImFreq
             self._init_ImFreq_objects()
             self._init_ReFreq_hartree()
             # sets up solver
             self.triqs_solver = self._create_hartree_solver()
             self.git_hash = triqs_hartree_fock_hash
             self.version = version
 
-        elif self.general_params['solver_type'] == 'ftps':
+        elif self.solver_params['type'] == 'ftps':
             from forktps.version import forktps_hash, version
 
             # additional parameters
             self.bathfit_adjusted = self.iteration_offset != 0
             self.path_to_gs_accepted = bool(self.solver_params['path_to_gs'])
             self.convert_ftps = {'up': 'up', 'down': 'dn', 'ud': 'ud', 'ud_0': 'ud_0', 'ud_1': 'ud_1'}
             self.gf_struct = self.sum_k.gf_struct_solver_list[self.icrsh]
@@ -209,23 +219,23 @@
             self.bathfit_adjusted = self.iteration_offset != 0
             self.path_to_gs_accepted = bool(self.solver_params['path_to_gs'])
             # sets up solver
             self.triqs_solver, self.sector_params, self.dmrg_params, self.tevo_params, self.calc_me, self.calc_mapping = self._create_ftps_solver()
             self.git_hash = forktps_hash
             self.version = version
 
-        elif self.general_params['solver_type'] == 'inchworm':
+        elif self.solver_params['type'] == 'inchworm':
 
             # sets up necessary GF objects on ImFreq
             self._init_ImFreq_objects()
             # sets up solver
             self.triqs_solver = self._create_inchworm_solver()
             # self.git_hash = inchworm_hash
 
-        elif self.general_params['solver_type'] == 'ctseg':
+        elif self.solver_params['type'] == 'ctseg':
             from triqs_ctseg.version import triqs_ctseg_hash, version
 
             # sets up necessary GF objects on ImFreq
             self._init_ImFreq_objects()
             # sets up solver
             self.triqs_solver = self._create_ctseg_solver()
             self.git_hash = triqs_ctseg_hash
@@ -249,42 +259,48 @@
         self.G0_freq = self.G_freq.copy()
         self.G_freq_unsym = self.G_freq.copy()
         self.Delta_freq = self.G_freq.copy()
 
         # create all ImTime instances
         self.n_tau = self.general_params['n_tau']
         self.G_time = self.sum_k.block_structure.create_gf(ish=self.icrsh, gf_function=Gf, space='solver',
-                                                           mesh=MeshImTime(beta=self.general_params['beta'],
+                                                           mesh=MeshImTime(beta=self.sum_k.mesh.beta,
                                                                            S='Fermion', n_tau=self.n_tau)
                                                            )
         # copy
         self.Delta_time = self.G_time.copy()
 
         # create all Legendre instances
-        if (self.general_params['solver_type'] == 'cthyb' and self.solver_params['measure_G_l']
-            or self.general_params['solver_type'] == 'cthyb' and  self.general_params['legendre_fit']
-            or self.general_params['solver_type'] == 'ctseg' and self.solver_params['measure_gl']
-            or self.general_params['solver_type'] == 'ctseg' and  self.general_params['legendre_fit']
-            or self.general_params['solver_type'] == 'hubbardI' and self.solver_params['measure_G_l']):
+        if (self.solver_params['type'] in ['cthyb']
+                and (self.solver_params['measure_G_l'] or self.solver_params['legendre_fit'])
+                or self.solver_params['type'] == 'ctseg' and self.solver_params['legendre_fit']
+                or self.solver_params['type'] == 'hubbardI' and self.solver_params['measure_G_l']):
 
-            self.n_l = self.general_params['n_l']
+            self.n_l = self.solver_params['n_l']
             self.G_l = self.sum_k.block_structure.create_gf(ish=self.icrsh, gf_function=Gf, space='solver',
                                                             mesh=MeshLegendre(beta=self.general_params['beta'],
                                                                               max_n=self.n_l, S='Fermion')
                                                             )
             # move original G_freq to G_freq_orig
             self.G_time_orig = self.G_time.copy()
 
-        if self.general_params['solver_type'] in ['cthyb', 'hubbardI'] and self.solver_params['measure_density_matrix']:
+        if self.solver_params['type'] in ['cthyb', 'ctseg'] and self.solver_params['crm_dyson_solver']:
+            self.G_time_dlr = None
+            self.Sigma_dlr = None
+
+        if self.solver_params['type'] in ['cthyb', 'hubbardI'] and self.solver_params['measure_density_matrix']:
             self.density_matrix = None
             self.h_loc_diagonalization = None
 
-        if self.general_params['solver_type'] in ['cthyb'] and self.general_params['measure_chi'] != 'none':
+        if self.solver_params['type'] == 'cthyb' and self.solver_params['measure_chi'] is not None:
             self.O_time = None
 
+        if self.solver_params['type'] in ['cthyb'] and self.solver_params['delta_interface']:
+            self.Hloc_0 = Operator()
+
     def _init_ReFreq_objects(self):
         r'''
         Initialize all ReFreq objects
         '''
 
         # create all ReFreq instances
         self.n_w = self.general_params['n_w']
@@ -342,122 +358,113 @@
     # ********************************************************************
 
     def solve(self, **kwargs):
         r'''
         solve impurity problem with current solver
         '''
 
-        if self.random_seed_generator is None:
-            random_seed = {}
+        if self.random_seed_generator is not None:
+            self.triqs_solver_params['random_seed'] = int(self.random_seed_generator(it=kwargs["it"], rank=mpi.rank))
         else:
-            random_seed = { "random_seed": int(self.random_seed_generator(it=kwargs["it"], rank=mpi.rank)) }
-
-        if self.general_params['solver_type'] == 'cthyb':
-
-            if self.general_params['cthyb_delta_interface']:
-                mpi.report('\n Using the delta interface for cthyb passing Delta(tau) and Hloc0 directly.')
-                 # prepare solver input
-                sumk_eal = self.sum_k.eff_atomic_levels()[self.icrsh]
-                solver_eal = self.sum_k.block_structure.convert_matrix(sumk_eal, space_from='sumk', ish_from=self.sum_k.inequiv_to_corr[self.icrsh])
-                # fill Delta_time from Delta_freq sum_k to solver
-                for name, g0 in self.G0_freq:
-                    self.Delta_freq[name] << iOmega_n - inverse(g0) - solver_eal[name]
-                    known_moments = make_zero_tail(self.Delta_freq[name], 1)
-                    tail, err = fit_hermitian_tail(self.Delta_freq[name], known_moments)
-                    # without SOC delta_tau needs to be real
-                    if not self.sum_k.SO == 1:
-                        self.triqs_solver.Delta_tau[name] << make_gf_from_fourier(self.Delta_freq[name], self.triqs_solver.Delta_tau.mesh, tail).real
-                    else:
-                        self.triqs_solver.Delta_tau[name] << make_gf_from_fourier(self.Delta_freq[name], self.triqs_solver.Delta_tau.mesh, tail)
+            assert 'random_seed' not in self.triqs_solver_params
 
+        if self.solver_params['type'] == 'cthyb':
 
-                # Make non-interacting operator for Hloc0
-                Hloc_0 = Operator()
-                for spin, spin_block in solver_eal.items():
-                    for o1 in range(spin_block.shape[0]):
-                        for o2 in range(spin_block.shape[1]):
-                            # check if off-diag element is larger than threshold
-                            if o1 != o2 and abs(spin_block[o1,o2]) < self.solver_params['off_diag_threshold']:
-                                continue
-                            else:
-                                # TODO: adapt for SOC calculations, which should keep the imag part
-                                Hloc_0 += spin_block[o1,o2].real/2 * (c_dag(spin,o1) * c(spin,o2) + c_dag(spin,o2) * c(spin,o1))
-                self.solver_params['h_loc0'] = Hloc_0
+            if self.solver_params['delta_interface']:
+                self.triqs_solver.Delta_tau << self.Delta_time
+                self.triqs_solver_params['h_loc0'] = self.Hloc_0
             else:
                 # fill G0_freq from sum_k to solver
-                self.triqs_solver.G0_iw << self.G0_freq
+                self.triqs_solver.G0_iw << make_hermitian(self.G0_freq)
 
             # update solver in h5 archive one last time for debugging if solve command crashes
             if self.general_params['store_solver'] and mpi.is_master_node():
                 with HDFArchive(self.general_params['jobname']+'/'+self.general_params['seedname']+'.h5', 'a') as archive:
                     if not 'it_-1' in archive['DMFT_input/solver']:
                         archive['DMFT_input/solver'].create_group('it_-1')
                     archive['DMFT_input/solver/it_-1'][f'S_{self.icrsh}'] = self.triqs_solver
-                    archive['DMFT_input/solver/it_-1'][f'solve_params_{self.icrsh}'] = self.solver_params
+                    if self.solver_params['delta_interface']:
+                        archive['DMFT_input/solver/it_-1'][f'Delta_time_{self.icrsh}'] = self.triqs_solver.Delta_tau
+                    else:
+                        archive['DMFT_input/solver/it_-1'][f'G0_freq_{self.icrsh}'] = self.triqs_solver.G0_iw
+                    # archive['DMFT_input/solver/it_-1'][f'Delta_freq_{self.icrsh}'] = self.Delta_freq
+                    archive['DMFT_input/solver/it_-1'][f'solve_params_{self.icrsh}'] = prep_params_for_h5(self.solver_params)
+                    archive['DMFT_input/solver/it_-1'][f'triqs_solver_params_{self.icrsh}'] = prep_params_for_h5(self.triqs_solver_params)
                     archive['DMFT_input/solver/it_-1']['mpi_size'] = mpi.size
+            mpi.barrier()
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
+            self.triqs_solver.solve(h_int=self.h_int, **self.triqs_solver_params)
             # *************************************
 
             # call postprocessing
             self._cthyb_postprocessing()
 
-        elif self.general_params['solver_type'] == 'ctint':
+        elif self.solver_params['type'] == 'ctint':
             # fill G0_freq from sum_k to solver
             self.triqs_solver.G0_iw << self.G0_freq
 
-            if self.general_params['h_int_type'] == 'dynamic':
+            if self.general_params['h_int_type'][self.icrsh] == 'dynamic':
                 for b1, b2 in product(self.sum_k.gf_struct_solver_dict[self.icrsh].keys(), repeat=2):
                     self.triqs_solver.D0_iw[b1,b2] << self.U_iw[self.icrsh]
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
+            self.triqs_solver.solve(h_int=self.h_int, **self.triqs_solver_params)
             # *************************************
 
             # call postprocessing
             self._ctint_postprocessing()
 
-        elif self.general_params['solver_type'] == 'hubbardI':
+        elif self.solver_params['type'] == 'hubbardI':
             # fill G0_freq from sum_k to solver
             self.triqs_solver.G0_iw << self.G0_freq
 
             # Solve the impurity problem for icrsh shell
             # *************************************
             # this is done on every node due to very slow bcast of the AtomDiag object as of now
-            self.triqs_solver.solve(h_int=self.h_int, calc_gtau=self.solver_params['measure_G_tau'],
-                                    calc_gw=True, calc_gl=self.solver_params['measure_G_l'],
-                                    calc_dm=self.solver_params['measure_density_matrix'])
+            self.triqs_solver.solve(h_int=self.h_int, **self.triqs_solver_params)
             # if density matrix is measured, get this too. Needs to be done here,
             # because solver property 'dm' is not initialized/broadcastable
             if self.solver_params['measure_density_matrix']:
                 self.density_matrix = self.triqs_solver.dm
                 self.h_loc_diagonalization = self.triqs_solver.ad
+                # get moments
+                from triqs_cthyb.tail_fit import sigma_high_frequency_moments, green_high_frequency_moments
+                self.Sigma_moments = sigma_high_frequency_moments(self.density_matrix,
+                                                 self.h_loc_diagonalization,
+                                                 self.sum_k.gf_struct_solver_list[self.icrsh],
+                                                 self.h_int
+                                                 )
+                self.Sigma_Hartree = {bl: sigma_bl[0] for bl, sigma_bl in self.Sigma_moments.items()}
+                self.G_moments = green_high_frequency_moments(self.density_matrix,
+                                                 self.h_loc_diagonalization,
+                                                 self.sum_k.gf_struct_solver_list[self.icrsh],
+                                                 self.h_int
+                                                 )
+
             # *************************************
 
             # call postprocessing
             self._hubbardI_postprocessing()
 
-        elif self.general_params['solver_type'] == 'hartree':
+        elif self.solver_params['type'] == 'hartree':
             # fill G0_freq from sum_k to solver
             self.triqs_solver.G0_iw << self.G0_freq
 
             # Solve the impurity problem for icrsh shell
             # *************************************
             # this is done on every node due to very slow bcast of the AtomDiag object as of now
-            self.triqs_solver.solve(h_int=self.h_int, with_fock=self.solver_params['with_fock'],
-                                    one_shot=self.solver_params['one_shot'],
-                                    method=self.solver_params['method'], tol=self.solver_params['tol'])
+            self.triqs_solver.solve(h_int=self.h_int, **self.triqs_solver_params)
 
             # call postprocessing
             self._hartree_postprocessing()
 
-        elif self.general_params['solver_type'] == 'ftps':
+        elif self.solver_params['type'] == 'ftps':
             import forktps as ftps
             from forktps.DiscreteBath import DiscretizeBath, TimeStepEstimation
             from forktps.BathFitting import BathFitter
             from forktps.Helpers import MakeGFstruct
             # from . import OffDiagFitter as off_fitter
 
             def make_positive_definite(G):
@@ -481,16 +488,22 @@
                 self.Delta_freq[name] << Omega + 1j * self.general_params['eta'] - inverse(g0) - solver_eal
                 # solver Delta is symmetrized by just using 'up_0' channel
                 self.Delta_freq_solver[ftps_name] << Omega + 1j * self.general_params['eta'] - inverse(g0) - solver_eal
 
             # ensure that Delta is positive definite
             self.Delta_freq_solver = make_positive_definite(self.Delta_freq_solver)
 
+            if self.general_params['store_solver'] and mpi.is_master_node():
+                archive = HDFArchive(self.general_params['jobname']+'/'+self.general_params['seedname']+'.h5', 'a')
+                if not 'it_-1' in archive['DMFT_input/solver']:
+                    archive['DMFT_input/solver'].create_group('it_-1')
+                archive['DMFT_input/solver/it_-1']['Delta_orig'] = self.Delta_freq_solver
+
             # remove off-diagonal terms
-            if self.general_params['diag_delta']:
+            if self.solver_params['diag_delta']:
                 for name, delta in self.Delta_freq_solver:
                     for i_orb, j_orb in product(range(delta.target_shape[0]),range(delta.target_shape[1])):
                         if i_orb != j_orb:
                             delta[i_orb,j_orb] << 0.0 + 0.0j
 
             # option to increase bath sites, but run with previous eta to get increased accuracy
             if self.solver_params['n_bath'] != 0 and self.solver_params['refine_factor'] != 1:
@@ -507,15 +520,15 @@
                     Delta_discrete = fitter.FitBath(Delta=self.Delta_freq_solver, eta=self.general_params['eta'], ignoreWeight=self.solver_params['ignore_weight'],
                                                     SO=bool(self.sum_k.corr_shells[self.icrsh]['SO']))
                 else:
                     fitter = BathFitter(Nb=self.solver_params['n_bath']) if self.solver_params['n_bath'] != 0 else BathFitter(Nb=None)
                     Delta_discrete = fitter.FitBath(Delta=self.Delta_freq_solver, eta=self.general_params['eta'], ignoreWeight=self.solver_params['ignore_weight'])
             else:
                 # discretizebath
-                gap_interval = self.solver_params['enforce_gap'] if self.solver_params['enforce_gap'] != 'none' else None
+                gap_interval = self.solver_params['enforce_gap'] if self.solver_params['enforce_gap'] is not None else None
                 Delta_discrete = DiscretizeBath(Delta=self.Delta_freq_solver, Nb=self.solver_params['n_bath'], gap=gap_interval,
                                                 SO=bool(self.sum_k.corr_shells[self.icrsh]['SO']))
 
             # should be done only once after the first iteration
             if self.solver_params['n_bath'] != 0 and self.solver_params['refine_factor'] != 1:
                 if not self.bathfit_adjusted or self.bathfit_adjusted and self.iteration_offset > 0:
                     mpi.report('Rescaling "1/eta" with a factor of {}'.format(self.solver_params['refine_factor']))
@@ -542,33 +555,35 @@
             # get hloc_dft from effective atomic levels
             for name, gf in self.Delta_freq:
                 solver_eal = self.sum_k.block_structure.convert_matrix(sumk_eal, space_from='sumk', ish_from=self.sum_k.inequiv_to_corr[self.icrsh])[name]
                 if not self.sum_k.corr_shells[self.icrsh]['SO']:
                     name = self.convert_ftps[name.split('_')[0]]
                     solver_eal = solver_eal.real
                     # remove off-diagonal terms
-                    if self.general_params['diag_delta']:
+                    if self.solver_params['diag_delta']:
                         solver_eal = np.diag(np.diag(solver_eal))
                 h_loc.Fill(name, solver_eal)
 
             # fill solver h_loc
             self.triqs_solver.e0 = h_loc
 
             # FIXME: unfortunately, in the current implementation the solver initializations aren't included yet in dmft_cycle,
             # so for debugging it is done here again
             # store solver to h5 archive
             if self.general_params['store_solver'] and mpi.is_master_node():
-                archive = HDFArchive(self.general_params['jobname']+'/'+self.general_params['seedname']+'.h5', 'a')
-                archive['DMFT_input/solver'].create_group('it_-1')
-                archive['DMFT_input/solver/it_-1']['Delta'] = self.Delta_freq_solver
-                archive['DMFT_input/solver/it_-1']['S_'+str(self.icrsh)] = self.triqs_solver
+                with HDFArchive(self.general_params['jobname']+'/'+self.general_params['seedname']+'.h5', 'a') as archive:
+                    if not 'it_-1' in archive['DMFT_input/solver']:
+                        archive['DMFT_input/solver'].create_group('it_-1')
+                    archive['DMFT_input/solver'].create_group('it_-1')
+                    archive['DMFT_input/solver/it_-1']['Delta'] = self.Delta_freq_solver
+                    archive['DMFT_input/solver/it_-1']['S_'+str(self.icrsh)] = self.triqs_solver
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            path_to_gs = self.solver_params['path_to_gs'] if self.solver_params['path_to_gs'] != 'none' and self.path_to_gs_accepted else None
+            path_to_gs = self.solver_params['path_to_gs'] if self.solver_params['path_to_gs'] is not None and self.path_to_gs_accepted else None
             # fix to make sure this is only done in iteration 1
             if self.path_to_gs_accepted:
                 self.path_to_gs_accepted = False
             if path_to_gs != 'postprocess':
                 self.triqs_solver.solve(h_int=self.h_int, params_GS=self.dmrg_params, params_partSector=self.sector_params,
                                         tevo=self.tevo_params, eta=self.general_params['eta'], calc_me = self.calc_me,
                                         state_storage=self.solver_params['state_storage'],path_to_gs=path_to_gs)
@@ -577,38 +592,93 @@
                                                tevo=self.tevo_params, eta=self.general_params['eta'], calc_me = self.calc_me,
                                                state_storage=self.solver_params['state_storage'])
             # *************************************
 
             # call postprocessing
             self._ftps_postprocessing()
 
-        elif self.general_params['solver_type'] == 'inchworm':
+        elif self.solver_params['type'] == 'inchworm':
             # fill Delta_time from Delta_freq sum_k to solver
             self.triqs_solver.Delta_tau << make_gf_from_fourier(self.Delta_freq).real
 
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
+            self.triqs_solver.solve(h_int=self.h_int, **self.triqs_solver_params)
             # *************************************
 
             # call postprocessing
             self._inchworm_postprocessing()
 
-        if self.general_params['solver_type'] == 'ctseg':
+        if self.solver_params['type'] == 'ctseg':
             # fill G0_freq from sum_k to solver
-            self.triqs_solver.G0_iw << self.G0_freq
+            self.triqs_solver.Delta_tau << self.Delta_time
+            # extract hartree shift per orbital for solver
+            hloc_0_bm = block_matrix_from_op(self.Hloc_0, self.sum_k.gf_struct_solver_list[self.icrsh])
+            hartree_shift = []
+            for block in hloc_0_bm:
+                for iorb in range(block.shape[0]):
+                    # minus sign here as the solver treats the term as chemical potential and not Hloc0
+                    hartree_shift.append(-block[iorb,iorb].real)
+            mpi.report('hartree_shift:', hartree_shift)
+
+            if self.general_params['h_int_type'][self.icrsh] == 'dyn_density_density':
+                mpi.report('add dynamic interaction from bdft')
+                # convert 4 idx tensor to two index tensor
+                ish = self.sum_k.inequiv_to_corr[self.icrsh]
+                # prepare dynamic 2 idx parts
+                Uloc_dlr = self.gw_params['Uloc_dlr'][self.icrsh]['up']
+                Uloc_dlr_2idx = Gf(mesh=Uloc_dlr.mesh, target_shape=[Uloc_dlr.target_shape[0],Uloc_dlr.target_shape[1]])
+                Uloc_dlr_2idx_prime = Gf(mesh=Uloc_dlr.mesh, target_shape=[Uloc_dlr.target_shape[0],Uloc_dlr.target_shape[1]])
+
+                for coeff in Uloc_dlr.mesh:
+                    # Transposes rotation matrix here because TRIQS has a slightly different definition
+                    if self.sum_k.use_rotations:
+                        Uloc_dlr_idx = util.transform_U_matrix(Uloc_dlr[coeff], self.sum_k.rot_mat[ish].T)
+                    else:
+                        Uloc_dlr_idx = Uloc_dlr[coeff]
+                    U, Uprime = reduce_4index_to_2index(Uloc_dlr_idx)
+                    # apply rot mat here
+                    Uloc_dlr_2idx[coeff] = U
+                    Uloc_dlr_2idx_prime[coeff] = Uprime
+
+                # create full frequency objects
+                Uloc_tau_2idx = make_gf_imtime(Uloc_dlr_2idx, n_tau=self.solver_params['n_tau_k'])
+                Uloc_tau_2idx_prime = make_gf_imtime(Uloc_dlr_2idx_prime, n_tau=self.solver_params['n_tau_k'])
+
+                # fill D0_tau from Uloc_tau_2idx and Uloc_tau_2idx_prime
+                norb = Uloc_dlr.target_shape[0]
+                # same spin interaction
+                self.triqs_solver.D0_tau[0:norb, 0:norb] << Uloc_tau_2idx.real
+                self.triqs_solver.D0_tau[norb:2*norb, norb:2*norb] << Uloc_tau_2idx.real
+                # opposite spin interaction
+                self.triqs_solver.D0_tau[0:norb, norb:2*norb] << Uloc_tau_2idx_prime.real
+                self.triqs_solver.D0_tau[norb:2*norb, 0:norb] << Uloc_tau_2idx_prime.real
 
+                # TODO: add Jerp_Iw to the solver
 
-            if self.general_params['h_int_type'] == 'dynamic':
-                for b1, b2 in product(self.sum_k.gf_struct_solver_dict[self.icrsh].keys(), repeat=2):
-                    self.triqs_solver.D0_iw[b1+"|"+b2] << self.U_iw[self.icrsh]
+                # self.triqs_solver. Jperp_iw << make_gf_imfreq(Uloc_dlr_2idx, n_iw=self.general_params['n_w_b_nn']) + V
+            mpi.report('\nLocal interaction Hamiltonian is:',self.h_int)
 
+            # update solver in h5 archive one last time for debugging if solve command crashes
+            if self.general_params['store_solver'] and mpi.is_master_node():
+                with HDFArchive(self.general_params['jobname']+'/'+self.general_params['seedname']+'.h5', 'a') as archive:
+                    if 'it_-1' not in archive['DMFT_input/solver']:
+                        archive['DMFT_input/solver'].create_group('it_-1')
+                    archive['DMFT_input/solver/it_-1'][f'S_{self.icrsh}'] = self.triqs_solver
+                    archive['DMFT_input/solver/it_-1'][f'Delta_time_{self.icrsh}'] = self.triqs_solver.Delta_tau
+                    archive['DMFT_input/solver/it_-1'][f'solve_params_{self.icrsh}'] = prep_params_for_h5(self.solver_params)
+                    archive['DMFT_input/solver/it_-1'][f'triqs_solver_params_{self.icrsh}'] = prep_params_for_h5(self.triqs_solver_params)
+                    archive['DMFT_input/solver/it_-1']['mpi_size'] = mpi.size
+                    if self.general_params['h_int_type'][self.icrsh] == 'dyn_density_density':
+                        archive['DMFT_input/solver/it_-1'][f'Uloc_dlr_2idx_{self.icrsh}'] = Uloc_dlr_2idx
+                        archive['DMFT_input/solver/it_-1'][f'Uloc_dlr_2idx_prime_{self.icrsh}'] = Uloc_dlr_2idx_prime
+            mpi.barrier()
             # Solve the impurity problem for icrsh shell
             # *************************************
-            self.triqs_solver.solve(h_int=self.h_int, **{ **self.solver_params, **random_seed })
+            self.triqs_solver.solve(h_int=self.h_int, hartree_shift=hartree_shift, **self.triqs_solver_params)
             # *************************************
 
             # call postprocessing
             self._ctseg_postprocessing()
 
         return
 
@@ -618,36 +688,74 @@
 
     def _create_cthyb_solver(self):
         r'''
         Initialize cthyb solver instance
         '''
         from triqs_cthyb.solver import Solver as cthyb_solver
 
+        # Separately stores all params that go into solve() call of solver
+        self.triqs_solver_params = {}
+        keys_to_pass = ('imag_threshold', 'length_cycle', 'max_time', 'measure_density_matrix',
+                        'measure_G_l', 'measure_pert_order', 'move_double', 'move_shift',
+                        'off_diag_threshold', 'perform_tail_fit')
+        for key in keys_to_pass:
+            self.triqs_solver_params[key] = self.solver_params[key]
+
+        # Calculates number of sweeps per rank
+        self.triqs_solver_params['n_cycles'] = int(self.solver_params['n_cycles_tot'] / mpi.size)
+        # cast warmup cycles to int in case given in scientific notation
+        self.triqs_solver_params['n_warmup_cycles'] = int(self.solver_params['n_warmup_cycles'])
+
+        # Renames measure chi param
+        self.triqs_solver_params['measure_O_tau_min_ins'] = self.solver_params['measure_chi_insertions']
+
+        # use_norm_as_weight also required to measure the density matrix
+        self.triqs_solver_params['use_norm_as_weight'] = self.triqs_solver_params['measure_density_matrix']
+
+        if self.triqs_solver_params['perform_tail_fit']:
+            for key in ('fit_max_moment', 'fit_max_n', 'fit_max_w', 'fit_min_n', 'fit_min_w'):
+                self.triqs_solver_params[key] = self.solver_params[key]
+
+        # set loc_n_min and loc_n_max
+        if self.solver_params['loc_n_min'] is not None:
+            self.triqs_solver_params['loc_n_min'] = self.solver_params['loc_n_min']
+        if self.solver_params['loc_n_max'] is not None:
+            self.triqs_solver_params['loc_n_max'] = self.solver_params['loc_n_max']
+
         gf_struct = self.sum_k.gf_struct_solver_list[self.icrsh]
         # Construct the triqs_solver instances
         if self.solver_params['measure_G_l']:
             triqs_solver = cthyb_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
                             n_iw=self.general_params['n_iw'], n_tau=self.general_params['n_tau'],
-                            n_l=self.general_params['n_l'], delta_interface=self.general_params['cthyb_delta_interface'])
+                            n_l=self.solver_params['n_l'], delta_interface=self.solver_params['delta_interface'])
         else:
             triqs_solver = cthyb_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
                             n_iw=self.general_params['n_iw'], n_tau=self.general_params['n_tau'],
-                            delta_interface=self.general_params['cthyb_delta_interface'])
+                            delta_interface=self.solver_params['delta_interface'])
 
         return triqs_solver
 
     def _create_ctint_solver(self):
         r'''
         Initialize ctint solver instance
         '''
         from triqs_ctint import Solver as ctint_solver
 
+        # Separately stores all params that go into solve() call of solver
+        self.triqs_solver_params = {}
+        keys_to_pass = ('length_cycle', 'max_time', 'measure_pert_order', 'move_double', 'n_warmup_cycles')
+        for key in keys_to_pass:
+            self.triqs_solver_params[key] = self.solver_params[key]
+
+        # Calculates number of sweeps per rank
+        self.triqs_solver_params['n_cycles'] = int(self.solver_params['n_cycles_tot'] / mpi.size)
+
         gf_struct = self.sum_k.gf_struct_solver_list[self.icrsh]
 
-        if self.general_params['h_int_type'] == 'dynamic':
+        if self.general_params['h_int_type'][self.icrsh] == 'dyn_density_density':
             self.U_iw = None
             if  mpi.is_master_node():
                 with HDFArchive(self.general_params['jobname']+'/'+self.general_params['seedname']+'.h5', 'r') as archive:
                     self.U_iw = archive['dynamic_U']['U_iw']
             self.U_iw = mpi.bcast(self.U_iw)
             n_iw_dyn = self.U_iw[self.icrsh].mesh.last_index()+1
             # Construct the triqs_solver instances
@@ -663,20 +771,28 @@
 
     def _create_hubbardI_solver(self):
         r'''
         Initialize hubbardI solver instance
         '''
         from triqs_hubbardI import Solver as hubbardI_solver
 
+        # Separately stores all params that go into solve() call of solver
+        # All params need to be renamed
+        self.triqs_solver_params = {}
+        self.triqs_solver_params['calc_gtau'] = self.solver_params['measure_G_tau']
+        self.triqs_solver_params['calc_gw'] = True
+        self.triqs_solver_params['calc_gl'] = self.solver_params['measure_G_l']
+        self.triqs_solver_params['calc_dm'] = self.solver_params['measure_density_matrix']
+
         gf_struct =  self.sum_k.gf_struct_solver_list[self.icrsh]
         # Construct the triqs_solver instances
         if self.solver_params['measure_G_l']:
             triqs_solver = hubbardI_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
                                            n_iw=self.general_params['n_iw'], n_tau=self.general_params['n_tau'],
-                                           n_l=self.general_params['n_l'], n_w=self.general_params['n_w'],
+                                           n_l=self.solver_params['n_l'], n_w=self.general_params['n_w'],
                                            w_min=self.general_params['w_range'][0], w_max=self.general_params['w_range'][1],
                                            idelta=self.general_params['eta'])
         else:
             triqs_solver = hubbardI_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
                                            n_iw=self.general_params['n_iw'], n_tau=self.general_params['n_tau'],
                                            n_w=self.general_params['n_w'], idelta=self.general_params['eta'],
                                            w_min=self.general_params['w_range'][0], w_max=self.general_params['w_range'][1])
@@ -694,16 +810,21 @@
 
     def _create_hartree_solver(self):
         r'''
         Initialize hartree_fock solver instance
         '''
         from triqs_hartree_fock import ImpuritySolver as hartree_solver
 
-        gf_struct = self.sum_k.gf_struct_solver_list[self.icrsh]
+        # Separately stores all params that go into solve() call of solver
+        self.triqs_solver_params = {}
+        keys_to_pass = ('method', 'one_shot', 'tol', 'with_fock')
+        for key in keys_to_pass:
+            self.triqs_solver_params[key] = self.solver_params[key]
 
+        gf_struct = self.sum_k.gf_struct_solver_list[self.icrsh]
         # Construct the triqs_solver instances
         # Always initialize the solver with dc_U and dc_J equal to U and J and let the _interface_hartree_dc function
         # take care of changing the parameters
         triqs_solver = hartree_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
                                       n_iw=self.general_params['n_iw'], force_real=self.solver_params['force_real'],
                                       symmetries=[self._make_spin_equal],
                                       dc_U= self.general_params['U'][self.icrsh],
@@ -719,25 +840,25 @@
                 general_params : dict
                     solid_dmft general parameter dictionary
                 advanced_params : dict
                     solid_dmft advanced parameter dictionary
                 icrsh : int
                     correlated shell number
             """
-            for key in ['dc', 'dc_type']:
-                if key in general_params and general_params[key] != 'none':
-                    setattr(hartree_instance, key, general_params[key])
+            setattr(hartree_instance, 'dc', general_params['dc'])
+            if general_params['dc_type'][icrsh] is not None:
+                setattr(hartree_instance, 'dc_type', general_params['dc_type'][icrsh])
 
             for key in ['dc_factor', 'dc_fixed_value']:
-                if key in advanced_params and advanced_params[key] != 'none':
+                if key in advanced_params and advanced_params[key] is not None:
                     setattr(hartree_instance, key, advanced_params[key])
 
             #list valued keys
             for key in ['dc_U', 'dc_J', 'dc_fixed_occ']:
-                if key in advanced_params and advanced_params[key] != 'none':
+                if key in advanced_params and advanced_params[key][icrsh] is not None:
                     setattr(hartree_instance, key, advanced_params[key][icrsh])
 
             # Handle special cases
             if 'dc_dmft' in general_params:
                 if general_params['dc_dmft'] == False:
                     mpi.report('HARTREE SOLVER: Warning dft occupation in the DC calculations are meaningless for the hartree solver, reverting to dmft occupations')
 
@@ -771,48 +892,59 @@
 
     def _create_ctseg_solver(self):
         r'''
         Initialize cthyb solver instance
         '''
         from triqs_ctseg import Solver as ctseg_solver
 
-        if self.general_params['h_int_type'] == 'dynamic':
-            self.U_iw = None
-            if  mpi.is_master_node():
-                with HDFArchive(self.general_params['jobname']+'/'+self.general_params['seedname']+'.h5', 'r') as archive:
-                    self.U_iw = archive['dynamic_U']['U_iw']
-            self.U_iw = mpi.bcast(self.U_iw)
-            n_w_b_nn = self.U_iw[self.icrsh].mesh.last_index()+1
+        # Separately stores all params that go into solve() call of solver
+        self.triqs_solver_params = {}
+        keys_to_pass = ('length_cycle', 'max_time', 'measure_statehist', 'measure_nnt')
+        for key in keys_to_pass:
+            self.triqs_solver_params[key] = self.solver_params[key]
+
+        # Calculates number of sweeps per rank
+        self.triqs_solver_params['n_cycles'] = int(self.solver_params['n_cycles_tot'] / mpi.size)
+        # cast warmup cycles to int in case given in scientific notation
+        self.triqs_solver_params['n_warmup_cycles'] = int(self.solver_params['n_warmup_cycles'])
+
+        # Rename parameters that are differentin ctseg than cthyb
+        self.triqs_solver_params['measure_gt'] = self.solver_params['measure_G_tau']
+        self.triqs_solver_params['measure_perturbation_order_histograms'] = self.solver_params['measure_pert_order']
+
+        # Makes sure measure_gw is true if improved estimators are used
+        if self.solver_params['improved_estimator']:
+            self.triqs_solver_params['measure_gt'] = True
+            self.triqs_solver_params['measure_ft'] = True
         else:
-            n_w_b_nn = 1001
+            self.triqs_solver_params['measure_ft'] = False
+
 
         gf_struct = self.sum_k.gf_struct_solver_list[self.icrsh]
         # Construct the triqs_solver instances
-        if self.solver_params['measure_gl']:
-            triqs_solver = ctseg_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
-                            n_iw=self.general_params['n_iw'], n_tau=self.general_params['n_tau'],
-                            n_legendre_g=self.general_params['n_l'], n_w_b_nn = n_w_b_nn, n_tau_k=int(n_w_b_nn*2.5), n_tau_jperp=int(n_w_b_nn*2.5))
-        else:
-            triqs_solver = ctseg_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
-                            n_iw=self.general_params['n_iw'], n_tau=self.general_params['n_tau'],
-                            n_w_b_nn = n_w_b_nn, n_tau_k=int(n_w_b_nn*2.5), n_tau_jperp=int(n_w_b_nn*2.5))
-
+        triqs_solver = ctseg_solver(beta=self.general_params['beta'], gf_struct=gf_struct,
+                        n_tau=self.general_params['n_tau'],
+                        n_tau_k=int(self.solver_params['n_tau_k']))
         return triqs_solver
 
     def _create_ftps_solver(self):
         r'''
         Initialize ftps solver instance
         '''
         import forktps as ftps
 
-        # convert self.solver_struct_ftps to mapping and solver-friendly list
+        # TODO: add triqs_solver_params for ftps as well to make it analogous to other similars
+        # Not necessary but nicer. For now, just keep an empty dummy dict
+        self.triqs_solver_params = {}
+
+        # convert self.deg_orbs_ftps to mapping and solver-friendly list
         if not self.sum_k.corr_shells[self.icrsh]['SO']:
             # mapping dictionary
-            calc_mapping = {self.solver_struct_ftps[self.icrsh][deg_shell][0]:
-                    self.solver_struct_ftps[self.icrsh][deg_shell][1:] for deg_shell in range(len(self.solver_struct_ftps[self.icrsh]))}
+            calc_mapping = {self.deg_orbs_ftps[self.icrsh][deg_shell][0]:
+                    self.deg_orbs_ftps[self.icrsh][deg_shell][1:] for deg_shell in range(len(self.deg_orbs_ftps[self.icrsh]))}
             # make solver-friendly list from mapping keys
             calc_me = [[item.split('_')[0], int(item.split('_')[1])] for item in calc_mapping.keys()]
             # replace 'down' with 'dn'
             calc_me = [[item[0].replace('down','dn'),item[1]] for item in calc_me]
         else:
             # for SOC we just end up calculating everything for now
             # TODO: perhaps skip down channel
@@ -885,38 +1017,106 @@
             self.G_freq << make_hermitian(self.triqs_solver.G_iw)
             self.G_freq_unsym << self.G_freq
             self.sum_k.symm_deg_gf(self.G_freq, ish=self.icrsh)
             # set G_time
             self.G_time << self.triqs_solver.G_tau
             self.sum_k.symm_deg_gf(self.G_time, ish=self.icrsh)
 
-            if self.general_params['legendre_fit']:
+            if self.solver_params['legendre_fit']:
                 self.G_time_orig << self.triqs_solver.G_tau
                 # run the filter
-                self.G_l << legendre_filter.apply(self.G_time, self.general_params['n_l'])
+                self.G_l << legendre_filter.apply(self.G_time, self.solver_params['n_l'])
                 # get G_time, G_freq, Sigma_freq from G_l
                 set_Gs_from_G_l()
-            elif self.solver_params['perform_tail_fit'] and not self.general_params['legendre_fit']:
+            elif self.solver_params['perform_tail_fit'] and not self.solver_params['legendre_fit']:
                 # if tailfit has been used replace Sigma with the tail fitted Sigma from cthyb
                 self.Sigma_freq << self.triqs_solver.Sigma_iw
-                self.sum_k.symm_deg_gf(self.Sigma_freq, ish=self.icrsh)
+            elif self.solver_params['crm_dyson_solver']:
+                from triqs.gf.dlr_crm_dyson_solver import minimize_dyson
+
+                mpi.report('\nCRM Dyson solver to extract Σ impurity\n')
+                # fit QMC G_tau to DLR
+                if mpi.is_master_node():
+                    G_dlr = fit_gf_dlr(self.triqs_solver.G_tau,
+                                       w_max=self.general_params['dlr_wmax'], eps=self.general_params['dlr_eps'])
+                    self.G_time_dlr = make_gf_dlr_imtime(G_dlr)
+
+                    # assume little error on G0_iw and use to get G0_dlr
+                    mesh_dlr_iw = MeshDLRImFreq(G_dlr.mesh)
+                    G0_dlr_iw = self.sum_k.block_structure.create_gf(ish=self.icrsh, gf_function=Gf, mesh=mesh_dlr_iw, space='solver')
+                    for block, gf in G0_dlr_iw:
+                        for iwn in mesh_dlr_iw:
+                            gf[iwn] = self.G0_freq[block](iwn)
+                    self.sum_k.symm_deg_gf(G0_dlr_iw, ish=self.icrsh)
+
+                    # average moments
+                    self.sum_k.symm_deg_gf(self.triqs_solver.Sigma_Hartree, ish=self.icrsh)
+                    first_mom = {}
+                    for block, mom in self.triqs_solver.Sigma_moments.items():
+                        first_mom[block] = mom[1]
+                    self.sum_k.symm_deg_gf(first_mom, ish=self.icrsh)
+
+                    for block, mom in self.triqs_solver.Sigma_moments.items():
+                        mom[0] = self.triqs_solver.Sigma_Hartree[block]
+                        mom[1] = first_mom[block]
+
+                    # minimize dyson for the first entry of each deg shell
+                    self.Sigma_dlr = self.sum_k.block_structure.create_gf(ish=self.icrsh, gf_function=Gf, mesh=mesh_dlr_iw, space='solver')
+                    # without any degenerate shells we run the minimization for all blocks
+                    if self.sum_k.deg_shells[self.icrsh] == []:
+                        for block, gf in self.Sigma_dlr:
+                            np.random.seed(85281)
+                            print('Minimizing Dyson via CRM for Σ[block]:', block)
+                            gf, _, _ = minimize_dyson(G0_dlr=G0_dlr_iw[block],
+                                                      G_dlr=G_dlr[block],
+                                                      Sigma_moments=self.triqs_solver.Sigma_moments[block]
+                                                      )
+                    else:
+                        for deg_shell in self.sum_k.deg_shells[self.icrsh]:
+                            for i, block in enumerate(deg_shell):
+                                if i == 0:
+                                    np.random.seed(85281)
+                                    print('Minimizing Dyson via CRM for Σ[block]:', block)
+                                    self.Sigma_dlr[block], _, _ = minimize_dyson(G0_dlr=G0_dlr_iw[block],
+                                                                                 G_dlr=G_dlr[block],
+                                                                                 Sigma_moments=self.triqs_solver.Sigma_moments[block]
+                                                                                 )
+                                    sol_block = block
+                                else:
+                                    self.Sigma_dlr[block] << self.Sigma_dlr[sol_block]
+
+                                    print(f'Copying result from first block of deg list to {block}')
+                    print('\n')
+
+                    self.Sigma_freq = make_gf_imfreq(self.Sigma_dlr, n_iw=self.general_params['n_iw'])
+                    for block, gf in self.Sigma_freq:
+                        gf += self.triqs_solver.Sigma_moments[block][0]
+
+                mpi.barrier()
+                self.Sigma_freq = mpi.bcast(self.Sigma_freq)
+                self.Sigma_dlr = mpi.bcast(self.Sigma_dlr)
+                self.G_time = mpi.bcast(self.G_time)
+                self.G_time_dlr = mpi.bcast(self.G_time_dlr)
             else:
                 # obtain Sigma via dyson from symmetrized G_freq
                 self.Sigma_freq << inverse(self.G0_freq) - inverse(self.G_freq)
 
         # if density matrix is measured, get this too
         if self.solver_params['measure_density_matrix']:
             self.density_matrix = self.triqs_solver.density_matrix
             self.h_loc_diagonalization = self.triqs_solver.h_loc_diagonalization
+            self.Sigma_moments = self.triqs_solver.Sigma_moments
+            self.Sigma_Hartree = self.triqs_solver.Sigma_Hartree
+            self.G_moments = self.triqs_solver.G_moments
 
         if self.solver_params['measure_pert_order']:
             self.perturbation_order = self.triqs_solver.perturbation_order
             self.perturbation_order_total = self.triqs_solver.perturbation_order_total
 
-        if self.general_params['measure_chi'] != 'none':
+        if self.solver_params['measure_chi'] is not None:
             self.O_time = self.triqs_solver.O_tau
 
         return
 
     def _ctint_postprocessing(self):
         r'''
         Organize G_freq, G_time, Sigma_freq and G_l from cthyb solver
@@ -941,18 +1141,18 @@
         self.G_freq << make_hermitian(self.triqs_solver.G_iw)
         self.G_freq_unsym << self.G_freq
         self.sum_k.symm_deg_gf(self.G_freq, ish=self.icrsh)
         self.Sigma_freq << inverse(self.G0_freq) - inverse(self.G_freq)
         self.G_time << Fourier(self.G_freq)
 
         # TODO: probably not needed/sensible
-        # if self.general_params['legendre_fit']:
+        # if self.solver_params['legendre_fit']:
         #     self.G_freq_orig << self.triqs_solver.G_iw
         #     # run the filter
-        #     self.G_l << legendre_filter.apply(self.G_time, self.general_params['n_l'])
+        #     self.G_l << legendre_filter.apply(self.G_time, self.solver_params['n_l'])
         #     # get G_time, G_freq, Sigma_freq from G_l
         #     set_Gs_from_G_l()
 
         if self.solver_params['measure_histogram']:
             self.perturbation_order = self.triqs_solver.histogram
 
         return
@@ -1084,15 +1284,15 @@
     def _ctseg_postprocessing(self):
         r'''
         Organize G_freq, G_time, Sigma_freq and G_l from cthyb solver
         '''
 
         def set_Gs_from_G_l():
 
-            if self.solver_params['measure_ft'] and mpi.is_master_node():
+            if self.solver_params['improved_estimator'] and mpi.is_master_node():
                 print('\n !!!!WARNING!!!! \n you enabled both improved estimators and legendre based filtering / sampling. Sigma will be overwritten by legendre result.  \n !!!!WARNING!!!!\n')
 
             # create new G_freq and G_time
             for i, g in self.G_l:
                 g.enforce_discontinuity(np.identity(g.target_shape[0]))
                 # set G_freq from Legendre and Fouriertransform to get G_time
                 self.G_freq[i].set_from_legendre(g)
@@ -1105,71 +1305,128 @@
             # Dyson equation to get Sigma_freq
             self.Sigma_freq << inverse(self.G0_freq) - inverse(self.G_freq)
 
             return
 
         # first print average sign
         if mpi.is_master_node():
-            print('\nAverage sign: {}'.format(self.triqs_solver.average_sign))
+            print('\nAverage sign: {}'.format(self.triqs_solver.results.sign))
         # get Delta_time from solver
         self.Delta_time << self.triqs_solver.Delta_tau
 
-        self.G_time << self.triqs_solver.G_tau
+        self.G_time << self.triqs_solver.results.G_tau
         self.sum_k.symm_deg_gf(self.G_time, ish=self.icrsh)
 
-        if self.solver_params['measure_gw']:
-            self.G_freq << self.triqs_solver.G_iw
-        else:
-            if mpi.is_master_node():
-                # create empty moment container (list of np.arrays)
-                Gf_known_moments = make_zero_tail(self.G_freq,n_moments=2)
-                for i, bl in enumerate(self.G_freq.indices):
-                    # 0 moment is 0, dont touch it, but first moment is 1 for the Gf
-                    Gf_known_moments[i][1] = np.eye(self.G_freq[bl].target_shape[0])
-                    self.G_freq[bl] << Fourier(self.G_time[bl], Gf_known_moments[i])
-            self.G_freq << mpi.bcast(self.G_freq)
+        if mpi.is_master_node():
+            # create empty moment container (list of np.arrays)
+            Gf_known_moments = make_zero_tail(self.G_freq,n_moments=2)
+            for i, bl in enumerate(self.G_freq.indices):
+                # 0 moment is 0, dont touch it, but first moment is 1 for the Gf
+                Gf_known_moments[i][1] = np.eye(self.G_freq[bl].target_shape[0])
+                self.G_freq[bl] << Fourier(self.G_time[bl], Gf_known_moments[i])
+        self.G_freq << mpi.bcast(self.G_freq)
 
         self.G_freq << make_hermitian(self.G_freq)
         self.G_freq_unsym << self.G_freq
         self.sum_k.symm_deg_gf(self.G_freq, ish=self.icrsh)
 
         # if measured in Legendre basis, get G_l from solver too
-        if self.solver_params['measure_gl']:
-            # store original G_time into G_time_orig
-            self.G_time_orig << self.triqs_solver.G_tau
-            self.G_l << self.triqs_solver.G_l
-            # get G_time, G_freq, Sigma_freq from G_l
-            set_Gs_from_G_l()
-        elif self.general_params['legendre_fit']:
-            self.G_time_orig << self.triqs_solver.G_tau
-            self.G_l << legendre_filter.apply(self.G_time, self.general_params['n_l'])
+        if self.solver_params['legendre_fit']:
+            self.G_time_orig << self.triqs_solver.results.G_tau
+            self.G_l << legendre_filter.apply(self.G_time, self.solver_params['n_l'])
             # get G_time, G_freq, Sigma_freq from G_l
             set_Gs_from_G_l()
         # if improved estimators are turned on calc Sigma from F_tau, otherwise:
-        elif self.solver_params['measure_ft']:
+        elif self.solver_params['improved_estimator']:
             self.F_freq = self.G_freq.copy()
             self.F_freq << 0.0
             self.F_time = self.G_time.copy()
-            self.F_time << self.triqs_solver.F_tau
+            self.F_time << self.triqs_solver.results.F_tau
             F_known_moments = make_zero_tail(self.F_freq, n_moments=1)
             if mpi.is_master_node():
                 for i, bl in enumerate(self.F_freq.indices):
-                    self.F_freq[bl] << Fourier(self.triqs_solver.F_tau[bl], F_known_moments[i])
+                    self.F_freq[bl] << Fourier(self.triqs_solver.results.F_tau[bl], F_known_moments[i])
                 # fit tail of improved estimator and G_freq
                 self.F_freq << _gf_fit_tail_fraction(self.F_freq, fraction=0.9, replace=0.5, known_moments=F_known_moments)
                 self.G_freq << _gf_fit_tail_fraction(self.G_freq ,fraction=0.9, replace=0.5, known_moments=Gf_known_moments)
 
             self.F_freq << mpi.bcast(self.F_freq)
             self.G_freq << mpi.bcast(self.G_freq)
             for block, fw in self.F_freq:
                 for iw in fw.mesh:
                     self.Sigma_freq[block][iw] = self.F_freq[block][iw] / self.G_freq[block][iw]
 
+        elif self.solver_params['crm_dyson_solver']:
+            from triqs.gf.dlr_crm_dyson_solver import minimize_dyson
+
+            mpi.report('\nCRM Dyson solver to extract Σ impurity\n')
+            # fit QMC G_tau to DLR
+            if mpi.is_master_node():
+                G_dlr = fit_gf_dlr(self.triqs_solver.results.G_tau,
+                                   w_max=self.general_params['dlr_wmax'], eps=self.general_params['dlr_eps'])
+                self.G_time_dlr = make_gf_dlr_imtime(G_dlr)
+                self.G_freq = make_gf_imfreq(G_dlr, n_iw=self.general_params['n_iw'])
+
+                # assume little error on G0_iw and use to get G0_dlr
+                mesh_dlr_iw = MeshDLRImFreq(G_dlr.mesh)
+                G0_dlr_iw = self.sum_k.block_structure.create_gf(ish=self.icrsh, gf_function=Gf, mesh=mesh_dlr_iw, space='solver')
+                for block, gf in G0_dlr_iw:
+                    for iwn in mesh_dlr_iw:
+                        gf[iwn] = self.G0_freq[block](iwn)
+                self.sum_k.symm_deg_gf(G0_dlr_iw, ish=self.icrsh)
+                G0_dlr = make_gf_dlr(G0_dlr_iw)
+
+                # get Hartree shift for optimizer
+                G0_iw = make_gf_imfreq(G0_dlr, n_iw=self.general_params['n_iw'])
+                G_iw = make_gf_imfreq(G_dlr, n_iw=self.general_params['n_iw'])
+                Sigma_iw = inverse(G0_iw) - inverse(G_iw)
+
+                # minimize dyson for the first entry of each deg shell
+                self.Sigma_dlr = self.sum_k.block_structure.create_gf(ish=self.icrsh, gf_function=Gf, mesh=mesh_dlr_iw, space='solver')
+                # without any degenerate shells we run the minimization for all blocks
+                if self.sum_k.deg_shells[self.icrsh] == []:
+                    for block, gf in self.Sigma_dlr:
+                        tail, err = gf.fit_hermitian_tail()
+                        np.random.seed(85281)
+                        print('Minimizing Dyson via CRM for Σ[block]:', block)
+                        gf, _, _ = minimize_dyson(G0_dlr=G0_dlr_iw[block],
+                                                  G_dlr=G_dlr[block],
+                                                  Sigma_moments=tail[0:1]
+                                                    )
+                else:
+                    for deg_shell in self.sum_k.deg_shells[self.icrsh]:
+                        for i, block in enumerate(deg_shell):
+                            if i == 0:
+                                tail, err = Sigma_iw[block].fit_hermitian_tail()
+                                np.random.seed(85281)
+                                print('Minimizing Dyson via CRM for Σ[block]:', block)
+                                self.Sigma_dlr[block], _, _ = minimize_dyson(G0_dlr=G0_dlr_iw[block],
+                                                                    G_dlr=G_dlr[block],
+                                                                    Sigma_moments=tail[0:1]
+                                                                    )
+                                sol_block = block
+                            else:
+                                print(f'Copying result from first block of deg list to {block}')
+                                self.Sigma_dlr[block] << self.Sigma_dlr[sol_block]
+
+                            self.Sigma_freq[block] = make_gf_imfreq(self.Sigma_dlr[block], n_iw=self.general_params['n_iw'])
+                            self.Sigma_freq[block] += tail[0]
+                print('\n')
+
+
+            mpi.barrier()
+            self.Sigma_freq = mpi.bcast(self.Sigma_freq)
+            self.Sigma_dlr = mpi.bcast(self.Sigma_dlr)
+            self.G_time_dlr = mpi.bcast(self.G_time_dlr)
+            self.G_freq = mpi.bcast(self.G_freq)
         else:
-            mpi.report('\n!!!! WARNING !!!! tail of solver output not handled! Turn on either measure_ft, legendre_fit, or measure_gl\n')
+            mpi.report('\n!!!! WARNING !!!! tail of solver output not handled! Turn on either measure_ft, legendre_fit\n')
             self.Sigma_freq << inverse(self.G0_freq) - inverse(self.G_freq)
 
 
-        if self.solver_params['measure_hist']:
-            self.perturbation_order = self.triqs_solver.histogram
+        if self.solver_params['measure_statehist']:
+            self.state_histogram = self.triqs_solver.results.state_hist
+
+        if self.solver_params['measure_pert_order']:
+            self.perturbation_order_histo  = self.triqs_solver.results.perturbation_order_histo_Delta
 
         return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/main.py` & `solid_dmft-3.3.0/python/solid_dmft/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,96 +32,123 @@
 
 # system
 import os
 import sys
 import shutil
 from timeit import default_timer as timer
 
+try:
+    import tomllib
+except ImportError:
+    import tomli as tomllib
+
 # triqs
 import triqs.utility.mpi as mpi
 
 # own modules
-from solid_dmft.read_config import read_config
 from solid_dmft.dmft_cycle import dmft_cycle
 from solid_dmft.csc_flow import csc_flow_control
+from solid_dmft.io_tools import postproc_toml_dict, verify_input_params
 
-
-def main(argv=sys.argv):
-    """The main function for one-shot and charge-self-consistent calculations"""
+def run_dmft(params, config_file_name=None):
     # timing information
     if mpi.is_master_node():
         global_start = timer()
 
-    # reading configuration for calculation
-    general_params = None
-    solver_params = None
-    dft_params = None
-    advanced_params = None
-    if len(argv) > 1:
-        config_file_name = str(argv[1])
-    else:
-        config_file_name = 'dmft_config.ini'
-    if not os.path.isfile(config_file_name):
-        raise FileNotFoundError(f'Could not find config file {config_file_name}.')
+    # Reads in default params file and merges with params
+    full_params = None
+    default_config_name = os.path.join(os.path.dirname(__file__),
+                                       'io_tools', 'default.toml')
+    if mpi.is_master_node():
+        with open(default_config_name, 'rb') as file:
+            default_params = tomllib.load(file)
+        full_params = postproc_toml_dict.merge_config_with_default(params, default_params,
+                                                                   {'solver': 'type'})
+        verify_input_params.verify_before_dmft_cycle(full_params)
+    full_params = mpi.bcast(full_params)
 
+    # Prints parameters
     if mpi.is_master_node():
-        print('Reading the config file ' + config_file_name)
-        general_params, solver_params, dft_params, advanced_params = read_config(config_file_name)
-        general_params['config_file'] = config_file_name
-
-        print('-'*25 + '\nGeneral parameters:')
-        for key, value in general_params.items():
-            print('{0: <20} {1: <4}'.format(key, str(value)))
-        print('-'*25 + '\nSolver parameters:')
-        for key, value in solver_params.items():
-            print('{0: <20} {1: <4}'.format(key, str(value)))
-        print('-'*25 + '\nDFT parameters:')
-        for key, value in dft_params.items():
-            print('{0: <20} {1: <4}'.format(key, str(value)))
-        print('-'*25 + '\nAdvanced parameters, don\'t change them unless you know what you are doing:')
-        for key, value in advanced_params.items():
-            print('{0: <20} {1: <4}'.format(key, str(value)))
-
-    general_params = mpi.bcast(general_params)
-    solver_params = mpi.bcast(solver_params)
-    dft_params = mpi.bcast(dft_params)
-    advanced_params = mpi.bcast(advanced_params)
+        # Prints only sections that are in the input file
+        for section_name in params:
+            section = full_params[section_name]
+            print(f'\n{section_name} parameters')
+            if isinstance(section, dict):
+                for key, value in section.items():
+                    print(f'    {key: <30} {str(value)}')
+            else:
+                for i, entry in enumerate(section):
+                    print(f'entry {i+1}')
+                    for key, value in entry.items():
+                        print(f'    {key: <30} {str(value)}')
+        print('')
+    mpi.barrier()
+
+    general_params = full_params['general']
+    solver_params = full_params['solver']
+    dft_params = full_params['dft']
+    gw_params = full_params['gw']
+    advanced_params = full_params['advanced']
 
     if general_params['csc']:
         # Start CSC calculation, always in same folder as dmft_config
         general_params['jobname'] = '.'
         csc_flow_control(general_params, solver_params, dft_params, advanced_params)
+    elif general_params['gw_embedding']:
+        from solid_dmft.gw_embedding.gw_flow import embedding_driver
+        if mpi.is_master_node():
+            # Creates output directory if it does not exist
+            if not os.path.exists(general_params['jobname']):
+                os.makedirs(general_params['jobname'])
+        mpi.barrier()
+        # run GW embedding
+        embedding_driver(general_params, solver_params, gw_params, advanced_params)
     else:
         # Sets up one-shot calculation
         mpi.report('', '#'*80)
-        mpi.report(f'Using input file {general_params["seedname"]}.h5 '
-                   + f'and running in folder {general_params["jobname"]}')
+        mpi.report(f'Using input file "{general_params["seedname"]}.h5" '
+                   + f'and running in folder "{general_params["jobname"]}".')
 
         if mpi.is_master_node():
             # Checks for h5 file
             if not os.path.exists(general_params['seedname']+'.h5'):
                 raise FileNotFoundError('Input h5 file not found')
 
             # Creates output directory if it does not exist
             if not os.path.exists(general_params['jobname']):
                 os.makedirs(general_params['jobname'])
 
-            # Copies h5 archive and config file to subfolder if are not there
-            for file in (general_params['seedname']+'.h5',
-                         general_params['config_file']):
-                if not os.path.isfile(general_params['jobname']+'/'+os.path.basename(file)):
-                    shutil.copyfile(file, general_params['jobname']+'/'+os.path.basename(file))
+            # Copies h5 archive to subfolder if it is not there
+            h5_name = general_params['seedname']+'.h5'
+            if not os.path.isfile(general_params['jobname']+'/'+os.path.basename(h5_name)):
+                shutil.copyfile(h5_name, general_params['jobname']+'/'+os.path.basename(h5_name))
+
+            # Copies config file to subfolder
+            if config_file_name is not None:
+                shutil.copyfile(config_file_name, general_params['jobname']+'/'+os.path.basename(config_file_name))
         mpi.barrier()
 
         # Runs dmft_cycle
         dmft_cycle(general_params, solver_params, advanced_params,
-                   dft_params, general_params['n_iter_dmft'])
+                   dft_params, gw_params, general_params['n_iter_dmft'])
 
     mpi.barrier()
     if mpi.is_master_node():
         global_end = timer()
-        print('-------------------------------')
+        print('-'*80)
         print('overall elapsed time: %10.4f seconds'%(global_end-global_start))
 
+def main(argv=sys.argv):
+    """The main function for one-shot and charge-self-consistent calculations"""
+    config_file_name = str(argv[1]) if len(argv) > 1 else 'dmft_config.toml'
+
+    params = None
+    if mpi.is_master_node():
+        print('Reading the config file', config_file_name)
+        with open(config_file_name, 'rb') as file:
+            params = tomllib.load(file)
+    params = mpi.bcast(params)
+
+    run_dmft(params, config_file_name)
 
 if __name__ == '__main__':
     main(sys.argv)
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/postprocessing/__init__.py` & `solid_dmft-3.3.0/python/solid_dmft/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py` & `solid_dmft-3.3.0/python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,20 +187,22 @@
 
 
 def construct_Uijkl(Uijij, Uiijj):
     '''
     construct full 4 index Uijkl tensor from respack data
     assuming Uijji = Uiijj
 
-    ----------
+    Parameters:
+    -----------
     Uijij: np.ndarray
         Uijij matrix
     Uiijj: np.ndarray
         Uiijj matrix
 
+    Returns:
     -------
     uijkl : numpy array
         uijkl Coulomb tensor
 
     '''
 
     n_orb = Uijij.shape[0]
@@ -215,80 +217,86 @@
         elif i == l and j == k:  # Uijji
             Uijkl[i, j, k, l] = Uiijj[i, j]
         elif i == j and k == l:  # Uiijj
             Uijkl[i, j, k, l] = Uiijj[i, k]
     return Uijkl
 
 
-def fit_slater_fulld(u_ijij_crpa, u_ijji_crpa, U_init, J_init, fixed_F4_F2=True):
+def fit_slater(u_ijij_crpa, u_ijji_crpa, U_init, J_init, fixed_F4_F2=True):
     '''
     finds best Slater parameters U, J for given Uijij and Uijji matrices
     using the triqs U_matrix operator routine assumes F4/F2=0.625
 
     Parameters:
     -----------
-    u_ijij_crpa: np.ndarray of shape (5, 5)
+    u_ijij_crpa: np.ndarray of shape (3,3) or (5, 5)
         Uijij matrix
-    u_ijji_crpa: np.ndarray of shape (5, 5)
+    u_ijji_crpa: np.ndarray of shape (3,3) or (5, 5)
         Uijji matrix
     U_init: float
         inital value of U for optimization
     J_init: float
         inital value of J for optimization
     fixed_F4_F2: bool, optional default=True
         fix F4/F2 ratio to 0.625
+
     Returns:
     --------
     U_int: float
         averaged U value
     J_hund: float
         averaged J value
     '''
 
     from triqs.operators.util.U_matrix import U_matrix_slater, spherical_to_cubic, reduce_4index_to_2index, transform_U_matrix
     from scipy.optimize import minimize
 
     # input checks
-    assert u_ijij_crpa.shape == (5, 5), 'fit slater only implemented for full d shell (5 orbitals)'
-    assert u_ijji_crpa.shape == (5, 5), 'fit slater only implemented for full d shell (5 orbitals)'
+    if u_ijij_crpa.shape == (3,3):
+        l=1
+        # for p shell there are only 2 parameters
+        fixed_F4_F2 = True
+    elif u_ijij_crpa.shape == (5,5):
+        l=2
+    else:
+        raise ValueError('fit slater only implemented for full p or d shell')
 
     def minimizer(parameters):
         U_int, J_hund = parameters
-        Umat_full = U_matrix_slater(l=2, U_int=U_int, J_hund=J_hund, basis='spherical')
+        Umat_full = U_matrix_slater(l=l, U_int=U_int, J_hund=J_hund, basis='spherical')
         Umat_full = transform_U_matrix(Umat_full, T)
 
         Umat, u_ijij_slater = reduce_4index_to_2index(Umat_full)
         u_iijj_slater = u_ijij_slater - Umat
         return np.sum((u_ijji_crpa - u_iijj_slater)**2 + (u_ijij_crpa - u_ijij_slater)**2)
 
     def minimizer_radial(parameters):
-        F0, F2, F4 = parameters
-        Umat_full = U_matrix_slater(l=2, radial_integrals=[F0, F2, F4], basis='spherical')
+        Umat_full = U_matrix_slater(l=l, radial_integrals=parameters, basis='spherical')
         Umat_full = transform_U_matrix(Umat_full, T)
 
         Umat, u_ijij_slater = reduce_4index_to_2index(Umat_full)
         u_iijj_slater = u_ijij_slater - Umat
         return np.sum((u_ijji_crpa - u_iijj_slater)**2 + (u_ijij_crpa - u_ijij_slater)**2)
 
     # transformation matrix from spherical to w90 basis
-    T = spherical_to_cubic(l=2, convention='wannier90')
+    T = spherical_to_cubic(l=l, convention='wannier90')
 
     if fixed_F4_F2:
         result = minimize(minimizer, (U_init, J_init))
 
         U_int, J_hund = result.x
         print('Final results from fit: U = {:.3f} eV, J = {:.3f} eV'.format(U_int, J_hund))
         print('optimize error', result.fun)
     else:
         # start with 0.63 as guess
         F0 = U_init
         F2 = J_init * 14.0 / (1.0 + 0.63)
         F4 = 0.630 * F2
 
-        initial_guess = (F0, F2, F4)
+        initial_guess = [F0, F2, F4]
 
         print('Initial guess: F0 = {0[0]:.3f} eV, F2 = {0[1]:.3f} eV, F4 = {0[2]:.3f} eV'.format(initial_guess))
 
         result = minimize(minimizer_radial, initial_guess)
         F0, F2, F4 = result.x
         print('Final results from fit: F0 = {:.3f} eV, F2 = {:.3f} eV, F4 = {:.3f} eV'.format(F0, F2, F4))
         print('(F2+F4)/14 = {:.3f} eV'.format((F2+F4)/14))
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py` & `solid_dmft-3.3.0/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/postprocessing/maxent_gf_imp.py` & `solid_dmft-3.3.0/python/solid_dmft/postprocessing/maxent_gf_imp.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/postprocessing/maxent_gf_latt.py` & `solid_dmft-3.3.0/python/solid_dmft/postprocessing/maxent_gf_latt.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/postprocessing/maxent_sigma.py` & `solid_dmft-3.3.0/python/solid_dmft/postprocessing/maxent_sigma.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     * When using this on self-energies with SOC, please check that the formalism
       is correct, in particular the Kramers-Kronig relation.
 """
 
 import time
 import sys
 import numpy as np
+import warnings
 
 from triqs.utility import mpi
 from triqs_maxent.sigma_continuator import InversionSigmaContinuator, DirectSigmaContinuator
 from triqs_maxent.elementwise_maxent import PoormanMaxEnt
 from triqs_maxent.omega_meshes import HyperbolicOmegaMesh
 from triqs_maxent.alpha_meshes import LogAlphaMesh
 from triqs_maxent.logtaker import VerbosityFlags
@@ -102,14 +103,24 @@
     """
     Initializes the inversion and direct sigma continuator. Returns a list of
     continuators. Types of supported auxiliary Green's functions:
     * 'inversion_dc': inversion continuator, constant C = dc_potential for the impurity
     * 'inversion_sigmainf': inversion continuator, constant C = Sigma(i infinity) + chemical potential
     * 'direct': direct continuator
     """
+
+    for sigma_imp in sigma_iw:
+        for _, sigma_block in sigma_imp:
+            if sigma_block.data.shape[1] > 1:
+                warnings.warn('Continuation of matrix-valued selfenergies '
+                              + 'with nonzero offdiagonal components can be '
+                              + 'unstable since MaxEnt matrix continuation '
+                              + 'does not guarantee a positive semi-definite, '
+                              + 'Hermitian output.')
+
     n_inequiv_shells = len(sigma_iw)
 
     if continuator_type == 'inversion_dc':
         shifts = [None] * n_inequiv_shells
         for iineq in range(n_inequiv_shells):
             for dc_block in dc_potential[iineq].values():
                 # Reads first element from matrix for shift
@@ -186,14 +197,15 @@
         for j in range(opt_alphas[i].shape[0]):
             for k in range(j+1):
                 for l in range(2): # loop over complex numbers
                     if result.analyzer_results[k][j][l] == {}:
                         continue
                     opt_alphas[i][k, j, l] = result.analyzer_results[k][j][l][analyzer]['alpha_index']
 
+    mpi.barrier(1000)
     # Synchronizes information between ranks
     for i in imps_blocks_indices:
         spectral_funcs[i] = mpi.all_reduce(spectral_funcs[i])
         opt_alphas[i] = mpi.all_reduce(opt_alphas[i])
 
     for i, block_index in enumerate(imps_blocks):
         mpi.report(f'Optimal alphas, block {block_index}:')
@@ -242,14 +254,16 @@
 def main(external_path, iteration=None, continuator_type='inversion_sigmainf', maxent_error=.02,
          omega_min=-12., omega_max=12., n_points_maxent=400, n_points_alpha=50,
          analyzer='LineFitAnalyzer', n_points_interp=2000, n_points_final=1000):
     """
     Main function that reads the Matsubara self-energy from h5, analytically continues it,
     writes the results back to the h5 archive and also returns the results.
 
+    Function parallelizes using MPI over impurities and blocks.
+
     Parameters
     ----------
     external_path : string
         Path to the h5 archive to read from and write to
     iteration : int/string
         Iteration to read from and write to. Default to last_iter
     continuator_type : string
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/postprocessing/plot_correlated_bands.py` & `solid_dmft-3.3.0/python/solid_dmft/postprocessing/plot_correlated_bands.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             alatt_k_w = np.zeros((n_k, freq_dict['n_w']))
         else:
             alatt_k_w = np.zeros((n_k, freq_dict['n_w'], n_orb))
 
         def invert_and_trace(w, eta, mu, e_mat, sigma, trace, proj=None):
             # inversion is automatically vectorized over first axis of 3D array (omega first index now)
             Glatt = np.linalg.inv(w + eta[None, ...] + mu[None, ...] - e_mat[None, ...] - sigma.transpose(2, 0, 1))
-            A_w_nu = -1.0/np.pi * np.diagonal(Glatt, axis1=1, axis2=2).imag
+            A_w_nu = -1.0/(2.0 * np.pi)* np.diagonal(Glatt - Glatt.transpose(0,2,1).conj(), axis1=1, axis2=2).imag
             if isinstance(proj, np.ndarray):
                 A_w_nu = A_w_nu * proj[None, :]
             if trace:
                 return np.sum(A_w_nu, axis=1)
             else:
                 return A_w_nu
 
@@ -320,15 +320,15 @@
 
     if not qp_bands:
         alatt_k_w = np.zeros((n_kx, n_ky))
 
         def invert_and_trace(w, eta, mu, e_mat, sigma, proj=None):
             # inversion is automatically vectorized over first axis of 3D array (omega first index now)
             Glatt = np.linalg.inv(w + eta + mu - e_mat - sigma)
-            A_nu = -1.0/np.pi * np.diagonal(Glatt).imag
+            A_nu = -1.0/(2.0 * np.pi)* np.diagonal(Glatt - Glatt.transpose().conj()).imag
             if isinstance(proj, np.ndarray):
                 A_nu = A_nu * proj
             return np.sum(A_nu)
 
         for ikx, iky in itertools.product(range(n_kx), range(n_ky)):
             if isinstance(e_vecs, np.ndarray):
                 sigma_rot = np.einsum('ij,jk->ik',
@@ -389,15 +389,15 @@
                             idx_1 = idx_2
 
         alatt_k_w[np.where(alatt_k_w > 1)] = 1
 
     return alatt_k_w
 
 
-def _get_tb_bands(e_mat, proj_on_orb=[None], **specs):
+def get_tb_bands(e_mat, proj_on_orb=[None], **specs):
     '''
     calculate eigenvalues and eigenvectors for given list of e_mat on kmesh
 
     Parameters
     ----------
     e_mat : numpy array of shape (n_orb, n_orb, nk) or (n_orb, n_orb, nk, nk)
 
@@ -432,44 +432,52 @@
 
     return e_val, e_vec, total_proj
 
 
 def get_tb_kslice(tb, mu_tb, **specs):
 
     w90_paths = list(map(lambda section: (np.array(specs[section[0]]), np.array(specs[section[1]])), specs['bands_path']))
-    upper_left = np.diff(w90_paths[0][::-1], axis=0)[0]
-    lower_right = np.diff(w90_paths[1], axis=0)[0]
-    Z = np.array(specs['Z'])
+    upper_left = w90_paths[0][0]
+    lower_right = w90_paths[1][-1]
+    origin = w90_paths[0][1]
+    assert np.allclose(origin, w90_paths[1][0]), '"bands_path" coordinates for origin of Fermi surface needs to be consistent'
+    if 'kz' in specs and specs['kz'] != 0.:
+        assert 'Z' in specs, 'Please provide Z point coordinate in tb_data_dict as input coordinate'
+        Z = np.array(specs['Z'])
+        kz = specs['kz']
+    else:
+        kz = 0.
+        Z = np.zeros((3))
 
     # calculate FS at the mu_tb value
-    FS_kx_ky, band_char = get_kx_ky_FS(lower_right, upper_left, Z, tb, N_kxy=specs['n_k'], kz=specs['kz'], fermi=mu_tb)
+    FS_kx_ky, band_char = get_kx_ky_FS(lower_right, upper_left, origin, Z, tb, N_kxy=specs['n_k'], kz=kz, fermi=mu_tb)
 
     return FS_kx_ky, band_char
 
 
 def _fract_ind_to_val(x, ind):
     ind[ind == len(x)-1] = len(x)-1-1e-6
     int_ind = [int(indi) for indi in ind]
     int_ind_p1 = [int(indi)+1 for indi in ind]
     return x[int_ind] + (x[int_ind_p1] - x[int_ind])*(np.array(ind)-np.array(int_ind))
 
 
-def get_kx_ky_FS(lower_right, upper_left, Z, tb, select=None, N_kxy=10, kz=0.0, fermi=0.0):
+def get_kx_ky_FS(lower_right, upper_left, origin, Z, tb, select=None, N_kxy=10, kz=0.0, fermi=0.0):
 
     # create mesh
     kx = np.linspace(0, 0.5, N_kxy)
     ky = np.linspace(0, 0.5, N_kxy)
 
     if select is None:
         select = np.array(range(tb.n_orbitals))
 
     # go in horizontal arrays from bottom to top
     E_FS = np.zeros((tb.n_orbitals, N_kxy, N_kxy))
     for kyi in range(N_kxy):
-        path_FS = [(upper_left/(N_kxy-1)*kyi + kz*Z, lower_right+upper_left/(N_kxy-1)*kyi+kz*Z)]
+        path_FS = [((upper_left - origin)/(N_kxy-1)*kyi+kz*Z+origin, origin+(lower_right-origin)+(upper_left-origin)/(N_kxy-1)*kyi+kz*Z)]
         k_vec, dst, tks = k_space_path(path_FS, num=N_kxy)
         E_FS[:, :, kyi] = tb.dispersion(k_vec).transpose() - fermi
 
     contours = {}
     FS_kx_ky = {}
     FS_kx_ky_prim = {}
     band_char = {}
@@ -554,15 +562,15 @@
 
     if tb:
         # if projection is requested, _get_tb_bands() ran already
         if proj_on_orb[0] is not None:
             eps_nuk = tb_data['e_mat']
             evec_nuk = tb_data['e_vecs']
         else:
-            eps_nuk, evec_nuk, _ = _get_tb_bands(**tb_data)
+            eps_nuk, evec_nuk, _ = get_tb_bands(**tb_data)
         for band in range(n_orb):
             if not proj_on_orb[0] is not None:
                 if isinstance(plot_dict['colorscheme_bands'], str):
                     color = eval('cm.'+plot_dict['colorscheme_bands'])(1.0)
                 else:
                     color = plot_dict['colorscheme_bands']
                 ax.plot(tb_data['k_mesh'], eps_nuk[band, band].real - tb_data['mu_tb'], c=color, label=r'tight-binding', zorder=1., lw=1)
@@ -609,14 +617,15 @@
     sign = [1, -1]
     quarters = np.array([sign, sign])
     four_quarters = list(itertools.product(*quarters))
     used_quarters = [four_quarters[x] for x in quarter]
 
     vmax = plot_dict['vmax'] if 'vmax' in plot_dict else np.max(alatt_k_w)
     vmin = plot_dict['vmin'] if 'vmin' in plot_dict else 0.0
+    assert vmax > vmin, 'vmax needs to be larger than vmin'
 
     if alatt:
         if alatt_k_w is None:
             raise ValueError('A(k,w) unknown. Specify "with_sigma = True"')
         n_kx, n_ky = tb_data['e_mat'].shape[2:4]
         kx, ky = np.meshgrid(range(n_kx), range(n_ky))
         draw_colorbar = True
@@ -655,31 +664,35 @@
                             solid_capstyle='round', c=color, zorder=1., label=plot_dict['label'] if 'label' in plot_dict else '')
 
     setup_plot_kslice(ax)
 
     return ax
 
 
-def get_dmft_bands(n_orb, w90_path, w90_seed, mu_tb, add_spin=False, add_lambda=None, add_local=None,
+def get_dmft_bands(n_orb, mu_tb, w90_path=None, w90_seed=None, TB_obj=None, add_spin=False, add_lambda=None, add_local=None,
                    with_sigma=None, fermi_slice=False, qp_bands=False, orbital_order_to=None,
                    add_mu_tb=False, band_basis=False, proj_on_orb=None, trace=True, eta=0.0,
                    mu_shift=0.0, proj_nuk=None, **specs):
     '''
-    Extract tight-binding from given w90 seed_hr.dat and seed.wout files, and then extract from
+    Extract tight-binding from given w90 seed_hr.dat and seed.wout files or alternatively given TB_obj, and then extract from
     given solid_dmft calculation the self-energy and construct the spectral function A(k,w) on
     given k-path.
 
     Parameters
     ----------
     n_orb : int
         Number of Wannier orbitals in seed_hr.dat
+    mu_tb : float
+        Chemical potential of tight-binding calculation
     w90_path : string
         Path to w90 files
     w90_seed : string
         Seed of wannier90 calculation, i.e. seed_hr.dat and seed.wout
+    TB_obj : TB object
+        Tight-binding object from TB_from_wannier90
     add_spin : bool, default=False
         Extend w90 Hamiltonian by spin indices
     add_lambda : float, default=None
         Add SOC term with strength add_lambda (works only for t2g shells)
     add_local : numpy array, default=None
         Add local term of dimension (n_orb x n_orb)
     with_sigma : str, or BlockGf, default=None
@@ -751,27 +764,35 @@
     if proj_on_orb[0] is not None:
         band_basis = True
 
     # if proj_nuk is given we need to use the band_basis
     if isinstance(proj_nuk, np.ndarray) and not band_basis:
         band_basis = True
 
-    # set up Wannier Hamiltonian
-    n_orb = 2 * n_orb if add_spin else n_orb
-    change_of_basis = change_basis(n_orb, orbital_order_to, orbital_order_w90)
-    H_add_loc = np.zeros((n_orb, n_orb), dtype=complex)
-    if not isinstance(add_local, type(None)):
-        assert np.shape(add_local) == (n_orb, n_orb), 'add_local must have dimension (n_orb, n_orb), but has '\
-                f'dimension {np.shape(add_local)}'
-        H_add_loc += add_local
-    if add_spin and add_lambda:
-        H_add_loc += lambda_matrix_w90_t2g(add_lambda)
+    if TB_obj is None:
+        assert w90_path is not None and w90_seed is not None, 'Please provide either a TB object or a path to the wannier90 files'
+        # set up Wannier Hamiltonian
+        n_orb = 2 * n_orb if add_spin else n_orb
+        change_of_basis = change_basis(n_orb, orbital_order_to, orbital_order_w90)
+        H_add_loc = np.zeros((n_orb, n_orb), dtype=complex)
+        if not isinstance(add_local, type(None)):
+            assert np.shape(add_local) == (n_orb, n_orb), 'add_local must have dimension (n_orb, n_orb), but has '\
+                    f'dimension {np.shape(add_local)}'
+            H_add_loc += add_local
+        if add_spin and add_lambda:
+            H_add_loc += lambda_matrix_w90_t2g(add_lambda)
+
+        tb = TB_from_wannier90(path=w90_path, seed=w90_seed, extend_to_spin=add_spin, add_local=H_add_loc)
+    else:
+        assert not add_spin, 'add_spin is only valid when reading from wannier90 files'
+        change_of_basis = change_basis(n_orb, orbital_order_to, orbital_order_w90)
+        tb = TB_obj
+
     eta = eta * 1j
 
-    tb = TB_from_wannier90(path=w90_path, seed=w90_seed, extend_to_spin=add_spin, add_local=H_add_loc)
     # print local H(R)
     h_of_r = np.einsum('ij, jk -> ik', np.linalg.inv(change_of_basis), np.einsum('ij, jk -> ik', tb.hoppings[(0, 0, 0)], change_of_basis))
     if n_orb <= 12:
         print_matrix(h_of_r, n_orb, 'H(R=0)')
 
     # kmesh prep
     if ('bands_path' in specs and 'kmesh' in specs) or ('bands_path' not in specs and 'kmesh' not in specs):
@@ -815,32 +836,38 @@
     # calculate tight-binding eigenvalues for non slices
     if not fermi_slice:
         # Fourier trafo on input grid / path
         e_mat = tb.fourier(k_vec).transpose(1, 2, 0)
         e_mat = np.einsum('ij, jkl -> ikl', np.linalg.inv(change_of_basis),
                           np.einsum('ijk, jm -> imk', e_mat, change_of_basis))
     else:
-        assert 'Z' in specs, 'Please provide Z point coordinate in tb_data_dict as input coordinate'
-        Z = np.array(specs['Z'])
+        if 'kz' in specs and specs['kz'] != 0.:
+            assert 'Z' in specs, 'Please provide Z point coordinate in tb_data_dict as input coordinate'
+            Z = np.array(specs['Z'])
+            kz = specs['kz']
+        else:
+            kz = 0.
+            Z = np.zeros((3))
 
         k_vec = np.zeros((n_k*n_k, 3))
         e_mat = np.zeros((n_orb, n_orb, n_k, n_k), dtype=complex)
 
-        upper_left = np.diff(w90_paths[0][::-1], axis=0)[0]
-        lower_right = np.diff(w90_paths[1], axis=0)[0]
+        upper_left = w90_paths[0][0]
+        lower_right = w90_paths[1][-1]
+        origin = w90_paths[0][1]
         for ik_y in range(n_k):
-            path_along_x = [(upper_left/(n_k-1)*ik_y + specs['kz']*Z, lower_right+upper_left/(n_k-1)*ik_y+specs['kz']*Z)]
+            path_along_x = [((upper_left - origin)/(n_k-1)*ik_y+kz*Z+origin, origin+(lower_right-origin)+(upper_left-origin)/(n_k-1)*ik_y+kz*Z)]
             k_vec[ik_y*n_k:ik_y*n_k+n_k, :], k_1d, special_k = k_space_path(path_along_x, bz=tb.bz, num=n_k)
             e_mat[:, :, :, ik_y] = tb.fourier(k_vec[ik_y*n_k:ik_y*n_k+n_k, :]).transpose(1, 2, 0)
         #if add_spin:
         #    e_mat = e_mat[2:5, 2:5]
         e_mat = np.einsum('ij, jklm -> iklm', np.linalg.inv(change_of_basis), np.einsum('ijkl, jm -> imkl', e_mat, change_of_basis))
 
     if band_basis:
-        e_mat, e_vecs, orb_proj = _get_tb_bands(e_mat, proj_on_orb)
+        e_mat, e_vecs, orb_proj = get_tb_bands(e_mat, proj_on_orb)
     else:
         e_vecs = total_proj = orb_proj = None
 
     # now we merge proj_nuk and orb_proj (has reverse shape)
     if isinstance(proj_nuk, np.ndarray) and isinstance(orb_proj, np.ndarray):
         proj_nuk = proj_nuk * orb_proj
     elif not isinstance(proj_nuk, np.ndarray) and isinstance(orb_proj, np.ndarray):
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft/util/__init__.py` & `solid_dmft-3.3.0/python/solid_dmft/util/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/util/symmetrize_gamma_file.py` & `solid_dmft-3.3.0/python/solid_dmft/util/symmetrize_gamma_file.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/util/write_kslice_to_h5.py` & `solid_dmft-3.3.0/python/solid_dmft/util/write_kslice_to_h5.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.2.3/python/solid_dmft/version.py` & `solid_dmft-3.3.0/python/solid_dmft/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 # You should have received a copy of the GNU General Public License along with
 # solid_dmft (in the file COPYING.txt in this directory). If not, see
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 
-version = "3.2.3"
-triqs_hash = "8216931d15230ad4ffd4acba3db651046c040d99"
-solid_dmft_hash = "5a6299a234bc906a59921f32e93962a91d2c59cc"
+version = "3.3.0"
+triqs_hash = "d7868de5b996d2fc756f53ec924b2ce0c2a163db"
+solid_dmft_hash = "98c5d0945c327fa0b105f60a61b6e1f5fb0f0144"
 
 def show_version():
   print("\nYou are using solid_dmft version %s\n"%version)
 
 def show_git_hash():
-  print("\nYou are using solid_dmft git hash %s based on triqs git hash %s\n"%("5a6299a234bc906a59921f32e93962a91d2c59cc", triqs_hash))
+  print("\nYou are using solid_dmft git hash %s based on triqs git hash %s\n"%("98c5d0945c327fa0b105f60a61b6e1f5fb0f0144", triqs_hash))
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft.egg-info/PKG-INFO` & `solid_dmft-3.3.0/python/solid_dmft.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solid_dmft
-Version: 3.2.3
+Version: 3.3.0
 Summary: solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library
 Author-email: Alexander Hampel <ahampel@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/solid_dmft
 Project-URL: Bug Tracker, https://github.com/triqs/solid_dmft/issues
 Project-URL: Paper, https://doi.org/10.21105/joss.04623
 Keywords: DMFT,DFT,triqs
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: COPYING.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: pytest
+Requires-Dist: scikit-image
 
 ![logo_soliDMFT](https://raw.githubusercontent.com/triqs/solid_dmft/unstable/doc/logos/logo_solid_dmft.png)
 
 ![CI](https://github.com/triqs/solid_dmft/actions/workflows/build.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/solid_dmft.svg)](https://badge.fury.io/py/solid_dmft)
 [![status](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922/status.svg)](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922)
```

### Comparing `solid_dmft-3.2.3/python/solid_dmft.egg-info/SOURCES.txt` & `solid_dmft-3.3.0/python/solid_dmft.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 MANIFEST.in
 README.md
 pyproject.toml
 python/solid_dmft/__init__.py
 python/solid_dmft/csc_flow.py
 python/solid_dmft/dmft_cycle.py
 python/solid_dmft/main.py
-python/solid_dmft/read_config.py
 python/solid_dmft/version.py
 python/solid_dmft.egg-info/PKG-INFO
 python/solid_dmft.egg-info/SOURCES.txt
 python/solid_dmft.egg-info/dependency_links.txt
 python/solid_dmft.egg-info/entry_points.txt
 python/solid_dmft.egg-info/requires.txt
 python/solid_dmft.egg-info/top_level.txt
@@ -28,19 +27,27 @@
 python/solid_dmft/dmft_tools/interaction_hamiltonian.py
 python/solid_dmft/dmft_tools/legendre_filter.py
 python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
 python/solid_dmft/dmft_tools/matheval.py
 python/solid_dmft/dmft_tools/observables.py
 python/solid_dmft/dmft_tools/results_to_archive.py
 python/solid_dmft/dmft_tools/solver.py
+python/solid_dmft/gw_embedding/__init__.py
+python/solid_dmft/gw_embedding/bdft_converter.py
+python/solid_dmft/gw_embedding/gw_flow.py
+python/solid_dmft/gw_embedding/iaft.py
+python/solid_dmft/gw_embedding/qp_evs_to_eig.py
+python/solid_dmft/io_tools/__init__.py
+python/solid_dmft/io_tools/dict_to_h5.py
+python/solid_dmft/io_tools/postproc_toml_dict.py
+python/solid_dmft/io_tools/verify_input_params.py
 python/solid_dmft/postprocessing/__init__.py
 python/solid_dmft/postprocessing/eval_U_cRPA_RESPACK.py
 python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
 python/solid_dmft/postprocessing/maxent_gf_imp.py
 python/solid_dmft/postprocessing/maxent_gf_latt.py
 python/solid_dmft/postprocessing/maxent_sigma.py
+python/solid_dmft/postprocessing/pade_sigma.py
 python/solid_dmft/postprocessing/plot_correlated_bands.py
 python/solid_dmft/util/__init__.py
 python/solid_dmft/util/symmetrize_gamma_file.py
-python/solid_dmft/util/update_dmft_config.py
-python/solid_dmft/util/update_results_h5.py
 python/solid_dmft/util/write_kslice_to_h5.py
```

