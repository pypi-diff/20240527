# Comparing `tmp/fenics_beat-0.0.5.tar.gz` & `tmp/fenics_beat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics_beat-0.0.5.tar", last modified: Mon May 13 18:44:05 2024, max compression
+gzip compressed data, was "fenics_beat-0.0.6.tar", last modified: Mon May 27 14:37:16 2024, max compression
```

## Comparing `fenics_beat-0.0.5.tar` & `fenics_beat-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.519651 fenics_beat-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 18:44:05.519651 fenics_beat-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.507651 fenics_beat-0.0.5/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/licenses/LICENSE_dolfin_pyvista_adapter
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:44:05.519651 fenics_beat-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.507651 fenics_beat-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.511651 fenics_beat-0.0.5/src/beat/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/bidomain_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.511651 fenics_beat-0.0.5/src/beat/cellmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/beeler_reuter_1977.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/fitzhughnagumo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.511651 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68630 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)    68719 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)    68702 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.515651 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   286750 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)   286758 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)   286743 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/mid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/monodomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/single_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/src/beat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.515651 fenics_beat-0.0.5/src/fenics_beat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 18:44:05.000000 fenics_beat-0.0.5/src/fenics_beat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:44:05.515651 fenics_beat-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_bidomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_cellmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_monodomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_single_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-13 18:44:02.000000 fenics_beat-0.0.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.454603 fenics_beat-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-27 14:37:16.454603 fenics_beat-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.438603 fenics_beat-0.0.6/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/licenses/LICENSE_dolfin_pyvista_adapter
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:37:16.454603 fenics_beat-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.438603 fenics_beat-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.442603 fenics_beat-0.0.6/src/beat/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/bidomain_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.442603 fenics_beat-0.0.6/src/beat/cellmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/beeler_reuter_1977.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/fitzhughnagumo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.446603 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68630 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68719 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68702 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.446603 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286750 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286758 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286743 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/mid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/conductivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/monodomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/single_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.450603 fenics_beat-0.0.6/src/fenics_beat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.450603 fenics_beat-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_bidomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_cellmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_monodomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_single_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_utils.py
```

### Comparing `fenics_beat-0.0.5/LICENSE` & `fenics_beat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/PKG-INFO` & `fenics_beat-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
@@ -28,20 +28,25 @@
 Requires-Dist: twine; extra == "pypi"
 Requires-Dist: build; extra == "pypi"
 Provides-Extra: demos
 Requires-Dist: cardiac-geometries; extra == "demos"
 Requires-Dist: ldrb; extra == "demos"
 Requires-Dist: pint; extra == "demos"
 Requires-Dist: gotranx; extra == "demos"
+Requires-Dist: ap_features; extra == "demos"
 Requires-Dist: numba; extra == "demos"
-Provides-Extra: pyvista
-Requires-Dist: pyvista[trame]; extra == "pyvista"
+Requires-Dist: jupyter; extra == "demos"
+Requires-Dist: pyvista[all]>=0.43.0; extra == "demos"
+Requires-Dist: trame-vuetify; extra == "demos"
+Requires-Dist: ipywidgets; extra == "demos"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
+Requires-Dist: jupyterlab_myst; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
 Requires-Dist: fenics-beat[pypi]; extra == "all"
 Requires-Dist: fenics-beat[dev]; extra == "all"
 Requires-Dist: fenics-beat[demos]; extra == "all"
```

### Comparing `fenics_beat-0.0.5/licenses/LICENSE_dolfin_pyvista_adapter` & `fenics_beat-0.0.6/licenses/LICENSE_dolfin_pyvista_adapter`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/pyproject.toml` & `fenics_beat-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-beat"
-version = "0.0.5"
+version = "0.0.6"
 description = "Library to run cardiac EP simulations"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["cardiac", "electrophysiology"]
 dependencies = [
@@ -21,15 +21,15 @@
 Tracker = "https://github.com/finsberg/fenics-beat/issues"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "gotranx",
-    "numba"
+    "numba",
 ]
 dev = [
     "pdbpp",
     "ipython",
     "bump2version",
     "pre-commit",
 ]
@@ -38,23 +38,26 @@
     "build"
 ]
 demos = [
    "cardiac-geometries",
    "ldrb",
    "pint",
    "gotranx",
+   "ap_features",
    "numba",
+   "jupyter",
+   "pyvista[all]>=0.43.0",
+   "trame-vuetify",
+   "ipywidgets",
 ]
-pyvista = [
-    "pyvista[trame]",
-]
-
 docs = [
    "jupyter-book",
    "jupytext",
+   "jupyterlab_myst",
+   "sphinxcontrib-bibtex",
    "fenics-beat[demos]"
 ]
 all = [
    "fenics-beat[test]",
    "fenics-beat[docs]",
    "fenics-beat[pypi]",
    "fenics-beat[dev]",
```

### Comparing `fenics_beat-0.0.5/src/beat/__init__.py` & `fenics_beat-0.0.6/src/beat/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,25 @@
     monodomain_solver,
     bidomain_model,
     base_model,
     cellmodels,
     odesolver,
     ecg,
     utils,
+    units,
+    stimulation,
+    postprocess,
+    conductivities,
+    geometry,
+    single_cell,
 )
 
 from .monodomain_model import MonodomainModel
 from .bidomain_model import BidomainModel
+from .geometry import Geometry
 from .monodomain_solver import MonodomainSplittingSolver
 
 
 __all__ = [
     "monodomain_model",
     "cellmodels",
     "bidomain_model",
@@ -22,8 +29,15 @@
     "base_model",
     "MonodomainModel",
     "BidomainModel",
     "monodomain_solver",
     "MonodomainSplittingSolver",
     "ecg",
     "utils",
+    "units",
+    "stimulation",
+    "postprocess",
+    "conductivities",
+    "geometry",
+    "Geometry",
+    "single_cell",
 ]
```

### Comparing `fenics_beat-0.0.5/src/beat/base_model.py` & `fenics_beat-0.0.6/src/beat/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,29 @@
     import ufl_legacy as ufl
     from ufl_legacy.core.expr import Expr
 except ImportError:
     import ufl
     from ufl.core.expr import Expr
 
 
+from .stimulation import Stimulus
+
 logger = logging.getLogger(__name__)
 
 
 class Status(str, Enum):
     OK = auto()
     NOT_CONVERGING = auto()
 
 
 class Results(NamedTuple):
     state: dolfin.Function
     status: Status
 
 
-class Stimulus(NamedTuple):
-    dz: dolfin.Measure
-    expr: dolfin.Expression
-
-
 class BaseModel(abc.ABC):
     def __init__(
         self,
         time: dolfin.Constant,
         mesh: dolfin.Mesh,
         params: dict[str, Any] | None = None,
         I_s: Stimulus | ufl.Coefficient | None = None,
```

### Comparing `fenics_beat-0.0.5/src/beat/bidomain_model.py` & `fenics_beat-0.0.6/src/beat/bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/__init__.py` & `fenics_beat-0.0.6/src/beat/cellmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/beeler_reuter_1977.py` & `fenics_beat-0.0.6/src/beat/cellmodels/beeler_reuter_1977.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/fitzhughnagumo.py` & `fenics_beat-0.0.6/src/beat/cellmodels/fitzhughnagumo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py` & `fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py` & `fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py` & `fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/endo.py` & `fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/endo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/epi.py` & `fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/epi.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/cellmodels/torord_dyn_chloride/mid.py` & `fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/mid.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/ecg.py` & `fenics_beat-0.0.6/src/beat/ecg.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/monodomain_model.py` & `fenics_beat-0.0.6/src/beat/monodomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/monodomain_solver.py` & `fenics_beat-0.0.6/src/beat/monodomain_solver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/odesolver.py` & `fenics_beat-0.0.6/src/beat/odesolver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/single_cell.py` & `fenics_beat-0.0.6/src/beat/single_cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         for t in times:
             if j % save_freq == 0:
                 i = 0
                 for index in track_indices:
                     track_values[k, i] = y[index]
                     i += 1
                 k += 1
+
             y[:] = fun(states=y, t=t, parameters=p, dt=dt)
             j += 1
     return y, track_values
 
 
 @jit(nopython=True)
 def solve_without_save(fun, nbeats, times, y, p, dt):
@@ -116,35 +117,39 @@
         "fun": jit(nopython=True)(fun),
         "nbeats": nbeats,
         "times": times,
         "y": init_states,
         "p": parameters,
         "dt": dt,
     }
+
     if track_indices is not None:
+        save_freq = int(np.ceil(save_every_ms / dt))
+        M = int(np.ceil(len(times) / save_freq) * nbeats)
         N = len(track_indices)
-        save_freq = round(save_every_ms / dt)
-        track_values = np.zeros((nbeats * len(times) // save_freq, N))
+        track_values = np.zeros((M, N))
+
         indices = np.array(track_indices).astype(np.int32)
         kwargs.update(
             {
                 "track_values": track_values,
                 "track_indices": indices,
                 "save_freq": save_freq,
             }
         )
         y, track_values = solve_with_save(**kwargs)
         np.save(outdir / f"tracked_values_{hash_input}.npy", track_values)
         fig, ax = plt.subplots(N, 2, sharex="col", sharey="row")
         for i in range(N):
-            ax[i, 0].plot(np.arange(0, BCL * nbeats, save_every_ms), track_values[:, i])
+            ax[i, 0].plot(np.linspace(0, BCL * nbeats, M), track_values[:, i])
             ax[i, 1].plot(
-                times[::save_freq][-round(BCL // save_every_ms) :],
-                track_values[-round(BCL // save_every_ms) :, i],
+                times[::save_freq][-int(np.ceil(BCL // save_every_ms)) :],
+                track_values[-int(np.ceil(BCL // save_every_ms)) :, i],
             )
         fig.tight_layout()
         fig.savefig(outdir / f"tracked_values_{hash_input}.png")
+        plt.close()
     else:
         y = solve_without_save(**kwargs)
 
     np.save(fname, y)
     return y
```

### Comparing `fenics_beat-0.0.5/src/beat/utils.py` & `fenics_beat-0.0.6/src/beat/utils.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/beat/viz.py` & `fenics_beat-0.0.6/src/beat/viz.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/src/fenics_beat.egg-info/PKG-INFO` & `fenics_beat-0.0.6/src/fenics_beat.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
@@ -28,20 +28,25 @@
 Requires-Dist: twine; extra == "pypi"
 Requires-Dist: build; extra == "pypi"
 Provides-Extra: demos
 Requires-Dist: cardiac-geometries; extra == "demos"
 Requires-Dist: ldrb; extra == "demos"
 Requires-Dist: pint; extra == "demos"
 Requires-Dist: gotranx; extra == "demos"
+Requires-Dist: ap_features; extra == "demos"
 Requires-Dist: numba; extra == "demos"
-Provides-Extra: pyvista
-Requires-Dist: pyvista[trame]; extra == "pyvista"
+Requires-Dist: jupyter; extra == "demos"
+Requires-Dist: pyvista[all]>=0.43.0; extra == "demos"
+Requires-Dist: trame-vuetify; extra == "demos"
+Requires-Dist: ipywidgets; extra == "demos"
 Provides-Extra: docs
 Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
+Requires-Dist: jupyterlab_myst; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
 Requires-Dist: fenics-beat[demos]; extra == "docs"
 Provides-Extra: all
 Requires-Dist: fenics-beat[test]; extra == "all"
 Requires-Dist: fenics-beat[docs]; extra == "all"
 Requires-Dist: fenics-beat[pypi]; extra == "all"
 Requires-Dist: fenics-beat[dev]; extra == "all"
 Requires-Dist: fenics-beat[demos]; extra == "all"
```

### Comparing `fenics_beat-0.0.5/src/fenics_beat.egg-info/SOURCES.txt` & `fenics_beat-0.0.6/src/fenics_beat.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 licenses/LICENSE_dolfin_pyvista_adapter
 src/beat/__init__.py
 src/beat/base_model.py
 src/beat/bidomain_model.py
+src/beat/conductivities.py
 src/beat/ecg.py
+src/beat/geometry.py
 src/beat/monodomain_model.py
 src/beat/monodomain_solver.py
 src/beat/odesolver.py
+src/beat/postprocess.py
 src/beat/single_cell.py
+src/beat/stimulation.py
+src/beat/units.py
 src/beat/utils.py
 src/beat/viz.py
 src/beat/cellmodels/__init__.py
 src/beat/cellmodels/beeler_reuter_1977.py
 src/beat/cellmodels/fitzhughnagumo.py
 src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
 src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
```

### Comparing `fenics_beat-0.0.5/tests/test_bidomain_model.py` & `fenics_beat-0.0.6/tests/test_bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/tests/test_cellmodels.py` & `fenics_beat-0.0.6/tests/test_cellmodels.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/tests/test_ecg.py` & `fenics_beat-0.0.6/tests/test_ecg.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/tests/test_monodomain.py` & `fenics_beat-0.0.6/tests/test_monodomain.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/tests/test_monodomain_solver.py` & `fenics_beat-0.0.6/tests/test_monodomain_solver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/tests/test_odesolver.py` & `fenics_beat-0.0.6/tests/test_odesolver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/tests/test_single_cell.py` & `fenics_beat-0.0.6/tests/test_single_cell.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.5/tests/test_utils.py` & `fenics_beat-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

