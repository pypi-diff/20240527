# Comparing `tmp/texase-0.2.0.tar.gz` & `tmp/texase-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texase-0.2.0.tar", max compression
+gzip compressed data, was "texase-0.2.1.tar", max compression
```

## Comparing `texase-0.2.0.tar` & `texase-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    16725 2024-05-01 19:37:53.728919 texase-0.2.0/LICENSE
--rw-r--r--   0        0        0     2937 2024-05-01 19:37:53.728919 texase-0.2.0/README.md
--rw-r--r--   0        0        0      742 2024-05-01 19:37:53.740919 texase-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/__init__.py
--rw-r--r--   0        0        0     2320 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/addcolumn.py
--rw-r--r--   0        0        0    21660 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/app.py
--rw-r--r--   0        0        0    30660 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/data.py
--rw-r--r--   0        0        0    11362 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/details.py
--rw-r--r--   0        0        0     1951 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/edit.py
--rw-r--r--   0        0        0     4681 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/files_io.py
--rw-r--r--   0        0        0     8166 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/filter.py
--rw-r--r--   0        0        0     6056 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/formatting.py
--rw-r--r--   0        0        0     2982 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/help.py
--rw-r--r--   0        0        0     4629 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/input_screens.py
--rw-r--r--   0        0        0     1515 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/keys.py
--rw-r--r--   0        0        0     1153 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/saved_columns.py
--rw-r--r--   0        0        0     2950 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/search.py
--rw-r--r--   0        0        0    15826 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/table.py
--rw-r--r--   0        0        0     2062 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/texase.tcss
--rw-r--r--   0        0        0     1243 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/validators.py
--rw-r--r--   0        0        0     1122 2024-05-01 19:37:53.740919 texase-0.2.0/src/texase/yesno.py
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 texase-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-05-27 12:11:01.186810 texase-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3148 2024-05-27 12:11:01.186810 texase-0.2.1/README.md
+-rw-r--r--   0        0        0      742 2024-05-27 12:11:01.198810 texase-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 12:11:01.198810 texase-0.2.1/src/texase/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-27 12:11:01.198810 texase-0.2.1/src/texase/addcolumn.py
+-rw-r--r--   0        0        0    21660 2024-05-27 12:11:01.198810 texase-0.2.1/src/texase/app.py
+-rw-r--r--   0        0        0    31405 2024-05-27 12:11:01.198810 texase-0.2.1/src/texase/data.py
+-rw-r--r--   0        0        0    11362 2024-05-27 12:11:01.198810 texase-0.2.1/src/texase/details.py
+-rw-r--r--   0        0        0     1951 2024-05-27 12:11:01.198810 texase-0.2.1/src/texase/edit.py
+-rw-r--r--   0        0        0     4681 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/files_io.py
+-rw-r--r--   0        0        0     8166 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/filter.py
+-rw-r--r--   0        0        0     6239 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/formatting.py
+-rw-r--r--   0        0        0     2982 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/help.py
+-rw-r--r--   0        0        0     4629 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/input_screens.py
+-rw-r--r--   0        0        0     1515 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/keys.py
+-rw-r--r--   0        0        0     1153 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/saved_columns.py
+-rw-r--r--   0        0        0     2950 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/search.py
+-rw-r--r--   0        0        0    15826 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/table.py
+-rw-r--r--   0        0        0     2062 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/texase.tcss
+-rw-r--r--   0        0        0     1243 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/validators.py
+-rw-r--r--   0        0        0     1122 2024-05-27 12:11:01.202810 texase-0.2.1/src/texase/yesno.py
+-rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 texase-0.2.1/PKG-INFO
```

### Comparing `texase-0.2.0/LICENSE` & `texase-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/README.md` & `texase-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,36 @@
 
 > Texase is a TUI[^1] for [ASE](https://wiki.fysik.dtu.dk/ase/) databases. It allows you to quickly get an overview and navigate an ASE database.
 
 [^1]: Textual User Interface (Also known as a Terminal/Text User Interface)
 
 > Built with [Textual](https://textual.textualize.io/)
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
+![PyPI - Version](https://img.shields.io/pypi/v/texase)
+[![MPL License](https://img.shields.io/badge/License-MPL-green.svg)](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/texase)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/steenlysgaard/texase/python-package.yml)
+
 <!-- [![][versions-image]][versions-url] -->
 
 
 ![Demo](demo.gif)
 
 <!-- ## Screenshots -->
 
 <!-- ![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here) -->
 
 
-<!-- ## Installation -->
+## Installation
 
-<!-- Install texase with pip -->
+Install texase with pip
 
-<!-- ```bash -->
-<!--   pip install texase -->
-<!-- ``` -->
+```bash
+pip install texase
+```
 
 ## Usage
 
 After installation do `texase file.db` where `file.db` is your ASE database.
 
 - Press __`?`__ to view all keybindings
 
@@ -77,13 +81,13 @@
 
 Now I can just do `texase file.db` and navigate with single key presses.
 
 
 
 ## License
 
-[MIT](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
+[MPL](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
 
 
 <!-- ## Badges -->
 
 <!-- Add badges from somewhere like: [shields.io](https://shields.io/) -->
```

### Comparing `texase-0.2.0/pyproject.toml` & `texase-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "texase"
-version = "0.2.0"
+version = "0.2.1"
 description = "Textual user interface for ASE db."
 authors = ["Steen Lysgaard <stly@dtu.dk>"]
 license = "MPL"
 readme = "README.md"
 packages = [{include = "texase", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `texase-0.2.0/src/texase/addcolumn.py` & `texase-0.2.1/src/texase/addcolumn.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/app.py` & `texase-0.2.1/src/texase/app.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/data.py` & `texase-0.2.1/src/texase/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 import pandas as pd
 from ase import Atoms
 from ase.db import connect
 from ase.db.table import all_columns
 from ase.io import read, write
 from textual.cache import LRUCache
 
-from texase.formatting import format_column, get_age_string, pbc_str_to_array
+from texase.formatting import (
+    convert_str_to_bool,
+    format_column,
+    get_age_string,
+    pbc_str_to_array,
+)
 from texase.saved_columns import SavedColumns
 
 ops = {
     "==": operator.eq,
     "!=": operator.ne,
     "<": operator.lt,
     ">": operator.gt,
@@ -36,14 +41,15 @@
     return x
 
 
 ALL_COLUMNS = list(all_columns) + ["modified"]
 COLUMN_DTYPES = {
     "id": "int",
     "age": "float",
+    "modified": "float",
     "user": pd.StringDtype(),
     "formula": pd.StringDtype(),
     "calculator": pd.StringDtype(),
     "energy": "float",
     "natoms": "int",
     "fmax": "float",
     "pbc": pd.StringDtype(),
@@ -57,21 +63,24 @@
 
 def get_default_columns():
     """Return default columns used in ASE db and here, i.e. don't show
     modified by default."""
     return list(all_columns)
 
 
-operator_type_conversion = {
-    "<": float,
-    "<=": float,
-    "==": nothing,
-    ">=": float,
-    ">": float,
-    "!=": nothing,
+dtype_type_conversion = {
+    pd.Int64Dtype(): int,
+    pd.BooleanDtype(): convert_str_to_bool,
+    pd.StringDtype(): str,
+    np.dtype("int"): int,
+    np.dtype("float"): float,
+    np.dtype("object"): nothing,
+    "int": int,
+    "object": nothing,
+    "float": float,
 }
 
 
 def cache(f):
     @wraps(f)
     def wrapper(self, *args, **kwds):
         cache_key = tuple(args)
@@ -466,15 +475,15 @@
             mask &= self._filter_mask(filter)
         return mask
 
     @cache
     def _filter_mask(self, filter: tuple) -> np.ndarray:
         """Returns a boolean array of indices that pass the filter"""
         filter_key, op, filter_value = filter
-        mask = ops[op](self.df[filter_key], operator_type_conversion[op](filter_value))
+        mask = get_mask(self.df[filter_key], op, filter_value)
         return mask.to_numpy()
 
     def add_filter(self, key, operator, value) -> None:
         # We get the value as a string. Maybe we should convert it to
         # the correct type if the column values are not strings? But
         # how do we know? We try to deduce from the operator
 
@@ -843,7 +852,21 @@
         return True
     incompatible_types = ["float", pd.BooleanDtype(), pd.StringDtype(), pd.Int64Dtype()]
     # Test all combinations of size 2 of incompatible types
     for a, b in combinations(incompatible_types, 2):
         if a in types and b in types:
             return False
     raise ValueError(f"Unknown dtype: {dtype1} or {dtype2}")
+
+
+def get_mask(series: pd.Series, op: str, value: str):
+    """Get a mask for a pd.Series based on an operation and a value.
+
+    The operator != (not equal to) is the only operator that returns
+    True if the result is NA. For example, [NA, "apple", "banana"] !=
+    "apple" returns [True, False, True]. This is because the NA value
+    is not equal to "apple".
+
+    """
+    if op == "!=":
+        return ops[op](series, dtype_type_conversion[series.dtype](value)).fillna(True)
+    return ops[op](series, dtype_type_conversion[series.dtype](value)).fillna(False)
```

### Comparing `texase-0.2.0/src/texase/details.py` & `texase-0.2.1/src/texase/details.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/edit.py` & `texase-0.2.1/src/texase/edit.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/files_io.py` & `texase-0.2.1/src/texase/files_io.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/filter.py` & `texase-0.2.1/src/texase/filter.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/formatting.py` & `texase-0.2.1/src/texase/formatting.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,23 @@
     """
     try:
         return int(value)
     except ValueError:
         try:
             value = float(value)
         except ValueError:
-            value = {"true": True, "false": False}.get(value.lower(), value)
+            value = convert_str_to_bool(value)
         return value
 
 
+def convert_str_to_bool(str_value: str) -> bool | str:
+    """Convert string to bool if possible. Otherwise return the value as is."""
+    return {"true": True, "false": False}.get(str_value.lower(), str_value)
+
+
 def convert_str_to_other_type(str_value: str) -> Any:
     """Convert string to dict, list or np.ndarray if possible. Otherwise return the value as is."""
     try:
         return ast.literal_eval(str_value)
     except (SyntaxError, ValueError):
         # Maybe this is a numpy array
         if is_numpy_array(str_value):
```

### Comparing `texase-0.2.0/src/texase/help.py` & `texase-0.2.1/src/texase/help.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/input_screens.py` & `texase-0.2.1/src/texase/input_screens.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/keys.py` & `texase-0.2.1/src/texase/keys.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/saved_columns.py` & `texase-0.2.1/src/texase/saved_columns.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/search.py` & `texase-0.2.1/src/texase/search.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/table.py` & `texase-0.2.1/src/texase/table.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/texase.tcss` & `texase-0.2.1/src/texase/texase.tcss`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/validators.py` & `texase-0.2.1/src/texase/validators.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/src/texase/yesno.py` & `texase-0.2.1/src/texase/yesno.py`

 * *Files identical despite different names*

### Comparing `texase-0.2.0/PKG-INFO` & `texase-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texase
-Version: 0.2.0
+Version: 0.2.1
 Summary: Textual user interface for ASE db.
 License: MPL
 Author: Steen Lysgaard
 Author-email: stly@dtu.dk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -24,32 +24,36 @@
 
 > Texase is a TUI[^1] for [ASE](https://wiki.fysik.dtu.dk/ase/) databases. It allows you to quickly get an overview and navigate an ASE database.
 
 [^1]: Textual User Interface (Also known as a Terminal/Text User Interface)
 
 > Built with [Textual](https://textual.textualize.io/)
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
+![PyPI - Version](https://img.shields.io/pypi/v/texase)
+[![MPL License](https://img.shields.io/badge/License-MPL-green.svg)](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/texase)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/steenlysgaard/texase/python-package.yml)
+
 <!-- [![][versions-image]][versions-url] -->
 
 
 ![Demo](demo.gif)
 
 <!-- ## Screenshots -->
 
 <!-- ![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here) -->
 
 
-<!-- ## Installation -->
+## Installation
 
-<!-- Install texase with pip -->
+Install texase with pip
 
-<!-- ```bash -->
-<!--   pip install texase -->
-<!-- ``` -->
+```bash
+pip install texase
+```
 
 ## Usage
 
 After installation do `texase file.db` where `file.db` is your ASE database.
 
 - Press __`?`__ to view all keybindings
 
@@ -98,14 +102,14 @@
 
 Now I can just do `texase file.db` and navigate with single key presses.
 
 
 
 ## License
 
-[MIT](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
+[MPL](https://github.com/steenlysgaard/texase/blob/main/LICENSE)
 
 
 <!-- ## Badges -->
 
 <!-- Add badges from somewhere like: [shields.io](https://shields.io/) -->
```

