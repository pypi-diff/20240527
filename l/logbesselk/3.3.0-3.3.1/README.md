# Comparing `tmp/logbesselk-3.3.0.tar.gz` & `tmp/logbesselk-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logbesselk-3.3.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `logbesselk-3.3.0.tar` & `logbesselk-3.3.1.tar`

### file list

```diff
@@ -1,27 +1,51 @@
--rw-r--r--   0        0        0    11357 2024-05-25 17:20:21.509063 logbesselk-3.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2265 2024-05-25 17:20:21.509063 logbesselk-3.3.0/README.md
--rw-r--r--   0        0        0     2091 2024-05-25 17:20:21.525063 logbesselk-3.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/__init__.py
--rw-r--r--   0        0        0      220 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/__init__.py
--rw-r--r--   0        0        0     1800 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/asymptotic.py
--rw-r--r--   0        0        0     1812 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/cfraction.py
--rw-r--r--   0        0        0     1667 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/ica.py
--rw-r--r--   0        0        0     2603 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/integral.py
--rw-r--r--   0        0        0     1714 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/math.py
--rw-r--r--   0        0        0      781 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/misc.py
--rw-r--r--   0        0        0     1788 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/sca.py
--rw-r--r--   0        0        0     2412 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/series.py
--rw-r--r--   0        0        0     2358 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/utils.py
--rw-r--r--   0        0        0     2423 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/wrap.py
--rw-r--r--   0        0        0      283 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/__init__.py
--rw-r--r--   0        0        0     1977 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/asymptotic.py
--rw-r--r--   0        0        0     1913 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/cfraction.py
--rw-r--r--   0        0        0     2729 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/integral.py
--rw-r--r--   0        0        0     1992 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/math.py
--rw-r--r--   0        0        0      876 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/misc.py
--rw-r--r--   0        0        0     1874 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/sca.py
--rw-r--r--   0        0        0     2485 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/series.py
--rw-r--r--   0        0        0     3272 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/utils.py
--rw-r--r--   0        0        0     2194 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/wrap.py
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 logbesselk-3.3.0/setup.py
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 logbesselk-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 logbesselk-3.3.1/requirements-dev.lock
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 logbesselk-3.3.1/requirements.lock
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 logbesselk-3.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 logbesselk-3.3.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 logbesselk-3.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 logbesselk-3.3.1/.github/workflows/upload.yml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/eval_jax.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/eval_tensorflow.py
+-rw-r--r--   0        0        0   552752 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/data/dlogkdv_mathematica.csv
+-rw-r--r--   0        0        0   563711 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/data/dlogkdx_mathematica.csv
+-rw-r--r--   0        0        0   567279 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/data/ke_mathematica.csv
+-rw-r--r--   0        0        0   553117 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/data/kratio_mathematica.csv
+-rw-r--r--   0        0        0   552053 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/data/log_dkdv_mathematica.csv
+-rw-r--r--   0        0        0   556808 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/data/log_dkdx_mathematica.csv
+-rw-r--r--   0        0        0   538917 2020-02-02 00:00:00.000000 logbesselk-3.3.1/eval/data/logk_mathematica.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/__init__.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/asymptotic.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/cfraction.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/ica.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/integral.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/math.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/misc.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/sca.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/series.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/utils.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/jax/wrap.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/__init__.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/asymptotic.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/cfraction.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/ica.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/integral.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/math.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/misc.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/sca.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/series.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/utils.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 logbesselk-3.3.1/src/logbesselk/tensorflow/wrap.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/test_jax.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/test_tensorflow.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/data/dlogkdx.csv
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/data/ke.csv
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/data/log_abs_dkdv.csv
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/data/log_abs_dkdx.csv
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 logbesselk-3.3.1/tests/data/log_k.csv
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 logbesselk-3.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 logbesselk-3.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 logbesselk-3.3.1/README.md
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 logbesselk-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 logbesselk-3.3.1/PKG-INFO
```

### Comparing `logbesselk-3.3.0/LICENSE.txt` & `logbesselk-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/README.md` & `logbesselk-3.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 ## Author
 TAKEKAWA Takashi <takekawa@tk2lab.org>
 
 
 ## For Tensorflow
 
 ### Require
-- Python (>=3.8)
-- Tensorflow (>=2.6)
+- Python (>=3.10)
+- Tensorflow (>=2.8)
 
 ### Installation
 ```shell
 pip install tensorflow logbesselk
 ```
 
 ### Examples
 ```python
 import tensorflow as tf
 from logbesselk.tensorflow import log_bessel_k as logk
-from logbesselk.jax import bessel_ke as ke
-from logbesselk.jax import bessel_kratio as kratio
+from logbesselk.tensorflow import bessel_ke as ke
+from logbesselk.tensorflow import bessel_kratio as kratio
 
 v = 1.0
 x = 1.0
 a = logk(v, x)
 
-v = jnp.linspace(1, 10, 10)
-x = jnp.linspace(1, 10, 10)
+v = tf.linspace(1, 10, 10)
+x = tf.linspace(1, 10, 10)
 b = logk(v, x)
 
 # gradient
 with tf.GradientTape() as g:
     g.watch(v, x)
     f = logk(v, x)
 dlogkdv = g.gradient(f, v)
@@ -54,16 +54,16 @@
 logdkdx = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 1)
 ```
 
 
 ## For jax
 
 ### Require
-- Python (>=3.8)
-- jax (>=0.3)
+- Python (>=3.10)
+- jax (>=0.4)
 
 ### Installation
 ```shell
 pip install jax[cuda] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 pip install logbesselk
 ```
```

### Comparing `logbesselk-3.3.0/pyproject.toml` & `logbesselk-3.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,115 @@
-[tool.poetry]
+[project]
 name = "logbesselk"
-version = "3.3.0"
+version = "3.3.1"
 description = "Provide function to calculate the modified Bessel function of the second kind"
 license = "Apache-2.0"
-authors = ["TAKEKAWA Takashi <takekawa@tk2lab.org>"]
+authors = [
+    { name = "TAKEKAWA Takashi", email = "takekawa@tk2lab.org" }
+]
 readme = "README.md"
 repository = "https://github.com/tk2lab/logbesselk"
+classifiers = [
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
+
+requires-python = ">=3.10"
+
+[project.optional-dependences]
+jax = [
+    "jax>=0.4",
+    "jaxlib>=0.4",
+]
+tensorflow = [
+    "tensorflow>=2.8",
+]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.rye]
+manaed = true
 
-[tool.poetry.dependencies]
-python = ">=3.8,<3.13"
-#tensorflow = ">=2.6,<2.12"
-#jax = "^0.2+cuda"
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-force_grid_wrap = 1
-
-[tool.flake8]
-max-line-length = 88
-extend-ignore = ["E203"]
+[[tool.rye.sources]]
+name = "jax"
+url = "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
+type = "find-links"
 
 [tool.pytest.ini_options]
 markers = [
     "vec",
 ]
 
+[tool.ruff]
+target-version = "py310"
+
+[tool.ruff.format]
+quote-style = "single"
+
+[tool.ruff.lint]
+select = ["E4", "E7", "E9", "F", "W", "N", "I"]
+
+[ttol.ruff.lint.per-file-ignores]
+"__init__.py" = ["F401"]
+
+[tool.ruff.lint.isort]
+combine-as-imports = true
+force-wrap-aliases = true
+split-on-trailing-comma = true
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 min_version = 4.0
-isolated_build = True
+rye_discovery = true
 env_list = 
-    py{310,311,312}-jax{3,4}
-    py{310,311,312}-tf{29,210,211,212,213,214,215,216}
-    lint
+    py{310,311,312}-jax{latest,4}
+    py{310,311}-tf{latest,28,29,210,211,212,213,214,215,216}
+    py312-tf{latest,216}
     eval_tf
     eval_jax
 
 [gh-actions]
 python =
-    3.10: py310-jax3, py310-tf29
-    3.12: py312-jax4, py312-tf216
+    3.10: py310-jax4, py310-tf28
+    3.12: py312-jaxlatest, py312-tflatest
 
-[testenv:py{310,311,312}-jax{3,4}]
+[testenv:py{310,311,312}-jax{4,latest}]
 deps =
-    jax3: jax[cuda] (>=0.3,<0.4)
-    jax4: jax[cuda] (>=0.4,<0.5)
+    jaxlatest: jax[cuda12]
+    jax4: jax[cuda12] (>=0.4,<0.5)
     pytest
     pandas
-install_command =
-    pip install --upgrade -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html {opts} {packages}
 commands =
     {envpython} -m pytest tests/test_jax.py {posargs}
 
-[testenv:py{310,311,312}-tf{29,210,211,212,213,214,215,216}]
+[testenv:py{310,311,312}-tf{latest,28,29,210,211,212,213,214,215,216}]
 deps =
-    tf29: tensorflow (>=2.9,<2.10)
-    tf210: tensorflow (>=2.10,<2.11)
-    tf211: tensorflow (>=2.11,<2.12)
-    tf212: tensorflow (>=2.12,<2.13)
-    tf213: tensorflow (>=2.13,<2.14)
-    tf214: tensorflow (>=2.14,<2.15)
-    tf215: tensorflow (>=2.15,<2.16)
+    tflatest: tensorflow
     tf216: tensorflow (>=2.16,<2.17)
+    tf215: tensorflow (>=2.15,<2.16)
+    tf214: tensorflow (>=2.14,<2.15)
+    tf213: tensorflow (>=2.13,<2.14)
+    tf212: tensorflow (>=2.12,<2.13)
+    tf211: tensorflow (>=2.11,<2.12)
+    tf210: tensorflow (>=2.10,<2.11)
+    tf29: tensorflow (>=2.9,<2.10)
+    tf28: tensorflow (>=2.8,<2.9)
     pytest
     pandas
 commands =
     {envpython} -m pytest tests/test_tensorflow.py {posargs}
 
 [testenv:eval_jax]
 deps =
-    jax[cuda]
+    jax[cuda12]
     pandas
-install_command =
-    pip install --upgrade -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html {opts} {packages}
 commands =
     {envpython} eval/eval_jax.py
 
 [testenv:eval_tf]
 deps =
     tensorflow
     pandas
```

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/asymptotic.py` & `logbesselk-3.3.1/src/logbesselk/jax/asymptotic.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/cfraction.py` & `logbesselk-3.3.1/src/logbesselk/jax/cfraction.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/ica.py` & `logbesselk-3.3.1/src/logbesselk/jax/ica.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/integral.py` & `logbesselk-3.3.1/src/logbesselk/jax/integral.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/math.py` & `logbesselk-3.3.1/src/logbesselk/jax/math.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/misc.py` & `logbesselk-3.3.1/src/logbesselk/jax/misc.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/sca.py` & `logbesselk-3.3.1/src/logbesselk/jax/sca.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/series.py` & `logbesselk-3.3.1/src/logbesselk/jax/series.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/utils.py` & `logbesselk-3.3.1/src/logbesselk/jax/utils.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/jax/wrap.py` & `logbesselk-3.3.1/src/logbesselk/jax/wrap.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/asymptotic.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/asymptotic.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/cfraction.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/cfraction.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/integral.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/integral.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/math.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/misc.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/misc.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/sca.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/sca.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/series.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/series.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/utils.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/src/logbesselk/tensorflow/wrap.py` & `logbesselk-3.3.1/src/logbesselk/tensorflow/wrap.py`

 * *Files identical despite different names*

### Comparing `logbesselk-3.3.0/PKG-INFO` & `logbesselk-3.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: logbesselk
-Version: 3.3.0
+Version: 3.3.1
 Summary: Provide function to calculate the modified Bessel function of the second kind
-Home-page: https://github.com/tk2lab/logbesselk
-License: Apache-2.0
-Author: TAKEKAWA Takashi
-Author-email: takekawa@tk2lab.org
-Requires-Python: >=3.8,<3.13
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Author-email: TAKEKAWA Takashi <takekawa@tk2lab.org>
+License-Expression: Apache-2.0
+License-File: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Project-URL: Repository, https://github.com/tk2lab/logbesselk
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # logbesselk
 Provide function to calculate the modified Bessel function of the second kind
 and its derivatives.
 
 ## Reference
@@ -27,35 +22,35 @@
 ## Author
 TAKEKAWA Takashi <takekawa@tk2lab.org>
 
 
 ## For Tensorflow
 
 ### Require
-- Python (>=3.8)
-- Tensorflow (>=2.6)
+- Python (>=3.10)
+- Tensorflow (>=2.8)
 
 ### Installation
 ```shell
 pip install tensorflow logbesselk
 ```
 
 ### Examples
 ```python
 import tensorflow as tf
 from logbesselk.tensorflow import log_bessel_k as logk
-from logbesselk.jax import bessel_ke as ke
-from logbesselk.jax import bessel_kratio as kratio
+from logbesselk.tensorflow import bessel_ke as ke
+from logbesselk.tensorflow import bessel_kratio as kratio
 
 v = 1.0
 x = 1.0
 a = logk(v, x)
 
-v = jnp.linspace(1, 10, 10)
-x = jnp.linspace(1, 10, 10)
+v = tf.linspace(1, 10, 10)
+x = tf.linspace(1, 10, 10)
 b = logk(v, x)
 
 # gradient
 with tf.GradientTape() as g:
     g.watch(v, x)
     f = logk(v, x)
 dlogkdv = g.gradient(f, v)
@@ -72,16 +67,16 @@
 logdkdx = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 1)
 ```
 
 
 ## For jax
 
 ### Require
-- Python (>=3.8)
-- jax (>=0.3)
+- Python (>=3.10)
+- jax (>=0.4)
 
 ### Installation
 ```shell
 pip install jax[cuda] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 pip install logbesselk
 ```
 
@@ -125,8 +120,7 @@
 
 log_dkdv = lambda v, x: log_abs_deriv_bessel_k(v, x, 1, 0)
 log_dkdx = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 1)
 
 log_dkdv_jit = jax.jit(jax.vmap(log_dkdv))
 log_dkdx_jit = jax.jit(jax.vmap(log_dkdx))
 ```
-
```

