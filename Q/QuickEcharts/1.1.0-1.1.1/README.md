# Comparing `tmp/quickecharts-1.1.0.tar.gz` & `tmp/quickecharts-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickEcharts-1.1.0.tar", last modified: Thu May 23 16:22:02 2024, max compression
+gzip compressed data, was "QuickEcharts-1.1.1.tar", last modified: Mon May 27 18:27:33 2024, max compression
```

## Comparing `quickecharts-1.1.0.tar` & `quickecharts-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:22:02.642511 QuickEcharts-1.1.0/
--rw-rw-rw-   0        0        0    31892 2023-06-03 03:56:56.000000 QuickEcharts-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       78 2024-03-22 23:36:21.000000 QuickEcharts-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    69628 2024-05-23 16:22:02.642009 QuickEcharts-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 16:22:02.623010 QuickEcharts-1.1.0/QuickEcharts/
--rw-rw-rw-   0        0        0   340583 2024-05-23 16:19:21.000000 QuickEcharts-1.1.0/QuickEcharts/Charts.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:22:02.640511 QuickEcharts-1.1.0/QuickEcharts.egg-info/
--rw-rw-rw-   0        0        0    69628 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:22:02.000000 QuickEcharts-1.1.0/QuickEcharts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    69141 2024-05-23 16:21:14.000000 QuickEcharts-1.1.0/README.md
--rw-rw-rw-   0        0        0      693 2024-03-26 19:47:36.000000 QuickEcharts-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       19 2024-03-05 17:52:13.000000 QuickEcharts-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 16:22:02.642511 QuickEcharts-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1046 2024-05-23 16:19:42.000000 QuickEcharts-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:27:33.142087 QuickEcharts-1.1.1/
+-rw-rw-rw-   0        0        0    31892 2023-06-03 03:56:56.000000 QuickEcharts-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       78 2024-03-22 23:36:21.000000 QuickEcharts-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    69628 2024-05-27 18:27:33.141587 QuickEcharts-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-27 18:27:33.124087 QuickEcharts-1.1.1/QuickEcharts/
+-rw-rw-rw-   0        0        0   340514 2024-05-27 18:26:13.000000 QuickEcharts-1.1.1/QuickEcharts/Charts.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:27:33.140087 QuickEcharts-1.1.1/QuickEcharts.egg-info/
+-rw-rw-rw-   0        0        0    69628 2024-05-27 18:27:33.000000 QuickEcharts-1.1.1/QuickEcharts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-05-27 18:27:33.000000 QuickEcharts-1.1.1/QuickEcharts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:27:33.000000 QuickEcharts-1.1.1/QuickEcharts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-27 18:27:33.000000 QuickEcharts-1.1.1/QuickEcharts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:27:33.000000 QuickEcharts-1.1.1/QuickEcharts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    69141 2024-05-23 16:21:14.000000 QuickEcharts-1.1.1/README.md
+-rw-rw-rw-   0        0        0      693 2024-03-26 19:47:36.000000 QuickEcharts-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       19 2024-03-05 17:52:13.000000 QuickEcharts-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:27:33.142087 QuickEcharts-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1046 2024-05-27 18:26:25.000000 QuickEcharts-1.1.1/setup.py
```

### Comparing `QuickEcharts-1.1.0/LICENSE` & `QuickEcharts-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QuickEcharts-1.1.0/PKG-INFO` & `QuickEcharts-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickEcharts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Create Echart plots in a single simple function call, with internal data wrangling via polars
 Home-page: https://github.com/AdrianAntico/QuickEcharts
 Author: ['Adrian Antico']
 Author-email: adrianantico@gmail.com
 License: AGPL >= 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `QuickEcharts-1.1.0/QuickEcharts/Charts.py` & `QuickEcharts-1.1.1/QuickEcharts/Charts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # Module: Charts
 # Author: Adrian Antico <adrianantico@gmail.com>
 # License: APGL (>= 3)
-# Release: quickecharts 1.1.0
+# Release: quickecharts 1.1.1
 # Last modified : 2024-03-26
 
 def NumericTransformation(dt, YVar, Trans):
   """
   Parameters
   dt: polars dataframe
   YVar: column to transform
   Trans: transformation method. Choose from 'sqrt', 'log', 'logmin', 'asinh', 'perc_rank'
   """
   Trans = Trans.lower()
-  import math
+  import numpy as np
   import polars as pl
   if Trans == "sqrt":
-    dt = dt.with_columns(pl.col(YVar).map_elements(math.sqrt))
+    dt = dt.with_columns(pl.col(YVar).sqrt())
   elif Trans == 'log':
-    dt = dt.with_columns(pl.col(YVar).map_elements(math.log))
+    dt = dt.with_columns(pl.col(YVar).log())
   elif Trans == 'asinh':
-    dt = dt.with_columns(pl.col(YVar).map_elements(math.asinh))
+    dt = dt.with_columns(np.arcsinh(pl.col(YVar)))
   elif Trans == 'logmin':
     dt = dt.with_columns(YVar = dt[YVar] + 1 + dt[YVar].min())
     dt = dt.drop(YVar)
     dt = dt.rename({"YVar": YVar})
-    dt = dt.with_columns(pl.col(YVar).map_elements(math.log))
+    dt = dt.with_columns(pl.col(YVar).log())
   elif Trans == 'perc_rank':
     perc_rank = dt[YVar].rank() / dt[YVar].count()
     dt = dt.drop(YVar)
     dt = dt.with_columns(perc_rank.rename(YVar))
   return dt
 
 
 def PolarsAggregation(dt, AggMethod, NumericVariable, GroupVariable, DateVariable):
   import polars as pl
-  import math
   if AggMethod == "count":
     if not GroupVariable is None and not DateVariable is None:
       dt = dt.group_by(GroupVariable, DateVariable).agg(pl.col(NumericVariable).len())
     elif not GroupVariable is None:
       dt = dt.group_by(GroupVariable).agg(pl.col(NumericVariable).len())
     else:
       dt = dt.group_by(DateVariable).agg(pl.col(NumericVariable).len())
@@ -276,15 +275,15 @@
     from pyecharts import options as opts
     from pyecharts.charts import Bar, Grid, Timeline
     import polars as pl
     import math
 
     # SampleSize = 100000
     # YVar = 'Daily Liters'
-    # GroupVar = 'Brand' # None 
+    # GroupVar = 'Brand' # None
     # FacetRows = 2
     # FacetCols = 2
     # FacetLevels = None
     # TimeLine = False
     # YVarTrans = None
     # XAxisTitle = YVar
     # XAxisNameLocation = 'middle'
@@ -8321,20 +8320,20 @@
 
     dt1 = dt.select(cols)
     if not PreAgg:
       dt1 = PolarsAggregation(dt1, AggMethod, NumericVariable = YVars, GroupVariable = GroupVar, DateVariable = DateVar)
 
     # Transformation
     if not YVarTrans is None:
-      if isinstance(YVar, list):
-        for i in range(len(YVar)):# i = 0
+      if isinstance(YVars, list):
+        for i in range(len(YVars)):# i = 0
           if not YVarTrans[i] is None:
-            dt1 = NumericTransformation(dt1, YVar[i], Trans = YVarTrans[i].lower())
+            dt1 = NumericTransformation(dt1, YVars[i], Trans = YVarTrans[i].lower())
       else:
-        dt1 = NumericTransformation(dt1, YVar, Trans = YVarTrans.lower())
+        dt1 = NumericTransformation(dt1, YVars, Trans = YVarTrans.lower())
 
     if isinstance(YVars, list):
       if len(YVars) > 1:
         x_data = YVars
         dt2 = dt1.melt(id_vars = DateVar, value_vars = YVars)
         dt2 = dt2.rename({"variable": "Series", "value": "Values"})
         DateVal = dt2[DateVar].to_list()
```

### Comparing `QuickEcharts-1.1.0/QuickEcharts.egg-info/PKG-INFO` & `QuickEcharts-1.1.1/QuickEcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickEcharts
-Version: 1.1.0
+Version: 1.1.1
 Summary: Create Echart plots in a single simple function call, with internal data wrangling via polars
 Home-page: https://github.com/AdrianAntico/QuickEcharts
 Author: ['Adrian Antico']
 Author-email: adrianantico@gmail.com
 License: AGPL >= 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `QuickEcharts-1.1.0/README.md` & `QuickEcharts-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `QuickEcharts-1.1.0/pyproject.toml` & `QuickEcharts-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `QuickEcharts-1.1.0/setup.py` & `QuickEcharts-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 with open(os.path.join(HERE, "requirements.txt")) as f:
     required = f.read().splitlines()
 
 setup(
     name="QuickEcharts",
-    version="1.1.0",
+    version="1.1.1",
     description="Create Echart plots in a single simple function call, with internal data wrangling via polars",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/AdrianAntico/QuickEcharts",
     author=["Adrian Antico"],
     author_email="adrianantico@gmail.com",
     license="AGPL >= 3",
```

