# Comparing `tmp/openeo_pg_parser_networkx-2024.4.0.tar.gz` & `tmp/openeo_pg_parser_networkx-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_pg_parser_networkx-2024.4.0.tar", max compression
+gzip compressed data, was "openeo_pg_parser_networkx-2024.5.0.tar", max compression
```

## Comparing `openeo_pg_parser_networkx-2024.4.0.tar` & `openeo_pg_parser_networkx-2024.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10765 2024-04-16 13:48:34.049644 openeo_pg_parser_networkx-2024.4.0/LICENSE
--rw-r--r--   0        0        0     5886 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/README.md
--rw-r--r--   0        0        0      241 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/__init__.py
--rw-r--r--   0        0        0    19598 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/graph.py
--rw-r--r--   0        0        0    10036 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/pg_schema.py
--rw-r--r--   0        0        0     5125 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/process_registry.py
--rw-r--r--   0        0        0    11644 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/resolving_utils.py
--rw-r--r--   0        0        0    10738 2024-04-16 13:48:34.053644 openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/utils.py
--rw-r--r--   0        0        0     1590 2024-04-16 13:48:34.057644 openeo_pg_parser_networkx-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0     7170 1970-01-01 00:00:00.000000 openeo_pg_parser_networkx-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10765 2024-05-27 13:57:35.950908 openeo_pg_parser_networkx-2024.5.0/LICENSE
+-rw-r--r--   0        0        0     5886 2024-05-27 13:57:35.950908 openeo_pg_parser_networkx-2024.5.0/README.md
+-rw-r--r--   0        0        0      241 2024-05-27 13:57:35.954908 openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/__init__.py
+-rw-r--r--   0        0        0    19688 2024-05-27 13:57:35.954908 openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/graph.py
+-rw-r--r--   0        0        0    10174 2024-05-27 13:57:35.954908 openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/pg_schema.py
+-rw-r--r--   0        0        0     5125 2024-05-27 13:57:35.954908 openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/process_registry.py
+-rw-r--r--   0        0        0    11644 2024-05-27 13:57:35.954908 openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/resolving_utils.py
+-rw-r--r--   0        0        0    10708 2024-05-27 13:57:35.954908 openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/utils.py
+-rw-r--r--   0        0        0     1590 2024-05-27 13:57:35.954908 openeo_pg_parser_networkx-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7170 1970-01-01 00:00:00.000000 openeo_pg_parser_networkx-2024.5.0/PKG-INFO
```

### Comparing `openeo_pg_parser_networkx-2024.4.0/LICENSE` & `openeo_pg_parser_networkx-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.4.0/README.md` & `openeo_pg_parser_networkx-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/graph.py` & `openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from __future__ import annotations
 
+import sys
+
+sys.setrecursionlimit(16385)  # Necessary when parsing really big graphs
 import functools
 import json
 import logging
 import random
 from collections import namedtuple
 from dataclasses import dataclass, field
 from functools import partial
@@ -106,15 +109,15 @@
 
     @staticmethod
     def _parse_datamodel(nested_graph: dict) -> ProcessGraph:
         """
         Parses a nested process graph into the Pydantic datamodel for ProcessGraph.
         """
 
-        return ProcessGraph.parse_obj(nested_graph)
+        return ProcessGraph.model_validate(nested_graph)
 
     def _parse_process_graph(self, process_graph: ProcessGraph, arg_name: str = None):
         """
         Start recursively walking a process graph from its result node and parse its information into self.G.
         This step passes process_graph.uid to make sure that each process graph operates within its own namespace so that nodes are unique.
         """
```

### Comparing `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/pg_schema.py` & `openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/pg_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import datetime
 import json
 import logging
 from enum import Enum
 from re import match
-from typing import Any, Optional, Union
+from typing import Annotated, Any, List, Optional, Union
 from uuid import UUID, uuid4
 
 import numpy as np
 import pendulum
 import pyproj
 from geojson_pydantic import (
     Feature,
@@ -18,17 +18,21 @@
     MultiPolygon,
     Polygon,
 )
 from pydantic import (
     BaseModel,
     Extra,
     Field,
+    RootModel,
+    StringConstraints,
     ValidationError,
     conlist,
     constr,
+    field_validator,
+    model_validator,
     validator,
 )
 from shapely.geometry import Polygon
 
 logger = logging.getLogger(__name__)
 
 # TODO: Move this to a proper settings object for this repo and use in tests, possibly using pydantic settings: https://pydantic-docs.helpmanual.io/usage/settings/
@@ -61,21 +65,22 @@
 
 
 class ParameterReference(BaseModel, extra=Extra.forbid):
     from_parameter: str
 
 
 class ProcessNode(BaseModel, arbitrary_types_allowed=True):
-    process_id: constr(regex=r'^\w+$')
+    process_id: Annotated[str, StringConstraints(pattern=r'^\w+$')]
+
     namespace: Optional[Optional[str]] = None
     result: Optional[bool] = False
     description: Optional[Optional[str]] = None
     arguments: dict[
         str,
-        Optional[
+        Annotated[
             Union[
                 ResultReference,
                 ParameterReference,
                 ProcessGraph,
                 BoundingBox,
                 JobId,
                 Year,
@@ -83,19 +88,20 @@
                 DateTime,
                 Duration,
                 TemporalInterval,
                 TemporalIntervals,
                 # GeoJson, disable while https://github.com/developmentseed/geojson-pydantic/issues/92 is open
                 Time,
                 float,
-                str,
                 bool,
                 list,
                 dict,
-            ]
+                str,
+            ],
+            Field(union_mode='left_to_right'),
         ],
     ]
 
     def __str__(self):
         return json.dumps(self.dict(), indent=4)
 
 
@@ -129,17 +135,17 @@
 
 
 class BoundingBox(BaseModel, arbitrary_types_allowed=True):
     west: float
     east: float
     north: float
     south: float
-    base: Optional[float]
-    height: Optional[float]
-    crs: Optional[Union[str, int]]
+    base: Optional[float] = None
+    height: Optional[float] = None
+    crs: Optional[Union[str, int]] = None
 
     # validators
     _parse_crs: classmethod = crs_validator('crs')
 
     @property
     def polygon(self) -> Polygon:
         """"""
@@ -149,199 +155,205 @@
                 (self.west, self.north),
                 (self.east, self.north),
                 (self.east, self.south),
             ]
         )
 
 
-class Date(BaseModel):
-    __root__: datetime.datetime
+class Date(RootModel):
+    root: datetime.datetime
 
-    @validator("__root__", pre=True)
+    @field_validator("root", mode="before")
     def validate_time(cls, value: Any) -> Any:
         if (
             isinstance(value, str)
             and len(value) <= 11
             and match(r"[0-9]{4}[-/][0-9]{2}[-/][0-9]{2}T?", value)
         ):
             return pendulum.parse(value)
-        raise ValidationError("Could not parse `Date` from input.")
+        raise ValueError("Could not parse `Date` from input.")
 
     def to_numpy(self):
-        return np.datetime64(self.__root__)
+        return np.datetime64(self.root)
 
     def __repr__(self):
-        return self.__root__.__repr__()
+        return self.root.__repr__()
+
+    def __gt__(self, date1):
+        return self.root > date1.root
 
 
-class DateTime(BaseModel):
-    __root__: datetime.datetime
+class DateTime(RootModel):
+    root: datetime.datetime
 
-    @validator("__root__", pre=True)
+    @field_validator("root", mode="before")
     def validate_time(cls, value: Any) -> Any:
         if isinstance(value, str) and match(
             r"[0-9]{4}-[0-9]{2}-[0-9]{2}T?[0-9]{2}:[0-9]{2}:?([0-9]{2})?Z?", value
         ):
             return pendulum.parse(value)
-        raise ValidationError("Could not parse `DateTime` from input.")
+        raise ValueError("Could not parse `DateTime` from input.")
 
     def to_numpy(self):
-        return np.datetime64(self.__root__)
+        return np.datetime64(self.root)
 
     def __repr__(self):
-        return self.__root__.__repr__()
+        return self.root.__repr__()
+
+    def __gt__(self, date1):
+        return self.root > date1.root
 
 
-class Time(BaseModel):
-    __root__: pendulum.Time
+class Time(RootModel):
+    root: datetime.time
 
-    @validator("__root__", pre=True)
+    @field_validator("root", mode="before")
     def validate_time(cls, value: Any) -> Any:
         if (
             isinstance(value, str)
             and len(value) >= 5
             and len(value) <= 9
             and match(r"[0-9]{2}:[0-9]{2}:?([0-9]{2})?Z?", value)
         ):
             return pendulum.parse(value).time()
-        raise ValidationError("Could not parse `Time` from input.")
+        raise ValueError("Could not parse `Time` from input.")
 
     def to_numpy(self):
         raise NotImplementedError
 
     def __repr__(self):
-        return self.__root__.__repr__()
+        return self.time.__repr__()
 
 
-class Year(BaseModel):
-    __root__: datetime.datetime
+class Year(RootModel):
+    root: datetime.datetime
 
-    @validator("__root__", pre=True)
+    @field_validator("root", mode="before")
     def validate_time(cls, value: Any) -> Any:
         if isinstance(value, str) and len(value) <= 4 and match(r"^\d{4}$", value):
             return pendulum.parse(value)
-        raise ValidationError("Could not parse `Year` from input.")
+        raise ValueError("Could not parse `Year` from input.")
 
     def to_numpy(self):
-        return np.datetime64(self.__root__)
+        return np.datetime64(self.root)
 
     def __repr__(self):
-        return self.__root__.__repr__()
+        return self.root.__repr__()
 
 
-class Duration(BaseModel):
-    __root__: datetime.timedelta
+class Duration(RootModel):
+    root: datetime.timedelta
 
-    @validator("__root__", pre=True)
+    @field_validator("root", mode="before")
     def validate_time(cls, value: Any) -> Any:
         if isinstance(value, str) and match(
             r"P[0-9]*Y?[0-9]*M?[0-9]*D?T?[0-9]*H?[0-9]*M?[0-9]*S?", value
         ):
             return pendulum.parse(value).as_timedelta()
-        raise ValidationError("Could not parse `Duration` from input.")
+        raise ValueError("Could not parse `Duration` from input.")
 
     def to_numpy(self):
-        return np.timedelta64(self.__root__)
+        return np.timedelta64(self.root)
 
     def __repr__(self):
-        return self.__root__.__repr__()
+        return self.root.__repr__()
 
 
-class TemporalInterval(BaseModel):
-    __root__: conlist(Union[Year, Date, DateTime, Time, None], min_items=2, max_items=2)
+class TemporalInterval(RootModel):
+    root: conlist(Union[Year, Date, DateTime, Time, None], min_length=2, max_length=2)
 
-    @validator("__root__")
+    @field_validator("root")
     def validate_temporal_interval(cls, value: Any) -> Any:
         start = value[0]
         end = value[1]
 
         if start is None and end is None:
-            raise ValidationError("Could not parse `TemporalInterval` from input.")
+            raise ValueError("Could not parse `TemporalInterval` from input.")
 
         # Disambiguate the Time subtype
         if isinstance(start, Time) or isinstance(end, Time):
             if isinstance(start, Time) and isinstance(end, Time):
-                raise ValidationError(
+                raise ValueError(
                     "Ambiguous TemporalInterval, both start and end are of type `Time`"
                 )
             if isinstance(start, Time):
                 if end is None:
-                    raise ValidationError(
+                    raise ValueError(
                         "Cannot disambiguate TemporalInterval, start is `Time` and end is `None`"
                     )
                 logger.warning(
                     "Start time of temporal interval is of type `time`. Assuming same date as the end time."
                 )
                 start = DateTime(
-                    __root__=pendulum.datetime(
-                        end.__root__.year,
-                        end.__root__.month,
-                        end.__root__.day,
-                        start.__root__.hour,
-                        start.__root__.minute,
-                        start.__root__.second,
-                        start.__root__.microsecond,
+                    root=pendulum.datetime(
+                        end.root.year,
+                        end.root.month,
+                        end.root.day,
+                        start.root.hour,
+                        start.root.minute,
+                        start.root.second,
+                        start.root.microsecond,
                     ).to_rfc3339_string()
                 )
             elif isinstance(end, Time):
                 if start is None:
-                    raise ValidationError(
+                    raise ValueError(
                         "Cannot disambiguate TemporalInterval, start is `None` and end is `Time`"
                     )
                 logger.warning(
                     "End time of temporal interval is of type `time`. Assuming same date as the start time."
                 )
                 end = DateTime(
-                    __root__=pendulum.datetime(
-                        start.__root__.year,
-                        start.__root__.month,
-                        start.__root__.day,
-                        end.__root__.hour,
-                        end.__root__.minute,
-                        end.__root__.second,
-                        end.__root__.microsecond,
+                    root=pendulum.datetime(
+                        start.root.year,
+                        start.root.month,
+                        start.root.day,
+                        end.root.hour,
+                        end.root.minute,
+                        end.root.second,
+                        end.root.microsecond,
                     ).to_rfc3339_string()
                 )
 
-        if not (start is None or end is None) and start.__root__ > end.__root__:
-            raise ValidationError("Start time > end time")
+        if not (start is None or end is None) and start > end:
+            raise ValueError("Start time > end time")
 
         return [start, end]
 
     @property
     def start(self):
-        return self.__root__[0]
+        return self.root[0]
 
     @property
     def end(self):
-        return self.__root__[1]
+        return self.root[1]
 
     def __iter__(self):
-        return iter(self.__root__)
+        return iter(self.root)
 
     def __getitem__(self, item):
-        return self.__root__[item]
+        return self.root[item]
 
 
-class TemporalIntervals(BaseModel):
-    __root__: list[TemporalInterval]
+class TemporalIntervals(RootModel):
+    root: list[TemporalInterval]
 
     def __iter__(self):
-        return iter(self.__root__)
+        return iter(self.root)
 
     def __getitem__(self, item) -> TemporalInterval:
-        return self.__root__[item]
+        return self.root[item]
 
 
 GeoJson = Union[FeatureCollection, Feature, GeometryCollection, MultiPolygon, Polygon]
 # The GeoJson spec (https://www.rfc-editor.org/rfc/rfc7946.html#ref-GJ2008) doesn't
 # have a crs field anymore and recommends assuming it to be EPSG:4326, so we do the same.
 
 
-class JobId(BaseModel):
-    __root__: str = Field(
-        regex=r"(eodc-jb-|jb-)[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}"
+class JobId(RootModel):
+    root: str = Field(
+        pattern=r"(eodc-jb-|jb-)[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}"
     )
 
 
-ResultReference.update_forward_refs()
-ProcessNode.update_forward_refs()
+ResultReference.model_rebuild()
+ProcessNode.model_rebuild()
```

### Comparing `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/process_registry.py` & `openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/process_registry.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/resolving_utils.py` & `openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/resolving_utils.py`

 * *Files identical despite different names*

### Comparing `openeo_pg_parser_networkx-2024.4.0/openeo_pg_parser_networkx/utils.py` & `openeo_pg_parser_networkx-2024.5.0/openeo_pg_parser_networkx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 from openeo_pg_parser_networkx.pg_schema import ParameterReference, ResultReference
 
 
 def parse_nested_parameter(parameter: Any):
     try:
         return ResultReference.parse_obj(parameter)
-    except pydantic.error_wrappers.ValidationError:
+    except pydantic.ValidationError:
         pass
     except TypeError:
         pass
 
     try:
         return ParameterReference.parse_obj(parameter)
-    except pydantic.error_wrappers.ValidationError:
+    except pydantic.ValidationError:
         pass
     except TypeError:
         pass
 
     return parameter
```

### Comparing `openeo_pg_parser_networkx-2024.4.0/pyproject.toml` & `openeo_pg_parser_networkx-2024.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openeo-pg-parser-networkx"
-version = "2024.4.0"
+version = "2024.5.0"
 
 description = "Parse OpenEO process graphs from JSON to traversible Python objects."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/Open-EO/openeo-pg-parser-networkx"
 classifiers = [
@@ -20,19 +20,19 @@
 
 packages = [
     { include = "openeo_pg_parser_networkx" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pydantic = "^1.9.1"
+pydantic = "^2.4.0"
 pyproj = "^3.4.0"
 networkx = "^2.8.6"
 shapely = ">=1.8"
-geojson-pydantic = "^0.5.0"
+geojson-pydantic = "^1.0.0"
 numpy = "^1.20.3"
 pendulum = "^2.1.2"
 matplotlib = { version = "^3.7.1", optional = true }
 traitlets = "<=5.9.0"
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.7.1"
```

### Comparing `openeo_pg_parser_networkx-2024.4.0/PKG-INFO` & `openeo_pg_parser_networkx-2024.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openeo-pg-parser-networkx
-Version: 2024.4.0
+Version: 2024.5.0
 Summary: Parse OpenEO process graphs from JSON to traversible Python objects.
 Home-page: https://github.com/Open-EO/openeo-pg-parser-networkx
 License: Apache 2.0
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: plot
-Requires-Dist: geojson-pydantic (>=0.5.0,<0.6.0)
+Requires-Dist: geojson-pydantic (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) ; extra == "plot"
 Requires-Dist: networkx (>=2.8.6,<3.0.0)
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: pydantic (>=2.4.0,<3.0.0)
 Requires-Dist: pyproj (>=3.4.0,<4.0.0)
 Requires-Dist: shapely (>=1.8)
 Requires-Dist: traitlets (<=5.9.0)
 Project-URL: Repository, https://github.com/Open-EO/openeo-pg-parser-networkx
 Description-Content-Type: text/markdown
 
 # OpenEO Process Graph Parser (Python & networkx)
```

