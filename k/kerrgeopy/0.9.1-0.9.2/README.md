# Comparing `tmp/kerrgeopy-0.9.1.tar.gz` & `tmp/kerrgeopy-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerrgeopy-0.9.1.tar", last modified: Tue Nov 14 20:38:27 2023, max compression
+gzip compressed data, was "kerrgeopy-0.9.2.tar", last modified: Mon May 27 15:23:23 2024, max compression
```

## Comparing `kerrgeopy-0.9.1.tar` & `kerrgeopy-0.9.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:38:27.488941 kerrgeopy-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2023-11-14 20:38:27.488941 kerrgeopy-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:38:27.488941 kerrgeopy-0.9.1/kerrgeopy/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20209 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24640 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28990 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/orbit.py
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/plunge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/spacetime.py
--rw-r--r--   0 runner    (1001) docker     (127)    17033 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/stable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/kerrgeopy/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:38:27.488941 kerrgeopy-0.9.1/kerrgeopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2023-11-14 20:38:27.000000 kerrgeopy-0.9.1/kerrgeopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-11-14 20:38:27.000000 kerrgeopy-0.9.1/kerrgeopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 20:38:27.000000 kerrgeopy-0.9.1/kerrgeopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 20:38:27.000000 kerrgeopy-0.9.1/kerrgeopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-14 20:38:27.000000 kerrgeopy-0.9.1/kerrgeopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 20:38:27.488941 kerrgeopy-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 20:38:27.488941 kerrgeopy-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/tests/test_four_velocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/tests/test_frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/tests/test_initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/tests/test_plunging_solutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2023-11-14 20:38:17.000000 kerrgeopy-0.9.1/tests/test_stable_solutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/kerrgeopy/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27367 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32635 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24000 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/plunge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/spacetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/stable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/kerrgeopy/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/kerrgeopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 15:23:23.000000 kerrgeopy-0.9.2/kerrgeopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:23:23.259323 kerrgeopy-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_four_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_plunging_solutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-27 15:23:19.000000 kerrgeopy-0.9.2/tests/test_stable_solutions.py
```

### Comparing `kerrgeopy-0.9.1/LICENSE` & `kerrgeopy-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.1/PKG-INFO` & `kerrgeopy-0.9.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-Metadata-Version: 2.1
-Name: kerrgeopy
-Version: 0.9.1
-Summary: Library for computing stable and plunging geodesics in Kerr spacetime
-Home-page: https://github.com/BlackHolePerturbationToolkit/KerrGeoPy
-Author: Seyong Park
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Natural Language :: English
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scipy>=1.8
-Requires-Dist: numpy
-Requires-Dist: matplotlib>=3.7
-Requires-Dist: tqdm
+[![GitHub release (with filter)](https://img.shields.io/github/v/release/BlackHolePerturbationToolkit/KerrGeoPy)](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/releases)
+[![Test Status](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/actions/workflows/tests.yml/badge.svg)](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/actions)
+[![PyPI - Version](https://img.shields.io/pypi/v/kerrgeopy)](https://pypi.org/project/kerrgeopy/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/kerrgeopy.svg)](https://anaconda.org/conda-forge/kerrgeopy)
+[![Documentation Status](https://readthedocs.org/projects/kerrgeopy/badge/?version=latest)](https://kerrgeopy.readthedocs.io/en/latest/?badge=latest)
+[![GitHub License](https://img.shields.io/github/license/BlackHolePerturbationToolkit/KerrGeoPy)](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/blob/main/LICENSE)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8417442.svg)](https://doi.org/10.5281/zenodo.8417442)
 
 # KerrGeoPy
 
 KerrGeoPy is a python implementation of the [KerrGeodesics](https://bhptoolkit.org/KerrGeodesics/) Mathematica library. It is intended for use in computing orbital trajectories for extreme-mass-ratio inspirals (EMRIs). It implements the analytical solutions for plunging orbits from [Dyson and van de Meent](https://arxiv.org/abs/2302.03704), as well as solutions for stable orbits from [Fujita and Hikida](https://arxiv.org/abs/0906.1420). The library also provides a set of methods for computing constants of motion and orbital frequencies. See the [documentation](https://kerrgeopy.readthedocs.io/en/latest/) for more information.
 
 ## Installation
 
-Install the latest version of kerrgeopy using pip
-
+Install using Anaconda
+```bash
+conda install -c conda-forge kerrgeopy
+```
+or using pip
 ```bash
 pip install kerrgeopy
 ```
+
+> **Note**
+>
+> This library uses functions introduced in scipy 1.8, so it may also be necessary to update scipy by running `pip install scipy -U`, although in most cases this should be done automatically by pip. Certain plotting and animation functions also make use of features introduced in matplotlib 3.7 and rely on [ffmpeg](https://ffmpeg.org/download.html), which can be easily installed using [homebrew](https://formulae.brew.sh/formula/ffmpeg) or [anaconda](https://anaconda.org/conda-forge/ffmpeg).
+
+## Contributing
+
+For contribution guidelines, see [CONTRIBUTING](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/blob/main/CONTRIBUTING.md).
+
 ## Stable Bound Orbits
 
-Kerrgeopy computes orbits in Boyer-Lindquist coordinates $(t,r,\theta,\phi)$. Let $M$ to represent the mass of the primary body and let $J$ represent its angular momentum. Working in geometrized units where $G=c=1$, stable bound orbits are parametrized using the following variables:
+KerrGeoPy computes orbits in Boyer-Lindquist coordinates $(t,r,\theta,\phi)$. Let $M$ to represent the mass of the primary body and let $J$ represent its angular momentum. Working in geometrized units where $G=c=1$, stable bound orbits are parametrized using the following variables:
 
 $a$ - spin of the primary body
 <br>
 $p$ - orbital semilatus rectum
 <br>
 $e$ - orbital eccentricity
 <br>
@@ -58,15 +62,15 @@
 
 ```python
 fig, ax = orbit.plot(0,10)
 ```
 
 
     
-![png](README_files/Getting%20Started_3_0.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_3_0.png)
     
 
 
 Next, compute the time, radial, polar and azimuthal components of the trajectory as a function of Mino time using the `trajectory()` method. By default, the time and radial components of the trajectory are given in geometrized units and are normalized using $M$ so that they are dimensionless.
 
 
 ```python
@@ -103,15 +107,15 @@
 plt.ylabel(r"$\phi(\lambda)$")
 ```
 
 
 
 
     
-![png](README_files/Getting%20Started_6_1.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_6_1.png)
     
 
 
 ## Orbital Properties
 
 Use the `constants_of_motion()` method to compute the dimensionless energy, angular momentum and Carter constant. By default, constants of motion are given in geometrized units where $G=c=1$ and are scale-invariant, meaning that they are normalized according to the masses of the two bodies as follows:
 
@@ -230,15 +234,15 @@
 plt.plot(time, phi(time))
 plt.xlabel("$\lambda$")
 plt.ylabel(r"$\phi(\lambda)$")
 ```
 
 
     
-![png](README_files/Getting%20Started_15_1.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_15_1.png)
     
 
 
 
 ## Alternative Parametrizations
 
 Use the `from_constants()` class method to construct a `StableOrbit` from the spin parameter and constants of motion $(a,E,L,Q)$
@@ -285,14 +289,14 @@
 
 plt.subplot(1,4,4)
 plt.plot(time, phi(time))
 plt.xlabel("$\lambda$")
 plt.ylabel(r"$\phi(\lambda)$")
 ```
     
-![png](README_files/Getting%20Started_20_1.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_20_1.png)
     
 
 ## Authors
 
 * Seyong Park
-* Zach Nasipak
+* Zach Nasipak
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy/constants.py` & `kerrgeopy-0.9.2/kerrgeopy/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,98 @@
-"""
-Module containing functions for computing the constants of motion for an orbit in Kerr Spacetime.
+"""Module containing functions for computing the constants of motion for an orbit in Kerr Spacetime.
 Constants of motion are computed using the method described in Appendix B of `Schmidt <https://doi.org/10.48550/arXiv.gr-qc/0202090>`_.
 """
 from numpy import sign, sqrt, copysign, pi, nan, inf
 from scipy.optimize import root_scalar
 from .units import *
 from scipy.interpolate import RectBivariateSpline
 import numpy as np
 from numpy.polynomial import Polynomial
 
-def stable_radial_roots(a,p,e,x,constants=None):
-    """
-    Computes the radial roots for a stable bound orbit as defined in equation 10 of `Fujita and Hikida <https://doi.org/10.48550/arXiv.0906.1420>`_.
-    Roots are given in decreasing order.
 
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity
-    :type e: double
-    :param x: cosine of the orbital inclination
-    :type x: tuple(double, double, double, double)
-    :param constants: dimensionless constants of motion for the orbit
-    :type constants: tuple(double, double, double)
+def stable_radial_roots(a, p, e, x, constants=None):
+    """Computes the radial roots for a stable bound orbit as defined in 
+    equation 10 of `Fujita and Hikida <https://doi.org/10.48550/arXiv.0906.1420>`_. 
+    Roots are given in decreasing order.
 
-    :return: tuple containing the four roots of the radial equation
-    :rtype: tuple(double, double, double, double)
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity
+    x : tuple(double, double, double, double)
+        cosine of the orbital inclination
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit
+
+    Returns
+    -------
+    tuple(double, double, double, double)
+        tuple containing the four roots of the radial equation
     """
-    if constants is None: constants = constants_of_motion(a,p,e,x)
+    if constants is None:
+        constants = constants_of_motion(a, p, e, x)
     E, L, Q = constants
-    
-    r1 = p/(1-e)
-    r2 = p/(1+e)
-    
-    A_plus_B = 2/(1-E**2)-r1-r2
-    AB = a**2*Q/(r1*r2*(1-E**2))
-    
-    r3 = (A_plus_B+sqrt(A_plus_B**2-4*AB))/2
-    r4 = AB/r3
-    
-    return r1, r2, r3, r4
 
+    r1 = p / (1 - e)
+    r2 = p / (1 + e)
 
-def plunging_radial_roots(a,E,L,Q):
-    """
-    Computes the radial roots for a plunging orbit. 
-    If all roots are real, roots are sorted such that the motion is between r1 and r2 and roots are otherwise in decreasing order.
-    If there are two complex roots, r1 < r2 are real and r3/r4 are complex conjugates.
-
-    :param a: dimensionless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
+    A_plus_B = 2 / (1 - E**2) - r1 - r2
+    AB = a**2 * Q / (r1 * r2 * (1 - E**2))
+
+    r3 = (A_plus_B + sqrt(A_plus_B**2 - 4 * AB)) / 2
+    r4 = AB / r3
+
+    return r1, r2, r3, r4
 
-    :return: tuple of radial roots
-    :rtype: tuple(double,double,double,double)
+
+def plunging_radial_roots(a, E, L, Q):
+    """Computes the radial roots for a plunging orbit. If all roots are real, 
+    roots are sorted such that the motion is between r1 and r2 and roots are 
+    otherwise in decreasing order. If there are two complex roots, 
+    r1 < r2 are real and r3/r4 are complex conjugates.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin parameter
+    E : double
+        dimensionless energy
+    L : double
+        dimensionless angular momentum
+    Q : double
+        dimensionless Carter constant
+
+    Returns
+    -------
+    tuple(double,double,double,double)
+        tuple of radial roots
     """
     # standard form of the radial polynomial R(r)
-    R = Polynomial([-a**2*Q, 2*L**2+2*Q+2*a**2*E**2-4*a*E*L, a**2*E**2-L**2-Q-a**2, 2, E**2-1])
+    R = Polynomial(
+        [
+            -(a**2) * Q,
+            2 * L**2 + 2 * Q + 2 * a**2 * E**2 - 4 * a * E * L,
+            a**2 * E**2 - L**2 - Q - a**2,
+            2,
+            E**2 - 1,
+        ]
+    )
     roots = R.roots()
     # get the real roots and the complex roots
     real_roots = np.sort(np.real(roots[np.isreal(roots)]))
     complex_roots = roots[np.iscomplex(roots)]
 
-    r_minus = 1-sqrt(1-a**2)
+    r_minus = 1 - sqrt(1 - a**2)
 
-    # if there are 4 real roots, by convention r4 < r3 < r2 < r1 (consistent with stable orbits)
+    # if there are 4 real roots, by convention r4 < r3 < r2 < r1 
+    # (consistent with stable orbits)
     if len(real_roots) == 4:
         # if there are three roots outside the event horizon swap r1/r3 and r2/r4
         if real_roots[1] > r_minus:
             r1 = real_roots[1]
             r2 = real_roots[0]
             r3 = real_roots[3]
             r4 = real_roots[2]
@@ -84,342 +102,466 @@
     # in the case of two complex roots, r1 < r2 are real and r3/r4 are complex conjugates
     elif len(real_roots) == 2:
         r1, r2 = real_roots
         r3, r4 = complex_roots
 
     return r1, r2, r3, r4
 
-def stable_polar_roots(a,p,e,x,constants=None):
-    r"""
-    Computes the polar roots for a stable bound orbit as defined in equation 10 of `Fujita and Hikida <https://doi.org/10.48550/arXiv.0906.1420>`_.
-    Roots are given in increasing order.
 
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity
-    :type e: double
-    :param x: cosine of the orbital inclination
-    :type x: tuple(double, double, double)
-    :param constants: dimensionless constants of motion for the orbit
-    :type constants: tuple(double, double, double)
+def stable_polar_roots(a, p, e, x, constants=None):
+    r"""Computes the polar roots for a stable bound orbit as defined in equation 
+    10 of `Fujita and Hikida <https://doi.org/10.48550/arXiv.0906.1420>`_. 
+    Roots are given in increasing order.
 
-    :return: tuple of roots :math:`(z_-, z_+)`
-    :rtype: tuple(double, double, double, double)
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity
+    x : tuple(double, double, double)
+        cosine of the orbital inclination
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit
+
+    Returns
+    -------
+    tuple(double, double, double, double)
+        tuple of roots :math:`(z_-, z_+)`
     """
-    if constants is None: constants = constants_of_motion(a,p,e,x)
+    if constants is None:
+        constants = constants_of_motion(a, p, e, x)
     E, L, Q = constants
-    epsilon0 = a**2*(1-E**2)/L**2
-    z_minus = 1-x**2
-    #z_plus = a**2*(1-E**2)/(L**2*epsilon0)+1/(epsilon0*(1-z_minus))
+    epsilon0 = a**2 * (1 - E**2) / L**2
+    z_minus = 1 - x**2
+    # z_plus = a**2*(1-E**2)/(L**2*epsilon0)+1/(epsilon0*(1-z_minus))
     # simplified using definition of carter constant
-    z_plus = nan if a == 0 else 1+1/(epsilon0*(1-z_minus)) 
-    
+    z_plus = nan if a == 0 else 1 + 1 / (epsilon0 * (1 - z_minus))
+
     return z_minus, z_plus
 
-def _coefficients(r,a,x):
-    """
-    Computes the coefficients f, g, h and d from equation B.5 in `Schmidt <https://doi.org/10.48550/arXiv.gr-qc/0202090>`_
-    
-    :param r: dimensionless distance from the black hole
-    :type r: double
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param x: cosine of the orbital inclination
-    :type x: double
-    
-    :rtype: tuple(double, double, double, double)
-    """
-    z = sqrt(1-x**2)
-    delta = r**2-2*r+a**2
-    f = lambda r: r**4+a**2*(r*(r+2)+z**2*delta)
-    g = lambda r: 2*a*r
-    h = lambda r: r*(r-2)+z**2/(1-z**2)*delta
-    d = lambda r: (r**2+a**2*z**2)*delta
-    
+
+def _coefficients(r, a, x):
+    """Computes the coefficients f, g, h and d from equation B.5 in 
+    `Schmidt <https://doi.org/10.48550/arXiv.gr-qc/0202090>`_
+
+    Parameters
+    ----------
+    r : double
+        dimensionless distance from the black hole
+    a : double
+        dimensionless spin of the black hole
+    x : double
+        cosine of the orbital inclination
+
+    Returns
+    -------
+    tuple(double, double, double, double)
+    """
+    z = sqrt(1 - x**2)
+    delta = r**2 - 2 * r + a**2
+    f = lambda r: r**4 + a**2 * (r * (r + 2) + z**2 * delta)
+    g = lambda r: 2 * a * r
+    h = lambda r: r * (r - 2) + z**2 / (1 - z**2) * delta
+    d = lambda r: (r**2 + a**2 * z**2) * delta
+
     return f(r), g(r), h(r), d(r)
 
-def _coefficients_derivative(r,a,x):
-    """
-    Computes the derivatives f', g', h' and d' of the coefficients from equation B.5 in `Schmidt <https://doi.org/10.48550/arXiv.gr-qc/0202090>`_
-    
-    :param r: dimensionless distance from the black hole
-    :type r: double
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param x: cosine of the orbital inclination
-    :type x: double
-    
-    :rtype: tuple(double, double, double, double)
-    """
-    z = sqrt(1-x**2)
-    f_prime = lambda r: 4*r**3+2*a**2*((1+z**2)*r+(1-z**2))
-    g_prime = lambda r: 2*a
-    h_prime = lambda r: 2*(r-1)/(1-z**2)
-    d_prime = lambda r: 2*(2*r-3)*r**2+2*a**2*((1+z**2)*r-z**2)
-    
+
+def _coefficients_derivative(r, a, x):
+    """Computes the derivatives f', g', h' and d' of the coefficients from 
+    equation B.5 in `Schmidt <https://doi.org/10.48550/arXiv.gr-qc/0202090>`_
+
+    Parameters
+    ----------
+    r : double
+        dimensionless distance from the black hole
+    a : double
+        dimensionless spin of the black hole
+    x : double
+        cosine of the orbital inclination
+
+    Returns
+    -------
+    tuple(double, double, double, double)
+    """
+    z = sqrt(1 - x**2)
+    f_prime = lambda r: 4 * r**3 + 2 * a**2 * ((1 + z**2) * r + (1 - z**2))
+    g_prime = lambda r: 2 * a
+    h_prime = lambda r: 2 * (r - 1) / (1 - z**2)
+    d_prime = lambda r: 2 * (2 * r - 3) * r**2 + 2 * a**2 * ((1 + z**2) * r - z**2)
+
     return f_prime(r), g_prime(r), h_prime(r), d_prime(r)
 
-def _standardize_params(a,x):
-    """
-    Changes signs of a and x so that a is positive and x encodes the direction of the orbit.
 
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param x: cosine of the orbital inclination
-    :type x: double
-
-    :rtype: tuple(double, double)
-    """
-    return abs(a), x*copysign(1,a)
-
-def energy(a,p,e,x):
-    """
-    Computes the dimensionless energy of a bound orbit with the given parameters
-    
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e <= 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
-    :type x: double
-    
-    :rtype: double
-    """
-    a, x = _standardize_params(a,x)
-
-    if a == 1: raise ValueError("Extreme Kerr not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
-    if not is_stable(a,p,e,x): raise ValueError("Not a stable orbit")
+def _standardize_params(a, x):
+    """Changes signs of a and x so that a is positive 
+    and x encodes the direction of the orbit.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    x : double
+        cosine of the orbital inclination
+
+    Returns
+    -------
+    tuple(double, double)
+    """
+    return abs(a), x * copysign(1, a)
+
+
+def energy(a, p, e, x):
+    """Computes the dimensionless energy of a bound orbit with the given parameters
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e <= 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
+
+    Returns
+    -------
+    double
+    """
+    a, x = _standardize_params(a, x)
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
+    if not is_stable(a, p, e, x):
+        raise ValueError("Not a stable orbit")
 
     # marginally bound case
     if e == 1:
         return 1
-    
+
     # polar case
     if x == 0:
         # expression from ConstantsOfMotion.m in the KerrGeodesics mathematica library
-        return sqrt(-((p*(a**4*(-1 + e**2)**2 + (-4*e**2 + (-2 + p)**2)*p**2 + \
-                2*a**2*p*(-2 + p + e**2*(2 + p))))/ \
-                (a**4*(-1 + e**2)**2*(-1 + e**2 - p) + (3 + e**2 - p)*p**4 - \
-                2*a**2*p**2*(-1 - e**4 + p + e**2*(2 + p)))))
-    
+        return sqrt(
+            -(
+                (
+                    p
+                    * (
+                        a**4 * (-1 + e**2) ** 2
+                        + (-4 * e**2 + (-2 + p) ** 2) * p**2
+                        + 2 * a**2 * p * (-2 + p + e**2 * (2 + p))
+                    )
+                )
+                / (
+                    a**4 * (-1 + e**2) ** 2 * (-1 + e**2 - p)
+                    + (3 + e**2 - p) * p**4
+                    - 2 * a**2 * p**2 * (-1 - e**4 + p + e**2 * (2 + p))
+                )
+            )
+        )
+
     # spherical case
     if e == 0:
         r0 = p
-        f1, g1, h1, d1 = _coefficients(r0,a,x)
-        f2, g2, h2, d2 = _coefficients_derivative(r0,a,x)
+        f1, g1, h1, d1 = _coefficients(r0, a, x)
+        f2, g2, h2, d2 = _coefficients_derivative(r0, a, x)
     # generic case
     else:
-        r1 = p/(1-e)
-        r2 = p/(1+e)
-        f1, g1, h1, d1 = _coefficients(r1,a,x)
-        f2, g2, h2, d2 = _coefficients(r2,a,x)
-    
+        r1 = p / (1 - e)
+        r2 = p / (1 + e)
+        f1, g1, h1, d1 = _coefficients(r1, a, x)
+        f2, g2, h2, d2 = _coefficients(r2, a, x)
+
     # equation B.19 - B.21
-    kappa = d1*h2-h1*d2
-    rho = f1*h2-h1*f2
-    sigma = g1*h2-h1*g2
-    epsilon = d1*g2-g1*d2
-    eta = f1*g2-g1*f2
-    
+    kappa = d1 * h2 - h1 * d2
+    rho = f1 * h2 - h1 * f2
+    sigma = g1 * h2 - h1 * g2
+    epsilon = d1 * g2 - g1 * d2
+    eta = f1 * g2 - g1 * f2
+
     # equation B.22
     return sqrt(
-                (kappa*rho+2*epsilon*sigma-sign(x)*2*sqrt(sigma*(sigma*epsilon**2+rho*epsilon*kappa-eta*kappa**2)))
-                /(rho**2+4*eta*sigma)
-               )
-
-def angular_momentum(a,p,e,x,E=None):
-    """
-    Computes the dimensionless angular momentum of a bound orbit with the given parameters
-    
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e <= 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
-    :type x: double
-    :param E: dimensionless energy of the orbit can be passed in to speed computation if it is already known
-    :type E: double, optional
-    
-    :rtype: double
-    """
-    a, x = _standardize_params(a,x)
-
-    if a == 1: raise ValueError("Extreme Kerr not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
-    if not is_stable(a,p,e,x): raise ValueError("Not a stable orbit")
+        (
+            kappa * rho
+            + 2 * epsilon * sigma
+            - sign(x)
+            * 2
+            * sqrt(sigma * (sigma * epsilon**2 + rho * epsilon * kappa - eta * kappa**2))
+        )
+        / (rho**2 + 4 * eta * sigma)
+    )
+
+
+def angular_momentum(a, p, e, x, E=None):
+    """Computes the dimensionless angular momentum 
+    of a bound orbit with the given parameters
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e <= 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
+    E : double, optional
+        dimensionless energy of the orbit can be passed in to speed
+        computation if it is already known
+
+    Returns
+    -------
+    double
+    """
+    a, x = _standardize_params(a, x)
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
+    if not is_stable(a, p, e, x):
+        raise ValueError("Not a stable orbit")
 
     # compute energy if not given
-    if E is None: E = energy(a,p,e,x)
+    if E is None:
+        E = energy(a, p, e, x)
 
     # polar case
     if x == 0:
         return 0
-    
+
     # marginally bound case
     if e == 1:
-        r2 = p/(1+e)
-        f2, g2, h2, d2 = _coefficients(r2,a,x)
+        r2 = p / (1 + e)
+        f2, g2, h2, d2 = _coefficients(r2, a, x)
         # obtained by solving equation B.17 for L
-        return (-E*g2 + sign(x)*sqrt(-d2*h2 + E**2*(g2**2 + f2*h2)))/h2
-    
+        return (-E * g2 + sign(x) * sqrt(-d2 * h2 + E**2 * (g2**2 + f2 * h2))) / h2
+
     # generic case
     else:
-        r1 = p/(1-e)
-        f1, g1, h1, d1 = _coefficients(r1,a,x)
+        r1 = p / (1 - e)
+        f1, g1, h1, d1 = _coefficients(r1, a, x)
         # obtained by solving equation B.17 for L
-        return (-E*g1 + sign(x)*sqrt(-d1*h1 + E**2*(g1**2 + f1*h1)))/h1
-    
-def carter_constant(a,p,e,x,E=None,L=None):
-    """
-    Computes the dimensionless carter constant of a bound orbit with the given parameters
-    
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e <= 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
-    :type x: double
-    :param E: dimensionless energy of the orbit can be passed in to speed computation if it is already known
-    :type E: double, optional
-    :param L: dimensionless angular momentum of the orbit can be passed in to speed computation if it is already known
-    :type L: double, optional
-    
-    :rtype: double
-    """
-    a, x = _standardize_params(a,x)
-
-    if a == 1:  raise ValueError("Extreme Kerr not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
-    if not is_stable(a,p,e,x): raise ValueError("Not a stable orbit")
+        return (-E * g1 + sign(x) * sqrt(-d1 * h1 + E**2 * (g1**2 + f1 * h1))) / h1
+
+
+def carter_constant(a, p, e, x, E=None, L=None):
+    """Computes the dimensionless carter constant 
+    of a bound orbit with the given parameters
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e <= 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
+    E : double, optional
+        dimensionless energy of the orbit can be passed in to speed
+        computation if it is already known
+    L : double, optional
+        dimensionless angular momentum of the orbit can be passed in to
+        speed computation if it is already known
+
+    Returns
+    -------
+    double
+    """
+    a, x = _standardize_params(a, x)
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
+    if not is_stable(a, p, e, x):
+        raise ValueError("Not a stable orbit")
 
     # polar case
     if x == 0:
         # expression from ConstantsOfMotion.m in the KerrGeodesics mathematica library
-        return -((p**2*(a**4*(-1+e**2)**2+p**4+2*a**2*p*(-2+p+e**2*(2+p)))) \
-                 /(a**4*(-1+e**2)**2*(-1+e**2-p)+(3+e**2-p)*p**4-2*a**2*p**2*(-1-e**4+p+e**2*(2+p))))
-    
-    z = sqrt(1-x**2)
+        return -(
+            (
+                p**2
+                * (
+                    a**4 * (-1 + e**2) ** 2
+                    + p**4
+                    + 2 * a**2 * p * (-2 + p + e**2 * (2 + p))
+                )
+            )
+            / (
+                a**4 * (-1 + e**2) ** 2 * (-1 + e**2 - p)
+                + (3 + e**2 - p) * p**4
+                - 2 * a**2 * p**2 * (-1 - e**4 + p + e**2 * (2 + p))
+            )
+        )
+
+    z = sqrt(1 - x**2)
     # compute energy and angular momentum if not given
-    if E is None: E = energy(a,p,e,x)
-    if L is None: L = angular_momentum(a,p,e,x,E)
+    if E is None:
+        E = energy(a, p, e, x)
+    if L is None:
+        L = angular_momentum(a, p, e, x, E)
     #  equation B.4
-    return z**2 * (a**2 * (1 - E**2) + L**2/(1 - z**2))
+    return z**2 * (a**2 * (1 - E**2) + L**2 / (1 - z**2))
 
-def constants_of_motion(a,p,e,x):
-    """
-    Computes the dimensionless energy, angular momentum, and Carter constant of a bound orbit with the given parameters
-    
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e <= 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
-    :type x: double
-    
-    :return: tuple of constants of motion :math:`(E, L, Q)`
-    :rtype: tuple(double, double, double)
-    """
-    E = energy(a,p,e,x)
-    L = angular_momentum(a,p,e,x,E)
-    Q = carter_constant(a,p,e,x,E,L)
+
+def constants_of_motion(a, p, e, x):
+    """Computes the dimensionless energy, angular momentum, and 
+    Carter constant of a bound orbit with the given parameters
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e <= 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
+
+    Returns
+    -------
+    tuple(double, double, double)
+        tuple of constants of motion :math:`(E, L, Q)`
+    """
+    E = energy(a, p, e, x)
+    L = angular_momentum(a, p, e, x, E)
+    Q = carter_constant(a, p, e, x, E, L)
     return E, L, Q
 
-def apex_from_constants(a,E,L,Q):
-    r"""
-    Computes the orbital parameters :math:`(a,p,e,x)` for a stable bound orbit with the given constants of motion
-    
-    :param a: spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
 
-    :return: tuple of orbital parameters :math:`(a,p,e,x)`
-    :rtype: tuple(double,double,double,double)
+def apex_from_constants(a, E, L, Q):
+    r"""Computes the orbital parameters :math:`(a,p,e,x)` for a 
+    stable bound orbit with the given constants of motion
+
+    Parameters
+    ----------
+    a : double
+        spin parameter
+    E : double
+        dimensionless energy
+    L : double
+        dimensionless angular momentum
+    Q : double
+        dimensionless Carter constant
+
+    Returns
+    -------
+    tuple(double,double,double,double)
+        tuple of orbital parameters :math:`(a,p,e,x)`
     """
     # Radial polynomial
-    R = Polynomial([-a**2*Q, 2*L**2+2*Q+2*a**2*E**2-4*a*E*L, a**2*E**2-L**2-Q-a**2, 2, E**2-1])
+    R = Polynomial(
+        [
+            -(a**2) * Q,
+            2 * L**2 + 2 * Q + 2 * a**2 * E**2 - 4 * a * E * L,
+            a**2 * E**2 - L**2 - Q - a**2,
+            2,
+            E**2 - 1,
+        ]
+    )
     radial_roots = R.roots()
     # numpy returns roots in increasing order
     r4, r3, r2, r1 = radial_roots
 
     # polar polynomial written in terms of z = cos^2(theta)
-    Z = Polynomial([Q,-(Q+a**2*(1-E**2)+L**2),a**2*(1-E**2)])
+    Z = Polynomial([Q, -(Q + a**2 * (1 - E**2) + L**2), a**2 * (1 - E**2)])
     polar_roots = Z.roots()
-    if a == 0: polar_roots = [polar_roots[0], polar_roots[0]]
+    if a == 0:
+        polar_roots = [polar_roots[0], polar_roots[0]]
     z_minus, z_plus = polar_roots
 
-    p = 2*r1*r2/(r1+r2)
-    e = (r1-r2)/(r1+r2)
-    x = np.sign(L)*sqrt(1-z_minus)
+    p = 2 * r1 * r2 / (r1 + r2)
+    e = (r1 - r2) / (r1 + r2)
+    x = np.sign(L) * sqrt(1 - z_minus)
 
     return a, p, e, x
 
-def _S_polar(p,a,e):
-    """
-    Separatrix polynomial for a polar orbit from equation 37 in `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
 
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param e: orbital eccentricity
-    :type e: double
-
-    :rtype: double
-    """
-    return      p**5*(-6 - 2*e + p) \
-                + a**2*p**3*(-4*(-1+e)*(1+e)**2 + (3 + e*(2 + 3*e))*p) \
-                - a**4*(1 + e)**2*p*(6 + 2*e**3 + 2*e*(-1 + p) - 3*p - 3*e**2*(2 + p)) \
-                + a**6*(-1 + e)**2*(1 + e)**4
-
-def _S_equatorial(p,a,e):
-    """
-    Separatrix polynomial for an equatorial orbit from equation 23 in `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
-
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param e: orbital eccentricity
-    :type e: double
-
-    :rtype: double
-    """
-    return      a**4*(-3 - 2*e + e**2)**2 \
-                + p**2*(-6 - 2*e + p)**2 \
-                - 2*a**2*(1 + e)*p*(14 + 2*e**2 + 3*p - e*p)
-
-def _S(p,a,e,x):
-    """
-    Full separatrix polynomial from equation A1 in `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
-
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param e: orbital eccentricity
-    :type e: double
-
-    :rtype: double
+def _S_polar(p, a, e):
+    """Separatrix polynomial for a polar orbit from equation 37 in
+    `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
+
+    Parameters
+    ----------
+    p : double
+        orbital semi-latus rectum
+    a : double
+        dimensionless spin of the black hole
+    e : double
+        orbital eccentricity
+
+    Returns
+    -------
+    double
+    """
+    return (
+        p**5 * (-6 - 2 * e + p)
+        + a**2 * p**3 * (-4 * (-1 + e) * (1 + e) ** 2 + (3 + e * (2 + 3 * e)) * p)
+        - a**4
+        * (1 + e) ** 2
+        * p
+        * (6 + 2 * e**3 + 2 * e * (-1 + p) - 3 * p - 3 * e**2 * (2 + p))
+        + a**6 * (-1 + e) ** 2 * (1 + e) ** 4
+    )
+
+
+def _S_equatorial(p, a, e):
+    """Separatrix polynomial for an equatorial orbit from equation 23 in
+    `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
+
+    Parameters
+    ----------
+    p : double
+        orbital semi-latus rectum
+    a : double
+        dimensionless spin of the black hole
+    e : double
+        orbital eccentricity
+
+    Returns
+    -------
+    double
+    """
+    return (
+        a**4 * (-3 - 2 * e + e**2) ** 2
+        + p**2 * (-6 - 2 * e + p) ** 2
+        - 2 * a**2 * (1 + e) * p * (14 + 2 * e**2 + 3 * p - e * p)
+    )
+
+
+def _S(p, a, e, x):
+    """Full separatrix polynomial from equation A1 in
+    `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
+
+    Parameters
+    ----------
+    p : double
+        orbital semi-latus rectum
+    a : double
+        dimensionless spin of the black hole
+    e : double
+        orbital eccentricity
+
+    Returns
+    -------
+    double
     """
+    # fmt: off
     return -4*(3 + e)*p**11 + p**12 + \
        a**12*(-1 + e)**4*(1 + e)**8*(-1 + x)**4*(1 + x)**4 - \
        4*a**10*(-3 + e)*(-1 + e)**3*(1 + e)**7*p*(-1 + x**2)**4 - \
        4*a**8*(-1 + e)*(1 + e)**5*p**3*(-1 + x)**3*(1 + x)**3* \
         (7 - 7*x**2 - e**2*(-13 + x**2) + e**3*(-5 + x**2) + 7*e*(-1 + x**2)) + \
        8*a**6*(-1 + e)*(1 + e)**3*p**5*(-1 + x**2)**2* \
         (3 + e + 12*x**2 + 4*e*x**2 + e**3*(-5 + 2*x**2) + e**2*(1 + 2*x**2)) - \
@@ -440,135 +582,165 @@
         (-2*(11 - 14*e**2 + 3*e**4)*(-1 + x**2) + \
           a**2*(5 - 5*x**2 - 9*x**4 + 4*e**3*x**2*(-2 + x**2) + \
              e**4*(5 - 5*x**2 + x**4) + e**2*(6 - 6*x**2 + 4*x**4))) + \
        a**2*p**8*(-16*(1 + e)**2*(-3 + 2*e + e**2)*(-1 + x**2) + \
           a**2*(15 - 36*x**2 + 30*x**4 + e**4*(15 - 20*x**2 + 6*x**4) + \
              4*e**3*(5 - 12*x**2 + 6*x**4) + 4*e*(5 - 12*x**2 + 10*x**4) + \
              e**2*(26 - 72*x**2 + 44*x**4)))
+    # fmt: on
 
-def separatrix(a,e,x):
-    """
-    Returns the value of p at the separatrix for the given orbital parameters computed using the bracked root finding method described in `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
-    
-    :param a: dimensionless spin of the black hole (must satisfy 0 <= a < 1)
-    :type a: double
-    :param e: orbital eccentricity (must satisfy 0 <= e <= 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
-    :type x: double
-    
-    :rtype: double
-    """
 
-    if a == 1: raise ValueError("Extreme Kerr not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
+def separatrix(a, e, x):
+    """Returns the value of p at the separatrix for the given orbital parameters 
+    computed using the bracked root finding method described in 
+    `Stein and Warburton <https://doi.org/10.48550/arXiv.1912.07609>`_
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy 0 <= a < 1)
+    e : double
+        orbital eccentricity (must satisfy 0 <= e <= 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 <= x^2 <= 1)
+
+    Returns
+    -------
+    double
+    """
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
 
     if a == 0:
-        return 6+2*e
-    
-    polar_bracket = [1+sqrt(3)+sqrt(3+2*sqrt(3)), 8]
-    p_polar = root_scalar(_S_polar, args=(a,e), bracket=polar_bracket)
-    
+        return 6 + 2 * e
+
+    polar_bracket = [1 + sqrt(3) + sqrt(3 + 2 * sqrt(3)), 8]
+    p_polar = root_scalar(_S_polar, args=(a, e), bracket=polar_bracket)
+
     if x == 0:
         return p_polar.root
-        
-    equatorial_prograde_bracket = [1+e, 6+2*e]
-    p_equatorial_prograde = root_scalar(_S_equatorial,args=(a,e),bracket=equatorial_prograde_bracket)
-    
-    if x == 1: 
+
+    equatorial_prograde_bracket = [1 + e, 6 + 2 * e]
+    p_equatorial_prograde = root_scalar(
+        _S_equatorial, args=(a, e), bracket=equatorial_prograde_bracket
+    )
+
+    if x == 1:
         return p_equatorial_prograde.root
-    
+
     if x == -1:
-        equatorial_retrograde_bracket = [6+2*e, 5+e+4*sqrt(1+e)]
-        p_equatorial_retrograde = root_scalar(_S_equatorial,args=(a,e),bracket=equatorial_retrograde_bracket)
+        equatorial_retrograde_bracket = [6 + 2 * e, 5 + e + 4 * sqrt(1 + e)]
+        p_equatorial_retrograde = root_scalar(
+            _S_equatorial, args=(a, e), bracket=equatorial_retrograde_bracket
+        )
         return p_equatorial_retrograde.root
-    
+
     if x > 0:
-        p = root_scalar(_S,args=(a,e,x),bracket=[p_equatorial_prograde.root, p_polar.root])
+        p = root_scalar(_S, args=(a, e, x), bracket=[p_equatorial_prograde.root, p_polar.root])
         return p.root
-    
+
     if x < 0:
-        p = root_scalar(_S,args=(a,e,x),bracket=[p_polar.root, 12])
+        p = root_scalar(_S, args=(a, e, x), bracket=[p_polar.root, 12])
         return p.root
-    
-def fast_separatrix(a, grid_spacing=0.01):
-    """
-    Constructs a faster separatrix function for a given value of :math:`a` by interpolating over a grid of :math:`e` and :math:`x` values.
 
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param grid_spacing: spacing of the grid over which to interpolate, defaults to 0.01
-    :type grid_spacing: double, optional
 
-    :return: interpolated function of e and x
-    :rtype: scipy.interpolate.RectBivariateSpline
+def fast_separatrix(a, grid_spacing=0.01):
+    """Constructs a faster separatrix function for a given value of :math:`a` 
+    by interpolating over a grid of :math:`e` and :math:`x` values.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    grid_spacing : double, optional
+        spacing of the grid over which to interpolate, defaults to 0.01
+
+    Returns
+    -------
+    scipy.interpolate.RectBivariateSpline
+        interpolated function of e and x
     """
-    
+
     # create grid of e and x values to interpolate over
-    num_e_pts = int(1/grid_spacing)
-    num_x_pts = int(2/grid_spacing)
-    e = np.linspace(0,1,num_e_pts)
-    x = np.linspace(-1,1,num_x_pts)
-    E, X = np.meshgrid(e,x)
+    num_e_pts = int(1 / grid_spacing)
+    num_x_pts = int(2 / grid_spacing)
+    e = np.linspace(0, 1, num_e_pts)
+    x = np.linspace(-1, 1, num_x_pts)
+    E, X = np.meshgrid(e, x)
 
     # compute separatrix values on grid
-    P = np.zeros((num_e_pts,num_x_pts))
+    P = np.zeros((num_e_pts, num_x_pts))
     for i in range(num_e_pts):
         for j in range(num_x_pts):
-            P[i,j] = separatrix(a,E[j,i],X[j,i])
+            P[i, j] = separatrix(a, E[j, i], X[j, i])
 
     # create interpolator
-    interpolator = RectBivariateSpline(e,x,P)
+    interpolator = RectBivariateSpline(e, x, P)
 
     return interpolator
 
-def is_stable(a,p,e,x):
-    """
-    Tests whether or not the given orbital parameters define a stable bound orbit
-    
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity
-    :type e: double
-    :param x: cosine of the orbital inclination
-    :type x: double
-    
-    :rtype: boolean
+
+def is_stable(a, p, e, x):
+    """Tests whether or not the given orbital parameters define a stable bound orbit
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity
+    x : double
+        cosine of the orbital inclination
+
+    Returns
+    -------
+    boolean
     """
-    if p > separatrix(a,e,x):
+    if p > separatrix(a, e, x):
         return True
     return False
 
-def valid_params(a,e,x):
-    """
-    Tests whether the given parameters fall into the allowed ranges
 
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param e: orbital eccentricity
-    :type e: double
-    :param x: cosine of the orbital inclination
-    :type x: double
+def valid_params(a, e, x):
+    """Tests whether the given parameters fall into the allowed ranges
 
-    :rtype: boolean
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    e : double
+        orbital eccentricity
+    x : double
+        cosine of the orbital inclination
+
+    Returns
+    -------
+    boolean
     """
     if (0 <= a <= 1) and (0 <= e <= 1) and (-1 <= x <= 1):
         return True
     return False
 
-def scale_constants(constants,M,mu):
-    """
-    Scales the dimensionless constants of motion to the given mass parameters
-    
-    :param constants: dimensionless constants of motion in the form (E, L, Q)
-    :type constants: tuple
-    :param M: mass of the black hole
-    :type M: double
-    :param mu: mass ratio
-    :type mu: double
-    
-    :rtype: tuple(double, double, double)
+
+def scale_constants(constants, M, mu):
+    """Scales the dimensionless constants of motion to the given mass parameters
+
+    Parameters
+    ----------
+    constants : tuple
+        dimensionless constants of motion in the form (E, L, Q)
+    M : double
+        mass of the black hole
+    mu : double
+        mass ratio
+
+    Returns
+    -------
+    tuple(double, double, double)
     """
     M = mass_in_kg(M)
-    return constants[0]*mu, constants[1]*mu*M, constants[2]*mu**2*M**2
+    return constants[0] * mu, constants[1] * mu * M, constants[2] * mu**2 * M**2
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy/frequencies.py` & `kerrgeopy-0.9.2/kerrgeopy/frequencies.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,578 +1,828 @@
-"""
-Module containing functions for computing frequencies of motion for orbits in Kerr spacetime.
+"""Module containing functions for computing frequencies of motion for orbits in Kerr spacetime.
 Frequencies are computed using the method derived in `Fujita and Hikida <https://doi.org/10.48550/arXiv.0906.1420>`_
 """
 from .constants import _standardize_params
 from .constants import *
 from scipy.special import ellipk, ellipe, elliprj, elliprf, elliprd
 from numpy import sin, cos, sqrt, pi, arcsin, floor, where
 
-def _ellipeinc(phi,m):
-    r"""
-    Incomplete elliptic integral of the second kind defined as :math:`E(\phi,m) = \int_0^{\phi} \sqrt{1-m\sin^2\theta}d\theta`.
+
+def _ellipeinc(phi, m):
+    r"""Incomplete elliptic integral of the second kind defined as 
+    :math:`E(\phi,m) = \int_0^{\phi} \sqrt{1-m\sin^2\theta}d\theta`.
+
+    Parameters
+    ----------
+    phi : double
+    m : double
+
+    Returns
+    -------
+    double
     """
     # count the number of half periods
-    
-    num_cycles = floor(phi/(pi/2))
+
+    num_cycles = floor(phi / (pi / 2))
     # map phi to [0,pi/2]
     phi = abs(arcsin(sin(phi)))
 
     # formula from https://en.wikipedia.org/wiki/Carlson_symmetric_form
-    integral = sin(phi)*elliprf(cos(phi)**2,1-m*sin(phi)**2,1)-1/3*m*sin(phi)**3*elliprd(cos(phi)**2,1-m*sin(phi)**2,1)
-    result = where(num_cycles % 2 == 0, num_cycles*ellipe(m)+integral, (num_cycles+1)*ellipe(m)-integral)
-    
+    integral = sin(phi) * elliprf(cos(phi) ** 2, 1 - m * sin(phi) ** 2, 1) - 1 / 3 * m * sin(
+        phi
+    ) ** 3 * elliprd(cos(phi) ** 2, 1 - m * sin(phi) ** 2, 1)
+    result = where(
+        num_cycles % 2 == 0,
+        num_cycles * ellipe(m) + integral,
+        (num_cycles + 1) * ellipe(m) - integral,
+    )
+
     # return scalar for scalar input
     return result.item() if np.isscalar(phi) else result
 
-def _ellippi(n,m):
-    r"""
-    Complete elliptic integral of the third kind defined as :math:`\Pi(n,m) = \int_0^{\frac{\pi}{2}} \frac{d\theta}{(1-n\sin^2{\theta})\sqrt{1-m\sin^2{\theta}}}`
-    
-    :type n: double
-    :type m: double
 
-    :rtype: double
+def _ellippi(n, m):
+    r"""Complete elliptic integral of the third kind defined as 
+    :math:`\Pi(n,m) = \int_0^{\frac{\pi}{2}} \frac{d\theta}{(1-n\sin^2{\theta})\sqrt{1-m\sin^2{\theta}}}`
+
+    Parameters
+    ----------
+    n : double
+    m : double
+
+    Returns
+    -------
+    double
     """
     # Note: sign of n is reversed from the definition in Fujita and Hikida
 
     # formula from https://en.wikipedia.org/wiki/Carlson_symmetric_form
-    return elliprf(0,1-m,1)+1/3*n*elliprj(0,1-m,1,1-n)
+    return elliprf(0, 1 - m, 1) + 1 / 3 * n * elliprj(0, 1 - m, 1, 1 - n)
 
-def _ellippiinc(phi,n,m):
-    r"""
-    Incomplete elliptic integral of the third kind defined as :math:`\Pi(\phi,n,m) = \int_0^{\phi} \frac{1}{1-n\sin^2\theta}\frac{1}{\sqrt{1-m\sin^2\theta}}d\theta`.
 
-    :type phi: double
-    :type n: double
-    :type m: double
-
-    :rtype: double
+def _ellippiinc(phi, n, m):
+    r"""Incomplete elliptic integral of the third kind defined as 
+    :math:`\Pi(\phi,n,m) = \int_0^{\phi} \frac{1}{1-n\sin^2\theta}\frac{1}{\sqrt{1-m\sin^2\theta}}d\theta`.
+
+    Parameters
+    ----------
+    phi : double
+    n : double
+    m : double
+
+    Returns
+    -------
+    double
     """
     # Note: sign of n is reversed from the definition in Fujita and Hikida
 
     # count the number of half periods
-    num_cycles = floor(phi/(pi/2))
+    num_cycles = floor(phi / (pi / 2))
     # map phi to [0,pi/2]
     phi = abs(arcsin(sin(phi)))
     # formula from https://en.wikipedia.org/wiki/Carlson_symmetric_form
-    integral = sin(phi)*elliprf(cos(phi)**2,1-m*sin(phi)**2,1)+1/3*n*sin(phi)**3*elliprj(cos(phi)**2,1-m*sin(phi)**2,1,1-n*sin(phi)**2)
-
-    result =  where(num_cycles % 2 == 0, num_cycles*_ellippi(n,m)+integral, (num_cycles+1)*_ellippi(n,m)-integral)
+    integral = sin(phi) * elliprf(cos(phi) ** 2, 1 - m * sin(phi) ** 2, 1) + 1 / 3 * n * sin(
+        phi
+    ) ** 3 * elliprj(cos(phi) ** 2, 1 - m * sin(phi) ** 2, 1, 1 - n * sin(phi) ** 2)
+
+    result = where(
+        num_cycles % 2 == 0,
+        num_cycles * _ellippi(n, m) + integral,
+        (num_cycles + 1) * _ellippi(n, m) - integral,
+    )
 
     # return scalar for scalar input
     return result.item() if np.isscalar(phi) else result
 
-def r_frequency(a,p,e,x,constants=None):
-    """
-    Computes the frequency of motion in r in Mino time
 
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e < 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
-    :type x: double
-    :param constants: dimensionless constants of motion for the orbit can be passed in to speed computation if they are already known
-    :type constants: tuple(double, double, double), optional
-
-    :rtype: double
-    """
-    a, x = _standardize_params(a,x)
-
-    if a == 1: raise ValueError("Extreme Kerr not supported")
-    if x == 0: raise ValueError("Polar orbits not supported")
-    if e == 1: raise ValueError("Marginally bound orbits not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
-    if not is_stable(a,p,e,x): raise ValueError("Not a stable orbit")
+def r_frequency(a, p, e, x, constants=None):
+    """Computes the frequency of motion in r in Mino time
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e < 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
+    constants : tuple(double, double, double), optional
+        dimensionless constants of motion for the orbit can be passed in
+        to speed computation if they are already known
+
+    Returns
+    -------
+    double
+    """
+    a, x = _standardize_params(a, x)
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if x == 0:
+        raise ValueError("Polar orbits not supported")
+    if e == 1:
+        raise ValueError("Marginally bound orbits not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
+    if not is_stable(a, p, e, x):
+        raise ValueError("Not a stable orbit")
 
     # compute constants if not passed in
-    if constants is None: constants = constants_of_motion(a,p,e,x)
+    if constants is None:
+        constants = constants_of_motion(a, p, e, x)
     E, L, Q = constants
 
-    r1,r2,r3,r4 = stable_radial_roots(a,p,e,x,constants)
+    r1, r2, r3, r4 = stable_radial_roots(a, p, e, x, constants)
     # equation 13
-    k_r = sqrt((r1-r2)*(r3-r4)/((r1-r3)*(r2-r4)))
+    k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
     # equation 15
-    return pi*sqrt((1-E**2)*(r1-r3)*(r2-r4))/(2*ellipk(k_r**2))
+    return pi * sqrt((1 - E**2) * (r1 - r3) * (r2 - r4)) / (2 * ellipk(k_r**2))
 
-def theta_frequency(a,p,e,x,constants=None):
-    """
-    Computes the frequency of motion in theta in Mino time
-    
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e < 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
-    :type x: double
-    :param constants: dimensionless constants of motion for the orbit can be passed in to speed computation if they are already known
-    :type constants: tuple(double, double, double), optional
-    
-    :rtype: double
-    """
-
-    a, x = _standardize_params(a,x)
-
-    if a == 1: raise ValueError("Extreme Kerr not supported")
-    if x == 0: raise ValueError("Polar orbits not supported")
-    if e == 1: raise ValueError("Marginally bound orbits not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
-    if not is_stable(a,p,e,x): raise ValueError("Not a stable orbit")
+
+def theta_frequency(a, p, e, x, constants=None):
+    """Computes the frequency of motion in theta in Mino time
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e < 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
+    constants : tuple(double, double, double), optional
+        dimensionless constants of motion for the orbit can be passed in
+        to speed computation if they are already known
+
+    Returns
+    -------
+    double
+    """
+
+    a, x = _standardize_params(a, x)
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if x == 0:
+        raise ValueError("Polar orbits not supported")
+    if e == 1:
+        raise ValueError("Marginally bound orbits not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
+    if not is_stable(a, p, e, x):
+        raise ValueError("Not a stable orbit")
 
     # Schwarzschild case
     if a == 0:
-        return p/sqrt(-3-e**2+p)*(sign(x) if e == 0 else 1)
-    
+        return p / sqrt(-3 - e**2 + p) * (sign(x) if e == 0 else 1)
+
     # compute constants if not provided
-    if constants is None: constants = constants_of_motion(a,p,e,x)
+    if constants is None:
+        constants = constants_of_motion(a, p, e, x)
     E, L, Q = constants
-    z_minus, z_plus = stable_polar_roots(a,p,e,x,constants)
-    
+    z_minus, z_plus = stable_polar_roots(a, p, e, x, constants)
+
     # equation 13
-    k_theta = sqrt(z_minus/z_plus)
+    k_theta = sqrt(z_minus / z_plus)
     # simplified form of epsilon0*z_plus
-    e0zp = (a**2*(1-E**2)*(1-z_minus)+L**2)/(L**2*(1-z_minus))
-    
+    e0zp = (a**2 * (1 - E**2) * (1 - z_minus) + L**2) / (L**2 * (1 - z_minus))
+
     # equation 15
-    return pi*L*sqrt(e0zp)/(2*ellipk(k_theta**2))
+    return pi * L * sqrt(e0zp) / (2 * ellipk(k_theta**2))
 
-def phi_frequency(a,p,e,x,constants=None,upsilon_r=None,upsilon_theta=None):
-    """
-    Computes the frequency of motion in phi in Mino time
-    
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e < 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
-    :type x: double
-    :param constants: dimensionless constants of motion for the orbit can be passed in to speed computation if they are already known
-    :type constants: tuple(double, double, double), optional
-    :param upsilon_r: Mino frequency of motion in r can be passed in to speed computation if it is already known
-    :type upsilon_r: double, optional
-    :param upsilon_theta: Mino frequency of motion in theta can be passed in to speed computation if it is already known
-    :type upsilon_theta: double, optional
-    
-    :rtype: double
-    """
-    a, x = _standardize_params(a,x)
-
-    if a == 1: raise ValueError("Extreme Kerr not supported")
-    if x == 0: raise ValueError("Polar orbits not supported")
-    if e == 1: raise ValueError("Marginally bound orbits not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
-    if not is_stable(a,p,e,x): raise ValueError("Not a stable orbit")
+
+def phi_frequency(a, p, e, x, constants=None, upsilon_r=None, upsilon_theta=None):
+    """Computes the frequency of motion in phi in Mino time
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e < 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
+    constants : tuple(double, double, double), optional
+        dimensionless constants of motion for the orbit can be passed in
+        to speed computation if they are already known
+    upsilon_r : double, optional
+        Mino frequency of motion in r can be passed in to speed
+        computation if it is already known
+    upsilon_theta : double, optional
+        Mino frequency of motion in theta can be passed in to speed
+        computation if it is already known
+
+    Returns
+    -------
+    double
+    """
+    a, x = _standardize_params(a, x)
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if x == 0:
+        raise ValueError("Polar orbits not supported")
+    if e == 1:
+        raise ValueError("Marginally bound orbits not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
+    if not is_stable(a, p, e, x):
+        raise ValueError("Not a stable orbit")
 
     # Schwarzschild case
     if a == 0:
-        return sign(x)*p/sqrt(-3-e**2+p)
-    
+        return sign(x) * p / sqrt(-3 - e**2 + p)
+
     # compute constants if they are not passed in
-    if constants is None: constants = constants_of_motion(a,p,e,x)
+    if constants is None:
+        constants = constants_of_motion(a, p, e, x)
     E, L, Q = constants
-    r1,r2,r3,r4 = stable_radial_roots(a,p,e,x,constants)
-    z_minus, z_plus = stable_polar_roots(a,p,e,x,constants)
-    
+    r1, r2, r3, r4 = stable_radial_roots(a, p, e, x, constants)
+    z_minus, z_plus = stable_polar_roots(a, p, e, x, constants)
+
     # compute frequencies if they are not passed in
-    if upsilon_r is None: upsilon_r = r_frequency(a,p,e,x,constants)
-    if upsilon_theta is None: upsilon_theta = theta_frequency(a,p,e,x,constants)
-    
+    if upsilon_r is None:
+        upsilon_r = r_frequency(a, p, e, x, constants)
+    if upsilon_theta is None:
+        upsilon_theta = theta_frequency(a, p, e, x, constants)
+
     # simplified form of epsilon0*z_plus
-    e0zp = (a**2*(1-E**2)*(1-z_minus)+L**2)/(L**2*(1-z_minus))
+    e0zp = (a**2 * (1 - E**2) * (1 - z_minus) + L**2) / (L**2 * (1 - z_minus))
+
+    r_plus = 1 + sqrt(1 - a**2)
+    r_minus = 1 - sqrt(1 - a**2)
+
+    h_plus = (r1 - r2) * (r3 - r_plus) / ((r1 - r3) * (r2 - r_plus))
+    h_minus = (r1 - r2) * (r3 - r_minus) / ((r1 - r3) * (r2 - r_minus))
 
-    r_plus = 1+sqrt(1-a**2)
-    r_minus = 1-sqrt(1-a**2)
-    
-    h_plus = (r1-r2)*(r3-r_plus)/((r1-r3)*(r2-r_plus))
-    h_minus = (r1-r2)*(r3-r_minus)/((r1-r3)*(r2-r_minus))
-    
     # equation 13
-    k_theta = sqrt(z_minus/z_plus)
-    k_r = sqrt((r1-r2)*(r3-r4)/((r1-r3)*(r2-r4)))
-    
+    k_theta = sqrt(z_minus / z_plus)
+    k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
+
     # equation 21
-    return  2*upsilon_theta/(pi*sqrt(e0zp))*_ellippi(z_minus,k_theta**2) \
-            + 2*a*upsilon_r/(pi*(r_plus-r_minus)*sqrt((1-E**2)*(r1-r3)*(r2-r4))) \
-            * ((2*E*r_plus-a*L)/(r3-r_plus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_plus)*_ellippi(h_plus,k_r**2)) \
-               - (2*E*r_minus-a*L)/(r3-r_minus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_minus)*_ellippi(h_minus,k_r**2))
-              )
-
-def gamma(a,p,e,x,constants=None,upsilon_r=None,upsilon_theta=None):
-    """
-    Computes the average rate at which observer time accumulates in Mino time
-    
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e < 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
-    :type x: double
-    :param constants: dimensionless constants of motion for the orbit can be passed in to speed computation if they are already known
-    :type constants: tuple(double, double, double), optional
-    :param upsilon_r: Mino frequency of motion in r can be passed in to speed computation if it is already known
-    :type upsilon_r: double, optional
-    :param upsilon_theta: Mino frequency of motion in theta can be passed in to speed computation if it is already known
-    :type upsilon_theta: double, optional
-    
-    :rtype: double
-    """
-    a, x = _standardize_params(a,x)
-
-    if a == 1: raise ValueError("Extreme Kerr not supported")
-    if x == 0: raise ValueError("Polar orbits not supported")
-    if e == 1: raise ValueError("Marginally bound orbits not supported")
-    if not valid_params(a,e,x): raise ValueError("a^2, e and x^2 must be between 0 and 1")
-    if not is_stable(a,p,e,x): raise ValueError("Not a stable orbit")
-    
+    return 2 * upsilon_theta / (pi * sqrt(e0zp)) * _ellippi(
+        z_minus, k_theta**2
+    ) + 2 * a * upsilon_r / (
+        pi * (r_plus - r_minus) * sqrt((1 - E**2) * (r1 - r3) * (r2 - r4))
+    ) * (
+        (2 * E * r_plus - a * L)
+        / (r3 - r_plus)
+        * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_plus) * _ellippi(h_plus, k_r**2))
+        - (2 * E * r_minus - a * L)
+        / (r3 - r_minus)
+        * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_minus) * _ellippi(h_minus, k_r**2))
+    )
+
+
+def gamma(a, p, e, x, constants=None, upsilon_r=None, upsilon_theta=None):
+    """Computes the average rate at which observer time accumulates in Mino time
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e < 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
+    constants : tuple(double, double, double), optional
+        dimensionless constants of motion for the orbit can be passed in
+        to speed computation if they are already known
+    upsilon_r : double, optional
+        Mino frequency of motion in r can be passed in to speed
+        computation if it is already known
+    upsilon_theta : double, optional
+        Mino frequency of motion in theta can be passed in to speed
+        computation if it is already known
+
+    Returns
+    -------
+    double
+    """
+    a, x = _standardize_params(a, x)
+
+    if a == 1:
+        raise ValueError("Extreme Kerr not supported")
+    if x == 0:
+        raise ValueError("Polar orbits not supported")
+    if e == 1:
+        raise ValueError("Marginally bound orbits not supported")
+    if not valid_params(a, e, x):
+        raise ValueError("a^2, e and x^2 must be between 0 and 1")
+    if not is_stable(a, p, e, x):
+        raise ValueError("Not a stable orbit")
+
     # marginally bound case
     if e == 1:
         return inf
-    
+
     # compute constants if they are not passed in
-    if constants is None: constants = constants_of_motion(a,p,e,x)
+    if constants is None:
+        constants = constants_of_motion(a, p, e, x)
     E, L, Q = constants
-    r1,r2,r3,r4 = stable_radial_roots(a,p,e,x,constants)
-    z_minus, z_plus = stable_polar_roots(a,p,e,x,constants)
-    epsilon0 = a**2*(1-E**2)/L**2
+    r1, r2, r3, r4 = stable_radial_roots(a, p, e, x, constants)
+    z_minus, z_plus = stable_polar_roots(a, p, e, x, constants)
+    epsilon0 = a**2 * (1 - E**2) / L**2
     # simplified form of a**2*sqrt(z_plus/epsilon0)
-    a2sqrt_zp_over_e0 = L**2/((1-E**2)*sqrt(1-z_minus)) if a == 0 else a**2*z_plus/sqrt(epsilon0*z_plus)
-    
+    a2sqrt_zp_over_e0 = (
+        L**2 / ((1 - E**2) * sqrt(1 - z_minus))
+        if a == 0
+        else a**2 * z_plus / sqrt(epsilon0 * z_plus)
+    )
+
     # compute frequencies if they are not passed in
-    if upsilon_r is None: upsilon_r = r_frequency(a,p,e,x,constants)
-    if upsilon_theta is None: upsilon_theta = theta_frequency(a,p,e,x,constants)
-    
-    r_plus = 1+sqrt(1-a**2)
-    r_minus = 1-sqrt(1-a**2)
-    
-    h_r = (r1-r2)/(r1-r3)
-    h_plus = (r1-r2)*(r3-r_plus)/((r1-r3)*(r2-r_plus))
-    h_minus = (r1-r2)*(r3-r_minus)/((r1-r3)*(r2-r_minus))
-    
+    if upsilon_r is None:
+        upsilon_r = r_frequency(a, p, e, x, constants)
+    if upsilon_theta is None:
+        upsilon_theta = theta_frequency(a, p, e, x, constants)
+
+    r_plus = 1 + sqrt(1 - a**2)
+    r_minus = 1 - sqrt(1 - a**2)
+
+    h_r = (r1 - r2) / (r1 - r3)
+    h_plus = (r1 - r2) * (r3 - r_plus) / ((r1 - r3) * (r2 - r_plus))
+    h_minus = (r1 - r2) * (r3 - r_minus) / ((r1 - r3) * (r2 - r_minus))
+
     # equation 13
-    k_theta = 0 if a == 0 else sqrt(z_minus/z_plus)
-    k_r = sqrt((r1-r2)*(r3-r4)/((r1-r3)*(r2-r4)))
-    
+    k_theta = 0 if a == 0 else sqrt(z_minus / z_plus)
+    k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
+
     # equation 21
-    return 4*E + 2*a2sqrt_zp_over_e0*E*upsilon_theta*(ellipk(k_theta**2)-ellipe(k_theta**2))/(pi*L) \
-            + 2*upsilon_r/(pi*sqrt((1-E**2)*(r1-r3)*(r2-r4))) \
-            * (E/2*((r3*(r1+r2+r3)-r1*r2)*ellipk(k_r**2) + (r2-r3)*(r1+r2+r3+r4)*_ellippi(h_r,k_r**2)+ (r1-r3)*(r2-r4)*ellipe(k_r**2)) \
-               + 2*E*(r3*ellipk(k_r**2)+(r2-r3)*_ellippi(h_r,k_r**2))\
-               +2/(r_plus-r_minus)*(((4*E-a*L)*r_plus-2*a**2*E)/(r3-r_plus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_plus)*_ellippi(h_plus,k_r**2)) \
-                                    -((4*E-a*L)*r_minus-2*a**2*E)/(r3-r_minus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_minus)*_ellippi(h_minus,k_r**2))
-                                   )
-              )
-
-def mino_frequencies(a,p,e,x):
-    r"""
-    Computes frequencies of orbital motion in Mino time
-
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e < 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
-    :type x: double
-
-    :return: tuple of the form :math:`(\Upsilon_r, \Upsilon_\theta, \Upsilon_\phi, \Gamma)`
-    :rtype: tuple
-    """
-    constants = constants_of_motion(a,p,e,x)
-    upsilon_r = r_frequency(a,p,e,x,constants)
-    upsilon_theta = theta_frequency(a,p,e,x,constants)
-    upsilon_phi = phi_frequency(a,p,e,x,constants,upsilon_r,upsilon_theta)
-    Gamma = gamma(a,p,e,x,constants,upsilon_r,upsilon_theta)
+    return (
+        4 * E
+        + 2
+        * a2sqrt_zp_over_e0
+        * E
+        * upsilon_theta
+        * (ellipk(k_theta**2) - ellipe(k_theta**2))
+        / (pi * L)
+        + 2
+        * upsilon_r
+        / (pi * sqrt((1 - E**2) * (r1 - r3) * (r2 - r4)))
+        * (
+            E
+            / 2
+            * (
+                (r3 * (r1 + r2 + r3) - r1 * r2) * ellipk(k_r**2)
+                + (r2 - r3) * (r1 + r2 + r3 + r4) * _ellippi(h_r, k_r**2)
+                + (r1 - r3) * (r2 - r4) * ellipe(k_r**2)
+            )
+            + 2 * E * (r3 * ellipk(k_r**2) + (r2 - r3) * _ellippi(h_r, k_r**2))
+            + 2
+            / (r_plus - r_minus)
+            * (
+                ((4 * E - a * L) * r_plus - 2 * a**2 * E)
+                / (r3 - r_plus)
+                * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_plus) * _ellippi(h_plus, k_r**2))
+                - ((4 * E - a * L) * r_minus - 2 * a**2 * E)
+                / (r3 - r_minus)
+                * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_minus) * _ellippi(h_minus, k_r**2))
+            )
+        )
+    )
+
+
+def mino_frequencies(a, p, e, x):
+    r"""Computes frequencies of orbital motion in Mino time
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e < 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
+
+    Returns
+    -------
+    tuple
+        tuple of the form :math:`(\Upsilon_r, \Upsilon_\theta,
+        \Upsilon_\phi, \Gamma)`
+    """
+    constants = constants_of_motion(a, p, e, x)
+    upsilon_r = r_frequency(a, p, e, x, constants)
+    upsilon_theta = theta_frequency(a, p, e, x, constants)
+    upsilon_phi = phi_frequency(a, p, e, x, constants, upsilon_r, upsilon_theta)
+    Gamma = gamma(a, p, e, x, constants, upsilon_r, upsilon_theta)
 
     return upsilon_r, abs(upsilon_theta), upsilon_phi, Gamma
-    
-def fundamental_frequencies(a,p,e,x):
-    r"""
-    Computes frequencies of orbital motion in Boyer-Lindquist time
-
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param p: orbital semi-latus rectum
-    :type p: double
-    :param e: orbital eccentricity (must satisfy 0 <= e < 1)
-    :type e: double
-    :param x: cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
-    :type x: double
-
-    :return: tuple of the form :math:`(\Omega_r, \Omega_\theta, \Omega_\phi)`
-    :rtype: tuple
-    """
-    constants = constants_of_motion(a,p,e,x)
-    upsilon_r = r_frequency(a,p,e,x,constants)
-    upsilon_theta = theta_frequency(a,p,e,x,constants)
-    upsilon_phi = phi_frequency(a,p,e,x,constants,upsilon_r,upsilon_theta)
-    Gamma = gamma(a,p,e,x,constants,upsilon_r,upsilon_theta)
-    
-    return upsilon_r/Gamma, abs(upsilon_theta)/Gamma, upsilon_phi/Gamma
-
-def plunging_mino_frequencies(a,E,L,Q):
-    r"""
-    Computes the radial and polar mino frequencies for a plunging orbit.
-
-    :param a: dimensionless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
 
-    :return: radial and polar mino frequencies :math:`(\Upsilon_r,\Upsilon_\theta)`
-    :rtype: tuple(double,double)
+
+def fundamental_frequencies(a, p, e, x):
+    r"""Computes frequencies of orbital motion in Boyer-Lindquist time
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    p : double
+        orbital semi-latus rectum
+    e : double
+        orbital eccentricity (must satisfy 0 <= e < 1)
+    x : double
+        cosine of the orbital inclination (must satisfy 0 < x^2 <= 1)
+
+    Returns
+    -------
+    tuple
+        tuple of the form :math:`(\Omega_r, \Omega_\theta, \Omega_\phi)`
+    """
+    constants = constants_of_motion(a, p, e, x)
+    upsilon_r = r_frequency(a, p, e, x, constants)
+    upsilon_theta = theta_frequency(a, p, e, x, constants)
+    upsilon_phi = phi_frequency(a, p, e, x, constants, upsilon_r, upsilon_theta)
+    Gamma = gamma(a, p, e, x, constants, upsilon_r, upsilon_theta)
+
+    return upsilon_r / Gamma, abs(upsilon_theta) / Gamma, upsilon_phi / Gamma
+
+
+def plunging_mino_frequencies(a, E, L, Q):
+    r"""Computes the radial and polar mino frequencies for a plunging orbit.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin parameter
+    E : double
+        dimensionless energy
+    L : double
+        dimensionless angular momentum
+    Q : double
+        dimensionless Carter constant
+
+    Returns
+    -------
+    tuple(double,double)
+        radial and polar mino frequencies
+        :math:`(\Upsilon_r,\Upsilon_\theta)`
     """
 
-    radial_roots = plunging_radial_roots(a,E,L,Q)
+    radial_roots = plunging_radial_roots(a, E, L, Q)
     r1, r2, r3, r4 = radial_roots
     rho_r = np.real(r3)
     rho_i = np.imag(r4)
     if np.iscomplex(radial_roots[3]):
         # equation 42
-        A = sqrt((r2-rho_r)**2+rho_i**2)
-        B = sqrt((r1-rho_r)**2+rho_i**2)
-        k_r = sqrt(abs(((r2-r1)**2-(A-B)**2)/(4*A*B)))
+        A = sqrt((r2 - rho_r) ** 2 + rho_i**2)
+        B = sqrt((r1 - rho_r) ** 2 + rho_i**2)
+        k_r = sqrt(abs(((r2 - r1) ** 2 - (A - B) ** 2) / (4 * A * B)))
 
         # equation 52
-        upsilon_r = pi*sqrt(A*B*(1-E**2))/(2*ellipk(k_r**2))
+        upsilon_r = pi * sqrt(A * B * (1 - E**2)) / (2 * ellipk(k_r**2))
 
         # equation 14
-        z1 = sqrt(1/2*(1+(L**2+Q)/(a**2*(1-E**2))-sqrt((1+(L**2+Q)/(a**2*(1-E**2)))**2-4*Q/(a**2*(1-E**2)))))
-        z2 = sqrt(a**2*(1-E**2)/2*(1+(L**2+Q)/(a**2*(1-E**2))+sqrt((1+(L**2+Q)/(a**2*(1-E**2)))**2-4*Q/(a**2*(1-E**2)))))
-        k_theta = a*sqrt(1-E**2)*z1/z2
+        z1 = sqrt(
+            1
+            / 2
+            * (
+                1
+                + (L**2 + Q) / (a**2 * (1 - E**2))
+                - sqrt(
+                    (1 + (L**2 + Q) / (a**2 * (1 - E**2))) ** 2
+                    - 4 * Q / (a**2 * (1 - E**2))
+                )
+            )
+        )
+        z2 = sqrt(
+            a**2
+            * (1 - E**2)
+            / 2
+            * (
+                1
+                + (L**2 + Q) / (a**2 * (1 - E**2))
+                + sqrt(
+                    (1 + (L**2 + Q) / (a**2 * (1 - E**2))) ** 2
+                    - 4 * Q / (a**2 * (1 - E**2))
+                )
+            )
+        )
+        k_theta = a * sqrt(1 - E**2) * z1 / z2
 
         # equation 53
-        upsilon_theta = pi/2*z2/ellipk(k_theta**2)
+        upsilon_theta = pi / 2 * z2 / ellipk(k_theta**2)
     else:
         # polar polynomial written in terms of z = cos^2(theta)
-        Z = Polynomial([Q,-(Q+a**2*(1-E**2)+L**2),a**2*(1-E**2)])
+        Z = Polynomial([Q, -(Q + a**2 * (1 - E**2) + L**2), a**2 * (1 - E**2)])
         polar_roots = Z.roots()
-        if a == 0: polar_roots = [polar_roots[0], polar_roots[0]]
-        constants = (E,L,Q)
-        upsilon_r, upsilon_theta, upsilon_phi, gamma = _mino_frequencies_from_constants(a,constants,radial_roots,polar_roots)
-
+        if a == 0:
+            polar_roots = [polar_roots[0], polar_roots[0]]
+        constants = (E, L, Q)
+        upsilon_r, upsilon_theta, upsilon_phi, gamma = _mino_frequencies_from_constants(
+            a, constants, radial_roots, polar_roots
+        )
 
     return upsilon_r, upsilon_theta
 
-def _r_frequency_from_constants(constants,radial_roots):
-    """
-    Computes the frequency of motion in r in Mino time.
 
-    :param constants: dimensionless constants of motion for the orbit in the form :math:`(E,L,Q)`
-    :type constants: tuple(double, double, double)
-    :param radial_roots: tuple containing the four roots of the radial equation :math:`(r_1, r_2, r_3, r_4)`.
-    :type radial_roots: tuple(double, double, double, double)
+def _r_frequency_from_constants(constants, radial_roots):
+    """Computes the frequency of motion in r in Mino time.
 
-    :rtype: double
+    Parameters
+    ----------
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit in the form
+        :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    radial_roots : tuple(double, double, double, double)
+        tuple containing the four roots of the radial equation
+        :math:`(r_1, r_2, r_3, r_4)`.
+
+    Returns
+    -------
+    double
     """
     E, L, Q = constants
 
-    r1,r2,r3,r4 = radial_roots
+    r1, r2, r3, r4 = radial_roots
     # equation 13
-    k_r = sqrt((r1-r2)*(r3-r4)/((r1-r3)*(r2-r4)))
+    k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
     # equation 15
-    return pi*sqrt((1-E**2)*(r1-r3)*(r2-r4))/(2*ellipk(k_r**2))
+    return pi * sqrt((1 - E**2) * (r1 - r3) * (r2 - r4)) / (2 * ellipk(k_r**2))
 
-def _theta_frequency_from_constants(a,constants,radial_roots,polar_roots):
-    """
-    Computes the frequency of motion in theta in Mino time.
-    
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param constants: dimensionless constants of motion for the orbit in the form :math:`(E,L,Q)`
-    :type constants: tuple(double, double, double)
-    :param radial_roots: tuple containing the four roots of the radial polynomial :math:`(r_1, r_2, r_3, r_4)`.
-    :type radial_roots: tuple(double, double, double, double)
-    :param polar_roots: tuple containing the roots of the polar equation :math:`(z_-, z_+)`
-    :type polar_roots: tuple(double, double)
-    
-    :rtype: double
+
+def _theta_frequency_from_constants(a, constants, radial_roots, polar_roots):
+    """Computes the frequency of motion in theta in Mino time.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit in the form
+        :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    radial_roots : tuple(double, double, double, double)
+        tuple containing the four roots of the radial polynomial
+        :math:`(r_1, r_2, r_3, r_4)`.
+    polar_roots : tuple(double, double)
+        tuple containing the roots of the polar equation :math:`(z_-,
+        z_+)`
+
+    Returns
+    -------
+    double
     """
     r1, r2, r3, r4 = radial_roots
     z_minus, z_plus = polar_roots
     E, L, Q = constants
 
     # Schwarzschild case
     if a == 0:
-        p = 2*r1*r2/(r1+r2)
-        e = (r1-r2)/(r1+r2)
-        return p/sqrt(-3-e**2+p)*(sign(L) if e == 0 else 1)
-    
-    
+        p = 2 * r1 * r2 / (r1 + r2)
+        e = (r1 - r2) / (r1 + r2)
+        return p / sqrt(-3 - e**2 + p) * (sign(L) if e == 0 else 1)
+
     # equation 13
-    k_theta = sqrt(z_minus/z_plus)
+    k_theta = sqrt(z_minus / z_plus)
     # simplified form of epsilon0*z_plus
-    e0zp = (a**2*(1-E**2)*(1-z_minus)+L**2)/(L**2*(1-z_minus))
-    
+    e0zp = (a**2 * (1 - E**2) * (1 - z_minus) + L**2) / (L**2 * (1 - z_minus))
+
     # equation 15
-    return pi*L*sqrt(e0zp)/(2*ellipk(k_theta**2))
+    return pi * L * sqrt(e0zp) / (2 * ellipk(k_theta**2))
 
-def _phi_frequency_from_constants(a,constants,radial_roots,polar_roots,upsilon_r=None,upsilon_theta=None):
-    """
-    Computes the frequency of motion in phi in Mino time.
-    
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param constants: dimensionless constants of motion for the orbit in the form :math:`(E,L,Q)`
-    :type constants: tuple(double, double, double)
-    :param radial_roots: tuple containing the four roots of the radial polynomial :math:`(r_1, r_2, r_3, r_4)`.
-    :type radial_roots: tuple(double, double, double, double)
-    :param polar_roots: tuple containing the roots of the polar equation :math:`(z_-, z_+)`
-    :type polar_roots: tuple(double, double)
-    :param upsilon_r: Mino frequency of motion in r can be passed in to speed computation if it is already known
-    :type upsilon_r: double, optional
-    :param upsilon_theta: Mino frequency of motion in theta can be passed in to speed computation if it is already known
-    :type upsilon_theta: double, optional
-    
-    :rtype: double
+
+def _phi_frequency_from_constants(
+    a, constants, radial_roots, polar_roots, upsilon_r=None, upsilon_theta=None
+):
+    """Computes the frequency of motion in phi in Mino time.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit in the form
+        :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    radial_roots : tuple(double, double, double, double)
+        tuple containing the four roots of the radial polynomial
+        :math:`(r_1, r_2, r_3, r_4)`.
+    polar_roots : tuple(double, double)
+        tuple containing the roots of the polar equation :math:`(z_-, z_+)`
+    upsilon_r : double, optional
+        Mino frequency of motion in r can be passed in to speed
+        computation if it is already known
+    upsilon_theta : double, optional
+        Mino frequency of motion in theta can be passed in to speed
+        computation if it is already known
+
+    Returns
+    -------
+    double
     """
 
     E, L, Q = constants
-    r1,r2,r3,r4 = radial_roots
+    r1, r2, r3, r4 = radial_roots
     z_minus, z_plus = polar_roots
 
     # Schwarzschild case
     if a == 0:
-        p = 2*r1*r2/(r1+r2)
-        e = (r1-r2)/(r1+r2)
-        return sign(L)*p/sqrt(-3-e**2+p)
-    
+        p = 2 * r1 * r2 / (r1 + r2)
+        e = (r1 - r2) / (r1 + r2)
+        return sign(L) * p / sqrt(-3 - e**2 + p)
+
     # compute frequencies if they are not passed in
-    if upsilon_r is None: upsilon_r = _r_frequency_from_constants(a,constants,radial_roots)
-    if upsilon_theta is None: upsilon_theta = _theta_frequency_from_constants(a,constants,radial_roots,polar_roots)
-    
+    if upsilon_r is None:
+        upsilon_r = _r_frequency_from_constants(a, constants, radial_roots)
+    if upsilon_theta is None:
+        upsilon_theta = _theta_frequency_from_constants(a, constants, radial_roots, polar_roots)
+
     # simplified form of epsilon0*z_plus
-    e0zp = (a**2*(1-E**2)*(1-z_minus)+L**2)/(L**2*(1-z_minus))
+    e0zp = (a**2 * (1 - E**2) * (1 - z_minus) + L**2) / (L**2 * (1 - z_minus))
+
+    r_plus = 1 + sqrt(1 - a**2)
+    r_minus = 1 - sqrt(1 - a**2)
+
+    h_plus = (r1 - r2) * (r3 - r_plus) / ((r1 - r3) * (r2 - r_plus))
+    h_minus = (r1 - r2) * (r3 - r_minus) / ((r1 - r3) * (r2 - r_minus))
 
-    r_plus = 1+sqrt(1-a**2)
-    r_minus = 1-sqrt(1-a**2)
-    
-    h_plus = (r1-r2)*(r3-r_plus)/((r1-r3)*(r2-r_plus))
-    h_minus = (r1-r2)*(r3-r_minus)/((r1-r3)*(r2-r_minus))
-    
     # equation 13
-    k_theta = sqrt(z_minus/z_plus)
-    k_r = sqrt((r1-r2)*(r3-r4)/((r1-r3)*(r2-r4)))
-    
+    k_theta = sqrt(z_minus / z_plus)
+    k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
+
     # equation 21
-    return  2*upsilon_theta/(pi*sqrt(e0zp))*_ellippi(z_minus,k_theta**2) \
-            + 2*a*upsilon_r/(pi*(r_plus-r_minus)*sqrt((1-E**2)*(r1-r3)*(r2-r4))) \
-            * ((2*E*r_plus-a*L)/(r3-r_plus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_plus)*_ellippi(h_plus,k_r**2)) \
-               - (2*E*r_minus-a*L)/(r3-r_minus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_minus)*_ellippi(h_minus,k_r**2))
-              )
-
-def _gamma_from_constants(a,constants,radial_roots,polar_roots,upsilon_r=None,upsilon_theta=None):
-    """
-    Computes the average rate at which observer time accumulates in Mino time.
-    
-    :param a: dimensionless spin of the black hole
-    :type a: double
-    :param constants: dimensionless constants of motion for the orbit in the form :math:`(E,L,Q)`
-    :type constants: tuple(double, double, double)
-    :param radial_roots: tuple containing the four roots of the radial polynomial :math:`(r_1, r_2, r_3, r_4)`.
-    :type radial_roots: tuple(double, double, double, double)
-    :param polar_roots: tuple containing the roots of the polar equation :math:`(z_-, z_+)`
-    :type polar_roots: tuple(double, double)
-    :param upsilon_r: Mino frequency of motion in r can be passed in to speed computation if it is already known
-    :type upsilon_r: double, optional
-    :param upsilon_theta: Mino frequency of motion in theta can be passed in to speed computation if it is already known
-    :type upsilon_theta: double, optional
-    
-    :rtype: double
+    return 2 * upsilon_theta / (pi * sqrt(e0zp)) * _ellippi(
+        z_minus, k_theta**2
+    ) + 2 * a * upsilon_r / (
+        pi * (r_plus - r_minus) * sqrt((1 - E**2) * (r1 - r3) * (r2 - r4))
+    ) * (
+        (2 * E * r_plus - a * L)
+        / (r3 - r_plus)
+        * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_plus) * _ellippi(h_plus, k_r**2))
+        - (2 * E * r_minus - a * L)
+        / (r3 - r_minus)
+        * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_minus) * _ellippi(h_minus, k_r**2))
+    )
+
+
+def _gamma_from_constants(
+    a, constants, radial_roots, polar_roots, upsilon_r=None, upsilon_theta=None
+):
+    """Computes the average rate at which observer time accumulates in Mino time.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit in the form
+        :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    radial_roots : tuple(double, double, double, double)
+        tuple containing the four roots of the radial polynomial
+        :math:`(r_1, r_2, r_3, r_4)`.
+    polar_roots : tuple(double, double)
+        tuple containing the roots of the polar equation :math:`(z_-, z_+)`
+    upsilon_r : double, optional
+        Mino frequency of motion in r can be passed in to speed
+        computation if it is already known
+    upsilon_theta : double, optional
+        Mino frequency of motion in theta can be passed in to speed
+        computation if it is already known
+
+    Returns
+    -------
+    double
     """
-    r1,r2,r3,r4 = radial_roots
+    r1, r2, r3, r4 = radial_roots
     z_minus, z_plus = polar_roots
 
-    e = (r1-r2)/(r1+r2)
+    e = (r1 - r2) / (r1 + r2)
     # marginally bound case
     if e == 1:
         return inf
-    
+
     E, L, Q = constants
-    
-    epsilon0 =  a**2*(1-E**2)/L**2
+
+    epsilon0 = a**2 * (1 - E**2) / L**2
     # simplified form of a**2*sqrt(z_plus/epsilon0)
-    a2sqrt_zp_over_e0 = L**2/((1-E**2)*sqrt(1-z_minus)) if a == 0 else a**2*z_plus/sqrt(epsilon0*z_plus)
-    
+    a2sqrt_zp_over_e0 = (
+        L**2 / ((1 - E**2) * sqrt(1 - z_minus))
+        if a == 0
+        else a**2 * z_plus / sqrt(epsilon0 * z_plus)
+    )
+
     # compute frequencies if they are not passed in
-    if upsilon_r is None: upsilon_r = _r_frequency_from_constants(a,constants,radial_roots)
-    if upsilon_theta is None: upsilon_theta = _theta_frequency_from_constants(a,constants,radial_roots,polar_roots)
-    
-    r_plus = 1+sqrt(1-a**2)
-    r_minus = 1-sqrt(1-a**2)
-    
-    h_r = (r1-r2)/(r1-r3)
-    h_plus = (r1-r2)*(r3-r_plus)/((r1-r3)*(r2-r_plus))
-    h_minus = (r1-r2)*(r3-r_minus)/((r1-r3)*(r2-r_minus))
-    
+    if upsilon_r is None:
+        upsilon_r = _r_frequency_from_constants(a, constants, radial_roots)
+    if upsilon_theta is None:
+        upsilon_theta = _theta_frequency_from_constants(a, constants, radial_roots, polar_roots)
+
+    r_plus = 1 + sqrt(1 - a**2)
+    r_minus = 1 - sqrt(1 - a**2)
+
+    h_r = (r1 - r2) / (r1 - r3)
+    h_plus = (r1 - r2) * (r3 - r_plus) / ((r1 - r3) * (r2 - r_plus))
+    h_minus = (r1 - r2) * (r3 - r_minus) / ((r1 - r3) * (r2 - r_minus))
+
     # equation 13
-    k_theta = 0 if a == 0 else sqrt(z_minus/z_plus)
-    k_r = sqrt((r1-r2)*(r3-r4)/((r1-r3)*(r2-r4)))
-    
+    k_theta = 0 if a == 0 else sqrt(z_minus / z_plus)
+    k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
+
     # equation 21
-    return 4*E + 2*a2sqrt_zp_over_e0*E*upsilon_theta*(ellipk(k_theta**2)-ellipe(k_theta**2))/(pi*L) \
-            + 2*upsilon_r/(pi*sqrt((1-E**2)*(r1-r3)*(r2-r4))) \
-            * (E/2*((r3*(r1+r2+r3)-r1*r2)*ellipk(k_r**2) + (r2-r3)*(r1+r2+r3+r4)*_ellippi(h_r,k_r**2)+ (r1-r3)*(r2-r4)*ellipe(k_r**2)) \
-               + 2*E*(r3*ellipk(k_r**2)+(r2-r3)*_ellippi(h_r,k_r**2))\
-               +2/(r_plus-r_minus)*(((4*E-a*L)*r_plus-2*a**2*E)/(r3-r_plus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_plus)*_ellippi(h_plus,k_r**2)) \
-                                    -((4*E-a*L)*r_minus-2*a**2*E)/(r3-r_minus)*(ellipk(k_r**2)-(r2-r3)/(r2-r_minus)*_ellippi(h_minus,k_r**2))
-                                   )
-              )
-
-def _mino_frequencies_from_constants(a,constants,radial_roots,polar_roots):
-    r"""
-    Computes frequencies of orbital motion in Mino time.
-
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param constants: dimensionless constants of motion for the orbit in the form :math:`(E,L,Q)`
-    :type constants: tuple(double, double, double)
-    :param radial_roots: tuple containing the four roots of the radial polynomial :math:`(r_1, r_2, r_3, r_4)`.
-    :type radial_roots: tuple(double, double, double, double)
-    :param polar_roots: tuple containing the roots of the polar equation :math:`(z_-, z_+)`
-    :type polar_roots: tuple(double, double)
-
-    :return: tuple of frequencies in the form :math:`(\Upsilon_r, \Upsilon_\theta, \Upsilon_\phi, \Gamma)`
-    :rtype: tuple(double, double, double, double)
-    """
-    upsilon_r = _r_frequency_from_constants(constants,radial_roots)
-    upsilon_theta = _theta_frequency_from_constants(a,constants,radial_roots,polar_roots)
-    upsilon_phi = _phi_frequency_from_constants(a,constants,radial_roots,polar_roots,upsilon_r,upsilon_theta)
-    Gamma = _gamma_from_constants(a,constants,radial_roots,polar_roots,upsilon_r,upsilon_theta)
+    return (
+        4 * E
+        + 2
+        * a2sqrt_zp_over_e0
+        * E
+        * upsilon_theta
+        * (ellipk(k_theta**2) - ellipe(k_theta**2))
+        / (pi * L)
+        + 2
+        * upsilon_r
+        / (pi * sqrt((1 - E**2) * (r1 - r3) * (r2 - r4)))
+        * (
+            E
+            / 2
+            * (
+                (r3 * (r1 + r2 + r3) - r1 * r2) * ellipk(k_r**2)
+                + (r2 - r3) * (r1 + r2 + r3 + r4) * _ellippi(h_r, k_r**2)
+                + (r1 - r3) * (r2 - r4) * ellipe(k_r**2)
+            )
+            + 2 * E * (r3 * ellipk(k_r**2) + (r2 - r3) * _ellippi(h_r, k_r**2))
+            + 2
+            / (r_plus - r_minus)
+            * (
+                ((4 * E - a * L) * r_plus - 2 * a**2 * E)
+                / (r3 - r_plus)
+                * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_plus) * _ellippi(h_plus, k_r**2))
+                - ((4 * E - a * L) * r_minus - 2 * a**2 * E)
+                / (r3 - r_minus)
+                * (ellipk(k_r**2) - (r2 - r3) / (r2 - r_minus) * _ellippi(h_minus, k_r**2))
+            )
+        )
+    )
+
+
+def _mino_frequencies_from_constants(a, constants, radial_roots, polar_roots):
+    r"""Computes frequencies of orbital motion in Mino time.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit in the form
+        :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    radial_roots : tuple(double, double, double, double)
+        tuple containing the four roots of the radial polynomial
+        :math:`(r_1, r_2, r_3, r_4)`.
+    polar_roots : tuple(double, double)
+        tuple containing the roots of the polar equation :math:`(z_-, z_+)`
+
+    Returns
+    -------
+    tuple(double, double, double, double)
+        tuple of frequencies in the form :math:`(\Upsilon_r,
+        \Upsilon_\theta, \Upsilon_\phi, \Gamma)`
+    """
+    upsilon_r = _r_frequency_from_constants(constants, radial_roots)
+    upsilon_theta = _theta_frequency_from_constants(a, constants, radial_roots, polar_roots)
+    upsilon_phi = _phi_frequency_from_constants(
+        a, constants, radial_roots, polar_roots, upsilon_r, upsilon_theta
+    )
+    Gamma = _gamma_from_constants(
+        a, constants, radial_roots, polar_roots, upsilon_r, upsilon_theta
+    )
 
     return upsilon_r, abs(upsilon_theta), upsilon_phi, Gamma
-    
-def _fundamental_frequencies_from_constants(a,constants,radial_roots,polar_roots):
-    r"""
-    Computes frequencies of orbital motion in Boyer-Lindquist time.
-
-    :param a: dimensionless spin of the black hole (must satisfy -1 < a < 1)
-    :type a: double
-    :param constants: dimensionless constants of motion for the orbit in the form :math:`(E,L,Q)`
-    :type constants: tuple(double, double, double)
-    :param radial_roots: tuple containing the four roots of the radial polynomial :math:`(r_1, r_2, r_3, r_4)`.
-    :type radial_roots: tuple(double, double, double, double)
-    :param polar_roots: tuple containing the roots of the polar equation :math:`(z_-, z_+)`
-    :type polar_roots: tuple(double, double)
-
-    :return: tuple of frequencies in the form :math:`(\Omega_r, \Omega_\theta, \Omega_\phi)`
-    :rtype: tuple(double, double, double)
-    """
-    upsilon_r = _r_frequency_from_constants(constants,radial_roots)
-    upsilon_theta = _theta_frequency_from_constants(a,constants,radial_roots,polar_roots)
-    upsilon_phi = _phi_frequency_from_constants(a,constants,radial_roots,polar_roots,upsilon_r,upsilon_theta)
-    Gamma = _gamma_from_constants(a,constants,radial_roots,polar_roots,upsilon_r,upsilon_theta)
 
-    return upsilon_r/Gamma, abs(upsilon_theta)/Gamma, upsilon_phi/Gamma
+
+def _fundamental_frequencies_from_constants(a, constants, radial_roots, polar_roots):
+    r"""Computes frequencies of orbital motion in Boyer-Lindquist time.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin of the black hole (must satisfy -1 < a < 1)
+    constants : tuple(double, double, double)
+        dimensionless constants of motion for the orbit in the form
+        :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    radial_roots : tuple(double, double, double, double)
+        tuple containing the four roots of the radial polynomial
+        :math:`(r_1, r_2, r_3, r_4)`.
+    polar_roots : tuple(double, double)
+        tuple containing the roots of the polar equation :math:`(z_-, z_+)`
+
+    Returns
+    -------
+    tuple(double, double, double)
+        tuple of frequencies in the form :math:`(\Omega_r,
+        \Omega_\theta, \Omega_\phi)`
+    """
+    upsilon_r = _r_frequency_from_constants(constants, radial_roots)
+    upsilon_theta = _theta_frequency_from_constants(a, constants, radial_roots, polar_roots)
+    upsilon_phi = _phi_frequency_from_constants(
+        a, constants, radial_roots, polar_roots, upsilon_r, upsilon_theta
+    )
+    Gamma = _gamma_from_constants(
+        a, constants, radial_roots, polar_roots, upsilon_r, upsilon_theta
+    )
+
+    return upsilon_r / Gamma, abs(upsilon_theta) / Gamma, upsilon_phi / Gamma
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy/initial_conditions.py` & `kerrgeopy-0.9.2/kerrgeopy/initial_conditions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,257 +1,383 @@
-"""
-Module containing functions to compute orbital properties from initial conditions
-"""
-from .frequencies import _r_frequency_from_constants, _theta_frequency_from_constants, plunging_mino_frequencies
+"""Module containing functions to compute orbital properties from initial conditions"""
+from .frequencies import (
+    _r_frequency_from_constants,
+    _theta_frequency_from_constants,
+    plunging_mino_frequencies,
+)
 from .constants import plunging_radial_roots
 import numpy as np
 from numpy import sin, cos, sqrt, pi, arcsin, arccos
 from numpy.polynomial import Polynomial
 from scipy.special import ellipkinc
 
-def constants_from_initial_conditions(a,initial_position,initial_velocity):
-    r"""
-    Computes the constants of motion :math:`(E,L,Q)` of the orbit with the given initial conditions
-
-    :param a: spin parameter
-    :type a: double
-    :param initial_position: initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
-    :type initial_position: tuple(double,double,double,double)
-    :param initial_velocity: initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
-    :type initial_velocity: tuple(double,double,double,double)
 
-    :return: tuple of constants of motion :math:`(E,L,Q)`
-    :rtype: tuple(double,double,double)
+def constants_from_initial_conditions(a, initial_position, initial_velocity):
+    r"""Computes the constants of motion :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})` 
+    of the orbit with the given initial conditions.
+
+    Parameters
+    ----------
+    a : double
+        spin parameter
+    initial_position : tuple(double,double,double,double)
+        initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
+    initial_velocity : tuple(double,double,double,double)
+        initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
+
+    Returns
+    -------
+    tuple(double,double,double)
+        tuple of constants of motion :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
     """
 
     t0, r0, theta0, phi0 = initial_position
     dt0, dr0, dtheta0, dphi0 = initial_velocity
 
-    sigma = r0**2+a**2*cos(theta0)**2
-    delta = r0**2-2*r0+a**2
+    sigma = r0**2 + a**2 * cos(theta0) ** 2
+    delta = r0**2 - 2 * r0 + a**2
 
     # solve for E and L by writing the t and phi geodesic equations as a matrix equation
     A = np.array(
-        [[(r0**2+a**2)**2/delta-a**2*(1-cos(theta0)**2), a-a*(r0**2+a**2)/delta],
-        [a*(r0**2+a**2)/delta-a, 1/(1-cos(theta0)**2)-a**2/delta]]
+        [
+            [
+                (r0**2 + a**2) ** 2 / delta - a**2 * (1 - cos(theta0) ** 2),
+                a - a * (r0**2 + a**2) / delta,
+            ],
+            [a * (r0**2 + a**2) / delta - a, 1 / (1 - cos(theta0) ** 2) - a**2 / delta],
+        ]
     )
-    b = np.array([sigma*dt0,sigma*dphi0])
-    E, L = np.linalg.solve(A,b)
+    b = np.array([sigma * dt0, sigma * dphi0])
+    E, L = np.linalg.solve(A, b)
 
     # solve for Q by substituting E and L back into the theta equation
-    Q = ((sigma*dtheta0*sin(theta0))**2 + cos(theta0)**2*(a**2*(1-E**2)*(1-cos(theta0)**2)+L**2))/(1-cos(theta0)**2)
+    Q = (
+        (sigma * dtheta0 * sin(theta0)) ** 2
+        + cos(theta0) ** 2 * (a**2 * (1 - E**2) * (1 - cos(theta0) ** 2) + L**2)
+    ) / (1 - cos(theta0) ** 2)
 
     return E, L, Q
 
-def is_stable(a,initial_position,initial_velocity,constants=None,tol=1e-4):
-    r"""
-    Tests whether the orbit with the given initial conditions is stable
-
-    :param a: spin parameter
-    :type a: double
-    :param initial_position: initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
-    :type initial_position: tuple(double,double,double,double)
-    :param initial_velocity: initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
-    :type initial_velocity: tuple(double,double,double,double)
-    :param constants: tuple of constants of motion :math:`(E,L,Q)` can be passed in to avoid recomputing them
-    :type constants: tuple(double,double,double), optional
-    :param tol: numerical tolerance used when comparing :math:`r_0` to radial roots, defaults to 1e-4
-    :type tol: double, optional
 
-    :return: True if the orbit is stable, False otherwise
-    :rtype: bool
+def is_stable(a, initial_position, initial_velocity, constants=None, tol=1e-4):
+    r"""Tests whether the orbit with the given initial conditions is stable
+
+    Parameters
+    ----------
+    a : double
+        spin parameter
+    initial_position : tuple(double,double,double,double)
+        initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
+    initial_velocity : tuple(double,double,double,double)
+        initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
+    constants : tuple(double,double,double), optional
+        tuple of constants of motion :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})` 
+        can be passed in to avoid recomputing them
+    tol : double, optional
+        numerical tolerance used when comparing :math:`r_0` to radial
+        roots, defaults to 1e-4
+
+    Returns
+    -------
+    bool
+        True if the orbit is stable, False otherwise
     """
 
     t0, r0, theta0, phi0 = initial_position
     # recompute constants if they are not passed in
-    if constants is None: constants = constants_from_initial_conditions(a,initial_position,initial_velocity)
+    if constants is None:
+        constants = constants_from_initial_conditions(a, initial_position, initial_velocity)
     E, L, Q = constants
 
     # radial polynomial
-    R = Polynomial([-a**2*Q, 2*L**2+2*Q+2*a**2*E**2-4*a*E*L, a**2*E**2-L**2-Q-a**2, 2, E**2-1])
+    R = Polynomial(
+        [
+            -(a**2) * Q,
+            2 * L**2 + 2 * Q + 2 * a**2 * E**2 - 4 * a * E * L,
+            a**2 * E**2 - L**2 - Q - a**2,
+            2,
+            E**2 - 1,
+        ]
+    )
     radial_roots = R.roots()
 
     # get the real roots and the complex roots
     real_roots = np.sort(np.real(radial_roots[np.isreal(radial_roots)]))
     complex_roots = radial_roots[np.iscomplex(radial_roots)]
 
     # event horizon radius
-    r_minus = 1-sqrt(1-a**2)
+    r_minus = 1 - sqrt(1 - a**2)
 
-    if len(complex_roots) == 4: 
+    if len(complex_roots) == 4:
         raise ValueError("Not a physical orbit")
-    
+
     if len(complex_roots) == 2:
         return False
-    
+
     r4, r3, r2, r1 = real_roots
     # r4 < r3 < [r2 < r_minus < r_plus < r1]
-    if (r2 < r_minus) & (r0 <= r1+tol) & (r0 >= r2-tol):
+    if (r2 < r_minus) & (r0 <= r1 + tol) & (r0 >= r2 - tol):
         return False
     # r4 < r_minus < r_plus < r3 < [r2 < r1]
-    if (r2 > r_minus) & (r0 <= r1+tol) & (r0 >= r2-tol):
+    if (r2 > r_minus) & (r0 <= r1 + tol) & (r0 >= r2 - tol):
         return True
     # [r4 < r_minus < r_plus < r3] < r2 < r1
-    if (r2 > r_minus) & (r0 <= r3+tol) & (r0 >= r4-tol):
+    if (r2 > r_minus) & (r0 <= r3 + tol) & (r0 >= r4 - tol):
         return False
-    
+
     raise ValueError("Not a physical orbit")
-    
 
-def stable_orbit_initial_phases(a,initial_position,initial_velocity,constants=None,radial_roots=None,upsilon_r=None,upsilon_theta=None,tol=1e-4):
-    r"""
-    Computes the initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})` of a stable bound orbit with the given initial conditions.
-    Computes phases with respect to the starting point :math:`(t_0,r_0,\theta_0,\phi_0) = (0,r_\text{min},\theta_\text{min},0)`.
-
-    :param a: spin parameter
-    :type a: double
-    :param initial_position: initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
-    :type initial_position: tuple(double,double,double,double)
-    :param initial_velocity: initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
-    :type initial_velocity: tuple(double,double,double,double)
-    :param constants: constants of motion :math:`(E,L,Q)` can be passed in to avoid recomputing them
-    :type constants: tuple(double,double,double), optional
-    :param radial_roots: radial roots :math:`(r_1,r_2,r_3,r_4)` can be passed in to avoid recomputing them
-    :type radial_roots: tuple(double,double,double,double), optional
-    :param upsilon_r: radial frequency :math:`\Upsilon_r` can be passed in to avoid recomputing it
-    :type upsilon_r: double, optional
-    :param upsilon_theta: polar frequency :math:`\Upsilon_\theta` can be passed in to avoid recomputing it
-    :type upsilon_theta: double, optional
-    :param tol: numerical tolerance used when checking for turning points, defaults to 1e-4
-    :type tol: double, optional
 
-    :return: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-    :rtype: tuple(double,double,double,double)
+def stable_orbit_initial_phases(
+    a,
+    initial_position,
+    initial_velocity,
+    constants=None,
+    radial_roots=None,
+    upsilon_r=None,
+    upsilon_theta=None,
+    tol=1e-4,
+):
+    r"""Computes the initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})` 
+    of a stable bound orbit with the given initial conditions. Computes phases 
+    with respect to the starting point :math:`(t_0,r_0,\theta_0,\phi_0) = 
+    (0,r_\text{min},\theta_\text{min},0)`.
+
+    Parameters
+    ----------
+    a : double
+        spin parameter
+    initial_position : tuple(double,double,double,double)
+        initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
+    initial_velocity : tuple(double,double,double,double)
+        initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
+    constants : tuple(double,double,double), optional
+        constants of motion :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})` 
+        can be passed in to avoid recomputing them
+    radial_roots : tuple(double,double,double,double), optional
+        radial roots :math:`(r_1,r_2,r_3,r_4)` can be passed in to avoid
+        recomputing them
+    upsilon_r : double, optional
+        radial frequency :math:`\Upsilon_r` can be passed in to avoid
+        recomputing it
+    upsilon_theta : double, optional
+        polar frequency :math:`\Upsilon_\theta` can be passed in to
+        avoid recomputing it
+    tol : double, optional
+        numerical tolerance used when checking for turning points,
+        defaults to 1e-4
+
+    Returns
+    -------
+    tuple(double,double,double,double)
+        tuple of initial phases
+        :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
     """
     t0, r0, theta0, phi0 = initial_position
     dt0, dr0, dtheta0, dphi0 = initial_velocity
 
     # recompute constants if they are not passed in
-    if constants is None: constants = constants_from_initial_conditions(a,initial_position,initial_velocity)
+    if constants is None:
+        constants = constants_from_initial_conditions(a, initial_position, initial_velocity)
     E, L, Q = constants
 
     # polar polynomial written in terms of z = cos^2(theta)
-    Z = Polynomial([Q,-(Q+a**2*(1-E**2)+L**2),a**2*(1-E**2)])
+    Z = Polynomial([Q, -(Q + a**2 * (1 - E**2) + L**2), a**2 * (1 - E**2)])
     polar_roots = Z.roots()
-    if a == 0: polar_roots = [polar_roots[0], polar_roots[0]]
+    if a == 0:
+        polar_roots = [polar_roots[0], polar_roots[0]]
     z_minus, z_plus = polar_roots
 
     # recompute radial roots if they are not passed in
     if radial_roots is None:
-        R = Polynomial([-a**2*Q, 2*L**2+2*Q+2*a**2*E**2-4*a*E*L, a**2*E**2-L**2-Q-a**2, 2, E**2-1])
+        R = Polynomial(
+            [
+                -(a**2) * Q,
+                2 * L**2 + 2 * Q + 2 * a**2 * E**2 - 4 * a * E * L,
+                a**2 * E**2 - L**2 - Q - a**2,
+                2,
+                E**2 - 1,
+            ]
+        )
         radial_roots = R.roots()
         # numpy returns roots in increasing order
         r4, r3, r2, r1 = radial_roots
     else:
         r1, r2, r3, r4 = radial_roots
 
     # check for turning points in r
-    if abs(r0-r2) < tol:
+    if abs(r0 - r2) < tol:
         q_r0 = 0
-    elif abs(r0-r1) < tol:
+    elif abs(r0 - r1) < tol:
         q_r0 = pi
     else:
         # compute r frequency
-        if upsilon_r is None: upsilon_r = _r_frequency_from_constants(constants,radial_roots)
+        if upsilon_r is None:
+            upsilon_r = _r_frequency_from_constants(constants, radial_roots)
 
         # Fujita and Hikida equation 13
-        k_r = sqrt((r1-r2)*(r3-r4)/((r1-r3)*(r2-r4)))
-        y_r = sqrt((r1-r3)*(r0-r2)/((r1-r2)*(r0-r3)))
+        k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
+        y_r = sqrt((r1 - r3) * (r0 - r2) / ((r1 - r2) * (r0 - r3)))
         # Fujita and Hikida equation 26
-        lambda_r0 = 1/sqrt(1-E**2)*2/sqrt((r1-r3)*(r2-r4))*ellipkinc(arcsin(y_r),k_r**2)
+        lambda_r0 = (
+            1
+            / sqrt(1 - E**2)
+            * 2
+            / sqrt((r1 - r3) * (r2 - r4))
+            * ellipkinc(arcsin(y_r), k_r**2)
+        )
 
         # Fujita and Hikida equation 24
-        q_r0 = lambda_r0*upsilon_r if dr0 > 0 else 2*pi-lambda_r0*upsilon_r
+        q_r0 = lambda_r0 * upsilon_r if dr0 > 0 else 2 * pi - lambda_r0 * upsilon_r
 
     # Fujita and Hikida equation 11
     theta_min = arccos(sqrt(z_minus))
-    theta_max = pi-theta_min
+    theta_max = pi - theta_min
 
     # check for turning points in theta
-    if abs(theta0-theta_min) < tol:
+    if abs(theta0 - theta_min) < tol:
         q_theta0 = 0
-    elif abs(theta0-theta_max) < tol:
+    elif abs(theta0 - theta_max) < tol:
         q_theta0 = pi
     else:
         # compute theta frequency
-        if upsilon_theta is None: upsilon_theta = _theta_frequency_from_constants(a,constants,radial_roots,polar_roots)
-
-        k_theta = sqrt(z_minus/z_plus)
-        y_theta = cos(theta0)/sqrt(z_minus)
-        e0zp = (a**2*(1-E**2)*(1-z_minus)+L**2)/(L**2*(1-z_minus))
+        if upsilon_theta is None:
+            upsilon_theta = _theta_frequency_from_constants(
+                a, constants, radial_roots, polar_roots
+            )
+
+        k_theta = sqrt(z_minus / z_plus)
+        y_theta = cos(theta0) / sqrt(z_minus)
+        e0zp = (a**2 * (1 - E**2) * (1 - z_minus) + L**2) / (L**2 * (1 - z_minus))
 
         # Fujita and Hikida equation 37
-        lambda_theta0 = 1/(L*sqrt(e0zp))*ellipkinc(arcsin(y_theta),k_theta**2)
+        lambda_theta0 = 1 / (L * sqrt(e0zp)) * ellipkinc(arcsin(y_theta), k_theta**2)
 
         # Fujita and Hikida equation 36
-        if dtheta0 < 0: q_theta0 = lambda_theta0*upsilon_theta+3*pi/2
-        if (dtheta0 == 0) & (theta0 == pi/2): q_theta0 = 0 # special case for equatorial orbits
-        if dtheta0 >= 0: q_theta0 = pi/2-lambda_theta0*upsilon_theta
+        if dtheta0 < 0:
+            q_theta0 = lambda_theta0 * upsilon_theta + 3 * pi / 2
+        if (dtheta0 == 0) & (theta0 == pi / 2):
+            q_theta0 = 0  # special case for equatorial orbits
+        if dtheta0 >= 0:
+            q_theta0 = pi / 2 - lambda_theta0 * upsilon_theta
 
     q_t0 = t0
     q_phi0 = phi0
 
     return q_t0, q_r0, q_theta0, q_phi0
 
-def plunging_orbit_initial_phases(a,initial_position,initial_velocity,constants=None,radial_roots=None,tol=1e-4):
-    r"""
-    Computes the initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})` of a plunging orbit with the given initial conditions.
-    Computes phases with respect to the starting point :math:`(t_0,r_0,\theta_0,\phi_0) = (0,r_\text{min},\theta_{\text{min}},0)`.
-
-    :param a: spin parameter
-    :type a: double
-    :param initial_position: initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
-    :type initial_position: tuple(double,double,double,double)
-    :param initial_velocity: initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
-    :type initial_velocity: tuple(double,double,double,double)
-    :param constants: constants of motion :math:`(E,L,Q)` can be passed in to avoid recomputing them
-    :type constants: tuple(double,double,double), optional
-    :param radial_roots: radial roots :math:`(r_1,r_2,r_3,r_4)` can be passed in to avoid recomputing them
-    :type radial_roots: tuple(double,double,double,double), optional
-    :param tol: numerical tolerance used when checking for turning points, defaults to 1e-4
-    :type tol: double, optional
 
-    :return: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-    :rtype: tuple(double,double,double,double)
+def plunging_orbit_initial_phases(
+    a, initial_position, initial_velocity, constants=None, radial_roots=None, tol=1e-4
+):
+    r"""Computes the initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})` 
+    of a plunging orbit with the given initial conditions. Computes phases with 
+    respect to the starting point :math:`(t_0,r_0,\theta_0,\phi_0) = 
+    (0,r_\text{min},\theta_{\text{min}},0)`.
+
+    Parameters
+    ----------
+    a : double
+        spin parameter
+    initial_position : tuple(double,double,double,double)
+        initial position :math:`(t_0,r_0,\theta_0,\phi_0)`
+    initial_velocity : tuple(double,double,double,double)
+        initial four-velocity :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
+    constants : tuple(double,double,double), optional
+        constants of motion :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})` 
+        can be passed in to avoid recomputing them
+    radial_roots : tuple(double,double,double,double), optional
+        radial roots :math:`(r_1,r_2,r_3,r_4)` can be passed in to avoid
+        recomputing them
+    tol : double, optional
+        numerical tolerance used when checking for turning points,
+        defaults to 1e-4
+
+    Returns
+    -------
+    tuple(double,double,double,double)
+        tuple of initial phases
+        :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
     """
     t0, r0, theta0, phi0 = initial_position
     dt0, dr0, dtheta0, dphi0 = initial_velocity
 
     # recompute constants if they are not passed in
-    if constants is None: constants = constants_from_initial_conditions(a,initial_position,initial_velocity)
+    if constants is None:
+        constants = constants_from_initial_conditions(a, initial_position, initial_velocity)
     E, L, Q = constants
 
     # recompute radial roots if they are not passed in
-    if radial_roots is None: radial_roots = plunging_radial_roots(a,E,L,Q)
+    if radial_roots is None:
+        radial_roots = plunging_radial_roots(a, E, L, Q)
     r1, r2, r3, r4 = radial_roots
 
-
     if np.iscomplex(r3):
-        z1 = sqrt(1/2*(1+(L**2+Q)/(a**2*(1-E**2))-sqrt((1+(L**2+Q)/(a**2*(1-E**2)))**2-4*Q/(a**2*(1-E**2)))))
-        z2 = sqrt(a**2*(1-E**2)/2*(1+(L**2+Q)/(a**2*(1-E**2))+sqrt((1+(L**2+Q)/(a**2*(1-E**2)))**2-4*Q/(a**2*(1-E**2)))))
-        k_theta = a*sqrt(1-E**2)*z1/z2
+        z1 = sqrt(
+            1
+            / 2
+            * (
+                1
+                + (L**2 + Q) / (a**2 * (1 - E**2))
+                - sqrt(
+                    (1 + (L**2 + Q) / (a**2 * (1 - E**2))) ** 2
+                    - 4 * Q / (a**2 * (1 - E**2))
+                )
+            )
+        )
+        z2 = sqrt(
+            a**2
+            * (1 - E**2)
+            / 2
+            * (
+                1
+                + (L**2 + Q) / (a**2 * (1 - E**2))
+                + sqrt(
+                    (1 + (L**2 + Q) / (a**2 * (1 - E**2))) ** 2
+                    - 4 * Q / (a**2 * (1 - E**2))
+                )
+            )
+        )
+        k_theta = a * sqrt(1 - E**2) * z1 / z2
         rho_r = np.real(r3)
         rho_i = np.imag(r4)
 
         # equation 47
-        A = sqrt((r2-rho_r)**2+rho_i**2)
-        B = sqrt((r1-rho_r)**2+rho_i**2)
-        k_r = sqrt(((r2-r1)**2-(A-B)**2)/(4*A*B))
+        A = sqrt((r2 - rho_r) ** 2 + rho_i**2)
+        B = sqrt((r1 - rho_r) ** 2 + rho_i**2)
+        k_r = sqrt(((r2 - r1) ** 2 - (A - B) ** 2) / (4 * A * B))
         # equation 49
-        lambda_r0 = -1/sqrt((1-E**2)*A*B)*ellipkinc(pi/2-arcsin((B*(r2-r0)-A*(r0-r1))/(B*(r2-r0)+A*(r0-r1))),k_r**2)
+        lambda_r0 = (
+            -1
+            / sqrt((1 - E**2) * A * B)
+            * ellipkinc(
+                pi / 2 - arcsin((B * (r2 - r0) - A * (r0 - r1)) / (B * (r2 - r0) + A * (r0 - r1))),
+                k_r**2,
+            )
+        )
         # derived by inverting equation 29
-        lambda_theta0 = 1/z2*ellipkinc(arcsin(cos(theta0)/z1),k_theta**2)
+        lambda_theta0 = 1 / z2 * ellipkinc(arcsin(cos(theta0) / z1), k_theta**2)
 
-        upsilon_r, upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
+        upsilon_r, upsilon_theta = plunging_mino_frequencies(a, E, L, Q)
 
         q_t0 = t0
-        q_r0 = -lambda_r0*upsilon_r if dr0 > 0 else 2*pi+lambda_r0*upsilon_r
+        q_r0 = -lambda_r0 * upsilon_r if dr0 > 0 else 2 * pi + lambda_r0 * upsilon_r
 
-        if dtheta0 < 0: q_theta0 = lambda_theta0*upsilon_theta+3*pi/2
-        if (dtheta0 == 0) & (theta0 == pi/2): q_theta0 = 0 # special case for equatorial orbits
-        if dtheta0 >= 0: q_theta0 = pi/2-lambda_theta0*upsilon_theta
+        if dtheta0 < 0:
+            q_theta0 = lambda_theta0 * upsilon_theta + 3 * pi / 2
+        if (dtheta0 == 0) & (theta0 == pi / 2):
+            q_theta0 = 0  # special case for equatorial orbits
+        if dtheta0 >= 0:
+            q_theta0 = pi / 2 - lambda_theta0 * upsilon_theta
 
         q_phi0 = phi0
 
         return q_t0, q_r0, q_theta0, q_phi0
     else:
-        return stable_orbit_initial_phases(a,initial_position,initial_velocity,constants=constants,radial_roots=radial_roots,tol=tol)
+        return stable_orbit_initial_phases(
+            a,
+            initial_position,
+            initial_velocity,
+            constants=constants,
+            radial_roots=radial_roots,
+            tol=tol,
+        )
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy/orbit.py` & `kerrgeopy-0.9.2/kerrgeopy/orbit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,566 +1,880 @@
-"""
-Module containing the Orbit class
-"""
+"""Module containing the Orbit class"""
 from .spacetime import KerrSpacetime
 from .initial_conditions import *
 from .units import *
-from .constants import scale_constants, apex_from_constants, stable_polar_roots, stable_radial_roots
+from .constants import (
+    scale_constants,
+    apex_from_constants,
+    stable_polar_roots,
+    stable_radial_roots,
+)
 from .frequencies import mino_frequencies, fundamental_frequencies
 from numpy import sin, cos, sqrt, pi
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d.art3d import Line3DCollection
 from matplotlib.animation import FuncAnimation
 from matplotlib.animation import FFMpegWriter
 from tqdm import tqdm
 
+
 class Orbit:
-    r"""
-    Class representing an orbit in Kerr spacetime defined using initial conditions.
+    r"""Class representing an orbit in Kerr spacetime defined using initial conditions.
 
-    :param a: spin parameter
-    :type a: double
-    :param initial_position: initial position of the orbit :math:`(t_0,r_0,\theta_0,\phi_0)`
-    :type initial_position: tuple(double,double,double,double)
-    :param initial_velocity: initial four-velocity of the orbit :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
-    :type initial_velocity: tuple(double,double,double,double)
-    :param M: mass of the primary in solar masses
-    :type M: double, optional
-    :param mu: mass of the smaller body in solar masses
-    :type mu: double, optional
-
-    :ivar a: spin parameter
-    :ivar initial_position: initial position of the orbit :math:`(t_0,r_0,\theta_0,\phi_0)`
-    :ivar initial_velocity: initial four-velocity of the orbit :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
-    :ivar E: dimensionless energy
-    :ivar L: dimensionless angular momentum
-    :ivar Q: dimensionless carter constant
-    :ivar stable: boolean indicating whether the orbit is stable
-    :ivar upsilon_r: dimensionless radial orbital frequency in Mino time
-    :ivar upsilon_theta: dimensionless polar orbital frequency in Mino time
+    Parameters
+    ----------
+    a : double
+        spin parameter
+    initial_position : tuple(double,double,double,double)
+        initial position of the orbit :math:`(t_0,r_0,\theta_0,\phi_0)`
+    initial_velocity : tuple(double,double,double,double)
+        initial four-velocity of the orbit
+        :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
+    M : double, optional
+        mass of the primary in solar masses
+    mu : double, optional
+        mass of the smaller body in solar masses
+
+    Attributes
+    ----------
+    a
+        spin parameter
+    initial_position
+        initial position of the orbit :math:`(t_0,r_0,\theta_0,\phi_0)`
+    initial_velocity
+        initial four-velocity of the orbit
+        :math:`(u^t_0,u^r_0,u^\theta_0,u^\phi_0)`
+    E
+        dimensionless energy
+    L
+        dimensionless angular momentum
+    Q
+        dimensionless carter constant
+    stable
+        boolean indicating whether the orbit is stable
+    upsilon_r
+        dimensionless radial orbital frequency in Mino time
+    upsilon_theta
+        dimensionless polar orbital frequency in Mino time
     """
-    def __init__(self,a,initial_position,initial_velocity, M=None, mu=None):
-        self.a, self.initial_position, self.initial_velocity, self.M, self.mu = a, initial_position, initial_velocity, M, mu
+
+    def __init__(self, a, initial_position, initial_velocity, M=None, mu=None):
+        self.a, self.initial_position, self.initial_velocity, self.M, self.mu = (
+            a,
+            initial_position,
+            initial_velocity,
+            M,
+            mu,
+        )
 
         # check if initial four-velocity is valid
         spacetime = KerrSpacetime(a)
-        initial_norm =  spacetime.norm(*initial_position,initial_velocity)
-        if initial_norm >= 0: raise ValueError("Initial velocity is not timelike")
-        if abs(initial_norm + 1) > 1e-6: raise ValueError("Initial velocity is not normalized")
-
-        E, L, Q = constants_from_initial_conditions(a,initial_position,initial_velocity)
+        initial_norm = spacetime.norm(*initial_position, initial_velocity)
+        if initial_norm >= 0:
+            raise ValueError("Initial velocity is not timelike")
+        if abs(initial_norm + 1) > 1e-6:
+            raise ValueError("Initial velocity is not normalized")
+
+        E, L, Q = constants_from_initial_conditions(
+            a, initial_position, initial_velocity
+        )
         self.E, self.L, self.Q = E, L, Q
 
-        if is_stable(a,initial_position,initial_velocity):
+        if is_stable(a, initial_position, initial_velocity):
             self.stable = True
-            a, p, e, x = apex_from_constants(a,E,L,Q)
+            a, p, e, x = apex_from_constants(a, E, L, Q)
             self.a, self.p, self.e, self.x = a, p, e, x
-            self.upsilon_r, self.upsilon_theta, self.upsilon_phi, self.gamma = mino_frequencies(a,p,e,x)
-            self.omega_r, self.omega_theta, self.omega_phi = fundamental_frequencies(a,p,e,x)
-            self.initial_phases = stable_orbit_initial_phases(a,initial_position,initial_velocity)
+            (
+                self.upsilon_r,
+                self.upsilon_theta,
+                self.upsilon_phi,
+                self.gamma,
+            ) = mino_frequencies(a, p, e, x)
+            self.omega_r, self.omega_theta, self.omega_phi = fundamental_frequencies(
+                a, p, e, x
+            )
+            self.initial_phases = stable_orbit_initial_phases(
+                a, initial_position, initial_velocity
+            )
         else:
-            if a == 0: raise ValueError("Schwarzschild plunges are not currently supported")
+            if a == 0:
+                raise ValueError("Schwarzschild plunges are not currently supported")
             self.stable = False
-            self.upsilon_r, self.upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
-            self.initial_phases = plunging_orbit_initial_phases(a,initial_position,initial_velocity)
-
-    def trajectory_deltas(self,initial_phases=None):
-        r"""
-        Computes the trajectory deltas :math:`t_r(q_r)`, :math:`t_\theta(q_\theta)`, :math:`\phi_r(q_r)` and :math:`\phi_\theta(q_\theta)`
-
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
+            self.upsilon_r, self.upsilon_theta = plunging_mino_frequencies(a, E, L, Q)
+            self.initial_phases = plunging_orbit_initial_phases(
+                a, initial_position, initial_velocity
+            )
 
-        :return: tuple of trajectory deltas :math:`(t_r(q_r), t_\theta(q_\theta), \phi_r(q_r),\phi_\theta(q_\theta))`
-        :rtype: tuple(function, function, function, function)
+    def trajectory_deltas(self, initial_phases=None):
+        r"""Computes the trajectory deltas :math:`t_r(q_r)`, :math:`t_\theta(q_\theta)`,
+        :math:`\phi_r(q_r)` and :math:`\phi_\theta(q_\theta)`
+
+        Parameters
+        ----------
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+
+        Returns
+        -------
+        tuple(function, function, function, function)
+            tuple of trajectory deltas :math:`(t_r(q_r),
+            t_\theta(q_\theta), \phi_r(q_r),\phi_\theta(q_\theta))`
         """
-        if initial_phases is None: initial_phases = self.initial_phases
+        if initial_phases is None:
+            initial_phases = self.initial_phases
         q_t0, q_r0, q_theta0, q_phi0 = initial_phases
 
         if self.stable:
             from .stable import radial_solutions, polar_solutions
 
-            constants = (self.E,self.L,self.Q)
-            radial_roots = stable_radial_roots(self.a,self.p,self.e,self.x,constants)
-            polar_roots = stable_polar_roots(self.a,self.p,self.e,self.x,constants)
-            r, t_r, phi_r = radial_solutions(self.a,constants,radial_roots)
-            theta, t_theta, phi_theta = polar_solutions(self.a,constants,polar_roots)
+            constants = (self.E, self.L, self.Q)
+            radial_roots = stable_radial_roots(
+                self.a, self.p, self.e, self.x, constants
+            )
+            polar_roots = stable_polar_roots(self.a, self.p, self.e, self.x, constants)
+            r, t_r, phi_r = radial_solutions(self.a, constants, radial_roots)
+            theta, t_theta, phi_theta = polar_solutions(self.a, constants, polar_roots)
         else:
-            radial_roots = plunging_radial_roots(self.a,self.E,self.L,self.Q)
+            radial_roots = plunging_radial_roots(self.a, self.E, self.L, self.Q)
             if np.iscomplex(radial_roots[3]):
-                from .plunge import plunging_radial_solutions_complex, plunging_polar_solutions
+                from .plunge import (
+                    plunging_radial_solutions_complex,
+                    plunging_polar_solutions,
+                )
 
                 # adjust q_theta0 so that initial conditions are consistent with stable orbits
-                q_theta0 = q_theta0 + pi/2
-                r, t_r, phi_r = plunging_radial_solutions_complex(self.a,self.E,self.L,self.Q)
-                theta, t_theta, phi_theta = plunging_polar_solutions(self.a,self.E,self.L,self.Q)
+                q_theta0 = q_theta0 + pi / 2
+                r, t_r, phi_r = plunging_radial_solutions_complex(
+                    self.a, self.E, self.L, self.Q
+                )
+                theta, t_theta, phi_theta = plunging_polar_solutions(
+                    self.a, self.E, self.L, self.Q
+                )
             else:
                 from .stable import radial_solutions, polar_solutions
 
-                constants = (self.E,self.L,self.Q)
-                r, t_r, phi_r = radial_solutions(self.a,constants,radial_roots)
-                theta, t_theta, phi_theta = polar_solutions(self.a,constants,radial_roots)
-        
-        return (lambda q_r: t_r(q_r+q_r0), lambda q_theta: t_theta(q_theta+q_theta0),
-                lambda q_r: phi_r(q_r+q_r0), lambda q_theta: phi_theta(q_theta+q_theta0))
-
-    def trajectory(self,initial_phases=None,distance_units="natural",time_units="natural"):
-        r"""
-        Computes the components of the trajectory as a function of Mino time
-        
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
-        :param distance_units: units to compute the radial component of the trajectory in (options are "natural", "mks", "cgs", "au" and "km"), defaults to "natural"
-        :type distance_units: str, optional
-        :param time_units: units to compute the time component of the trajectory in (options are "natural", "mks", "cgs", and "days"), defaults to "natural"
-        :type time_units: str, optional
-
-        :return: tuple of functions :math:`(t(\lambda), r(\lambda), \theta(\lambda), \phi(\lambda))`
-        :rtype: tuple(function, function, function, function)
+                constants = (self.E, self.L, self.Q)
+                r, t_r, phi_r = radial_solutions(self.a, constants, radial_roots)
+                theta, t_theta, phi_theta = polar_solutions(
+                    self.a, constants, radial_roots
+                )
+
+        return (
+            lambda q_r: t_r(q_r + q_r0),
+            lambda q_theta: t_theta(q_theta + q_theta0),
+            lambda q_r: phi_r(q_r + q_r0),
+            lambda q_theta: phi_theta(q_theta + q_theta0),
+        )
+
+    def trajectory(
+        self, initial_phases=None, distance_units="natural", time_units="natural"
+    ):
+        r"""Computes the components of the trajectory as a function of Mino time
+
+        Parameters
+        ----------
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+        distance_units : str, optional
+            units to compute the radial component of the trajectory in
+            (options are "natural", "mks", "cgs", "au" and "km"),
+            defaults to "natural"
+        time_units : str, optional
+            units to compute the time component of the trajectory in
+            (options are "natural", "mks", "cgs", and "days"), defaults
+            to "natural"
+
+        Returns
+        -------
+        tuple(function, function, function, function)
+            tuple of functions :math:`(t(\lambda), r(\lambda),
+            \theta(\lambda), \phi(\lambda))`
         """
-        if initial_phases is None: initial_phases = self.initial_phases
+        if initial_phases is None:
+            initial_phases = self.initial_phases
         if self.stable:
             from .stable import stable_trajectory
-            return stable_trajectory(self.a,self.p,self.e,self.x,initial_phases,self.M,distance_units,time_units)
+
+            return stable_trajectory(
+                self.a,
+                self.p,
+                self.e,
+                self.x,
+                initial_phases,
+                self.M,
+                distance_units,
+                time_units,
+            )
         else:
             from .plunge import plunging_trajectory
-            return plunging_trajectory(self.a,self.E,self.L,self.Q,initial_phases,self.M,distance_units,time_units)
-        
+
+            return plunging_trajectory(
+                self.a,
+                self.E,
+                self.L,
+                self.Q,
+                initial_phases,
+                self.M,
+                distance_units,
+                time_units,
+            )
+
     def constants_of_motion(self, units="natural"):
-        """
-        Computes the energy, angular momentum, and carter constant for the orbit. Computes dimensionless constants in geometried units by default.
+        """Computes the energy, angular momentum, and carter constant for the orbit.
+        Computes dimensionless constants in geometried units by default.
         M and mu must be defined in order to convert to physical units.
 
-        :param units: units to return the constants of motion in (options are "natural", "mks" and "cgs"), defaults to "natural"
-        :type units: str, optional
-
-        :return: tuple of the form (E, L, Q)
-        :rtype: tuple(double, double, double)
+        Parameters
+        ----------
+        units : str, optional
+            units to return the constants of motion in (options are
+            "natural", "mks" and "cgs"), defaults to "natural"
+
+        Returns
+        -------
+        tuple(double, double, double)
+            tuple of the form (E, L, Q)
         """
         constants = self.E, self.L, self.Q
         if units == "natural":
             return constants
-        
-        if self.M is None or self.mu is None: raise ValueError("M and mu must be specified to convert constants of motion to physical units")
-        
+
+        if self.M is None or self.mu is None:
+            raise ValueError(
+                "M and mu must be specified to convert constants of motion to physical units"
+            )
+
         if units == "mks":
-            E, L, Q = scale_constants(constants,1,self.mu/self.M)
-            return energy_in_joules(E,self.M), angular_momentum_in_mks(L,self.M), carter_constant_in_mks(Q,self.M)
-        
-        if units == "cgs":
-            E, L, Q = scale_constants(constants,1,self.mu/self.M)
-            return energy_in_ergs(E,self.M), angular_momentum_in_cgs(L,self.M), carter_constant_in_cgs(Q,self.M)
-        
-        raise ValueError("units must be one of 'natural', 'mks', or 'cgs'")
-    
+            E, L, Q = scale_constants(constants, 1, self.mu / self.M)
+            return (
+                energy_in_joules(E, self.M),
+                angular_momentum_in_mks(L, self.M),
+                carter_constant_in_mks(Q, self.M),
+            )
 
-    def four_velocity(self,initial_phases=None):
-        r"""
-        Computes the four velocity of the orbit as a function of Mino time using the geodesic equation.
+        if units == "cgs":
+            E, L, Q = scale_constants(constants, 1, self.mu / self.M)
+            return (
+                energy_in_ergs(E, self.M),
+                angular_momentum_in_cgs(L, self.M),
+                carter_constant_in_cgs(Q, self.M),
+            )
 
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
+        raise ValueError("units must be one of 'natural', 'mks', or 'cgs'")
 
-        :return: components of the four velocity (i.e. :math:`u^t,u^r,u^\theta,u^\phi`)
-        :rtype: tuple(function, function, function, function)
+    def four_velocity(self, initial_phases=None):
+        r"""Computes the four velocity of the orbit as a function of Mino time using
+        the geodesic equation.
+
+        Parameters
+        ----------
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+
+        Returns
+        -------
+        tuple(function, function, function, function)
+            components of the four velocity (i.e.
+            :math:`u^t,u^r,u^\theta,u^\phi`)
         """
-        if initial_phases is None: initial_phases = self.initial_phases
+        if initial_phases is None:
+            initial_phases = self.initial_phases
         t, r, theta, phi = self.trajectory(initial_phases)
         spacetime = KerrSpacetime(self.a)
         constants = self.E, self.L, self.Q
 
-        return spacetime.four_velocity(t,r,theta,phi,constants,self.upsilon_r,self.upsilon_theta,initial_phases)
-    
-    def _four_velocity_norm(self,initial_phases=None):
-        r"""
-        Computes the norm of the four velocity of the orbit as a function of Mino time
-
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
-
-        :return: norm of the four velocity :math:`g_{\mu\nu}u^\mu u^\nu`
-        :rtype: function
+        return spacetime.four_velocity(
+            t,
+            r,
+            theta,
+            phi,
+            constants,
+            self.upsilon_r,
+            self.upsilon_theta,
+            initial_phases,
+        )
+
+    def _four_velocity_norm(self, initial_phases=None):
+        r"""Computes the norm of the four velocity of the orbit as a function of Mino time
+
+        Parameters
+        ----------
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+
+        Returns
+        -------
+        function
+            norm of the four velocity :math:`g_{\mu\nu}u^\mu u^\nu`
         """
-        if initial_phases is None: initial_phases = self.initial_phases
+        if initial_phases is None:
+            initial_phases = self.initial_phases
         t, r, theta, phi = self.trajectory(initial_phases)
         spacetime = KerrSpacetime(self.a)
         constants = self.E, self.L, self.Q
-        t_prime, r_prime, theta_prime, phi_prime = self.four_velocity(initial_phases=initial_phases)
+        t_prime, r_prime, theta_prime, phi_prime = self.four_velocity(
+            initial_phases=initial_phases
+        )
 
         def norm(time):
-            u = [t_prime(time),r_prime(time),theta_prime(time),phi_prime(time)]
-            return spacetime.norm(t(time),r(time),theta(time),phi(time),u)
+            u = [t_prime(time), r_prime(time), theta_prime(time), phi_prime(time)]
+            return spacetime.norm(t(time), r(time), theta(time), phi(time), u)
 
         return norm
-    
-    def _numerical_four_velocity_norm(self,dx=1e-6,initial_phases=None):
-        r"""
-        Computes the norm of the four velocity of the orbit as a function of Mino time
 
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
+    def _numerical_four_velocity_norm(self, dx=1e-6, initial_phases=None):
+        r"""Computes the norm of the four velocity of the orbit as a function of Mino time
 
-        :return: norm of the four velocity :math:`g_{\mu\nu}u^\mu u^\nu`
-        :rtype: function
+        Parameters
+        ----------
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+
+        Returns
+        -------
+        function
+            norm of the four velocity :math:`g_{\mu\nu}u^\mu u^\nu`
         """
-        if initial_phases is None: initial_phases = self.initial_phases
+        if initial_phases is None:
+            initial_phases = self.initial_phases
         t, r, theta, phi = self.trajectory(initial_phases)
         spacetime = KerrSpacetime(self.a)
         constants = self.E, self.L, self.Q
-        t_prime, r_prime, theta_prime, phi_prime = self.numerical_four_velocity(dx=dx,initial_phases=initial_phases)
+        t_prime, r_prime, theta_prime, phi_prime = self.numerical_four_velocity(
+            dx=dx, initial_phases=initial_phases
+        )
 
         def norm(time):
-            u = [t_prime(time),r_prime(time),theta_prime(time),phi_prime(time)]
-            return spacetime.norm(t(time),r(time),theta(time),phi(time),u)
+            u = [t_prime(time), r_prime(time), theta_prime(time), phi_prime(time)]
+            return spacetime.norm(t(time), r(time), theta(time), phi(time), u)
 
         return norm
-    
-    def numerical_four_velocity(self,dx=1e-6,initial_phases=None):
-        r"""
-        Computes the four velocity of the orbit as a function of Mino time using numerical differentiation
-
-        :param dx: step size, defaults to 1e-6
-        :type dx: double, optional
-        :param initial_phases: initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`, defaults to None
-        :type initial_phases: tuple(double,double,double,double), optional
 
-        :return: components of the four velocity (i.e. :math:`u^t,u^r,u^\theta,u^\phi`)
-        :rtype: tuple(function, function, function, function)
+    def numerical_four_velocity(self, dx=1e-6, initial_phases=None):
+        r"""Computes the four velocity of the orbit as a function of Mino time using
+        numerical differentiation.
+
+        Parameters
+        ----------
+        dx : double, optional
+            step size, defaults to 1e-6
+        initial_phases : tuple(double,double,double,double), optional
+            initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`, defaults
+            to None
+
+        Returns
+        -------
+        tuple(function, function, function, function)
+            components of the four velocity (i.e.
+            :math:`u^t,u^r,u^\theta,u^\phi`)
         """
-        if initial_phases is None: initial_phases = self.initial_phases
+        if initial_phases is None:
+            initial_phases = self.initial_phases
         t, r, theta, phi = self.trajectory(initial_phases)
 
         def u_t(mino_time):
-            sigma = r(mino_time)**2 + self.a**2*cos(theta(mino_time))**2
-            return (-t(mino_time+2*dx)+8*t(mino_time+dx)-8*t(mino_time-dx)+t(mino_time-2*dx))/(12*dx*sigma)
+            sigma = r(mino_time) ** 2 + self.a**2 * cos(theta(mino_time)) ** 2
+            return (
+                -t(mino_time + 2 * dx)
+                + 8 * t(mino_time + dx)
+                - 8 * t(mino_time - dx)
+                + t(mino_time - 2 * dx)
+            ) / (12 * dx * sigma)
+
         def u_r(mino_time):
-            sigma = r(mino_time)**2 + self.a**2*cos(theta(mino_time))**2
-            return (-r(mino_time+2*dx)+8*r(mino_time+dx)-8*r(mino_time-dx)+r(mino_time-2*dx))/(12*dx*sigma)
+            sigma = r(mino_time) ** 2 + self.a**2 * cos(theta(mino_time)) ** 2
+            return (
+                -r(mino_time + 2 * dx)
+                + 8 * r(mino_time + dx)
+                - 8 * r(mino_time - dx)
+                + r(mino_time - 2 * dx)
+            ) / (12 * dx * sigma)
+
         def u_theta(mino_time):
-            sigma = r(mino_time)**2 + self.a**2*cos(theta(mino_time))**2
-            return (-theta(mino_time+2*dx)+8*theta(mino_time+dx)-8*theta(mino_time-dx)+theta(mino_time-2*dx))/(12*dx*sigma)
+            sigma = r(mino_time) ** 2 + self.a**2 * cos(theta(mino_time)) ** 2
+            return (
+                -theta(mino_time + 2 * dx)
+                + 8 * theta(mino_time + dx)
+                - 8 * theta(mino_time - dx)
+                + theta(mino_time - 2 * dx)
+            ) / (12 * dx * sigma)
+
         def u_phi(mino_time):
-            sigma = r(mino_time)**2 + self.a**2*cos(theta(mino_time))**2
-            return (-phi(mino_time+2*dx)+8*phi(mino_time+dx)-8*phi(mino_time-dx)+phi(mino_time-2*dx))/(12*dx*sigma)
-        return u_t, u_r, u_theta, u_phi
+            sigma = r(mino_time) ** 2 + self.a**2 * cos(theta(mino_time)) ** 2
+            return (
+                -phi(mino_time + 2 * dx)
+                + 8 * phi(mino_time + dx)
+                - 8 * phi(mino_time - dx)
+                + phi(mino_time - 2 * dx)
+            ) / (12 * dx * sigma)
 
-    def plot(self,lambda0=0, lambda1=10, elevation=30 ,azimuth=-60, initial_phases=None, grid=True, axes=True, lw=1,color="red",tau=np.inf,point_density=200):
-        r"""
-        Creates a plot of the orbit
-
-        :param lambda0: starting mino time
-        :type lambda0: double, optional
-        :param lambda1: ending mino time
-        :type lambda1: double, optional
-        :param elevation: camera elevation angle in degrees, defaults to 30
-        :type elevation: double, optional
-        :param azimuth: camera azimuthal angle in degrees, defaults to -60
-        :type azimuth: double, optional
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
-        :param grid: if true, grid lines are shown on plot
-        :type grid: bool, optional
-        :param axes: if true, axes are shown on plot
-        :type axes: bool, optional
-        :param lw: linewidth of the orbital trajectory, defaults to 1
-        :type lw: double, optional
-        :param color: color of the orbital trajectory, defaults to "red"
-        :type color: str, optional
-        :param tau: time constant for the exponential decay of the linewidth, defaults to infinity
-        :type tau: double, optional
-        :param point_density: number of points to plot per unit of mino time, defaults to 200
-        :type point_density: int, optional
+        return u_t, u_r, u_theta, u_phi
 
-        :return: matplotlib figure and axes
-        :rtype: matplotlib.figure.Figure, matplotlib.axes._subplots.AxesSubplot
+    def plot(
+        self,
+        lambda0=0,
+        lambda1=10,
+        elevation=30,
+        azimuth=-60,
+        initial_phases=None,
+        grid=True,
+        axes=True,
+        lw=1,
+        color="red",
+        tau=np.inf,
+        point_density=200,
+    ):
+        r"""Creates a plot of the orbit
+
+        Parameters
+        ----------
+        lambda0 : double, optional
+            starting mino time
+        lambda1 : double, optional
+            ending mino time
+        elevation : double, optional
+            camera elevation angle in degrees, defaults to 30
+        azimuth : double, optional
+            camera azimuthal angle in degrees, defaults to -60
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+        grid : bool, optional
+            if true, grid lines are shown on plot
+        axes : bool, optional
+            if true, axes are shown on plot
+        lw : double, optional
+            linewidth of the orbital trajectory, defaults to 1
+        color : str, optional
+            color of the orbital trajectory, defaults to "red"
+        tau : double, optional
+            time constant for the exponential decay of the linewidth,
+            defaults to infinity
+        point_density : int, optional
+            number of points to plot per unit of mino time, defaults to
+            200
+
+        Returns
+        -------
+        matplotlib.figure.Figure, matplotlib.axes._subplots.AxesSubplot
+            matplotlib figure and axes
         """
-        if initial_phases is None: initial_phases = self.initial_phases
+        if initial_phases is None:
+            initial_phases = self.initial_phases
         lambda_range = lambda1 - lambda0
-        num_pts = int(lambda_range*point_density)
-        time = np.linspace(lambda0,lambda1,num_pts)
+        num_pts = int(lambda_range * point_density)
+        time = np.linspace(lambda0, lambda1, num_pts)
 
         t, r, theta, phi = self.trajectory(initial_phases=initial_phases)
 
         # compute trajectory in cartesian coordinates
-        trajectory_x = r(time)*sin(theta(time))*cos(phi(time))
-        trajectory_y = r(time)*sin(theta(time))*sin(phi(time))
-        trajectory_z = r(time)*cos(theta(time))
-        trajectory = np.column_stack((trajectory_x,trajectory_y,trajectory_z))
+        trajectory_x = r(time) * sin(theta(time)) * cos(phi(time))
+        trajectory_y = r(time) * sin(theta(time)) * sin(phi(time))
+        trajectory_z = r(time) * cos(theta(time))
+        trajectory = np.column_stack((trajectory_x, trajectory_y, trajectory_z))
 
         # create sphere with radius equal to event horizon radius
-        event_horizon = 1+sqrt(1-self.a**2)
+        event_horizon = 1 + sqrt(1 - self.a**2)
         u = np.linspace(0, 2 * np.pi, 50)
         v = np.linspace(0, np.pi, 25)
         x_sphere = event_horizon * np.outer(np.cos(u), np.sin(v))
         y_sphere = event_horizon * np.outer(np.sin(u), np.sin(v))
         z_sphere = event_horizon * np.outer(np.ones(np.size(u)), np.cos(v))
 
         # replace z values for points behind the black hole with nan so they are not plotted
         # https://matplotlib.org/stable/gallery/lines_bars_and_markers/masked_demo.html
-        visible = self.is_visible(trajectory,elevation,azimuth)
+        visible = self.is_visible(trajectory, elevation, azimuth)
         trajectory_z_visible = trajectory_z.copy()
         trajectory_z_visible[~visible] = np.nan
 
         # compute linewidths using exponential decay
-        decay = np.flip(0.1+lw*np.exp(-(time-time[0])/tau))
+        decay = np.flip(0.1 + lw * np.exp(-(time - time[0]) / tau))
 
         # https://stackoverflow.com/questions/19390895/matplotlib-plot-with-variable-line-width
-        points = np.array([[[x, y, z]] for x, y, z in zip(trajectory_x,trajectory_y,trajectory_z_visible)])
+        points = np.array(
+            [
+                [[x, y, z]]
+                for x, y, z in zip(trajectory_x, trajectory_y, trajectory_z_visible)
+            ]
+        )
         # create a segment connecting every pair of consecutive points
         segments = np.concatenate([points[:-1], points[1:]], axis=1)
         tail = Line3DCollection(segments, linewidth=decay, color=color)
 
         fig = plt.figure()
-        ax = fig.add_subplot(projection='3d')
-        
+        ax = fig.add_subplot(projection="3d")
+
         # plot black hole
-        ax.plot_surface(x_sphere, y_sphere, z_sphere, color='black')
+        ax.plot_surface(x_sphere, y_sphere, z_sphere, color="black")
         # plot orbit
         ax.add_collection(tail)
         # plot smaller body
-        ax.scatter(trajectory_x[-1],trajectory_y[-1],trajectory_z[-1],color="black",s=20)
+        ax.scatter(
+            trajectory_x[-1], trajectory_y[-1], trajectory_z[-1], color="black", s=20
+        )
 
         # set axis limits
-        x_values = np.concatenate((trajectory_x,x_sphere.flatten()))
-        y_values = np.concatenate((trajectory_y,y_sphere.flatten()))
-        z_values = np.concatenate((trajectory_z,z_sphere.flatten()))
-        ax.set_xlim([x_values.min(),x_values.max()])
-        ax.set_ylim([y_values.min(),y_values.max()])
-        ax.set_zlim([z_values.min(),z_values.max()])
+        x_values = np.concatenate((trajectory_x, x_sphere.flatten()))
+        y_values = np.concatenate((trajectory_y, y_sphere.flatten()))
+        z_values = np.concatenate((trajectory_z, z_sphere.flatten()))
+        ax.set_xlim([x_values.min(), x_values.max()])
+        ax.set_ylim([y_values.min(), y_values.max()])
+        ax.set_zlim([z_values.min(), z_values.max()])
         # set viewing angle
-        ax.view_init(elevation,azimuth)
+        ax.view_init(elevation, azimuth)
         # set equal aspect ratio and orthogonal projection
         ax.set_aspect("equal")
         # https://matplotlib.org/stable/gallery/mplot3d/projections.html
-        ax.set_proj_type('ortho')
+        ax.set_proj_type("ortho")
 
         # turn off grid and axes if specified
-        if not grid: ax.grid(False)
-        if not axes: ax.axis("off")
+        if not grid:
+            ax.grid(False)
+        if not axes:
+            ax.axis("off")
 
         return fig, ax
-    
-    def is_visible(self,points,elevation,azimuth):
-        """
-        Determines if a point is visible from a given viewing angle or obscured by the black hole. 
-        Viewing angles are defined as in https://matplotlib.org/stable/api/toolkits/mplot3d/view_angles.html and black hole is centered at the origin.
 
-        :param points: list of points given in cartesian coordinates
-        :type points: array_like
-        :param elevation: camera elevation angle in degrees
-        :type elevation: double
-        :param azimuth: camera azimuthal angle in degrees
-        :type azimuth: double
-
-        :return: boolean array indicating whether each point is visible
-        :rtype: np.array
+    def is_visible(self, points, elevation, azimuth):
+        """Determines if a point is visible from a given viewing angle or obscured
+        by the black hole. Viewing angles are defined as in
+        https://matplotlib.org/stable/api/toolkits/mplot3d/view_angles.html and
+        black hole is centered at the origin.
+
+        Parameters
+        ----------
+        points : array_like
+            list of points given in cartesian coordinates
+        elevation : double
+            camera elevation angle in degrees
+        azimuth : double
+            camera azimuthal angle in degrees
+
+        Returns
+        -------
+        np.array
+            boolean array indicating whether each point is visible
         """
         # compute event horizon radius
-        event_horizon = 1+sqrt(1-self.a**2)
+        event_horizon = 1 + sqrt(1 - self.a**2)
 
         # convert viewing angles to radians
-        elevation_rad = elevation*pi/180
-        azimuth_rad = azimuth*pi/180
+        elevation_rad = elevation * pi / 180
+        azimuth_rad = azimuth * pi / 180
 
         # https://matplotlib.org/stable/api/toolkits/mplot3d/view_angles.html
-        view_plane_normal = [cos(elevation_rad)*cos(azimuth_rad),cos(elevation_rad)*sin(azimuth_rad),sin(elevation_rad)]
+        view_plane_normal = [
+            cos(elevation_rad) * cos(azimuth_rad),
+            cos(elevation_rad) * sin(azimuth_rad),
+            sin(elevation_rad),
+        ]
 
         normal_component = points.dot(view_plane_normal)
         # compute the projection of each trajectory point onto the viewing plane
-        projection = points-np.transpose(normal_component*np.transpose(np.broadcast_to(view_plane_normal,(len(points),3))))
+        projection = points - np.transpose(
+            normal_component
+            * np.transpose(np.broadcast_to(view_plane_normal, (len(points), 3)))
+        )
         # find points in front of the viewing plane or outside the event horizon when projected onto the viewing plane
-        return ((normal_component >= 0) | (np.linalg.norm(projection,axis=1) > event_horizon)) & (np.linalg.norm(points) > event_horizon)
-    
-    def animate(self,filename,lambda0=0, lambda1=10, elevation=30 ,azimuth=-60, initial_phases=None, grid=True, axes=True, color="red", tau=2, tail_length=5, 
-                lw=2, azimuthal_pan=None, elevation_pan=None, roll=None, speed=1, background_color=None, axis_limit=None, plot_components=False):
-        r"""
-        Saves an animation of the orbit as an mp4 file. 
-        Note that this function requires ffmpeg to be installed and may take several minutes to run depending on the length of the animation.
-
-        :param filename: filename to save the animation to
-        :type filename: str
-        :param lambda0: starting mino time, defaults to 0
-        :type lambda0: double, optional
-        :param lambda1: ending mino time, defaults to 10
-        :type lambda1: double, optional
-        :param elevation: camera elevation angle in degrees, defaults to 30
-        :type elevation: double, optional
-        :param azimuth: camera azimuthal angle in degrees, defaults to -60
-        :type azimuth: double, optional
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
-        :param grid: sets visibility of the grid, defaults to True
-        :type grid: bool, optional
-        :param axes: sets visibility of axes, defaults to True
-        :type axes: bool, optional
-        :param color: color of the orbital tail, defaults to "red"
-        :type color: str, optional
-        :param tau: time constant for the exponential decay in the opacity of the tail, defaults to 2
-        :type tau: double, optional
-        :param tail_length: length of the tail in units of mino time, defaults to 5
-        :type tail_length: double, optional
-        :param lw: linewidth of the orbital trajectory, defaults to 2
-        :type lw: double, optional
-        :param azimuthal_pan: function defining the azimuthal angle of the camera in degrees as a function of mino time, defaults to None
-        :type azimuthal_pan: function, optional
-        :param elevation_pan: function defining the elevation angle of the camera in degrees as a function of mino time, defaults to None
-        :type elevation_pan: function, optional
-        :param roll: function defining the roll angle of the camera in degrees as a function of mino time, defaults to None
-        :type roll: function, optional
-        :param axis_limit: sets the axis limit as a function of mino time, defaults to None
-        :type axis_limit: function, optional
-        :param speed: playback speed of the animation in units of mino time per second (must be a multiple of 1/8), defaults to 1
-        :type speed: double, optional
-        :param background_color: color of the background, defaults to None
-        :type background_color: str, optional
-        :param plot_components: if true, plots the components of the trajectory in addition to the trajectory itself, defaults to False
-        :type plot_components: bool, optional
+        return (
+            (normal_component >= 0)
+            | (np.linalg.norm(projection, axis=1) > event_horizon)
+        ) & (np.linalg.norm(points) > event_horizon)
+
+    def animate(
+        self,
+        filename,
+        lambda0=0,
+        lambda1=10,
+        elevation=30,
+        azimuth=-60,
+        initial_phases=None,
+        grid=True,
+        axes=True,
+        color="red",
+        tau=2,
+        tail_length=5,
+        lw=2,
+        azimuthal_pan=None,
+        elevation_pan=None,
+        roll=None,
+        speed=1,
+        background_color=None,
+        axis_limit=None,
+        plot_components=False,
+    ):
+        r"""Saves an animation of the orbit as an mp4 file.
+        Note that this function requires ffmpeg to be installed and may take several
+        minutes to run depending on the length of the animation.
+
+        Parameters
+        ----------
+        filename : str
+            filename to save the animation to
+        lambda0 : double, optional
+            starting mino time, defaults to 0
+        lambda1 : double, optional
+            ending mino time, defaults to 10
+        elevation : double, optional
+            camera elevation angle in degrees, defaults to 30
+        azimuth : double, optional
+            camera azimuthal angle in degrees, defaults to -60
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+        grid : bool, optional
+            sets visibility of the grid, defaults to True
+        axes : bool, optional
+            sets visibility of axes, defaults to True
+        color : str, optional
+            color of the orbital tail, defaults to "red"
+        tau : double, optional
+            time constant for the exponential decay in the opacity of
+            the tail, defaults to 2
+        tail_length : double, optional
+            length of the tail in units of mino time, defaults to 5
+        lw : double, optional
+            linewidth of the orbital trajectory, defaults to 2
+        azimuthal_pan : function, optional
+            function defining the azimuthal angle of the camera in
+            degrees as a function of mino time, defaults to None
+        elevation_pan : function, optional
+            function defining the elevation angle of the camera in
+            degrees as a function of mino time, defaults to None
+        roll : function, optional
+            function defining the roll angle of the camera in degrees as
+            a function of mino time, defaults to None
+        axis_limit : function, optional
+            sets the axis limit as a function of mino time, defaults to
+            None
+        speed : double, optional
+            playback speed of the animation in units of mino time per
+            second (must be a multiple of 1/8), defaults to 1
+        background_color : str, optional
+            color of the background, defaults to None
+        plot_components : bool, optional
+            if true, plots the components of the trajectory in addition
+            to the trajectory itself, defaults to False
         """
         lambda_range = lambda1 - lambda0
-        point_density = 240 # number of points per unit of mino time
-        num_pts = int(lambda_range*point_density) # total number of points
-        time = np.linspace(lambda0,lambda1,num_pts)
-        speed_multiplier = int(speed*8)
-        num_frames = int(num_pts/speed_multiplier)
+        point_density = 240  # number of points per unit of mino time
+        num_pts = int(lambda_range * point_density)  # total number of points
+        time = np.linspace(lambda0, lambda1, num_pts)
+        speed_multiplier = int(speed * 8)
+        num_frames = int(num_pts / speed_multiplier)
         # compute trajectory
         t, r, theta, phi = self.trajectory(initial_phases)
 
-        fig = plt.figure(figsize=((18,12) if plot_components else (12,12)))
+        fig = plt.figure(figsize=((18, 12) if plot_components else (12, 12)))
         if plot_components:
             ax_dict = fig.subplot_mosaic(
-            """
+                """
             OOOOTT
             OOOORR
             OOOOΘΘ
             OOOOΦΦ
             """,
-            per_subplot_kw={"O":{"projection":"3d"},"T":{"facecolor":"none"},"R":{"facecolor":"none"},"Θ":{"facecolor":"none"},"Φ":{"facecolor":"none"}}
+                per_subplot_kw={
+                    "O": {"projection": "3d"},
+                    "T": {"facecolor": "none"},
+                    "R": {"facecolor": "none"},
+                    "Θ": {"facecolor": "none"},
+                    "Φ": {"facecolor": "none"},
+                },
             )
             ax = ax_dict["O"]
 
             ax_dict["T"].set_ylabel("$t$")
             ax_dict["R"].set_ylabel("$r$")
             ax_dict["Θ"].set_ylabel(r"$\theta$")
             ax_dict["Φ"].set_ylabel(r"$\phi$")
-            t_plot, = ax_dict["T"].plot(time,t(time))
-            r_plot, = ax_dict["R"].plot(time,r(time))
-            theta_plot, = ax_dict["Θ"].plot(time,theta(time))
-            phi_plot, = ax_dict["Φ"].plot(time,phi(time))
+            (t_plot,) = ax_dict["T"].plot(time, t(time))
+            (r_plot,) = ax_dict["R"].plot(time, r(time))
+            (theta_plot,) = ax_dict["Θ"].plot(time, theta(time))
+            (phi_plot,) = ax_dict["Φ"].plot(time, phi(time))
             # add text with parameters and time
-            text = ax.text2D(0.05, 0.95, "", transform=ax.transAxes, fontsize=20, bbox=dict(facecolor='none', pad=10.0))
-        
+            text = ax.text2D(
+                0.05,
+                0.95,
+                "",
+                transform=ax.transAxes,
+                fontsize=20,
+                bbox=dict(facecolor="none", pad=10.0),
+            )
+
         else:
-            ax = fig.add_subplot(projection='3d')
+            ax = fig.add_subplot(projection="3d")
 
-        eh = 1+sqrt(1-self.a**2) # event horizon radius
+        eh = 1 + sqrt(1 - self.a**2)  # event horizon radius
 
         # compute trajectory in cartesian coordinates
-        trajectory_x = r(time)*sin(theta(time))*cos(phi(time))
-        trajectory_y = r(time)*sin(theta(time))*sin(phi(time))
-        trajectory_z = r(time)*cos(theta(time))
-        trajectory = np.column_stack((trajectory_x,trajectory_y,trajectory_z))
+        trajectory_x = r(time) * sin(theta(time)) * cos(phi(time))
+        trajectory_y = r(time) * sin(theta(time)) * sin(phi(time))
+        trajectory_z = r(time) * cos(theta(time))
+        trajectory = np.column_stack((trajectory_x, trajectory_y, trajectory_z))
 
         # create sphere with radius equal to event horizon radius
         u = np.linspace(0, 2 * np.pi, 50)
         v = np.linspace(0, np.pi, 25)
         x_sphere = eh * np.outer(np.cos(u), np.sin(v))
         y_sphere = eh * np.outer(np.sin(u), np.sin(v))
         z_sphere = eh * np.outer(np.ones(np.size(u)), np.cos(v))
 
         # plot black hole
         black_hole_color = "#333" if background_color == "black" else "black"
-        ax.plot_surface(x_sphere, y_sphere, z_sphere, color=black_hole_color,shade=(background_color == "black"), zorder=0)
+        ax.plot_surface(
+            x_sphere,
+            y_sphere,
+            z_sphere,
+            color=black_hole_color,
+            shade=(background_color == "black"),
+            zorder=0,
+        )
         # create orbital tail
-        decay = np.flip(0.1+0.9*np.exp(-(time-time[0])/tau)) # exponential decay
+        decay = np.flip(
+            0.1 + 0.9 * np.exp(-(time - time[0]) / tau)
+        )  # exponential decay
         tail = Line3DCollection([], color=color, linewidths=lw, zorder=1)
         ax.add_collection(tail)
         # plot smaller body
-        body = ax.scatter([],[],[],c="black")
+        body = ax.scatter([], [], [], c="black")
 
         # set axis limits so that the black hole is centered
-        x_values = np.concatenate((trajectory_x,x_sphere.flatten()))
-        y_values = np.concatenate((trajectory_y,y_sphere.flatten()))
-        z_values = np.concatenate((trajectory_z,z_sphere.flatten()))
-        limit = abs(max(x_values.min(),y_values.min(),z_values.min(),x_values.max(),y_values.max(),z_values.max(),key=abs))
-        ax.set_xlim(-limit,limit)
-        ax.set_ylim(-limit,limit)
-        ax.set_zlim(-limit,limit)
+        x_values = np.concatenate((trajectory_x, x_sphere.flatten()))
+        y_values = np.concatenate((trajectory_y, y_sphere.flatten()))
+        z_values = np.concatenate((trajectory_z, z_sphere.flatten()))
+        limit = abs(
+            max(
+                x_values.min(),
+                y_values.min(),
+                z_values.min(),
+                x_values.max(),
+                y_values.max(),
+                z_values.max(),
+                key=abs,
+            )
+        )
+        ax.set_xlim(-limit, limit)
+        ax.set_ylim(-limit, limit)
+        ax.set_zlim(-limit, limit)
         # set equal aspect ratio and orthogonal projection
         ax.set_aspect("equal")
         # https://matplotlib.org/stable/gallery/mplot3d/projections.html
-        ax.set_proj_type('ortho')
+        ax.set_proj_type("ortho")
 
         # turn off grid and axes if specified
-        if not grid: ax.grid(False)
-        if not axes: ax.axis("off")
+        if not grid:
+            ax.grid(False)
+        if not axes:
+            ax.axis("off")
 
         # remove margins
         fig.tight_layout()
-            
+
         # set background color if specified
-        if background_color is not None: 
+        if background_color is not None:
             fig.set_facecolor(background_color)
             ax.set_facecolor(background_color)
             # make the panes transparent so that the background color shows through the grid
             ax.xaxis.pane.fill = False
             ax.yaxis.pane.fill = False
             ax.zaxis.pane.fill = False
 
         # start progress bar
-        with tqdm(total=num_frames,ncols=80) as pbar:
-            def draw_frame(i,body,tail):
+        with tqdm(total=num_frames, ncols=80) as pbar:
+
+            def draw_frame(i, body, tail):
                 # update progress bar
                 pbar.update(1)
 
-                j = speed_multiplier*i
-                j0 = max(0,j-tail_length*point_density)
+                j = speed_multiplier * i
+                j0 = max(0, j - tail_length * point_density)
                 current_time = time[j]
 
                 # update camera angles
-                updated_azimuth = azimuthal_pan(current_time) if azimuthal_pan is not None else azimuth
-                updated_elevation = elevation_pan(current_time) if elevation_pan is not None else elevation
+                updated_azimuth = (
+                    azimuthal_pan(current_time)
+                    if azimuthal_pan is not None
+                    else azimuth
+                )
+                updated_elevation = (
+                    elevation_pan(current_time)
+                    if elevation_pan is not None
+                    else elevation
+                )
                 updated_roll = roll(current_time) if roll is not None else 0
-                ax.view_init(updated_elevation,updated_azimuth,updated_roll)
+                ax.view_init(updated_elevation, updated_azimuth, updated_roll)
 
                 # update axis limits
                 if axis_limit is not None:
                     updated_limit = axis_limit(current_time)
-                    ax.set_xlim(-updated_limit,updated_limit)
-                    ax.set_ylim(-updated_limit,updated_limit)
-                    ax.set_zlim(-updated_limit,updated_limit)
+                    ax.set_xlim(-updated_limit, updated_limit)
+                    ax.set_ylim(-updated_limit, updated_limit)
+                    ax.set_zlim(-updated_limit, updated_limit)
 
                 # filter out points behind the black hole
-                visible = self.is_visible(trajectory[j0:j],updated_elevation,updated_azimuth)
+                visible = self.is_visible(
+                    trajectory[j0:j], updated_elevation, updated_azimuth
+                )
                 trajectory_z_visible = trajectory_z[j0:j].copy()
                 trajectory_z_visible[~visible] = np.nan
                 # create segments connecting every consecutive pair of points
-                points = np.array([[[x, y, z]] for x, y, z in zip(trajectory_x[j0:j],trajectory_y[j0:j],trajectory_z_visible)])
-                segments = np.concatenate([points[:-1], points[1:]], axis=1) if len(points) > 1 else []
+                points = np.array(
+                    [
+                        [[x, y, z]]
+                        for x, y, z in zip(
+                            trajectory_x[j0:j], trajectory_y[j0:j], trajectory_z_visible
+                        )
+                    ]
+                )
+                segments = (
+                    np.concatenate([points[:-1], points[1:]], axis=1)
+                    if len(points) > 1
+                    else []
+                )
                 # update tail
                 tail.set_segments(segments)
-                tail.set_alpha(decay[-(j-j0):])
+                tail.set_alpha(decay[-(j - j0) :])
                 # update body
-                body._offsets3d = ([trajectory_x[j]],[trajectory_y[j]],[trajectory_z[j]])
+                body._offsets3d = (
+                    [trajectory_x[j]],
+                    [trajectory_y[j]],
+                    [trajectory_z[j]],
+                )
 
                 # update plots
                 if plot_components:
-                    t_plot.set_data(time[:j],t(time[:j]))
-                    r_plot.set_data(time[:j],r(time[:j]))
-                    theta_plot.set_data(time[:j],theta(time[:j]))
-                    phi_plot.set_data(time[:j],phi(time[:j]))
+                    t_plot.set_data(time[:j], t(time[:j]))
+                    r_plot.set_data(time[:j], r(time[:j]))
+                    theta_plot.set_data(time[:j], theta(time[:j]))
+                    phi_plot.set_data(time[:j], phi(time[:j]))
                     # set text
                     if self.stable:
-                        text.set_text(f"$a = {self.a}\quad p = {self.p}\quad e = {self.e}\quad x = {self.x:.3f}\quad \lambda = {current_time:.2f}$")
+                        text.set_text(
+                            f"$a = {self.a}\quad p = {self.p}\quad e = {self.e}\quad x = {self.x:.3f}\quad \lambda = {current_time:.2f}$"
+                        )
                     else:
-                        text.set_text(f"$a = {self.a}\quad E = {self.E:.3f}\quad L = {self.L:.3f}\quad Q = {self.Q:.3f}\quad \lambda = {current_time:.2f}$")
-                                
+                        text.set_text(
+                            f"$a = {self.a}\quad E = {self.E:.3f}\quad L = {self.L:.3f}\quad Q = {self.Q:.3f}\quad \lambda = {current_time:.2f}$"
+                        )
+
             # save to file
-            ani = FuncAnimation(fig,draw_frame,num_frames,fargs=(body,tail))
+            ani = FuncAnimation(fig, draw_frame, num_frames, fargs=(body, tail))
             FFwriter = FFMpegWriter(fps=30)
             # savefig overrides the facecolor so we need to set it again
             if background_color is not None:
-                ani.save(filename,savefig_kwargs={"facecolor":background_color}, writer = FFwriter)
+                ani.save(
+                    filename,
+                    savefig_kwargs={"facecolor": background_color},
+                    writer=FFwriter,
+                )
             else:
-                ani.save(filename, writer = FFwriter)
+                ani.save(filename, writer=FFwriter)
             # close figure so it doesn't show up in notebook
-            plt.close(fig)
+            plt.close(fig)
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy/plunge.py` & `kerrgeopy-0.9.2/kerrgeopy/stable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,440 +1,559 @@
-"""
-Module implementing the plunging orbit solutions of `Dyson and van de Meent <https://doi.org/10.48550/arXiv.2302.03704>`_
-"""
-from numpy import sqrt, arctan, arctan2, arccos, log, pi
-from numpy.polynomial import Polynomial
-import numpy as np
-from scipy.special import ellipj, ellipeinc, ellipk
-from .frequencies import _mino_frequencies_from_constants, _ellippiinc
-from .stable import *
+"""Module implementing the stable bound orbit solutions of `Fujita and Hikida <https://doi.org/10.48550/arXiv.0906.1420>`_"""
+from .constants import *
+from .constants import _standardize_params
+from .frequencies import _ellippi, _ellippiinc, _ellipeinc
+from .frequencies import *
+from scipy.special import ellipj
 from .orbit import Orbit
-from .units import *
+from numpy import pi, arccos
 
-class PlungingOrbit(Orbit):
-    r"""
-    Class representing a plunging orbit in Kerr spacetime.
-
-    :param a: dimensionaless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
-    :param initial_phases: tuple of initial phases :math:`(q^t_0, q^r_0, q^\theta_0, q^\phi_0)`, defaults to (0,0,0,0)
-    :type initial_phases: tuple, optional
-    :param M: mass of the primary in solar masses, optional
-    :type M: double
-    :param mu: mass of the smaller body in solar masses, optional
-    :type mu: double
-
-    :ivar a: dimensionaless spin parameter
-    :ivar E: dimensionless energy
-    :ivar L: dimensionless angular momentum
-    :ivar Q: dimensionless Carter constant
-    :ivar initial_phases: tuple of initial phases :math:`(q^t_0, q^r_0, q^\theta_0, q^\phi_0)`
-    :ivar stable: boolean indicating whether the orbit is stable
-    :ivar initial_position: tuple of initial position coordinates :math:`(t_0, r_0, \theta_0, \phi_0)`
-    :ivar initial_velocity: tuple of initial four-velocity components :math:`(u^t_0, u^r_0, u^\theta_0, u^\phi_0)`
-    :ivar M: mass of the primary in solar masses
-    :ivar mu: mass of the smaller body in solar masses
-    :ivar upsilon_r: radial Mino frequency
-    :ivar upsilon_theta: polar Mino frequency
+
+class StableOrbit(Orbit):
+    r"""Class representing a stable bound orbit in Kerr spacetime.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless angular momentum
+    p : double
+        semi-latus rectum
+    e : double
+        orbital eccentricity
+    x : double
+        cosine of the orbital inclination
+    initial_phases : tuple, optional
+        tuple of initial phases
+        :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`, defaults to (0,0,0,0)
+    M : double
+        mass of the primary in solar masses, optional
+    mu : double
+        mass of the smaller body in solar masses, optional
+
+    Attributes
+    ----------
+    a
+        dimensionless angular momentum
+    p
+        semi-latus rectum
+    e
+        orbital eccentricity
+    x
+        cosine of the orbital inclination
+    M
+        mass of the primary in solar masses
+    mu
+        mass of the smaller body in solar masses
+    E
+        dimensionless energy
+    L
+        dimensionless angular momentum
+    Q
+        dimensionless carter constant
+    initial_phases
+        tuple of initial phases
+        :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+    stable
+        boolean indicating whether the orbit is stable
+    initial_position
+        tuple of initial position coordinates :math:`(t_0, r_0, \theta_0, \phi_0)`
+    initial_velocity
+        tuple of initial four-velocity components :math:`(u^t_0, u^r_0, u^\theta_0, u^\phi_0)`
+    upsilon_r
+        dimensionless radial orbital frequency in Mino time
+    upsilon_theta
+        dimensionless polar orbital frequency in Mino time
+    upsilon_phi
+        dimensionless azimuthal orbital frequency in Mino time
+    gamma
+        dimensionless time dilation factor
+    omega_r
+        dimensionless radial orbital frequency in Boyer-Lindquist time
+    omega_theta
+        dimensionless polar orbital frequency in Boyer-Lindquist time
+    omega_phi
+        dimensionless azimuthal orbital frequency in Boyer-Lindquist
+        time
     """
-    def __init__(self,a,E,L,Q,initial_phases=(0,0,0,0),M=None,mu=None):
-        self.a, self.E, self.L, self.Q, self.initial_phases, self.M, self.mu = a, E, L, Q, initial_phases, M, mu
 
-        if a == 0: raise ValueError("Schwarzschild plunges are not currently supported")
+    def __init__(self, a, p, e, x, initial_phases=(0, 0, 0, 0), M=None, mu=None):
+        a, x = _standardize_params(a, x)
+        self.a, self.p, self.e, self.x, self.initial_phases, self.M, self.mu = (
+            a,
+            p,
+            e,
+            x,
+            initial_phases,
+            M,
+            mu,
+        )
+        constants = constants_of_motion(a, p, e, x)
+
+        self.E, self.L, self.Q = constants
+        self.upsilon_r, self.upsilon_theta, self.upsilon_phi, self.gamma = mino_frequencies(
+            a, p, e, x
+        )
+        self.omega_r, self.omega_theta, self.omega_phi = fundamental_frequencies(a, p, e, x)
+        self.stable = True
 
-        self.stable = False
-        self.upsilon_r, self.upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
-        
         u_t, u_r, u_theta, u_phi = self.four_velocity()
         t, r, theta, phi = self.trajectory()
         self.initial_position = t(0), r(0), theta(0), phi(0)
         self.initial_velocity = u_t(0), u_r(0), u_theta(0), u_phi(0)
-    
-    def trajectory_deltas(self,initial_phases=None):
-        r"""
-        Computes the trajectory deltas :math:`t_r(q_r)`, :math:`t_\theta(q_\theta)`, :math:`\phi_r(q_r)` and :math:`\phi_\theta(q_\theta)`
 
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
-
-        :return: tuple of trajectory deltas :math:`(t_r(q_r), t_\theta(q_\theta), \phi_r(q_r),\phi_\theta(q_\theta))`
-        :rtype: tuple(function, function, function, function)
+    @classmethod
+    def from_constants(cls, a, E, L, Q, initial_phases=(0, 0, 0, 0), M=None, mu=None):
+        """Alternative constructor method that takes the constants of motion as arguments.
+
+        Parameters
+        ----------
+        a : double
+            spin parameter
+        E : double
+            dimensionless energy
+        L : double
+            dimensionless angular momentum
+        Q : double
+            dimensionless Carter constant
+        M : double, optional
+            mass of the primary in solar masses
+        mu : double, optional
+            mass of the smaller body in solar masses
         """
-        if initial_phases is None: initial_phases = self.initial_phases
-        q_t0, q_r0, q_theta0, q_phi0 = initial_phases
+        a, p, e, x = apex_from_constants(a, E, L, Q)
 
-        radial_roots = plunging_radial_roots(self.a,self.E,self.L,self.Q)
-        if np.iscomplex(radial_roots[3]):
-            # adjust q_theta0 so that initial conditions are consistent with stable orbits
-            q_theta0 = q_theta0 + pi/2
-            r, t_r, phi_r = plunging_radial_solutions_complex(self.a,self.E,self.L,self.Q)
-            theta, t_theta, phi_theta = plunging_polar_solutions(self.a,self.E,self.L,self.Q)
-        else:
-            constants = (self.E,self.L,self.Q)
-            r, t_r, phi_r = radial_solutions(self.a,constants,radial_roots)
-            theta, t_theta, phi_theta = polar_solutions(self.a,constants,radial_roots)
-
-        return (lambda q_r: t_r(q_r+q_r0), lambda q_theta: t_theta(q_theta+q_theta0),
-                lambda q_r: phi_r(q_r+q_r0), lambda q_theta: phi_theta(q_theta+q_theta0))
-
-    def trajectory(self,initial_phases=None,distance_units="natural",time_units="natural"):
-        r"""
-        Computes the components of the trajectory as a function of mino time
-
-        :param initial_phases: tuple of initial phases :math:`(q^t_0, q^r_0, q^\theta_0, q^\phi_0)`
-        :type initial_phases: tuple, optional
-        :param distance_units: units to compute the radial component of the trajectory in (options are "natural", "mks", "cgs", "au" and "km"), defaults to "natural"
-        :type distance_units: str, optional
-        :param time_units: units to compute the time component of the trajectory in (options are "natural", "mks", "cgs", and "days"), defaults to "natural"
-        :type time_units: str, optional
-        
-        :return: tuple of functions :math:`t(\lambda), r(\lambda), \theta(\lambda), \phi(\lambda)`
-        :rtype: tuple(function,function,function,function)
+        return cls(a, p, e, x, initial_phases, M, mu)
+
+    def mino_frequencies(self, units="natural"):
+        r"""Computes orbital frequencies in Mino time. Returns dimensionless frequencies 
+        in geometrized units by default. M and mu must be defined in order to convert 
+        to physical units.
+
+        Parameters
+        ----------
+        units : str, optional
+            units to return the frequencies in (options are "natural",
+            "mks" and "cgs"), defaults to "natural"
+
+        Returns
+        -------
+        tuple(double, double, double, double)
+            tuple of orbital frequencies :math:`(\Upsilon_r,
+            \Upsilon_\theta, \Upsilon_\phi, \Gamma)`
         """
-        if initial_phases is None: initial_phases = self.initial_phases
-        return plunging_trajectory(self.a,self.E,self.L,self.Q,initial_phases,self.M,distance_units,time_units)
+        upsilon_r, upsilon_theta, upsilon_phi, gamma = (
+            self.upsilon_r,
+            self.upsilon_theta,
+            self.upsilon_phi,
+            self.gamma,
+        )
+        if units == "natural":
+            return upsilon_r, upsilon_theta, upsilon_phi, gamma
+
+        if self.M is None:
+            raise ValueError("M must be specified to convert frequencies to physical units")
+
+        if units == "mks" or units == "cgs":
+            return (
+                time_in_seconds(upsilon_r, self.M),
+                time_in_seconds(upsilon_theta, self.M),
+                time_in_seconds(upsilon_phi, self.M),
+                time2_in_seconds2(gamma, self.M),
+            )
 
-def plunging_radial_integrals(a,E,L,Q):
-    r"""
-    Computes the radial integrals :math:`I_r`, :math:`I_{r^2}` and :math:`I_{r_\pm}` defined in equation 39 of `Dyson and van de Meent <https://doi.org/10.48550/arXiv.2302.03704>`_ as a function of the radial phase.
-    Used to compute the radial solutions for the case of two complex roots.
-
-    :param a: dimensionless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
+        raise ValueError("units must be one of 'natural', 'mks', or 'cgs'")
 
-    :return: radial integrals :math:`(I_r,I_{r^2},I_{r_+},I_{r_-})`
-    :rtype: tuple(function,function,function,function)
-    """
-    r1, r2, r3, r4 = plunging_radial_roots(a,E,L,Q)
-    rho_r = np.real(r3)
-    rho_i = np.imag(r4)
-
-    # inner and outer horizons
-    r_plus = 1+sqrt(1-a**2)
-    r_minus = 1-sqrt(1-a**2)
-
-    # equation 42
-    A = sqrt((r2-rho_r)**2+rho_i**2)
-    B = sqrt((r1-rho_r)**2+rho_i**2)
-    f = 4*A*B/(A-B)**2
-    k_r = sqrt(((r2-r1)**2-(A-B)**2)/(4*A*B))
-
-    upsilon_r, upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
-
-    # equation 48
-    D_plus = sqrt(4*A*B*(r2-r_plus)*(r_plus-r1))/(A*(r_plus-r1)+B*(r2-r_plus))
-    D_minus = sqrt(4*A*B*(r2-r_minus)*(r_minus-r1))/(A*(r_minus-r1)+B*(r2-r_minus))
-
-    def I_r(q_r):
-        # equation 43
-        sn, cn, dn, xi_r = ellipj(2*ellipk(k_r**2)*q_r/pi,k_r**2)
-        mino_time = q_r/upsilon_r
-        # equation 46
-        return (A*r1-B*r2)/(A-B)*mino_time - 1/sqrt(1-E**2)*arctan((r2-r1)*sn/(2*sqrt(A*B)*dn)) \
-                + (A+B)*(r2-r1)/(2*(A-B)*sqrt(A*B*(1-E**2)))*_ellippiinc(xi_r,-1/f,k_r**2)
-    
-    def I_r2(q_r):
-        # equation 43
-        sn, cn, dn, xi_r = ellipj(2*ellipk(k_r**2)*q_r/pi,k_r**2)
-        mino_time = q_r/upsilon_r
-        # equation 47
-        return (A*r1**2-B*r2**2)/(A-B)*mino_time + sqrt(A*B)/sqrt(1-E**2)*ellipeinc(xi_r,k_r**2) \
-                - (A+B)*(A**2+2*r1**2-B**2-2*r2**2)/(4*(A-B)*sqrt((1-E**2)*A*B))*_ellippiinc(xi_r,-1/f,k_r**2) \
-                - sqrt(A*B)*(A+B-(A-B)*cn)*sn*dn/((A-B)*sqrt(1-E**2)*(f+sn**2)) \
-                + (A**2+2*r1**2-B**2-2*r2**2)/(4*(r2-r1)*sqrt(1-E**2))*arctan2(2*sn*dn*sqrt(f*(1+f*k_r**2)),f-(1+2*f*k_r**2)*sn**2)
-        
-    def I_r_plus(q_r):
-        # equation 43
-        sn, cn, dn, xi_r = ellipj(2*ellipk(k_r**2)*q_r/pi,k_r**2)
-        mino_time = q_r/upsilon_r
-        # equation 48
-        return (A-B)*mino_time/(A*(r1-r_plus)-B*(r2-r_plus)) \
-            + (r2-r1)*(A*(r1-r_plus)+B*(r2-r_plus))/(2*sqrt(A*B*(1-E**2))*(r_plus-r1)*(r2-r_plus)*(A*(r1-r_plus)-B*(r2-r_plus)))*_ellippiinc(xi_r,1/D_plus**2,k_r**2) \
-            - (sqrt(r2-r1)*log(
-                ((D_plus*sqrt(1-D_plus**2*k_r**2)+dn*sn)**2 + (k_r*(D_plus**2-sn**2))**2) /
-                ((D_plus*sqrt(1-D_plus**2*k_r**2)-dn*sn)**2 + (k_r*(D_plus**2-sn**2))**2)
-                )  /
-                (4*sqrt((1-E**2)*(r2-r_plus)*(r_plus-r1))*sqrt(A**2*(r_plus-r1)-(r2-r_plus)*(r1**2-B**2+r2*r_plus-r1*(r2+r_plus))))
+    def fundamental_frequencies(self, units="natural"):
+        r"""Computes orbital frequencies in Boyer-Lindquist time. Returns dimensionless 
+        frequencies in geometrized units by default. M and mu must be defined in order 
+        to convert to physical units.
+
+        Parameters
+        ----------
+        units : str, optional
+            units to return the frequencies in (options are "natural",
+            "mks", "cgs" and "mHz"), defaults to "natural"
+
+        Returns
+        -------
+        tuple(double, double, double)
+            tuple of orbital frequencies :math:`(\Omega_r, \Omega_\theta, \Omega_\phi)`
+        """
+        upsilon_r, upsilon_theta, upsilon_phi, gamma = (
+            self.upsilon_r,
+            self.upsilon_theta,
+            self.upsilon_phi,
+            self.gamma,
+        )
+        if units == "natural":
+            return upsilon_r / gamma, upsilon_theta / gamma, upsilon_phi / gamma
+
+        if self.M is None:
+            raise ValueError("M must be specified to convert frequencies to physical units")
+
+        if units == "mks" or units == "cgs":
+            return (
+                frequency_in_Hz(upsilon_r / gamma, self.M),
+                frequency_in_Hz(upsilon_theta / gamma, self.M),
+                frequency_in_Hz(upsilon_phi / gamma, self.M),
             )
-    
-    def I_r_minus(q_r):
-        # equation 43
-        sn, cn, dn, xi_r = ellipj(2*ellipk(k_r**2)*q_r/pi,k_r**2)
-        mino_time = q_r/upsilon_r
-        # equation 48
-        return (A-B)*mino_time/(A*(r1-r_minus)-B*(r2-r_minus)) \
-            + (r2-r1)*(A*(r1-r_minus)+B*(r2-r_minus))/(2*sqrt(A*B*(1-E**2))*(r_minus-r1)*(r2-r_minus)*(A*(r1-r_minus)-B*(r2-r_minus)))*_ellippiinc(xi_r,1/D_minus**2,k_r**2) \
-            - (sqrt(r2-r1)*log(
-                ((D_minus*sqrt(1-D_minus**2*k_r**2)+dn*sn)**2 + (k_r*(D_minus**2-sn**2))**2) /
-                ((D_minus*sqrt(1-D_minus**2*k_r**2)-dn*sn)**2 + (k_r*(D_minus**2-sn**2))**2)
-                )  /
-                (4*sqrt((1-E**2)*(r2-r_minus)*(r_minus-r1))*sqrt(A**2*(r_minus-r1)-(r2-r_minus)*(r1**2-B**2+r2*r_minus-r1*(r2+r_minus))))
+        if units == "mHz":
+            return (
+                frequency_in_mHz(upsilon_r / gamma, self.M),
+                frequency_in_mHz(upsilon_theta / gamma, self.M),
+                frequency_in_mHz(upsilon_phi / gamma, self.M),
             )
 
-    return I_r, I_r2, I_r_plus, I_r_minus
+        raise ValueError("units must be one of 'natural', 'mks', 'cgs', or 'mHz'")
+
+    def trajectory_deltas(self, initial_phases=None):
+        r"""Computes the trajectory deltas :math:`t_r(q_r)`, :math:`t_\theta(q_\theta)`, 
+        :math:`\phi_r(q_r)` and :math:`\phi_\theta(q_\theta)`
+
+        Parameters
+        ----------
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+
+        Returns
+        -------
+        tuple(function, function, function, function)
+            tuple of trajectory deltas :math:`(t_r(q_r),
+            t_\theta(q_\theta), \phi_r(q_r),\phi_\theta(q_\theta))`
+        """
+        if initial_phases is None:
+            initial_phases = self.initial_phases
+        q_t0, q_r0, q_theta0, q_phi0 = initial_phases
 
-def plunging_radial_solutions_complex(a,E,L,Q):
-    r"""
-    Computes the radial solutions :math:`r(q_r), t_r(q_r), \phi_r(q_r)` from equation 50 and 51 of `Dyson and van de Meent <https://doi.org/10.48550/arXiv.2302.03704>`_ for the case of two complex radial roots.
-
-    :param a: dimensionless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
+        constants = (self.E, self.L, self.Q)
+        radial_roots = stable_radial_roots(self.a, self.p, self.e, self.x, constants)
+        polar_roots = stable_polar_roots(self.a, self.p, self.e, self.x, constants)
+        r, t_r, phi_r = radial_solutions(self.a, constants, radial_roots)
+        theta, t_theta, phi_theta = polar_solutions(self.a, constants, polar_roots)
+
+        return (
+            lambda q_r: t_r(q_r + q_r0),
+            lambda q_theta: t_theta(q_theta + q_theta0),
+            lambda q_r: phi_r(q_r + q_r0),
+            lambda q_theta: phi_theta(q_theta + q_theta0),
+        )
+
+    def trajectory(self, initial_phases=None, distance_units="natural", time_units="natural"):
+        r"""Computes the time, radial, polar, and azimuthal coordinates of the orbit 
+        as a function of mino time.
+
+        Parameters
+        ----------
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+        distance_units : str, optional
+            units to compute the radial component of the trajectory in
+            (options are "natural", "mks", "cgs", "au" and "km"),
+            defaults to "natural"
+        time_units : str, optional
+            units to compute the time component of the trajectory in
+            (options are "natural", "mks", "cgs", and "days"), defaults
+            to "natural"
+
+        Returns
+        -------
+        tuple(function, function, function, function)
+            tuple of functions :math:`(t(\lambda), r(\lambda), \theta(\lambda), \phi(\lambda))`
+        """
+        if initial_phases is None:
+            initial_phases = self.initial_phases
 
-    :return: tuple of radial solutions :math:`(r(q_r), t_r(q_r), \phi_r(q_r))`
-    :rtype: tuple(function, function, function)
+        return stable_trajectory(
+            self.a, self.p, self.e, self.x, initial_phases, self.M, distance_units, time_units
+        )
+
+
+def radial_solutions(a, constants, radial_roots):
+    r"""Computes the radial solutions :math:`r(q_r), t^{(r)}(q_r), \phi^{(r)}(q_r)` 
+    from equation 6 of `Fujita and Hikida <https://doi.org/10.48550/arXiv.0906.1420>`_. 
+    :math:`q_r` is defined as :math:`q_r = \Upsilon_r \lambda = 2\pi \frac{\lambda}{\Lambda_r}`. 
+    Assumes the initial conditions :math:`r(0) = r_{\text{min}}` and 
+    :math:`\theta(0) = \theta_{\text{min}}`.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin parameter
+    constants : tuple(double,double,double)
+        tuple of constants :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    radial_roots : tuple(double,double,double,double)
+        tuple of roots :math:`(r_1,r_2,r_3,r_4)`. Assumes that motion is
+        between :math:`r_1` and :math:`r_2` and that roots are otherwise
+        in decreasing order.
+
+    Returns
+    -------
+    tuple(function, function, function)
+        tuple of functions :math:`(r, t^{(r)}, \phi^{(r)})`
     """
-    roots = plunging_radial_roots(a,E,L,Q)
-    if np.iscomplex(roots).sum() != 2: raise ValueError("There should be two complex roots")
+    E, L, Q = constants
+    r1, r2, r3, r4 = radial_roots
 
-    r1, r2, r3, r4 = roots # r1 < r2 are real and r3/r4 are complex conjugates
-    rho_r = np.real(r3)
-    rho_i = np.imag(r4)
+    r_plus = 1 + sqrt(1 - a**2)
+    r_minus = 1 - sqrt(1 - a**2)
 
-    # inner and outer horizons
-    r_plus = 1+sqrt(1-a**2)
-    r_minus = 1-sqrt(1-a**2)
+    h_r = (r1 - r2) / (r1 - r3)
+    h_plus = (r1 - r2) * (r3 - r_plus) / ((r1 - r3) * (r2 - r_plus))
+    h_minus = (r1 - r2) * (r3 - r_minus) / ((r1 - r3) * (r2 - r_minus))
 
-    # equation 42
-    A = sqrt((r2-rho_r)**2+rho_i**2)
-    B = sqrt((r1-rho_r)**2+rho_i**2)
-    k_r = sqrt(((r2-r1)**2-(A-B)**2)/(4*A*B))
+    # equation 13
+    k_r = sqrt((r1 - r2) * (r3 - r4) / ((r1 - r3) * (r2 - r4)))
 
-    upsilon_r, upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
+    def r(q_r):
+        # equation 27
+        u_r = ellipk(k_r**2) * q_r / pi
 
-    I_r, I_r2, I_r_plus, I_r_minus = plunging_radial_integrals(a,E,L,Q)
+        sn, cn, dn, psi_r = ellipj(u_r, k_r**2)
+        return (r3 * (r1 - r2) * sn**2 - r2 * (r1 - r3)) / ((r1 - r2) * sn**2 - (r1 - r3))
 
-    def r(q_r):
-        # equation 43
-        sn, cn, dn, xi_r = ellipj(2*ellipk(k_r**2)*q_r/pi,k_r**2)
-        # equation 49
-        return ((A-B)*(A*r1-B*r2)*sn**2+2*A*B*(r1+r2)-2*A*B*(r2-r1)*cn)/(4*A*B+(A-B)**2*sn**2)
-    
     def t_r(q_r):
-        mino_time = q_r/upsilon_r
-        # equation 41
-        return E*(r_plus**2+r_minus**2+r_plus*r_minus+2*a**2)*mino_time + \
-            E*(I_r2(q_r)+I_r(q_r)*(r_minus+r_plus)) + \
-            ((r_minus**2+a**2)*(E*(r_minus**2+a**2)-a*L)/(r_minus-r_plus)*I_r_minus(q_r) + 
-             (r_plus**2+a**2)*(E*(r_plus**2+a**2)-a*L)/(r_plus-r_minus)*I_r_plus(q_r)
-            )
+        # equation 27
+        u_r = ellipk(k_r**2) * q_r / pi
+        sn, cn, dn, psi_r = ellipj(u_r, k_r**2)
 
-    def phi_r(q_r):
-        mino_time = q_r/upsilon_r
-        # equation 40
-        return a*(
-            (E*(r_minus**2+a**2)-a*L)/(r_minus-r_plus)*I_r_minus(q_r) +
-            (E*(r_plus**2+a**2)-a*L)/(r_plus-r_minus)*I_r_plus(q_r)
+        # equation 28
+        return (
+            2
+            / sqrt((1 - E**2) * (r1 - r3) * (r2 - r4))
+            * (
+                E
+                / 2
+                * (
+                    (r2 - r3)
+                    * (r1 + r2 + r3 + r4)
+                    * (_ellippiinc(psi_r, h_r, k_r**2) - q_r / pi * _ellippi(h_r, k_r**2))
+                    + (r1 - r3)
+                    * (r2 - r4)
+                    * (
+                        _ellipeinc(psi_r, k_r**2)
+                        + h_r * sn * cn * sqrt(1 - k_r**2 * sn**2) / (h_r * sn**2 - 1)
+                        - q_r / pi * ellipe(k_r**2)
+                    )
+                )
+                + 2
+                * E
+                * (r2 - r3)
+                * (_ellippiinc(psi_r, h_r, k_r**2) - q_r / pi * _ellippi(h_r, k_r**2))
+                - 2
+                / (r_plus - r_minus)
+                * (
+                    ((4 * E - a * L) * r_plus - 2 * a**2 * E)
+                    * (r2 - r3)
+                    / ((r3 - r_plus) * (r2 - r_plus))
+                    * (
+                        _ellippiinc(psi_r, h_plus, k_r**2)
+                        - q_r / pi * _ellippi(h_plus, k_r**2)
+                    )
+                    - ((4 * E - a * L) * r_minus - 2 * a**2 * E)
+                    * (r2 - r3)
+                    / ((r3 - r_minus) * (r2 - r_minus))
+                    * (
+                        _ellippiinc(psi_r, h_minus, k_r**2)
+                        - q_r / pi * _ellippi(h_minus, k_r**2)
+                    )
+                )
             )
-    
-    return r, t_r, phi_r
+        )
 
-def plunging_polar_solutions(a,E,L,Q):
-    r"""
-    Computes the polar solutions :math:`\theta(q_\theta), t_\theta(q_\theta), \phi_\theta(q_\theta)` from equation 33 and 37 of `Dyson and van de Meent <https://doi.org/10.48550/arXiv.2302.03704>`_
-
-    :param a: dimensionless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
-    
-    :return: tuple of polar solutions :math:`(\theta(q_\theta), t_\theta(q_\theta), \phi_\theta(q_\theta))`
-    :rtype: tuple(function, function, function)
-    """
-    z1 = sqrt(1/2*(1+(L**2+Q)/(a**2*(1-E**2))-sqrt((1+(L**2+Q)/(a**2*(1-E**2)))**2-4*Q/(a**2*(1-E**2)))))
-    z2 = sqrt(a**2*(1-E**2)/2*(1+(L**2+Q)/(a**2*(1-E**2))+sqrt((1+(L**2+Q)/(a**2*(1-E**2)))**2-4*Q/(a**2*(1-E**2)))))
-    k_theta = a*sqrt(1-E**2)*z1/z2
-
-    upsilon_r, upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
-
-    def theta(q_theta):
-        mino_time = q_theta/upsilon_theta
-        # equation 28
-        sn, cn, dn, xi_theta = ellipj(z2*mino_time,k_theta**2)
+    def phi_r(q_r):
         # equation 27
-        return arccos(z1*sn)
-    
-    def t_theta(q_theta):
-        mino_time = q_theta/upsilon_theta
-        # equation 28
-        sn, cn, dn, xi_theta = ellipj(z2*mino_time,k_theta**2)
-        # equation 35
-        return E/(1-E**2)*((z2**2-a**2*(1-E**2))*mino_time-z2*ellipeinc(xi_theta,k_theta**2))
-    
-    def phi_theta(q_theta):
-        mino_time = q_theta/upsilon_theta
+        u_r = ellipk(k_r**2) * q_r / pi
+        sn, cn, dn, psi_r = ellipj(u_r, k_r**2)
         # equation 28
-        sn, cn, dn, xi_theta = ellipj(z2*mino_time,k_theta**2)
-        # equation 31
-        return L/z2*_ellippiinc(xi_theta,z1**2,k_theta**2)
-    
-    return theta, t_theta, phi_theta
+        return (
+            -2
+            * a
+            / ((r_plus - r_minus) * sqrt((1 - E**2) * (r1 - r3) * (r2 - r4)))
+            * (
+                (2 * E * r_plus - a * L)
+                * (r2 - r3)
+                / ((r3 - r_plus) * (r2 - r_plus))
+                * (_ellippiinc(psi_r, h_plus, k_r**2) - q_r / pi * _ellippi(h_plus, k_r**2))
+                - (2 * E * r_minus - a * L)
+                * (r2 - r3)
+                / ((r3 - r_minus) * (r2 - r_minus))
+                * (_ellippiinc(psi_r, h_minus, k_r**2) - q_r / pi * _ellippi(h_minus, k_r**2))
+            )
+        )
 
-def plunging_trajectory(a,E,L,Q,initial_phases=(0,0,0,0),M=None,distance_units="natural",time_units="natural"):
-        r"""
-        Computes the components of the trajectory as a function of mino time for a plunging orbit with the given parameters.
-
-        :param a: dimensionless spin parameter
-        :type a: double
-        :param E: dimensionless energy
-        :type E: double
-        :param L: dimensionless angular momentum
-        :type L: double
-        :param Q: dimensionless Carter constant
-        :type Q: double
-        :param initial_phases: tuple of initial phases :math:`(q^t_0, q^r_0, q^\theta_0, q^\phi_0)`
-        :type initial_phases: tuple, optional
-        :param M: mass of the primary in solar masses
-        :type M: double, optional
-        :param distance_units: units to compute the radial component of the trajectory in (options are "natural", "mks", "cgs", "au" and "km"), defaults to "natural"
-        :type distance_units: str, optional
-        :param time_units: units to compute the time component of the trajectory in (options are "natural", "mks", "cgs", and "days"), defaults to "natural"
-        :type time_units: str, optional
-        
-        :return: components of the trajectory :math:`t(\lambda), r(\lambda), \theta(\lambda), \phi(\lambda)`
-        :rtype: tuple(function,function,function,function)
-        """
-        radial_roots = plunging_radial_roots(a,E,L,Q)
+    return r, t_r, phi_r
 
-        if np.iscomplex(radial_roots[3]):
-            return _complex_plunge_trajectory(a,E,L,Q,initial_phases,M,distance_units,time_units)
-        else:
-            return _real_plunge_trajectory(a,E,L,Q,initial_phases,M,distance_units,time_units)
-
-def _complex_plunge_trajectory(a,E,L,Q,initial_phases=(0,0,0,0), M=None, distance_units="natural",time_units="natural"):
-    r"""
-    Computes the components of the trajectory for a plunging orbit with the given parameters assuming that the radial polynomial has two complex roots and two real roots.
-
-    :param a: dimensionless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
-    :param initial_phases: tuple of initial phases :math:`(q^t_0, q^r_0, q^\theta_0, q^\phi_0)`
-    :type initial_phases: tuple, optional
-    :param M: mass of the primary in solar masses
-    :type M: double, optional
-    :param distance_units: units to compute the radial component of the trajectory in (options are "natural", "mks", "cgs", "au" and "km"), defaults to "natural"
-    :type distance_units: str, optional
-    :param time_units: units to compute the time component of the trajectory in (options are "natural", "mks", "cgs", and "days"), defaults to "natural"
-    :type time_units: str, optional
 
-    :return: components of the trajectory :math:`t(\lambda), r(\lambda), \theta(\lambda), \phi(\lambda)`
-    :rtype: tuple(function,function,function,function)
+def polar_solutions(a, constants, polar_roots):
+    r"""Computes the polar solutions :math:`\theta(q_\theta), t^{(\theta)}(q_\theta), 
+    \phi^{(\theta)}(q_\theta)` from equation 6 of `Fujita and Hikida 
+    <https://doi.org/10.48550/arXiv.0906.1420>`_. :math:`q_\theta` is defined as 
+    :math:`q_\theta = \Upsilon_\theta \lambda = 2\pi \frac{\lambda}{\Lambda_\theta}`.
+    Assumes the initial conditions :math:`r(0) = r_{\text{min}}` and 
+    :math:`\theta(0) = \theta_{\text{min}}`.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin parameter
+    constants : tuple(double,double,double)
+        tuple of constants :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+    polar_roots : tuple(double,double)
+        tuple of roots :math:`(z_-,z_+)`
+
+    Returns
+    -------
+    tuple(function, function, function)
+        tuple of functions :math:`(\theta, t^{(\theta)}, \phi^{(\theta)})`
     """
-    if ((distance_units != "natural") or (time_units != "natural")) and M is None: raise ValueError("M must be specified to convert to physical units")
+    E, L, Q = constants
+    z_minus, z_plus = polar_roots
+    epsilon0 = a**2 * (1 - E**2) / L**2
+    # simplified form of epsilon0*z_plus
+    e0zp = (a**2 * (1 - E**2) * (1 - z_minus) + L**2) / (L**2 * (1 - z_minus))
+    # simplified form of a**2*sqrt(z_plus/epsilon0)
+    a2sqrt_zp_over_e0 = (
+        L**2 / ((1 - E**2) * sqrt(1 - z_minus))
+        if a == 0
+        else a**2 * z_plus / sqrt(epsilon0 * z_plus)
+    )
 
-    upsilon_r, upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
-    r_phases, t_r, phi_r = plunging_radial_solutions_complex(a,E,L,Q)
-    theta_phases, t_theta, phi_theta = plunging_polar_solutions(a,E,L,Q)
-    q_t0, q_r0, q_theta0, q_phi0 = initial_phases
-
-    distance_conversion_func = {"natural": lambda x,M: x, "mks": distance_in_meters, "cgs": distance_in_cm, "au": distance_in_au,"km": distance_in_km}
-    time_conversion_func = {"natural": lambda x,M: x, "mks": time_in_seconds, "cgs": time_in_seconds, "days": time_in_days}
+    # equation 13
+    k_theta = 0 if a == 0 else sqrt(z_minus / z_plus)
 
-    # adjust q_theta0 so that initial conditions are consistent with stable orbits
-    q_theta0 = q_theta0 + pi/2
+    def theta(q_theta):
+        u_theta = 2 / pi * ellipk(k_theta**2) * (q_theta + pi / 2)
+        sn, cn, dn, ph = ellipj(u_theta, k_theta**2)
+        # equation 38
+        return arccos(sqrt(z_minus) * sn)
 
-    # Calculate normalization constants so that t = 0 and phi = 0 at lambda = 0 when q_t0 = 0 and q_phi0 = 0 
-    C_t = t_r(q_r0)+t_theta(q_theta0)
-    C_phi= phi_r(q_r0)+phi_theta(q_theta0)
+    def t_theta(q_theta):
+        u_theta = 2 / pi * ellipk(k_theta**2) * (q_theta + pi / 2)
+        sn, cn, dn, psi_theta = ellipj(u_theta, k_theta**2)
+        # equation 39
+        return (
+            sign(L)
+            * a2sqrt_zp_over_e0
+            * E
+            / L
+            * (
+                2 / pi * ellipe(k_theta**2) * (q_theta + pi / 2)
+                - _ellipeinc(psi_theta, k_theta**2)
+            )
+        )
 
-    def t(mino_time):
-        return time_conversion_func[time_units](t_r(upsilon_r*mino_time+q_r0) + t_theta(upsilon_theta*mino_time+q_theta0) - C_t + q_t0, M)
-    
-    def r(mino_time):
-        return distance_conversion_func[distance_units](r_phases(upsilon_r*mino_time+q_r0), M)
-    
-    def theta(mino_time):
-        return theta_phases(upsilon_theta*mino_time+q_theta0)
-    
-    def phi(mino_time):
-        return phi_r(upsilon_r*mino_time+q_r0) + phi_theta(upsilon_theta*mino_time+q_theta0) - C_phi + q_phi0
-    
-    return t, r, theta, phi
+    def phi_theta(q_theta):
+        sn, cn, dn, psi_theta = ellipj(
+            2 / pi * ellipk(k_theta**2) * (q_theta + pi / 2), k_theta**2
+        )
+        # equation 39
+        return (
+            sign(L)
+            * 1
+            / sqrt(e0zp)
+            * (
+                _ellippiinc(psi_theta, z_minus, k_theta**2)
+                - 2 / pi * _ellippi(z_minus, k_theta**2) * (q_theta + pi / 2)
+            )
+        )
 
+    return theta, t_theta, phi_theta
 
-def _real_plunge_trajectory(a,E,L,Q,initial_phases=(0,0,0,0),M=None,distance_units="natural",time_units="natural"):
-    r"""
-    Computes the components of the trajectory for a plunging orbit with the given parameters assuming that there are four real roots of the radial polynomial.
-
-    :param a: dimensionless spin parameter
-    :type a: double
-    :param E: dimensionless energy
-    :type E: double
-    :param L: dimensionless angular momentum
-    :type L: double
-    :param Q: dimensionless Carter constant
-    :type Q: double
-    :param initial_phases: tuple of initial phases :math:`(q^t_0, q^r_0, q^\theta_0, q^\phi_0)`
-    :type initial_phases: tuple, optional
-    :param M: mass of the primary in solar masses
-    :type M: double, optional
-    :param distance_units: units to compute the radial component of the trajectory in (options are "natural", "mks", "cgs", "au" and "km"), defaults to "natural"
-    :type distance_units: str, optional
-    :param time_units: units to compute the time component of the trajectory in (options are "natural", "mks", "cgs", and "days"), defaults to "natural"
-    :type time_units: str, optional
 
-    :return: components of the trajectory :math:`t(\lambda), r(\lambda), \theta(\lambda), \phi(\lambda)`
-    :rtype: tuple(function,function,function,function)
+def stable_trajectory(
+    a, p, e, x, initial_phases=(0, 0, 0, 0), M=None, distance_units="natural", time_units="natural"
+):
+    r"""Computes the time, radial, polar, and azimuthal coordinates of the orbit with the given 
+    parameters as a function of mino time.
+
+    Parameters
+    ----------
+    a : double
+        dimensionless spin parameter
+    p : double
+        semi-latus rectum
+    e : double
+        orbital eccentricity
+    x : double
+        cosine of the orbital inclination
+    initial_phases : tuple, optional
+        tuple of initial phases
+        :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`, defaults to (0,0,0,0)
+    M : double, optional
+        mass of the primary in solar masses
+    distance_units : str, optional
+        units to compute the radial component of the trajectory in
+        (options are "natural", "mks", "cgs", "au" and "km"), defaults
+        to "natural"
+    time_units : str, optional
+        units to compute the time component of the trajectory in
+        (options are "natural", "mks", "cgs", and "days"), defaults to
+        "natural"
+
+    Returns
+    -------
+    tuple(function, function, function, function)
+        tuple of functions :math:`(t(\lambda), r(\lambda),
+        \theta(\lambda), \phi(\lambda))`
     """
-    if ((distance_units != "natural") or (time_units != "natural")) and M is None: raise ValueError("M must be specified to convert to physical units")
+    if ((distance_units != "natural") or (time_units != "natural")) and M is None:
+        raise ValueError("M must be specified to convert to physical units")
 
-    constants = (E,L,Q)
-    radial_roots = plunging_radial_roots(a,E,L,Q)
+    upsilon_r, upsilon_theta, upsilon_phi, gamma = mino_frequencies(a, p, e, x)
+    constants = constants_of_motion(a, p, e, x)
+    radial_roots = stable_radial_roots(a, p, e, x, constants)
+    polar_roots = stable_polar_roots(a, p, e, x, constants)
 
-    # polar polynomial written in terms of z = cos^2(theta)
-    Z = Polynomial([Q,-(Q+a**2*(1-E**2)+L**2),a**2*(1-E**2)])
-    polar_roots = Z.roots()
-    if a == 0: polar_roots = [polar_roots[0], polar_roots[0]]
-
-    upsilon_r, upsilon_theta, upsilon_phi, gamma = _mino_frequencies_from_constants(a,constants,radial_roots,polar_roots)
-    r_phases, t_r, phi_r = radial_solutions(a,constants,radial_roots)
-    theta_phases, t_theta, phi_theta = polar_solutions(a,constants,polar_roots)
+    r_phases, t_r, phi_r = radial_solutions(a, constants, radial_roots)
+    theta_phases, t_theta, phi_theta = polar_solutions(a, constants, polar_roots)
     q_t0, q_r0, q_theta0, q_phi0 = initial_phases
 
-    distance_conversion_func = {"natural": lambda x,M: x, "mks": distance_in_meters, "cgs": distance_in_cm, "au": distance_in_au,"km": distance_in_km}
-    time_conversion_func = {"natural": lambda x,M: x, "mks": time_in_seconds, "cgs": time_in_seconds, "days": time_in_days}
-
-    # Calculate normalization constants so that t = 0 and phi = 0 at lambda = 0 when q_t0 = 0 and q_phi0 = 0 
-    C_t = t_r(q_r0)+t_theta(q_theta0)
-    C_phi= phi_r(q_r0)+phi_theta(q_theta0)
+    distance_conversion_func = {
+        "natural": lambda x, M: x,
+        "mks": distance_in_meters,
+        "cgs": distance_in_cm,
+        "au": distance_in_au,
+        "km": distance_in_km,
+    }
+    time_conversion_func = {
+        "natural": lambda x, M: x,
+        "mks": time_in_seconds,
+        "cgs": time_in_seconds,
+        "days": time_in_days,
+    }
+
+    # Calculate normalization constants so that t = 0 and phi = 0 at lambda = 0 when q_t0 = 0 and q_phi0 = 0
+    C_t = t_r(q_r0) + t_theta(q_theta0)
+    C_phi = phi_r(q_r0) + phi_theta(q_theta0)
 
     def t(mino_time):
         # equation 6
-        return time_conversion_func[time_units](q_t0 + gamma*mino_time + t_r(upsilon_r*mino_time+q_r0) + t_theta(upsilon_theta*mino_time+q_theta0) - C_t, M)
-    
+        return time_conversion_func[time_units](
+            q_t0
+            + gamma * mino_time
+            + t_r(upsilon_r * mino_time + q_r0)
+            + t_theta(upsilon_theta * mino_time + q_theta0)
+            - C_t,
+            M,
+        )
+
     def r(mino_time):
-        return distance_conversion_func[distance_units](r_phases(upsilon_r*mino_time+q_r0), M)
-    
+        return distance_conversion_func[distance_units](
+            r_phases(upsilon_r * mino_time + q_r0), 
+            M)
+
     def theta(mino_time):
-        return theta_phases(upsilon_theta*mino_time+q_theta0)
-    
+        return theta_phases(upsilon_theta * mino_time + q_theta0)
+
     def phi(mino_time):
         # equation 6
-        return q_phi0 + upsilon_phi*mino_time + phi_r(upsilon_r*mino_time+q_r0) + phi_theta(upsilon_theta*mino_time+q_theta0) - C_phi
-    
-    return t, r, theta, phi
+        return (
+            q_phi0
+            + upsilon_phi * mino_time
+            + phi_r(upsilon_r * mino_time + q_r0)
+            + phi_theta(upsilon_theta * mino_time + q_theta0)
+            - C_phi
+        )
+
+    return t, r, theta, phi
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy/spacetime.py` & `kerrgeopy-0.9.2/kerrgeopy/spacetime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,210 @@
-"""
-Module containing the KerrSpacetime class
-"""
+"""Module containing the KerrSpacetime class"""
 from .constants import *
 from numpy import cos, sin
 import numpy as np
 
+
 class KerrSpacetime:
-    """
-        Class representing spacetime around a black hole with mass :math:`M` and spin parameter :math:`a`
+    """Class representing spacetime around a black hole with mass :math:`M` 
+    and spin parameter :math:`a`
 
-        :param a: dimensionless angular momentum
-        :type a: double
-        :param M: mass of the black hole
-        :type M: double
-
-        :ivar a: dimensionless angular momentum
-        :ivar M: mass of the black hole
-        :ivar inner_horizon: radius of the inner horizon
-        :ivar outer_horizon: radius of the outer horizon
+    Parameters
+    ----------
+    a : double
+        dimensionless angular momentum
+    M : double
+        mass of the black hole
+
+    Attributes
+    ----------
+    a
+        dimensionless angular momentum
+    M
+        mass of the black hole
+    inner_horizon
+        radius of the inner horizon
+    outer_horizon
+        radius of the outer horizon
     """
-    def __init__(self,a,M=None):
-        self.a, self.M = a, M
-        self.inner_horizon = 1-sqrt(1-self.a**2)
-        self.outer_horizon = 1+sqrt(1-self.a**2)
 
-    def separatrix(self,e,x):
-        """
-        Computes the value of p at the separatrix for a given value of e and x
-
-        :param e: orbital eccentricity
-        :type e: double
-        :param x: cosine of the orbital inclination
-        :type x: double
-
-        :rtype: double
-        """
-        return separatrix(self.a,e,x)
-    
-    def is_stable(self,p,e,x):
-        """
-        Determines whether a given orbit is stable or not
-
-        :param p: dimensionless semi-latus rectum
-        :type p: double
-        :param e: orbital eccentricity
-        :type e: double
-        :param x: cosine of the orbital inclination
-        :type x: double
-        
-        :rtype: bool
-        """
-        return is_stable(self.a,p,e,x)
-    
-    def metric(self,t,r,theta,phi):
-        """
-        Returns the matrix representation of the metric at a given point expressed in Boyer-Lindquist coordinates.
+    def __init__(self, a, M=None):
+        self.a, self.M = a, M
+        self.inner_horizon = 1 - sqrt(1 - self.a**2)
+        self.outer_horizon = 1 + sqrt(1 - self.a**2)
 
-        :param t: time coordinate
-        :type t: double
-        :param r: radial coordinate
-        :type r: double
-        :param theta: polar coordinate
-        :type theta: double
-        :param phi: azimuthal coordinate
-        :type phi: double
+    def separatrix(self, e, x):
+        """Computes the value of p at the separatrix for a given value of e and x
 
-        :rtype: numpy.ndarray
+        Parameters
+        ----------
+        e : double
+            orbital eccentricity
+        x : double
+            cosine of the orbital inclination
+
+        Returns
+        -------
+        double
+        """
+        return separatrix(self.a, e, x)
+
+    def is_stable(self, p, e, x):
+        """Determines whether a given orbit is stable or not
+
+        Parameters
+        ----------
+        p : double
+            dimensionless semi-latus rectum
+        e : double
+            orbital eccentricity
+        x : double
+            cosine of the orbital inclination
+
+        Returns
+        -------
+        bool
+        """
+        return is_stable(self.a, p, e, x)
+
+    def metric(self, t, r, theta, phi):
+        """Returns the matrix representation of the metric at a given point 
+        expressed in Boyer-Lindquist coordinates.
+
+        Parameters
+        ----------
+        t : double
+            time coordinate
+        r : double
+            radial coordinate
+        theta : double
+            polar coordinate
+        phi : double
+            azimuthal coordinate
+
+        Returns
+        -------
+        numpy.ndarray
         """
         a = self.a
-        sigma = r**2+a**2*cos(theta)**2
-        delta = r**2-2*r+a**2
+        sigma = r**2 + a**2 * cos(theta) ** 2
+        delta = r**2 - 2 * r + a**2
+        # fmt: off
         return np.array(
             [[-(1-2*r/sigma),               0,              0,      -2*a*r*sin(theta)**2/sigma],
              [0,                            sigma/delta,    0,      0],
              [0,                            0,              sigma,  0],
              [-2*a*r*sin(theta)**2/sigma,   0,              0,      sin(theta)**2*(r**2+a**2+2*a**2*r*sin(theta)**2/sigma)]
              ]
         )
-    
-    def norm(self,t,r,theta,phi,v):
-        """
-        Computes the norm of a vector at a given point in spacetime expressed in Boyer-Lindquist coordinates
-
-        :param t: time coordinate
-        :type t: double
-        :param r: radial coordinate
-        :type r: double
-        :param theta: polar coordinate
-        :type theta: double
-        :param phi: azimuthal coordinate
-        :type phi: double
-        :param v: vector to compute the norm of
-        :type v: array_like
-
-        :return: norm of v
-        :rtype: double
-        """
-        return np.dot(v,np.dot(self.metric(t,r,theta,phi),v))
-    
-    def four_velocity(self,t,r,theta,phi,constants,upsilon_r,upsilon_theta,initial_phases):
-        r"""
-        Computes the four velocity of a given trajectory
-
-        :param t: time component of trajectory
-        :type t: function
-        :param r: radial component of trajectory
-        :type r: function
-        :param theta: polar component of trajectory
-        :type theta: function
-        :param phi: azimuthal component of trajectory
-        :type phi: function
-        :param constants: tuple of constants of motion in the form :math:`(E,L,Q)`
-        :type constants: tuple(double, double, double)
-        :param upsilon_r: radial frequency
-        :type upsilon_r: double
-        :param upsilon_theta: polar frequency
-        :type upsilon_theta: double
-        :param initial_phases: tuple of initial phases :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
-        :type initial_phases: tuple, optional
+        # fmt: on
 
-        :return: components of the four velocity (i.e. :math:`(u^t,u^r,u^\theta,u^\phi)`)
-        :rtype: tuple(function, function, function, function)
+    def norm(self, t, r, theta, phi, v):
+        """Computes the norm of a vector at a given point in spacetime 
+        expressed in Boyer-Lindquist coordinates
+
+        Parameters
+        ----------
+        t : double
+            time coordinate
+        r : double
+            radial coordinate
+        theta : double
+            polar coordinate
+        phi : double
+            azimuthal coordinate
+        v : array_like
+            vector to compute the norm of
+
+        Returns
+        -------
+        double
+            norm of v
+        """
+        return np.dot(v, np.dot(self.metric(t, r, theta, phi), v))
+
+    def four_velocity(self, t, r, theta, phi, constants, upsilon_r, upsilon_theta, initial_phases):
+        r"""Computes the four velocity of a given trajectory
+
+        Parameters
+        ----------
+        t : function
+            time component of trajectory
+        r : function
+            radial component of trajectory
+        theta : function
+            polar component of trajectory
+        phi : function
+            azimuthal component of trajectory
+        constants : tuple(double, double, double)
+            tuple of constants of motion in the form 
+            :math:`(\mathcal{E},\mathcal{L},\mathcal{Q})`
+        upsilon_r : double
+            radial frequency
+        upsilon_theta : double
+            polar frequency
+        initial_phases : tuple, optional
+            tuple of initial phases
+            :math:`(q_{t_0},q_{r_0},q_{\theta_0},q_{\phi_0})`
+
+        Returns
+        -------
+        tuple(function, function, function, function)
+            components of the four velocity (i.e.
+            :math:`(u^t,u^r,u^\theta,u^\phi)`)
         """
         a = self.a
         E, L, Q = constants
         q_t0, q_r0, q_theta0, q_phi0 = initial_phases
 
         # radial polynomial
-        R = lambda r: (E*(r**2+a**2)-a*L)**2-(r**2-2*r+a**2)*(r**2+(a*E-L)**2+Q)
-        # R = Polynomial([-a**2*Q, 2*L**2+2*Q+2*a**2*E**2-4*a*E*L, a**2*E**2-L**2-Q-a**2, 2, E**2-1])
-
+        R = lambda r: (E * (r**2 + a**2) - a * L) ** 2 - (r**2 - 2 * r + a**2) * (
+            r**2 + (a * E - L) ** 2 + Q
+        )
         # polar polynomial
-        Z = lambda z: Q-(Q+a**2*(1-E**2)+L**2)*z**2+a**2*(1-E**2)*z**4
-        # Z = lambda z: Q-z**2*(a**2*(1-E**2)*(1-z**2)+L**2+Q)
-        # Z = Polynomial([Q,-(Q+a**2*(1-E**2)+L**2),a**2*(1-E**2)])
-
+        Z = (
+            lambda z: Q
+            - (Q + a**2 * (1 - E**2) + L**2) * z**2
+            + a**2 * (1 - E**2) * z**4
+        )
+        
         def u_t(time):
-            delta = r(time)**2-2*r(time)+a**2
-            sigma = r(time)**2+a**2*cos(theta(time))**2
-            return 1/sigma*((r(time)**2+a**2)/delta*(E*(r(time)**2+a**2)-a*L)-a**2*E*(1-cos(theta(time))**2)+a*L)
+            delta = r(time) ** 2 - 2 * r(time) + a**2
+            sigma = r(time) ** 2 + a**2 * cos(theta(time)) ** 2
+            return (
+                1
+                / sigma
+                * (
+                    (r(time) ** 2 + a**2) / delta * (E * (r(time) ** 2 + a**2) - a * L)
+                    - a**2 * E * (1 - cos(theta(time)) ** 2)
+                    + a * L
+                )
+            )
 
         def u_r(time):
-            q_r = upsilon_r*time + q_r0
-            sigma = r(time)**2+a**2*cos(theta(time))**2
-            return np.copysign(1,sin(q_r))*sqrt(abs(R(r(time))))/sigma
+            q_r = upsilon_r * time + q_r0
+            sigma = r(time) ** 2 + a**2 * cos(theta(time)) ** 2
+            return np.copysign(1, sin(q_r)) * sqrt(abs(R(r(time)))) / sigma
 
         def u_theta(time):
-            q_theta = upsilon_theta*time + q_theta0
-            sigma = r(time)**2+a**2*cos(theta(time))**2
-            return np.copysign(1,sin(q_theta))*sqrt(abs(Z(cos(theta(time)))))/(sigma*sin(theta(time)))
-        
+            q_theta = upsilon_theta * time + q_theta0
+            sigma = r(time) ** 2 + a**2 * cos(theta(time)) ** 2
+            return (
+                np.copysign(1, sin(q_theta))
+                * sqrt(abs(Z(cos(theta(time)))))
+                / (sigma * sin(theta(time)))
+            )
+
         def u_phi(time):
-            sigma = r(time)**2+a**2*cos(theta(time))**2
-            delta = r(time)**2-2*r(time)+a**2
-            return 1/sigma*(a/delta*(E*(r(time)**2+a**2)-a*L)+L/(1-cos(theta(time))**2)-a*E)
-        
-        return u_t, u_r, u_theta, u_phi
+            sigma = r(time) ** 2 + a**2 * cos(theta(time)) ** 2
+            delta = r(time) ** 2 - 2 * r(time) + a**2
+            return (
+                1
+                / sigma
+                * (
+                    a / delta * (E * (r(time) ** 2 + a**2) - a * L)
+                    + L / (1 - cos(theta(time)) ** 2)
+                    - a * E
+                )
+            )
+
+        return u_t, u_r, u_theta, u_phi
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy.egg-info/PKG-INFO` & `kerrgeopy-0.9.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,57 @@
 Metadata-Version: 2.1
 Name: kerrgeopy
-Version: 0.9.1
+Version: 0.9.2
 Summary: Library for computing stable and plunging geodesics in Kerr spacetime
 Home-page: https://github.com/BlackHolePerturbationToolkit/KerrGeoPy
 Author: Seyong Park
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy>=1.8
 Requires-Dist: numpy
 Requires-Dist: matplotlib>=3.7
 Requires-Dist: tqdm
 
+[![GitHub release (with filter)](https://img.shields.io/github/v/release/BlackHolePerturbationToolkit/KerrGeoPy)](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/releases)
+[![Test Status](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/actions/workflows/tests.yml/badge.svg)](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/actions)
+[![PyPI - Version](https://img.shields.io/pypi/v/kerrgeopy)](https://pypi.org/project/kerrgeopy/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/kerrgeopy.svg)](https://anaconda.org/conda-forge/kerrgeopy)
+[![Documentation Status](https://readthedocs.org/projects/kerrgeopy/badge/?version=latest)](https://kerrgeopy.readthedocs.io/en/latest/?badge=latest)
+[![GitHub License](https://img.shields.io/github/license/BlackHolePerturbationToolkit/KerrGeoPy)](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/blob/main/LICENSE)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8417442.svg)](https://doi.org/10.5281/zenodo.8417442)
+
 # KerrGeoPy
 
 KerrGeoPy is a python implementation of the [KerrGeodesics](https://bhptoolkit.org/KerrGeodesics/) Mathematica library. It is intended for use in computing orbital trajectories for extreme-mass-ratio inspirals (EMRIs). It implements the analytical solutions for plunging orbits from [Dyson and van de Meent](https://arxiv.org/abs/2302.03704), as well as solutions for stable orbits from [Fujita and Hikida](https://arxiv.org/abs/0906.1420). The library also provides a set of methods for computing constants of motion and orbital frequencies. See the [documentation](https://kerrgeopy.readthedocs.io/en/latest/) for more information.
 
 ## Installation
 
-Install the latest version of kerrgeopy using pip
-
+Install using Anaconda
+```bash
+conda install -c conda-forge kerrgeopy
+```
+or using pip
 ```bash
 pip install kerrgeopy
 ```
+
+> **Note**
+>
+> This library uses functions introduced in scipy 1.8, so it may also be necessary to update scipy by running `pip install scipy -U`, although in most cases this should be done automatically by pip. Certain plotting and animation functions also make use of features introduced in matplotlib 3.7 and rely on [ffmpeg](https://ffmpeg.org/download.html), which can be easily installed using [homebrew](https://formulae.brew.sh/formula/ffmpeg) or [anaconda](https://anaconda.org/conda-forge/ffmpeg).
+
+## Contributing
+
+For contribution guidelines, see [CONTRIBUTING](https://github.com/BlackHolePerturbationToolkit/KerrGeoPy/blob/main/CONTRIBUTING.md).
+
 ## Stable Bound Orbits
 
-Kerrgeopy computes orbits in Boyer-Lindquist coordinates $(t,r,\theta,\phi)$. Let $M$ to represent the mass of the primary body and let $J$ represent its angular momentum. Working in geometrized units where $G=c=1$, stable bound orbits are parametrized using the following variables:
+KerrGeoPy computes orbits in Boyer-Lindquist coordinates $(t,r,\theta,\phi)$. Let $M$ to represent the mass of the primary body and let $J$ represent its angular momentum. Working in geometrized units where $G=c=1$, stable bound orbits are parametrized using the following variables:
 
 $a$ - spin of the primary body
 <br>
 $p$ - orbital semilatus rectum
 <br>
 $e$ - orbital eccentricity
 <br>
@@ -58,15 +78,15 @@
 
 ```python
 fig, ax = orbit.plot(0,10)
 ```
 
 
     
-![png](README_files/Getting%20Started_3_0.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_3_0.png)
     
 
 
 Next, compute the time, radial, polar and azimuthal components of the trajectory as a function of Mino time using the `trajectory()` method. By default, the time and radial components of the trajectory are given in geometrized units and are normalized using $M$ so that they are dimensionless.
 
 
 ```python
@@ -103,15 +123,15 @@
 plt.ylabel(r"$\phi(\lambda)$")
 ```
 
 
 
 
     
-![png](README_files/Getting%20Started_6_1.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_6_1.png)
     
 
 
 ## Orbital Properties
 
 Use the `constants_of_motion()` method to compute the dimensionless energy, angular momentum and Carter constant. By default, constants of motion are given in geometrized units where $G=c=1$ and are scale-invariant, meaning that they are normalized according to the masses of the two bodies as follows:
 
@@ -230,15 +250,15 @@
 plt.plot(time, phi(time))
 plt.xlabel("$\lambda$")
 plt.ylabel(r"$\phi(\lambda)$")
 ```
 
 
     
-![png](README_files/Getting%20Started_15_1.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_15_1.png)
     
 
 
 
 ## Alternative Parametrizations
 
 Use the `from_constants()` class method to construct a `StableOrbit` from the spin parameter and constants of motion $(a,E,L,Q)$
@@ -285,14 +305,14 @@
 
 plt.subplot(1,4,4)
 plt.plot(time, phi(time))
 plt.xlabel("$\lambda$")
 plt.ylabel(r"$\phi(\lambda)$")
 ```
     
-![png](README_files/Getting%20Started_20_1.png)
+![png](https://raw.githubusercontent.com/BlackHolePerturbationToolkit/KerrGeoPy/main/README_files/Getting%20Started_20_1.png)
     
 
 ## Authors
 
 * Seyong Park
 * Zach Nasipak
```

### Comparing `kerrgeopy-0.9.1/kerrgeopy.egg-info/SOURCES.txt` & `kerrgeopy-0.9.2/kerrgeopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kerrgeopy-0.9.1/setup.py` & `kerrgeopy-0.9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="kerrgeopy",
-    version="0.9.1",
+    version="0.9.2",
     author="Seyong Park",
     description="Library for computing stable and plunging geodesics in Kerr spacetime",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/BlackHolePerturbationToolkit/KerrGeoPy",
     packages=setuptools.find_packages(exclude=["tests"]),
     classifiers=(
```

### Comparing `kerrgeopy-0.9.1/tests/test_four_velocity.py` & `kerrgeopy-0.9.2/tests/test_four_velocity.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,112 +4,146 @@
 from kerrgeopy.plunge import *
 from pathlib import Path
 
 THIS_DIR = Path(__file__).parent
 
 DATA_DIR = THIS_DIR.parent / "tests/data"
 
-stable_orbit_values = np.genfromtxt(DATA_DIR / "stable_orbit_parameters.txt", delimiter=",")
-complex_plunging_orbit_values = np.genfromtxt(DATA_DIR / "plunging_orbit_parameters_complex.txt", delimiter=",")
-real_plunging_orbit_values = np.genfromtxt(DATA_DIR / "plunging_orbit_parameters_real.txt", delimiter=",")
-plunging_orbit_values = np.concatenate((complex_plunging_orbit_values,real_plunging_orbit_values),axis=0)
+stable_orbit_parameters = np.genfromtxt(
+    DATA_DIR / "stable_orbit_parameters.txt", delimiter=","
+)
+complex_plunging_orbit_parameters = np.genfromtxt(
+    DATA_DIR / "plunging_orbit_parameters_complex.txt", delimiter=","
+)
+real_plunging_orbit_parameters = np.genfromtxt(
+    DATA_DIR / "plunging_orbit_parameters_real.txt", delimiter=","
+)
+plunging_orbit_parameters = np.concatenate(
+    (complex_plunging_orbit_parameters, real_plunging_orbit_parameters), axis=0
+)
 times = np.genfromtxt(DATA_DIR / "stable_orbit_times.txt", delimiter=",")
 
+
 class TestFourVelocity(unittest.TestCase):
     def test_stable_orbit_four_velocity(self):
-        components = ["ut","ur","utheta","uphi"]
+        """
+        Test four_velocity method against output from the KerrGeodesics
+        Mathematica library for a random set of orbits.
+        """
+        components = ["ut", "ur", "utheta", "uphi"]
+
+        for i, orbit in enumerate(stable_orbit_parameters):
+            mathematica_trajectory = np.genfromtxt(
+                DATA_DIR / f"four_velocity/trajectory{i}.txt", delimiter=","
+            )
 
-        for i, orbit in enumerate(stable_orbit_values):
-            mathematica_trajectory = np.genfromtxt(DATA_DIR / f"four_velocity/trajectory{i}.txt", delimiter=",")
-            
-            a,p,e,x = orbit
-            stable_orbit = StableOrbit(a,p,e,x)
+            a, p, e, x = orbit
+            stable_orbit = StableOrbit(a, p, e, x)
             u_t, u_r, u_theta, u_phi = stable_orbit.four_velocity()
 
             python_trajectory = np.transpose(
-                np.apply_along_axis(lambda x: np.array([u_t(x),u_r(x),u_theta(x),u_phi(x)]),0,times)
+                np.apply_along_axis(
+                    lambda x: np.array([u_t(x), u_r(x), u_theta(x), u_phi(x)]), 0, times
                 )
-            
+            )
+
             for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
-                                  diff=np.max(np.abs(mathematica_trajectory[:,j]-python_trajectory[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(mathematica_trajectory[:,j],python_trajectory[:,j],atol=1e-6))
-    
+                with self.subTest(
+                    i=i,
+                    component=component,
+                    params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
+                    diff=np.max(
+                        np.abs(mathematica_trajectory[:, j] - python_trajectory[:, j])
+                    ),
+                ):
+                    self.assertTrue(
+                        np.allclose(
+                            mathematica_trajectory[:, j],
+                            python_trajectory[:, j],
+                            atol=1e-6,
+                        )
+                    )
+
     def test_norm(self):
-        times = np.linspace(0,10,10)
+        """
+        Check if the norm of the four-velocity is -1
+        """
+        times = np.linspace(0, 10, 10)
         # stable orbits
-        for i, orbit in enumerate(stable_orbit_values):
-            a,p,e,x = orbit
-            stable_orbit = StableOrbit(a,p,e,x)
+        for i, orbit in enumerate(stable_orbit_parameters):
+            a, p, e, x = orbit
+            stable_orbit = StableOrbit(a, p, e, x)
             norm = stable_orbit._four_velocity_norm()
-            for j, time in enumerate(times):
-                with self.subTest(i=i,
-                                params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
-                                norm = norm(time)
-                                ):
-                    self.assertTrue(abs(norm(time)+1)<1e-8)
+            for time in times:
+                with self.subTest(
+                    i=i,
+                    params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
+                    norm=norm(time),
+                ):
+                    self.assertTrue(abs(norm(time) + 1) < 1e-8)
 
         # plunging orbits
-        for i, orbit in enumerate(plunging_orbit_values):
-            a,E,L,Q = orbit
-            plunging_orbit = PlungingOrbit(a,E,L,Q)
+        for i, orbit in enumerate(plunging_orbit_parameters):
+            a, E, L, Q = orbit
+            plunging_orbit = PlungingOrbit(a, E, L, Q)
             norm = plunging_orbit._four_velocity_norm()
             for j, time in enumerate(times):
-                with self.subTest(i=i,
-                                params="a = {}, E = {}, L = {}, Q = {}".format(*orbit),
-                                norm = norm(time)
-                                ):
-                    self.assertTrue(abs(norm(time)+1)<1e-1)
+                with self.subTest(
+                    i=i,
+                    params="a = {}, E = {}, L = {}, Q = {}".format(*orbit),
+                    norm=norm(time),
+                ):
+                    self.assertTrue(abs(norm(time) + 1) < 1e-3)
 
     def test_using_numerical_differentiation(self):
-        components = ["ut","ur","utheta","uphi"]
+        """
+        Check that the four velocity computed using the geodesic equation matches with the
+        four velocity computed using numerical differentiation.
+        """
+        components = ["ut", "ur", "utheta", "uphi"]
 
-        #stable orbits
-        for i, orbit in enumerate(stable_orbit_values):
-            a,p,e,x = orbit
-            stable_orbit = StableOrbit(a,p,e,x)
+        # stable orbits
+        for i, orbit in enumerate(stable_orbit_parameters):
+            a, p, e, x = orbit
+            stable_orbit = StableOrbit(a, p, e, x)
             u_t, u_r, u_theta, u_phi = stable_orbit.four_velocity()
-            delta_t, delta_r, delta_theta, delta_phi = stable_orbit.numerical_four_velocity()
+            (
+                delta_t,
+                delta_r,
+                delta_theta,
+                delta_phi,
+            ) = stable_orbit.numerical_four_velocity()
 
             analytic_four_velocity = np.transpose(
-                np.apply_along_axis(lambda x: np.array([u_t(x),u_r(x),u_theta(x),u_phi(x)]),0,times)
+                np.apply_along_axis(
+                    lambda x: np.array([u_t(x), u_r(x), u_theta(x), u_phi(x)]), 0, times
                 )
-            
+            )
+
             numerical_four_velocity = np.transpose(
-                np.apply_along_axis(lambda x: np.array([delta_t(x),delta_r(x),delta_theta(x),delta_phi(x)]),0,times)
+                np.apply_along_axis(
+                    lambda x: np.array(
+                        [delta_t(x), delta_r(x), delta_theta(x), delta_phi(x)]
+                    ),
+                    0,
+                    times,
                 )
-            
+            )
+
             for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
-                                  diff=np.max(np.abs(analytic_four_velocity[:,j]-numerical_four_velocity[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(analytic_four_velocity[:,j],numerical_four_velocity[:,j],atol=1e-3))
-
-        #plunging orbits
-
-        # for i, orbit in enumerate(plunging_orbit_values):
-        #     a,E,L,Q = orbit
-        #     plunging_orbit = PlungingOrbit(a,E,L,Q)
-        #     u_t, u_r, u_theta, u_phi = plunging_orbit.four_velocity()
-        #     delta_t, delta_r, delta_theta, delta_phi = plunging_orbit.numerical_four_velocity()
-
-        #     analytic_four_velocity = np.transpose(
-        #         np.apply_along_axis(lambda x: np.array([u_t(x),u_r(x),u_theta(x),u_phi(x)]),0,times)
-        #         )
-            
-        #     numerical_four_velocity = np.transpose(
-        #         np.apply_along_axis(lambda x: np.array([delta_t(x),delta_r(x),delta_theta(x),delta_phi(x)]),0,times)
-        #         )
-            
-        #     for j, component in enumerate(components):
-        #         with self.subTest(i=i,
-        #                           component=component,
-        #                           params="a = {}, E = {}, L = {}, Q = {}".format(*orbit),
-        #                           diff=np.max(np.abs(analytic_four_velocity[:,j]-numerical_four_velocity[:,j]))
-        #                           ):
-        #             self.assertTrue(np.allclose(analytic_four_velocity[:,j],numerical_four_velocity[:,j],rtol=1e-3,atol=1e-1))
-    
+                with self.subTest(
+                    i=i,
+                    component=component,
+                    params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
+                    diff=np.max(
+                        np.abs(
+                            analytic_four_velocity[:, j] - numerical_four_velocity[:, j]
+                        )
+                    ),
+                ):
+                    self.assertTrue(
+                        np.allclose(
+                            analytic_four_velocity[:, j],
+                            numerical_four_velocity[:, j],
+                            atol=1e-3,
+                        )
+                    )
```

### Comparing `kerrgeopy-0.9.1/tests/test_plunging_solutions.py` & `kerrgeopy-0.9.2/tests/test_stable_solutions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,128 @@
 import unittest
 import numpy as np
-from kerrgeopy.plunge import *
+from kerrgeopy.stable import *
+from kerrgeopy.constants import stable_radial_roots, stable_polar_roots
 from pathlib import Path
 
 THIS_DIR = Path(__file__).parent
 
 DATA_DIR = THIS_DIR.parent / "tests/data"
 
-complex_orbit_values = np.genfromtxt(DATA_DIR / "plunging_orbit_parameters_complex.txt", delimiter=",")
-real_orbit_values = np.genfromtxt(DATA_DIR / "plunging_orbit_parameters_real.txt", delimiter=",")
-times = np.genfromtxt(DATA_DIR / "plunging_orbit_times.txt", delimiter=",")
-
-class TestPlungingSolutions(unittest.TestCase):
-    def test_integrals(self):
-        components = ["I_r","I_r2","I_r_plus","I_r_minus"]
-        for i, orbit in enumerate(complex_orbit_values):
-            mathematica_trajectory = np.genfromtxt(DATA_DIR / f"plunging_integrals/trajectory{i}.txt", delimiter=",")
-            
-            a,E,L,Q = orbit
-            I_r, I_r2, I_r_plus, I_r_minus = plunging_radial_integrals(a,E,L,Q)
-            upsilon_r, upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
 
-            python_trajectory = np.transpose(
-                np.apply_along_axis(lambda x: np.array([I_r(upsilon_r*x),I_r2(upsilon_r*x),I_r_plus(upsilon_r*x),I_r_minus(upsilon_r*x)]),0,times)
-                )
-            
-            for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, E = {}, L = {}, Q = {}".format(*orbit),
-                                  diff=np.max(np.abs(mathematica_trajectory[:,j]-python_trajectory[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(mathematica_trajectory[:,j],python_trajectory[:,j]))
-    
-    def test_solutions(self):
-        components = ["t_r","phi_r","t_theta","t_phi"]
-        for i, orbit in enumerate(complex_orbit_values):
-            mathematica_trajectory = np.genfromtxt(DATA_DIR / f"plunging_solutions/trajectory{i}.txt", delimiter=",")
-            
-            a,E,L,Q = orbit
-            r, t_r, phi_r = plunging_radial_solutions_complex(a,E,L,Q)
-            theta, t_theta, phi_theta = plunging_polar_solutions(a,E,L,Q)
-            upsilon_r, upsilon_theta = plunging_mino_frequencies(a,E,L,Q)
+orbit_parameters = np.genfromtxt(DATA_DIR / "stable_orbit_parameters.txt", delimiter=",")
+orbit_times = np.genfromtxt(DATA_DIR / "stable_orbit_times.txt", delimiter=",")
+
+
+class TestStableSolutions(unittest.TestCase):
+    def test_random(self):
+        """
+        Test trajectory deltas against Mathematica output for a random set of stable orbits.
+        """
+        components = ["t_r", "t_theta", "phi_r", "phi_theta"]
+
+        for i, orbit in enumerate(orbit_parameters):
+            mathematica_trajectory = np.genfromtxt(
+                DATA_DIR / f"stable_solutions/trajectory{i}.txt", delimiter=","
+            )
+
+            a, p, e, x = orbit
+            constants = constants_of_motion(*orbit)
+            radial_roots = stable_radial_roots(a, p, e, x, constants)
+            polar_roots = stable_polar_roots(a, p, e, x, constants)
+            r, t_r, phi_r = radial_solutions(a, constants, radial_roots)
+            theta, t_theta, phi_theta = polar_solutions(a, constants, polar_roots)
 
             python_trajectory = np.transpose(
-                np.apply_along_axis(lambda x: np.array([t_r(upsilon_r*x),phi_r(upsilon_r*x),t_theta(upsilon_theta*x),phi_theta(upsilon_theta*x)]),0,times)
-                )
-            
-            for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, E = {}, L = {}, Q = {}".format(*orbit),
-                                  diff=np.max(np.abs(mathematica_trajectory[:,j]-python_trajectory[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(mathematica_trajectory[:,j],python_trajectory[:,j]))
-
-    def test_orbit_complex(self):
-        components = ["t","r","theta","phi"]
-        for i, orbit in enumerate(complex_orbit_values):
-            mathematica_trajectory = np.genfromtxt(DATA_DIR / f"plunging_orbits_complex/trajectory{i}.txt", delimiter=",")
-            
-            a,E,L,Q = orbit
-            plunging_orbit = PlungingOrbit(a,E,L,Q)
-            t, r, theta, phi = plunging_orbit.trajectory(initial_phases=(0,0,-pi/2,0))
-            python_trajectory = np.transpose(
-                np.apply_along_axis(lambda x: np.array([t(x),r(x),theta(x),phi(x)]),0,times)
+                np.apply_along_axis(
+                    lambda x: np.array([t_r(x), t_theta(x), phi_r(x), phi_theta(x)]),
+                    0,
+                    orbit_times,
                 )
-            
+            )
+
             for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, E = {}, L = {}, Q = {}".format(*orbit),
-                                  diff=np.max(np.abs(mathematica_trajectory[:,j]-python_trajectory[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(mathematica_trajectory[:,j],python_trajectory[:,j]))
-
-    def test_orbit_real(self):
-        components = ["t","r","theta","phi"]
-        for i, orbit in enumerate(real_orbit_values):
-            mathematica_trajectory = np.genfromtxt(DATA_DIR / f"plunging_orbits_real/trajectory{i}.txt", delimiter=",")
-            
-            a,E,L,Q = orbit
-            plunging_orbit = PlungingOrbit(a,E,L,Q)
-            t, r, theta, phi = plunging_orbit.trajectory(initial_phases=(0,0,-pi/2,0))
+                with self.subTest(
+                    i=i,
+                    component=component,
+                    params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
+                    diff=np.max(
+                        np.abs(mathematica_trajectory[:, j] - python_trajectory[:, j])
+                    ),
+                ):
+                    self.assertTrue(
+                        np.allclose(
+                            mathematica_trajectory[:, j], python_trajectory[:, j]
+                        )
+                    )
+
+
+class TestStableOrbit(unittest.TestCase):
+    def test_extreme_kerr(self):
+        """
+        Test that a ValueError is raised when a = 1.
+        """
+        with self.assertRaises(ValueError):
+            StableOrbit(1, 12, 0.5, 0.5)
+
+    def test_polar(self):
+        """
+        Test that a ValueError is raised when x = 0.
+        """
+        with self.assertRaises(ValueError):
+            StableOrbit(0.5, 12, 0.5, 0)
+
+    def test_marginally_bound(self):
+        """
+        Test that a ValueError is raised when e = 1
+        """
+        with self.assertRaises(ValueError):
+            StableOrbit(0.5, 12, 1, 0.5)
+
+    def test_invalid_arguments(self):
+        """
+        Test that a ValueError is raised for invalid arguments.
+        """
+        with self.assertRaises(ValueError):
+            StableOrbit(2, 5, 0.5, 0.5)
+        with self.assertRaises(ValueError):
+            StableOrbit(0.5, 5, -0.5, 0.5)
+
+    def test_unstable(self):
+        """
+        Test that a ValueError is raised when p is < separatrix(a,e,x)
+        """
+        with self.assertRaises(ValueError):
+            StableOrbit(0.5, 5, 0.5, 0.5)
+
+    def test_random(self):
+        """
+        Test the trajectory method against Mathematica output for a random set of stable orbits.
+        """
+        components = ["t", "r", "theta", "phi"]
+
+        for i, orbit in enumerate(orbit_parameters):
+            mathematica_trajectory = np.genfromtxt(
+                DATA_DIR / f"stable_orbits/trajectory{i}.txt", delimiter=","
+            )
+            test_orbit = StableOrbit(*orbit)
+            t, r, theta, phi = test_orbit.trajectory()
             python_trajectory = np.transpose(
-                np.apply_along_axis(lambda x: np.array([t(x),r(x),theta(x),phi(x)]),0,times)
+                np.apply_along_axis(
+                    lambda x: np.array([t(x), r(x), theta(x), phi(x)]), 0, orbit_times
                 )
-            
+            )
+
             for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, E = {}, L = {}, Q = {}".format(*orbit),
-                                  diff=np.max(np.abs(mathematica_trajectory[:,j]-python_trajectory[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(mathematica_trajectory[:,j],python_trajectory[:,j]))
+                with self.subTest(
+                    i=i,
+                    component=component,
+                    params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
+                    diff=np.max(
+                        np.abs(mathematica_trajectory[:, j] - python_trajectory[:, j])
+                    ),
+                ):
+                    self.assertTrue(
+                        np.allclose(
+                            mathematica_trajectory[:, j], python_trajectory[:, j]
+                        )
+                    )
```

### Comparing `kerrgeopy-0.9.1/tests/test_stable_solutions.py` & `kerrgeopy-0.9.2/tests/test_constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,106 @@
 import unittest
 import numpy as np
-from kerrgeopy.stable import *
-from kerrgeopy.constants import stable_radial_roots, stable_polar_roots
+from kerrgeopy.constants import *
 from pathlib import Path
 
 THIS_DIR = Path(__file__).parent
 
 DATA_DIR = THIS_DIR.parent / "tests/data"
 
 
-orbit_values = np.genfromtxt(DATA_DIR / "stable_orbit_parameters.txt", delimiter=",")
-orbit_times = np.genfromtxt(DATA_DIR / "stable_orbit_times.txt", delimiter=",")
+class TestConstants(unittest.TestCase):
+    def test_extreme_kerr(self):
+        """
+        Test that a ValueError is raised when a = 1.
+        """
+        with self.assertRaises(ValueError):
+            constants_of_motion(1, 12, 0.5, 0.5)
+        with self.assertRaises(ValueError):
+            energy(1, 0.5, 12, 0.5)
+        with self.assertRaises(ValueError):
+            angular_momentum(1, 0.5, 12, 0.5)
+        with self.assertRaises(ValueError):
+            carter_constant(1, 0.5, 12, 0.5)
 
-class TestStableSolutions(unittest.TestCase):
-    def test_random(self):
-        components = ["t_r","t_theta","phi_r","phi_theta"]
-
-        for i, orbit in enumerate(orbit_values):
-            mathematica_trajectory = np.genfromtxt(DATA_DIR / f"stable_solutions/trajectory{i}.txt", delimiter=",")
-            
-            a,p,e,x = orbit
-            constants = constants_of_motion(*orbit)
-            radial_roots = stable_radial_roots(a,p,e,x,constants)
-            polar_roots = stable_polar_roots(a,p,e,x,constants)
-            r, t_r, phi_r = radial_solutions(a,constants,radial_roots)
-            theta, t_theta, phi_theta = polar_solutions(a,constants,polar_roots)
+    def test_unstable(self):
+        """
+        Test that a ValueError is raised when p is < separatrix(a,e,x)
+        """
+        with self.assertRaises(ValueError):
+            constants_of_motion(0.5, 5, 0.5, 0.5)
+        with self.assertRaises(ValueError):
+            energy(0.5, 5, 0.5, 0.5)
+        with self.assertRaises(ValueError):
+            angular_momentum(0.5, 5, 0.5, 0.5)
+        with self.assertRaises(ValueError):
+            carter_constant(0.5, 5, 0.5, 0.5)
 
-            python_trajectory = np.transpose(
-                np.apply_along_axis(lambda x: np.array([t_r(x),t_theta(x),phi_r(x),phi_theta(x)]),0,orbit_times)
+    def test_invalid_arguments(self):
+        """
+        Test that a ValueError is raised for invalid arguments.
+        """
+        with self.assertRaises(ValueError):
+            constants_of_motion(2, 5, 0.5, 0.5)
+        with self.assertRaises(ValueError):
+            energy(0.5, 5, 2, 0.5)
+        with self.assertRaises(ValueError):
+            angular_momentum(0.5, 5, 0.5, 2)
+        with self.assertRaises(ValueError):
+            carter_constant(-0.5, 5, -0.5, 0.5)
+
+    def test_constants_random(self):
+        """
+        Test constants_of_motion method against output from the KerrGeodesics
+        Mathematica library for a random set of orbits.
+        """
+        parameters = np.genfromtxt(DATA_DIR / "const_parameters.txt", delimiter=",")
+        mathematica_const_output = np.genfromtxt(
+            DATA_DIR / "mathematica_const_output.txt"
+        )
+        python_const_output = np.apply_along_axis(
+            lambda x: constants_of_motion(*x), 1, parameters
+        )
+
+        for i, params in enumerate(parameters):
+            with self.subTest(i=i, params=params):
+                self.assertTrue(
+                    np.allclose(mathematica_const_output[i], python_const_output[i])
                 )
-            
-            for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
-                                  diff=np.max(np.abs(mathematica_trajectory[:,j]-python_trajectory[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(mathematica_trajectory[:,j],python_trajectory[:,j]))
-
-class TestStableOrbit(unittest.TestCase):
-    def test_extreme_kerr(self):
-        with self.assertRaises(ValueError): StableOrbit(1,12,0.5,0.5)
 
-    def test_polar(self):
-        with self.assertRaises(ValueError): StableOrbit(0.5,12,0.5,0)
 
-    def test_marginally_bound(self):
-        with self.assertRaises(ValueError): StableOrbit(0.5,12,1,0.5)
+class TestSeparatrix(unittest.TestCase):
+    def test_extreme_kerr(self):
+        """
+        Test that a ValueError is raised when a = 1.
+        """
+        with self.assertRaises(ValueError):
+            separatrix(1, 0.5, 0.5)
 
     def test_invalid_arguments(self):
-        with self.assertRaises(ValueError): StableOrbit(2,5,0.5,0.5)
-        with self.assertRaises(ValueError): StableOrbit(0.5,5,-0.5,0.5)
-
-    def test_unstable(self):
-        with self.assertRaises(ValueError): StableOrbit(0.5,5,0.5,0.5)
-
-    def test_random(self):
-        components = ["t","r","theta","phi"]
-        
-        for i, orbit in enumerate(orbit_values):
-            mathematica_trajectory = np.genfromtxt(DATA_DIR / f"stable_orbits/trajectory{i}.txt", delimiter=",")
-            test_orbit = StableOrbit(*orbit)
-            t, r , theta, phi = test_orbit.trajectory()
-            python_trajectory = np.transpose(
-                np.apply_along_axis(lambda x: np.array([t(x),r(x),theta(x),phi(x)]),0,orbit_times)
+        """
+        Test that a ValueError is raised for invalid arguments.
+        """
+        with self.assertRaises(ValueError):
+            separatrix(2, -0.5, -0.5)
+
+    def test_separatrix_random(self):
+        """
+        Test separatrix method against output from the KerrGeodesics
+        Mathematica library for a random set of inputs.
+        """
+        sep_parameters = np.genfromtxt(
+            DATA_DIR / "separatrix_parameters.txt", delimiter=","
+        )
+        mathematica_separatrix_output = np.genfromtxt(
+            DATA_DIR / "mathematica_separatrix_output.txt"
+        )
+        python_separatrix_output = np.apply_along_axis(
+            lambda x: separatrix(*x), 1, sep_parameters
+        )
+        for i, params in enumerate(sep_parameters):
+            with self.subTest(i=i, params=params):
+                self.assertTrue(
+                    np.allclose(
+                        python_separatrix_output[i], mathematica_separatrix_output[i]
+                    )
                 )
-            
-            for j, component in enumerate(components):
-                with self.subTest(i=i,
-                                  component=component,
-                                  params="a = {}, p = {}, e = {}, x = {}".format(*orbit),
-                                  diff=np.max(np.abs(mathematica_trajectory[:,j]-python_trajectory[:,j]))
-                                  ):
-                    self.assertTrue(np.allclose(mathematica_trajectory[:,j],python_trajectory[:,j]))
```

