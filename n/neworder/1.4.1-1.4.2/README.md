# Comparing `tmp/neworder-1.4.1.tar.gz` & `tmp/neworder-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neworder-1.4.1.tar", last modified: Wed Aug 30 16:50:44 2023, max compression
+gzip compressed data, was "neworder-1.4.2.tar", last modified: Mon May 27 12:56:11 2024, max compression
```

## Comparing `neworder-1.4.1.tar` & `neworder-1.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 16:50:44.445983 neworder-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (999)     1085 2023-08-30 16:50:20.000000 neworder-1.4.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (999)      107 2023-08-30 16:50:20.000000 neworder-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     6425 2023-08-30 16:50:44.445983 neworder-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4520 2023-08-30 16:50:20.000000 neworder-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 16:50:44.437983 neworder-1.4.1/neworder/
--rw-r--r--   0 runner    (1001) docker     (999)      357 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    13861 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (999)     1290 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/df.pyi
--rw-r--r--   0 runner    (1001) docker     (999)     8930 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/domain.py
--rw-r--r--   0 runner    (1001) docker     (999)     2406 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (999)      490 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/mc.py
--rw-r--r--   0 runner    (1001) docker     (999)      398 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/mpi.pyi
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/py.typed
--rw-r--r--   0 runner    (1001) docker     (999)     1328 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/stats.pyi
--rw-r--r--   0 runner    (1001) docker     (999)     1098 2023-08-30 16:50:20.000000 neworder-1.4.1/neworder/time.pyi
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 16:50:44.437983 neworder-1.4.1/neworder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     6425 2023-08-30 16:50:44.000000 neworder-1.4.1/neworder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      760 2023-08-30 16:50:44.000000 neworder-1.4.1/neworder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 16:50:44.000000 neworder-1.4.1/neworder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 16:50:43.000000 neworder-1.4.1/neworder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      354 2023-08-30 16:50:44.000000 neworder-1.4.1/neworder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       24 2023-08-30 16:50:44.000000 neworder-1.4.1/neworder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1435 2023-08-30 16:50:25.000000 neworder-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      315 2023-08-30 16:50:44.445983 neworder-1.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (999)      988 2023-08-30 16:50:20.000000 neworder-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 16:50:44.445983 neworder-1.4.1/src/
--rw-r--r--   0 runner    (1001) docker     (999)     4097 2023-08-30 16:50:20.000000 neworder-1.4.1/src/ArrayHelpers.h
--rw-r--r--   0 runner    (1001) docker     (999)     5789 2023-08-30 16:50:20.000000 neworder-1.4.1/src/DataFrame.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      633 2023-08-30 16:50:20.000000 neworder-1.4.1/src/DataFrame.h
--rw-r--r--   0 runner    (1001) docker     (999)      410 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Error.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      547 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Error.h
--rw-r--r--   0 runner    (1001) docker     (999)      500 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Helpers.h
--rw-r--r--   0 runner    (1001) docker     (999)      644 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Log.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     2395 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Log.h
--rw-r--r--   0 runner    (1001) docker     (999)     3194 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Model.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     1346 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Model.h
--rw-r--r--   0 runner    (1001) docker     (999)    10705 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Module.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      662 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Module.h
--rw-r--r--   0 runner    (1001) docker     (999)    14331 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Module_docstr.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     9940 2023-08-30 16:50:20.000000 neworder-1.4.1/src/MonteCarlo.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     2938 2023-08-30 16:50:20.000000 neworder-1.4.1/src/MonteCarlo.h
--rw-r--r--   0 runner    (1001) docker     (999)      643 2023-08-30 16:50:20.000000 neworder-1.4.1/src/NPArray.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      526 2023-08-30 16:50:20.000000 neworder-1.4.1/src/NPArray.h
--rw-r--r--   0 runner    (1001) docker     (999)      393 2023-08-30 16:50:20.000000 neworder-1.4.1/src/NewOrder.h
--rw-r--r--   0 runner    (1001) docker     (999)    10329 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Timeline.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     6427 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Timeline.h
--rw-r--r--   0 runner    (1001) docker     (999)      550 2023-08-30 16:50:20.000000 neworder-1.4.1/src/Timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:56:11.195991 neworder-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-27 12:55:53.000000 neworder-1.4.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 12:55:53.000000 neworder-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-05-27 12:56:11.195991 neworder-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-27 12:55:53.000000 neworder-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:56:11.187991 neworder-1.4.2/neworder/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15862 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/df.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/mc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/mpi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-27 12:55:53.000000 neworder-1.4.2/neworder/time.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:56:11.191991 neworder-1.4.2/neworder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-05-27 12:56:11.000000 neworder-1.4.2/neworder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-27 12:56:11.000000 neworder-1.4.2/neworder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:56:11.000000 neworder-1.4.2/neworder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:56:10.000000 neworder-1.4.2/neworder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-27 12:56:11.000000 neworder-1.4.2/neworder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 12:56:11.000000 neworder-1.4.2/neworder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-27 12:55:59.000000 neworder-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 12:56:11.195991 neworder-1.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      988 2024-05-27 12:55:53.000000 neworder-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:56:11.191991 neworder-1.4.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-27 12:55:53.000000 neworder-1.4.2/src/ArrayHelpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-27 12:55:53.000000 neworder-1.4.2/src/DataFrame.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-27 12:55:53.000000 neworder-1.4.2/src/DataFrame.h
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Error.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Error.h
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Model.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Module.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Module.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Module_docstr.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-05-27 12:55:53.000000 neworder-1.4.2/src/MonteCarlo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-27 12:55:53.000000 neworder-1.4.2/src/MonteCarlo.h
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-27 12:55:53.000000 neworder-1.4.2/src/NPArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-27 12:55:53.000000 neworder-1.4.2/src/NPArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-27 12:55:53.000000 neworder-1.4.2/src/NewOrder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Timeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Timeline.h
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-27 12:55:53.000000 neworder-1.4.2/src/Timer.h
```

### Comparing `neworder-1.4.1/LICENCE.md` & `neworder-1.4.2/LICENCE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright &copy; 2017-2023 Andrew P Smith
+Copyright &copy; 2017-2024 Andrew P Smith
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `neworder-1.4.1/PKG-INFO` & `neworder-1.4.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: neworder
-Version: 1.4.1
+Version: 1.4.2
 Summary: A dynamic microsimulation framework
 Author-email: Andrew Smith <andrew@friarswood.net>
 License: # MIT License
         
-        Copyright &copy; 2017-2023 Andrew P Smith
+        Copyright &copy; 2017-2024 Andrew P Smith
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -21,26 +21,46 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.**
         
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://neworder.readthedocs.io/
+Project-URL: Bug Tracker, https://github.com/virgesmith/neworder/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENCE.md
+Requires-Dist: pandas>=1.5.0
+Requires-Dist: pandas-stubs
+Requires-Dist: scipy>=1.9.3
+Requires-Dist: matplotlib>=3.6.2
 Provides-Extra: geospatial
+Requires-Dist: networkx>3.0; extra == "geospatial"
+Requires-Dist: osmnx>=1.3.0; extra == "geospatial"
+Requires-Dist: geopandas>=0.12.2; extra == "geospatial"
+Requires-Dist: shapely>=2.0.0; extra == "geospatial"
 Provides-Extra: parallel
+Requires-Dist: mpi4py>=3.0.3; extra == "parallel"
 Provides-Extra: dev
-License-File: LICENCE.md
+Requires-Dist: pybind11>=2.10.3; extra == "dev"
+Requires-Dist: pytest>=7.1.3; extra == "dev"
+Requires-Dist: mypy>=1.5.0; extra == "dev"
+Requires-Dist: mypy-extensions>=1.0.0; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mkdocs>=1.4.2; extra == "dev"
+Requires-Dist: mkdocs-macros-plugin>=0.7.0; extra == "dev"
+Requires-Dist: mkdocs-material>=9.0.2; extra == "dev"
+Requires-Dist: mkdocs-material-extensions>=1.1.1; extra == "dev"
+Requires-Dist: mkdocs-video>=1.3.0; extra == "dev"
 
 # neworder
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neworder)](https://pypi.org/project/neworder/)
 [![PyPI](https://img.shields.io/pypi/v/neworder)](https://pypi.org/project/neworder/)
 
 [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `neworder-1.4.1/README.md` & `neworder-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/neworder/__init__.pyi` & `neworder-1.4.2/neworder/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,135 @@
 """
 A dynamic microsimulation framework";
 """
+
 from __future__ import annotations
-import typing
+
 import datetime
-import numpy as np
-import numpy.typing as npt
+import typing
 
-import df  # type: ignore
-import mpi # type: ignore
-from . import time
-import stats # type: ignore
-from .domain import NPFloatArray
-
-date_t = datetime.datetime | datetime.date
-FloatArray1d = NPFloatArray | list[float]
-NPIntArray = npt.NDArray[np.int64]
-IntArray1d = NPIntArray | list[int]
+import numpy
+import numpy.typing as npt
 
+from . import df, mpi, stats, time
+from .domain import Domain, Edge, Space, StateGrid
+from .mc import as_np
 
 __all__ = [
+    "as_np",
     "CalendarTimeline",
     "LinearTimeline",
     "Model",
     "MonteCarlo",
     "NoTimeline",
     "NumericTimeline",
     "Timeline",
     "checked",
     "df",
     "log",
     "mpi",
     "run",
     "stats",
     "time",
-    "verbose"
+    "verbose",
+    "Space",
+    "Domain",
+    "Edge",
+    "StateGrid",
+    "as_np",
 ]
 
 
-class Timeline():
-    def __init__(self) -> None: ...
-    def __repr__(self) -> str:
-        """
-        Prints a human-readable representation of the timeline object
-        """
-    @property
-    def at_end(self) -> bool:
-        """
-            Returns True if the current step is the end of the timeline
-
-        :type: bool
-        """
-    @property
-    def dt(self) -> float:
-        """
-            Returns the step size size of the timeline
-
-        :type: float
-        """
-    @property
-    def end(self) -> object:
-        """
-            Returns the time of the end of the timeline
-
-        :type: object
-        """
-    @property
-    def index(self) -> int:
-        """
-            Returns the index of the current step in the timeline
+class CalendarTimeline(Timeline):
+    """
 
-        :type: int
-        """
-    @property
-    def nsteps(self) -> int:
-        """
-            Returns the number of steps in the timeline (or -1 if open-ended)
+    A calendar-based timeline
+    """
 
-        :type: int
+    @typing.overload
+    def __init__(
+        self, start: datetime.date, end: datetime.date, step: int, unit: str
+    ) -> None:
         """
-    @property
-    def start(self) -> object:
+        Constructs a calendar-based timeline, given start and end dates, an increment specified as a multiple of days, months or years
         """
-            Returns the time of the start of the timeline
-
-        :type: object
+    @typing.overload
+    def __init__(self, start: datetime.date, step: int, unit: str) -> None:
         """
-    @property
-    def time(self) -> object:
+        Constructs an open-ended calendar-based timeline, given a start date and an increment specified as a multiple of days, months or years.
+         NB the model will run until the Model.halt() method is explicitly called (from inside the step() method). Note also that nsteps() will
+         return -1 for timelines constructed this way
         """
-            Returns the time of the current step in the timeline
 
-        :type: object
-        """
-    pass
 class LinearTimeline(Timeline):
     """
+
     An equally-spaced non-calendar timeline .
     """
+
     @typing.overload
     def __init__(self, start: float, end: float, nsteps: int) -> None:
         """
         Constructs a timeline from start to end, with the given number of steps.
         """
     @typing.overload
     def __init__(self, start: float, step: float) -> None:
         """
         Constructs an open-ended timeline give a start value and a step size. NB the model will run until the Model.halt() method is explicitly called
         (from inside the step() method). Note also that nsteps() will return -1 for timelines constructed this way
         """
-        pass
-class Model():
+
+class Model:
     """
+
     The base model class from which all neworder models should be subclassed
     """
-    def __init__(self, timeline: Timeline, seeder: typing.Callable[[int], int] = MonteCarlo.deterministic_independent_stream) -> None:
+
+    class RunState:
+        """
+        Members:
+
+          NOT_STARTED
+
+          RUNNING
+
+          HALTED
+
+          COMPLETED
+        """
+
+        COMPLETED: typing.ClassVar[Model.RunState]  # value = <RunState.COMPLETED: 3>
+        HALTED: typing.ClassVar[Model.RunState]  # value = <RunState.HALTED: 2>
+        NOT_STARTED: typing.ClassVar[
+            Model.RunState
+        ]  # value = <RunState.NOT_STARTED: 0>
+        RUNNING: typing.ClassVar[Model.RunState]  # value = <RunState.RUNNING: 1>
+        __members__: typing.ClassVar[
+            dict[str, Model.RunState]
+        ]  # value = {'NOT_STARTED': <RunState.NOT_STARTED: 0>, 'RUNNING': <RunState.RUNNING: 1>, 'HALTED': <RunState.HALTED: 2>, 'COMPLETED': <RunState.COMPLETED: 3>}
+        def __eq__(self, other: typing.Any) -> bool: ...
+        def __getstate__(self) -> int: ...
+        def __hash__(self) -> int: ...
+        def __index__(self) -> int: ...
+        def __init__(self, value: int) -> None: ...
+        def __int__(self) -> int: ...
+        def __ne__(self, other: typing.Any) -> bool: ...
+        def __repr__(self) -> str: ...
+        def __setstate__(self, state: int) -> None: ...
+        def __str__(self) -> str: ...
+        @property
+        def name(self) -> str: ...
+        @property
+        def value(self) -> int: ...
+
+    COMPLETED: typing.ClassVar[Model.RunState]  # value = <RunState.COMPLETED: 3>
+    HALTED: typing.ClassVar[Model.RunState]  # value = <RunState.HALTED: 2>
+    NOT_STARTED: typing.ClassVar[Model.RunState]  # value = <RunState.NOT_STARTED: 0>
+    RUNNING: typing.ClassVar[Model.RunState]  # value = <RunState.RUNNING: 1>
+    def __init__(self, timeline: Timeline, seeder: typing.Callable = ...) -> None:
         """
         Constructs a model object with a timeline and (optionally) a seeder function for the random stream(s)
         """
     def check(self) -> bool:
         """
         User-overridable method used to check internal state at each timestep.
         Default behaviour is to simply return True.
@@ -135,212 +146,276 @@
         """
     def halt(self) -> None:
         """
         Signal to the model to stop execution gracefully at the end of the current timestep, e.g. if some convergence criterion has been met,
         or input is required from an upstream model. The model can be subsequently resumed by calling the run() function.
         For trapping exceptional/error conditions, prefer to raise an exception, or return False from the Model.check() function
         """
-    def modify(self, r: int) -> None:
+    def modify(self) -> None:
         """
         User-overridable method used to modify state in a per-process basis for multiprocess model runs.
         Default behaviour is to do nothing.
         This function should not be called directly, it is used by the Model.run() function
         """
     def step(self) -> None:
         """
         User-implemented method used to advance state of a model.
         Default behaviour raises NotImplementedError.
         This function should not be called directly, it is used by the Model.run() function
         """
     @property
     def mc(self) -> MonteCarlo:
         """
-            The model's Monte-Carlo engine
-
-        :type: MonteCarlo
+        The model's Monte-Carlo engine
+        """
+    @property
+    def run_state(self) -> Model.RunState:
+        """
+        The model's current state - one of:
+            NOT_STARTED: model has not been run
+            RUNNING: model is in progress
+            HALTED: model has been explicitly halted by calling its halt() method
+            COMPLETED: model has run to the end of its timeline
         """
     @property
     def timeline(self) -> Timeline:
         """
-            The model's timeline object
-
-        :type: Timeline
+        The model's timeline object
         """
-    pass
-class MonteCarlo():
+
+class MonteCarlo:
     """
+
     The model's Monte-Carlo engine with configurable options for parallel execution
     """
+
+    @staticmethod
+    def deterministic_identical_stream() -> int:
+        """
+        Returns a deterministic seed (19937). Input argument is ignored
+        """
+    @staticmethod
+    def deterministic_independent_stream() -> int:
+        """
+        Returns a deterministic seed that is a function of the input (19937+r).
+        The model uses the MPI rank as the input argument, allowing for differently seeded streams in each process
+        """
+    @staticmethod
+    def nondeterministic_stream() -> int:
+        """
+        Returns a random seed from the platform's random_device. Input argument is ignored
+        """
     def __repr__(self) -> str:
         """
         Prints a human-readable representation of the MonteCarlo engine
         """
-    def arrivals(self, lambda_: FloatArray1d, dt: float, n: int, mingap: float) -> NPFloatArray:
+    def arrivals(
+        self, lambda_: npt.NDArray[numpy.float64], dt: float, n: int, mingap: float
+    ) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of n arrays of multiple arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with a minimum separation between events of mingap. Sampling uses the Lewis-Shedler "thinning" algorithm
         The final value of lambda must be zero, and thus arrivals don't always occur, indicated by a value of neworder.time.never()
         The inner dimension of the returned 2d array is governed by the the maximum number of arrivals sampled, and will thus vary
         """
-    def counts(self, lambda_: FloatArray1d, dt: float) -> NPIntArray:
+    def counts(
+        self, lambda_: npt.NDArray[numpy.float64], dt: float
+    ) -> npt.NDArray[numpy.int64]:
         """
         Returns an array of simulated arrival counts (within time dt) for each intensity in lambda
         """
-    @staticmethod
-    def deterministic_identical_stream(r: int) -> int:
-        """
-        Returns a deterministic seed (19937). Input argument is ignored
-        """
-    @staticmethod
-    def deterministic_independent_stream(r: int) -> int:
-        """
-        Returns a deterministic seed that is a function of the input (19937+r).
-        The model uses the MPI rank as the input argument, allowing for differently seeded streams in each process
-        """
     @typing.overload
-    def first_arrival(self, lambda_: FloatArray1d, dt: float, n: int) -> NPFloatArray:
+    def first_arrival(
+        self, lambda_: npt.NDArray[numpy.float64], dt: float, n: int, minval: float
+    ) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of length n of first arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with a minimum start time of minval. Sampling uses the Lewis-Shedler "thinning" algorithm
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
         """
     @typing.overload
-    def first_arrival(self, lambda_: FloatArray1d, dt: float, n: int, minval: float) -> NPFloatArray:
+    def first_arrival(
+        self, lambda_: npt.NDArray[numpy.float64], dt: float, n: int
+    ) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of length n of first arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with no minimum start time. Sampling uses the Lewis-Shedler "thinning" algorithm
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
         """
     @typing.overload
-    def hazard(self, p: float, n: int) -> NPFloatArray:
+    def hazard(self, p: float, n: int) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of ones (with hazard rate lambda) or zeros of length n
         """
     @typing.overload
-    def hazard(self, p: NPFloatArray) -> NPFloatArray:
+    def hazard(self, p: npt.NDArray[numpy.float64]) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of ones (with hazard rate lambda[i]) or zeros for each element in p
         """
     @typing.overload
-    def next_arrival(self, startingpoints: FloatArray1d, lambda_: FloatArray1d, dt: float) -> NPFloatArray:
+    def next_arrival(
+        self,
+        startingpoints: npt.NDArray[numpy.float64],
+        lambda_: npt.NDArray[numpy.float64],
+        dt: float,
+        relative: bool,
+        minsep: float,
+    ) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of length n of subsequent arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with start times given by startingpoints with a minimum offset of mingap. Sampling uses the Lewis-Shedler "thinning" algorithm.
         If the relative flag is True, then lambda[0] corresponds to start time + mingap, not to absolute time
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
         """
     @typing.overload
-    def next_arrival(self, startingpoints: FloatArray1d, lambda_: FloatArray1d, dt: float, relative: bool) -> NPFloatArray:
+    def next_arrival(
+        self,
+        startingpoints: npt.NDArray[numpy.float64],
+        lambda_: npt.NDArray[numpy.float64],
+        dt: float,
+        relative: bool,
+    ) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of length n of subsequent arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with start times given by startingpoints. Sampling uses the Lewis-Shedler "thinning" algorithm.
         If the relative flag is True, then lambda[0] corresponds to start time, not to absolute time
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
         """
     @typing.overload
-    def next_arrival(self, startingpoints: FloatArray1d, lambda_: FloatArray1d, dt: float, relative: bool, minsep: float) -> NPFloatArray:
+    def next_arrival(
+        self,
+        startingpoints: npt.NDArray[numpy.float64],
+        lambda_: npt.NDArray[numpy.float64],
+        dt: float,
+    ) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of length n of subsequent arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with start times given by startingpoints. Sampling uses the Lewis-Shedler "thinning" algorithm.
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
         """
-    @staticmethod
-    def nondeterministic_stream(r: int) -> int:
-        """
-        Returns a random seed from the platform's random_device. Input argument is ignored
-        """
     def raw(self) -> int:
         """
         Returns a random 64-bit unsigned integer. Useful for seeding other generators.
         """
     def reset(self) -> None:
         """
         Resets the generator using the original seed.
         Use with care, esp in multi-process models with identical streams
         """
-    def sample(self, n: int, cat_weights: NPFloatArray) -> NPIntArray:
+    def sample(
+        self, n: int, cat_weights: npt.NDArray[numpy.float64]
+    ) -> npt.NDArray[numpy.int64]:
         """
         Returns an array of length n containing randomly sampled categorical values, weighted according to cat_weights
         """
     def seed(self) -> int:
         """
         Returns the seed used to initialise the random stream
         """
     def state(self) -> int:
         """
         Returns a hash of the internal state of the generator. Avoids the extra complexity of tranmitting variable-length strings over MPI.
         """
     @typing.overload
-    def stopping(self, lambda_: float, n: int) -> NPFloatArray:
+    def stopping(self, lambda_: float, n: int) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of stopping times (with hazard rate lambda) of length n
         """
     @typing.overload
-    def stopping(self, lambda_: NPFloatArray) -> NPFloatArray:
+    def stopping(
+        self, lambda_: npt.NDArray[numpy.float64]
+    ) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of stopping times (with hazard rate lambda[i]) for each element in lambda
         """
-    def ustream(self, n: int) -> NPFloatArray:
+    def ustream(self, n: int) -> npt.NDArray[numpy.float64]:
         """
         Returns an array of uniform random [0,1) variates of length n
         """
-    pass
+
 class NoTimeline(Timeline):
     """
+
     An arbitrary one step timeline, for continuous-time models with no explicit (discrete) timeline
     """
+
     def __init__(self) -> None:
         """
         Constructs an arbitrary one step timeline, where the start and end times are undefined and there is a single step of size zero. Useful for continuous-time models
         """
-    pass
+
 class NumericTimeline(Timeline):
     """
+
     An custom non-calendar timeline where the user explicitly specifies the time points, which must be monotonically increasing.
     """
-    def __init__(self, times: typing.List[float]) -> None:
+
+    def __init__(self, times: list[float]) -> None:
         """
         Constructs a timeline from an array of time points.
         """
-    pass
-class CalendarTimeline(Timeline):
-    """
-    A calendar-based timeline
-    """
-    @typing.overload
-    def __init__(self, start: date_t, end: date_t, step: int, unit: str) -> None:
+
+class Timeline:
+    def __init__(self) -> None: ...
+    def __repr__(self) -> str:
         """
-        Constructs a calendar-based timeline, given start and end dates, an increment specified as a multiple of days, months or years
+        Prints a human-readable representation of the timeline object
         """
-    @typing.overload
-    def __init__(self, start: date_t, step: int, unit: str) -> None:
+    @property
+    def at_end(self) -> bool:
         """
-        Constructs an open-ended calendar-based timeline, given a start date and an increment specified as a multiple of days, months or years.
-         NB the model will run until the Model.halt() method is explicitly called (from inside the step() method). Note also that nsteps() will
-         return -1 for timelines constructed this way
+        Returns True if the current step is the end of the timeline
+        """
+    @property
+    def dt(self) -> float:
+        """
+        Returns the step size size of the timeline
+        """
+    @property
+    def end(self) -> typing.Any:
+        """
+        Returns the time of the end of the timeline
+        """
+    @property
+    def index(self) -> int:
+        """
+        Returns the index of the current step in the timeline
+        """
+    @property
+    def nsteps(self) -> int:
+        """
+        Returns the number of steps in the timeline (or -1 if open-ended)
+        """
+    @property
+    def start(self) -> typing.Any:
+        """
+        Returns the time of the start of the timeline
         """
-    pass
+    @property
+    def time(self) -> typing.Any:
+        """
+        Returns the time of the current step in the timeline
+        """
+
 def checked(checked: bool = True) -> None:
     """
     Sets the checked flag, which determines whether the model runs checks during execution
     """
-def log(obj: object) -> None:
+
+def log(obj: typing.Any) -> None:
     """
     The logging function. Prints obj to the console, annotated with process information
     """
+
 def run(model: Model) -> bool:
     """
     Runs the model. If the model has previously run it will resume from the point at which it was given the "halt" instruction. This is useful
     for external processing of model data, and/or feedback from external sources. If the model has already reached the end of the timeline, this
     function will have no effect. To re-run the model from the start, you must construct a new model object.
     Returns:
         True if model succeeded, False otherwise
     """
+
 def verbose(verbose: bool = True) -> None:
     """
     Sets the verbose flag, which toggles detailed runtime logs
     """
-
-def as_np(mc: MonteCarlo) -> np.random.Generator:
-  """
-  Returns an adapter enabling the MonteCarlo object to be used with numpy random functionality
-  """
```

### Comparing `neworder-1.4.1/neworder/df.pyi` & `neworder-1.4.2/neworder/df.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 """
-    Submodule for operations involving direct manipulation of pandas dataframes
+
+Submodule for operations involving direct manipulation of pandas dataframes
 """
+
 from __future__ import annotations
-from typing import TypeVar
-import neworder
-import numpy as np
-# _Shape = typing.Tuple[int, ...]
 
-T = TypeVar("T")
-nparray = np.ndarray[T, np.dtype[T]]
+import typing
 
-__all__ = [
-    "testfunc",
-    "transition",
-    "unique_index"
-]
+import numpy
+import numpy.typing as npt
 
+import neworder
 
-def testfunc(model: neworder.Model, df: object, colname: str) -> None:
+__all__ = ["testfunc", "transition", "unique_index"]
+
+def testfunc(model: neworder.Model, df: typing.Any, colname: str) -> None:
     """
     Test function for direct dataframe manipulation. Results may vary. Do not use.
     """
-def transition(model: neworder.Model, categories: nparray[np.int64], transition_matrix: nparray[np.float64], df: object, colname: str) -> None:
+
+def transition(
+    model: neworder.Model,
+    categories: npt.NDArray[numpy.int64],
+    transition_matrix: npt.NDArray[numpy.float64],
+    df: typing.Any,
+    colname: str,
+) -> None:
     """
     Randomly changes categorical data in a dataframe, according to supplied transition probabilities.
     Args:
         model: The model (for access to the MonteCarlo engine).
         categories: The set of possible categories
         transition_matrix: The probabilities of transitions between categories
         df: The dataframe, which is modified in-place
         colname: The name of the column in the dataframe
     """
-def unique_index(n: int) -> nparray[np.int64]:
+
+def unique_index(n: int) -> npt.NDArray[numpy.int64]:
     """
     Generates an array of n unique values, even across multiple processes, that can be used to unambiguously index multiple dataframes.
     """
```

### Comparing `neworder-1.4.1/neworder/domain.py` & `neworder-1.4.2/neworder/domain.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,246 +1,290 @@
 """
 Spatial structures for positioning and moving entities and computing distances
 """
 
 from __future__ import annotations
-from typing import Union, Optional, Any, Callable
+
 from enum import Enum, auto
+from typing import Any, Callable, Optional, Union
+
 import numpy as np
 import numpy.typing as npt
 from scipy import signal  # type: ignore
 
 NPFloatArray = npt.NDArray[np.float64]
 
+
 class Edge(Enum):
-  """
-  Edge behaviour
-  """
-  UNBOUNDED = auto()
-  WRAP = auto()
-  CONSTRAIN = auto()
-  BOUNCE = auto()
+    """
+    Edge behaviour
+    """
+
+    UNBOUNDED = auto()
+    WRAP = auto()
+    CONSTRAIN = auto()
+    BOUNCE = auto()
 
 
 class Domain:
-  """
-  Base class for spatial domains.
-  """
-
-  def __init__(self, dim: int, edge: Edge, continuous: bool):
-    self.__dim = dim
-    self.__edge = edge
-    self.__continuous = continuous
-
-  @property
-  def dim(self) -> int:
-    """ The dimension of the spatial domain """
-    return self.__dim
-
-  @property
-  def edge(self) -> Edge:
-    """ The tyoe of edge constraint """
-    return self.__edge
-
-  @property
-  def continuous(self) -> bool:
-    """ Whether space is continuous or discrete """
-    return self.__continuous
+    """
+    Base class for spatial domains.
+    """
+
+    def __init__(self, dim: int, edge: Edge, continuous: bool):
+        self.__dim = dim
+        self.__edge = edge
+        self.__continuous = continuous
+
+    @property
+    def dim(self) -> int:
+        """The dimension of the spatial domain"""
+        return self.__dim
+
+    @property
+    def edge(self) -> Edge:
+        """The tyoe of edge constraint"""
+        return self.__edge
+
+    @property
+    def continuous(self) -> bool:
+        """Whether space is continuous or discrete"""
+        return self.__continuous
 
 
 class Space(Domain):
-  """
-  Continuous rectangular n-dimensional finite or infinite domain.
-  If finite, positioning and/or movement near the domain boundary is
-  dictated by the `wrap` attribute.
-  """
-
-  @staticmethod
-  def unbounded(dim: int) -> Space:
-    """ Construct an unbounded Space """
-    assert dim > 0
-    return Space(np.full(dim, -np.inf), np.full(dim, +np.inf), edge=Edge.UNBOUNDED)
-
-  def __init__(self, min: NPFloatArray, max: NPFloatArray, edge: Edge=Edge.CONSTRAIN):
-    assert len(min) and len(min) == len(max)
-    super().__init__(len(min), edge, True)
-
-    # Space supports all edge behaviours
-    assert edge in [Edge.UNBOUNDED, Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE]
-
-    assert np.all(max > min)
-
-    self.min = min
-    self.max = max
-
-  @property
-  def extent(self) -> tuple[NPFloatArray, NPFloatArray]:
-    """ The extent of the space in terms of two opposing points """
-    return self.min, self.max
-
-  def move(self, positions: Any,
-                 velocities: Any,
-                 delta_t: float,
-                 ungroup: bool=False) -> tuple[NPFloatArray, NPFloatArray]:
-    """ Returns translated positions AND velocities """
-    # group tuples into a single array if necessary
-    if isinstance(positions, tuple):
-      positions = np.column_stack(positions)
-    if isinstance(velocities, tuple):
-      velocities = np.column_stack(velocities)
-
-    assert positions.dtype == float
-    assert velocities.dtype == float
-    assert positions.shape[-1] == self.dim and velocities.shape[-1] == self.dim
-    if self.edge == Edge.UNBOUNDED:
-      p = positions + velocities * delta_t
-      v = velocities
-    elif self.edge == Edge.CONSTRAIN:
-      p = positions + velocities * delta_t
-      v = velocities
-      hitmin = np.where(p < self.min, 1, 0)
-      p = np.where(hitmin, self.min, p)
-      v = np.where(hitmin, 0, v)
-      hitmax = np.where(p > self.max, 1, 0)
-      p = np.where(hitmax, self.max, p)
-      v = np.where(hitmax, 0, v)
-    elif self.edge == Edge.BOUNCE:
-      p = positions + velocities * delta_t
-      v = velocities
-      hitmin = np.where(p < self.min, 1, 0)
-      p = np.where(hitmin, 2 * self.min - p, p)
-      v = np.where(hitmin, -v, v)
-      hitmax = np.where(p > self.max, 1, 0)
-      p = np.where(hitmax, 2 * self.max - p, p)
-      v = np.where(hitmax, -v, v)
-    else:
-      p = self.min + np.mod(positions + velocities * delta_t - self.min, self.max - self.min)
-      v = velocities
-
-    if ungroup:
-      p = np.split(p, self.dim, axis=1)
-      v = np.split(v, self.dim, axis=1)
-    return p, v
-
-  def dists2(self, positions: Union[tuple[NPFloatArray, ...], NPFloatArray], to_points: Optional[NPFloatArray]=None) -> tuple[NPFloatArray, Any]:
-    """ The squared distance between points and separations along each axis """
-    # group tuples into a single array if necessary
-    if isinstance(positions, tuple):
-      positions = np.column_stack(positions)
-    if isinstance(to_points, tuple):
-      to_points = np.column_stack(to_points)
-    # distances w.r.t. self if to_points not explicitly specified
-    if to_points is None:
-      to_points = positions
-    assert positions.dtype == float
-    assert to_points.dtype == float
-    n = positions.shape[0]
-    m = to_points.shape[0]
-    d = positions.shape[1]
-    d2 = np.zeros((m, n))
-    separations: tuple[Any, ...] = ()
-    if self.edge != Edge.WRAP:
-      for i in range(d):
-        delta = np.tile(positions[:, i], m).reshape((m, n)) - np.repeat(to_points[:, i], n).reshape(m, n)
-        separations += (delta,)
-        d2 += delta * delta
-    else: # wrapped domains need special treatment - distance across an edge may be less than naive distance
-      for i in range(d):
-        delta = np.tile(positions[:, i], m).reshape((m, n)) - np.repeat(to_points[:, i], n).reshape(m, n)
-        r = self.max[i] - self.min[i]
-        delta = np.where(delta > r / 2, delta - r, delta)
-        delta = np.where(delta < -r / 2, delta + r, delta)
-        separations += (delta,)
-        d2 += delta * delta
-
-    return d2, separations
-
-  def dists(self, positions: Union[tuple[NPFloatArray, ...], NPFloatArray], to_points: Optional[NPFloatArray]=None) -> NPFloatArray:
-    """ Returns distances between the points"""
-    return np.sqrt(self.dists2(positions, to_points)[0])
-
-  def in_range(self, distance: Any, positions: Any, count: Optional[bool]=False) -> NPFloatArray:
-    """ Returns either indices or counts of points within the specified distance from each point """
-    ind = np.where(self.dists2(positions)[0] < distance * distance, 1, 0)
-    # fill diagonal so as not to include self - TODO how does this work if to_points!=positions
-    np.fill_diagonal(ind, 0)
-    return ind if not count else np.sum(ind, axis=1)
+    """
+    Continuous rectangular n-dimensional finite or infinite domain.
+    If finite, positioning and/or movement near the domain boundary is
+    dictated by the `wrap` attribute.
+    """
+
+    @staticmethod
+    def unbounded(dim: int) -> Space:
+        """Construct an unbounded Space"""
+        assert dim > 0
+        return Space(np.full(dim, -np.inf), np.full(dim, +np.inf), edge=Edge.UNBOUNDED)
+
+    def __init__(
+        self, min: NPFloatArray, max: NPFloatArray, edge: Edge = Edge.CONSTRAIN
+    ):
+        assert len(min) and len(min) == len(max)
+        super().__init__(len(min), edge, True)
+
+        # Space supports all edge behaviours
+        assert edge in [Edge.UNBOUNDED, Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE]
+
+        assert np.all(max > min)
+
+        self.min = min
+        self.max = max
+
+    @property
+    def extent(self) -> tuple[NPFloatArray, NPFloatArray]:
+        """The extent of the space in terms of two opposing points"""
+        return self.min, self.max
+
+    def move(
+        self, positions: Any, velocities: Any, delta_t: float, ungroup: bool = False
+    ) -> tuple[NPFloatArray, NPFloatArray]:
+        """Returns translated positions AND velocities"""
+        # group tuples into a single array if necessary
+        if isinstance(positions, tuple):
+            positions = np.column_stack(positions)
+        if isinstance(velocities, tuple):
+            velocities = np.column_stack(velocities)
+
+        assert positions.dtype == float
+        assert velocities.dtype == float
+        assert positions.shape[-1] == self.dim and velocities.shape[-1] == self.dim
+        if self.edge == Edge.UNBOUNDED:
+            p = positions + velocities * delta_t
+            v = velocities
+        elif self.edge == Edge.CONSTRAIN:
+            p = positions + velocities * delta_t
+            v = velocities
+            hitmin = np.where(p < self.min, 1, 0)
+            p = np.where(hitmin, self.min, p)
+            v = np.where(hitmin, 0, v)
+            hitmax = np.where(p > self.max, 1, 0)
+            p = np.where(hitmax, self.max, p)
+            v = np.where(hitmax, 0, v)
+        elif self.edge == Edge.BOUNCE:
+            p = positions + velocities * delta_t
+            v = velocities
+            hitmin = np.where(p < self.min, 1, 0)
+            p = np.where(hitmin, 2 * self.min - p, p)
+            v = np.where(hitmin, -v, v)
+            hitmax = np.where(p > self.max, 1, 0)
+            p = np.where(hitmax, 2 * self.max - p, p)
+            v = np.where(hitmax, -v, v)
+        else:
+            p = self.min + np.mod(
+                positions + velocities * delta_t - self.min, self.max - self.min
+            )
+            v = velocities
+
+        if ungroup:
+            p = np.split(p, self.dim, axis=1)
+            v = np.split(v, self.dim, axis=1)
+        return p, v
+
+    def dists2(
+        self,
+        positions: Union[tuple[NPFloatArray, ...], NPFloatArray],
+        to_points: Optional[NPFloatArray] = None,
+    ) -> tuple[NPFloatArray, Any]:
+        """The squared distance between points and separations along each axis"""
+        # group tuples into a single array if necessary
+        if isinstance(positions, tuple):
+            positions = np.column_stack(positions)
+        if isinstance(to_points, tuple):
+            to_points = np.column_stack(to_points)
+        # distances w.r.t. self if to_points not explicitly specified
+        if to_points is None:
+            to_points = positions
+        assert positions.dtype == float
+        assert to_points.dtype == float
+        n = positions.shape[0]
+        m = to_points.shape[0]
+        d = positions.shape[1]
+        d2 = np.zeros((m, n))
+        separations: tuple[Any, ...] = ()
+        if self.edge != Edge.WRAP:
+            for i in range(d):
+                delta = np.tile(positions[:, i], m).reshape((m, n)) - np.repeat(
+                    to_points[:, i], n
+                ).reshape(m, n)
+                separations += (delta,)
+                d2 += delta * delta
+        else:  # wrapped domains need special treatment - distance across an edge may be less than naive distance
+            for i in range(d):
+                delta = np.tile(positions[:, i], m).reshape((m, n)) - np.repeat(
+                    to_points[:, i], n
+                ).reshape(m, n)
+                r = self.max[i] - self.min[i]
+                delta = np.where(delta > r / 2, delta - r, delta)
+                delta = np.where(delta < -r / 2, delta + r, delta)
+                separations += (delta,)
+                d2 += delta * delta
+
+        return d2, separations
+
+    def dists(
+        self,
+        positions: Union[tuple[NPFloatArray, ...], NPFloatArray],
+        to_points: Optional[NPFloatArray] = None,
+    ) -> NPFloatArray:
+        """Returns distances between the points"""
+        return np.sqrt(self.dists2(positions, to_points)[0])
+
+    def in_range(
+        self, distance: Any, positions: Any, count: Optional[bool] = False
+    ) -> NPFloatArray:
+        """Returns either indices or counts of points within the specified distance from each point"""
+        ind = np.where(self.dists2(positions)[0] < distance * distance, 1, 0)
+        # fill diagonal so as not to include self - TODO how does this work if to_points!=positions
+        np.fill_diagonal(ind, 0)
+        return ind if not count else np.sum(ind, axis=1)
+
+    def __repr__(self) -> str:
+        return "%s dim=%d min=%s max=%s edge=%s" % (
+            self.__class__.__name__,
+            self.dim,
+            self.min,
+            self.max,
+            self.edge,
+        )
 
-  def __repr__(self) -> str:
-    return "%s dim=%d min=%s max=%s edge=%s" % (self.__class__.__name__, self.dim, self.min, self.max, self.edge)
 
 def _bounce(i: int, N: int) -> int:
-  s = (i // N) % 2
-  k = i % N
-  return N * s + (-1) ** s * k
+    s = (i // N) % 2
+    k = i % N
+    return N * s + (-1) ** s * k
 
-class StateGrid(Domain):
-  """
-  Discrete rectangular n-dimensional finite grid domain with each cell having an integer state.
-  Allows for counting of neighbours according to the supported edge behaviours:
-    CONSTRAIN (no neighburs over edge), WRAP (toroidal), BOUNCE (reflect)
-  """
-
-  __mode_lookup: dict[Edge, str] = {
-    Edge.CONSTRAIN: "constant",
-    Edge.WRAP: "wrap",
-    Edge.BOUNCE: "reflect"
-  }
-
-  def __init__(self, initial_values: NPFloatArray, edge: Edge=Edge.CONSTRAIN):
-    super().__init__(initial_values.ndim, edge, False)
-
-    # StateGrid supports two edge behaviours
-    if edge not in [Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE]:
-      raise ValueError("edge policy must be one of Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE")
-
-    if initial_values.ndim < 1:
-      raise ValueError("state array must have dimension of 1 or above")
-    if initial_values.size < 1:
-      raise ValueError("state array must have size of 1 or above in every dimension")
-
-    self.state = initial_values
-
-    # int neighbour kernel (not including self)
-    self.kernel = np.ones([3] * self.dim)
-    self.kernel[(1,) * self.dim] = 0
-
-  def __get_point(self, p: tuple[int, ...]) -> tuple[int, ...]:
-    assert len(p) == self.state.ndim, f"dimensionality mismatch: {len(p)} but grid has {self.state.ndim}"
-    match self.edge:
-      case Edge.WRAP:
-        p = tuple(p[i] % self.state.shape[i] for i in range(len(p)))
-      case Edge.CONSTRAIN:
-        p = tuple(np.clip(p[i], 0, self.state.shape[i] - 1) for i in range(len(p)))
-      case Edge.BOUNCE:
-        p = tuple(_bounce(p[i], self.state.shape[i] - 1) for i in range(len(p)))
-    return p
-
-  def __getitem__(self, p: tuple[int, ...]) -> Any:
-    return self.state[self.__get_point(p)]
-
-  def __setitem__(self, p: tuple[int, ...], value: Any) -> None:
-    self.state[self.__get_point(p)] = value
-
-  def shift(self, position: tuple[int, ...], delta: tuple[int, ...]) -> tuple[int, ...]:
-    """This translates a point according to the grid's edge behaviour. It does *not* change any state"""
-    point = self.__get_point(position)
-    p = tuple(point[i] + delta[i] for i in range(self.dim))
-    return self.__get_point(p)
-
-  @property
-  def extent(self) -> Any:
-    """ The extent of the space in terms of two opposing points """
-    return self.state.shape
-
-  def count_neighbours(self, indicator: Callable[[float], bool]=lambda x: x == 1) -> NPFloatArray:
-    """ Counts neighbouring cells with a state indicated by supplied indicator function """
-
-    ind: NPFloatArray = np.array([indicator(x) for x in self.state]).astype(int)  # automagically preserves shape
-    # pad with boundary according to edge policy
-    bounded = np.pad(ind, pad_width=1, mode=self.__mode_lookup[self.edge])  # type: ignore # bug?
-
-    # count neighbours, drop padding, covert to int
-    count = signal.convolve(bounded, self.kernel, mode="same", method="direct")[(slice(1, -1),) * self.dim].astype(int)
 
-    return count
+class StateGrid(Domain):
+    """
+    Discrete rectangular n-dimensional finite grid domain with each cell having an integer state.
+    Allows for counting of neighbours according to the supported edge behaviours:
+      CONSTRAIN (no neighburs over edge), WRAP (toroidal), BOUNCE (reflect)
+    """
+
+    __mode_lookup: dict[Edge, str] = {
+        Edge.CONSTRAIN: "constant",
+        Edge.WRAP: "wrap",
+        Edge.BOUNCE: "reflect",
+    }
+
+    def __init__(self, initial_values: NPFloatArray, edge: Edge = Edge.CONSTRAIN):
+        super().__init__(initial_values.ndim, edge, False)
+
+        # StateGrid supports two edge behaviours
+        if edge not in [Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE]:
+            raise ValueError(
+                "edge policy must be one of Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE"
+            )
+
+        if initial_values.ndim < 1:
+            raise ValueError("state array must have dimension of 1 or above")
+        if initial_values.size < 1:
+            raise ValueError(
+                "state array must have size of 1 or above in every dimension"
+            )
+
+        self.state = initial_values
+
+        # int neighbour kernel (not including self)
+        self.kernel = np.ones([3] * self.dim)
+        self.kernel[(1,) * self.dim] = 0
+
+    def __get_point(self, p: tuple[int, ...]) -> tuple[int, ...]:
+        assert (
+            len(p) == self.state.ndim
+        ), f"dimensionality mismatch: {len(p)} but grid has {self.state.ndim}"
+        match self.edge:
+            case Edge.WRAP:
+                p = tuple(p[i] % self.state.shape[i] for i in range(len(p)))
+            case Edge.CONSTRAIN:
+                p = tuple(
+                    np.clip(p[i], 0, self.state.shape[i] - 1) for i in range(len(p))
+                )
+            case Edge.BOUNCE:
+                p = tuple(_bounce(p[i], self.state.shape[i] - 1) for i in range(len(p)))
+        return p
+
+    def __getitem__(self, p: tuple[int, ...]) -> Any:
+        return self.state[self.__get_point(p)]
+
+    def __setitem__(self, p: tuple[int, ...], value: Any) -> None:
+        self.state[self.__get_point(p)] = value
+
+    def shift(
+        self, position: tuple[int, ...], delta: tuple[int, ...]
+    ) -> tuple[int, ...]:
+        """This translates a point according to the grid's edge behaviour. It does *not* change any state"""
+        point = self.__get_point(position)
+        p = tuple(point[i] + delta[i] for i in range(self.dim))
+        return self.__get_point(p)
+
+    @property
+    def extent(self) -> Any:
+        """The extent of the space in terms of two opposing points"""
+        return self.state.shape
+
+    def count_neighbours(
+        self, indicator: Callable[[float], bool] = lambda x: x == 1
+    ) -> NPFloatArray:
+        """Counts neighbouring cells with a state indicated by supplied indicator function"""
+
+        ind: NPFloatArray = np.array([indicator(x) for x in self.state]).astype(
+            int
+        )  # automagically preserves shape
+        # pad with boundary according to edge policy
+        bounded = np.pad(ind, pad_width=1, mode=self.__mode_lookup[self.edge])  # type: ignore # bug?
+
+        # count neighbours, drop padding, covert to int
+        count = signal.convolve(bounded, self.kernel, mode="same", method="direct")[
+            (slice(1, -1),) * self.dim
+        ].astype(int)
 
+        return count
```

### Comparing `neworder-1.4.1/neworder/geospatial.py` & `neworder-1.4.2/neworder/geospatial.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,83 @@
 from __future__ import annotations
+
 from typing import Any, Generator
 
 try:
-  import networkx as nx  # type: ignore[import]
-  import osmnx as ox  # type: ignore[import]
-  from shapely.ops import linemerge  # type: ignore[import]
-  from shapely.geometry import LineString, MultiLineString, Polygon  # type: ignore[import]
-  import geopandas as gpd  # type: ignore[import]
+    import geopandas as gpd  # type: ignore[import]
+    import networkx as nx  # type: ignore[import]
+    import osmnx as ox  # type: ignore[import]
+    from shapely.geometry import (  # type: ignore[import]
+        LineString,
+        MultiLineString,
+        Polygon,
+    )
+    from shapely.ops import linemerge  # type: ignore[import]
 except ImportError:
-  raise ImportError("""optional dependencies are not installed.
+    raise ImportError(
+        """optional dependencies are not installed.
 Reinstalling neworder with the geospatial option should fix this:
-pip install neworder[geospatial]""")
+pip install neworder[geospatial]"""
+    )
 
 
 class GeospatialGraph:
-  """
-  Spatial domains on Earth's surface that are defined by graphs/networks.
-  Use of this class requires "geospatial" extras: pip install neworder[geospatial]
-  """
-
-  def __init__(self, G: nx.Graph, crs: str | None = None) -> None:
-    if crs:
-      self.__graph = ox.project_graph(G, to_crs=crs)
-    else:
-      self.__graph = G
-    self.__nodes, self.__edges = ox.graph_to_gdfs(self.__graph)
-
-  @classmethod
-  def from_point(cls, point: tuple[float, float], *args: Any, crs: str | None = None,  **kwargs: Any) -> GeospatialGraph:
-    G = ox.graph_from_point(point, *args, **kwargs)
-    return cls(G, crs)
-
-  @property
-  def crs(self) -> str:
-    return self.__graph.graph["crs"]
-
-  @property
-  def graph(self) -> nx.MultiDiGraph | nx.Graph:
-    return self.__graph
-
-  @property
-  def all_nodes(self) -> gpd.GeoDataFrame:
-    return self.__nodes
-
-  @property
-  def all_edges(self) -> gpd.GeoDataFrame:
-    return self.__edges
-
-  def edges_to(self, node: int) -> Generator[list[tuple[int, int]], None, None]:
-    return self.__graph.in_edges(node)
-
-  def edges_from(self, node: int) -> Generator[list[tuple[int, int]], None, None]:
-    return self.__graph.out_edges(node)
-
-  def shortest_path(self, origin: int, dest: int, **kwargs: Any) -> LineString:
-    nodes = nx.shortest_path(self.__graph, origin, dest, **kwargs)
-    route_segments = [self.__edges.loc[(nodes[i], nodes[i+1], 0), "geometry"] for i in range(len(nodes) - 1)]
-    return linemerge(MultiLineString(route_segments))
-
-  def subgraph(self, origin: int, **kwargs: Any) -> nx.Graph:
-    return nx.ego_graph(self.__graph, origin, **kwargs)
-
-  def isochrone(self, origin: int, **kwargs: Any) -> Polygon:
-    subgraph = nx.ego_graph(self.__graph, origin, **kwargs)
-    nodes, _ = ox.graph_to_gdfs(subgraph)
-    return nodes.geometry.unary_union.convex_hull
-
+    """
+    Spatial domains on Earth's surface that are defined by graphs/networks.
+    Use of this class requires "geospatial" extras: pip install neworder[geospatial]
+    """
+
+    def __init__(self, G: nx.Graph, crs: str | None = None) -> None:
+        if crs:
+            self.__graph = ox.project_graph(G, to_crs=crs)
+        else:
+            self.__graph = G
+        self.__nodes, self.__edges = ox.graph_to_gdfs(self.__graph)
+
+    @classmethod
+    def from_point(
+        cls,
+        point: tuple[float, float],
+        *args: Any,
+        crs: str | None = None,
+        **kwargs: Any,
+    ) -> GeospatialGraph:
+        G = ox.graph_from_point(point, *args, **kwargs)
+        return cls(G, crs)
+
+    @property
+    def crs(self) -> str:
+        return self.__graph.graph["crs"]
+
+    @property
+    def graph(self) -> nx.MultiDiGraph | nx.Graph:
+        return self.__graph
+
+    @property
+    def all_nodes(self) -> gpd.GeoDataFrame:
+        return self.__nodes
+
+    @property
+    def all_edges(self) -> gpd.GeoDataFrame:
+        return self.__edges
+
+    def edges_to(self, node: int) -> Generator[list[tuple[int, int]], None, None]:
+        return self.__graph.in_edges(node)
+
+    def edges_from(self, node: int) -> Generator[list[tuple[int, int]], None, None]:
+        return self.__graph.out_edges(node)
+
+    def shortest_path(self, origin: int, dest: int, **kwargs: Any) -> LineString:
+        nodes = nx.shortest_path(self.__graph, origin, dest, **kwargs)
+        route_segments = [
+            self.__edges.loc[(nodes[i], nodes[i + 1], 0), "geometry"]
+            for i in range(len(nodes) - 1)
+        ]
+        return linemerge(MultiLineString(route_segments))
+
+    def subgraph(self, origin: int, **kwargs: Any) -> nx.Graph:
+        return nx.ego_graph(self.__graph, origin, **kwargs)
+
+    def isochrone(self, origin: int, **kwargs: Any) -> Polygon:
+        subgraph = nx.ego_graph(self.__graph, origin, **kwargs)
+        nodes, _ = ox.graph_to_gdfs(subgraph)
+        return nodes.geometry.unary_union.convex_hull
```

### Comparing `neworder-1.4.1/neworder/time.pyi` & `neworder-1.4.2/neworder/time.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 """
-    Temporal values and comparison.
+
+Temporal values and comparison, including the attributes:
+NEVER: a value that compares unequal to any value, including itself.
+DISTANT_PAST: a value that compares less than any other value but itself and NEVER
+FAR_FUTURE: a value that compares greater than any other value but itself and NEVER
 """
+
 from __future__ import annotations
+
 import typing
-import numpy as np
-import numpy.typing as npt
 
-__all__ = [
-    "DISTANT_PAST",
-    "FAR_FUTURE",
-    "NEVER",
-    "isnever"
-]
+import numpy
+import numpy.typing as npt
 
+__all__ = ["DISTANT_PAST", "FAR_FUTURE", "NEVER", "isnever"]
 
 @typing.overload
 def isnever(t: float) -> bool:
     """
     Returns whether the value of t corresponds to "never". As "never" is implemented as a floating-point NaN,
     direct comparison will always fail, since NaN != NaN.
     """
 
 @typing.overload
-def isnever(t: npt.NDArray[np.float64] | list[float]) -> npt.NDArray[np.bool8]:
+def isnever(t: npt.NDArray[numpy.float64]) -> npt.NDArray:
     """
     Returns an array of booleans corresponding to whether the element of an array correspond to "never". As "never" is
     implemented as a floating-point NaN, direct comparison will always fails, since NaN != NaN.
     """
-DISTANT_PAST: float # value = -inf
-"""A value that compares less than any other value but itself and NEVER"""
-
-FAR_FUTURE: float # value = inf
-"""A value that compares greater than any other value but itself and NEVER"""
 
-NEVER: float # value = nan
-"""A value that compares unequal to any value, including itself"""
+DISTANT_PAST: float  # value = -inf
+FAR_FUTURE: float  # value = inf
+NEVER: float  # value = nan
```

### Comparing `neworder-1.4.1/neworder.egg-info/PKG-INFO` & `neworder-1.4.2/neworder.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: neworder
-Version: 1.4.1
+Version: 1.4.2
 Summary: A dynamic microsimulation framework
 Author-email: Andrew Smith <andrew@friarswood.net>
 License: # MIT License
         
-        Copyright &copy; 2017-2023 Andrew P Smith
+        Copyright &copy; 2017-2024 Andrew P Smith
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -21,26 +21,46 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.**
         
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://neworder.readthedocs.io/
+Project-URL: Bug Tracker, https://github.com/virgesmith/neworder/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENCE.md
+Requires-Dist: pandas>=1.5.0
+Requires-Dist: pandas-stubs
+Requires-Dist: scipy>=1.9.3
+Requires-Dist: matplotlib>=3.6.2
 Provides-Extra: geospatial
+Requires-Dist: networkx>3.0; extra == "geospatial"
+Requires-Dist: osmnx>=1.3.0; extra == "geospatial"
+Requires-Dist: geopandas>=0.12.2; extra == "geospatial"
+Requires-Dist: shapely>=2.0.0; extra == "geospatial"
 Provides-Extra: parallel
+Requires-Dist: mpi4py>=3.0.3; extra == "parallel"
 Provides-Extra: dev
-License-File: LICENCE.md
+Requires-Dist: pybind11>=2.10.3; extra == "dev"
+Requires-Dist: pytest>=7.1.3; extra == "dev"
+Requires-Dist: mypy>=1.5.0; extra == "dev"
+Requires-Dist: mypy-extensions>=1.0.0; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mkdocs>=1.4.2; extra == "dev"
+Requires-Dist: mkdocs-macros-plugin>=0.7.0; extra == "dev"
+Requires-Dist: mkdocs-material>=9.0.2; extra == "dev"
+Requires-Dist: mkdocs-material-extensions>=1.1.1; extra == "dev"
+Requires-Dist: mkdocs-video>=1.3.0; extra == "dev"
 
 # neworder
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/neworder)](https://pypi.org/project/neworder/)
 [![PyPI](https://img.shields.io/pypi/v/neworder)](https://pypi.org/project/neworder/)
 
 [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `neworder-1.4.1/neworder.egg-info/SOURCES.txt` & `neworder-1.4.2/neworder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/pyproject.toml` & `neworder-1.4.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,26 @@
     "pytest"
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neworder"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Andrew Smith", email="andrew@friarswood.net" },
 ]
 license = {file = "LICENCE.md"}
 description = "A dynamic microsimulation framework"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "pandas>=1.5.0",
   "pandas-stubs",
   "scipy>=1.9.3",
@@ -56,22 +57,22 @@
   "mkdocs-material>=9.0.2",
   "mkdocs-material-extensions>=1.1.1",
   "mkdocs-video>=1.3.0"
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://neworder.readthedocs.io/"
+"Bug Tracker" = "https://github.com/virgesmith/neworder/issues"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = [
     "test"
 ]
 
-[tool.ruff]
-select = ["E", "F"]
+[tool.ruff.lint]
+select = ["E", "F", "I"]
 ignore = ["E501"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "**/__init__.py" = ["F401", "F403"]
```

### Comparing `neworder-1.4.1/setup.py` & `neworder-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/ArrayHelpers.h` & `neworder-1.4.2/src/ArrayHelpers.h`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/DataFrame.cpp` & `neworder-1.4.2/src/DataFrame.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/DataFrame.h` & `neworder-1.4.2/src/DataFrame.h`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/Error.h` & `neworder-1.4.2/src/Error.h`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/Log.cpp` & `neworder-1.4.2/src/Log.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/Log.h` & `neworder-1.4.2/src/Log.h`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/Model.cpp` & `neworder-1.4.2/src/Model.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include "Log.h"
 #include "Error.h"
 #include "Helpers.h"
 
 #include <pybind11/pybind11.h>
 
 no::Model::Model(no::Timeline& timeline, const py::function& seeder)
-  : m_timeline(timeline), m_timeline_handle(py::cast(&timeline)),
+  : m_runState(no::Model::NOT_STARTED), m_timeline(timeline), m_timeline_handle(py::cast(&timeline)),
   m_monteCarlo(seeder().cast<int32_t>())
 {
   no::log("model init: timeline=%% mc=%%"s % m_timeline.repr() % m_monteCarlo.repr());
 }
 
 
 void no::Model::modify()
@@ -22,15 +22,15 @@
   // verbose only
   no::log("defaulted to no-op Model::modify()");
 }
 
 void no::Model::halt()
 {
   no::log("sending halt signal to Model::run()");
-  no::env::halt = true;
+  m_runState = Model::HALTED;
 }
 
 bool no::Model::check()
 {
   // verbose only
   no::log("defaulted to no-op Model::check()");
   return true;
@@ -52,26 +52,34 @@
     throw std::runtime_error("environment is not correctly initialised, model will not be run");
   }
 
   // access the timeline properties via the python object for consistency
   // (we can use the methods for C++ implementations, but not for python implementations)
   auto pytimeline = PyAccessor(model.timeline());
 
+  // check the model hasn't already completed
+  if (pytimeline.get_as<bool>("at_end")) {
+    throw py::stop_iteration("Model has already run to completion. Reinstantiate the timeline if necessary");
+  }
+
+  model.m_runState = no::Model::RUNNING;
+
   // get the Model class name
   const std::string& model_name = py::cast(&model).attr("__class__").attr("__name__").cast<std::string>();
 
-  no::log("starting %% model run. start time=%%"s % model_name % pytimeline.get("start"));
+
+  no::log("starting %% model run. start time=%%"s % model_name % pytimeline.get("time"));
 
   // apply the modifier, if implemented in the derived class
   no::log("t=%%(%%) %%.modify(%%)"s % pytimeline.get("time") % pytimeline.get("index") % model_name % rank);
   model.modify();
 
   // Loop over timeline
   bool ok = true;
-  while (!pytimeline.get_as<bool>("at_end"))
+  while (model.m_runState == Model::RUNNING)
   {
     py::object t = pytimeline.get("time");
     int64_t timeindex = pytimeline.get_as<int64_t>("index");
 
     // call the step method, then increment the timeline
     no::log("t=%%(%%) %%.step()"s % t % timeindex % model_name);
     model.step();
@@ -88,25 +96,24 @@
         // emit warning as well on failure (since the above message only appears when verbose mode is on)
         no::warn("check() FAILED in %%, halting model run at t=%%(%%)"s % model_name % t % timeindex);
         break;
       }
     }
 
     // check python hasn't signalled early termination
-    if (no::env::halt)
+    if (model.m_runState == no::Model::HALTED)
     {
       no::log("t=%%(%%) received halt signal"s % t % timeindex);
-      // reset the flag so that subsequent model runs don't halt immediately
-      no::env::halt = false;
-      break;
     }
-  }
-  // call the finalise method (if not explicitly halted mid-timeline)
-  if (pytimeline.get_as<bool>("at_end"))
-  {
-    no::log("t=%%(%%) %%.finalise()"s % pytimeline.get("time") % pytimeline.get("index") % model_name );
-    model.finalise();
+
+    // normal completion if not explicitly halted
+    if (model.m_runState == no::Model::RUNNING && pytimeline.get_as<bool>("at_end"))
+    {
+      model.m_runState = Model::COMPLETED;
+      no::log("t=%%(%%) %%.finalise()"s % pytimeline.get("time") % pytimeline.get("index") % model_name );
+      model.finalise();
+    }
   }
   no::log("%% exec time=%%s"s % (ok ? "SUCCESS": "ERRORED") % timer.elapsed_s());
   return ok;
 }
```

### Comparing `neworder-1.4.1/src/Model.h` & `neworder-1.4.2/src/Model.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 #pragma once
 
 #include "NewOrder.h"
 #include "Timeline.h"
 #include "MonteCarlo.h"
 #include "Module.h"
 
-namespace no {
-
-class Environment;
-
-class NEWORDER_EXPORT Model
+namespace no
 {
-public:
-  Model(no::Timeline& timeline, const py::function& seeder);
-
-  virtual ~Model() = default;
-
-  Model(const Model&) = delete;
-  Model& operator=(const Model&) = delete;
-  Model(Model&&) = delete;
-  Model& operator=(Model&&) = delete;
-
-  static bool run(Model& model);
-
-  // getters
-  Timeline& timeline() { return m_timeline; }
-  MonteCarlo& mc() { return m_monteCarlo; }
 
-  // functions to override
-  virtual void modify(); // optional, parallel runs only
-  virtual void step() = 0; // compulsory
-  virtual bool check(); // optional
-  virtual void finalise(); // optional
-
-  // set the halt flag
-  void halt();
-
-private:
-  Timeline& m_timeline;
-  py::object m_timeline_handle; // ensures above ref isnt deleted during the lifetime of this object
-  MonteCarlo m_monteCarlo;
-};
-
-
-class PyModel: private Model
-{
-  using Model::Model;
-  using Model::operator=;
+  class Environment;
 
-  // trampoline methods
-  void modify() override { PYBIND11_OVERRIDE(void, Model, modify); }
+  class NEWORDER_EXPORT Model
+  {
+  public:
+    // deliberately use pre-C++11 enum - scope will be e.g. Model::RUN
+    enum RunState
+    {
+      NOT_STARTED,
+      RUNNING,
+      HALTED, // immediate exit without calling finalise
+      COMPLETED // reached end of timeline, finalise called
+    };
+
+    Model(no::Timeline &timeline, const py::function &seeder);
+
+    virtual ~Model() = default;
+
+    Model(const Model &) = delete;
+    Model &operator=(const Model &) = delete;
+    Model(Model &&) = delete;
+    Model &operator=(Model &&) = delete;
+
+    static bool run(Model &model);
+
+    // getters
+    Timeline &timeline() { return m_timeline; }
+    MonteCarlo &mc() { return m_monteCarlo; }
+
+    // functions to override
+    virtual void modify();   // optional, parallel runs only
+    virtual void step() = 0; // compulsory
+    virtual bool check();    // optional
+    virtual void finalise(); // optional
+
+    // set the halt flag
+    void halt();
+
+    // get the run state
+    RunState runState() const { return m_runState; }
+
+  private:
+    RunState m_runState;
+    Timeline &m_timeline;
+    py::object m_timeline_handle; // ensures above ref isnt deleted during the lifetime of this object
+    MonteCarlo m_monteCarlo;
+  };
+
+  class PyModel : private Model
+  {
+    using Model::Model;
+    using Model::operator=;
+
+    // trampoline methods
+    void modify() override { PYBIND11_OVERRIDE(void, Model, modify); }
 
-  void step() override { PYBIND11_OVERRIDE_PURE(void, Model, step); }
+    void step() override { PYBIND11_OVERRIDE_PURE(void, Model, step); }
 
-  bool check() override { PYBIND11_OVERRIDE(bool, Model, check); }
+    bool check() override { PYBIND11_OVERRIDE(bool, Model, check); }
 
-  void finalise() override { PYBIND11_OVERRIDE(void, Model, finalise); }
-};
+    void finalise() override { PYBIND11_OVERRIDE(void, Model, finalise); }
+  };
 
 }
```

### Comparing `neworder-1.4.1/src/Module.cpp` & `neworder-1.4.2/src/Module.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 }
 
 // initially set to invalid values (so that if model is not properly initialised its immediately apparent)
 std::atomic_int no::env::rank = -1;
 std::atomic_int no::env::size = -1;
 std::atomic_bool no::env::verbose = false;
 std::atomic_bool no::env::checked = true;
-std::atomic_bool no::env::halt = false;
 std::atomic_int64_t no::env::uniqueIndex = -1;
 // these types are not trivially copyable so can't be atomic
 std::string no::env::logPrefix[2];
 
 
 void init_env(py::object mpi)
 {
@@ -77,17 +76,14 @@
 
   m.doc() = module_docstr;
 
   // time-related module
   auto time = m.def_submodule("time", time_docstr)
     .def("isnever", no::time::isnever, time_isnever_docstr, "t"_a) // scalar
     .def("isnever", no::time::isnever_a, time_isnever_a_docstr, "t"_a); // array
-    // .def("distant_past", no::time::distant_past, time_distant_past_docstr)
-    // .def("far_future", no::time::far_future, time_far_future_docstr)
-    // .def("never", no::time::never, time_never_docstr)
   time.attr("DISTANT_PAST") = no::time::distant_past();
   time.attr("FAR_FUTURE") = no::time::far_future();
   time.attr("NEVER") = no::time::never();
 
   // register abstract base class
   py::class_<no::Timeline, no::PyTimeline>(m, "Timeline")
     .def(py::init<>())
@@ -169,27 +165,35 @@
                            return self.next_arrival(startingpoints, lambda_t, dt, false, 0.0);
                          },
                          mc_next_arrival3_docstr,
                          "startingpoints"_a, "lambda_"_a, "dt"_a)
     .def("__repr__", &no::MonteCarlo::repr, mc_repr_docstr);
 
   // Microsimulation (or ABM) model class
-  py::class_<no::Model, no::PyModel>(m, "Model", model_docstr)
+  auto model = py::class_<no::Model, no::PyModel>(m, "Model", model_docstr)
     .def(py::init<no::Timeline&, const py::function&>(), model_init_docstr,"timeline"_a,
        "seeder"_a = py::cpp_function(no::MonteCarlo::deterministic_independent_stream))
     // properties are readonly only in the sense you can't assign to them; you CAN call their mutable methods
     .def_property_readonly("timeline", &no::Model::timeline, model_timeline_docstr)
     .def_property_readonly("mc", &no::Model::mc, model_mc_docstr)
+    .def_property_readonly("run_state", &no::Model::runState, model_runstate_docstr)
     .def("modify", &no::Model::modify, model_modify_docstr)
     .def("step", &no::Model::step, model_step_docstr)
     .def("check", &no::Model::check, model_check_docstr)
     .def("finalise", &no::Model::finalise, model_finalise_docstr)
     .def("halt", &no::Model::halt, model_halt_docstr);
     // NB the all-important run function is not exposed to python, it can only be executed via the `neworder.run` function
 
+  py::enum_<no::Model::RunState>(model, "RunState")
+  .value("NOT_STARTED", no::Model::NOT_STARTED)
+  .value("RUNNING", no::Model::RUNNING)
+  .value("HALTED", no::Model::HALTED)
+  .value("COMPLETED", no::Model::COMPLETED)
+  .export_values();
+
   // statistical utils
   m.def_submodule("stats", stats_docstr)
     .def("logistic", no::logistic,
                      stats_logistic_docstr,
                      "x"_a, "x0"_a, "k"_a)
     .def("logistic", [](const py::array_t<double>& a, double k) { return no::logistic(a, 0.0, k); },
                      stats_logistic_docstr_2,
```

### Comparing `neworder-1.4.1/src/Module.h` & `neworder-1.4.2/src/Module.h`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 // module-level attributes that should *not be modified directly* - call the env_init function. But note:
 // - python functions are exposed for modifying verbose and checked
 // - halt (if true) is reset in no::Model::run
 namespace env {
 
 extern std::atomic_bool verbose;
 extern std::atomic_bool checked;
-extern std::atomic_bool halt;
 extern std::atomic_int rank;
 extern std::atomic_int size;
 extern std::atomic_int64_t uniqueIndex;
 
 struct Context { enum Value { CPP, PY, SIZE }; };
 
 // strings are not trivially copyable so can't be atomic
```

### Comparing `neworder-1.4.1/src/Module_docstr.cpp` & `neworder-1.4.2/src/Module_docstr.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,21 @@
 
 const char* model_timeline_docstr = R"docstr(
     The model's timeline object
 )docstr";
 const char* model_mc_docstr = R"docstr(
     The model's Monte-Carlo engine
 )docstr";
+const char* model_runstate_docstr = R"docstr(
+    The model's current state - one of:
+        NOT_STARTED: model has not been run
+        RUNNING: model is in progress
+        HALTED: model has been explicitly halted by calling its halt() method
+        COMPLETED: model has run to the end of its timeline
+)docstr";
 const char* model_modify_docstr = R"docstr(
     User-overridable method used to modify state in a per-process basis for multiprocess model runs.
     Default behaviour is to do nothing.
     This function should not be called directly, it is used by the Model.run() function
 )docstr";
 const char* model_step_docstr = R"docstr(
     User-implemented method used to advance state of a model.
```

### Comparing `neworder-1.4.1/src/MonteCarlo.cpp` & `neworder-1.4.2/src/MonteCarlo.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/MonteCarlo.h` & `neworder-1.4.2/src/MonteCarlo.h`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/NPArray.cpp` & `neworder-1.4.2/src/NPArray.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/NPArray.h` & `neworder-1.4.2/src/NPArray.h`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/Timeline.cpp` & `neworder-1.4.2/src/Timeline.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/Timeline.h` & `neworder-1.4.2/src/Timeline.h`

 * *Files identical despite different names*

### Comparing `neworder-1.4.1/src/Timer.h` & `neworder-1.4.2/src/Timer.h`

 * *Files identical despite different names*

