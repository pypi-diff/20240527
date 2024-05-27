# Comparing `tmp/ministats-0.3.1.tar.gz` & `tmp/ministats-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ministats-0.3.1.tar", last modified: Wed May  1 12:37:52 2024, max compression
+gzip compressed data, was "ministats-0.3.2.tar", last modified: Mon May 27 17:04:11 2024, max compression
```

## Comparing `ministats-0.3.1.tar` & `ministats-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.685646 ministats-0.3.1/
--rw-r--r--   0 ivan       (501) staff       (20)     3644 2023-06-29 19:55:38.000000 ministats-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 ivan       (501) staff       (20)      165 2024-03-28 16:54:20.000000 ministats-0.3.1/HISTORY.md
--rw-r--r--   0 ivan       (501) staff       (20)     1069 2023-06-29 19:16:59.000000 ministats-0.3.1/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)      239 2024-03-28 14:53:04.000000 ministats-0.3.1/MANIFEST.in
--rw-r--r--   0 ivan       (501) staff       (20)     2648 2024-05-01 12:37:52.685849 ministats-0.3.1/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     1558 2024-03-29 16:17:49.000000 ministats-0.3.1/README.md
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.673581 ministats-0.3.1/docs/
--rw-r--r--   0 ivan       (501) staff       (20)      610 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/Makefile
--rwxr-xr-x   0 ivan       (501) staff       (20)     4822 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/conf.py
--rw-r--r--   0 ivan       (501) staff       (20)       33 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/contributing.rst
--rw-r--r--   0 ivan       (501) staff       (20)       28 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/history.rst
--rw-r--r--   0 ivan       (501) staff       (20)      301 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/index.rst
--rw-r--r--   0 ivan       (501) staff       (20)     1168 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/installation.rst
--rw-r--r--   0 ivan       (501) staff       (20)      771 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/make.bat
--rw-r--r--   0 ivan       (501) staff       (20)       27 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/readme.rst
--rw-r--r--   0 ivan       (501) staff       (20)       79 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/usage.rst
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.680012 ministats-0.3.1/ministats/
--rw-r--r--   0 ivan       (501) staff       (20)     1528 2024-05-01 12:36:30.000000 ministats-0.3.1/ministats/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     2919 2024-03-29 15:17:22.000000 ministats-0.3.1/ministats/confidence_intervals.py
--rw-r--r--   0 ivan       (501) staff       (20)     1017 2024-03-29 15:01:45.000000 ministats-0.3.1/ministats/estimators.py
--rw-r--r--   0 ivan       (501) staff       (20)     1228 2024-03-29 15:17:16.000000 ministats-0.3.1/ministats/formulas.py
--rw-r--r--   0 ivan       (501) staff       (20)    10121 2024-03-29 15:00:07.000000 ministats-0.3.1/ministats/hypothesis_tests.py
--rw-r--r--   0 ivan       (501) staff       (20)    36208 2024-04-28 17:35:06.000000 ministats-0.3.1/ministats/plots.py
--rw-r--r--   0 ivan       (501) staff       (20)     2869 2024-03-29 14:58:15.000000 ministats-0.3.1/ministats/probs.py
--rw-r--r--   0 ivan       (501) staff       (20)     1686 2024-03-29 14:58:48.000000 ministats-0.3.1/ministats/sampling.py
--rw-r--r--   0 ivan       (501) staff       (20)     4106 2024-03-29 15:17:12.000000 ministats-0.3.1/ministats/simulations.py
--rw-r--r--   0 ivan       (501) staff       (20)     2118 2024-03-28 14:51:57.000000 ministats-0.3.1/ministats/utils.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.682778 ministats-0.3.1/ministats.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)     2648 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      721 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/not-zip-safe
--rw-r--r--   0 ivan       (501) staff       (20)       85 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)       10 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/top_level.txt
--rw-r--r--   0 ivan       (501) staff       (20)      424 2024-05-01 12:37:52.686796 ministats-0.3.1/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1652 2024-05-01 12:36:30.000000 ministats-0.3.1/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.684929 ministats-0.3.1/tests/
--rw-r--r--   0 ivan       (501) staff       (20)       39 2023-06-29 19:16:59.000000 ministats-0.3.1/tests/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     1188 2024-03-29 14:15:25.000000 ministats-0.3.1/tests/test_estimtors.py
--rw-r--r--   0 ivan       (501) staff       (20)      526 2024-03-29 14:15:20.000000 ministats-0.3.1/tests/test_ministats.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-27 17:04:11.837557 ministats-0.3.2/
+-rw-r--r--   0 ivan       (501) staff       (20)     3644 2023-06-29 19:55:38.000000 ministats-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 ivan       (501) staff       (20)      165 2024-03-28 16:54:20.000000 ministats-0.3.2/HISTORY.md
+-rw-r--r--   0 ivan       (501) staff       (20)     1069 2023-06-29 19:16:59.000000 ministats-0.3.2/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)      239 2024-03-28 14:53:04.000000 ministats-0.3.2/MANIFEST.in
+-rw-r--r--   0 ivan       (501) staff       (20)     2823 2024-05-27 17:04:11.837382 ministats-0.3.2/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     1558 2024-03-29 16:17:49.000000 ministats-0.3.2/README.md
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-27 17:04:11.824482 ministats-0.3.2/docs/
+-rw-r--r--   0 ivan       (501) staff       (20)      610 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/Makefile
+-rwxr-xr-x   0 ivan       (501) staff       (20)     4822 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/conf.py
+-rw-r--r--   0 ivan       (501) staff       (20)       33 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/contributing.rst
+-rw-r--r--   0 ivan       (501) staff       (20)       28 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/history.rst
+-rw-r--r--   0 ivan       (501) staff       (20)      301 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/index.rst
+-rw-r--r--   0 ivan       (501) staff       (20)     1168 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/installation.rst
+-rw-r--r--   0 ivan       (501) staff       (20)      771 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/make.bat
+-rw-r--r--   0 ivan       (501) staff       (20)       27 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/readme.rst
+-rw-r--r--   0 ivan       (501) staff       (20)       79 2023-06-29 19:16:59.000000 ministats-0.3.2/docs/usage.rst
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-27 17:04:11.831318 ministats-0.3.2/ministats/
+-rw-r--r--   0 ivan       (501) staff       (20)     1528 2024-05-27 17:03:40.000000 ministats-0.3.2/ministats/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2919 2024-03-29 15:17:22.000000 ministats-0.3.2/ministats/confidence_intervals.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1017 2024-03-29 15:01:45.000000 ministats-0.3.2/ministats/estimators.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1228 2024-05-10 12:59:00.000000 ministats-0.3.2/ministats/formulas.py
+-rw-r--r--   0 ivan       (501) staff       (20)    10121 2024-03-29 15:00:07.000000 ministats-0.3.2/ministats/hypothesis_tests.py
+-rw-r--r--   0 ivan       (501) staff       (20)    37792 2024-05-17 03:14:57.000000 ministats-0.3.2/ministats/plots.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2869 2024-03-29 14:58:15.000000 ministats-0.3.2/ministats/probs.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1686 2024-03-29 14:58:48.000000 ministats-0.3.2/ministats/sampling.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4106 2024-03-29 15:17:12.000000 ministats-0.3.2/ministats/simulations.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2118 2024-03-28 14:51:57.000000 ministats-0.3.2/ministats/utils.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-27 17:04:11.836778 ministats-0.3.2/ministats.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)     2823 2024-05-27 17:04:11.000000 ministats-0.3.2/ministats.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      721 2024-05-27 17:04:11.000000 ministats-0.3.2/ministats.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2024-05-27 17:04:11.000000 ministats-0.3.2/ministats.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2024-05-27 17:04:11.000000 ministats-0.3.2/ministats.egg-info/not-zip-safe
+-rw-r--r--   0 ivan       (501) staff       (20)       85 2024-05-27 17:04:11.000000 ministats-0.3.2/ministats.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       10 2024-05-27 17:04:11.000000 ministats-0.3.2/ministats.egg-info/top_level.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      424 2024-05-27 17:04:11.838247 ministats-0.3.2/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1652 2024-05-27 17:03:40.000000 ministats-0.3.2/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-27 17:04:11.836024 ministats-0.3.2/tests/
+-rw-r--r--   0 ivan       (501) staff       (20)       39 2023-06-29 19:16:59.000000 ministats-0.3.2/tests/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1188 2024-03-29 14:15:25.000000 ministats-0.3.2/tests/test_estimtors.py
+-rw-r--r--   0 ivan       (501) staff       (20)      526 2024-03-29 14:15:20.000000 ministats-0.3.2/tests/test_ministats.py
```

### Comparing `ministats-0.3.1/CONTRIBUTING.md` & `ministats-0.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/LICENSE` & `ministats-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/PKG-INFO` & `ministats-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ministats
-Version: 0.3.1
+Version: 0.3.2
 Summary: Common statistical testing procedures used for STATS 101 topics. The code is intentionally simple to make it easy to forllow for beginners.
 Home-page: https://github.com/minireference/ministats
 Author: Ivan Savov
 Author-email: ivan@minireference.com
 License: MIT license
 Keywords: ministats
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: numpy>=1.24
+Requires-Dist: scipy>=1.6
+Requires-Dist: pandas>=2
+Requires-Dist: seaborn>=0.13.2
+Requires-Dist: statsmodels>=0.14.1
 
 # Mini Stats Helpers
 
 [![image](https://img.shields.io/pypi/v/ministats.svg)](https://pypi.python.org/pypi/ministats)
 [![Documentation Status](https://readthedocs.org/projects/ministats/badge/?version=latest)](https://ministats.readthedocs.io/en/latest/?version=latest)
 
 Common statistical testing procedures used for STATS 101 topics.
```

### Comparing `ministats-0.3.1/README.md` & `ministats-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/docs/Makefile` & `ministats-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/docs/conf.py` & `ministats-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/docs/installation.rst` & `ministats-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/docs/make.bat` & `ministats-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/__init__.py` & `ministats-0.3.2/ministats/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Mini Statistics."""
 
 __author__ = """Ivan Savov"""
 __email__ = 'ivan@minireference.com'
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 from .confidence_intervals import (
     ci_mean,
     ci_var,
     ci_dmeans,
 )
```

### Comparing `ministats-0.3.1/ministats/confidence_intervals.py` & `ministats-0.3.2/ministats/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/estimators.py` & `ministats-0.3.2/ministats/estimators.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/formulas.py` & `ministats-0.3.2/ministats/formulas.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/hypothesis_tests.py` & `ministats-0.3.2/ministats/hypothesis_tests.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/plots.py` & `ministats-0.3.2/ministats/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import matplotlib.pyplot as plt
+import matplotlib.lines as mlines
 import numpy as np
 import pandas as pd
 from scipy.integrate import quad
 import seaborn as sns
 import statsmodels.formula.api as smf
 import statsmodels.api as sm
 
@@ -10,14 +11,15 @@
 from scipy.stats import nbinom     # display parameter n as r
 from scipy.stats import hypergeom  # special handling M=a+b, n=a, N=n
 from scipy.stats import expon      # hide loc=0 parameter
 from scipy.stats import gamma      # hide loc=0 parameter
 from scipy.stats import norm
 from scipy.stats import t as tdist
 
+
 from .utils import ensure_containing_dir_exists
 from .utils import default_labeler
 from .sampling import gen_sampling_dist
 
 # Useful colors
 snspal = sns.color_palette()
 blue, orange, red, purple = snspal[0], snspal[1], snspal[3], snspal[4]
@@ -890,15 +892,15 @@
     return ax
 
 
 def plot_lm_partial(lmfit, pred, others=None, ax=None):
     """
     Generate a partial regression plot from the best-fit line
     of the predictor `pred`, where the intercept is calculated
-    from the average of the `other` predictors time their params.
+    from the average of the `other` predictors.
     """
     ax = plt.gca() if ax is None else ax
     data = lmfit.model.data.orig_exog
     params = lmfit.params
     allpreds = set(data.columns) - {"Intercept"}
     assert pred in allpreds 
     others = allpreds - {pred} if others is None else others
@@ -908,57 +910,87 @@
     slope = params[pred]
     print(pred, "intercept=", intercept, "slope=", slope)
     xs = np.linspace(data[pred].min(), data[pred].max())
     ys = intercept + slope*xs
     sns.lineplot(x=xs, y=ys, ax=ax)
 
 
+def plot_lm_partial_cat(lmfit, pred, others=None, color="C0", linestyle="solid", cats=None, ax=None):
+    """
+    Generate a partial regression plot from the best-fit line
+    of the predictor `pred`, where the intercept is calculated
+    from the average of the `other` predictors,
+    including the value of categorical predictors `cats` in the slope.
+    """
+    ax = plt.gca() if ax is None else ax
+    data = lmfit.model.data.orig_exog
+    params = lmfit.params
+    allpreds = set(data.columns) - {"Intercept"}
+    allnoncatpreds = set([pred for pred in allpreds if "T." not in pred])
+    assert pred in allnoncatpreds
+    others = allnoncatpreds - {pred} if others is None else others
+    intercept = params["Intercept"]
+    for other in others:
+        intercept += params[other]*data[other].mean() 
+    for cat in cats:
+        intercept += params[cat]
+    slope = params[pred]
+    print(pred, "intercept=", intercept, "slope=", slope)
+    xs = np.linspace(data[pred].min(), data[pred].max())
+    ys = intercept + slope*xs
+    sns.lineplot(x=xs, y=ys, color=color, ax=ax, linestyle=linestyle)
+
+
+
 def plot_lm_ttest(data, x, y, ax=None):
     """
     Plot a combined scatterplot, means, and LM slope line
     to illustrate the equivalence between two-sample t-test
     and a linear model with a single binary predictor `x`.
     """
     # Fit the linear model
     lm = smf.ols(formula=f"{y} ~ 1 + C({x})", data=data).fit()
     beta0, beta1 = lm.params
     interceptlab, slopelab = lm.params.index
 
     # Plot the data
     ax = plt.gca() if ax is None else ax
-    sns.stripplot(data=data, x=x, y=y, hue=x, jitter=0, alpha=0.3)
+    sns.stripplot(data=data, x=x, y=y, hue=x, size=3, jitter=0, alpha=0.2)
     sns.pointplot(data=data, x=x, y=y, hue=x, estimator="mean", errorbar=None, marker="D")
 
     # Customize plot labels
     xlabel0, xlabel1 = [l.get_text() for l in ax.get_xticklabels()]
     newxlabel0 = xlabel0 + "\n0"
     newxlabel1 = xlabel1 + "\n1"
     ax.set_xticks([0,1])
     ax.set_xticklabels([newxlabel0, newxlabel1])
     ax.set_xlim([-0.3, 1.3])
+    ax.set_xlabel(f"$\\texttt{{{x}}}_{{\\texttt{{{xlabel1}}}}}$")
+    ax.xaxis.set_label_coords(0.5, -0.15)
 
     # Get seaborn colors
     snspal = sns.color_palette()
 
     # Add h-lines to represent the two group means
-    ax.hlines(beta0, xmin=-0.3, xmax=1.3, color=snspal[0],
-              label=f"$\\beta_0$ = \\texttt{{{interceptlab}}} = {xlabel0} mean")
-    ax.hlines(beta0+beta1, xmin=0.8, xmax=1.2, color=snspal[1],
-              label=f"$\\beta_0 + \\beta_{{\\texttt{{{xlabel1}}}}}$ = {xlabel1} mean")
+    ax.hlines(beta0, xmin=-0.3, xmax=1.3, color=snspal[0])
+    ax.hlines(beta0+beta1, xmin=0.8, xmax=1.2, color=snspal[1])
 
     # Add diagonal to represent difference between means
-    ax.plot(
-        [0, 1],
-        [beta0, beta0 + beta1],
-        color="k",
-        label=f"$\\beta_{{\\texttt{{{xlabel1}}}}}$ = \\texttt{{{slopelab}}} slope",
-    )
+    ax.plot([0, 1], [beta0, beta0 + beta1], color="k")
+
+    # Draw custom legend
+    blue_diamond = mlines.Line2D([], [], color=snspal[0], marker='D', ls="",
+        label=f"$\\widehat{{\\beta}}_0$ = \\texttt{{{interceptlab}}} = {xlabel0} mean")
+    yellow_diamond = mlines.Line2D([], [], color=snspal[1], marker='D', ls="",
+        label=f"$\\widehat{{\\beta}}_0 + \\widehat{{\\beta}}_{{\\texttt{{{xlabel1}}}}}$ = {xlabel1} mean")
+    slope_line = mlines.Line2D([], [], color="k",
+        label=f"$\\widehat{{\\beta}}_{{\\texttt{{{xlabel1}}}}}$ = \\texttt{{{slopelab}}} slope")
+    ax.legend(handles=[blue_diamond, yellow_diamond, slope_line])
 
     # Return axes
-    ax.legend()
     return ax
 
 
 def plot_lm_anova(data, x, y, ax=None):
     """
     Plot a combined scatterplot, means, and LM slope lines
     to illustrate the equivalence between ANOVA test and
@@ -974,32 +1006,32 @@
     snspal = sns.color_palette()
     linestyles = ['solid', 'dotted', 'dashed', 'dashdot',
                   (0, (3, 5, 1, 5, 1, 5)),  # dashdotdotted
                   (5, (10, 3))]             # long dash with offset
 
     # Plot the data
     ax = plt.gca() if ax is None else ax
-    sns.stripplot(data=data, x=x, y=y, hue=x, jitter=0, alpha=0.3, order=labels, hue_order=labels)
+    sns.stripplot(data=data, x=x, y=y, hue=x, size=3, jitter=0, alpha=0.2, order=labels, hue_order=labels)
     sns.pointplot(data=data, x=x, y=y, hue=x, estimator="mean", errorbar=None, marker="D", hue_order=labels)
     
     # Group 1 (baseline)
-    beta0 = lm.params[0]
+    beta0 = lm.params.iloc[0]
     interceptlab = lm.params.index[0]
     ax.axhline(beta0, color=snspal[0], linewidth=1,
-               label=f"$\\beta_0$ = \\texttt{{{interceptlab}}} = {labels[0]} mean")
+               label=f"$\\widehat{{\\beta}}_0$ = \\texttt{{{interceptlab}}} = \\texttt{{{labels[0]}}} mean")
 
     # Remaining groups
     for i in range(1, len(labels)):
         label = labels[i]
-        beta = lm.params[i]
+        beta = lm.params.iloc[i]
         slopelab = lm.params.index[i]
         linestyle = linestyles[i%len(linestyles)]
         ax.hlines(beta0+beta, xmin=i-0.2, xmax=i+0.2, color=snspal[i])
         ax.plot([i-0.7, i], [beta0, beta0 + beta], color="k", linestyle=linestyle,
-                label=f"$\\beta_{{\\texttt{{{label}}}}}$ = \\texttt{{{slopelab}}} slope")
+                label=f"$\\widehat{{\\beta}}_{{\\texttt{{{label}}}}}$ = \\texttt{{{slopelab}}} slope")
 
     # Return axes
     ax.legend()
     return ax
 
 
 def plot_lm_scale_loc(lmfit, pred=None):
```

### Comparing `ministats-0.3.1/ministats/probs.py` & `ministats-0.3.2/ministats/probs.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/sampling.py` & `ministats-0.3.2/ministats/sampling.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/simulations.py` & `ministats-0.3.2/ministats/simulations.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats/utils.py` & `ministats-0.3.2/ministats/utils.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/ministats.egg-info/PKG-INFO` & `ministats-0.3.2/ministats.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ministats
-Version: 0.3.1
+Version: 0.3.2
 Summary: Common statistical testing procedures used for STATS 101 topics. The code is intentionally simple to make it easy to forllow for beginners.
 Home-page: https://github.com/minireference/ministats
 Author: Ivan Savov
 Author-email: ivan@minireference.com
 License: MIT license
 Keywords: ministats
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib>=3.7
+Requires-Dist: numpy>=1.24
+Requires-Dist: scipy>=1.6
+Requires-Dist: pandas>=2
+Requires-Dist: seaborn>=0.13.2
+Requires-Dist: statsmodels>=0.14.1
 
 # Mini Stats Helpers
 
 [![image](https://img.shields.io/pypi/v/ministats.svg)](https://pypi.python.org/pypi/ministats)
 [![Documentation Status](https://readthedocs.org/projects/ministats/badge/?version=latest)](https://ministats.readthedocs.io/en/latest/?version=latest)
 
 Common statistical testing procedures used for STATS 101 topics.
```

### Comparing `ministats-0.3.1/ministats.egg-info/SOURCES.txt` & `ministats-0.3.2/ministats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/setup.py` & `ministats-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     include_package_data=True,
     keywords='ministats',
     name='ministats',
     packages=find_packages(include=['ministats', 'ministats.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/minireference/ministats',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False,
 )
```

### Comparing `ministats-0.3.1/tests/test_estimtors.py` & `ministats-0.3.2/tests/test_estimtors.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.1/tests/test_ministats.py` & `ministats-0.3.2/tests/test_ministats.py`

 * *Files identical despite different names*

