# Comparing `tmp/jaxquantum-0.1.0.tar.gz` & `tmp/jaxquantum-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxquantum-0.1.0.tar", last modified: Mon Mar  4 10:49:11 2024, max compression
+gzip compressed data, was "jaxquantum-0.1.1.tar", last modified: Mon May 27 04:58:49 2024, max compression
```

## Comparing `jaxquantum-0.1.0.tar` & `jaxquantum-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:49:11.683045 jaxquantum-0.1.0/
--rw-r--r--   0 phionx     (501) staff       (20)    11357 2024-02-27 03:55:06.000000 jaxquantum-0.1.0/LICENSE
--rw-r--r--   0 phionx     (501) staff       (20)       78 2024-03-04 10:42:28.000000 jaxquantum-0.1.0/MANIFEST.in
--rw-r--r--   0 phionx     (501) staff       (20)     6164 2024-03-04 10:49:11.682755 jaxquantum-0.1.0/PKG-INFO
--rw-r--r--   0 phionx     (501) staff       (20)     4543 2024-03-04 10:09:31.000000 jaxquantum-0.1.0/README.md
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:49:11.677165 jaxquantum-0.1.0/docs/
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:49:11.677352 jaxquantum-0.1.0/docs/assets/
--rw-r--r--   0 phionx     (501) staff       (20)    92891 2024-03-04 08:04:16.000000 jaxquantum-0.1.0/docs/assets/logo.png
--rw-r--r--   0 phionx     (501) staff       (20)      943 2024-02-27 03:55:06.000000 jaxquantum-0.1.0/docs/gen_ref_pages.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:49:11.678398 jaxquantum-0.1.0/jaxquantum/
--rw-r--r--   0 phionx     (501) staff       (20)        5 2024-02-27 03:55:06.000000 jaxquantum-0.1.0/jaxquantum/VERSION.txt
--rw-r--r--   0 phionx     (501) staff       (20)      276 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/__init__.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:49:11.681239 jaxquantum-0.1.0/jaxquantum/core/
--rw-r--r--   0 phionx     (501) staff       (20)      179 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/core/__init__.py
--rw-r--r--   0 phionx     (501) staff       (20)     1644 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/core/conversions.py
--rw-r--r--   0 phionx     (501) staff       (20)     2757 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/core/operators.py
--rw-r--r--   0 phionx     (501) staff       (20)    11324 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/core/qarray.py
--rw-r--r--   0 phionx     (501) staff       (20)       68 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/core/settings.py
--rw-r--r--   0 phionx     (501) staff       (20)     8724 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/core/solvers.py
--rw-r--r--   0 phionx     (501) staff       (20)     1950 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/core/visualization.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:49:11.681631 jaxquantum-0.1.0/jaxquantum/utils/
--rw-r--r--   0 phionx     (501) staff       (20)       34 2024-02-27 03:55:06.000000 jaxquantum-0.1.0/jaxquantum/utils/__init__.py
--rw-r--r--   0 phionx     (501) staff       (20)     1964 2024-03-04 07:42:24.000000 jaxquantum-0.1.0/jaxquantum/utils/utils.py
-drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-03-04 10:49:11.681817 jaxquantum-0.1.0/jaxquantum.egg-info/
--rw-r--r--   0 phionx     (501) staff       (20)     6164 2024-03-04 10:49:11.000000 jaxquantum-0.1.0/jaxquantum.egg-info/PKG-INFO
--rw-r--r--   0 phionx     (501) staff       (20)      553 2024-03-04 10:49:11.000000 jaxquantum-0.1.0/jaxquantum.egg-info/SOURCES.txt
--rw-r--r--   0 phionx     (501) staff       (20)        1 2024-03-04 10:49:11.000000 jaxquantum-0.1.0/jaxquantum.egg-info/dependency_links.txt
--rw-r--r--   0 phionx     (501) staff       (20)      197 2024-03-04 10:49:11.000000 jaxquantum-0.1.0/jaxquantum.egg-info/requires.txt
--rw-r--r--   0 phionx     (501) staff       (20)       37 2024-03-04 10:49:11.000000 jaxquantum-0.1.0/jaxquantum.egg-info/top_level.txt
--rw-r--r--   0 phionx     (501) staff       (20)       38 2024-03-04 10:49:11.683094 jaxquantum-0.1.0/setup.cfg
--rw-r--r--   0 phionx     (501) staff       (20)     2181 2024-03-04 10:36:14.000000 jaxquantum-0.1.0/setup.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 04:58:49.794161 jaxquantum-0.1.1/
+-rw-r--r--   0 phionx     (501) staff       (20)    11357 2024-02-27 03:55:06.000000 jaxquantum-0.1.1/LICENSE
+-rw-r--r--   0 phionx     (501) staff       (20)       78 2024-03-04 10:42:28.000000 jaxquantum-0.1.1/MANIFEST.in
+-rw-r--r--   0 phionx     (501) staff       (20)     6228 2024-05-27 04:58:49.793942 jaxquantum-0.1.1/PKG-INFO
+-rw-r--r--   0 phionx     (501) staff       (20)     4608 2024-05-27 04:57:15.000000 jaxquantum-0.1.1/README.md
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 04:58:49.788586 jaxquantum-0.1.1/docs/
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 04:58:49.788864 jaxquantum-0.1.1/docs/assets/
+-rw-r--r--   0 phionx     (501) staff       (20)    92891 2024-03-04 08:04:16.000000 jaxquantum-0.1.1/docs/assets/logo.png
+-rw-r--r--   0 phionx     (501) staff       (20)      943 2024-02-27 03:55:06.000000 jaxquantum-0.1.1/docs/gen_ref_pages.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 04:58:49.789747 jaxquantum-0.1.1/jaxquantum/
+-rw-r--r--   0 phionx     (501) staff       (20)        5 2024-05-27 04:00:50.000000 jaxquantum-0.1.1/jaxquantum/VERSION.txt
+-rw-r--r--   0 phionx     (501) staff       (20)      276 2024-03-04 07:42:24.000000 jaxquantum-0.1.1/jaxquantum/__init__.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 04:58:49.792120 jaxquantum-0.1.1/jaxquantum/core/
+-rw-r--r--   0 phionx     (501) staff       (20)      179 2024-03-04 07:42:24.000000 jaxquantum-0.1.1/jaxquantum/core/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)     2376 2024-05-02 18:30:35.000000 jaxquantum-0.1.1/jaxquantum/core/conversions.py
+-rw-r--r--   0 phionx     (501) staff       (20)     2757 2024-03-04 07:42:24.000000 jaxquantum-0.1.1/jaxquantum/core/operators.py
+-rw-r--r--   0 phionx     (501) staff       (20)    12212 2024-03-30 18:49:06.000000 jaxquantum-0.1.1/jaxquantum/core/qarray.py
+-rw-r--r--   0 phionx     (501) staff       (20)       68 2024-03-04 07:42:24.000000 jaxquantum-0.1.1/jaxquantum/core/settings.py
+-rw-r--r--   0 phionx     (501) staff       (20)     8724 2024-03-04 07:42:24.000000 jaxquantum-0.1.1/jaxquantum/core/solvers.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1950 2024-03-04 07:42:24.000000 jaxquantum-0.1.1/jaxquantum/core/visualization.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 04:58:49.792906 jaxquantum-0.1.1/jaxquantum/utils/
+-rw-r--r--   0 phionx     (501) staff       (20)       34 2024-02-27 03:55:06.000000 jaxquantum-0.1.1/jaxquantum/utils/__init__.py
+-rw-r--r--   0 phionx     (501) staff       (20)     1964 2024-03-04 07:42:24.000000 jaxquantum-0.1.1/jaxquantum/utils/utils.py
+drwxr-xr-x   0 phionx     (501) staff       (20)        0 2024-05-27 04:58:49.793104 jaxquantum-0.1.1/jaxquantum.egg-info/
+-rw-r--r--   0 phionx     (501) staff       (20)     6228 2024-05-27 04:58:49.000000 jaxquantum-0.1.1/jaxquantum.egg-info/PKG-INFO
+-rw-r--r--   0 phionx     (501) staff       (20)      553 2024-05-27 04:58:49.000000 jaxquantum-0.1.1/jaxquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 phionx     (501) staff       (20)        1 2024-05-27 04:58:49.000000 jaxquantum-0.1.1/jaxquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 phionx     (501) staff       (20)      197 2024-05-27 04:58:49.000000 jaxquantum-0.1.1/jaxquantum.egg-info/requires.txt
+-rw-r--r--   0 phionx     (501) staff       (20)       42 2024-05-27 04:58:49.000000 jaxquantum-0.1.1/jaxquantum.egg-info/top_level.txt
+-rw-r--r--   0 phionx     (501) staff       (20)       38 2024-05-27 04:58:49.794201 jaxquantum-0.1.1/setup.cfg
+-rw-r--r--   0 phionx     (501) staff       (20)     2181 2024-03-04 10:36:14.000000 jaxquantum-0.1.1/setup.py
```

### Comparing `jaxquantum-0.1.0/LICENSE` & `jaxquantum-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/PKG-INFO` & `jaxquantum-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxquantum
-Version: 0.1.0
+Version: 0.1.1
 Summary: jaxquantum
 Home-page: https://github.com/EQuS/jaxquantum
 Author: Shantanu Jha, Shoumik Chowdhury, Max Hays
 Author-email: shantanu.rajesh.jha@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://equs.github.io/jaxquantum
 Project-URL: Source Code, https://github.com/EQuS/jaxquantum
@@ -38,27 +38,27 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 
 <h1 align="center">
-    <img src="./docs/assets/logo.png" height="120" alt="jaxquantum logo">
+    <img src="https://github.com/EQuS/jaxquantum/raw/main/docs/assets/logo.png" height="120" alt="jaxquantum logo">
 </h1>
 
 
 [![License](https://img.shields.io/github/license/EQuS/jaxquantum.svg?style=popout-square)](https://opensource.org/license/apache-2-0) [![](https://img.shields.io/github/release/EQuS/jaxquantum.svg?style=popout-square)](https://github.com/EQuS/jaxquantum/releases) [![](https://img.shields.io/pypi/dm/jaxquantum.svg?style=popout-square)](https://pypi.org/project/jaxquantum/)
 
 [S. R. Jha](https://github.com/Phionx), [S. Chowdhury](https://github.com/shoumikdc), [M. Hays](https://scholar.google.com/citations?user=06z0MjwAAAAJ), [J. A. Grover](https://scholar.google.com/citations?user=igewch8AAAAJ), [W. D. Oliver](https://scholar.google.com/citations?user=4vNbnqcAAAAJ&hl=en)
 
 ***Docs:** [https://equs.github.io/jaxquantum](https://equs.github.io/jaxquantum)
 
 `jaxquantum` leverages [JAX](https://github.com/google/jax) to enable the auto differentiable and (CPU, GPU, TPU) accelerated simulation of quantum dynamical systems, including tooling such as operator construction, unitary evolution and master equation solving. As such, `jaxquantum` serves as a QuTiP drop-in replacement written entirely in JAX.
 
-This package also serves as an essential dependency for [`bosonic-jax`](https://github.com/EQuS/bosonic-jax) and [`qcsys`](https://github.com/EQuS/qcsys). Together, these packages form an end-to-end toolkit for quantum circuit design, simulation and control. 
+This package also serves as an essential dependency for [`bosonic`](https://github.com/EQuS/bosonic) and [`qcsys`](https://github.com/EQuS/qcsys). Together, these packages form an end-to-end toolkit for quantum circuit design, simulation and control. 
 
 
 ## Installation
 
 `jaxquantum` is published on PyPI. So, to install the latest version from PyPI, simply run the following code to install the package:
 
 ```bash
@@ -67,15 +67,15 @@
 
 For more details, please visit the getting started > installation section of our [docs](https://equs.github.io/jaxquantum/getting_started/installation.html).
 
 ## An Example
 
 Here's an example of how to set up a simulation in jaxquantum.
 
-```
+```python
 from jax import jit
 import jaxquantum as jqt
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 
 omega_q = 5.0 #GHz
 Omega = .1
@@ -106,26 +106,27 @@
 ```
 
 ## Acknowledgements & History
 
 **Core Devs:** [Shantanu A. Jha](https://github.com/Phionx), [Shoumik Chowdhury](https://github.com/shoumikdc)
 
 
-This package was initially a small part of [`bosonic-jax`](https://github.com/EQuS/bosonic-jax). In early 2022, `jaxquantum` was extracted and made into its own package. This package was briefly announced to the world at APS March Meeting 2023 and released to a select few academic groups shortly after. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
+This package was initially a small part of [`bosonic`](https://github.com/EQuS/bosonic). In early 2022, `jaxquantum` was extracted and made into its own package. This package was briefly announced to the world at APS March Meeting 2023 and released to a select few academic groups shortly after. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
 
 ## Citation
 
 Thank you for taking the time to try our package out. If you found it useful in your research, please cite us as follows:
 
-``` 
-@unpublished{jha2024jaxquantum,
+```bibtex
+@software{jha2024jaxquantum,
+  author = {Shantanu R. Jha and Shoumik Chowdhury and Max Hays and Jeff A. Grover and William D. Oliver},
   title  = {An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control},
-  author = {Shantanu R. Jha, Shoumik Chowdhury, Max Hays, Jeff A. Grover, William D. Oliver},
+  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic, https://github.com/EQuS/qcsys},
+  version = {0.1.0},
   year   = {2024},
-  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic-jax, https://github.com/EQuS/qcsys}
 }
 ```
 > S. R. Jha, S. Chowdhury, M. Hays, J. A. Grover, W. D. Oliver. An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control (2024), in preparation.
 
 
 ## Contributions & Contact
```

### Comparing `jaxquantum-0.1.0/README.md` & `jaxquantum-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <h1 align="center">
-    <img src="./docs/assets/logo.png" height="120" alt="jaxquantum logo">
+    <img src="https://github.com/EQuS/jaxquantum/raw/main/docs/assets/logo.png" height="120" alt="jaxquantum logo">
 </h1>
 
 
 [![License](https://img.shields.io/github/license/EQuS/jaxquantum.svg?style=popout-square)](https://opensource.org/license/apache-2-0) [![](https://img.shields.io/github/release/EQuS/jaxquantum.svg?style=popout-square)](https://github.com/EQuS/jaxquantum/releases) [![](https://img.shields.io/pypi/dm/jaxquantum.svg?style=popout-square)](https://pypi.org/project/jaxquantum/)
 
 [S. R. Jha](https://github.com/Phionx), [S. Chowdhury](https://github.com/shoumikdc), [M. Hays](https://scholar.google.com/citations?user=06z0MjwAAAAJ), [J. A. Grover](https://scholar.google.com/citations?user=igewch8AAAAJ), [W. D. Oliver](https://scholar.google.com/citations?user=4vNbnqcAAAAJ&hl=en)
 
 ***Docs:** [https://equs.github.io/jaxquantum](https://equs.github.io/jaxquantum)
 
 `jaxquantum` leverages [JAX](https://github.com/google/jax) to enable the auto differentiable and (CPU, GPU, TPU) accelerated simulation of quantum dynamical systems, including tooling such as operator construction, unitary evolution and master equation solving. As such, `jaxquantum` serves as a QuTiP drop-in replacement written entirely in JAX.
 
-This package also serves as an essential dependency for [`bosonic-jax`](https://github.com/EQuS/bosonic-jax) and [`qcsys`](https://github.com/EQuS/qcsys). Together, these packages form an end-to-end toolkit for quantum circuit design, simulation and control. 
+This package also serves as an essential dependency for [`bosonic`](https://github.com/EQuS/bosonic) and [`qcsys`](https://github.com/EQuS/qcsys). Together, these packages form an end-to-end toolkit for quantum circuit design, simulation and control. 
 
 
 ## Installation
 
 `jaxquantum` is published on PyPI. So, to install the latest version from PyPI, simply run the following code to install the package:
 
 ```bash
@@ -24,15 +24,15 @@
 
 For more details, please visit the getting started > installation section of our [docs](https://equs.github.io/jaxquantum/getting_started/installation.html).
 
 ## An Example
 
 Here's an example of how to set up a simulation in jaxquantum.
 
-```
+```python
 from jax import jit
 import jaxquantum as jqt
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 
 omega_q = 5.0 #GHz
 Omega = .1
@@ -63,27 +63,28 @@
 ```
 
 ## Acknowledgements & History
 
 **Core Devs:** [Shantanu A. Jha](https://github.com/Phionx), [Shoumik Chowdhury](https://github.com/shoumikdc)
 
 
-This package was initially a small part of [`bosonic-jax`](https://github.com/EQuS/bosonic-jax). In early 2022, `jaxquantum` was extracted and made into its own package. This package was briefly announced to the world at APS March Meeting 2023 and released to a select few academic groups shortly after. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
+This package was initially a small part of [`bosonic`](https://github.com/EQuS/bosonic). In early 2022, `jaxquantum` was extracted and made into its own package. This package was briefly announced to the world at APS March Meeting 2023 and released to a select few academic groups shortly after. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
 
 ## Citation
 
 Thank you for taking the time to try our package out. If you found it useful in your research, please cite us as follows:
 
-``` 
-@unpublished{jha2024jaxquantum,
+```bibtex
+@software{jha2024jaxquantum,
+  author = {Shantanu R. Jha and Shoumik Chowdhury and Max Hays and Jeff A. Grover and William D. Oliver},
   title  = {An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control},
-  author = {Shantanu R. Jha, Shoumik Chowdhury, Max Hays, Jeff A. Grover, William D. Oliver},
+  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic, https://github.com/EQuS/qcsys},
+  version = {0.1.0},
   year   = {2024},
-  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic-jax, https://github.com/EQuS/qcsys}
 }
 ```
 > S. R. Jha, S. Chowdhury, M. Hays, J. A. Grover, W. D. Oliver. An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control (2024), in preparation.
 
 
 ## Contributions & Contact
 
-This package is open source and, as such, very open to contributions. Please don't hesitate to open an issue, report a bug, request a feature, or create a pull request. We are also open to deeper collaborations to create a tool that is more useful for everyone. If a discussion would be helpful, please email [shanjha@mit.edu](mailto:shanjha@mit.edu) to set up a meeting. 
+This package is open source and, as such, very open to contributions. Please don't hesitate to open an issue, report a bug, request a feature, or create a pull request. We are also open to deeper collaborations to create a tool that is more useful for everyone. If a discussion would be helpful, please email [shanjha@mit.edu](mailto:shanjha@mit.edu) to set up a meeting.
```

### Comparing `jaxquantum-0.1.0/docs/assets/logo.png` & `jaxquantum-0.1.1/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/docs/gen_ref_pages.py` & `jaxquantum-0.1.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/jaxquantum/core/conversions.py` & `jaxquantum-0.1.1/jaxquantum/core/conversions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Converting between different object types.
 """
 
+from numbers import Number
 from jax import config, Array
 from qutip import Qobj
-from typing import Optional
+from typing import Optional, Union, List
 import jax.numpy as jnp
 import numpy as np
 
 
 from jaxquantum.core.qarray import Qarray, DIMS_TYPE
 
 
@@ -42,35 +43,59 @@
         QuTiP state.
     """
     if isinstance(jqt_obj, Qobj) or jqt_obj is None:
         return jqt_obj
     
     return Qobj(np.array(jqt_obj.data), dims=jqt_obj.dims)
 
-def jnp2jqt(arr: Array, dims: Optional[DIMS_TYPE] = None):
+
+def extract_dims(arr: Array, dims: Optional[Union[DIMS_TYPE, List[int]]] = None):
+    """Extract dims from a JAX array or Qarray.
+
+    Args:
+        arr: JAX array or Qarray.
+        dims: Qarray dims.
+
+    Returns:
+        Qarray dims.
+    """
+    if isinstance(dims[0], Number):
+        is_op = len(arr.shape) == 2 and arr.shape[0] == arr.shape[1]
+        if is_op:
+            dims = [dims, dims]
+        else:
+            dims = [dims, [1] * len(dims)] # defaults to ket 
+    return dims
+                 
+
+def jnp2jqt(arr: Array, dims: Optional[Union[DIMS_TYPE, List[int]]] = None):
     """JAX array -> QuTiP state.
 
     Args:
         jnp_obj: JAX array.
+        dims: Qarray dims.
 
     Returns:
         QuTiP state.
     """
+    dims = extract_dims(arr, dims) if dims is not None else None
     return Qarray.create(arr, dims=dims)
 
 
 def jnps2jqts(arrs: Array, dims: Optional[DIMS_TYPE] = None):
     """JAX array -> QuTiP state.
 
     Args:
         jnp_obj: JAX array.
 
     Returns:
         QuTiP state.
     """
+
+    dims = extract_dims(arrs[0], dims) if dims is not None else None
     return [Qarray.create(arr, dims=dims) for arr in arrs]
 
 def jqts2jnps(qarrs: Qarray):
     """QuTiP state -> JAX array.
 
     Args:
         qt_obj: QuTiP state.
```

### Comparing `jaxquantum-0.1.0/jaxquantum/core/operators.py` & `jaxquantum-0.1.1/jaxquantum/core/operators.py`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/jaxquantum/core/qarray.py` & `jaxquantum-0.1.1/jaxquantum/core/qarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,14 +235,17 @@
     def dims(self):
         return self._qdims.dims
     
     @property
     def data(self):
         return self._data
     
+    @property
+    def shaped_data(self):
+        return self._data.reshape(self.dims[0] + self.dims[1])
 
     def _str_header(self):
         out = ", ".join([
             "Quantum array: dims = " + str(self.dims),
             "shape = " + str(self._data.shape),
             "type = " + str(self.qtype),
         ])
@@ -330,41 +333,82 @@
     dims = deepcopy(args[0].dims)
     for arg in args[1:]:
         data = jnp.kron(data, arg.data)
         dims[0] += arg.dims[0]
         dims[1] += arg.dims[1]
     return Qarray.create(data, dims=dims)
 
-def tr(qarr: Qarray, **kwargs) -> Qarray:
+def tr(qarr: Qarray, **kwargs) -> jnp.complex128:
     """Full trace.
 
     Args:
         qarr (Qarray): quantum array    
 
     Returns:
         Full trace.
     """
-    return jnp.trace(qarr.data, **kwargs)
+    return trace(qarr, **kwargs)
+
+
+def expm_data(data: Array, **kwargs) -> Array:
+    """Matrix exponential wrapper.
+
+    Returns:
+        matrix exponential
+    """
+    return jsp.linalg.expm(data, **kwargs)
 
 def expm(qarr: Qarray, **kwargs) -> Qarray:
     """Matrix exponential wrapper.
 
     Returns:
         matrix exponential
     """
-    data = jsp.linalg.expm(qarr.data, **kwargs)
-    dims = deepcopy(qarr.dims)
+    dims = qarr.dims
+    data = expm_data(qarr.data, **kwargs)
     return Qarray.create(data, dims=dims)
 
 
+def cosm_data(data: Array, **kwargs) -> Array:
+    """Matrix cosine wrapper.
+
+    Returns:
+        matrix cosine
+    """
+    return (expm_data(1j*data) + expm_data(-1j*data))/2 
+
 def cosm(qarr: Qarray) -> Qarray:
-    return (expm(1j*qarr) + expm(-1j*qarr))/2 
+    """Matrix cosine wrapper.
+
+    Args:
+        qarr (Qarray): quantum array
+
+    Returns:
+        matrix cosine
+    """
+    dims = qarr.dims
+    data = cosm_data(qarr.data)
+    return Qarray.create(data, dims=dims)
+
+
+def sinm_data(data: Array, **kwargs) -> Array:
+    """Matrix sine wrapper.
+
+    Args:
+        data: matrix
+
+    Returns:
+        matrix sine
+    """
+    return (expm_data(1j*data) - expm_data(-1j*data))/(2j)
 
 def sinm(qarr: Qarray) -> Qarray:
-    return (expm(1j*qarr) - expm(-1j*qarr))/(2j)
+    dims = qarr.dims
+    data = sinm_data(qarr.data)
+    return Qarray.create(data, dims=dims)
 
 
 def keep_only_diag_elements(qarr: Qarray) -> Qarray:
     dims = qarr.dims
     data = jnp.diag(jnp.diag(qarr.data))
     return Qarray.create(data, dims=dims)
 
@@ -380,35 +424,35 @@
     Returns:
         partial traced out density matrix
 
     TODO: Fix weird tracing errors that arise with reshape
     """
 
     qarr = ket2dm(qarr)
-    rho = qarr.data
+    rho = qarr.shaped_data
     dims = qarr.dims
 
     Nq = len(dims[0])
-    dims2 = jnp.concatenate(jnp.array(dims))
-
-    rho = rho.reshape(dims2)
 
     indxs = [indx, indx + Nq]
     for j in range(Nq):
         if j == indx:
             continue
         indxs.append(j)
         indxs.append(j + Nq)
     rho = rho.transpose(indxs)
 
     for j in range(Nq - 1):
         rho = jnp.trace(rho, axis1=2, axis2=3)
 
     return Qarray.create(rho)
 
+def trace(qarr: Qarray, **kwargs) -> Qarray:
+    return jnp.trace(qarr.data, **kwargs)
+
 def dag(qarr: Qarray) -> Qarray:
     """Conjugate transpose.
 
     Args:
         qarr (Qarray): quantum array
 
     Returns:
```

### Comparing `jaxquantum-0.1.0/jaxquantum/core/solvers.py` & `jaxquantum-0.1.1/jaxquantum/core/solvers.py`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/jaxquantum/core/visualization.py` & `jaxquantum-0.1.1/jaxquantum/core/visualization.py`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/jaxquantum/utils/utils.py` & `jaxquantum-0.1.1/jaxquantum/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/jaxquantum.egg-info/PKG-INFO` & `jaxquantum-0.1.1/jaxquantum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxquantum
-Version: 0.1.0
+Version: 0.1.1
 Summary: jaxquantum
 Home-page: https://github.com/EQuS/jaxquantum
 Author: Shantanu Jha, Shoumik Chowdhury, Max Hays
 Author-email: shantanu.rajesh.jha@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://equs.github.io/jaxquantum
 Project-URL: Source Code, https://github.com/EQuS/jaxquantum
@@ -38,27 +38,27 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 
 <h1 align="center">
-    <img src="./docs/assets/logo.png" height="120" alt="jaxquantum logo">
+    <img src="https://github.com/EQuS/jaxquantum/raw/main/docs/assets/logo.png" height="120" alt="jaxquantum logo">
 </h1>
 
 
 [![License](https://img.shields.io/github/license/EQuS/jaxquantum.svg?style=popout-square)](https://opensource.org/license/apache-2-0) [![](https://img.shields.io/github/release/EQuS/jaxquantum.svg?style=popout-square)](https://github.com/EQuS/jaxquantum/releases) [![](https://img.shields.io/pypi/dm/jaxquantum.svg?style=popout-square)](https://pypi.org/project/jaxquantum/)
 
 [S. R. Jha](https://github.com/Phionx), [S. Chowdhury](https://github.com/shoumikdc), [M. Hays](https://scholar.google.com/citations?user=06z0MjwAAAAJ), [J. A. Grover](https://scholar.google.com/citations?user=igewch8AAAAJ), [W. D. Oliver](https://scholar.google.com/citations?user=4vNbnqcAAAAJ&hl=en)
 
 ***Docs:** [https://equs.github.io/jaxquantum](https://equs.github.io/jaxquantum)
 
 `jaxquantum` leverages [JAX](https://github.com/google/jax) to enable the auto differentiable and (CPU, GPU, TPU) accelerated simulation of quantum dynamical systems, including tooling such as operator construction, unitary evolution and master equation solving. As such, `jaxquantum` serves as a QuTiP drop-in replacement written entirely in JAX.
 
-This package also serves as an essential dependency for [`bosonic-jax`](https://github.com/EQuS/bosonic-jax) and [`qcsys`](https://github.com/EQuS/qcsys). Together, these packages form an end-to-end toolkit for quantum circuit design, simulation and control. 
+This package also serves as an essential dependency for [`bosonic`](https://github.com/EQuS/bosonic) and [`qcsys`](https://github.com/EQuS/qcsys). Together, these packages form an end-to-end toolkit for quantum circuit design, simulation and control. 
 
 
 ## Installation
 
 `jaxquantum` is published on PyPI. So, to install the latest version from PyPI, simply run the following code to install the package:
 
 ```bash
@@ -67,15 +67,15 @@
 
 For more details, please visit the getting started > installation section of our [docs](https://equs.github.io/jaxquantum/getting_started/installation.html).
 
 ## An Example
 
 Here's an example of how to set up a simulation in jaxquantum.
 
-```
+```python
 from jax import jit
 import jaxquantum as jqt
 import jax.numpy as jnp
 import matplotlib.pyplot as plt
 
 omega_q = 5.0 #GHz
 Omega = .1
@@ -106,26 +106,27 @@
 ```
 
 ## Acknowledgements & History
 
 **Core Devs:** [Shantanu A. Jha](https://github.com/Phionx), [Shoumik Chowdhury](https://github.com/shoumikdc)
 
 
-This package was initially a small part of [`bosonic-jax`](https://github.com/EQuS/bosonic-jax). In early 2022, `jaxquantum` was extracted and made into its own package. This package was briefly announced to the world at APS March Meeting 2023 and released to a select few academic groups shortly after. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
+This package was initially a small part of [`bosonic`](https://github.com/EQuS/bosonic). In early 2022, `jaxquantum` was extracted and made into its own package. This package was briefly announced to the world at APS March Meeting 2023 and released to a select few academic groups shortly after. Since then, this package has been open sourced and developed while conducting research in the Engineering Quantum Systems Group at MIT with invaluable advice from [Prof. William D. Oliver](https://equs.mit.edu/william-d-oliver/). 
 
 ## Citation
 
 Thank you for taking the time to try our package out. If you found it useful in your research, please cite us as follows:
 
-``` 
-@unpublished{jha2024jaxquantum,
+```bibtex
+@software{jha2024jaxquantum,
+  author = {Shantanu R. Jha and Shoumik Chowdhury and Max Hays and Jeff A. Grover and William D. Oliver},
   title  = {An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control},
-  author = {Shantanu R. Jha, Shoumik Chowdhury, Max Hays, Jeff A. Grover, William D. Oliver},
+  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic, https://github.com/EQuS/qcsys},
+  version = {0.1.0},
   year   = {2024},
-  url    = {https://github.com/EQuS/jaxquantum, https://github.com/EQuS/bosonic-jax, https://github.com/EQuS/qcsys}
 }
 ```
 > S. R. Jha, S. Chowdhury, M. Hays, J. A. Grover, W. D. Oliver. An auto differentiable and hardware accelerated software toolkit for quantum circuit design, simulation and control (2024), in preparation.
 
 
 ## Contributions & Contact
```

### Comparing `jaxquantum-0.1.0/jaxquantum.egg-info/SOURCES.txt` & `jaxquantum-0.1.1/jaxquantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxquantum-0.1.0/setup.py` & `jaxquantum-0.1.1/setup.py`

 * *Files identical despite different names*

