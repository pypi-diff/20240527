# Comparing `tmp/intersphinx_registry-0.0.4.tar.gz` & `tmp/intersphinx_registry-0.2405.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intersphinx_registry-0.0.4.tar", last modified: Mon May  6 08:28:29 2024, max compression
+gzip compressed data, was "intersphinx_registry-0.2405.27.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `intersphinx_registry-0.0.4.tar` & `intersphinx_registry-0.2405.27.tar`

### file list

```diff
@@ -1,10 +1,7 @@
--rw-r--r--   0        0        0      698 2024-05-03 15:35:42.574589 intersphinx_registry-0.0.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0        6 2024-05-03 12:40:56.982097 intersphinx_registry-0.0.4/.gitignore
--rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.0.4/LICENSE
--rw-r--r--   0        0        0      975 2024-05-03 09:31:21.573054 intersphinx_registry-0.0.4/README.md
--rw-r--r--   0        0        0     1328 2024-05-06 08:27:56.979465 intersphinx_registry-0.0.4/intersphinx_registry/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.0.4/intersphinx_registry/py.typed
--rw-r--r--   0        0        0     9824 2024-05-06 08:27:56.974573 intersphinx_registry-0.0.4/intersphinx_registry/registry.json
--rw-r--r--   0        0        0      637 2024-05-03 13:38:36.749859 intersphinx_registry-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      884 2024-05-03 15:35:42.576100 intersphinx_registry-0.0.4/tests/test_basic.py
--rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 intersphinx_registry-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.2405.27/LICENSE
+-rw-r--r--   0        0        0     1017 2024-05-27 08:45:56.933382 intersphinx_registry-0.2405.27/README.md
+-rw-r--r--   0        0        0     1705 2024-05-27 08:49:29.949581 intersphinx_registry-0.2405.27/intersphinx_registry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.2405.27/intersphinx_registry/py.typed
+-rw-r--r--   0        0        0     9785 2024-05-27 08:45:56.933718 intersphinx_registry-0.2405.27/intersphinx_registry/registry.json
+-rw-r--r--   0        0        0      637 2024-05-03 13:38:36.749859 intersphinx_registry-0.2405.27/pyproject.toml
+-rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 intersphinx_registry-0.2405.27/PKG-INFO
```

### Comparing `intersphinx_registry-0.0.4/LICENSE` & `intersphinx_registry-0.2405.27/LICENSE`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.4/README.md` & `intersphinx_registry-0.2405.27/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 Usage in `conf.py`
 
 ```python
 from intersphinx_registry import get_intersphinx_mapping
 
 # ...
-
-intersphinx_mapping = get_intersphinx_mapping()
+intersphinx_mapping = get_intersphinx_mapping(
+    only={"ipython", "matplotlib", "pandas", "python"}
+)
 intersphinx_mapping.update({
     'overwrite': ('<url>', None),
     'my-package' : ('<url>', None),
 })
 ```
 
 
-## Why ? 
+## Why ?
 
 Sometime packages docs move and it's hard to keep track of. We _try_ to keep the
 registry up to date, so yo do not have to ask yourself questions and update your
 intersphinx-mapping.
 
 You also might not want to think about adding intersphinx mapping when you refer
 to dependencies.
@@ -30,18 +31,8 @@
 
 Please send a PR updating only this package in the `registry.json`. We try to
 link only to _stable_ package, not dev versions.
 
 ## A package is missing !
 
 We can't do all packages, but if you think a package is widely used and missing,
-please send an PR. 
-
-
-
-
-
-
-
-
-
-
+please send a PR.
```

### Comparing `intersphinx_registry-0.0.4/intersphinx_registry/registry.json` & `intersphinx_registry-0.2405.27/intersphinx_registry/registry.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9675324675324676%*

 * *Differences: {"'build'": "{insert: [(0, 'https://build.pypa.io/en/latest/')], delete: [0]}",*

 * * "'jupyter'": "{insert: [(0, 'https://docs.jupyter.org/en/latest/')], delete: [0]}",*

 * * "'jupyterbook'": "{insert: [(0, 'https://jupyterbook.org/en/stable/')], delete: [0]}",*

 * * "'pillow'": "['https://pillow.readthedocs.io/en/stable/', None]",*

 * * "'pypug'": "{insert: [(0, 'https://packaging.python.org/en/latest/')], delete: [0]}",*

 * * "'pypy'": "{insert: [(0, 'https://doc.pypy.org/en/latest/')], delete: [0]}",*

 * * "'pytorch_lightning'": "{i […]*

```diff
@@ -1,16 +1,8 @@
 {
-    "Pillow": [
-        "https://pillow.readthedocs.io/en/stable/",
-        null
-    ],
-    "PyPUG": [
-        "https://packaging.python.org/en/latest/",
-        null
-    ],
     "anndata": [
         "https://anndata.readthedocs.io/en/stable/",
         null
     ],
     "asdf-astropy": [
         "https://asdf-astropy.readthedocs.io/en/latest/",
         null
@@ -44,15 +36,15 @@
         null
     ],
     "bottle": [
         "https://bottlepy.org/docs/dev/",
         null
     ],
     "build": [
-        "https://pypa-build.readthedocs.io/en/latest/",
+        "https://build.pypa.io/en/latest/",
         null
     ],
     "cartopy": [
         "https://scitools.org.uk/cartopy/docs/latest/",
         null
     ],
     "cffi": [
@@ -176,27 +168,27 @@
         null
     ],
     "joblib": [
         "https://joblib.readthedocs.io/en/latest/",
         null
     ],
     "jupyter": [
-        "https://jupyter.readthedocs.io/en/latest/",
+        "https://docs.jupyter.org/en/latest/",
         null
     ],
     "jupyter-server": [
         "https://jupyter-server.readthedocs.io/en/stable/",
         null
     ],
     "jupyter_core": [
         "https://jupyter-core.readthedocs.io/en/stable/",
         null
     ],
     "jupyterbook": [
-        "https://jupyterbook.org/",
+        "https://jupyterbook.org/en/stable/",
         null
     ],
     "jupyterclient": [
         "https://jupyter-client.readthedocs.io/en/latest/",
         null
     ],
     "jupytercore": [
@@ -347,14 +339,18 @@
         "https://parso.readthedocs.io/en/latest/",
         null
     ],
     "patsy": [
         "https://patsy.readthedocs.io/en/latest/",
         null
     ],
+    "pillow": [
+        "https://pillow.readthedocs.io/en/stable/",
+        null
+    ],
     "pip": [
         "https://pip.pypa.io/en/latest/",
         null
     ],
     "pipenv": [
         "https://pipenv.pypa.io/en/latest/",
         null
@@ -408,19 +404,19 @@
         null
     ],
     "pypa": [
         "https://www.pypa.io/en/latest/",
         null
     ],
     "pypug": [
-        "https://packaging.python.org/",
+        "https://packaging.python.org/en/latest/",
         null
     ],
     "pypy": [
-        "https://pypy.readthedocs.io/en/latest/",
+        "https://doc.pypy.org/en/latest/",
         null
     ],
     "pyqtgraph": [
         "https://pyqtgraph.readthedocs.io/en/latest/",
         null
     ],
     "pyro": [
@@ -436,15 +432,15 @@
         null
     ],
     "python-guide": [
         "https://docs.python-guide.org/",
         null
     ],
     "pytorch_lightning": [
-        "https://pytorch-lightning.readthedocs.io/en/stable/",
+        "https://lightning.ai/docs/pytorch/stable/",
         null
     ],
     "pyvista": [
         "https://docs.pyvista.org/version/stable/",
         null
     ],
     "qiskit": [
```

### Comparing `intersphinx_registry-0.0.4/pyproject.toml` & `intersphinx_registry-0.2405.27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.4/PKG-INFO` & `intersphinx_registry-0.2405.27/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intersphinx_registry
-Version: 0.0.4
+Version: 0.2405.27
 Summary: This package provides convenient utilities and data to write a sphinx config file.
 Author-email: Matthias Bussonnier <bussonniermatthias@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pytest>=7.0 ; extra == "tests"
 Requires-Dist: pytest-xdist ; extra == "tests"
 Requires-Dist: requests ; extra == "tests"
@@ -17,24 +17,25 @@
 
 Usage in `conf.py`
 
 ```python
 from intersphinx_registry import get_intersphinx_mapping
 
 # ...
-
-intersphinx_mapping = get_intersphinx_mapping()
+intersphinx_mapping = get_intersphinx_mapping(
+    only={"ipython", "matplotlib", "pandas", "python"}
+)
 intersphinx_mapping.update({
     'overwrite': ('<url>', None),
     'my-package' : ('<url>', None),
 })
 ```
 
 
-## Why ? 
+## Why ?
 
 Sometime packages docs move and it's hard to keep track of. We _try_ to keep the
 registry up to date, so yo do not have to ask yourself questions and update your
 intersphinx-mapping.
 
 You also might not want to think about adding intersphinx mapping when you refer
 to dependencies.
@@ -43,19 +44,9 @@
 
 Please send a PR updating only this package in the `registry.json`. We try to
 link only to _stable_ package, not dev versions.
 
 ## A package is missing !
 
 We can't do all packages, but if you think a package is widely used and missing,
-please send an PR. 
-
-
-
-
-
-
-
-
-
-
+please send a PR.
```

