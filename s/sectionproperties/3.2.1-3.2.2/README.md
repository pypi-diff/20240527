# Comparing `tmp/sectionproperties-3.2.1.tar.gz` & `tmp/sectionproperties-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sectionproperties-3.2.1.tar", max compression
+gzip compressed data, was "sectionproperties-3.2.2.tar", max compression
```

## Comparing `sectionproperties-3.2.1.tar` & `sectionproperties-3.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1074 2024-04-15 00:54:11.020640 sectionproperties-3.2.1/LICENSE
--rw-r--r--   0        0        0     4155 2024-04-15 00:54:11.020640 sectionproperties-3.2.1/README.md
--rw-r--r--   0        0        0     4386 2024-04-15 00:54:21.876767 sectionproperties-3.2.1/pyproject.toml
--rw-r--r--   0        0        0      353 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/__init__.py
--rw-r--r--   0        0        0      225 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/__main__.py
--rw-r--r--   0        0        0       97 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/__init__.py
--rw-r--r--   0        0        0    40040 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/fea.py
--rw-r--r--   0        0        0    15869 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/plastic_section.py
--rw-r--r--   0        0        0   126376 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/section.py
--rw-r--r--   0        0        0     5423 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/analysis/solver.py
--rw-r--r--   0        0        0       40 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/__init__.py
--rw-r--r--   0        0        0     6406 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/fibre.py
--rw-r--r--   0        0        0    31352 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/post.py
--rw-r--r--   0        0        0    40740 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/post/stress_post.py
--rw-r--r--   0        0        0      157 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/__init__.py
--rw-r--r--   0        0        0     3718 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/bisect_section.py
--rw-r--r--   0        0        0   106318 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/geometry.py
--rw-r--r--   0        0        0     1486 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/__init__.py
--rw-r--r--   0        0        0     8677 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/bridge_sections.py
--rw-r--r--   0        0        0    23678 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/concrete_sections.py
--rw-r--r--   0        0        0    46245 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/nastran_sections.py
--rw-r--r--   0        0        0     9883 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/primitive_sections.py
--rw-r--r--   0        0        0    49709 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/steel_sections.py
--rw-r--r--   0        0        0     1781 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/library/utils.py
--rw-r--r--   0        0        0     5020 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/pre.py
--rw-r--r--   0        0        0     5041 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/pre/rhino.py
--rw-r--r--   0        0        0        0 2024-04-15 00:54:11.040640 sectionproperties-3.2.1/src/sectionproperties/py.typed
--rw-r--r--   0        0        0    22125 2024-04-15 00:54:11.044640 sectionproperties-3.2.1/tests/geometry/complex_shape.txt
--rw-r--r--   0        0        0    24105 2024-04-15 00:54:11.044640 sectionproperties-3.2.1/tests/geometry/compound_shape.txt
--rw-r--r--   0        0        0     6505 1970-01-01 00:00:00.000000 sectionproperties-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-27 05:31:18.701929 sectionproperties-3.2.2/LICENSE
+-rw-r--r--   0        0        0     4140 2024-05-27 05:31:18.701929 sectionproperties-3.2.2/README.md
+-rw-r--r--   0        0        0     4393 2024-05-27 05:31:27.505854 sectionproperties-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0      353 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/__main__.py
+-rw-r--r--   0        0        0       97 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/analysis/__init__.py
+-rw-r--r--   0        0        0    40040 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/analysis/fea.py
+-rw-r--r--   0        0        0    15869 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/analysis/plastic_section.py
+-rw-r--r--   0        0        0   126376 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/analysis/section.py
+-rw-r--r--   0        0        0     5423 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/analysis/solver.py
+-rw-r--r--   0        0        0       40 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/post/__init__.py
+-rw-r--r--   0        0        0     6406 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/post/fibre.py
+-rw-r--r--   0        0        0    31352 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/post/post.py
+-rw-r--r--   0        0        0    40740 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/post/stress_post.py
+-rw-r--r--   0        0        0      157 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/pre/__init__.py
+-rw-r--r--   0        0        0     3718 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/pre/bisect_section.py
+-rw-r--r--   0        0        0   106318 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/pre/geometry.py
+-rw-r--r--   0        0        0     1486 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/pre/library/__init__.py
+-rw-r--r--   0        0        0     8677 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/pre/library/bridge_sections.py
+-rw-r--r--   0        0        0    23678 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/pre/library/concrete_sections.py
+-rw-r--r--   0        0        0    46245 2024-05-27 05:31:18.717929 sectionproperties-3.2.2/src/sectionproperties/pre/library/nastran_sections.py
+-rw-r--r--   0        0        0     9883 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/src/sectionproperties/pre/library/primitive_sections.py
+-rw-r--r--   0        0        0    49886 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/src/sectionproperties/pre/library/steel_sections.py
+-rw-r--r--   0        0        0     1781 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/src/sectionproperties/pre/library/utils.py
+-rw-r--r--   0        0        0     5020 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/src/sectionproperties/pre/pre.py
+-rw-r--r--   0        0        0     5041 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/src/sectionproperties/pre/rhino.py
+-rw-r--r--   0        0        0        0 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/src/sectionproperties/py.typed
+-rw-r--r--   0        0        0    22125 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/tests/geometry/complex_shape.txt
+-rw-r--r--   0        0        0    24105 2024-05-27 05:31:18.721929 sectionproperties-3.2.2/tests/geometry/compound_shape.txt
+-rw-r--r--   0        0        0     6403 1970-01-01 00:00:00.000000 sectionproperties-3.2.2/PKG-INFO
```

### Comparing `sectionproperties-3.2.1/LICENSE` & `sectionproperties-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/README.md` & `sectionproperties-3.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 </picture>
 
 [![PyPI](https://img.shields.io/pypi/v/sectionproperties.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/sectionproperties.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/sectionproperties)][python version]
 [![License](https://img.shields.io/pypi/l/sectionproperties)][license]
 [![Read the documentation at https://sectionproperties.readthedocs.io/](https://img.shields.io/readthedocs/sectionproperties/stable.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/robbievanleeuwen/section-properties/workflows/Tests/badge.svg)][tests]
+[![Tests](https://github.com/robbievanleeuwen/section-properties/actions/workflows/tests.yml/badge.svg?branch=master)][tests]
 [![Codecov](https://codecov.io/gh/robbievanleeuwen/section-properties/branch/master/graph/badge.svg)][codecov]
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-[![JOSS](https://joss.theoj.org/papers/6c3ad57a38202562726b4a7b86a86c32/status.svg)][joss]
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06105/status.svg)][joss]
 
 [pypi_]: https://pypi.org/project/sectionproperties/
 [status]: https://pypi.org/project/sectionproperties/
 [python version]: https://pypi.org/project/sectionproperties
 [read the docs]: https://sectionproperties.readthedocs.io/
 [tests]: https://github.com/robbievanleeuwen/section-properties/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/robbievanleeuwen/section-properties
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
-[joss]: https://joss.theoj.org/papers/6c3ad57a38202562726b4a7b86a86c32
+[joss]: https://doi.org/10.21105/joss.06105
 
 `sectionproperties` is a python package for the analysis of arbitrary cross-sections
 using the finite element method. `sectionproperties` can be used to determine
 section properties to be used in structural design and visualise cross-sectional
 stresses resulting from combinations of applied forces and bending moments.
 
 [Subscribe](http://eepurl.com/dMMUeg) to the `sectionproperties` mailing list!
```

### Comparing `sectionproperties-3.2.1/pyproject.toml` & `sectionproperties-3.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sectionproperties"
-version = "3.2.1"
+version = "3.2.2"
 description = "A python package for the analysis of arbitrary cross-sections using the finite element method."
 license = "MIT"
 authors = [
     "Robbie van Leeuwen <robbie.vanleeuwen@gmail.com>",
 ]
 maintainers = [
     "Robbie van Leeuwen <robbie.vanleeuwen@gmail.com>",
@@ -55,19 +55,20 @@
 shapely = "^2.0.3"
 triangle = "^20230923"
 rich = "^13.7.1"
 click = "^8.1.7"
 more-itertools = "^10.2.0"
 numba = { version = "^0.59.0", optional = true }
 cad-to-shapely = { version = "^0.3.1", optional = true }
-rhino-shapley-interop = { version = "^0.0.4", python = ">=3.9.0,<3.12", optional = true }
-rhino3dm = { version = "^8.4.0", python = ">=3.9.0,<3.12", optional = true }
+rhino-shapley-interop = { version = "^0.0.4", optional = true }
+rhino3dm = { version = "==8.6.0", optional = true }
 pypardiso = { version = "^0.4.5", optional = true }
 intel-openmp = { version = "==2023.2.0", optional = true }
 mkl = { version = "==2023.2.0", optional = true }
+tbb = { version = "==2021.10.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 coverage = { extras = ["toml"], version = "^7.4.3" }
 darglint = "^1.8.1"
 flake8 = "^7.0.0"
 flake8-bugbear = "^24.2.6"
@@ -97,15 +98,15 @@
 sphinx-copybutton = "^0.5.2"
 sphinxext-opengraph = "^0.9.1"
 
 [tool.poetry.extras]
 dxf = ["cad-to-shapely"]
 rhino = ["rhino-shapley-interop", "rhino3dm"]
 numba = ["numba"]
-pardiso = ["pypardiso", "intel-openmp", "mkl"]
+pardiso = ["pypardiso", "intel-openmp", "mkl", "tbb"]
 
 [tool.poetry.scripts]
 sectionproperties = "sectionproperties.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
```

### Comparing `sectionproperties-3.2.1/src/sectionproperties/analysis/fea.py` & `sectionproperties-3.2.2/src/sectionproperties/analysis/fea.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/analysis/plastic_section.py` & `sectionproperties-3.2.2/src/sectionproperties/analysis/plastic_section.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/analysis/section.py` & `sectionproperties-3.2.2/src/sectionproperties/analysis/section.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/analysis/solver.py` & `sectionproperties-3.2.2/src/sectionproperties/analysis/solver.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/post/fibre.py` & `sectionproperties-3.2.2/src/sectionproperties/post/fibre.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/post/post.py` & `sectionproperties-3.2.2/src/sectionproperties/post/post.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/post/stress_post.py` & `sectionproperties-3.2.2/src/sectionproperties/post/stress_post.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/bisect_section.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/bisect_section.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/geometry.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/geometry.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/library/__init__.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/library/__init__.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/library/bridge_sections.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/library/bridge_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/library/concrete_sections.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/library/concrete_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/library/nastran_sections.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/library/nastran_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/library/primitive_sections.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/library/primitive_sections.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/library/steel_sections.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/library/steel_sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -981,15 +981,15 @@
         n_r: Number of points discretising the radii
         material: Material to associate with this geometry
 
     Returns:
         Angle section geometry
 
     Raises:
-        ValueError: If the toe radius is larger than the toe thickness
+        ValueError: If the toe radius is larger than the thickness
 
     Example:
         The following example creates an angle section with a depth of 150 mm, a width
         of 100 mm, a thickness of 8 mm, a root radius of 12 mm and a toe radius of 5 mm,
         using 16 points to discretise the radii:
 
         .. plot::
@@ -998,37 +998,40 @@
 
             from sectionproperties.pre.library import angle_section
 
             angle_section(d=150, b=100, t=8, r_r=12, r_t=5, n_r=16).plot_geometry()
     """
     if r_t > t:
         raise ValueError(
-            "The radius of the toe (r_t) cannot be larger than the toe thickness (t)."
+            "The radius of the toe (r_t) cannot be larger than the thickness (t)."
         )
 
     points: list[tuple[float, float]] = []
 
-    # add first two points
+    # add first two points, but don't add second if the toe radius equals the thickness
     points.append((0, 0))
-    points.append((b, 0))
+
+    if not np.isclose(t, r_t):
+        points.append((b, 0))
 
     # construct the bottom toe radius
     pt = b - r_t, t - r_t
     points += sp_utils.draw_radius(pt=pt, r=r_t, theta=0, n=n_r)
 
     # construct the root radius
     pt = t + r_r, t + r_r
     points += sp_utils.draw_radius(pt=pt, r=r_r, theta=1.5 * np.pi, n=n_r, ccw=False)
 
     # construct the top toe radius
     pt = t - r_t, d - r_t
     points += sp_utils.draw_radius(pt=pt, r=r_t, theta=0, n=n_r)
 
-    # add the next point
-    points.append((0, d))
+    # add the last point, only if the toe radius does not equal the thickness
+    if not np.isclose(t, r_t):
+        points.append((0, d))
 
     polygon = Polygon(points)
 
     return geometry.Geometry(geom=polygon, material=material)
 
 
 def cee_section(
```

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/library/utils.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/library/utils.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/pre.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/pre.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/src/sectionproperties/pre/rhino.py` & `sectionproperties-3.2.2/src/sectionproperties/pre/rhino.py`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/tests/geometry/complex_shape.txt` & `sectionproperties-3.2.2/tests/geometry/complex_shape.txt`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/tests/geometry/compound_shape.txt` & `sectionproperties-3.2.2/tests/geometry/compound_shape.txt`

 * *Files identical despite different names*

### Comparing `sectionproperties-3.2.1/PKG-INFO` & `sectionproperties-3.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectionproperties
-Version: 3.2.1
+Version: 3.2.2
 Summary: A python package for the analysis of arbitrary cross-sections using the finite element method.
 Home-page: https://github.com/robbievanleeuwen/section-properties
 License: MIT
 Keywords: cross-section,structural-engineering,finite-element-analysis,computational-mechanics
 Author: Robbie van Leeuwen
 Author-email: robbie.vanleeuwen@gmail.com
 Maintainer: Robbie van Leeuwen
@@ -29,19 +29,20 @@
 Requires-Dist: intel-openmp (==2023.2.0) ; extra == "pardiso"
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: mkl (==2023.2.0) ; extra == "pardiso"
 Requires-Dist: more-itertools (>=10.2.0,<11.0.0)
 Requires-Dist: numba (>=0.59.0,<0.60.0) ; extra == "numba"
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pypardiso (>=0.4.5,<0.5.0) ; extra == "pardiso"
-Requires-Dist: rhino-shapley-interop (>=0.0.4,<0.0.5) ; (python_full_version >= "3.9.0" and python_version < "3.12") and (extra == "rhino")
-Requires-Dist: rhino3dm (>=8.4.0,<9.0.0) ; (python_full_version >= "3.9.0" and python_version < "3.12") and (extra == "rhino")
+Requires-Dist: rhino-shapley-interop (>=0.0.4,<0.0.5) ; extra == "rhino"
+Requires-Dist: rhino3dm (==8.6.0) ; extra == "rhino"
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: shapely (>=2.0.3,<3.0.0)
+Requires-Dist: tbb (==2021.10.0) ; extra == "pardiso"
 Requires-Dist: triangle (>=20230923,<20230924)
 Project-URL: Bug Tracker, https://github.com/robbievanleeuwen/section-properties/issues
 Project-URL: Changelog, https://github.com/robbievanleeuwen/section-properties/releases
 Project-URL: Documentation, https://sectionproperties.readthedocs.io
 Project-URL: Repository, https://github.com/robbievanleeuwen/section-properties
 Description-Content-Type: text/markdown
 
@@ -52,29 +53,29 @@
 </picture>
 
 [![PyPI](https://img.shields.io/pypi/v/sectionproperties.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/sectionproperties.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/sectionproperties)][python version]
 [![License](https://img.shields.io/pypi/l/sectionproperties)][license]
 [![Read the documentation at https://sectionproperties.readthedocs.io/](https://img.shields.io/readthedocs/sectionproperties/stable.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/robbievanleeuwen/section-properties/workflows/Tests/badge.svg)][tests]
+[![Tests](https://github.com/robbievanleeuwen/section-properties/actions/workflows/tests.yml/badge.svg?branch=master)][tests]
 [![Codecov](https://codecov.io/gh/robbievanleeuwen/section-properties/branch/master/graph/badge.svg)][codecov]
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
-[![JOSS](https://joss.theoj.org/papers/6c3ad57a38202562726b4a7b86a86c32/status.svg)][joss]
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06105/status.svg)][joss]
 
 [pypi_]: https://pypi.org/project/sectionproperties/
 [status]: https://pypi.org/project/sectionproperties/
 [python version]: https://pypi.org/project/sectionproperties
 [read the docs]: https://sectionproperties.readthedocs.io/
 [tests]: https://github.com/robbievanleeuwen/section-properties/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/robbievanleeuwen/section-properties
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
-[joss]: https://joss.theoj.org/papers/6c3ad57a38202562726b4a7b86a86c32
+[joss]: https://doi.org/10.21105/joss.06105
 
 `sectionproperties` is a python package for the analysis of arbitrary cross-sections
 using the finite element method. `sectionproperties` can be used to determine
 section properties to be used in structural design and visualise cross-sectional
 stresses resulting from combinations of applied forces and bending moments.
 
 [Subscribe](http://eepurl.com/dMMUeg) to the `sectionproperties` mailing list!
```

