# Comparing `tmp/CompactObject_TOV-1.8.1.tar.gz` & `tmp/CompactObject_TOV-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CompactObject_TOV-1.8.1.tar", last modified: Mon Jul 24 22:52:30 2023, max compression
+gzip compressed data, was "CompactObject_TOV-1.9.0.tar", last modified: Mon May 27 11:56:28 2024, max compression
```

## Comparing `CompactObject_TOV-1.8.1.tar` & `CompactObject_TOV-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,25 @@
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.923030 CompactObject_TOV-1.8.1/
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.856800 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/
--rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)      587 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/SOURCES.txt
--rw-r--r--   0 a9         (501) staff       (20)        1 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/dependency_links.txt
--rw-r--r--   0 a9         (501) staff       (20)       42 2023-07-24 22:52:30.000000 CompactObject_TOV-1.8.1/CompactObject_TOV.egg-info/top_level.txt
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.858800 CompactObject_TOV-1.8.1/EOSgenerators/
--rw-r--r--   0 a9         (501) staff       (20)     9223 2023-07-18 21:03:49.000000 CompactObject_TOV-1.8.1/EOSgenerators/RMF_EOS.py
--rw-r--r--   0 a9         (501) staff       (20)       21 2023-07-24 22:46:50.000000 CompactObject_TOV-1.8.1/EOSgenerators/__init__.py
--rw-r--r--   0 a9         (501) staff       (20)     1112 2023-07-18 21:08:17.000000 CompactObject_TOV-1.8.1/EOSgenerators/crust_EOS.py
--rw-r--r--   0 a9         (501) staff       (20)     9814 2023-07-18 22:03:03.000000 CompactObject_TOV-1.8.1/EOSgenerators/fastRMF_EoS.py
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.869106 CompactObject_TOV-1.8.1/InferenceWorkflow/
--rw-r--r--   0 a9         (501) staff       (20)     3480 2023-07-24 22:49:11.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/BayesianSampler.py
--rw-r--r--   0 a9         (501) staff       (20)    11009 2023-07-19 16:32:07.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/Likelihood.py
--rw-r--r--   0 a9         (501) staff       (20)       21 2023-07-24 22:49:13.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/__int__.py
--rw-r--r--   0 a9         (501) staff       (20)     1141 2023-07-18 21:25:02.000000 CompactObject_TOV-1.8.1/InferenceWorkflow/prior.py
--rw-r--r--   0 a9         (501) staff       (20)     1099 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/LICENSE
--rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-24 22:52:30.919409 CompactObject_TOV-1.8.1/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)     5021 2023-07-18 22:23:01.000000 CompactObject_TOV-1.8.1/README.md
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-24 22:52:30.911679 CompactObject_TOV-1.8.1/TOVsolver/
--rw-r--r--   0 a9         (501) staff       (20)     2620 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/TOVsolver/EoS_import.py
--rw-r--r--   0 a9         (501) staff       (20)       25 2023-07-24 22:46:38.000000 CompactObject_TOV-1.8.1/TOVsolver/__init__.py
--rw-r--r--   0 a9         (501) staff       (20)      158 2023-07-17 19:25:29.000000 CompactObject_TOV-1.8.1/TOVsolver/constant.py
--rw-r--r--   0 a9         (501) staff       (20)     8666 2023-07-18 18:57:17.000000 CompactObject_TOV-1.8.1/TOVsolver/main.py
--rw-r--r--   0 a9         (501) staff       (20)     8979 2023-07-18 19:01:46.000000 CompactObject_TOV-1.8.1/TOVsolver/solver_code.py
--rw-r--r--   0 a9         (501) staff       (20)      785 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/TOVsolver/speed_of_sound.py
--rw-r--r--   0 a9         (501) staff       (20)     1772 2023-07-16 23:02:27.000000 CompactObject_TOV-1.8.1/TOVsolver/tests_script.py
--rw-r--r--   0 a9         (501) staff       (20)       38 2023-07-24 22:52:30.923774 CompactObject_TOV-1.8.1/setup.cfg
--rw-r--r--   0 a9         (501) staff       (20)      170 2023-07-24 22:52:22.000000 CompactObject_TOV-1.8.1/setup.py
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2024-05-27 11:56:28.634600 CompactObject_TOV-1.9.0/
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2024-05-27 11:56:28.633068 CompactObject_TOV-1.9.0/CompactObject_TOV.egg-info/
+-rw-r--r--   0 a9         (501) staff       (20)       83 2024-05-27 11:56:28.000000 CompactObject_TOV-1.9.0/CompactObject_TOV.egg-info/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)      489 2024-05-27 11:56:28.000000 CompactObject_TOV-1.9.0/CompactObject_TOV.egg-info/SOURCES.txt
+-rw-r--r--   0 a9         (501) staff       (20)        1 2024-05-27 11:56:28.000000 CompactObject_TOV-1.9.0/CompactObject_TOV.egg-info/dependency_links.txt
+-rw-r--r--   0 a9         (501) staff       (20)       24 2024-05-27 11:56:28.000000 CompactObject_TOV-1.9.0/CompactObject_TOV.egg-info/top_level.txt
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2024-05-27 11:56:28.633501 CompactObject_TOV-1.9.0/EOSgenerators/
+-rw-r--r--   0 a9         (501) staff       (20)     1311 2024-03-21 01:11:50.000000 CompactObject_TOV-1.9.0/EOSgenerators/Polytrope.py
+-rw-r--r--   0 a9         (501) staff       (20)     9223 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/EOSgenerators/RMF_EOS.py
+-rw-r--r--   0 a9         (501) staff       (20)        0 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/EOSgenerators/__init__.py
+-rw-r--r--   0 a9         (501) staff       (20)     1112 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/EOSgenerators/crust_EOS.py
+-rw-r--r--   0 a9         (501) staff       (20)     9814 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/EOSgenerators/fastRMF_EoS.py
+-rw-r--r--   0 a9         (501) staff       (20)     1099 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/LICENSE
+-rw-r--r--   0 a9         (501) staff       (20)       83 2024-05-27 11:56:28.634495 CompactObject_TOV-1.9.0/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)     5270 2024-04-10 21:35:54.000000 CompactObject_TOV-1.9.0/README.md
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2024-05-27 11:56:28.634353 CompactObject_TOV-1.9.0/TOVsolver/
+-rw-r--r--   0 a9         (501) staff       (20)     2620 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/TOVsolver/EoS_import.py
+-rw-r--r--   0 a9         (501) staff       (20)       25 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/TOVsolver/__init__.py
+-rw-r--r--   0 a9         (501) staff       (20)      158 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/TOVsolver/constant.py
+-rw-r--r--   0 a9         (501) staff       (20)     8666 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/TOVsolver/main.py
+-rw-r--r--   0 a9         (501) staff       (20)     9617 2024-04-10 21:33:24.000000 CompactObject_TOV-1.9.0/TOVsolver/solver_code.py
+-rw-r--r--   0 a9         (501) staff       (20)      785 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/TOVsolver/speed_of_sound.py
+-rw-r--r--   0 a9         (501) staff       (20)     1772 2024-03-19 14:38:28.000000 CompactObject_TOV-1.9.0/TOVsolver/tests_script.py
+-rw-r--r--   0 a9         (501) staff       (20)       38 2024-05-27 11:56:28.634631 CompactObject_TOV-1.9.0/setup.cfg
+-rw-r--r--   0 a9         (501) staff       (20)      136 2024-05-27 11:21:37.000000 CompactObject_TOV-1.9.0/setup.py
```

### Comparing `CompactObject_TOV-1.8.1/EOSgenerators/RMF_EOS.py` & `CompactObject_TOV-1.9.0/EOSgenerators/RMF_EOS.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.8.1/EOSgenerators/crust_EOS.py` & `CompactObject_TOV-1.9.0/EOSgenerators/crust_EOS.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.8.1/EOSgenerators/fastRMF_EoS.py` & `CompactObject_TOV-1.9.0/EOSgenerators/fastRMF_EoS.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.8.1/LICENSE` & `CompactObject_TOV-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.8.1/README.md` & `CompactObject_TOV-1.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,24 @@
 ## About The Project
 
 1. Dealing with complex Relativistic Mean field (RMF) theory to generate Equation of State (EOS) of neutron star. ([EOSgenerators](https://github.com/ChunHuangPhy/EoS_inference/blob/main/EOSgenerators) Package)
 2. Solves the Tolman-Oppenheimer-Volkoff equation for a spherically symmetric compact object out of given equation of state of neutron star. ([TOVsolver](https://github.com/ChunHuangPhy/EoS_inference/blob/main/TOVsolver) Package)
 3. Implementing Neutron state EOS inference by Nested Sampling, draw constraints from Nuclear experiments, Neutron star mass (and/or) radius observations (from X-ray timing and/or radio timing) (and/or) Tidal measurement from Gravitational wave detection. That all workflow is inside this folder. ([InferenceWorkflow](https://github.com/ChunHuangPhy/EoS_inference/blob/main/InferenceWorkflow) Package) 
 
 
-Project papers list based these package: (Please consider cite them!)
+Project papers list based these package: (Please consider cite them, if you are using this package)
 
-[1]. [Huang, C., Raaijmakers, G., Watts, A. L., Tolos, L., and Providência, C., “Constraining fundamental nuclear physics parameters using neutron star mass-radius measurements I: Nucleonic models”, <i>arXiv e-prints</i>, 2023. doi:10.48550/arXiv.2303.17518.](https://arxiv.org/abs/2303.17518)
+[1]. [Huang, C., Raaijmakers, G., Watts, A. L., Tolos, L., and Providência, C., “Constraining fundamental nuclear physics parameters using neutron star mass-radius measurements I: Nucleonic models”,Monthly Notices of the Royal Astronomical Society,2024, 10.1093/mnras/stae844,529, https://academic.oup.com/mnras/article/529/4/4650/7634362
+
+
+```diff
+- check this project website: https://chunhuangphy.github.io/EoS_inference/
+```
+
+[CompactObject-TOV package website](https://chunhuangphy.github.io/EoS_inference/)
 
 ### Inlcudes
 1. Routine to check a valid equation of state input
 2. Return the mass, radius, and tidal deformability, and compute the corresponding speed of sound.
 3. [Sample TOV solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_TOVsolver.ipynb), [Sample RMF Equation of state solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_EOSgenerators.ipynb) and [Sample Analysis Notebook on Equation of state Inference and tutorial](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_Inference.ipynb) on the github to show off what we can do currently and how to use our code. (**please read them before you start to work on your own project, to familiar with the coding routine.**)
 4. Test cases and documentation
 ### v.1.3 new features:
```

#### html2text {}

```diff
@@ -6,50 +6,54 @@
 [TOVsolver](https://github.com/ChunHuangPhy/EoS_inference/blob/main/TOVsolver)
 Package) 3. Implementing Neutron state EOS inference by Nested Sampling, draw
 constraints from Nuclear experiments, Neutron star mass (and/or) radius
 observations (from X-ray timing and/or radio timing) (and/or) Tidal measurement
 from Gravitational wave detection. That all workflow is inside this folder. (
 [InferenceWorkflow](https://github.com/ChunHuangPhy/EoS_inference/blob/main/
 InferenceWorkflow) Package) Project papers list based these package: (Please
-consider cite them!) [1]. [Huang, C., Raaijmakers, G., Watts, A. L., Tolos, L.,
-and ProvidÃªncia, C., âConstraining fundamental nuclear physics parameters
-using neutron star mass-radius measurements I: Nucleonic modelsâ, arXiv e-
-prints, 2023. doi:10.48550/arXiv.2303.17518.](https://arxiv.org/abs/2303.17518)
-### Inlcudes 1. Routine to check a valid equation of state input 2. Return the
-mass, radius, and tidal deformability, and compute the corresponding speed of
-sound. 3. [Sample TOV solver Notebook](https://github.com/ChunHuangPhy/
-EoS_inference/blob/main/Test_Case/test_TOVsolver.ipynb), [Sample RMF Equation
-of state solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/
-main/Test_Case/test_EOSgenerators.ipynb) and [Sample Analysis Notebook on
-Equation of state Inference and tutorial](https://github.com/ChunHuangPhy/
-EoS_inference/blob/main/Test_Case/test_Inference.ipynb) on the github to show
-off what we can do currently and how to use our code. (**please read them
-before you start to work on your own project, to familiar with the coding
-routine.**) 4. Test cases and documentation ### v.1.3 new features: 5. Added
-computation function of generating Relativistic mean field theory(RMF) model
-EOS functionality. Defined two files fastRMF_EOS and RMF_EOS, which the
-fastRMF_EOS is speed up by numba, which need gcc compiler, could be hard to
-implement in windows, so we leave the options for users. ### v.1.5 new
-features: 6. Added Whole workflow of Bayesian inference of neutron star
-equation of state. Include defining prior by InferenceWorkflow.prior, which
-included two types: flat distribution and gaussian type. Include defining
-liklihood generated from nuclear and astrophysical constraint. ## Installation
-_Below are commands to install and update the package as well as a link to
-pypi._ ##### [PyPi](https://pypi.org/project/CompactObject-TOV/) 1. Install
-package ```sh pip install CompactObject-TOV ``` 2. Update package ```sh pip
-install CompactObject-TOV --upgrade ``` When you call the package, if you need
-to do EoS computation just ```sh import EOSgenerators ``` if you need TOV
-solver, just ```sh import TOVsolver ``` if you need to do Bayesian inference,
-just ```sh import InferenceWorkflow ``` ## Physics notations 1. CGS units is
-using here, for input quantity (equation of state): Pressure (P) and Energy
-density (rho). P is in $MeV/fm^{-3}$, same for rho. However, to omit a lot of
-the repeat of c,G. We set P as rescaled: (value in $MeV/fm^{-3}$)*G/c^4, for
-rho we have (value in $MeV/fm^{-3}$)*G/c^2 2. Out put M in Mass of sun, radius
-in km, unit-less for spped of sound and tidal deformability. ## License
-Distributed under the MIT License. See `LICENSE.txt` for more information.
+consider cite them, if you are using this package) [1]. [Huang, C.,
+Raaijmakers, G., Watts, A. L., Tolos, L., and ProvidÃªncia, C., âConstraining
+fundamental nuclear physics parameters using neutron star mass-radius
+measurements I: Nucleonic modelsâ,Monthly Notices of the Royal Astronomical
+Society,2024, 10.1093/mnras/stae844,529, https://academic.oup.com/mnras/
+article/529/4/4650/7634362 ```diff - check this project website: https://
+chunhuangphy.github.io/EoS_inference/ ``` [CompactObject-TOV package website]
+(https://chunhuangphy.github.io/EoS_inference/) ### Inlcudes 1. Routine to
+check a valid equation of state input 2. Return the mass, radius, and tidal
+deformability, and compute the corresponding speed of sound. 3. [Sample TOV
+solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/main/
+Test_Case/test_TOVsolver.ipynb), [Sample RMF Equation of state solver Notebook]
+(https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/
+test_EOSgenerators.ipynb) and [Sample Analysis Notebook on Equation of state
+Inference and tutorial](https://github.com/ChunHuangPhy/EoS_inference/blob/
+main/Test_Case/test_Inference.ipynb) on the github to show off what we can do
+currently and how to use our code. (**please read them before you start to work
+on your own project, to familiar with the coding routine.**) 4. Test cases and
+documentation ### v.1.3 new features: 5. Added computation function of
+generating Relativistic mean field theory(RMF) model EOS functionality. Defined
+two files fastRMF_EOS and RMF_EOS, which the fastRMF_EOS is speed up by numba,
+which need gcc compiler, could be hard to implement in windows, so we leave the
+options for users. ### v.1.5 new features: 6. Added Whole workflow of Bayesian
+inference of neutron star equation of state. Include defining prior by
+InferenceWorkflow.prior, which included two types: flat distribution and
+gaussian type. Include defining liklihood generated from nuclear and
+astrophysical constraint. ## Installation _Below are commands to install and
+update the package as well as a link to pypi._ ##### [PyPi](https://pypi.org/
+project/CompactObject-TOV/) 1. Install package ```sh pip install CompactObject-
+TOV ``` 2. Update package ```sh pip install CompactObject-TOV --upgrade ```
+When you call the package, if you need to do EoS computation just ```sh import
+EOSgenerators ``` if you need TOV solver, just ```sh import TOVsolver ``` if
+you need to do Bayesian inference, just ```sh import InferenceWorkflow ``` ##
+Physics notations 1. CGS units is using here, for input quantity (equation of
+state): Pressure (P) and Energy density (rho). P is in $MeV/fm^{-3}$, same for
+rho. However, to omit a lot of the repeat of c,G. We set P as rescaled: (value
+in $MeV/fm^{-3}$)*G/c^4, for rho we have (value in $MeV/fm^{-3}$)*G/c^2 2. Out
+put M in Mass of sun, radius in km, unit-less for spped of sound and tidal
+deformability. ## License Distributed under the MIT License. See `LICENSE.txt`
+for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contact * Chun Huang - chun.h@wustl.edu * Nicole Osborn - n.osborn@wustl.edu
 * Nathan Whitsett - whitsett.n@wustl.edu Project Link: [[https://github.com/
 ChunHuangPhy/EoS_inference](https://github.com/ChunHuangPhy/EoS_inference)] [!
 [DOI](https://zenodo.org/badge/doi/10.5281/zenodo.8145167.svg)](http://
 dx.doi.org/10.5281/zenodo..8145167)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `CompactObject_TOV-1.8.1/TOVsolver/EoS_import.py` & `CompactObject_TOV-1.9.0/TOVsolver/EoS_import.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.8.1/TOVsolver/main.py` & `CompactObject_TOV-1.9.0/TOVsolver/main.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.8.1/TOVsolver/solver_code.py` & `CompactObject_TOV-1.9.0/TOVsolver/solver_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import math
 from scipy.interpolate import UnivariateSpline
 from scipy.constants import pi
 from scipy.integrate import odeint, ode
 from matplotlib import pyplot
 from scipy import optimize
 from itertools import repeat
-
+from scipy.interpolate import interp1d
 def m1_from_mc_m2(mc, m2):
     """a function that feed back the companion star mass from GW event measurement.
 
     Args:
         mc (float): chrip mass of a GW event, unit in solar mass.
         m2 (float or numpy array): the determined mass for one of the star, this 
         is computed from sampling of EoS.
@@ -137,16 +137,23 @@
     #We could change this to Double Log Interpolation。
 
 
     c = 3e10
     G = 6.67428e-8
     Msun = 1.989e33
 
-    eos = UnivariateSpline(energy_density, pressure, k=3, s=0)
-    inveos = UnivariateSpline(pressure, energy_density, k=3, s=0)
+    unique_pressure_indices = np.unique(pressure, return_index=True)[1]
+    unique_pressure = pressure[np.sort(unique_pressure_indices)]
+
+# Interpolate pressure vs. energy density
+    eos = interp1d(energy_density, pressure, kind='cubic', fill_value='extrapolate')
+
+# Interpolate energy density vs. pressure
+    inveos = interp1d(unique_pressure, energy_density[unique_pressure_indices], kind='cubic', fill_value='extrapolate')
+
     Pmin = pressure[20]
     
     r = 4.441e-16
     dr = 10.
     rmax = 50 * 1e5
     rhocent = center_rho * G/c**2.
     #pcent = 10**eos(np.log10(rhocent))
@@ -199,16 +206,23 @@
     #eos = UnivariateSpline(np.log10(energy_density), np.log10(pres), k=1, s=0)
     #inveos = UnivariateSpline(np.log10(pres), np.log10(energy_density), k=1, s=0)
     #We could change this to Double Log Interpolation。
     c = 3e10
     G = 6.67428e-8
     Msun = 1.989e33
 
-    eos = UnivariateSpline(energy_density, pressure, k=3, s=0)
-    inveos = UnivariateSpline(pressure, energy_density, k=3, s=0)
+    unique_pressure_indices = np.unique(pressure, return_index=True)[1]
+    unique_pressure = pressure[np.sort(unique_pressure_indices)]
+
+# Interpolate pressure vs. energy density
+    eos = interp1d(energy_density, pressure, kind='cubic', fill_value='extrapolate')
+
+# Interpolate energy density vs. pressure
+    inveos = interp1d(unique_pressure, energy_density[unique_pressure_indices], kind='cubic', fill_value='extrapolate')
+
     Pmin = pressure[20]
     r = 4.441e-16
     dr = 10.
     center_rho = center_rho * G/c**2.
     
     #pcent = 10**eos(np.log10(rhocent))
     pcent = eos(center_rho)
```

### Comparing `CompactObject_TOV-1.8.1/TOVsolver/speed_of_sound.py` & `CompactObject_TOV-1.9.0/TOVsolver/speed_of_sound.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.8.1/TOVsolver/tests_script.py` & `CompactObject_TOV-1.9.0/TOVsolver/tests_script.py`

 * *Files identical despite different names*

