# Comparing `tmp/weightfactors-0.0.3.tar.gz` & `tmp/weightfactors-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weightfactors-0.0.3.tar", max compression
+gzip compressed data, was "weightfactors-0.0.4.tar", max compression
```

## Comparing `weightfactors-0.0.3.tar` & `weightfactors-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2024-02-14 09:09:55.954071 weightfactors-0.0.3/LICENSE
--rw-r--r--   0        0        0      606 2024-05-06 07:47:28.888804 weightfactors-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1958 2024-05-06 07:47:28.886680 weightfactors-0.0.3/README.md
--rw-r--r--   0        0        0       92 2024-02-14 09:05:58.768979 weightfactors-0.0.3/weightfactors/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 09:05:58.769061 weightfactors-0.0.3/weightfactors/raking/__init__.py
--rw-r--r--   0        0        0    12804 2024-05-06 07:47:28.893080 weightfactors-0.0.3/weightfactors/raking/generalized_raker.py
--rw-r--r--   0        0        0        0 2024-02-14 09:38:04.963250 weightfactors-0.0.3/weightfactors/utils/__init__.py
--rw-r--r--   0        0        0      275 2024-02-14 09:05:58.774255 weightfactors-0.0.3/weightfactors/utils/exceptions.py
--rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 weightfactors-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-27 07:56:12.198870 weightfactors-0.0.4/LICENSE
+-rw-r--r--   0        0        0      606 2024-05-27 08:19:48.599802 weightfactors-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1958 2024-05-27 07:56:12.198870 weightfactors-0.0.4/README.md
+-rw-r--r--   0        0        0       92 2024-05-27 07:56:12.201933 weightfactors-0.0.4/weightfactors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:56:12.201933 weightfactors-0.0.4/weightfactors/raking/__init__.py
+-rw-r--r--   0        0        0    12954 2024-05-27 08:16:07.532158 weightfactors-0.0.4/weightfactors/raking/generalized_raker.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:56:12.201933 weightfactors-0.0.4/weightfactors/utils/__init__.py
+-rw-r--r--   0        0        0      275 2024-05-27 07:56:12.201933 weightfactors-0.0.4/weightfactors/utils/exceptions.py
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 weightfactors-0.0.4/PKG-INFO
```

### Comparing `weightfactors-0.0.3/LICENSE` & `weightfactors-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `weightfactors-0.0.3/pyproject.toml` & `weightfactors-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weightfactors"
-version = "0.0.3"
+version = "0.0.4"
 description = "Calculate weight factors for survey data to approximate a representative sample"
 authors = ["DemianvG <d.vangils@markteffect.nl>"]
 readme = "README.md"
 packages = [{include = "weightfactors"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `weightfactors-0.0.3/README.md` & `weightfactors-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `weightfactors-0.0.3/weightfactors/raking/generalized_raker.py` & `weightfactors-0.0.4/weightfactors/raking/generalized_raker.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,26 @@
             if key not in data.columns:
                 raise KeyError(f"There is no column {key} in the provided dataset")
             # Make sure there are no missing values in the columns used for calculating weights
             if data[key].isna().any(axis=None):
                 raise ValueError(f"Column {key} contains missing values")
             # Make sure all unique values in the target columns have been mapped
             # It is impossible to set values with observations to a weight of 0
-            if len(data[key].unique()) != len(value):
-                raise KeyError(
-                    f"There are observations for a value in '{key}' that has not been mapped to a population target"
-                )
+            for k in list(data[key].unique()):
+                if k not in list(value.keys()):
+                    raise KeyError(
+                        f"There are observations for a value in '{key}' that has not been mapped to a population target"
+                    )
             # Make sure we have at least 1 observation for each category
-            # It is impossible to set values without observations to a weight larger than 1
-            for k, _ in value.items():
-                if k not in data[key].unique():
-                    raise KeyError(f"There are no observations for {k} in column {key}")
+            # It is impossible to set values without observations to a weight larger than 0
+            for k, v in value.items():
+                if k not in data[key].unique() and v > 0:
+                    raise KeyError(
+                        f"There are no observations for {k} in column {key}, but a population target has been set"
+                    )
             # Make sure the inclusion column is valid
             if self.exclusion_column:
                 if self.exclusion_column not in data.columns:
                     raise KeyError(f"There is no column {key} in the provided dataset")
                 unique_values = set(data[self.exclusion_column])
                 if not len(unique_values) == 2 or not (
                     0 in unique_values and 1 in unique_values
```

### Comparing `weightfactors-0.0.3/PKG-INFO` & `weightfactors-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weightfactors
-Version: 0.0.3
+Version: 0.0.4
 Summary: Calculate weight factors for survey data to approximate a representative sample
 Author: DemianvG
 Author-email: d.vangils@markteffect.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

