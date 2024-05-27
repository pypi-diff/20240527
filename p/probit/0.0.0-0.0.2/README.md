# Comparing `tmp/probit-0.0.0.tar.gz` & `tmp/probit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probit-0.0.0.tar", last modified: Tue Jan 24 11:23:21 2023, max compression
+gzip compressed data, was "probit-0.0.2.tar", last modified: Mon May 27 15:37:17 2024, max compression
```

## Comparing `probit-0.0.0.tar` & `probit-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.821372 probit-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-24 11:23:00.000000 probit-0.0.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.813371 probit-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.817371 probit-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-24 11:23:00.000000 probit-0.0.0/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-24 11:23:00.000000 probit-0.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-24 11:23:00.000000 probit-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-24 11:23:00.000000 probit-0.0.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-24 11:23:00.000000 probit-0.0.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-01-24 11:23:21.821372 probit-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-01-24 11:23:00.000000 probit-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.817371 probit-0.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-01-24 11:23:00.000000 probit-0.0.0/examples/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-01-24 11:23:00.000000 probit-0.0.0/examples/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.821372 probit-0.0.0/probit/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-24 11:23:00.000000 probit-0.0.0/probit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-24 11:23:21.000000 probit-0.0.0/probit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-01-24 11:23:00.000000 probit-0.0.0/probit/approximators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.821372 probit-0.0.0/probit/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-01-24 11:23:00.000000 probit-0.0.0/probit/implicit/Laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-01-24 11:23:00.000000 probit-0.0.0/probit/implicit/VB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-01-24 11:23:00.000000 probit-0.0.0/probit/implicit/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.821372 probit-0.0.0/probit/test/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-24 11:23:00.000000 probit-0.0.0/probit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-24 11:23:00.000000 probit-0.0.0/probit/test/test_implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-01-24 11:23:00.000000 probit-0.0.0/probit/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:23:21.821372 probit-0.0.0/probit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-01-24 11:23:21.000000 probit-0.0.0/probit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-24 11:23:21.000000 probit-0.0.0/probit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 11:23:21.000000 probit-0.0.0/probit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-24 11:23:21.000000 probit-0.0.0/probit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-24 11:23:21.000000 probit-0.0.0/probit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-24 11:23:00.000000 probit-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    38783 2023-01-24 11:23:00.000000 probit-0.0.0/readme_classification_after_contour.png
--rw-r--r--   0 runner    (1001) docker     (123)    84704 2023-01-24 11:23:00.000000 probit-0.0.0/readme_classification_after_mean_variance.png
--rw-r--r--   0 runner    (1001) docker     (123)    28466 2023-01-24 11:23:00.000000 probit-0.0.0/readme_classification_before_contour.png
--rw-r--r--   0 runner    (1001) docker     (123)    75562 2023-01-24 11:23:00.000000 probit-0.0.0/readme_classification_before_mean_variance.png
--rw-r--r--   0 runner    (1001) docker     (123)    43740 2023-01-24 11:23:00.000000 probit-0.0.0/readme_grad.png
--rw-r--r--   0 runner    (1001) docker     (123)    32220 2023-01-24 11:23:00.000000 probit-0.0.0/readme_objective.png
--rw-r--r--   0 runner    (1001) docker     (123)    51360 2023-01-24 11:23:00.000000 probit-0.0.0/readme_regression_after.png
--rw-r--r--   0 runner    (1001) docker     (123)    59059 2023-01-24 11:23:00.000000 probit-0.0.0/readme_regression_before.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-24 11:23:00.000000 probit-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 11:23:21.821372 probit-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-24 11:23:00.000000 probit-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.526822 probit-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-27 15:36:53.000000 probit-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.514822 probit-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.522822 probit-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-27 15:36:53.000000 probit-0.0.2/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-27 15:36:53.000000 probit-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-27 15:36:53.000000 probit-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 15:36:53.000000 probit-0.0.2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-27 15:36:53.000000 probit-0.0.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-05-27 15:37:17.526822 probit-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-27 15:36:53.000000 probit-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.522822 probit-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    15519 2024-05-27 15:36:53.000000 probit-0.0.2/examples/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-27 15:36:53.000000 probit-0.0.2/examples/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.522822 probit-0.0.2/probit/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 15:36:53.000000 probit-0.0.2/probit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 15:37:17.000000 probit-0.0.2/probit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-27 15:36:53.000000 probit-0.0.2/probit/approximators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.522822 probit-0.0.2/probit/implicit/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-27 15:36:53.000000 probit-0.0.2/probit/implicit/Laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-27 15:36:53.000000 probit-0.0.2/probit/implicit/VB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-27 15:36:53.000000 probit-0.0.2/probit/implicit/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.522822 probit-0.0.2/probit/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 15:36:53.000000 probit-0.0.2/probit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-27 15:36:53.000000 probit-0.0.2/probit/test/test_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11762 2024-05-27 15:36:53.000000 probit-0.0.2/probit/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:37:17.526822 probit-0.0.2/probit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-05-27 15:37:17.000000 probit-0.0.2/probit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-27 15:37:17.000000 probit-0.0.2/probit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:37:17.000000 probit-0.0.2/probit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 15:37:17.000000 probit-0.0.2/probit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 15:37:17.000000 probit-0.0.2/probit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-27 15:36:53.000000 probit-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    38783 2024-05-27 15:36:53.000000 probit-0.0.2/readme_classification_after_contour.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84720 2024-05-27 15:36:53.000000 probit-0.0.2/readme_classification_after_mean_variance.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28466 2024-05-27 15:36:53.000000 probit-0.0.2/readme_classification_before_contour.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75616 2024-05-27 15:36:53.000000 probit-0.0.2/readme_classification_before_mean_variance.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43740 2024-05-27 15:36:53.000000 probit-0.0.2/readme_grad.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-27 15:36:53.000000 probit-0.0.2/readme_nplan.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32220 2024-05-27 15:36:53.000000 probit-0.0.2/readme_objective.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51360 2024-05-27 15:36:53.000000 probit-0.0.2/readme_regression_after.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59059 2024-05-27 15:36:53.000000 probit-0.0.2/readme_regression_before.png
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-27 15:36:53.000000 probit-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:37:17.526822 probit-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-27 15:36:53.000000 probit-0.0.2/setup.py
```

### Comparing `probit-0.0.0/.github/workflows/CI.yml` & `probit-0.0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/.github/workflows/publish.yml` & `probit-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/.gitignore` & `probit-0.0.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Autogenerated files
-sgm/_version.py
+probit/_version.py
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `probit-0.0.0/LICENSE.rst` & `probit-0.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/PKG-INFO` & `probit-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: probit
-Version: 0.0.0
-Summary: probit is a simple and accessible Gaussian process implementation in Jax.
+Version: 0.0.2
+Summary: probit is a simple and accessible Gaussian process implementation in Jax
 Home-page: https://github.com/bb515/probit
 Author: Benjamin Boys, Toby Boyne, Ieronymos Maxoutis
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: jaxopt>=0.5.5
+Requires-Dist: backends>=1.4.32
+Requires-Dist: mlkernels>=0.3.6
 
 # [probit](http://github.com/bb515/probit)
 [![CI](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml/badge.svg)](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml)
 [![Coverage Status](https://coveralls.io/repos/github/bb515/diffusionjax/badge.svg?branch=master)](https://coveralls.io/github/bb515/diffusionjax?branch=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-probit is a simple and accessible Gaussian process package in Jax.
+![nPlan](readme_nplan.png)
+
+probit is a simple and accessible Gaussian process package in JAX. Thank you to [nPlan](https://www.nplan.io/), who are supporting this project.
 
 probit uses [MLKernels](https://github.com/wesselb/mlkernels) for the GP prior, see the available [means](https://github.com/wesselb/mlkernels#available-means) and [kernels](https://github.com/wesselb/mlkernels#available-kernels) with [compositional design](https://github.com/wesselb/mlkernels#compositional-design).
 
 Contents:
 
 - [Installation](#installation)
 - [Examples](#examples)
@@ -36,32 +43,34 @@
 >>>     lengthscale, signal_variance = prior_parameters
 >>>     # Here you can define the kernel that defines the Gaussian process
 >>>     return signal_variance * EQ().stretch(lengthscale).periodic(0.5)
 >>>
 >>> gaussian_process = GP(data=(X, y), prior=prior, log_likelihood=log_gaussian_likelihood)
 >>> likelihood_parameters = 1.0
 >>> prior_parameters = (1.0, 1.0)
->>> parameters = (likelihood_parameters, prior_parameters)
+>>> parameters = (prior_parameters, likelihood_parameters)
 >>> weight, precision = gaussian_process.approximate_posterior(parameters)
 >>> predictive_mean, predictive_variance = gaussian_process.predict(
 >>>     X_test,
 >>>     parameters, weight, precision)
 ```
 
-
 ## Installation
-`pip install probit` or for developers,
+The package requires Python 3.8+. First, it is recommended to [create a new python virtual environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). 
+probit depends on JAX. Because the JAX installation is different depending on your CUDA version, probit does not list JAX as a dependency in `setup.py`.
+First, [follow these instructions](https://github.com/google/jax#installation) to install JAX with the relevant accelerator support.
+Then, `pip install probit` or for developers,
 - Clone the repository `git clone git@github.com:bb515/probit.git`
 - Install using pip `pip install -e .` from the root directory of the repository (see the `setup.py` for the requirements that this command installs)
 
 ## Examples
 You can find examples of how to use the package under:`examples/`.
 
 ### Regression and hyperparameter optimization
-Run the regression example by typing `python example/regression.py`.
+Run the regression example by typing `python examples/regression.py`.
 ```python
 >>> def prior(prior_parameters):
 >>>     lengthscale, signal_variance = prior_parameters
 >>>     # Here you can define the kernel that defines the Gaussian process
 >>>     return signal_variance * EQ().stretch(lengthscale).periodic(0.5)
 >>>
 >>> # Generate data
@@ -114,15 +123,15 @@
 >>> noise_variance = vs.struct.noise_std()**2
 >>> obs_variance = variance + noise_variance
 >>> plot((X, y), (X_show, f_show), mean, obs_variance, fname="readme_regression_after.png")
 ```
 ![Prediction](readme_regression_after.png)
 
 ### Ordinal regression and hyperparameter optimization
-Run the ordinal regression example by typing `python example/classification.py`.
+Run the ordinal regression example by typing `python examples/classification.py`.
 
 ```python
 >>> # Generate data
 >>> J = 3  # use a value of J=2 for GP binary classification
 >>> key = random.PRNGKey(1)
 >>> noise_variance = 0.4
 >>> signal_variance = 1.0
@@ -172,15 +181,14 @@
 >>>     obs_variance, X_show, f_show, X, y, g_true,
 >>>     J, colors, fname="readme_classification_before")
 ```
 ![Prediction](readme_classification_before_contour.png)
 ![Prediction](readme_classification_before_mean_variance.png)
 
 ```python
->>>
 >>> # Evaluate model
 >>> mean, variance = classifier.predict(
 >>>     X_test,
 >>>     parameters,
 >>>     weight, precision)
 >>> predictive_distributions = probit_predictive_distributions(
 >>>     parameters[1],
@@ -195,23 +203,21 @@
 mean_absolute_error=0.41\
 log_pred_probability=-140986.54\
 mean_zero_one_error=0.39
 
 Before optimization, 
 parameters=(Array(1.2, dtype=float32), (Array(0.63245553, dtype=float64, weak_type=True), Array([       -inf, -0.54599167,  0.50296235,         inf], dtype=float64)))
 ```python
->>>
 >>> minimise_l_bfgs_b(objective, vs)
 >>> parameters = model(vs)
 >>> print("After optimization, \nparameters={}".format(model(vs)))
 ```
 After optimization, 
 parameters=(Array(0.07389855, dtype=float32), (Array(0.63245553, dtype=float64, weak_type=True), Array([       -inf, -0.54599167,  0.50296235,         inf], dtype=float64)))
 ```python
->>>
 >>> # Approximate posterior
 >>> parameters = model(vs)
 >>> weight, precision = classifier.approximate_posterior(parameters)
 >>> mean, variance = classifier.predict(
 >>>     X_show,
 >>>     parameters,
 >>>     weight, precision)
@@ -295,8 +301,7 @@
   author = 	 {King, Nathaniel J. and Lawrence, Neil D.},\
   year = 	 {2005},\
   number = {CS-05-06},\
   url = 	 {http://inverseprobability.com/publications/king-ppa05.html}}
 
 An [implicit functions tutorial](http://implicit-layers-tutorial.org/implicit_functions/) was used to define the fixed-point layer.
 
-
```

### Comparing `probit-0.0.0/README.md` & `probit-0.0.2/probit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,30 @@
+Metadata-Version: 2.1
+Name: probit
+Version: 0.0.2
+Summary: probit is a simple and accessible Gaussian process implementation in Jax
+Home-page: https://github.com/bb515/probit
+Author: Benjamin Boys, Toby Boyne, Ieronymos Maxoutis
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: jaxopt>=0.5.5
+Requires-Dist: backends>=1.4.32
+Requires-Dist: mlkernels>=0.3.6
+
 # [probit](http://github.com/bb515/probit)
 [![CI](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml/badge.svg)](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml)
 [![Coverage Status](https://coveralls.io/repos/github/bb515/diffusionjax/badge.svg?branch=master)](https://coveralls.io/github/bb515/diffusionjax?branch=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-probit is a simple and accessible Gaussian process package in Jax.
+![nPlan](readme_nplan.png)
+
+probit is a simple and accessible Gaussian process package in JAX. Thank you to [nPlan](https://www.nplan.io/), who are supporting this project.
 
 probit uses [MLKernels](https://github.com/wesselb/mlkernels) for the GP prior, see the available [means](https://github.com/wesselb/mlkernels#available-means) and [kernels](https://github.com/wesselb/mlkernels#available-kernels) with [compositional design](https://github.com/wesselb/mlkernels#compositional-design).
 
 Contents:
 
 - [Installation](#installation)
 - [Examples](#examples)
@@ -26,32 +43,34 @@
 >>>     lengthscale, signal_variance = prior_parameters
 >>>     # Here you can define the kernel that defines the Gaussian process
 >>>     return signal_variance * EQ().stretch(lengthscale).periodic(0.5)
 >>>
 >>> gaussian_process = GP(data=(X, y), prior=prior, log_likelihood=log_gaussian_likelihood)
 >>> likelihood_parameters = 1.0
 >>> prior_parameters = (1.0, 1.0)
->>> parameters = (likelihood_parameters, prior_parameters)
+>>> parameters = (prior_parameters, likelihood_parameters)
 >>> weight, precision = gaussian_process.approximate_posterior(parameters)
 >>> predictive_mean, predictive_variance = gaussian_process.predict(
 >>>     X_test,
 >>>     parameters, weight, precision)
 ```
 
-
 ## Installation
-`pip install probit` or for developers,
+The package requires Python 3.8+. First, it is recommended to [create a new python virtual environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). 
+probit depends on JAX. Because the JAX installation is different depending on your CUDA version, probit does not list JAX as a dependency in `setup.py`.
+First, [follow these instructions](https://github.com/google/jax#installation) to install JAX with the relevant accelerator support.
+Then, `pip install probit` or for developers,
 - Clone the repository `git clone git@github.com:bb515/probit.git`
 - Install using pip `pip install -e .` from the root directory of the repository (see the `setup.py` for the requirements that this command installs)
 
 ## Examples
 You can find examples of how to use the package under:`examples/`.
 
 ### Regression and hyperparameter optimization
-Run the regression example by typing `python example/regression.py`.
+Run the regression example by typing `python examples/regression.py`.
 ```python
 >>> def prior(prior_parameters):
 >>>     lengthscale, signal_variance = prior_parameters
 >>>     # Here you can define the kernel that defines the Gaussian process
 >>>     return signal_variance * EQ().stretch(lengthscale).periodic(0.5)
 >>>
 >>> # Generate data
@@ -104,15 +123,15 @@
 >>> noise_variance = vs.struct.noise_std()**2
 >>> obs_variance = variance + noise_variance
 >>> plot((X, y), (X_show, f_show), mean, obs_variance, fname="readme_regression_after.png")
 ```
 ![Prediction](readme_regression_after.png)
 
 ### Ordinal regression and hyperparameter optimization
-Run the ordinal regression example by typing `python example/classification.py`.
+Run the ordinal regression example by typing `python examples/classification.py`.
 
 ```python
 >>> # Generate data
 >>> J = 3  # use a value of J=2 for GP binary classification
 >>> key = random.PRNGKey(1)
 >>> noise_variance = 0.4
 >>> signal_variance = 1.0
@@ -162,15 +181,14 @@
 >>>     obs_variance, X_show, f_show, X, y, g_true,
 >>>     J, colors, fname="readme_classification_before")
 ```
 ![Prediction](readme_classification_before_contour.png)
 ![Prediction](readme_classification_before_mean_variance.png)
 
 ```python
->>>
 >>> # Evaluate model
 >>> mean, variance = classifier.predict(
 >>>     X_test,
 >>>     parameters,
 >>>     weight, precision)
 >>> predictive_distributions = probit_predictive_distributions(
 >>>     parameters[1],
@@ -185,23 +203,21 @@
 mean_absolute_error=0.41\
 log_pred_probability=-140986.54\
 mean_zero_one_error=0.39
 
 Before optimization, 
 parameters=(Array(1.2, dtype=float32), (Array(0.63245553, dtype=float64, weak_type=True), Array([       -inf, -0.54599167,  0.50296235,         inf], dtype=float64)))
 ```python
->>>
 >>> minimise_l_bfgs_b(objective, vs)
 >>> parameters = model(vs)
 >>> print("After optimization, \nparameters={}".format(model(vs)))
 ```
 After optimization, 
 parameters=(Array(0.07389855, dtype=float32), (Array(0.63245553, dtype=float64, weak_type=True), Array([       -inf, -0.54599167,  0.50296235,         inf], dtype=float64)))
 ```python
->>>
 >>> # Approximate posterior
 >>> parameters = model(vs)
 >>> weight, precision = classifier.approximate_posterior(parameters)
 >>> mean, variance = classifier.predict(
 >>>     X_show,
 >>>     parameters,
 >>>     weight, precision)
@@ -285,8 +301,7 @@
   author = 	 {King, Nathaniel J. and Lawrence, Neil D.},\
   year = 	 {2005},\
   number = {CS-05-06},\
   url = 	 {http://inverseprobability.com/publications/king-ppa05.html}}
 
 An [implicit functions tutorial](http://implicit-layers-tutorial.org/implicit_functions/) was used to define the fixed-point layer.
 
-
```

### Comparing `probit-0.0.0/examples/classification.py` & `probit-0.0.2/examples/classification.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,146 +1,197 @@
 """Ordinal GP regression via approximate inference."""
+
 # Uncomment to enable double precision
 from jax.config import config
+
 config.update("jax_enable_x64", True)
 
 from probit.utilities import (
-    InvalidKernel, check_cutpoints,
-    log_probit_likelihood, probit_predictive_distributions)
+    InvalidKernel,
+    check_cutpoints,
+    log_probit_likelihood,
+    probit_predictive_distributions,
+)
 import numpy as np
 import lab as B
 import jax.numpy as jnp
 import jax.random as random
 from mlkernels import Kernel, Matern12, EQ
-from varz import Vars, minimise_l_bfgs_b, parametrised, Positive
+from varz import Vars, minimise_l_bfgs_b
 import matplotlib.pyplot as plt
 import argparse
 import cProfile
 from io import StringIO
 from pstats import Stats, SortKey
 import pathlib
-import matplotlib.cm as cm
-from scipy.optimize import minimize
 from jax import vmap, value_and_grad
 
 # For plotting
 BG_ALPHA = 1.0
 MG_ALPHA = 1.0
 FG_ALPHA = 0.3
 
 write_path = pathlib.Path()
 
 
-def plot(x, predictive_distributions, mean,
-         variance, X_show, f_show, X_train, y_train, g_train,
-         J, colors, fname="plot"):
+def plot(
+    x,
+    predictive_distributions,
+    mean,
+    variance,
+    X_show,
+    f_show,
+    X_train,
+    y_train,
+    g_train,
+    J,
+    colors,
+    fname="plot",
+):
     posterior_std = jnp.sqrt(variance)
     fig, ax = plt.subplots(1, 1)
-    fig.patch.set_facecolor('white')
+    fig.patch.set_facecolor("white")
     fig.patch.set_alpha(BG_ALPHA)
     ax.set_xlim((-0.5, 1.5))
     ax.set_ylim(0.0, 1.0)
     ax.set_xlabel(r"$x$", fontsize=10)
     ax.set_ylabel("Cumulative probability", fontsize=10)
-    ax.stackplot(x[:, 0], predictive_distributions.T, colors=colors,
+    ax.stackplot(
+        x[:, 0],
+        predictive_distributions.T,
+        colors=colors,
         labels=(
             r"$p(y=0|\mathcal{D}, \theta)$",
             r"$p(y=1|\mathcal{D}, \theta)$",
-            r"$p(y=2|\mathcal{D}, \theta)$"))
+            r"$p(y=2|\mathcal{D}, \theta)$",
+        ),
+    )
     val = 0.5  # where the data lies on the y-axis.
     plt.tight_layout()
     ax.legend()
-    fig.savefig(
-            "{}_contour.png".format(fname))
+    fig.savefig("{}_contour.png".format(fname))
     plt.close()
 
     fig, ax = plt.subplots(1, 1)
-    fig.patch.set_facecolor('white')
+    fig.patch.set_facecolor("white")
     fig.patch.set_alpha(BG_ALPHA)
-    ax.plot(x[:, 0], mean, color='blue', label="Prediction", linestyle="--")
+    ax.plot(x[:, 0], mean, color="blue", label="Prediction", linestyle="--")
     ax.fill_between(
-        x[:, 0], mean - 2*posterior_std,
-        mean + 2*posterior_std,
-        color='blue', alpha=FG_ALPHA)
+        x[:, 0],
+        mean - 2 * posterior_std,
+        mean + 2 * posterior_std,
+        color="blue",
+        alpha=FG_ALPHA,
+    )
     ax.set_ylim(-2.2, 2.2)
     ax.set_xlim(-0.5, 1.5)
-    ax.set_xlabel('x', fontsize=10)
-    ax.set_ylabel('y', fontsize=10)
-    ax.scatter(X_train, g_train, color=[colors[i] for i in y_train], s=4, label="Observations")
-    ax.plot(X_show, f_show, label="True", color='orange', alpha=FG_ALPHA)
-    ax.grid(visible=True, which='major', linestyle='-')
+    ax.set_xlabel("x", fontsize=10)
+    ax.set_ylabel("y", fontsize=10)
+    ax.scatter(
+        X_train, g_train, color=[colors[i] for i in y_train], s=4, label="Observations"
+    )
+    ax.plot(X_show, f_show, label="True", color="orange", alpha=FG_ALPHA)
+    ax.grid(visible=True, which="major", linestyle="-")
     ax.legend()
     plt.tight_layout()
-    fig.savefig("{}_mean_variance.png".format(fname),
-        facecolor=fig.get_facecolor(), edgecolor='none')
+    fig.savefig(
+        "{}_mean_variance.png".format(fname),
+        facecolor=fig.get_facecolor(),
+        edgecolor="none",
+    )
     plt.close()
 
 
 def plot_obj(x_hat, x_0, x, fs, gs, domain, xlabel, xscale, fname="plot"):
     # Calculate numerical derivatives wrt domain of plot
     if xscale == "log":
         log_x = jnp.log(x)
         dfsx = np.gradient(fs, log_x)
         gs *= x  # Jacobian
     elif xscale == "linear":
         dfsx = np.gradient(fs, x)
     fig = plt.figure()
-    fig.patch.set_facecolor('white')
+    fig.patch.set_facecolor("white")
     fig.patch.set_alpha(BG_ALPHA)
     ax = fig.add_subplot(111)
     ax.grid()
-    ax.plot(x, fs, 'g', label=r"$\mathcal{F}$ autodiff")
+    ax.plot(x, fs, "g", label=r"$\mathcal{F}$ autodiff")
     ylim = ax.get_ylim()
-    ax.set_xlim((10**domain[0][0], 10**domain[0][1]))
+    ax.set_xlim((10 ** domain[0][0], 10 ** domain[0][1]))
     ax.set_ylim(ylim)
-    ax.vlines(x_hat, ylim[0], ylim[1], 'r',
-        alpha=MG_ALPHA, label=r"$\hat\theta={:.2f}$".format(x_hat))
-    ax.vlines(x_0, ylim[0], ylim[1], 'k',
-        alpha=MG_ALPHA, label=r"$\theta={:.2f}$".format(x_0))
+    ax.vlines(
+        x_hat,
+        ylim[0],
+        ylim[1],
+        "r",
+        alpha=MG_ALPHA,
+        label=r"$\hat\theta={:.2f}$".format(x_hat),
+    )
+    ax.vlines(
+        x_0, ylim[0], ylim[1], "k", alpha=MG_ALPHA, label=r"$\theta={:.2f}$".format(x_0)
+    )
     ax.set_xlabel(xlabel, fontsize=10)
     ax.set_xscale(xscale)
     ax.set_ylabel(r"$\mathcal{F}$", fontsize=10)
-    ax.set_title('Hyper-parameter optimisation objective')
+    ax.set_title("Hyper-parameter optimisation objective")
     ax.legend()
-    fig.savefig("readme_objective.png",
-        facecolor=fig.get_facecolor(), edgecolor='none')
+    fig.savefig("readme_objective.png", facecolor=fig.get_facecolor(), edgecolor="none")
     plt.close()
 
     fig = plt.figure()
-    fig.patch.set_facecolor('white')
+    fig.patch.set_facecolor("white")
     fig.patch.set_alpha(BG_ALPHA)
     ax = fig.add_subplot(111)
     ax.grid()
     ax.plot(
-        x, gs, 'g', alpha=FG_ALPHA,
-        label=r"$\frac{\partial \mathcal{F}}{\partial \theta}$ JAX autodiff")
+        x,
+        gs,
+        "g",
+        alpha=FG_ALPHA,
+        label=r"$\frac{\partial \mathcal{F}}{\partial \theta}$ JAX autodiff",
+    )
     ax.set_ylim(ax.get_ylim())
-    ax.set_xlim((10**domain[0][0], 10**domain[0][1]))
+    ax.set_xlim((10 ** domain[0][0], 10 ** domain[0][1]))
     ax.plot(
-        x, dfsx, 'g--',
-        label=r"$\frac{\partial \mathcal{F}}{\partial \theta}$ numerical")
+        x,
+        dfsx,
+        "g--",
+        label=r"$\frac{\partial \mathcal{F}}{\partial \theta}$ numerical",
+    )
     ylim = ax.get_ylim()
-    ax.vlines(x_hat, ylim[0], ylim[1], 'r',
-        alpha=MG_ALPHA, label=r"$\hat\theta={:.2f}$".format(x_hat))
-    ax.vlines(x_0, ylim[0], ylim[1], 'k',
-        alpha=MG_ALPHA, label=r"$\theta={:.2f}$".format(x_0))
+    ax.vlines(
+        x_hat,
+        ylim[0],
+        ylim[1],
+        "r",
+        alpha=MG_ALPHA,
+        label=r"$\hat\theta={:.2f}$".format(x_hat),
+    )
+    ax.vlines(
+        x_0, ylim[0], ylim[1], "k", alpha=MG_ALPHA, label=r"$\theta={:.2f}$".format(x_0)
+    )
     ax.set_xscale(xscale)
     ax.set_xlabel(xlabel, fontsize=10)
     ax.set_ylabel(r"$\frac{\partial \mathcal{F}}{\partial \theta}$", fontsize=10)
-    ax.set_title('Hyper-parameter optimisation gradient')
+    ax.set_title("Hyper-parameter optimisation gradient")
     ax.legend()
-    fig.savefig("readme_grad.png",
-        facecolor=fig.get_facecolor(), edgecolor='none')
+    fig.savefig("readme_grad.png", facecolor=fig.get_facecolor(), edgecolor="none")
     plt.close()
 
 
 def generate_data(
-        key, N_train_per_class, N_test_per_class,
-        J, kernel, noise_variance,
-        N_show, jitter=1e-6):
+    key,
+    N_train_per_class,
+    N_test_per_class,
+    J,
+    kernel,
+    noise_variance,
+    N_show,
+    jitter=1e-6,
+):
     """
     Generate data from the GP prior, and choose some cutpoints that
     approximately divides data into equal bins.
 
     :arg key: JAX random key, a random seed.
     :arg int N_train_per_class: The number of data points per class.
     :arg int N_test_per_class: The number of data points per class.
@@ -173,16 +224,15 @@
     # Sample from a multivariate normal
     K = B.dense(kernel(X))
     K = K + jitter * jnp.identity(jnp.shape(X)[0])
     L_K = jnp.linalg.cholesky(K)
 
     # Generate normal samples for both sets of input data
     key, step_key = random.split(key, 2)
-    z = random.normal(key,
-        shape=(jnp.shape(X_data)[0] + jnp.shape(X_show)[0],))
+    z = random.normal(key, shape=(jnp.shape(X_data)[0] + jnp.shape(X_show)[0],))
     f = L_K @ z
 
     # Store f_show
     f_data = f[:N_total]
     f_show = f[N_total:]
 
     assert jnp.shape(f_show) == (jnp.shape(X_show)[0],)
@@ -202,24 +252,26 @@
     X = X[idx_sorted]
     X_js = []
     g_js = []
     f_js = []
     y_js = []
     cutpoints = jnp.empty(J + 1)
     for j in range(J):
-        X_js.append(X[N_per_class * j:N_per_class * (j + 1), :1])
-        g_js.append(g[N_per_class * j:N_per_class * (j + 1)])
-        f_js.append(f[N_per_class * j:N_per_class * (j + 1)])
+        X_js.append(X[N_per_class * j : N_per_class * (j + 1), :1])
+        g_js.append(g[N_per_class * j : N_per_class * (j + 1)])
+        f_js.append(f[N_per_class * j : N_per_class * (j + 1)])
         y_js.append(j * jnp.ones(N_per_class, dtype=int))
 
     for j in range(1, J):
         # Find the cutpoints
         cutpoint_j_min = g_js[j - 1][-1]
         cutpoint_j_max = g_js[j][0]
-        cutpoints = cutpoints.at[j].set(jnp.mean(jnp.array([cutpoint_j_max, cutpoint_j_min])))
+        cutpoints = cutpoints.at[j].set(
+            jnp.mean(jnp.array([cutpoint_j_max, cutpoint_j_min]))
+        )
     cutpoints = cutpoints.at[0].set(-jnp.inf)
     cutpoints = cutpoints.at[-1].set(jnp.inf)
     X_js = jnp.array(X_js)
     g_js = jnp.array(g_js)
     f_js = jnp.array(f_js)
     y_js = jnp.array(y_js, dtype=int)
     X = X.reshape(-1, X.shape[-1])
@@ -234,15 +286,15 @@
     X_test_js = []
     y_test_js = []
     for j in range(J):
         data = jnp.c_[g_js[j], X_js[j], y_js[j]]
         key, step_key = random.split(key, 2)
         random.shuffle(key, data)
         g_j = data[:, :1]
-        X_j = data[:, 1:1 + 1]
+        X_j = data[:, 1 : 1 + 1]
         y_j = data[:, -1]
         # split train vs test/validate
         g_train_j = g_j[:N_train_per_class]
         X_train_j = X_j[:N_train_per_class]
         y_train_j = y_j[:N_train_per_class]
         X_j = X_j[N_train_per_class:]
         y_j = y_j[N_train_per_class:]
@@ -263,18 +315,15 @@
     y_train = y_train_js.flatten()
     X_test = X_test_js.reshape(-1, X_test_js.shape[-1])
     y_test = y_test_js.flatten()
 
     y_train = jnp.array(y_train, dtype=int)
     y_test = jnp.array(y_test, dtype=int)
 
-    return (
-        N_show, X, g, y, cutpoints,
-        X_test, y_test,
-        X_show, f_show)
+    return (N_show, X, g, y, cutpoints, X_test, y_test, X_show, f_show)
 
 
 def calculate_metrics(y_test, predictive_distributions):
     y_pred = jnp.argmax(predictive_distributions, axis=1)
     predictive_likelihood = predictive_distributions[:, y_test]
     mean_absolute_error = jnp.sum(jnp.abs(y_pred - y_test)) / len(y_test)
     print(jnp.sum(y_pred != y_test), "sum incorrect")
@@ -284,55 +333,60 @@
     print("log_pred_probability={:.2f}".format(log_predictive_probability))
     mean_zero_one = jnp.sum(y_pred != y_test) / len(y_test)
     print("mean_zero_one_error={:.2f}".format(mean_zero_one))
     return (
         mean_zero_one,
         mean_absolute_error,
         log_predictive_probability,
-        predictive_likelihood)
+        predictive_likelihood,
+    )
 
 
 def main():
     """Make an approximation to the posterior, and optimise hyperparameters."""
     parser = argparse.ArgumentParser()
     # The --profile argument generates profiling information for the example
-    parser.add_argument('--profile', action='store_const', const=True)
+    parser.add_argument("--profile", action="store_const", const=True)
     args = parser.parse_args()
     if args.profile:
         profile = cProfile.Profile()
         profile.enable()
- 
+
     approximate_inference_method = "Laplace"
-    if approximate_inference_method=="Variational Bayes":
+    if approximate_inference_method == "Variational Bayes":
         from probit.approximators import VBGP as Approximator
-    elif approximate_inference_method=="Laplace":
+    elif approximate_inference_method == "Laplace":
         from probit.approximators import LaplaceGP as Approximator
 
     J = 3
-    cmap = plt.cm.get_cmap('PiYG', J)
+    cmap = plt.cm.get_cmap("PiYG", J)
     colors = []
     mapping = []
     for j in range(J):
-        colors.append(cmap((j + 0.5)/J))
-        mapping.append((j + 0.5)/J)
+        colors.append(cmap((j + 0.5) / J))
+        mapping.append((j + 0.5) / J)
     print(colors)
     print(mapping)
 
     # Generate data
     key = random.PRNGKey(1)
     noise_variance = 0.4
     signal_variance = 1.0
     lengthscale = 1.0
     kernel = signal_variance * Matern12().stretch(lengthscale)
-    (N_show, X, g_true, y, cutpoints,
-    X_test, y_test,
-    X_show, f_show) = generate_data(key,
-        N_train_per_class=10, N_test_per_class=100,
-        J=J, kernel=kernel, noise_variance=noise_variance,
-        N_show=1000, jitter=1e-6)
+    (N_show, X, g_true, y, cutpoints, X_test, y_test, X_show, f_show) = generate_data(
+        key,
+        N_train_per_class=10,
+        N_test_per_class=100,
+        J=J,
+        kernel=kernel,
+        noise_variance=noise_variance,
+        N_show=1000,
+        jitter=1e-6,
+    )
 
     # Initiate a misspecified model, using a kernel
     # other than the one used to generate data
     def prior(prior_parameters):
         # Here you can define the kernel that defines the Gaussian process
         return signal_variance * EQ().stretch(prior_parameters)
 
@@ -341,20 +395,22 @@
         raise InvalidKernel(prior(1.0))
 
     # check that the cutpoints are in the correct format
     # for the number of classes, J
     cutpoints = check_cutpoints(cutpoints, J)
     print("cutpoints={}".format(cutpoints))
 
-    classifier = Approximator(data=(X, y), prior=prior,
+    classifier = Approximator(
+        data=(X, y),
+        prior=prior,
         log_likelihood=log_probit_likelihood,
         # grad_log_likelihood=grad_log_probit_likelihood,
         # hessian_log_likelihood=hessian_log_probit_likelihood,
-        tolerance=1e-5  # tolerance for the jaxopt fixed-point resolution
-        )
+        tolerance=1e-5,  # tolerance for the jaxopt fixed-point resolution
+    )
     negative_evidence_lower_bound = classifier.objective()
 
     vs = Vars(jnp.float32)
 
     def model(vs):
         p = vs.struct
         noise_std = jnp.sqrt(noise_variance)
@@ -362,88 +418,98 @@
 
     def objective(vs):
         return negative_evidence_lower_bound(model(vs))
 
     # Approximate posterior
     parameters = model(vs)
     weight, precision = classifier.approximate_posterior(parameters)
-    mean, variance = classifier.predict(
-        X_show,
-        parameters,
-        weight, precision)
+    mean, variance = classifier.predict(X_show, parameters, weight, precision)
     obs_variance = variance + noise_variance
     predictive_distributions = probit_predictive_distributions(
-        parameters[1],
-        mean, variance)
-    plot(X_show, predictive_distributions, mean,
-        obs_variance, X_show, f_show, X, y, g_true,
-        J, colors, fname="readme_classification_before")
+        parameters[1], mean, variance
+    )
+    plot(
+        X_show,
+        predictive_distributions,
+        mean,
+        obs_variance,
+        X_show,
+        f_show,
+        X,
+        y,
+        g_true,
+        J,
+        colors,
+        fname="readme_classification_before",
+    )
 
     # Evaluate model
-    mean, variance = classifier.predict(
-        X_test,
-        parameters,
-        weight, precision)
+    mean, variance = classifier.predict(X_test, parameters, weight, precision)
     predictive_distributions = probit_predictive_distributions(
-        parameters[1],
-        mean, variance)
+        parameters[1], mean, variance
+    )
     print("\nEvaluation of model:")
     calculate_metrics(y_test, predictive_distributions)
 
     print("Before optimization, \nparameters={}".format(parameters))
     minimise_l_bfgs_b(objective, vs)
     parameters = model(vs)
     print("After optimization, \nparameters={}".format(model(vs)))
 
     # Approximate posterior
     parameters = model(vs)
     weight, precision = classifier.approximate_posterior(parameters)
-    mean, variance = classifier.predict(
-        X_show,
-        parameters,
-        weight, precision)
+    mean, variance = classifier.predict(X_show, parameters, weight, precision)
     predictive_distributions = probit_predictive_distributions(
-        parameters[1],
-        mean, variance)
-    plot(X_show, predictive_distributions, mean,
-        obs_variance, X_show, f_show, X, y, g_true,
-        J, colors, fname="readme_classification_after")
+        parameters[1], mean, variance
+    )
+    plot(
+        X_show,
+        predictive_distributions,
+        mean,
+        obs_variance,
+        X_show,
+        f_show,
+        X,
+        y,
+        g_true,
+        J,
+        colors,
+        fname="readme_classification_after",
+    )
 
     # Evaluate model
-    mean, variance = classifier.predict(
-        X_test,
-        parameters,
-        weight, precision)
+    mean, variance = classifier.predict(X_test, parameters, weight, precision)
     obs_variance = variance + noise_variance
     predictive_distributions = probit_predictive_distributions(
-        parameters[1],
-        mean, variance)
+        parameters[1], mean, variance
+    )
     print("\nEvaluation of model:")
     calculate_metrics(y_test, predictive_distributions)
 
-    nelbo = lambda x : negative_evidence_lower_bound(((x), (jnp.sqrt(noise_variance), cutpoints)))
+    nelbo = lambda x: negative_evidence_lower_bound(
+        ((x), (jnp.sqrt(noise_variance), cutpoints))
+    )
     fg = vmap(value_and_grad(nelbo))
 
     domain = ((-2, 2), None)
     resolution = (50, None)
-    x = jnp.logspace(
-        domain[0][0], domain[0][1], resolution[0])
+    x = jnp.logspace(domain[0][0], domain[0][1], resolution[0])
     xlabel = r"lengthscale, $\ell$"
     xscale = "log"
     phis = jnp.log(x)
 
     fgs = fg(x)
     fs = fgs[0]
     gs = fgs[1]
     plot_obj(vs.struct.lengthscale(), lengthscale, x, fs, gs, domain, xlabel, xscale)
 
     if args.profile:
         profile.disable()
         s = StringIO()
         stats = Stats(profile, stream=s).sort_stats(SortKey.CUMULATIVE)
-        stats.print_stats(.05)
+        stats.print_stats(0.05)
         print(s.getvalue())
 
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `probit-0.0.0/examples/regression.py` & `probit-0.0.2/examples/regression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """GP regression."""
+
 # Uncomment to enable double precision
 from jax.config import config
+
 config.update("jax_enable_x64", True)
 
 from probit.utilities import log_gaussian_likelihood
 from probit.approximators import LaplaceGP as GP
 import lab as B
 import jax.numpy as jnp
 import jax.random as random
 from mlkernels import EQ
-from varz import Vars, minimise_l_bfgs_b, parametrised, Positive
+from varz import Vars, minimise_l_bfgs_b
 import matplotlib.pyplot as plt
 import argparse
 import cProfile
 from io import StringIO
 from pstats import Stats, SortKey
 
 
 # For plotting
 BG_ALPHA = 1.0
 MG_ALPHA = 1.0
 FG_ALPHA = 0.3
 
 
-def generate_data(
-        key,
-        N_train,
-        kernel, noise_std,
-        N_show, jitter=1e-10):
+def generate_data(key, N_train, kernel, noise_std, N_show, jitter=1e-10):
     """
     Generate data from the GP prior.
 
     :arg key: JAX random key, a random seed.
     :arg int N_train: The number of data points.
     :arg kernel: The GP prior.
     :arg noise_std: The noise standard deviation.
@@ -55,16 +53,15 @@
     # Sample from a multivariate normal
     K = B.dense(kernel(X))
     K = K + jitter * jnp.identity(jnp.shape(X)[0])
     L_K = jnp.linalg.cholesky(K)
 
     # Generate normal samples for both sets of input data
     key, step_key = random.split(key, 2)
-    z = random.normal(key,
-        shape=(X_train.shape[0] + X_show.shape[0],))
+    z = random.normal(key, shape=(X_train.shape[0] + X_show.shape[0],))
     f = L_K @ z
 
     # Store f_show
     f_train = f[:N_train]
     f_show = f[N_train:]
 
     # Generate the latent variables
@@ -76,110 +73,111 @@
     # Reshuffle
     key, step_key = random.split(key, 2)
     data = jnp.c_[y_train, X_train]
     random.shuffle(key, data)
     y_train = data[:, :1].flatten()
     X_train = data[:, 1:]
 
-    return (
-        X_train, y_train,
-        X_show, f_show, N_show)
+    return (X_train, y_train, X_show, f_show, N_show)
 
 
-def plot(train_data, test_data, mean, variance,
-         fname="plot.png"):
+def plot(train_data, test_data, mean, variance, fname="plot.png"):
     X, y = train_data
     X_show, f_show = test_data
     # Plot result
     fig, ax = plt.subplots(1, 1)
     ax.plot(X_show, f_show, label="True", color="orange")
     ax.plot(X_show, mean, label="Prediction", linestyle="--", color="blue")
     ax.scatter(X, y, label="Observations", color="black", s=20)
     ax.fill_between(
-        X_show.flatten(), mean - 2. * jnp.sqrt(variance),
-        mean + 2. * jnp.sqrt(variance), alpha=FG_ALPHA, color="blue")
+        X_show.flatten(),
+        mean - 2.0 * jnp.sqrt(variance),
+        mean + 2.0 * jnp.sqrt(variance),
+        alpha=FG_ALPHA,
+        color="blue",
+    )
     ax.set_xlim((0.0, 1.0))
-    ax.grid(visible=True, which='major', linestyle='-')
-    ax.set_xlabel('x', fontsize=10)
-    ax.set_ylabel('y', fontsize=10)
-    fig.patch.set_facecolor('white')
+    ax.grid(visible=True, which="major", linestyle="-")
+    ax.set_xlabel("x", fontsize=10)
+    ax.set_ylabel("y", fontsize=10)
+    fig.patch.set_facecolor("white")
     fig.patch.set_alpha(BG_ALPHA)
     ax.patch.set_alpha(MG_ALPHA)
     ax.legend()
     fig.savefig(fname)
     plt.close()
 
 
 def main():
     """Make an approximation to the posterior, and optimise hyperparameters."""
     parser = argparse.ArgumentParser()
     # The --profile argument generates profiling information for the example
-    parser.add_argument('--profile', action='store_const', const=True)
+    parser.add_argument("--profile", action="store_const", const=True)
     args = parser.parse_args()
     if args.profile:
         profile = cProfile.Profile()
         profile.enable()
- 
+
     def prior(prior_parameters):
         lengthscale, signal_variance = prior_parameters
         # Here you can define the kernel that defines the Gaussian process
         return signal_variance * EQ().stretch(lengthscale).periodic(0.5)
 
     # Generate data
     key = random.PRNGKey(0)
     noise_std = 0.2
-    (X, y,
-     X_show, f_show, N_show) = generate_data(
-         key,
-         N_train=20,
-         kernel=prior((1.0, 1.0)), noise_std=noise_std,
-         N_show=1000)
-
-    gaussian_process = GP(data=(X, y), prior=prior,
-        log_likelihood=log_gaussian_likelihood)
+    (X, y, X_show, f_show, N_show) = generate_data(
+        key, N_train=20, kernel=prior((1.0, 1.0)), noise_std=noise_std, N_show=1000
+    )
+
+    gaussian_process = GP(
+        data=(X, y), prior=prior, log_likelihood=log_gaussian_likelihood
+    )
     negative_evidence = gaussian_process.objective()
 
     vs = Vars(jnp.float32)
 
     def model(vs):
         p = vs.struct
-        return (p.lengthscale.positive(), p.signal_variance.positive()), (p.noise_std.positive(),)
+        return (p.lengthscale.positive(), p.signal_variance.positive()), (
+            p.noise_std.positive(),
+        )
 
     def objective(vs):
         return negative_evidence(model(vs))
 
     # Approximate posterior
     parameters = model(vs)
     weight, precision = gaussian_process.approximate_posterior(parameters)
-    mean, variance = gaussian_process.predict(
-        X_show,
-        parameters,
-        weight, precision)
-    noise_variance = vs.struct.noise_std()**2
+    mean, variance = gaussian_process.predict(X_show, parameters, weight, precision)
+    noise_variance = vs.struct.noise_std() ** 2
     obs_variance = variance + noise_variance
     plot((X, y), (X_show, f_show), mean, variance, fname="readme_regression_before.png")
 
     print("Before optimization, \nparams={}".format(parameters))
     minimise_l_bfgs_b(objective, vs)
     parameters = model(vs)
     print("After optimization, \nparams={}".format(model(vs)))
 
     # Approximate posterior
     weight, precision = gaussian_process.approximate_posterior(parameters)
-    mean, variance = gaussian_process.predict(
-        X_show,
-        parameters,
-        weight, precision)
-    noise_variance = vs.struct.noise_std()**2
+    mean, variance = gaussian_process.predict(X_show, parameters, weight, precision)
+    noise_variance = vs.struct.noise_std() ** 2
     obs_variance = variance + noise_variance
-    plot((X, y), (X_show, f_show), mean, obs_variance, fname="readme_regression_after.png")
+    plot(
+        (X, y),
+        (X_show, f_show),
+        mean,
+        obs_variance,
+        fname="readme_regression_after.png",
+    )
 
     if args.profile:
         profile.disable()
         s = StringIO()
         stats = Stats(profile, stream=s).sort_stats(SortKey.CUMULATIVE)
-        stats.print_stats(.05)
+        stats.print_stats(0.05)
         print(s.getvalue())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `probit-0.0.0/probit/approximators.py` & `probit-0.0.2/probit/approximators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from abc import ABC, abstractmethod
-import pathlib
-import jax
 import lab.jax as B
 import jax.numpy as jnp
 from jax import value_and_grad, grad, jit, vmap
 from probit.implicit.solvers import (
-    fwd_solver, newton_solver,
-    fixed_point_layer, fixed_point_layer_fwd, fixed_point_layer_bwd)
+    fwd_solver,
+    newton_solver,
+    fixed_point_layer,
+    fixed_point_layer_fwd,
+    fixed_point_layer_bwd,
+)
 from probit.implicit.Laplace import f_LA, objective_LA
 from probit.implicit.VB import f_VB, objective_VB
 
 
 class Approximator(ABC):
     """
     Base class for GP regression/classification approximators.
@@ -39,73 +41,79 @@
         `weights` and `parameters` and can be used to define the
         second moment of an approximate posterior.
     """
 
     @abstractmethod
     def __repr__(self):
         """
-        Return a string representation of this class, used to import the class
+        Returns a string representation of this class, used to import the class
         from the string.
 
         This method should be implemented in every concrete Approximator.
         """
 
     @abstractmethod
     def __init__(
-            self, data, prior, log_likelihood,
-            grad_log_likelihood=None, hessian_log_likelihood=None,
-            tolerance=1e-5):
+        self,
+        data,
+        prior,
+        log_likelihood,
+        grad_log_likelihood=None,
+        hessian_log_likelihood=None,
+        tolerance=1e-5,
+    ):
         """
         Create an :class:`Approximator` object.
 
         This method should be implemented in every concrete Approximator.
 
         :arg prior: method, when evaluated prior(*args, **kwargs) returns
             a valid `:class:MLKernels.Kernel` object
             that is the kernel of the Gaussian Process.
-        :arg data: The data tuple. (X_train, y_train), where  
+        :arg data: The data tuple. (X_train, y_train), where
             X_train is the (N, D) The data vector and y_train (N, ) is the
-            target vector. 
+            target vector.
         :type data: (:class:`numpy.ndarray`, :class:`numpy.ndarray`)
         :arg log_likelihood: method, when evaluated
-            log_likelihood(*args, **kwargs) returns the log likelihood. Takes
+            log_likelihood(*args, **kwargs) return the log likelihood. Takes
             in arguments as log_likelihood(f, y, likelihood_parameters)
             where likelihood_parameters are the (trainable) parameters
             of the likelihood, f is a latent variable and y is a datum.
         :arg grad_log_likelihood: Optional argument supplying the
             (scalar) gradient of the log_likelihood wrt to its first argument,
             the latent variables, f.
         :arg hessian_log_likelihood: Optional argument supplying the
             (scalar) second derivative of the log_likelihood wrt to its first
             argument, the latent variables, f.
 
-        :returns: A :class:`Approximator` object
+        :return: A :class:`Approximator` object
         """
         self.tolerance = tolerance  # tolerance for the solvers
         self.prior = prior
         if grad_log_likelihood is None:  # Try JAX grad
             grad_log_likelihood = grad(log_likelihood)
         if hessian_log_likelihood is None:  # Try JAX grad
-            hessian_log_likelihood = grad(
-                lambda f, y, x: grad(log_likelihood)(f, y, x))
-        self.log_likelihood = jit(vmap(
-            log_likelihood, in_axes=(0, 0, None), out_axes=(0)))
-        self.grad_log_likelihood = jit(vmap(
-            grad_log_likelihood, in_axes=(0, 0, None), out_axes=(0)))
-        self.hessian_log_likelihood = jit(vmap(
-            hessian_log_likelihood, in_axes=(0, 0, None), out_axes=(0)))
+            hessian_log_likelihood = grad(lambda f, y, x: grad(log_likelihood)(f, y, x))
+        self.log_likelihood = jit(
+            vmap(log_likelihood, in_axes=(0, 0, None), out_axes=(0))
+        )
+        self.grad_log_likelihood = jit(
+            vmap(grad_log_likelihood, in_axes=(0, 0, None), out_axes=(0))
+        )
+        self.hessian_log_likelihood = jit(
+            vmap(hessian_log_likelihood, in_axes=(0, 0, None), out_axes=(0))
+        )
 
         # Get data and calculate the prior
         X_train, _ = data
         (self.N, self.D) = jnp.shape(X_train)
         self.data = data
 
         # Set up a JAX-transformable function for a custom VJP rule definition
-        fixed_point_layer.defvjp(
-            fixed_point_layer_fwd, fixed_point_layer_bwd)
+        fixed_point_layer.defvjp(fixed_point_layer_fwd, fixed_point_layer_bwd)
 
     @abstractmethod
     def construct(self):
         """
         The parameterized function, which takes in parameters, that is the
         implicit function to be satisfied by fixed point iteration.
 
@@ -127,57 +135,71 @@
 
     @abstractmethod
     def weight(self):
         """
         The weight, that is part of the solution of GP regression.
 
         This method should be implemented in every concrete Approximator.
-        Returns: A (N,) JAX array.
+        :return: A (N,) JAX array.
         """
 
     @abstractmethod
     def precision(self):
         """
         The precision, that is part of the solution of GP regression.
 
         This method should be implemented in every concrete Approximator.
-        Returns: A (N,) JAX array.
+        :return: A (N,) JAX array.
         """
 
-    def predict(
-        self,
-        X_test,
-        parameters,
-        weight, precision):
+    def predict(self, X_test, parameters, weight, precision):
         """
         Make posterior predictions given test data, X_test.
 
         :arg X_test: The new data points, array like (N_test, D).
         :arg parameters: The GP hyper-parameters like
             ((tuple), (tuple)).
         :arg weight: The solution of GP regression. Used to calculate
             the first moment of the posterior predictions.
         :type weight: Array like (N,)`
         :arg precision: Solution of GP regression. Used to calculate
             the second moment of the posterior predictions. Array
             like (N,).
         :type precision: Array like (N,)`
-        :return: Gaussian process predictive mean and variance array.
-        :rtype tuple: ((N_test,), (N_test,))
+        :return: Gaussian process predictive mean and variance JAX
+            array ((N_test,), (N_test,)).
         """
         kernel = self.prior(parameters[0])
         Kss = B.flatten(kernel.elwise(X_test, X_test))
         Kfs = kernel(self.data[0], X_test)
         Kff = kernel(self.data[0])
-        K = Kff + B.diag(1. / precision)
+        K = Kff + B.diag(1.0 / precision)
         predictive_posterior_variance = Kss - B.einsum(
-            'ij, ij -> j', B.dense(Kfs), B.solve(K, Kfs))
+            "ij, ij -> j", B.dense(Kfs), B.solve(K, Kfs)
+        )
         predictive_posterior_mean = B.flatten(Kfs.T @ weight)
         return predictive_posterior_mean, predictive_posterior_variance
 
+    def predict_covariance(self, X_test, parameters, weight, precision):
+        """
+        Make posterior predictive covariance given test data, X_test.
+
+        Args are the same as for `:meth:predict`.
+
+        :return: Gaussian process predictive covariance array.
+        :rtype array: (N_test, N_test)
+        """
+        kernel = self.prior(parameters[0])
+        Kss = B.dense(kernel(X_test, X_test))
+        Kfs = B.dense(kernel(self.data[0], X_test))
+        Kff = kernel(self.data[0])
+        K = Kff + B.diag(1.0 / precision)
+        predictive_posterior_covariance = Kss - Kfs.T @ B.solve(K, Kfs)
+        return predictive_posterior_covariance
+
     def posterior_mean(self, weight):
         """Returns a Gaussian Process mean."""
         K = B.dense(self.prior(parameters[0])(self.data[0]))
         return K @ weight
 
     def approximate_posterior(self, parameters):
         """Returns weights and precisions that can be used to
@@ -186,116 +208,132 @@
         w = self.weight(parameters)
         p, _ = self.precision(w, parameters)
         return w, p
 
 
 class LaplaceGP(Approximator):
     """
-    A GP classifier for ordinal likelihood using the Laplace
-    approximation.
+    A GP posterior approximation using the Laplace approximation.
 
     Inherits the Approximator ABC.
 
-    This class allows users to define a classification problem and get
-    predictions using approximate Bayesian inference. It is for ordinal
-    likelihood.
-
-    For this a :class:`probit.kernels.Kernel` is required for the Gaussian
-    Process.
+    This class allows users to define a regression/classification problem
+    and get predictions using approximate Bayesian inference.
     """
+
     def __repr__(self):
         """
-        Return a string representation of this class, used to import the class
+        Returns a string representation of this class, used to import the class
         from the string.
         """
         return "LaplaceGP"
 
-    def __init__(
-            self, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         """
         Create an :class:`LaplaceGP` Approximator object.
 
-        :returns: An :class:`LaplaceGP` object.
+        :return: An :class:`LaplaceGP` object.
         """
         super().__init__(*args, **kwargs)
 
     def construct(self):
         return lambda parameters, weight: f_LA(
             prior_parameters=parameters[0],
             likelihood_parameters=parameters[1],
-            prior=self.prior, grad_log_likelihood=self.grad_log_likelihood,
-            weight=weight, data=self.data)
+            prior=self.prior,
+            grad_log_likelihood=self.grad_log_likelihood,
+            weight=weight,
+            data=self.data,
+        )
 
     def objective(self):
         return lambda parameters: objective_LA(
-                parameters[0], parameters[1],
-                self.prior,
-                self.log_likelihood,
-                self.hessian_log_likelihood,
-                fixed_point_layer(jnp.zeros(self.N), self.tolerance,
-                    newton_solver, self.construct(), parameters),
-                self.data)
+            parameters[0],
+            parameters[1],
+            self.prior,
+            self.log_likelihood,
+            self.hessian_log_likelihood,
+            fixed_point_layer(
+                jnp.zeros(self.N),
+                self.tolerance,
+                newton_solver,
+                self.construct(),
+                parameters,
+            ),
+            self.data,
+        )
 
     def weight(self, parameters):
         f = self.construct()
-        return newton_solver(lambda z: f(parameters, z),
-            jnp.zeros(self.N), self.tolerance)
+        return newton_solver(
+            lambda z: f(parameters, z), jnp.zeros(self.N), self.tolerance
+        )
 
     def precision(self, weight, parameters):
         K = B.dense(self.prior(parameters[0])(self.data[0]))
         posterior_mean = K @ weight
         precision = -self.hessian_log_likelihood(
-            posterior_mean, self.data[1], parameters[1])
+            posterior_mean, self.data[1], parameters[1]
+        )
         return precision, posterior_mean
 
 
 class VBGP(Approximator):
     """
-    A GP classifier for ordinal likelihood using the Variational Bayes (VB)
+    A GP posterior approximation using the Variational Bayes (VB)
     approximation.
- 
-    Inherits the Approximator ABC. This class allows users to define a
-    classification problem, get predictions using approximate Bayesian
-    inference. It is for the ordinal likelihood. For this a
-    :class:`probit.kernels.Kernel` is required for the Gaussian Process.
+
+    Inherits the Approximator ABC.
+
+    This class allows users to define a regression/classification problem
+    and get predictions using approximate Bayesian inference.
     """
+
     def __repr__(self):
         """
-        Return a string representation of this class, used to import the class
+        Returns a string representation of this class, used to import the class
         from the string.
         """
         return "VBGP"
 
-    def __init__(
-            self, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         """
         Create an :class:`VBGP` Approximator object.
 
-        :returns: A :class:`VBGP` object.
+        :return: A :class:`VBGP` object.
         """
         super().__init__(*args, **kwargs)
 
     def construct(self):
         return lambda parameters, weight: f_VB(
             prior_parameters=parameters[0],
             likelihood_parameters=parameters[1],
-            prior=self.prior, grad_log_likelihood=self.grad_log_likelihood,
-            weight=weight, data=self.data)
+            prior=self.prior,
+            grad_log_likelihood=self.grad_log_likelihood,
+            weight=weight,
+            data=self.data,
+        )
 
     def objective(self):
         return lambda parameters: objective_VB(
-            parameters[0], parameters[1],
+            parameters[0],
+            parameters[1],
             self.prior,
             self.log_likelihood,
-            fixed_point_layer(jnp.zeros(self.N), self.tolerance,
-                fwd_solver, self.construct(), parameters),
-            self.data)
+            fixed_point_layer(
+                jnp.zeros(self.N),
+                self.tolerance,
+                fwd_solver,
+                self.construct(),
+                parameters,
+            ),
+            self.data,
+        )
 
     def weight(self, parameters):
         f = self.construct()
-        return fwd_solver(lambda z: f(parameters, z),
-            jnp.zeros(self.N), self.tolerance)
+        return fwd_solver(lambda z: f(parameters, z), jnp.zeros(self.N), self.tolerance)
 
     def precision(self, weight, parameters):
         K = B.dense(self.prior(parameters[0])(self.data[0]))
         posterior_mean = K @ weight
-        return 1./ parameters[1][0]**2 * jnp.ones(weight.shape[0]), posterior_mean
+        return 1.0 / parameters[1][0] ** 2 * jnp.ones(weight.shape[0]), posterior_mean
```

### Comparing `probit-0.0.0/probit/implicit/Laplace.py` & `probit-0.0.2/probit/implicit/Laplace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import lab.jax as B
 
 
-def f_LA(prior_parameters, likelihood_parameters, prior, grad_log_likelihood,
-        weight, data):
+def f_LA(
+    prior_parameters, likelihood_parameters, prior, grad_log_likelihood, weight, data
+):
     K = B.dense(prior(prior_parameters)(data[0]))
     posterior_mean = K @ weight
     return grad_log_likelihood(posterior_mean, data[1], likelihood_parameters)
 
 
-def objective_LA(prior_parameters, likelihood_parameters, prior,
-        log_likelihood, hessian_log_likelihood,
-        weight, data):
+def objective_LA(
+    prior_parameters,
+    likelihood_parameters,
+    prior,
+    log_likelihood,
+    hessian_log_likelihood,
+    weight,
+    data,
+):
     K = B.dense(prior(prior_parameters)(data[0]))
     posterior_mean = K @ weight
     precision = -hessian_log_likelihood(posterior_mean, data[1], likelihood_parameters)
-    L_cov = B.cholesky(prior(prior_parameters)(data[0]) + B.diag(1./ precision))
+    L_cov = B.cholesky(prior(prior_parameters)(data[0]) + B.diag(1.0 / precision))
     return (
-        - B.sum(log_likelihood(posterior_mean, data[1], likelihood_parameters))
+        -B.sum(log_likelihood(posterior_mean, data[1], likelihood_parameters))
         + 0.5 * posterior_mean.T @ weight
         + B.sum(B.log(B.diag(L_cov)))
         + 0.5 * B.sum(B.log(precision))
     )
```

### Comparing `probit-0.0.0/probit/implicit/VB.py` & `probit-0.0.2/probit/implicit/VB.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import lab.jax as B
 
 
 def f_VB(
-        prior_parameters, likelihood_parameters, prior, grad_log_likelihood,
-        weight, data):
+    prior_parameters, likelihood_parameters, prior, grad_log_likelihood, weight, data
+):
     K = B.dense(prior(prior_parameters)(data[0]))
     N = B.shape(data[0])[0]
-    posterior_mean = K @ weight 
-    L_cov = B.cholesky(likelihood_parameters[0]**2 * B.eye(N) + K)
+    posterior_mean = K @ weight
+    L_cov = B.cholesky(likelihood_parameters[0] ** 2 * B.eye(N) + K)
     return B.cholesky_solve(
         L_cov,
-        posterior_mean + likelihood_parameters[0] * grad_log_likelihood(
-            posterior_mean, data[1], likelihood_parameters))
+        posterior_mean
+        + likelihood_parameters[0]
+        * grad_log_likelihood(posterior_mean, data[1], likelihood_parameters),
+    )
 
 
-def objective_VB(prior_parameters, likelihood_parameters, prior,
-        log_likelihood, weight, data):
+def objective_VB(
+    prior_parameters, likelihood_parameters, prior, log_likelihood, weight, data
+):
     K = B.dense(prior(prior_parameters)(data[0]))
     posterior_mean = K @ weight
     N = B.shape(data[0])[0]
-    L_cov = B.cholesky(likelihood_parameters[0]**2 * B.eye(N) + K)
+    L_cov = B.cholesky(likelihood_parameters[0] ** 2 * B.eye(N) + K)
     L_covT_inv = B.triangular_solve(L_cov, B.eye(N), lower_a=True)
     cov = B.triangular_solve(L_cov.T, L_covT_inv, lower_a=False)
     log_det_cov = -2 * B.sum(B.log(B.diag(L_cov)))
     trace_cov = B.sum(B.diag(cov))
-    trace_posterior_cov_div_var = B.einsum(
-        'ij, ij -> ', K, cov)
-    trace_K_inv_posterior_cov = likelihood_parameters[0]**2 * trace_cov
-    return (0.5 * trace_posterior_cov_div_var
+    trace_posterior_cov_div_var = B.einsum("ij, ij -> ", K, cov)
+    trace_K_inv_posterior_cov = likelihood_parameters[0] ** 2 * trace_cov
+    return (
+        0.5 * trace_posterior_cov_div_var
         + 0.5 * trace_K_inv_posterior_cov
         + 0.5 * posterior_mean.T @ weight
         - N * B.log(likelihood_parameters[0])
         - 0.5 * log_det_cov
         - 0.5 * N
-        - B.sum(log_likelihood(posterior_mean, data[1], likelihood_parameters)))
+        - B.sum(log_likelihood(posterior_mean, data[1], likelihood_parameters))
+    )
```

### Comparing `probit-0.0.0/probit/implicit/solvers.py` & `probit-0.0.2/probit/implicit/solvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,34 +27,38 @@
 
 @partial(custom_vjp, nondiff_argnums=(2, 3))
 def fixed_point_layer(z_init, tolerance, solver, f, params):
     """
     Following the tutorial, Chapter 2 of
     http://implicit-layers-tutorial.org/implicit_functions/
 
-    A wrapper function for the parameterized fixed point sovler.
+    A wrapper function for the parameterized fixed point solver.
 
     :arg solver: Root finding numerical solver
     :arg params: Parameters for the non-linear set of equations that must
         be satisfied
         .. math::
             z = f(a, z)
         where :math:`a` are parameters and :math:`z` are the latent
         variables, and :math:`f` is a non-linear function.
-    """ 
-    return solver(
-        lambda z: f(params, z), z_init=z_init, tolerance=tolerance)
+    """
+    return solver(lambda z: f(params, z), z_init=z_init, tolerance=tolerance)
 
 
 def fixed_point_layer_fwd(z_init, tolerance, solver, f, params):
     z_star = fixed_point_layer(z_init, tolerance, solver, f, params)
     return z_star, (z_init, tolerance, params, z_star)
 
 
 def fixed_point_layer_bwd(solver, f, res, z_star_bar):
     z_init, tolerance, params, z_star = res
     _, vjp_a = vjp(lambda params: f(params, z_star), params)
     _, vjp_z = vjp(lambda z: f(params, z), z_star)
-    return (None, None, 
-        *vjp_a(solver(
-            lambda u: vjp_z(u)[0] + z_star_bar,
-            z_init=z_init, tolerance=tolerance)))
+    return (
+        None,
+        None,
+        *vjp_a(
+            solver(
+                lambda u: vjp_z(u)[0] + z_star_bar, z_init=z_init, tolerance=tolerance
+            )
+        ),
+    )
```

### Comparing `probit-0.0.0/probit/utilities.py` & `probit-0.0.2/probit/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 """Utility functions for probit."""
+
 import lab as B
 import jax
 import jax.numpy as jnp
 from math import inf
 import warnings
 
 
-over_sqrt_2_pi = 1. / B.sqrt(2 * B.pi)
+over_sqrt_2_pi = 1.0 / B.sqrt(2 * B.pi)
 log_over_sqrt_2_pi = jnp.log(over_sqrt_2_pi)
 sqrt_2 = B.sqrt(2)
 
 
-BOUNDS = {
-    "single": [1.3, 1.8, 2.3],
-    "double": [2.3, 3.6, 4.8]
-}
+BOUNDS = {"single": [1.3, 1.8, 2.3], "double": [2.3, 3.6, 4.8]}
 
 
 def ndtr(z):
-    return 0.5 * (1 + jax.lax.erf(z/sqrt_2))
+    return 0.5 * (1 + jax.lax.erf(z / sqrt_2))
 
 
 def norm_z_pdf(z):
-    return over_sqrt_2_pi * jnp.exp(- 0.5 * z**2)
+    return over_sqrt_2_pi * jnp.exp(-0.5 * z**2)
 
 
 def norm_pdf(x, loc=0.0, scale=1.0):
     z = (x - loc) / scale
     return norm_z_pdf(z) / scale
 
 
 def norm_cdf(x):
-    _x = jnp.where(jnp.isinf(x), 1., x)
-    extrema = jnp.where(x == jnp.inf, 1., 0.)
+    _x = jnp.where(jnp.isinf(x), 1.0, x)
+    extrema = jnp.where(x == jnp.inf, 1.0, 0.0)
     return jnp.where(jnp.isinf(x), extrema, ndtr(_x))
 
 
 def h(x):
     """
     Polynomial part of a series expansion for log survival function for a
     normal random variable. With the third term, for x>4, this is accurate
     to three decimal places. The third term becomes significant when sigma
-    is large. 
+    is large.
     """
     return -1 * x**-2 + 5 / 2 * x**-4 - 37 / 3 * x**-6
 
 
-def probit_likelihood(
-        f, y, likelihood_parameters):
+def probit_likelihood(f, y, likelihood_parameters):
     return probit(
         likelihood_parameters[0],
-        likelihood_parameters[1][y], likelihood_parameters[1][y + 1],
-        f)
+        likelihood_parameters[1][y],
+        likelihood_parameters[1][y + 1],
+        f,
+    )
 
 
-def log_probit_likelihood(
-        f, y, likelihood_parameters):
+def log_probit_likelihood(f, y, likelihood_parameters):
     return jnp.log(probit_likelihood(f, y, likelihood_parameters) + 1e-10)
 
 
-def log_gaussian_likelihood(
-    f, y, likelihood_parameters):
+def log_gaussian_likelihood(f, y, likelihood_parameters):
     return norm_logpdf(f, loc=y, scale=likelihood_parameters[0])
 
 
 def norm_z_logpdf(x):
     return log_over_sqrt_2_pi - x**2 / 2.0
 
 
@@ -84,115 +81,122 @@
 
 
 def _Z_far_tails(z):
     """Prevents overflow at large z."""
     return over_sqrt_2_pi / z * jnp.exp(-0.5 * z**2 + h(z))
 
 
-def _safe_Z(f, y, likelihood_parameters,
-    upper_bound=jnp.inf, upper_bound2=jnp.inf, upper_bound3=jnp.inf):
+def _safe_Z(
+    f,
+    y,
+    likelihood_parameters,
+    upper_bound=jnp.inf,
+    upper_bound2=jnp.inf,
+    upper_bound3=jnp.inf,
+):
     """Calculate the difference in CDFs between two z-scores, where z2 >= z1.
     Use approximations to avoid catastrophic cancellation at extreme values.
-    
+
     Nans are tracked through gradients. This function ensures that the functions
     are not evaluated at possible nan values."""
-    cutpoints_tplus1 = jnp.asarray(likelihood_parameters[1])[y+1]
+    cutpoints_tplus1 = jnp.asarray(likelihood_parameters[1])[y + 1]
     cutpoints_t = jnp.asarray(likelihood_parameters[1])[y]
 
     noise_std = likelihood_parameters[0]
 
-    _b = jnp.where(cutpoints_tplus1 == jnp.inf, 0., cutpoints_tplus1)
-    _a = jnp.where(cutpoints_t == -jnp.inf, 0., cutpoints_t)
+    _b = jnp.where(cutpoints_tplus1 == jnp.inf, 0.0, cutpoints_tplus1)
+    _a = jnp.where(cutpoints_t == -jnp.inf, 0.0, cutpoints_t)
 
     z2s = jnp.where(cutpoints_tplus1 == jnp.inf, jnp.inf, (_b - f) / noise_std)
     z1s = jnp.where(cutpoints_t == -jnp.inf, -jnp.inf, (_a - f) / noise_std)
 
     # Placeholder value used to signify that the function is *not* evalutated
     # at this point
-    SAFE = 1.
+    SAFE = 1.0
 
     # TODO: tidy up the below commented lines
     # _z1s = jnp.where(jnp.abs(z1s) < upper_bound, z1s, SAFE)
     # _z2s = jnp.where(jnp.abs(z2s) < upper_bound, z2s, SAFE+1)
-    Z  = norm_cdf(z2s) - norm_cdf(z1s)
+    Z = norm_cdf(z2s) - norm_cdf(z1s)
 
     # Remove any zero-values of z1s and z2s to avoid divide-by-zero
     # these values aren't used - only to avoid nans (https://github.com/google/jax/issues/1052 and 8247)
     _z1s = jnp.where((upper_bound < z1s) & (z1s <= upper_bound2), z1s, SAFE)
     __z2s = jnp.where(upper_bound < z1s, z2s, SAFE)
 
     _z2s = jnp.where((-upper_bound2 <= z2s) & (z2s < -upper_bound), z2s, SAFE)
     __z1s = jnp.where(-upper_bound > z2s, z1s, SAFE)
 
     # Using series expansion approximations
     Z = jnp.where(z1s > upper_bound, _Z_tails(_z1s, __z2s), Z)
     Z = jnp.where(z2s < -upper_bound, _Z_tails(__z1s, _z2s), Z)
 
-    _z1s = jnp.where((upper_bound2 < jnp.abs(z1s)) & (jnp.abs(z1s) < upper_bound3), z1s, SAFE)
-    _z2s = jnp.where((upper_bound2 < jnp.abs(z2s)) & (jnp.abs(z2s) < upper_bound3), z2s, SAFE)
+    _z1s = jnp.where(
+        (upper_bound2 < jnp.abs(z1s)) & (jnp.abs(z1s) < upper_bound3), z1s, SAFE
+    )
+    _z2s = jnp.where(
+        (upper_bound2 < jnp.abs(z2s)) & (jnp.abs(z2s) < upper_bound3), z2s, SAFE
+    )
 
     # Using one sided series expansion approximations
     Z = jnp.where(z1s > upper_bound2, _Z_far_tails(_z1s), Z)
     Z = jnp.where(z2s < -upper_bound2, _Z_far_tails(-_z2s), Z)
 
     # Ignore Z for linear approximation
     Z = jnp.where(z1s >= upper_bound3, SAFE, Z)
     Z = jnp.where(z2s <= -upper_bound3, SAFE, Z)
 
     return Z, z1s, z2s
 
 
-def grad_log_probit_likelihood(
-        f, y, likelihood_parameters,
-        single_precision=True):
-    upper_bound, upper_bound2, upper_bound3 = BOUNDS["single" if single_precision else "double"]
- 
+def grad_log_probit_likelihood(f, y, likelihood_parameters, single_precision=True):
+    upper_bound, upper_bound2, upper_bound3 = BOUNDS[
+        "single" if single_precision else "double"
+    ]
+
     noise_std = likelihood_parameters[0]
-    Z, z1s, z2s = _safe_Z(f, y, likelihood_parameters,
-        upper_bound, upper_bound2, upper_bound3)
+    Z, z1s, z2s = _safe_Z(
+        f, y, likelihood_parameters, upper_bound, upper_bound2, upper_bound3
+    )
 
     norm_pdf_z1s = norm_pdf(z1s)
     norm_pdf_z2s = norm_pdf(z2s)
 
     # ratio is approximated well linearly
     E = (norm_pdf_z1s - norm_pdf_z2s) / Z
     E = jnp.where(z1s > upper_bound3, z1s, E)
     E = jnp.where(z2s < -upper_bound3, z2s, E)
 
     return E / noise_std
 
 
-def hessian_log_probit_likelihood(
-        f, y, likelihood_parameters,
-        single_precision=True):
-
-    upper_bound, upper_bound2, upper_bound3 = BOUNDS["single" if single_precision else "double"]
+def hessian_log_probit_likelihood(f, y, likelihood_parameters, single_precision=True):
+    upper_bound, upper_bound2, upper_bound3 = BOUNDS[
+        "single" if single_precision else "double"
+    ]
 
     noise_std = likelihood_parameters[0]
-    Z, z1s, z2s = _safe_Z(f, y, likelihood_parameters,
-        upper_bound, upper_bound2, upper_bound3)
+    Z, z1s, z2s = _safe_Z(
+        f, y, likelihood_parameters, upper_bound, upper_bound2, upper_bound3
+    )
     norm_pdf_z1s = norm_pdf(z1s)
     norm_pdf_z2s = norm_pdf(z2s)
 
-    w = grad_log_probit_likelihood(f, y, likelihood_parameters,
-        single_precision)
+    w = grad_log_probit_likelihood(f, y, likelihood_parameters, single_precision)
 
     _z1s = jnp.where((z1s == -inf) | (z1s == inf), 0.0, z1s)
     _z2s = jnp.where((z2s == -inf) | (z2s == inf), 0.0, z2s)
-    V = -w**2 + (
-        _z1s * norm_pdf_z1s - _z2s * norm_pdf_z2s
-        ) / Z / noise_std**2
+    V = -(w**2) + (_z1s * norm_pdf_z1s - _z2s * norm_pdf_z2s) / Z / noise_std**2
 
-    V = jnp.where(z1s > upper_bound3, - noise_std ** -2, V)
-    V = jnp.where(z2s < -upper_bound3, - noise_std ** -2, V)
+    V = jnp.where(z1s > upper_bound3, -(noise_std**-2), V)
+    V = jnp.where(z2s < -upper_bound3, -(noise_std**-2), V)
     return V
 
 
-def probit(
-        noise_std, cutpoints_y, cutpoints_yplus1, f):
+def probit(noise_std, cutpoints_y, cutpoints_yplus1, f):
     """
     Return the normalising constants for the truncated normal distribution
     in a numerically stable manner.
 
     :arg float noise_std: The noise standard deviation.
     :arg cutpoints_y: cutpoints[y_train] (N, ) array of cutpoints
     :type cutpoints_y: :class:`numpy.ndarray`
@@ -201,58 +205,60 @@
     :arg f: The mean vector.
     :type f: :class:`numpy.ndarray`
     :arg y: data
     :type y: :class:`numpy.ndarray`
     :arg float upper_bound: The threshold of the normal z value for which
         the pdf is close enough to zero.
     :arg float upper_bound2: The threshold of the normal z value for which
-        the pdf is close enough to zero. 
+        the pdf is close enough to zero.
     :arg float tolerance: The tolerated absolute error.
     :returns: Z
     :rtype: :class:`numpy.ndarray`
     """
     # NOTE this is removing infs before and after an operation so that
     # the function can be automatically differentiated
     # TODO: double check that this is absolutely needed
     safe_z1s = jnp.where(cutpoints_y == -jnp.inf, 0.0, (cutpoints_y - f))
     safe_z2s = jnp.where(cutpoints_yplus1 == jnp.inf, 0.0, (cutpoints_yplus1 - f))
-    norm_cdf_z1s = jnp.where(cutpoints_y == -jnp.inf, 0.0, norm_cdf(safe_z1s / noise_std))
-    norm_cdf_z2s = jnp.where(cutpoints_yplus1 == jnp.inf, 1.0, norm_cdf(safe_z2s / noise_std))
+    norm_cdf_z1s = jnp.where(
+        cutpoints_y == -jnp.inf, 0.0, norm_cdf(safe_z1s / noise_std)
+    )
+    norm_cdf_z2s = jnp.where(
+        cutpoints_yplus1 == jnp.inf, 1.0, norm_cdf(safe_z2s / noise_std)
+    )
     Z = norm_cdf_z2s - norm_cdf_z1s
     return Z
 
 
 def probit_predictive_distributions(
-        likelihood_parameters,
-        posterior_mean, posterior_variance):
+    likelihood_parameters, posterior_mean, posterior_variance
+):
     """
     Return predictive distributions for the ordinal likelihood.
     """
     N_test = posterior_mean.shape[0]
     noise_std, cutpoints = likelihood_parameters
     J = B.size(cutpoints) - 1
     predictive_distributions = B.ones(N_test, J)
     posterior_pred_std = jnp.sqrt(posterior_variance + noise_std**2)
     posterior_pred_mean = posterior_mean
     for j in range(J):
         Z = probit(
-            posterior_pred_std,
-            cutpoints[j], cutpoints[j + 1],
-            posterior_pred_mean
-            )
+            posterior_pred_std, cutpoints[j], cutpoints[j + 1], posterior_pred_mean
+        )
         predictive_distributions[:, j] = Z
     return predictive_distributions
 
 
 def check_data(data):
     X_train, y_train = data
     if y_train.dtype not in [int, jnp.int32]:
         raise TypeError(
-            "t must contain only integer values (got {})".format(
-                y_train.dtype))
+            "t must contain only integer values (got {})".format(y_train.dtype)
+        )
     else:
         y_train = y_train.astype(int)
     return X_train, y_train
 
 
 def check_cutpoints(cutpoints, J):
     """
@@ -277,44 +283,45 @@
         if cutpoints[-1] != jnp.inf:
             if cutpoints[0] != jnp.NINF:
                 raise ValueError(
                     "Either the largest cutpoint parameter b_J is not "
                     "positive infinity, or the smallest cutpoint "
                     "parameter must b_0 is not negative infinity."
                     "(got {}, expected {})".format(
-                    [cutpoints[0], cutpoints[-1]], [jnp.inf, jnp.NINF]))
-            else:  #cutpoints[0] is -\infty
+                        [cutpoints[0], cutpoints[-1]], [jnp.inf, jnp.NINF]
+                    )
+                )
+            else:  # cutpoints[0] is -\infty
                 cutpoints.append(jnp.inf)
                 pass  # correct format
         else:
             cutpoints = jnp.insert(cutpoints, 0, jnp.NINF)
             pass  # correct format
     # Including all the cutpoints
     elif jnp.shape(cutpoints)[0] == J + 1:
         if cutpoints[0] != jnp.NINF:
             raise ValueError(
                 "The smallest cutpoint parameter b_0 must be negative "
-                "infinity (got {}, expected {})".format(
-                    cutpoints[0], jnp.NINF))
+                "infinity (got {}, expected {})".format(cutpoints[0], jnp.NINF)
+            )
         if cutpoints[-1] != jnp.inf:
             raise ValueError(
                 "The largest cutpoint parameter b_J must be positive "
-                "infinity (got {}, expected {})".format(
-                    cutpoints[-1], jnp.inf))
+                "infinity (got {}, expected {})".format(cutpoints[-1], jnp.inf)
+            )
         pass  # correct format
     else:
         raise ValueError(
             "Could not recognise cutpoints shape. "
-            "(jnp.shape(cutpoints) was {})".format(jnp.shape(cutpoints)))
+            "(jnp.shape(cutpoints) was {})".format(jnp.shape(cutpoints))
+        )
     assert cutpoints[0] == jnp.NINF
     assert cutpoints[-1] == jnp.inf
     assert jnp.shape(cutpoints)[0] == J + 1
-    if not all(
-            cutpoints[i] <= cutpoints[i + 1]
-            for i in range(J)):
+    if not all(cutpoints[i] <= cutpoints[i + 1] for i in range(J)):
         raise CutpointValueError(cutpoints)
     return cutpoints
 
 
 class CutpointValueError(Exception):
     """
     An invalid cutpoint argument was used to construct the classifier model.
@@ -326,18 +333,18 @@
 
         :arg cutpoint: The cutpoint parameters array.
         :type cutpoint: :class:`numpy.array` or list
 
         :rtype: :class:`CutpointValueError`
         """
         message = (
-                "The cutpoint list or array "
-                "must be in ascending order, "
-                f" {cutpoint} was given."
-                )
+            "The cutpoint list or array "
+            "must be in ascending order, "
+            f" {cutpoint} was given."
+        )
 
         super().__init__(message)
 
 
 class InvalidKernel(Exception):
     """An invalid kernel has been passed to `Approximator` or `Sampler`"""
 
@@ -345,13 +352,10 @@
         """
         Construct the exception.
 
         :arg kernel: The object pass to :class:`Approximator` or `Sampler`
             as the kernel argument.
         :rtype: :class:`InvalidKernel`
         """
-        message = (
-            f"{kernel} is not an instance of "
-            "mlkernels.Kernel"
-        )
+        message = f"{kernel} is not an instance of " "mlkernels.Kernel"
 
         super().__init__(message)
```

### Comparing `probit-0.0.0/probit.egg-info/PKG-INFO` & `probit-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-Metadata-Version: 2.1
-Name: probit
-Version: 0.0.0
-Summary: probit is a simple and accessible Gaussian process implementation in Jax.
-Home-page: https://github.com/bb515/probit
-Author: Benjamin Boys, Toby Boyne, Ieronymos Maxoutis
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # [probit](http://github.com/bb515/probit)
 [![CI](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml/badge.svg)](https://github.com/bb515/diffusionjax/actions/workflows/CI.yml)
 [![Coverage Status](https://coveralls.io/repos/github/bb515/diffusionjax/badge.svg?branch=master)](https://coveralls.io/github/bb515/diffusionjax?branch=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-probit is a simple and accessible Gaussian process package in Jax.
+![nPlan](readme_nplan.png)
+
+probit is a simple and accessible Gaussian process package in JAX. Thank you to [nPlan](https://www.nplan.io/), who are supporting this project.
 
 probit uses [MLKernels](https://github.com/wesselb/mlkernels) for the GP prior, see the available [means](https://github.com/wesselb/mlkernels#available-means) and [kernels](https://github.com/wesselb/mlkernels#available-kernels) with [compositional design](https://github.com/wesselb/mlkernels#compositional-design).
 
 Contents:
 
 - [Installation](#installation)
 - [Examples](#examples)
@@ -36,32 +28,34 @@
 >>>     lengthscale, signal_variance = prior_parameters
 >>>     # Here you can define the kernel that defines the Gaussian process
 >>>     return signal_variance * EQ().stretch(lengthscale).periodic(0.5)
 >>>
 >>> gaussian_process = GP(data=(X, y), prior=prior, log_likelihood=log_gaussian_likelihood)
 >>> likelihood_parameters = 1.0
 >>> prior_parameters = (1.0, 1.0)
->>> parameters = (likelihood_parameters, prior_parameters)
+>>> parameters = (prior_parameters, likelihood_parameters)
 >>> weight, precision = gaussian_process.approximate_posterior(parameters)
 >>> predictive_mean, predictive_variance = gaussian_process.predict(
 >>>     X_test,
 >>>     parameters, weight, precision)
 ```
 
-
 ## Installation
-`pip install probit` or for developers,
+The package requires Python 3.8+. First, it is recommended to [create a new python virtual environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). 
+probit depends on JAX. Because the JAX installation is different depending on your CUDA version, probit does not list JAX as a dependency in `setup.py`.
+First, [follow these instructions](https://github.com/google/jax#installation) to install JAX with the relevant accelerator support.
+Then, `pip install probit` or for developers,
 - Clone the repository `git clone git@github.com:bb515/probit.git`
 - Install using pip `pip install -e .` from the root directory of the repository (see the `setup.py` for the requirements that this command installs)
 
 ## Examples
 You can find examples of how to use the package under:`examples/`.
 
 ### Regression and hyperparameter optimization
-Run the regression example by typing `python example/regression.py`.
+Run the regression example by typing `python examples/regression.py`.
 ```python
 >>> def prior(prior_parameters):
 >>>     lengthscale, signal_variance = prior_parameters
 >>>     # Here you can define the kernel that defines the Gaussian process
 >>>     return signal_variance * EQ().stretch(lengthscale).periodic(0.5)
 >>>
 >>> # Generate data
@@ -114,15 +108,15 @@
 >>> noise_variance = vs.struct.noise_std()**2
 >>> obs_variance = variance + noise_variance
 >>> plot((X, y), (X_show, f_show), mean, obs_variance, fname="readme_regression_after.png")
 ```
 ![Prediction](readme_regression_after.png)
 
 ### Ordinal regression and hyperparameter optimization
-Run the ordinal regression example by typing `python example/classification.py`.
+Run the ordinal regression example by typing `python examples/classification.py`.
 
 ```python
 >>> # Generate data
 >>> J = 3  # use a value of J=2 for GP binary classification
 >>> key = random.PRNGKey(1)
 >>> noise_variance = 0.4
 >>> signal_variance = 1.0
@@ -172,15 +166,14 @@
 >>>     obs_variance, X_show, f_show, X, y, g_true,
 >>>     J, colors, fname="readme_classification_before")
 ```
 ![Prediction](readme_classification_before_contour.png)
 ![Prediction](readme_classification_before_mean_variance.png)
 
 ```python
->>>
 >>> # Evaluate model
 >>> mean, variance = classifier.predict(
 >>>     X_test,
 >>>     parameters,
 >>>     weight, precision)
 >>> predictive_distributions = probit_predictive_distributions(
 >>>     parameters[1],
@@ -195,23 +188,21 @@
 mean_absolute_error=0.41\
 log_pred_probability=-140986.54\
 mean_zero_one_error=0.39
 
 Before optimization, 
 parameters=(Array(1.2, dtype=float32), (Array(0.63245553, dtype=float64, weak_type=True), Array([       -inf, -0.54599167,  0.50296235,         inf], dtype=float64)))
 ```python
->>>
 >>> minimise_l_bfgs_b(objective, vs)
 >>> parameters = model(vs)
 >>> print("After optimization, \nparameters={}".format(model(vs)))
 ```
 After optimization, 
 parameters=(Array(0.07389855, dtype=float32), (Array(0.63245553, dtype=float64, weak_type=True), Array([       -inf, -0.54599167,  0.50296235,         inf], dtype=float64)))
 ```python
->>>
 >>> # Approximate posterior
 >>> parameters = model(vs)
 >>> weight, precision = classifier.approximate_posterior(parameters)
 >>> mean, variance = classifier.predict(
 >>>     X_show,
 >>>     parameters,
 >>>     weight, precision)
@@ -295,8 +286,7 @@
   author = 	 {King, Nathaniel J. and Lawrence, Neil D.},\
   year = 	 {2005},\
   number = {CS-05-06},\
   url = 	 {http://inverseprobability.com/publications/king-ppa05.html}}
 
 An [implicit functions tutorial](http://implicit-layers-tutorial.org/implicit_functions/) was used to define the fixed-point layer.
 
-
```

### Comparing `probit-0.0.0/probit.egg-info/SOURCES.txt` & `probit-0.0.2/probit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.md
 pyproject.toml
 readme_classification_after_contour.png
 readme_classification_after_mean_variance.png
 readme_classification_before_contour.png
 readme_classification_before_mean_variance.png
 readme_grad.png
+readme_nplan.png
 readme_objective.png
 readme_regression_after.png
 readme_regression_before.png
 requirements.txt
 setup.py
 .github/workflows/CI.yml
 .github/workflows/publish.yml
```

### Comparing `probit-0.0.0/readme_classification_after_contour.png` & `probit-0.0.2/readme_classification_after_contour.png`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/readme_classification_before_contour.png` & `probit-0.0.2/readme_classification_before_contour.png`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/readme_grad.png` & `probit-0.0.2/readme_grad.png`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/readme_objective.png` & `probit-0.0.2/readme_objective.png`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/readme_regression_after.png` & `probit-0.0.2/readme_regression_after.png`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/readme_regression_before.png` & `probit-0.0.2/readme_regression_before.png`

 * *Files identical despite different names*

### Comparing `probit-0.0.0/setup.py` & `probit-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """
 Setup script for probit.
 
 This setup is required or else
     >> ModuleNotFoundError: No module named 'probit'
 will occur.
 """
+
 from setuptools import setup, find_packages
 import pathlib
 
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
+
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
+
 # The text of the README file
 LICENSE = (HERE / "LICENSE.rst").read_text()
 
 
 setup(
     name="probit",
     python_requires=">=3.8",
-    description="probit is a simple and accessible Gaussian process implementation in Jax.",
+    description="probit is a simple and accessible Gaussian process implementation in Jax",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bb515/probit",
     author="Benjamin Boys, Toby Boyne, Ieronymos Maxoutis",
     license="MIT",
     license_file=LICENSE,
-    packages=find_packages(exclude=['*.test']),
+    packages=find_packages(exclude=["*.test"]),
     include_package_data=True,
     install_requires=[
-        'numpy',
-        'scipy',
-        'jaxlib>=0.4.1',
-        'jax>=0.4.1',
-        'jaxopt>=0.5.5'
-        'backends>=1.4.32',
-        'mlkernels>=0.3.6',
-        ]
-    )
+        "numpy",
+        "scipy",
+        "jaxopt>=0.5.5",
+        "backends>=1.4.32",
+        "mlkernels>=0.3.6",
+    ],
+)
```

