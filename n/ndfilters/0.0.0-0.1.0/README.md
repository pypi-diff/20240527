# Comparing `tmp/ndfilters-0.0.0.tar.gz` & `tmp/ndfilters-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndfilters-0.0.0.tar", last modified: Wed Jun  7 18:00:28 2023, max compression
+gzip compressed data, was "ndfilters-0.1.0.tar", last modified: Mon May 27 20:15:23 2024, max compression
```

## Comparing `ndfilters-0.0.0.tar` & `ndfilters-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.116980 ndfilters-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.112980 ndfilters-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.112980 ndfilters-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-07 18:00:17.000000 ndfilters-0.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-07 18:00:17.000000 ndfilters-0.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-07 18:00:17.000000 ndfilters-0.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-07 18:00:28.116980 ndfilters-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-07 18:00:17.000000 ndfilters-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.116980 ndfilters-0.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.116980 ndfilters-0.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.116980 ndfilters-0.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/_templates/class_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/_templates/function_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/_templates/module_custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-07 18:00:17.000000 ndfilters-0.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.116980 ndfilters-0.0.0/ndfilters/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 18:00:17.000000 ndfilters-0.0.0/ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-06-07 18:00:17.000000 ndfilters-0.0.0/ndfilters/_trimmed_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.116980 ndfilters-0.0.0/ndfilters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:17.000000 ndfilters-0.0.0/ndfilters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-07 18:00:17.000000 ndfilters-0.0.0/ndfilters/tests/test_trimmed_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:00:28.116980 ndfilters-0.0.0/ndfilters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-07 18:00:28.000000 ndfilters-0.0.0/ndfilters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-07 18:00:28.000000 ndfilters-0.0.0/ndfilters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:00:28.000000 ndfilters-0.0.0/ndfilters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 18:00:28.000000 ndfilters-0.0.0/ndfilters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 18:00:28.000000 ndfilters-0.0.0/ndfilters.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-07 18:00:17.000000 ndfilters-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:00:28.116980 ndfilters-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.382176 ndfilters-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.374176 ndfilters-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.378176 ndfilters-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-27 20:15:19.000000 ndfilters-0.1.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-27 20:15:19.000000 ndfilters-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 20:15:19.000000 ndfilters-0.1.0/.github/workflows/ruff.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-27 20:15:19.000000 ndfilters-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-27 20:15:19.000000 ndfilters-0.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-27 20:15:23.382176 ndfilters-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-27 20:15:19.000000 ndfilters-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.378176 ndfilters-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.378176 ndfilters-0.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.378176 ndfilters-0.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/_templates/class_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/_templates/function_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/_templates/module_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 20:15:19.000000 ndfilters-0.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.378176 ndfilters-0.1.0/ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-27 20:15:19.000000 ndfilters-0.1.0/ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-27 20:15:19.000000 ndfilters-0.1.0/ndfilters/_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.382176 ndfilters-0.1.0/ndfilters/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:19.000000 ndfilters-0.1.0/ndfilters/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-27 20:15:19.000000 ndfilters-0.1.0/ndfilters/_tests/test_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-27 20:15:19.000000 ndfilters-0.1.0/ndfilters/_tests/test_trimmed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-27 20:15:19.000000 ndfilters-0.1.0/ndfilters/_trimmed_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:15:23.382176 ndfilters-0.1.0/ndfilters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-27 20:15:23.000000 ndfilters-0.1.0/ndfilters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-27 20:15:23.000000 ndfilters-0.1.0/ndfilters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:15:23.000000 ndfilters-0.1.0/ndfilters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 20:15:23.000000 ndfilters-0.1.0/ndfilters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 20:15:23.000000 ndfilters-0.1.0/ndfilters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-27 20:15:19.000000 ndfilters-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:15:23.382176 ndfilters-0.1.0/setup.cfg
```

### Comparing `ndfilters-0.0.0/.github/workflows/publish.yml` & `ndfilters-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ndfilters-0.0.0/.github/workflows/tests.yml` & `ndfilters-0.1.0/.github/workflows/tests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 
 name: tests
 
-on: [push, workflow_dispatch, pull_request]
+on:
+  push:
+    branches:
+      - main
+  pull_request:
+
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [
           ubuntu-latest,
           windows-latest,
           macOS-latest,
         ]
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.10", "3.12"]
     name: ${{ matrix.os }}, Python ${{ matrix.python-version }} lint and test
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
@@ -26,15 +31,20 @@
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel
           pip install -e .[test]
       - name: Test with pytest
         run: |
           pip install pytest pytest-cov
-          pytest --doctest-modules --junitxml=junit/test-results.xml --cov=. --cov-report=xml --cov-report=html
+          pytest --cov=. --cov-report=xml
+      - name: Test with Numba disabled
+        env:
+          NUMBA_DISABLE_JIT: 1
+        run: |
+          pytest --cov=. --cov-report=xml
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           file: coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
```

### Comparing `ndfilters-0.0.0/docs/Makefile` & `ndfilters-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndfilters-0.0.0/docs/_templates/class_custom.rst` & `ndfilters-0.1.0/docs/_templates/class_custom.rst`

 * *Files identical despite different names*

### Comparing `ndfilters-0.0.0/docs/_templates/module_custom.rst` & `ndfilters-0.1.0/docs/_templates/module_custom.rst`

 * *Files identical despite different names*

### Comparing `ndfilters-0.0.0/docs/conf.py` & `ndfilters-0.1.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 html_theme_options = {
     "icon_links": [
         {
             "name": "GitHub",
-            "url": "https://github.com/byrdie/ndfilters",
+            "url": "https://github.com/sun-data/ndfilters",
             "icon": "fa-brands fa-github",
             "type": "fontawesome",
         },
         {
             "name": "PyPI",
             "url": "https://pypi.org/project/ndfilters/",
             "icon": "fa-brands fa-python",
```

### Comparing `ndfilters-0.0.0/docs/make.bat` & `ndfilters-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndfilters-0.0.0/ndfilters/tests/test_trimmed_mean.py` & `ndfilters-0.1.0/ndfilters/_tests/test_trimmed_mean.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,84 +4,88 @@
 import scipy.stats
 import ndfilters
 
 
 @pytest.mark.parametrize(
     argnames="array",
     argvalues=[
-        np.random.random(16),
-        np.random.random((16, 17)),
-        np.random.random((16, 17, 18)),
-    ]
+        np.random.random(5),
+        np.random.random((5, 6)),
+        np.random.random((5, 6, 7)),
+    ],
 )
 @pytest.mark.parametrize(
-    argnames="kernel_shape",
-    argvalues=[5, (5,), (5, 6), (5, 6, 7)],
+    argnames="size",
+    argvalues=[2, (3,), (3, 4), (3, 4, 5)],
 )
 @pytest.mark.parametrize(
     argnames="axis",
     argvalues=[
         0,
         -1,
-        (0, ),
-        (-1, ),
+        (0,),
+        (-1,),
         (0, 1),
         (-2, -1),
         (0, 1, 2),
         (2, 1, 0),
-    ]
+    ],
 )
 @pytest.mark.parametrize("proportion", [0.25, 0.45])
 def test_trimmed_mean_filter(
-        array: np.ndarray,
-        kernel_shape: int | tuple[int, ...],
-        axis: None | int | tuple[int, ...],
-        proportion: float,
+    array: np.ndarray,
+    size: int | tuple[int, ...],
+    axis: None | int | tuple[int, ...],
+    proportion: float,
 ):
     if axis is None:
         axis_normalized = tuple(range(array.ndim))
     else:
         try:
-            axis_normalized = np.core.numeric.normalize_axis_tuple(axis, ndim=array.ndim)
+            axis_normalized = np.core.numeric.normalize_axis_tuple(
+                axis, ndim=array.ndim
+            )
         except np.AxisError:
             with pytest.raises(np.AxisError):
                 ndfilters.trimmed_mean_filter(
                     array=array,
-                    kernel_shape=kernel_shape,
+                    size=size,
                     proportion=proportion,
                     axis=axis,
                 )
             return
 
-    kernel_shape_normalized = (kernel_shape,) * len(axis_normalized) if isinstance(kernel_shape, int) else kernel_shape
+    if isinstance(size, int):
+        size_normalized = (size,) * len(axis_normalized)
+    else:
+        size_normalized = size
 
-    if len(kernel_shape_normalized) != len(axis_normalized):
+    if len(size_normalized) != len(axis_normalized):
         with pytest.raises(ValueError):
             ndfilters.trimmed_mean_filter(
                 array=array,
-                kernel_shape=kernel_shape,
+                size=size,
                 proportion=proportion,
                 axis=axis,
             )
         return
 
     result = ndfilters.trimmed_mean_filter(
         array=array,
-        kernel_shape=kernel_shape,
+        size=size,
         proportion=proportion,
         axis=axis,
     )
 
-    kernel_shape_scipy = [1, ] * array.ndim
+    size_scipy = [1] * array.ndim
     for i, ax in enumerate(axis_normalized):
-        kernel_shape_scipy[ax] = kernel_shape_normalized[i]
+        size_scipy[ax] = size_normalized[i]
 
     expected = scipy.ndimage.generic_filter(
         input=array,
         function=scipy.stats.trim_mean,
-        size=kernel_shape_scipy,
+        size=size_scipy,
         mode="mirror",
         extra_keywords=dict(proportiontocut=proportion),
     )
 
     assert np.allclose(result, expected)
-
```

### Comparing `ndfilters-0.0.0/pyproject.toml` & `ndfilters-0.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -19,25 +19,30 @@
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "scipy",
+    "astropy",
 ]
 doc = [
     "pytest",
     "scipy",
     "pooch",
     "matplotlib",
     "graphviz",
     "sphinx-autodoc-typehints",
     "pydata-sphinx-theme",
+    "ipykernel",
     "jupyter-sphinx",
     "sphinx-favicon",
 ]
 
 [project.urls]
-Homepage = "https://github.com/byrdie/ndfilters"
+Homepage = "https://github.com/sun-data/ndfilters"
 Documentation = "https://ndfilters.readthedocs.io/en/latest"
 
+[tool.setuptools]
+packages = ["ndfilters"]
+
 [tool.setuptools_scm]
```

