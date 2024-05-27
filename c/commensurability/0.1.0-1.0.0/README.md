# Comparing `tmp/commensurability-0.1.0.tar.gz` & `tmp/commensurability-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commensurability-0.1.0.tar", last modified: Mon Jan 22 05:42:22 2024, max compression
+gzip compressed data, was "commensurability-1.0.0.tar", last modified: Mon May 27 21:00:41 2024, max compression
```

## Comparing `commensurability-0.1.0.tar` & `commensurability-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,20 @@
--rw-r--r--   0        0        0     1073 2024-01-22 05:42:09.943199 commensurability-0.1.0/LICENSE
--rw-r--r--   0        0        0     1249 2024-01-22 05:42:09.943199 commensurability-0.1.0/README.md
--rw-r--r--   0        0        0     1260 2024-01-22 05:42:22.467233 commensurability-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       80 2024-01-22 05:42:09.947199 commensurability-0.1.0/src/commensurability/__init__.py
--rw-r--r--   0        0        0     7754 2024-01-22 05:42:09.947199 commensurability-0.1.0/src/commensurability/base.py
--rw-r--r--   0        0        0     8794 2024-01-22 05:42:09.947199 commensurability-0.1.0/src/commensurability/interactive.py
--rw-r--r--   0        0        0      511 2024-01-22 05:42:09.947199 commensurability-0.1.0/src/commensurability/tessellation_analysis.py
--rw-r--r--   0        0        0      143 2024-01-22 05:42:09.947199 commensurability-0.1.0/src/commensurability/utils.py
--rw-r--r--   0        0        0     2141 1970-01-01 00:00:00.000000 commensurability-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-27 21:00:27.884791 commensurability-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1473 2024-05-27 21:00:27.884791 commensurability-1.0.0/README.md
+-rw-r--r--   0        0        0     1464 2024-05-27 21:00:41.184732 commensurability-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      548 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/__init__.py
+-rw-r--r--   0        0        0    20895 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/analysis.py
+-rw-r--r--   0        0        0     1037 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/evaluation.py
+-rw-r--r--   0        0        0    14817 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/interactive.py
+-rw-r--r--   0        0        0      668 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/tessellation/__init__.py
+-rw-r--r--   0        0        0     7981 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/tessellation/base.py
+-rw-r--r--   0        0        0     3845 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/tessellation/constructor.py
+-rw-r--r--   0        0        0     3771 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/tessellation/dim2.py
+-rw-r--r--   0        0        0     8484 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/tessellation/dim3.py
+-rw-r--r--   0        0        0      523 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/tessellation/exceptions.py
+-rw-r--r--   0        0        0     4020 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/tessellation/generic.py
+-rw-r--r--   0        0        0     1373 2024-05-27 21:00:27.924790 commensurability-1.0.0/src/commensurability/utils.py
+-rw-r--r--   0        0        0        0 2024-05-27 21:00:27.924790 commensurability-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 21:00:27.924790 commensurability-1.0.0/tests/tessellation/__init__.py
+-rw-r--r--   0        0        0    17432 2024-05-27 21:00:27.924790 commensurability-1.0.0/tests/tessellation/test_tessellation.py
+-rw-r--r--   0        0        0     6783 2024-05-27 21:00:27.924790 commensurability-1.0.0/tests/test_analysis.py
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 commensurability-1.0.0/PKG-INFO
```

### Comparing `commensurability-0.1.0/LICENSE` & `commensurability-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commensurability-0.1.0/README.md` & `commensurability-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/commensurability)](https://pypi.org/project/commensurability/)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 A Python package for performing analysis on orbit commensurabilities.
-[`orbit-tessellation`](https://github.com/ilikecubesnstuff/orbit-tessellation) is used for commensurability evaluation.
 
 This package uses [`pidgey`](https://github.com/ilikecubesnstuff/pidgey) as its orbit integration backend.
 
 ## Installation
 
 Install this package via `pip`:
 
 ```
-python -m pip install orbit-tessellation
+python -m pip install commensurability
 ```
 
 ## Usage
 
-See the `examples` folder for usage cases. `examples/demo` provides a walkthrough of the features.
+See the [documentation](https://commensurability.readthedocs.io/en/latest/) page.
+
+This package is to be used along with one of the galactic dynamics packages [`agama`](https://github.com/GalacticDynamics-Oxford/Agama), [`gala`](https://gala-astro.readthedocs.io/en/latest/), or [`galpy`](https://docs.galpy.org/en/latest/).
+There are scripts for each under the `examples` folder that can be run to test whether everything is working correctly.
```

### Comparing `commensurability-0.1.0/pyproject.toml` & `commensurability-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,77 @@
 [project]
 name = "commensurability"
-version = "0.1.0"
+version = "1.0.0"
 description = "A package for analyzing orbit commensurabilities."
 authors = [
     { name = "ilikecubesnstuff", email = "25328250+ilikecubesnstuff@users.noreply.github.com" },
 ]
 dependencies = [
-    "orbit-tessellation>=0.2.0",
-    "pidgey>=0.2.1",
+    "pidgey>=1.0.0",
     "matplotlib>=3.8.2",
     "tqdm>=4.66.1",
     "h5py>=3.10.0",
     "more_itertools>=10.2.0",
+    "scipy>=1.13.0",
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Physics",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.black]
 line-length = 100
 target-version = [
-    "py39",
-    "py310",
     "py311",
     "py312",
 ]
 
 [tool.isort]
 profile = "black"
 
-[tool.ruff]
-line-length = 100
-
-[tool.ruff.per-file-ignores]
-"__init__.py" = [
-    "F401",
-]
-
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.pdm]
-package-type = "library"
+distribution = true
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "tox-pdm>=0.7.2",
+    "tox>=4.15.0",
+]
+test = [
+    "pytest>=8.2.0",
+]
+type = [
+    "mypy>=1.10.0",
+]
+lint = [
+    "black>=24.4.2",
+    "isort>=5.13.2",
+]
+docs = [
+    "mkdocs>=1.6.0",
+    "mkdocs-gen-files>=0.5.0",
+    "mkdocs-literate-nav>=0.6.1",
+    "mkdocs-material>=9.5.21",
+    "mkdocstrings>=0.25.1",
+    "mkdocstrings-python>=1.10.0",
+]
+github = [
+    "tox-gh-actions>=3.2.0",
+]
```

### Comparing `commensurability-0.1.0/PKG-INFO` & `commensurability-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: commensurability
-Version: 0.1.0
+Version: 1.0.0
 Summary: A package for analyzing orbit commensurabilities.
 Author-Email: ilikecubesnstuff <25328250+ilikecubesnstuff@users.noreply.github.com>
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.9
-Requires-Dist: orbit-tessellation>=0.2.0
-Requires-Dist: pidgey>=0.2.1
+Requires-Python: >=3.11
+Requires-Dist: pidgey>=1.0.0
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: h5py>=3.10.0
 Requires-Dist: more_itertools>=10.2.0
+Requires-Dist: scipy>=1.13.0
 Description-Content-Type: text/markdown
 
 # commensurability
 
 [![PyPI - Version](https://img.shields.io/pypi/v/commensurability)](https://pypi.org/project/commensurability/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/commensurability)](https://pypi.org/project/commensurability/)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 A Python package for performing analysis on orbit commensurabilities.
-[`orbit-tessellation`](https://github.com/ilikecubesnstuff/orbit-tessellation) is used for commensurability evaluation.
 
 This package uses [`pidgey`](https://github.com/ilikecubesnstuff/pidgey) as its orbit integration backend.
 
 ## Installation
 
 Install this package via `pip`:
 
 ```
-python -m pip install orbit-tessellation
+python -m pip install commensurability
 ```
 
 ## Usage
 
-See the `examples` folder for usage cases. `examples/demo` provides a walkthrough of the features.
+See the [documentation](https://commensurability.readthedocs.io/en/latest/) page.
+
+This package is to be used along with one of the galactic dynamics packages [`agama`](https://github.com/GalacticDynamics-Oxford/Agama), [`gala`](https://gala-astro.readthedocs.io/en/latest/), or [`galpy`](https://docs.galpy.org/en/latest/).
+There are scripts for each under the `examples` folder that can be run to test whether everything is working correctly.
```

