# Comparing `tmp/concreteproperties-0.6.2.tar.gz` & `tmp/concreteproperties-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concreteproperties-0.6.2.tar", max compression
+gzip compressed data, was "concreteproperties-0.6.3.tar", max compression
```

## Comparing `concreteproperties-0.6.2.tar` & `concreteproperties-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1074 2024-03-08 06:50:14.958652 concreteproperties-0.6.2/LICENSE
--rw-r--r--   0        0        0     4175 2024-03-08 06:50:14.958652 concreteproperties-0.6.2/README.md
--rw-r--r--   0        0        0     2807 2024-03-08 06:50:29.382560 concreteproperties-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      939 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/__init__.py
--rw-r--r--   0        0        0      226 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/__main__.py
--rw-r--r--   0        0        0    23272 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/analysis_section.py
--rw-r--r--   0        0        0    82847 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/concrete_section.py
--rw-r--r--   0        0        0      163 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/design_codes/__init__.py
--rw-r--r--   0        0        0    22438 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/design_codes/as3600.py
--rw-r--r--   0        0        0     7075 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/design_codes/design_code.py
--rw-r--r--   0        0        0    82369 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/design_codes/nzs3101.py
--rw-r--r--   0        0        0     5922 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/material.py
--rw-r--r--   0        0        0     3097 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/post.py
--rw-r--r--   0        0        0    15006 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/pre.py
--rw-r--r--   0        0        0    36135 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/prestressed_section.py
--rw-r--r--   0        0        0        0 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/py.typed
--rw-r--r--   0        0        0    52996 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/results.py
--rw-r--r--   0        0        0    48457 2024-03-08 06:50:14.994652 concreteproperties-0.6.2/src/concreteproperties/stress_strain_profile.py
--rw-r--r--   0        0        0    16551 2024-03-08 06:50:14.998652 concreteproperties-0.6.2/src/concreteproperties/utils.py
--rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 concreteproperties-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-27 14:15:53.473051 concreteproperties-0.6.3/LICENSE
+-rw-r--r--   0        0        0     4175 2024-05-27 14:15:53.473051 concreteproperties-0.6.3/README.md
+-rw-r--r--   0        0        0     2887 2024-05-27 14:16:02.241038 concreteproperties-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      940 2024-05-27 14:15:53.509051 concreteproperties-0.6.3/src/concreteproperties/__init__.py
+-rw-r--r--   0        0        0      227 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/__main__.py
+-rw-r--r--   0        0        0    23272 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/analysis_section.py
+-rw-r--r--   0        0        0    82809 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/concrete_section.py
+-rw-r--r--   0        0        0      164 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/design_codes/__init__.py
+-rw-r--r--   0        0        0    22438 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/design_codes/as3600.py
+-rw-r--r--   0        0        0     7075 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/design_codes/design_code.py
+-rw-r--r--   0        0        0    82381 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/design_codes/nzs3101.py
+-rw-r--r--   0        0        0     5922 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/material.py
+-rw-r--r--   0        0        0     3097 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/post.py
+-rw-r--r--   0        0        0    15086 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/pre.py
+-rw-r--r--   0        0        0    36135 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/prestressed_section.py
+-rw-r--r--   0        0        0        0 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/py.typed
+-rw-r--r--   0        0        0    53026 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/results.py
+-rw-r--r--   0        0        0    48458 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/stress_strain_profile.py
+-rw-r--r--   0        0        0    16551 2024-05-27 14:15:53.513051 concreteproperties-0.6.3/src/concreteproperties/utils.py
+-rw-r--r--   0        0        0     5980 1970-01-01 00:00:00.000000 concreteproperties-0.6.3/PKG-INFO
```

### Comparing `concreteproperties-0.6.2/LICENSE` & `concreteproperties-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/README.md` & `concreteproperties-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/pyproject.toml` & `concreteproperties-0.6.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "concreteproperties"
-version = "0.6.2"
+version = "0.6.3"
 description = "A python package to determine cross-section propreties of reinforced concrete sections."
 license = "MIT"
 authors = [
     "Robbie van Leeuwen <robbie.vanleeuwen@gmail.com>",
 ]
 maintainers = [
     "Robbie van Leeuwen <robbie.vanleeuwen@gmail.com>",
@@ -28,65 +28,66 @@
     "Topic :: Scientific/Engineering",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "concreteproperties", from = "src" },
     { include = "src/concreteproperties/py.typed"},
 ]
 include = []
 
 [tool.poetry.urls]
 Changelog = "https://github.com/robbievanleeuwen/concrete-properties/releases"
 "Bug Tracker" = "https://github.com/robbievanleeuwen/concrete-properties/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.9.0,<3.12"
-numpy = "^1.24.0"
-scipy = "^1.10.0"
-matplotlib = "^3.8.2"
-shapely = "^2.0.2"
+python = ">=3.9.0,<3.13"
+numpy = "^1.26.4"
+scipy = "^1.12.0"
+matplotlib = "^3.8.3"
+shapely = "^2.0.3"
 triangle = "^20230923"
-rich = "^13.7.0"
+rich = "^13.7.1"
 click = "^8.1.7"
-more-itertools = "^10.0.0"
-sectionproperties = "^3.1.2"
+more-itertools = "^10.2.0"
+sectionproperties = "^3.2.2"
 
 [tool.poetry.dev-dependencies]
-black = "^23.10.1"
-coverage = { extras = ["toml"], version = "^7.3.3" }
+black = "^24.2.0"
+coverage = { extras = ["toml"], version = "^7.4.3" }
 darglint = "^1.8.1"
-flake8 = "^6.1.0"
-flake8-bugbear = "^23.12.2"
+flake8 = "^7.0.0"
+flake8-bugbear = "^24.2.6"
 flake8-docstrings = "^1.7.0"
 flake8-rst-docstrings = "^0.3.0"
 flake8-pytest-style = "^1.7.2"
-furo = "^2023.9.10"
-ipykernel = "^6.27.1"
-ipython = "^8.18.1"
-ipywidgets = "^8.1.1"
+furo = "^2024.01.29"
+ipykernel = "^6.29.3"
+ipython = "^8.18.1"  # 8.19 and above drops 3.9 support
+ipywidgets = "^8.1.2"
 isort = "^5.13.2"
-nbconvert = "^7.13.0"
+nbconvert = "^7.16.2"
 nbsphinx = "^0.9.3"
-notebook = "^7.0.6"
+notebook = "^7.1.1"
 pep8-naming = "^0.13.3"
-pre-commit = "^3.6.0"
+pre-commit = "^3.6.2"
 pre-commit-hooks = "^4.5.0"
 Pygments = "^2.17.2"
-pytest = "^7.4.3"
-pyupgrade = "^3.15.0"
+pytest = "^8.0.2"
+pyupgrade = "^3.15.1"
 sphinx = "^7.2.6"
-sphinx-autobuild = "^2021.3.14"
+sphinx-autobuild = "^2024.2.4"
 sphinx-click = "^5.1.0"
 sphinx-copybutton = "^0.5.2"
-sphinxext-opengraph = "^0.8.2"
+sphinxext-opengraph = "^0.9.1"
 
 [tool.poetry.scripts]
 concreteproperties = "concreteproperties.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
```

### Comparing `concreteproperties-0.6.2/src/concreteproperties/__init__.py` & `concreteproperties-0.6.3/src/concreteproperties/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """concreteproperties.
 
 A python package to calculate the section properties of arbitrary reinforced and
 prestressed concrete sections.
 """
+
 # analysis
 from concreteproperties.concrete_section import ConcreteSection
 
 # materials
 from concreteproperties.material import Concrete, Steel, SteelBar, SteelStrand
 
 # geometry
```

### Comparing `concreteproperties-0.6.2/src/concreteproperties/analysis_section.py` & `concreteproperties-0.6.3/src/concreteproperties/analysis_section.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/src/concreteproperties/concrete_section.py` & `concreteproperties-0.6.3/src/concreteproperties/concrete_section.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,17 +659,15 @@
                 except ValueError as exc:
                     if not moment_curvature._failure:
                         msg = "Analysis failed. Please raise an issue at "
                         msg += "https://github.com/robbievanleeuwen/concrete-properties"
                         msg += "/issues"
                         raise utils.AnalysisError(msg) from exc
 
-                m_xy = np.sqrt(
-                    moment_curvature._m_x_i**2 + moment_curvature._m_y_i**2
-                )
+                m_xy = np.sqrt(moment_curvature._m_x_i**2 + moment_curvature._m_y_i**2)
 
                 if progress:
                     text_update = "[red]Generating M-K diagram: "
                     text_update += f"M={m_xy:.3e}"
                     progress.update(task, description=text_update)
 
                 # save results
```

### Comparing `concreteproperties-0.6.2/src/concreteproperties/design_codes/as3600.py` & `concreteproperties-0.6.3/src/concreteproperties/design_codes/as3600.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/src/concreteproperties/design_codes/design_code.py` & `concreteproperties-0.6.3/src/concreteproperties/design_codes/design_code.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/src/concreteproperties/design_codes/nzs3101.py` & `concreteproperties-0.6.3/src/concreteproperties/design_codes/nzs3101.py`

 * *Files 0% similar despite different names*

```diff
@@ -722,23 +722,23 @@
         # determine NZS3101:2006 maximum tension and compression capacity
         max_ten = -self.max_ten_strength(os_design, prob_design)
         max_comp = self.max_comp_strength(cpe_design, os_design, prob_design)
 
         # compare to axial load
         if n_design < phi * max_ten:
             raise ValueError(
-                f"The specified axial load of {n_design*n_scale:.2f} kN, is less than "
-                f"the tension capacity of the concrete section, phiN_t = "
-                f"{phi*max_ten*n_scale:.2f} kN"
+                f"The specified axial load of {n_design * n_scale:.2f} kN, is less "
+                f"than the tension capacity of the concrete section, phiN_t = "
+                f"{phi * max_ten * n_scale:.2f} kN"
             )
         elif n_design > phi * max_comp:
             raise ValueError(
-                f"The specified axial load of {n_design*n_scale:.2f} kN, is greater "
+                f"The specified axial load of {n_design * n_scale:.2f} kN, is greater "
                 f"than the compression capacity of the concrete section, phiN_c = "
-                f"{phi*max_comp*n_scale:.2f} kN"
+                f"{phi * max_comp * n_scale:.2f} kN"
             )
 
     def check_f_y_limit(self) -> None:
         """Checks the reinforcement strenghts are within limits.
 
         Checks that the specified steel reinforcement strengths for all defined
         steel geometries comply with NZS3101:2006 CL 5.3.3.
```

### Comparing `concreteproperties-0.6.2/src/concreteproperties/material.py` & `concreteproperties-0.6.3/src/concreteproperties/material.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/src/concreteproperties/post.py` & `concreteproperties-0.6.3/src/concreteproperties/post.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/src/concreteproperties/pre.py` & `concreteproperties-0.6.3/src/concreteproperties/pre.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,23 +207,27 @@
             polys = [self.geom]
 
         # sort geometries
         top_polys, bot_polys = self.sort_polys(polys=polys, point=point, vector=vector)
 
         # assign material properties and create cp geometry objects
         top_geoms = [
-            CPGeomConcrete(geom=poly, material=self.material)
-            if isinstance(self.material, Concrete)
-            else CPGeom(geom=poly, material=self.material)
+            (
+                CPGeomConcrete(geom=poly, material=self.material)
+                if isinstance(self.material, Concrete)
+                else CPGeom(geom=poly, material=self.material)
+            )
             for poly in top_polys
         ]
         bot_geoms = [
-            CPGeomConcrete(geom=poly, material=self.material)
-            if isinstance(self.material, Concrete)
-            else CPGeom(geom=poly, material=self.material)
+            (
+                CPGeomConcrete(geom=poly, material=self.material)
+                if isinstance(self.material, Concrete)
+                else CPGeom(geom=poly, material=self.material)
+            )
             for poly in bot_polys
         ]
 
         # ensure top geoms is in compression
         if theta <= np.pi / 2 and theta >= -np.pi / 2:
             return top_geoms, bot_geoms
         else:
```

### Comparing `concreteproperties-0.6.2/src/concreteproperties/prestressed_section.py` & `concreteproperties-0.6.3/src/concreteproperties/prestressed_section.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/src/concreteproperties/results.py` & `concreteproperties-0.6.3/src/concreteproperties/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import warnings
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
-import matplotlib.cm as cm
+import matplotlib
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import matplotlib.tri as tri
 import numpy as np
 from matplotlib.collections import PatchCollection
 from matplotlib.colors import CenteredNorm
 from rich.console import Console
@@ -272,14 +272,15 @@
     :meth:`~concreteproperties.results.CrackedResults.calculate_transformed_properties`
     method.
 
     Args:
         theta: Angle (in radians) the neutral axis makes with the horizontal axis
             (:math:`-\pi \leq \theta \leq \pi`)
     """
+
     theta: float
     n: float = 0
     m: float = 0
     m_cr: float | tuple[float, float] = 0
     d_nc: float = 0
     cracked_geometries: list[CPGeom] = field(default_factory=list, repr=False)
     e_a_cr: float = 0
@@ -457,14 +458,15 @@
         m_xy: List of resultant bending moments
         failure_geometry: Geometry object of the region of the cross-section that
             failed, ending the moment curvature analysis
         convergence: The critical ratio between the strain and the failure strain within
             the cross-section for each curvature step in the analysis. A value of one
             indicates failure.
     """
+
     # results
     theta: float
     n_target: float
     kappa: list[float] = field(default_factory=list)
     n: list[float] = field(default_factory=list)
     m_x: list[float] = field(default_factory=list)
     m_y: list[float] = field(default_factory=list)
@@ -614,14 +616,15 @@
         k_u: Neutral axis parameter *(d_n / d)*
         n: Resultant axial force
         m_x: Resultant bending moment about the x-axis
         m_y: Resultant bending moment about the y-axis
         m_xy: Resultant bending moment
         label: Result label
     """
+
     # bending angle
     theta: float
 
     # ultimate neutral axis depth
     d_n: float = 0
     k_u: float = 0
 
@@ -1168,16 +1171,16 @@
 
             # plot background
             self.concrete_section.plot_section(
                 background=True, **dict(kwargs, ax=fig.axes[0])
             )
 
             # set up the colormaps
-            cmap_conc = cm.get_cmap(name=conc_cmap)
-            cmap_reinf = cm.get_cmap(name=reinf_cmap)
+            cmap_conc = matplotlib.colormaps.get_cmap(cmap=conc_cmap)
+            cmap_reinf = matplotlib.colormaps.get_cmap(cmap=reinf_cmap)
 
             # determine minimum and maximum stress values for the contour list
             # add tolerance for plotting stress blocks
             conc_sig_min = min([min(x) for x in self.concrete_stresses]) - 1e-12
             conc_sig_max = max([max(x) for x in self.concrete_stresses]) + 1e-12
 
             # if there is meshed reinforcement, calculate min and max
```

### Comparing `concreteproperties-0.6.2/src/concreteproperties/stress_strain_profile.py` & `concreteproperties-0.6.3/src/concreteproperties/stress_strain_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,14 +592,15 @@
             reinforcement material within the concrete cross section should also be
             defined with the same limit for the fracture strain
         n_confinement: Modifier for volumetric ratio of confinement reinforcement
 
     Raises:
         ValueError: If specified section type is not rect, circ_hoop or circ_spiral
     """
+
     strains: list[float] = field(init=False)
     stresses: list[float] = field(init=False)
     elastic_modulus: float
     ultimate_strain: float = field(init=False, default=0)
     compressive_strength: float
     tensile_strength: float
     sect_type: str | None = None
```

### Comparing `concreteproperties-0.6.2/src/concreteproperties/utils.py` & `concreteproperties-0.6.3/src/concreteproperties/utils.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.6.2/PKG-INFO` & `concreteproperties-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: concreteproperties
-Version: 0.6.2
+Version: 0.6.3
 Summary: A python package to determine cross-section propreties of reinforced concrete sections.
 Home-page: https://github.com/robbievanleeuwen/concrete-properties
 License: MIT
 Keywords: concrete,reinforced-concrete,prestressed-concrete,post-tensioned-concrete,cross-section,structural-engineering,finite-element-analysis,computational-mechanics
 Author: Robbie van Leeuwen
 Author-email: robbie.vanleeuwen@gmail.com
 Maintainer: Robbie van Leeuwen
 Maintainer-email: robbie.vanleeuwen@gmail.com
-Requires-Python: >=3.9.0,<3.12
+Requires-Python: >=3.9.0,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
-Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
-Requires-Dist: scipy (>=1.10.0,<2.0.0)
-Requires-Dist: sectionproperties (>=3.1.2,<4.0.0)
-Requires-Dist: shapely (>=2.0.2,<3.0.0)
+Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
+Requires-Dist: more-itertools (>=10.2.0,<11.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: scipy (>=1.12.0,<2.0.0)
+Requires-Dist: sectionproperties (>=3.2.2,<4.0.0)
+Requires-Dist: shapely (>=2.0.3,<3.0.0)
 Requires-Dist: triangle (>=20230923,<20230924)
 Project-URL: Bug Tracker, https://github.com/robbievanleeuwen/concrete-properties/issues
 Project-URL: Changelog, https://github.com/robbievanleeuwen/concrete-properties/releases
 Project-URL: Documentation, https://concrete-properties.readthedocs.io
 Project-URL: Repository, https://github.com/robbievanleeuwen/concrete-properties
 Description-Content-Type: text/markdown
```

