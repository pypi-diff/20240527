# Comparing `tmp/mkeima-0.5.0.tar.gz` & `tmp/mkeima-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkeima-0.5.0.tar", last modified: Sun Feb  5 13:33:18 2023, max compression
+gzip compressed data, was "mkeima-0.5.1.tar", last modified: Mon May 27 14:37:05 2024, max compression
```

## Comparing `mkeima-0.5.0.tar` & `mkeima-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-05 13:33:18.417501 mkeima-0.5.0/
--rw-rw-rw-   0        0        0    11358 2023-02-05 13:28:05.000000 mkeima-0.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2163 2023-02-05 13:33:18.415508 mkeima-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1545 2023-02-05 13:28:05.000000 mkeima-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-05 13:33:18.384286 mkeima-0.5.0/mkeima/
--rw-rw-rw-   0        0        0      339 2023-02-05 13:31:50.000000 mkeima-0.5.0/mkeima/__init__.py
--rw-rw-rw-   0        0        0     6816 2023-02-05 13:28:05.000000 mkeima-0.5.0/mkeima/analyze.py
--rw-rw-rw-   0        0        0    15577 2023-02-05 13:28:05.000000 mkeima-0.5.0/mkeima/plot.py
--rw-rw-rw-   0        0        0     4911 2023-02-05 13:28:05.000000 mkeima-0.5.0/mkeima/read.py
-drwxrwxrwx   0        0        0        0 2023-02-05 13:33:18.413511 mkeima-0.5.0/mkeima.egg-info/
--rw-rw-rw-   0        0        0     2163 2023-02-05 13:33:18.000000 mkeima-0.5.0/mkeima.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-02-05 13:33:18.000000 mkeima-0.5.0/mkeima.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-05 13:33:18.000000 mkeima-0.5.0/mkeima.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-02-05 13:33:18.000000 mkeima-0.5.0/mkeima.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-05 13:33:18.000000 mkeima-0.5.0/mkeima.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      857 2023-02-05 13:28:05.000000 mkeima-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-05 13:33:18.418498 mkeima-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-02-05 13:28:05.000000 mkeima-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:37:05.778262 mkeima-0.5.1/
+-rw-rw-rw-   0        0        0    11358 2023-02-05 13:28:05.000000 mkeima-0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2281 2024-05-27 14:37:05.778262 mkeima-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1545 2023-02-05 13:28:05.000000 mkeima-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 14:37:05.747015 mkeima-0.5.1/mkeima/
+-rw-rw-rw-   0        0        0      339 2024-05-27 14:34:03.000000 mkeima-0.5.1/mkeima/__init__.py
+-rw-rw-rw-   0        0        0     7647 2024-05-27 14:34:03.000000 mkeima-0.5.1/mkeima/analyze.py
+-rw-rw-rw-   0        0        0    15578 2024-05-27 14:34:03.000000 mkeima-0.5.1/mkeima/plot.py
+-rw-rw-rw-   0        0        0     4911 2023-02-05 13:28:05.000000 mkeima-0.5.1/mkeima/read.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:37:05.778262 mkeima-0.5.1/mkeima.egg-info/
+-rw-rw-rw-   0        0        0     2281 2024-05-27 14:37:05.000000 mkeima-0.5.1/mkeima.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-27 14:37:05.000000 mkeima-0.5.1/mkeima.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 14:37:05.000000 mkeima-0.5.1/mkeima.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-27 14:37:05.000000 mkeima-0.5.1/mkeima.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-27 14:37:05.000000 mkeima-0.5.1/mkeima.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      857 2023-02-05 13:28:05.000000 mkeima-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 14:37:05.778262 mkeima-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-02-05 13:28:05.000000 mkeima-0.5.1/setup.py
```

### Comparing `mkeima-0.5.0/LICENSE.txt` & `mkeima-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkeima-0.5.0/PKG-INFO` & `mkeima-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: mkeima
-Version: 0.5.0
+Version: 0.5.1
 Summary: Analysis of flow cytometry-based mKeima assays in Python
 Author-email: "David M. Hollenstein" <hollenstein.david@gmail.com>
 License: Apache-2.0
 Keywords: mkeima,flow cytometry,data analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: matplotlib>=3.4
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=1.4
+Requires-Dist: seaborn>=0.11
 
 # mkeima: Analyze flow cytometry-based mKeima assays in Python
 
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 
 mkeima is a Python library for the analysis and visualization of flow cytometry-based
 mKeima assays.
```

### Comparing `mkeima-0.5.0/README.md` & `mkeima-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mkeima-0.5.0/mkeima/analyze.py` & `mkeima-0.5.1/mkeima/analyze.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+"""This module provides functions for analyzing FACS data.
+
+The following functions are available:
+
+- `calculate_mkeima_score`: Adds "low pH mkeima" to "high pH mkeima" scores. mKeima
+    scores are log ratios of low pH to high pH mKeima signals, normalized to a reference
+    sample by calculating z-scores using the median and standard deviation of the
+    reference sample.
+- `summarize`: Calculates summary statistics (mean, median, std, and number  of cells).
+- `summarize_outliers`: Calculates the amount of outliers for each condition and
+    replicate. Outliers are defined as events with a value above the a certain
+    percentile (by default 98.5%) of the reference population.
+"""
 from typing import Optional
 
 import pandas as pd
 import numpy as np
 
 
 def calculate_mkeima_score(
@@ -128,40 +141,44 @@
             and outliers are calculated for each group separately.
 
     Returns:
         A dataframe containing the columns "Condition", "Replicate", "Total cells",
         "Outliers", "Outliers [%]", and the columns specified by the 'group_by'
         argument.
     """
-    groups = []
+    default_grouping = ["Condition", "Replicate"]
     if group_by is not None:
-        for group_name in data[group_by].unique():
-            group_mask = data[group_by] == group_name
-            groups.append((group_name, group_mask))
+        group_by = [by for by in group_by if by not in default_grouping]
+        if not group_by:
+            group_by = None
+
+    if group_by is None:
+        grouping = [(None, data)]
     else:
-        group_name = "Total"
-        group_mask = np.ones(data.shape[0], dtype=bool)
-        groups.append((group_name, group_mask))
-
-    results_list = []
-    for group_name, group_mask in groups:
-        group_data = data[group_mask].copy()
+        grouping = data.groupby(group_by)
+
+    group_results = []
+    for group_name, group_data in grouping:
         reference_mask = group_data["Condition"] == reference
         reference_scores = group_data.loc[reference_mask, on]
         cutoff_uppers = np.percentile(reference_scores, reference_percentile)
 
         results = (
-            group_data.groupby(by=["Condition", "Replicate"])
+            group_data.groupby(by=default_grouping)
             .agg(
                 Total_cells=(on, "size"),
                 Outliers=(on, lambda x: (x >= cutoff_uppers).sum()),
             )
             .reset_index()
         )
-
         results["Outliers [%]"] = (results["Outliers"] / results["Total_cells"]) * 100
         results.rename(columns={"Total_cells": "Total cells"}, inplace=True)
-        if groupby is not None:
-            results[groupby] = group_name
-        results_list.append(results)
-    results_table = pd.concat(results_list, ignore_index=True)
+
+        # Add columns from the user specified grouping
+        if group_name is not None:
+            if isinstance(group_name, str):
+                group_name = (group_name,)
+            for column_value, column in zip(group_name, group_by):
+                results[column] = column_value
+        group_results.append(results)
+    results_table = pd.concat(group_results, ignore_index=True)
     return results_table
```

### Comparing `mkeima-0.5.0/mkeima/plot.py` & `mkeima-0.5.1/mkeima/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,15 +416,15 @@
             palette=colors,
         )
         sns.swarmplot(
             data=group_data,
             x=group_by,
             y=on,
             order=group_order,
-            dodge=True,
+            dodge=False,
             edgecolor="#000000",
             linewidth=0.75,
             ax=ax,
             palette=colors,
         )
         if pos != 0:
             ax.set_ylabel("")
```

### Comparing `mkeima-0.5.0/mkeima/read.py` & `mkeima-0.5.1/mkeima/read.py`

 * *Files identical despite different names*

### Comparing `mkeima-0.5.0/mkeima.egg-info/PKG-INFO` & `mkeima-0.5.1/mkeima.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: mkeima
-Version: 0.5.0
+Version: 0.5.1
 Summary: Analysis of flow cytometry-based mKeima assays in Python
 Author-email: "David M. Hollenstein" <hollenstein.david@gmail.com>
 License: Apache-2.0
 Keywords: mkeima,flow cytometry,data analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: matplotlib>=3.4
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=1.4
+Requires-Dist: seaborn>=0.11
 
 # mkeima: Analyze flow cytometry-based mKeima assays in Python
 
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 
 mkeima is a Python library for the analysis and visualization of flow cytometry-based
 mKeima assays.
```

### Comparing `mkeima-0.5.0/pyproject.toml` & `mkeima-0.5.1/pyproject.toml`

 * *Files identical despite different names*

