# Comparing `tmp/openhexa_toolbox-0.2.2.tar.gz` & `tmp/openhexa_toolbox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa_toolbox-0.2.2.tar", last modified: Mon May 13 08:57:20 2024, max compression
+gzip compressed data, was "openhexa_toolbox-0.2.3.tar", last modified: Mon May 27 14:32:57 2024, max compression
```

## Comparing `openhexa_toolbox-0.2.2.tar` & `openhexa_toolbox-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.187732 openhexa_toolbox-0.2.2/openhexa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.187732 openhexa_toolbox-0.2.2/openhexa/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.187732 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/periods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 08:57:20.000000 openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:57:20.191732 openhexa_toolbox-0.2.2/tests/dhis2/
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 08:56:56.000000 openhexa_toolbox-0.2.2/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.109577 openhexa_toolbox-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-27 14:32:57.105577 openhexa_toolbox-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.101577 openhexa_toolbox-0.2.3/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.105577 openhexa_toolbox-0.2.3/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.105577 openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36916 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.105577 openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.105577 openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-27 14:32:57.000000 openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 14:32:57.000000 openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:32:57.000000 openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-27 14:32:57.000000 openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-27 14:32:57.000000 openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:32:57.109577 openhexa_toolbox-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.105577 openhexa_toolbox-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:32:57.105577 openhexa_toolbox-0.2.3/tests/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/tests/dhis2/test_dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/tests/dhis2/test_dhis2_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 14:32:35.000000 openhexa_toolbox-0.2.3/tests/test_lib.py
```

### Comparing `openhexa_toolbox-0.2.2/LICENSE` & `openhexa_toolbox-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/PKG-INFO` & `openhexa_toolbox-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.2 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.3 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `openhexa_toolbox-0.2.2/README.md` & `openhexa_toolbox-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/api.py` & `openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/api.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/dhis2.py` & `openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/dhis2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import itertools
 import json
 import logging
 import os
 from functools import wraps
-from typing import Callable, List, Tuple, Union
+from typing import Callable, Iterator, List, Tuple, Union
 from urllib.parse import urlparse
 
 import pandas as pd
 import polars as pl
 from diskcache import Cache
 
 from .api import Api, DHIS2Connection, DHIS2Error
+from .periods import Period
 
 logger = logging.getLogger(__name__)
 
 
 def use_cache(key: str, expire_time=86400):
     """Use sqlite-based diskcache.
 
@@ -507,15 +508,15 @@
         )
 
         if src_format == "pandas":
             df = df.to_pandas()
         return df
 
 
-def _split_list(src_list: list, length: int) -> List[list]:
+def _split_list(src_list: list, length: int) -> Iterator[List]:
     """Split list into chunks."""
     for i in range(0, len(src_list), length):
         yield src_list[i : i + length]
 
 
 class DataValueSets:
     def __init__(self, client: DHIS2):
@@ -555,15 +556,15 @@
         return chunks
 
     def get(
         self,
         data_elements: List[str] = None,
         datasets: List[str] = None,
         data_element_groups: List[str] = None,
-        periods: List[str] = None,
+        periods: List[Union[str, Period]] = None,
         start_date: str = None,
         end_date: str = None,
         org_units: List[str] = None,
         org_unit_groups: List[str] = None,
         children: bool = False,
         attribute_option_combos: List[str] = None,
         last_updated: str = None,
@@ -575,15 +576,15 @@
         ----------
         data_elements : list of str, optional
             Data element identifiers (requires DHIS2 >= 2.39)
         datasets : str, optional
             Dataset identifiers
         data_element_groups : str, optional
             Data element groups identifiers
-        periods : list of str, optional
+        periods : list of str or Period, optional
             Period identifiers in ISO format
         start_date : str, optional
             Start date for the time span of the values to export
         end_date : str, optional
             End date for the time span of the values to export
         org_units : list of str, optional
             Organisation units identifiers
@@ -614,14 +615,21 @@
             raise DHIS2Error("No spatial dimension provided")
         if not when:
             raise DHIS2Error("No temporal dimension provided")
 
         if data_elements and not self.client.version >= "2.39":
             raise DHIS2Error("Data elements parameter not supported for DHIS2 versions < 2.39")
 
+        if periods:
+            if all([isinstance(pe, Period) for pe in periods]):
+                # convert Period objects to ISO strings
+                periods = [str(pe) for pe in periods]
+            elif not all([isinstance(pe, str) for pe in periods]):
+                raise ValueError("Mixed period types")
+
         params = {
             "dataElement": data_elements,
             "dataSet": datasets,
             "dataElementGroup": data_element_groups,
             "period": periods,
             "startDate": start_date,
             "endDate": end_date,
@@ -633,15 +641,17 @@
             "last_updated_duration": last_updated_duration,
         }
 
         chunks = self.split_params(params)
         response = []
         for chunk in chunks:
             r = self.client.api.get("dataValueSets", params=chunk)
-            response += r.json()["dataValues"]
+            r_json = r.json()
+            if "dataValues" in r_json:
+                response += r.json()["dataValues"]
 
         return response
 
     def _validate(self, data_values: List[dict]):
         """Validate data values based on data element value type.
 
         Supported: NUMBER, INTEGER, UNIT_INTERVAL, PERCENTAGE, INTEGER_POSITIVE,
@@ -959,15 +969,15 @@
 
     def get(
         self,
         data_elements: List[str] = None,
         data_element_groups: List[str] = None,
         indicators: List[str] = None,
         indicator_groups: List[str] = None,
-        periods: List[str] = None,
+        periods: Union[str, Period] = None,
         org_units: List[str] = None,
         org_unit_groups: List[str] = None,
         org_unit_levels: List[int] = None,
         include_cocs: bool = True,
     ) -> List[dict]:
         """Get requested data values using the Analytics API endpoint.
 
@@ -981,15 +991,15 @@
             Data element identifiers
         data_element_groups : str, optional
             Data element groups identifiers
         indicators : list of str, optional
             Indicator identifiers
         indicator_groups : list of str, optional
             Indicator groups indifiers
-        periods : list of str, optional
+        periods : list of str or Period, optional
             Period identifiers in ISO format
         org_units : list of str, optional
             Organisation units identifiers
         org_unit_groups : list of str, optional
             Organisation unit groups identifiers
         org_unit_levels : list of int, optional
             Organisation unit levels
@@ -1007,14 +1017,20 @@
         if not what:
             raise DHIS2Error("No data dimension provided")
         if not where:
             raise DHIS2Error("No spatial dimension provided")
         if not when:
             raise DHIS2Error("No temporal dimension provided")
 
+        if all([isinstance(pe, Period) for pe in periods]):
+            # convert Period objects to ISO strings
+            periods = [str(pe) for pe in periods]
+        elif not all([isinstance(pe, str) for pe in periods]):
+            raise ValueError("Mixed period types")
+
         dimension = self.format_dimension_param(
             data_elements=data_elements,
             data_element_groups=data_element_groups,
             indicators=indicators,
             indicator_groups=indicator_groups,
             periods=periods,
             org_units=org_units,
```

### Comparing `openhexa_toolbox-0.2.2/openhexa/toolbox/dhis2/periods.py` & `openhexa_toolbox-0.2.3/openhexa/toolbox/dhis2/periods.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/api.py` & `openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/api.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/parse.py` & `openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/parse.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/openhexa/toolbox/kobo/utils.py` & `openhexa_toolbox-0.2.3/openhexa/toolbox/kobo/utils.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.2.2
+Version: 0.2.3
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.2 Summary: A set of
+Metadata-Version: 2.1 Name: openhexa.toolbox Version: 0.2.3 Summary: A set of
 tools to acquire & process data from various sources Author-email: Bluesquare
 bluesquarehub.com> Maintainer-email: Bluesquare
 bluesquarehub.com> License: MIT License Copyright (c) 2023 Bluesquare
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `openhexa_toolbox-0.2.2/openhexa.toolbox.egg-info/SOURCES.txt` & `openhexa_toolbox-0.2.3/openhexa.toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/pyproject.toml` & `openhexa_toolbox-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openhexa.toolbox"
-version = "0.2.2"
+version = "0.2.3"
 description = "A set of tools to acquire & process data from various sources"
 authors = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
 maintainers = [{ name = "Bluesquare", email = "dev@bluesquarehub.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2.py` & `openhexa_toolbox-0.2.3/tests/dhis2/test_dhis2.py`

 * *Files identical despite different names*

### Comparing `openhexa_toolbox-0.2.2/tests/dhis2/test_dhis2_periods.py` & `openhexa_toolbox-0.2.3/tests/dhis2/test_dhis2_periods.py`

 * *Files identical despite different names*

