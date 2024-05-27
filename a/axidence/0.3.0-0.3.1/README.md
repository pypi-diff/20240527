# Comparing `tmp/axidence-0.3.0.tar.gz` & `tmp/axidence-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axidence-0.3.0.tar", max compression
+gzip compressed data, was "axidence-0.3.1.tar", max compression
```

## Comparing `axidence-0.3.0.tar` & `axidence-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1522 2024-05-14 23:40:20.220815 axidence-0.3.0/LICENSE
--rw-r--r--   0        0        0     1046 2024-05-14 23:40:20.220815 axidence-0.3.0/README.md
--rw-r--r--   0        0        0      206 2024-05-14 23:40:20.220815 axidence-0.3.0/axidence/__init__.py
--rw-r--r--   0        0        0    11675 2024-05-14 23:40:20.220815 axidence-0.3.0/axidence/context.py
--rw-r--r--   0        0        0     2254 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/dtypes.py
--rw-r--r--   0        0        0     1376 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugin.py
--rw-r--r--   0        0        0      219 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/__init__.py
--rw-r--r--   0        0        0      261 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/__init__.py
--rw-r--r--   0        0        0     1001 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s1.py
--rw-r--r--   0        0        0     1146 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s2.py
--rw-r--r--   0        0        0      572 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cut_pairing_exists.py
--rw-r--r--   0        0        0     1001 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/cuts/cuts_event_building.py
--rw-r--r--   0        0        0      107 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/isolated/__init__.py
--rw-r--r--   0        0        0     1774 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/isolated/isolated_s1.py
--rw-r--r--   0        0        0     3098 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/isolated/isolated_s2.py
--rw-r--r--   0        0        0       47 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/meta/__init__.py
--rw-r--r--   0        0        0      500 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/meta/run_meta.py
--rw-r--r--   0        0        0      113 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/pairing/__init__.py
--rw-r--r--   0        0        0     7365 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/pairing/events_paired.py
--rw-r--r--   0        0        0    33605 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/pairing/peaks_paired.py
--rw-r--r--   0        0        0      353 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/__init__.py
--rw-r--r--   0        0        0     7993 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/event_building.py
--rw-r--r--   0        0        0     1422 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/event_combine.py
--rw-r--r--   0        0        0     2155 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/event_fields.py
--rw-r--r--   0        0        0     9693 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/events_salting.py
--rw-r--r--   0        0        0     4841 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/peak_correlation.py
--rw-r--r--   0        0        0     3148 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/plugins/salting/peaks_salted.py
--rw-r--r--   0        0        0     2035 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/samplers.py
--rw-r--r--   0        0        0     2685 2024-05-14 23:40:20.224815 axidence-0.3.0/axidence/utils.py
--rw-r--r--   0        0        0      933 2024-05-14 23:40:20.224815 axidence-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 axidence-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1522 2024-05-27 15:43:58.097395 axidence-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1040 2024-05-27 15:43:58.097395 axidence-0.3.1/README.md
+-rw-r--r--   0        0        0      183 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/__init__.py
+-rw-r--r--   0        0        0    11675 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/context.py
+-rw-r--r--   0        0        0     2254 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/dtypes.py
+-rw-r--r--   0        0        0      219 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/cuts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/cuts/cut_isolated_s1.py
+-rw-r--r--   0        0        0     1146 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/cuts/cut_isolated_s2.py
+-rw-r--r--   0        0        0      572 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/cuts/cut_pairing_exists.py
+-rw-r--r--   0        0        0     1001 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/cuts/cuts_event_building.py
+-rw-r--r--   0        0        0      107 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/isolated/__init__.py
+-rw-r--r--   0        0        0     1774 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/isolated/isolated_s1.py
+-rw-r--r--   0        0        0     3098 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/isolated/isolated_s2.py
+-rw-r--r--   0        0        0       47 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/meta/__init__.py
+-rw-r--r--   0        0        0      500 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/meta/run_meta.py
+-rw-r--r--   0        0        0      113 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/pairing/__init__.py
+-rw-r--r--   0        0        0     7365 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/pairing/events_paired.py
+-rw-r--r--   0        0        0    33605 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/pairing/peaks_paired.py
+-rw-r--r--   0        0        0      353 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/salting/__init__.py
+-rw-r--r--   0        0        0     7993 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/salting/event_building.py
+-rw-r--r--   0        0        0     1422 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/salting/event_combine.py
+-rw-r--r--   0        0        0     2155 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/salting/event_fields.py
+-rw-r--r--   0        0        0    10118 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/salting/events_salting.py
+-rw-r--r--   0        0        0     4841 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/salting/peak_correlation.py
+-rw-r--r--   0        0        0     3148 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/plugins/salting/peaks_salted.py
+-rw-r--r--   0        0        0     2035 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/samplers.py
+-rw-r--r--   0        0        0     2685 2024-05-27 15:43:58.097395 axidence-0.3.1/axidence/utils.py
+-rw-r--r--   0        0        0      932 2024-05-27 15:43:58.101395 axidence-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 axidence-0.3.1/PKG-INFO
```

### Comparing `axidence-0.3.0/LICENSE` & `axidence-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/context.py` & `axidence-0.3.1/axidence/context.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/dtypes.py` & `axidence-0.3.1/axidence/dtypes.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s1.py` & `axidence-0.3.1/axidence/plugins/cuts/cut_isolated_s1.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/cuts/cut_isolated_s2.py` & `axidence-0.3.1/axidence/plugins/cuts/cut_isolated_s2.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/cuts/cut_pairing_exists.py` & `axidence-0.3.1/axidence/plugins/cuts/cut_pairing_exists.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/cuts/cuts_event_building.py` & `axidence-0.3.1/axidence/plugins/cuts/cuts_event_building.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/isolated/isolated_s1.py` & `axidence-0.3.1/axidence/plugins/isolated/isolated_s1.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/isolated/isolated_s2.py` & `axidence-0.3.1/axidence/plugins/isolated/isolated_s2.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/pairing/events_paired.py` & `axidence-0.3.1/axidence/plugins/pairing/events_paired.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/pairing/peaks_paired.py` & `axidence-0.3.1/axidence/plugins/pairing/peaks_paired.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/salting/event_building.py` & `axidence-0.3.1/axidence/plugins/salting/event_building.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/salting/event_combine.py` & `axidence-0.3.1/axidence/plugins/salting/event_combine.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/salting/event_fields.py` & `axidence-0.3.1/axidence/plugins/salting/event_fields.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/salting/events_salting.py` & `axidence-0.3.1/axidence/plugins/salting/events_salting.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,26 @@
 
     veto_length_run_end = straxen.URLConfig(
         default=10**8,
         type=int,
         help="Min time delay in [ns] for events towards the run end boundary",
     )
 
+    min_drift_length = straxen.URLConfig(
+        default=0,
+        type=(int, float),
+        help="Manually set minimum length of drifting [cm]",
+    )
+
+    max_drift_length = straxen.URLConfig(
+        default=straxen.tpc_z,
+        infer_type=False,
+        help="Total length of the TPC from the bottom of gate to the top of cathode wires [cm]",
+    )
+
     assigned_area_fraction_top = straxen.URLConfig(
         default=1.0,
         type=(int, float, None),
         help="Assigned area fraction top for S2",
     )
 
     n_drift_time_window = straxen.URLConfig(
@@ -191,15 +203,16 @@
             self.events_salting["s1_n_hits"][indices] = 3
             self.events_salting["s1_tight_coincidence"][indices] = 3
 
         theta = self.rng.random(size=self.n_events) * 2 * np.pi - np.pi
         r = np.sqrt(self.rng.random(size=self.n_events)) * straxen.tpc_r
         self.events_salting["x"] = np.cos(theta) * r
         self.events_salting["y"] = np.sin(theta) * r
-        self.events_salting["z"] = -self.rng.random(size=self.n_events) * straxen.tpc_z
+        self.events_salting["z"] = -self.rng.random(size=self.n_events)
+        self.events_salting["z"] *= self.max_drift_length - self.min_drift_length
         s2_x, s2_y, z_naive = self.inverse_field_distortion(
             self.events_salting["x"],
             self.events_salting["y"],
             self.events_salting["z"],
         )
         self.events_salting["s2_x"] = s2_x
         self.events_salting["s2_y"] = s2_y
```

### Comparing `axidence-0.3.0/axidence/plugins/salting/peak_correlation.py` & `axidence-0.3.1/axidence/plugins/salting/peak_correlation.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/plugins/salting/peaks_salted.py` & `axidence-0.3.1/axidence/plugins/salting/peaks_salted.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/samplers.py` & `axidence-0.3.1/axidence/samplers.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/axidence/utils.py` & `axidence-0.3.1/axidence/utils.py`

 * *Files identical despite different names*

### Comparing `axidence-0.3.0/pyproject.toml` & `axidence-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "axidence"
-version = "0.3.0"
+version = "0.3.1"
 description = "strax-based data-driven accidental coincidence background simulation and peak-level salting"
 readme = "README.md"
 license = "BSD-3-Clause"
 authors = [
   "Dacheng Xu, <dx2227@columbia.edu>",
 ]
 requires-python = ">=3.9"
@@ -14,15 +14,15 @@
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Physics",
 ]
-repository = "https://github.com/dachengx/axidence"
+repository = "https://github.com/XENONnT/axidence"
 documentation = "https://readthedocs.org/projects/axidence/"
 
 [tool.poetry.dependencies]
 strax = ">=1.6.3"
 straxen = ">=2.2.1"
 GOFevaluation = ">=0.1.4"
```

### Comparing `axidence-0.3.0/PKG-INFO` & `axidence-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: axidence
-Version: 0.3.0
+Version: 0.3.1
 Summary: strax-based data-driven accidental coincidence background simulation and peak-level salting
-Home-page: https://github.com/dachengx/axidence
+Home-page: https://github.com/XENONnT/axidence
 License: BSD-3-Clause
 Author: Dacheng Xu,
 Author-email: dx2227@columbia.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2
@@ -23,24 +23,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: GOFevaluation (>=0.1.4)
 Requires-Dist: strax (>=1.6.3)
 Requires-Dist: straxen (>=2.2.1)
 Project-URL: Documentation, https://readthedocs.org/projects/axidence/
-Project-URL: Repository, https://github.com/dachengx/axidence
+Project-URL: Repository, https://github.com/XENONnT/axidence
 Description-Content-Type: text/markdown
 
 # Axidence
 
-[![Test package](https://github.com/dachengx/axidence/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/dachengx/axidence/actions/workflows/pytest.yml)
-[![Coverage Status](https://coveralls.io/repos/github/dachengx/axidence/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/dachengx/axidence?branch=main&kill_cache=1)
+[![Test package](https://github.com/XENONnT/axidence/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/XENONnT/axidence/actions/workflows/pytest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/XENONnT/axidence/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/XENONnT/axidence?branch=main&kill_cache=1)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/axidence.svg)](https://pypi.python.org/pypi/axidence/)
 [![Documentation Status](https://readthedocs.org/projects/axidence/badge/?version=latest)](https://axidence.readthedocs.io/en/latest/?badge=latest)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/dachengx/axidence/main.svg)](https://results.pre-commit.ci/latest/github/dachengx/axidence/main)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/XENONnT/axidence/main.svg)](https://results.pre-commit.ci/latest/github/XENONnT/axidence/main)
 
 Axidence is a stax-based data-driven accidental coincidence background simulation framework. It can also perform the peak-level salting to calculate the features related to ambient environment.
 
 # Installation
 ```
 cd axidence
 pip install ./ --user
```

