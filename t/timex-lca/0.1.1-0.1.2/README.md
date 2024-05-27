# Comparing `tmp/timex_lca-0.1.1.tar.gz` & `tmp/timex_lca-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timex_lca-0.1.1.tar", last modified: Sun May  5 08:57:55 2024, max compression
+gzip compressed data, was "timex_lca-0.1.2.tar", last modified: Mon May 27 20:58:03 2024, max compression
```

## Comparing `timex_lca-0.1.1.tar` & `timex_lca-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:57:55.310716 timex_lca-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-05 08:57:51.000000 timex_lca-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-05 08:57:55.310716 timex_lca-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-05 08:57:51.000000 timex_lca-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:57:55.306716 timex_lca-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 08:57:51.000000 timex_lca-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-05 08:57:51.000000 timex_lca-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:57:55.310716 timex_lca-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 08:57:51.000000 timex_lca-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:57:55.306716 timex_lca-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-05 08:57:51.000000 timex_lca-0.1.1/tests/test_amounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-05 08:57:51.000000 timex_lca-0.1.1/tests/test_bioflows.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 08:57:51.000000 timex_lca-0.1.1/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    20945 2024-05-05 08:57:51.000000 timex_lca-0.1.1/tests/test_temporal_distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-05 08:57:51.000000 timex_lca-0.1.1/tests/test_temporal_groupings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:57:55.306716 timex_lca-0.1.1/timex_lca/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:57:55.306716 timex_lca-0.1.1/timex_lca/data/
--rw-r--r--   0 runner    (1001) docker     (127)    69114 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/data/hodnebrog20.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/dynamic_biosphere_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    35436 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/dynamic_characterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/edge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/matrix_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/remapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/timeline_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    49116 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/timex_lca.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-05 08:57:51.000000 timex_lca-0.1.1/timex_lca/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:57:55.306716 timex_lca-0.1.1/timex_lca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-05 08:57:55.000000 timex_lca-0.1.1/timex_lca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-05 08:57:55.000000 timex_lca-0.1.1/timex_lca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:57:55.000000 timex_lca-0.1.1/timex_lca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-05 08:57:55.000000 timex_lca-0.1.1/timex_lca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 08:57:55.000000 timex_lca-0.1.1/timex_lca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:02.998918 timex_lca-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-27 20:57:59.000000 timex_lca-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-27 20:58:02.998918 timex_lca-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-27 20:57:59.000000 timex_lca-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:02.994918 timex_lca-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 20:57:59.000000 timex_lca-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-27 20:57:59.000000 timex_lca-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:58:02.998918 timex_lca-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-27 20:57:59.000000 timex_lca-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:02.994918 timex_lca-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-27 20:57:59.000000 timex_lca-0.1.2/tests/test_amounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-27 20:57:59.000000 timex_lca-0.1.2/tests/test_bioflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 20:57:59.000000 timex_lca-0.1.2/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20945 2024-05-27 20:57:59.000000 timex_lca-0.1.2/tests/test_temporal_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14257 2024-05-27 20:57:59.000000 timex_lca-0.1.2/tests/test_temporal_groupings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:02.994918 timex_lca-0.1.2/timex_lca/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:02.994918 timex_lca-0.1.2/timex_lca/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    69114 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/data/hodnebrog20.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/dynamic_biosphere_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35436 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/dynamic_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/edge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/matrix_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/remapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19465 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/timeline_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49116 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/timex_lca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-27 20:57:59.000000 timex_lca-0.1.2/timex_lca/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:58:02.998918 timex_lca-0.1.2/timex_lca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-27 20:58:02.000000 timex_lca-0.1.2/timex_lca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-27 20:58:02.000000 timex_lca-0.1.2/timex_lca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:58:02.000000 timex_lca-0.1.2/timex_lca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-27 20:58:02.000000 timex_lca-0.1.2/timex_lca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 20:58:02.000000 timex_lca-0.1.2/timex_lca.egg-info/top_level.txt
```

### Comparing `timex_lca-0.1.1/LICENSE` & `timex_lca-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/PKG-INFO` & `timex_lca-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timex_lca
-Version: 0.1.1
+Version: 0.1.2
 Summary: Time-explicit Life Cycle Assessment
 Author: Amelie Müller, Arthur Jakobs
 Author-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Maintainer: Amelie Müller
 Maintainer-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Project-URL: source, https://github.com/TimoDiepers/timex
 Project-URL: homepage, https://github.com/TimoDiepers/timex
@@ -77,7 +77,12 @@
 - [Installation Guide](https://timex.readthedocs.io/en/latest/content/installation.html)
 - [Example Notebook](https://github.com/TimoDiepers/timex/blob/main/notebooks/example_setac.ipynb)
 
 ## Contributing:
 We welcome contributions! If you have suggestions or want to fix a bug, please:
 - [Open an Issue](https://github.com/TimoDiepers/timex/issues)
 - [Send a Pull Request](https://github.com/TimoDiepers/timex/pulls)
+
+## Support: 
+If you have any questions or need help, do not hesitate to contact us:
+- Timo Diepers ([timo.diepers@ltt.rwth-aachen.de](mailto:timo.diepers@ltt.rwth-aachen.de))
+- Amelie Müller ([a.muller@cml.leidenuniv.nl](mailto:a.muller@cml.leidenuniv.nl))
```

### Comparing `timex_lca-0.1.1/README.md` & `timex_lca-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,7 +33,12 @@
 - [Installation Guide](https://timex.readthedocs.io/en/latest/content/installation.html)
 - [Example Notebook](https://github.com/TimoDiepers/timex/blob/main/notebooks/example_setac.ipynb)
 
 ## Contributing:
 We welcome contributions! If you have suggestions or want to fix a bug, please:
 - [Open an Issue](https://github.com/TimoDiepers/timex/issues)
 - [Send a Pull Request](https://github.com/TimoDiepers/timex/pulls)
+
+## Support: 
+If you have any questions or need help, do not hesitate to contact us:
+- Timo Diepers ([timo.diepers@ltt.rwth-aachen.de](mailto:timo.diepers@ltt.rwth-aachen.de))
+- Amelie Müller ([a.muller@cml.leidenuniv.nl](mailto:a.muller@cml.leidenuniv.nl))
```

### Comparing `timex_lca-0.1.1/pyproject.toml` & `timex_lca-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/tests/test_amounts.py` & `timex_lca-0.1.2/tests/test_amounts.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/tests/test_bioflows.py` & `timex_lca-0.1.2/tests/test_bioflows.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/tests/test_temporal_distributions.py` & `timex_lca-0.1.2/tests/test_temporal_distributions.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/tests/test_temporal_groupings.py` & `timex_lca-0.1.2/tests/test_temporal_groupings.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/data/hodnebrog20.csv` & `timex_lca-0.1.2/timex_lca/data/hodnebrog20.csv`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/dynamic_biosphere_builder.py` & `timex_lca-0.1.2/timex_lca/dynamic_biosphere_builder.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/dynamic_characterization.py` & `timex_lca-0.1.2/timex_lca/dynamic_characterization.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/edge_extractor.py` & `timex_lca-0.1.2/timex_lca/edge_extractor.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/matrix_modifier.py` & `timex_lca-0.1.2/timex_lca/matrix_modifier.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/remapping.py` & `timex_lca-0.1.2/timex_lca/remapping.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/timeline_builder.py` & `timex_lca-0.1.2/timex_lca/timeline_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,26 +82,21 @@
             ]
             if node_id
             not in self.node_id_collection_dict[
                 "first_level_background_node_ids_static"
             ]
         ]
 
-        # The graph traversal needs the matrix indices, not the database / node indices.
-        static_activity_matrix_indices = [
-            self.slca.dicts.product[node_id] for node_id in static_activity_db_indices
-        ]
-
         self.edge_extractor = EdgeExtractor(
             slca,
             *args,
             edge_filter_function=edge_filter_function,
             cutoff=self.cutoff,
             max_calc=self.max_calc,
-            static_activity_indices=set(static_activity_matrix_indices),
+            static_activity_indices=set(static_activity_db_indices),
             **kwargs,
         )
         self.edge_timeline = self.edge_extractor.build_edge_timeline()
 
     def check_database_names(self) -> None:
         """
         Check that the strings of the databases exist in the databases of the brightway project.
```

### Comparing `timex_lca-0.1.1/timex_lca/timex_lca.py` & `timex_lca-0.1.2/timex_lca/timex_lca.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca/utils.py` & `timex_lca-0.1.2/timex_lca/utils.py`

 * *Files identical despite different names*

### Comparing `timex_lca-0.1.1/timex_lca.egg-info/PKG-INFO` & `timex_lca-0.1.2/timex_lca.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timex_lca
-Version: 0.1.1
+Version: 0.1.2
 Summary: Time-explicit Life Cycle Assessment
 Author: Amelie Müller, Arthur Jakobs
 Author-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Maintainer: Amelie Müller
 Maintainer-email: Timo Diepers <timo.diepers@ltt.rwth-aachen.de>
 Project-URL: source, https://github.com/TimoDiepers/timex
 Project-URL: homepage, https://github.com/TimoDiepers/timex
@@ -77,7 +77,12 @@
 - [Installation Guide](https://timex.readthedocs.io/en/latest/content/installation.html)
 - [Example Notebook](https://github.com/TimoDiepers/timex/blob/main/notebooks/example_setac.ipynb)
 
 ## Contributing:
 We welcome contributions! If you have suggestions or want to fix a bug, please:
 - [Open an Issue](https://github.com/TimoDiepers/timex/issues)
 - [Send a Pull Request](https://github.com/TimoDiepers/timex/pulls)
+
+## Support: 
+If you have any questions or need help, do not hesitate to contact us:
+- Timo Diepers ([timo.diepers@ltt.rwth-aachen.de](mailto:timo.diepers@ltt.rwth-aachen.de))
+- Amelie Müller ([a.muller@cml.leidenuniv.nl](mailto:a.muller@cml.leidenuniv.nl))
```

### Comparing `timex_lca-0.1.1/timex_lca.egg-info/SOURCES.txt` & `timex_lca-0.1.2/timex_lca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

