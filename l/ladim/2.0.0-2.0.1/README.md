# Comparing `tmp/ladim-2.0.0.tar.gz` & `tmp/ladim-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladim-2.0.0.tar", last modified: Wed Mar 20 12:02:29 2024, max compression
+gzip compressed data, was "ladim-2.0.1.tar", last modified: Mon May 27 06:30:16 2024, max compression
```

## Comparing `ladim-2.0.0.tar` & `ladim-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.092685 ladim-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-20 12:02:21.000000 ladim-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-20 12:02:29.092685 ladim-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-20 12:02:21.000000 ladim-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.088685 ladim-2.0.0/ladim/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/forcing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.088685 ladim-2.0.0/ladim/gridforce/
--rw-r--r--   0 runner    (1001) docker     (127)    26888 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/gridforce/ROMS.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/gridforce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/gridforce/analytical.py
--rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/gridforce/zROMS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.088685 ladim-2.0.0/ladim/ibms/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/ibms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/ibms/light.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2812 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.088685 ladim-2.0.0/ladim/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-20 12:02:21.000000 ladim-2.0.0/ladim/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.092685 ladim-2.0.0/ladim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-20 12:02:29.000000 ladim-2.0.0/ladim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-20 12:02:29.000000 ladim-2.0.0/ladim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 12:02:29.000000 ladim-2.0.0/ladim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-20 12:02:29.000000 ladim-2.0.0/ladim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-20 12:02:29.000000 ladim-2.0.0/ladim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 12:02:29.000000 ladim-2.0.0/ladim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.088685 ladim-2.0.0/postladim/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-20 12:02:21.000000 ladim-2.0.0/postladim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-20 12:02:21.000000 ladim-2.0.0/postladim/cellcount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-20 12:02:21.000000 ladim-2.0.0/postladim/kde_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-03-20 12:02:21.000000 ladim-2.0.0/postladim/particlefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-03-20 12:02:21.000000 ladim-2.0.0/postladim/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-20 12:02:21.000000 ladim-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-20 12:02:29.092685 ladim-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:02:29.092685 ladim-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-20 12:02:21.000000 ladim-2.0.0/tests/test_ladim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-03-20 12:02:21.000000 ladim-2.0.0/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-20 12:02:21.000000 ladim-2.0.0/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-20 12:02:21.000000 ladim-2.0.0/tests/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.672659 ladim-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-27 06:30:12.000000 ladim-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-27 06:30:16.672659 ladim-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-27 06:30:12.000000 ladim-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.668659 ladim-2.0.1/ladim/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/forcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.672659 ladim-2.0.1/ladim/gridforce/
+-rw-r--r--   0 runner    (1001) docker     (127)    26888 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/gridforce/ROMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/gridforce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/gridforce/analytical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/gridforce/zROMS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.672659 ladim-2.0.1/ladim/ibms/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/ibms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/ibms/light.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2812 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.672659 ladim-2.0.1/ladim/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-27 06:30:12.000000 ladim-2.0.1/ladim/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.672659 ladim-2.0.1/ladim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-27 06:30:16.000000 ladim-2.0.1/ladim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 06:30:16.000000 ladim-2.0.1/ladim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:30:16.000000 ladim-2.0.1/ladim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-27 06:30:16.000000 ladim-2.0.1/ladim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 06:30:16.000000 ladim-2.0.1/ladim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 06:30:16.000000 ladim-2.0.1/ladim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.672659 ladim-2.0.1/postladim/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-27 06:30:12.000000 ladim-2.0.1/postladim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-27 06:30:12.000000 ladim-2.0.1/postladim/cellcount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-27 06:30:12.000000 ladim-2.0.1/postladim/kde_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-27 06:30:12.000000 ladim-2.0.1/postladim/particlefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-27 06:30:12.000000 ladim-2.0.1/postladim/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 06:30:12.000000 ladim-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-27 06:30:16.672659 ladim-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:30:16.672659 ladim-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-27 06:30:12.000000 ladim-2.0.1/tests/test_ladim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-27 06:30:12.000000 ladim-2.0.1/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-27 06:30:12.000000 ladim-2.0.1/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-27 06:30:12.000000 ladim-2.0.1/tests/test_solver.py
```

### Comparing `ladim-2.0.0/LICENSE` & `ladim-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/PKG-INFO` & `ladim-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladim
-Version: 2.0.0
+Version: 2.0.1
 Summary: Lagrangian Advection and Diffusion Model
 Home-page: https://github.com/pnsaevik/ladim
 Author: Bjørn Ådlandsvik
 Author-email: bjorn@imr.no
 Maintainer: Pål Næverlid Sævik
 Maintainer-email: paal.naeverlid.saevik@hi.no
 License: MIT
```

### Comparing `ladim-2.0.0/README.md` & `ladim-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/config.py` & `ladim-2.0.1/ladim/config.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/forcing.py` & `ladim-2.0.1/ladim/forcing.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/grid.py` & `ladim-2.0.1/ladim/grid.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/gridforce/ROMS.py` & `ladim-2.0.1/ladim/gridforce/ROMS.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/gridforce/analytical.py` & `ladim-2.0.1/ladim/gridforce/analytical.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/gridforce/zROMS.py` & `ladim-2.0.1/ladim/gridforce/zROMS.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/ibms/__init__.py` & `ladim-2.0.1/ladim/ibms/__init__.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/ibms/light.py` & `ladim-2.0.1/ladim/ibms/light.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/main.py` & `ladim-2.0.1/ladim/main.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/model.py` & `ladim-2.0.1/ladim/model.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/output.py` & `ladim-2.0.1/ladim/output.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/release.py` & `ladim-2.0.1/ladim/release.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         # Release file
         self._csv_fname = file   # Path name
         self._csv_column_names = colnames   # Column headers
         self._csv_column_formats = formats or dict()
         self._dataframe = None
 
         # Continuous release variables
-        self._frequency = read_timedelta(frequency)
+        self._frequency = read_timedelta(frequency) / np.timedelta64(1, 's')
         self._last_release_dataframe = pd.DataFrame()
         self._last_release_time = np.int64(-4611686018427387904)
 
         # Other parameters
         self._defaults = defaults or dict()
 
     def update(self):
@@ -76,14 +76,20 @@
         # current simulation time
         df = release_data_subset(
             dataframe=self.dataframe,
             start_time=self.model.solver.time,
             stop_time=self.model.solver.time + self.model.solver.step,
         ).copy(deep=True)
 
+        # If there are no new particles, but the state is empty, we should
+        # still initialize the state by adding the appropriate columns
+        if (len(df) == 0) and ('X' not in self.model.state):
+            self.model.state.append(df.to_dict(orient='list'))
+            self._last_release_dataframe = df
+
         # If there are no new particles and we don't use continuous release,
         # we are done.
         continuous_release = bool(self._frequency)
         if (len(df) == 0) and not continuous_release:
             return
 
         # If we have continuous release, but there are no new particles and
@@ -95,15 +101,15 @@
             return
 
         # If we are at the final time step, we should not release any more particles
         if continuous_release and self.model.solver.time >= self.model.solver.stop:
             return
 
         # If we have continuous release, but there are no new particles and
-        # the last release is NOT recent, we should replace the empty
+        # the last release is NOT recent, we should replace empty
         # dataframe with the previously released dataframe
         if continuous_release:
             if (len(df) == 0) and not last_release_is_recent:
                 df = self._last_release_dataframe
             self._last_release_dataframe = df  # Update release dataframe
             self._last_release_time = current_time
 
@@ -144,14 +150,15 @@
                     yield f
 
         if self._dataframe is None:
             if isinstance(self._csv_fname, pd.DataFrame):
                 self._dataframe = self._csv_fname
 
             else:
+                # noinspection PyArgumentList
                 with open_or_relay(self._csv_fname, 'r', encoding='utf-8') as fp:
                     self._dataframe = load_release_file(
                         stream=fp,
                         names=self._csv_column_names,
                         formats=self._csv_column_formats,
                     )
         return self._dataframe
```

### Comparing `ladim-2.0.0/ladim/sample.py` & `ladim-2.0.1/ladim/sample.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/solver.py` & `ladim-2.0.1/ladim/solver.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/state.py` & `ladim-2.0.1/ladim/state.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/tracker.py` & `ladim-2.0.1/ladim/tracker.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim/utilities.py` & `ladim-2.0.1/ladim/utilities.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/ladim.egg-info/PKG-INFO` & `ladim-2.0.1/ladim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladim
-Version: 2.0.0
+Version: 2.0.1
 Summary: Lagrangian Advection and Diffusion Model
 Home-page: https://github.com/pnsaevik/ladim
 Author: Bjørn Ådlandsvik
 Author-email: bjorn@imr.no
 Maintainer: Pål Næverlid Sævik
 Maintainer-email: paal.naeverlid.saevik@hi.no
 License: MIT
```

### Comparing `ladim-2.0.0/ladim.egg-info/SOURCES.txt` & `ladim-2.0.1/ladim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 ladim/__init__.py
+ladim/__main__.py
 ladim/config.py
 ladim/forcing.py
 ladim/grid.py
 ladim/main.py
 ladim/model.py
 ladim/output.py
 ladim/release.py
```

### Comparing `ladim-2.0.0/postladim/cellcount.py` & `ladim-2.0.1/postladim/cellcount.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/postladim/kde_plot.py` & `ladim-2.0.1/postladim/kde_plot.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/postladim/particlefile.py` & `ladim-2.0.1/postladim/particlefile.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/postladim/variable.py` & `ladim-2.0.1/postladim/variable.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/setup.cfg` & `ladim-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/tests/test_ladim.py` & `ladim-2.0.1/tests/test_ladim.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/tests/test_output.py` & `ladim-2.0.1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `ladim-2.0.0/tests/test_solver.py` & `ladim-2.0.1/tests/test_solver.py`

 * *Files identical despite different names*

