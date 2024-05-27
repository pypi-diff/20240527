# Comparing `tmp/chemfeat-2023.9.tar.gz` & `tmp/chemfeat-2024.1.tar.gz`

## Comparing `chemfeat-2023.9.tar` & `chemfeat-2024.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 chemfeat-2023.9/.gitlab-ci.yml
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 chemfeat-2023.9/codemeta.json
--rw-r--r--   0        0        0   178830 2020-02-02 00:00:00.000000 chemfeat-2023.9/features.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/requirements.txt
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/source/chemfeat.features.calculators.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/source/chemfeat.features.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/source/chemfeat.rst
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/source/conf.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/source/index.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/source/modules.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfeat-2023.9/doc/source/readme.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 chemfeat-2023.9/img/chemfeat_icon.svg
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 chemfeat-2023.9/img/chemfeat_logo.svg
--rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 chemfeat-2023.9/scripts/build_documentation.sh
--rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 chemfeat-2023.9/scripts/generate_doc_mds.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/__init__.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/csv_wrapper.py
--rw-r--r--   0        0        0    16660 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/database.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/main.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/markdown.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/modules.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/version.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/__init__.py
--rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculator.py
--rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/manager.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculators/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculators/ecfp.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculators/padel.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculators/qed.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculators/rdkdesc.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculators/rdkfp.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 chemfeat-2023.9/src/chemfeat/features/calculators/secfp.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chemfeat-2023.9/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 chemfeat-2023.9/LICENSE.txt
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 chemfeat-2023.9/README.md
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 chemfeat-2023.9/pyproject.toml
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 chemfeat-2023.9/PKG-INFO
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 chemfeat-2024.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 chemfeat-2024.1/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/requirements.txt
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/source/chemfeat.features.calculators.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/source/chemfeat.features.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/source/chemfeat.rst
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/source/conf.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/source/index.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/source/modules.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfeat-2024.1/doc/source/readme.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 chemfeat-2024.1/img/chemfeat_icon.svg
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 chemfeat-2024.1/img/chemfeat_logo.svg
+-rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 chemfeat-2024.1/scripts/build_documentation.sh
+-rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 chemfeat-2024.1/scripts/generate_doc_mds.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/__init__.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/csv_wrapper.py
+-rw-r--r--   0        0        0    16660 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/database.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/main.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/markdown.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/modules.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/version.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/__init__.py
+-rw-r--r--   0        0        0     7500 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculator.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/manager.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculators/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculators/ecfp.py
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculators/padel.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculators/qed.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculators/rdkdesc.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculators/rdkfp.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 chemfeat-2024.1/src/chemfeat/features/calculators/secfp.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chemfeat-2024.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 chemfeat-2024.1/LICENSE.txt
+-rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 chemfeat-2024.1/README.md
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 chemfeat-2024.1/pyproject.toml
+-rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 chemfeat-2024.1/PKG-INFO
```

### Comparing `chemfeat-2023.9/codemeta.json` & `chemfeat-2024.1/codemeta.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5714285714285714%*

 * *Differences: {"'author'": "[OrderedDict([('@id', 'https://orcid.org/0009-0005-0109-6598'), ('@type', 'Person'), "*

 * *             "('email', 'jan-michael.rye@inria.fr'), ('familyName', 'Rye'), ('givenName', "*

 * *             "'Jan-Michael')])]",*

 * * "'codeRepository'": "'https://gitlab.inria.fr/jrye/chemfeat.git'",*

 * * "'contributor'": "[OrderedDict([('@id', 'https://orcid.org/0009-0005-0109-6598'), ('@type', "*

 * *                  "'Person'), ('email', 'jan-michael.rye@inria.fr'), ('familyName', 'Rye'), "*

 * *                  "('givenNa […]*

```diff
@@ -3,24 +3,50 @@
         "https://doi.org/10.5063/schema/codemeta-2.0",
         "https://w3id.org/software-iodata",
         "https://raw.githubusercontent.com/jantman/repostatus.org/master/badges/latest/ontology.jsonld",
         "https://schema.org",
         "https://w3id.org/software-types"
     ],
     "@type": "SoftwareSourceCode",
-    "author": "Jan-Michael Rye",
-    "codeRepository": "https://gitlab.inria.fr/jrye/chemfeat",
+    "author": [
+        {
+            "@id": "https://orcid.org/0009-0005-0109-6598",
+            "@type": "Person",
+            "email": "jan-michael.rye@inria.fr",
+            "familyName": "Rye",
+            "givenName": "Jan-Michael"
+        }
+    ],
+    "codeRepository": "https://gitlab.inria.fr/jrye/chemfeat.git",
+    "contributor": [
+        {
+            "@id": "https://orcid.org/0009-0005-0109-6598",
+            "@type": "Person",
+            "email": "jan-michael.rye@inria.fr",
+            "familyName": "Rye",
+            "givenName": "Jan-Michael"
+        }
+    ],
     "description": "Calculate feature vectors for molecules using cheminformatics libraries.",
-    "email": "jan-michael.rye@inria.fr",
     "identifier": "chemfeat",
+    "issueTracker": "https://gitlab.inria.fr/jrye/chemfeat/-/issues",
     "license": "http://spdx.org/licenses/MIT",
+    "maintainer": {
+        "@id": "https://orcid.org/0009-0005-0109-6598",
+        "@type": "Person",
+        "email": "jan-michael.rye@inria.fr",
+        "familyName": "Rye",
+        "givenName": "Jan-Michael"
+    },
     "name": "chemfeat",
     "operatingSystem": "OS Independent",
+    "programmingLanguage": "Python",
+    "readme": "https://gitlab.inria.fr/jrye/chemfeat/-/blob/main/README.md",
     "runtimePlatform": "Python 3",
-    "softwareHelp": "https://jrye.gitlabpages.inria.fr/chemfeat/",
+    "softwareHelp": "https://jrye.gitlabpages.inria.fr/chemfeat",
     "softwareRequirements": [
         {
             "@type": "SoftwareApplication",
             "identifier": "docstring-parser",
             "name": "docstring-parser",
             "runtimePlatform": "Python 3"
         },
@@ -58,9 +84,10 @@
     "targetProduct": {
         "@type": "CommandLineApplication",
         "description": "\nCommand-line utility for calculating chemical features.\n",
         "executableName": "chemfeat",
         "name": "chemfeat",
         "runtimePlatform": "Python 3"
     },
-    "version": "2023.9.post1.dev0"
+    "url": "https://gitlab.inria.fr/jrye/chemfeat",
+    "version": "2024.1"
 }
```

### Comparing `chemfeat-2023.9/doc/Makefile` & `chemfeat-2024.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/doc/make.bat` & `chemfeat-2024.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/doc/source/chemfeat.features.calculators.rst` & `chemfeat-2024.1/doc/source/chemfeat.features.calculators.rst`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/doc/source/chemfeat.features.rst` & `chemfeat-2024.1/doc/source/chemfeat.features.rst`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/doc/source/chemfeat.rst` & `chemfeat-2024.1/doc/source/chemfeat.rst`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/doc/source/conf.py` & `chemfeat-2024.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/img/chemfeat_icon.svg` & `chemfeat-2024.1/img/chemfeat_icon.svg`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/img/chemfeat_logo.svg` & `chemfeat-2024.1/img/chemfeat_logo.svg`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/scripts/build_documentation.sh` & `chemfeat-2024.1/scripts/build_documentation.sh`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/scripts/generate_doc_mds.sh` & `chemfeat-2024.1/scripts/generate_doc_mds.sh`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/src/chemfeat/csv_wrapper.py` & `chemfeat-2024.1/src/chemfeat/csv_wrapper.py`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/src/chemfeat/database.py` & `chemfeat-2024.1/src/chemfeat/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     return dict(zip(fields, row))
 
 
 class FeatureDatabase():
     '''
     Database for saving features.
     '''
-    INCHI_COLUMN_NAME = 'InChi'
+    INCHI_COLUMN_NAME = 'InChI'
     INCHI_COLUMN_INFO = (INCHI_COLUMN_NAME, 'TEXT', False, None, True)
     FEATURE_NAMES_TABLE_NAME = 'feature_names'
     FEATURE_NAMES_TABLE_INFO = [
         ('table', 'TEXT', False, None, True),
         ('feature_names', 'TEXT', False, None, False),
     ]
     FEATURES_COLUMN_NAME = 'features'
@@ -222,15 +222,15 @@
         accumulate rows for chunked insertion with executemany().
 
         Args:
             items:
                 Same as insert_features.
 
         Returns:
-            A generator over 3-tuples of database names, InChi strings and
+            A generator over 3-tuples of database names, InChI strings and
             feature objects as JSON strings.
         '''
         is_first = True
         for inchi, features in items:
             if not features:
                 LOGGER.warning('No features for %s', inchi)
                 continue
@@ -266,29 +266,29 @@
         Insert rows into feature set tables.
 
         Args:
             name:
                 The feature set name.
 
             rows:
-                An iterator of 2-tuples of InChi strings and JSON strings.
+                An iterator of 2-tuples of InChI strings and JSON strings.
         '''
         LOGGER.info('Inserting %s row(s) into table %s.', len(rows), name)
 
         with self.conn as conn:
             conn.executemany(f'REPLACE INTO "{name}" VALUES(?, ?)', rows)
 
     def insert_features(self, items):
         '''
         Insert features into the database.
 
         Args:
             items:
                 An iterator over 3-tuples of (<name>, <inchi>, <features>) where
-                <name> is the feature set name, <inchi> is the molecule's InChi,
+                <name> is the feature set name, <inchi> is the molecule's InChI,
                 and <features> is a dict mapping feature names to their values.
 
                 This must be equivalent to the iterator returned by
                 FeatureManager.calculate_features.
         '''
         # Chunk size for database insertion using executemany().
         chunksize = 1000
@@ -303,44 +303,44 @@
 
         for name, rows in all_rows.items():
             if rows:
                 self._insert_rows(name, rows)
 
     def is_inchi_in_table(self, inchi, name):
         '''
-        Check if an InChi is already in a table.
+        Check if an InChI is already in a table.
 
         Args:
             inchi:
-                The InChi.
+                The InChI.
 
             name:
                 The table name.
 
         Returns:
-            A boolean indicating if the InChi exists in the given table.
+            A boolean indicating if the InChI exists in the given table.
         '''
         with self.conn as conn:
             return bool(
                 conn.execute(
                     f'SELECT 1 FROM "{name}" WHERE {self.INCHI_COLUMN_NAME}=?',
                     [inchi]
                 )
             )
 
     def inchis_in_table(self, name):
         '''
-        Return all the InChis in a given table.
+        Return all the InChIs in a given table.
 
         Args:
             name:
                 The table name.
 
         Returns:
-            A generator over the InChis in the given table.
+            A generator over the InChIs in the given table.
         '''
         try:
             with self.conn as conn:
                 for row in conn.execute(f'SELECT "{self.INCHI_COLUMN_NAME}" FROM "{name}"'):
                     yield row[0]
         except sqlite3.OperationalError as err:
             if not err.args[0].startswith(self.NO_SUCH_TABLE_ERROR):
@@ -359,25 +359,25 @@
         '''
         with self.conn as conn:
             conn.row_factory = dict_factory
             yield from conn.execute(*args, **kwargs)
 
     def get_features(self, inchi, name):
         '''
-        Get the features for the InChi from the given table.
+        Get the features for the InChI from the given table.
 
         Args:
             inchi:
-                The InChi.
+                The InChI.
 
             name:
                 The table name.
 
         Returns:
-            A dict with the features, or None if the InChi was not found.
+            A dict with the features, or None if the InChI was not found.
         '''
         keys = self.get_feature_names(name)
         if not keys:
             return None
 
         with self.conn as conn:
             for row in conn.execute(
@@ -388,15 +388,15 @@
                 values = json.loads(row[0])
                 return dict(zip(keys, values))
         return None
 
     def _get_join_sql_query(self, names):
         '''
         Get the SQL query to (inner) join the given table names. All tables will
-        be joined on the InChi primary key.
+        be joined on the InChI primary key.
 
         Args:
             names:
                 The names of the tables to include.
 
         Returns:
             The SQL query as a string.
@@ -455,15 +455,15 @@
         Filter rows without selected inchis.j
 
         Args:
             rows:
                 An iterator over dicts as returned by _get_join_dicts().
 
             inchis:
-                An iterable of InChis. Only rows with InChis in this set will be
+                An iterable of InChIs. Only rows with InChIs in this set will be
                 included in the output. If None then all rows will be returned.
 
         Returns:
             A generator over the filtered dicts.
         '''
         if inchis is None:
             yield from rows
@@ -482,15 +482,15 @@
         Get a Pandas Dataframe with the features of the given tables.
 
         Args:
             names:
                 The names of the tables to include.
 
             inchis:
-                An optional iterable of InChis.
+                An optional iterable of InChIs.
 
         Returns:
             The Pandas Dataframe.
         '''
         rows = self._get_join_dicts(names)
         rows = self._filter_inchis(rows, inchis)
         return pd.DataFrame(rows)
@@ -503,15 +503,15 @@
             path:
                 The output path.
 
             names:
                 The names of the tables to include.
 
             inchis:
-                An optional iterable of InChis.
+                An optional iterable of InChIs.
         '''
         if isinstance(inchis, pd.Series):
             inchis = inchis.values
 
         rows = self._get_join_dicts(names)
         rows = self._filter_inchis(rows, inchis)
```

### Comparing `chemfeat-2023.9/src/chemfeat/main.py` & `chemfeat-2024.1/src/chemfeat/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,24 +46,24 @@
         path.parent.mkdir(parents=True, exist_ok=True)
         with path.open('w', encoding='utf-8') as handle:
             yield handle
 
 
 def calculate_features(pargs):
     '''
-    Calculate chemical features for the requested InChis.
+    Calculate chemical features for the requested InChIs.
     '''
     LOGGER.info('Calculating chemical features.')
     inchi_column = pargs.inchi
     in_path = pargs.input.resolve()
-    LOGGER.info('Loading InChis from %s', in_path)
+    LOGGER.info('Loading InChIs from %s', in_path)
     inchis = pd.read_csv(in_path)[inchi_column]
 
     if inchis.empty:
-        LOGGER.warning('No InChis found in %s', in_path)
+        LOGGER.warning('No InChIs found in %s', in_path)
         return 1
 
     feat_specs_path = pargs.feat_spec
     with feat_specs_path.open('r', encoding='utf-8') as handle:
         feat_specs = yaml.safe_load(handle)
 
     feat_db_path = pargs.database.resolve()
@@ -197,46 +197,46 @@
         dest='command'
     )
 
     # ------------------------------ calculate ------------------------------- #
     calc_parser = subparsers.add_parser(
         'calculate',
         aliases=['calc'],
-        help='Calculate chemical features from InChis.'
+        help='Calculate chemical features from InChIs.'
     )
     calc_parser.add_argument(
         'feat_spec',
         metavar='<YAML file>',
         type=pathlib.Path,
         help='A YAML file specifying the features to calculate.'
     )
     calc_parser.add_argument(
         'input',
         metavar='<CSV file>',
         type=pathlib.Path,
         help=('''
-            A CSV file containing a column with the InChis of the molecules for
+            A CSV file containing a column with the InChIs of the molecules for
             which the features should be calulated.'
         ''')
     )
     calc_parser.add_argument(
         'output',
         metavar='<CSV file>',
         type=pathlib.Path,
         help=('''
               The path to which the calculated features should be saved as a CSV
               file.
         ''')
     )
     calc_parser.add_argument(
         '-i', '--inchi',
-        metavar='<InChi column name>',
-        default='InChi',
+        metavar='<InChI column name>',
+        default='InChI',
         help=('''
-            The name of the column containing InChi values in the input file. It
+            The name of the column containing InChI values in the input file. It
             will also be used in the output file. Default: %(default)s
         ''')
     )
     calc_parser.add_argument(
         '-d', '--database',
         metavar='<SQLite database file>',
         default='features.sqlite',
```

### Comparing `chemfeat-2023.9/src/chemfeat/modules.py` & `chemfeat-2024.1/src/chemfeat/modules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/env python3
 '''
 Functions for dynamically importing modules.
 '''
 
+import importlib.util
 import logging
 import pathlib
 import pkgutil
+import sys
+from collections import deque
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def import_modules(paths, path_log_msg=None):
     '''
@@ -25,34 +28,45 @@
             An optional logging format string for logging messages about the
             given paths. If given, it should contain a single "%s" placeholder
             for the path argument.
 
     Returns:
         The set of loaded module names.
     '''
-    paths = set(pathlib.Path(path).resolve() for path in paths)
+    # Dicts from version 3.7 preserve order.
+    paths = list(dict.fromkeys(pathlib.Path(path).resolve() for path in paths))
+    # Subpaths of other paths will be detected by the parent path so omit them.
+    paths = [
+        path for path in paths if not any(
+            path.is_relative_to(p) for p in paths if path != p
+        )
+    ]
     if not paths:
         LOGGER.warning('No paths passed to import_modules().')
 
     if path_log_msg:
         for path in sorted(paths):
             LOGGER.debug(path_log_msg, path)
 
-    file_paths = set()
-    dir_paths = set()
+    file_paths = []
+    dir_paths = []
+    all_dir_paths = []
     for path in paths:
         if path.is_dir():
-            dir_paths.add(path)
+            dir_paths.append(path)
+            all_dir_paths.append(path)
         else:
-            file_paths.add(path)
-
-    all_dir_paths = sorted(dir_paths | set(path.parent for path in file_paths))
+            file_paths.append(path)
+            all_dir_paths.append(path.parent)
 
     loaded = set()
     for loader, name, _is_pkg in pkgutil.walk_packages(path=all_dir_paths):
         path = pathlib.Path(loader.path) / f'{name}.py'
         if path in file_paths or any(path.is_relative_to(p) for p in dir_paths):
             LOGGER.debug('Loading module %s from %s', name, path)
-            loader.find_module(name).load_module(name)
+            spec = loader.find_spec(name)
+            mod = importlib.util.module_from_spec(spec)
+            sys.modules[name] = mod
+            spec.loader.exec_module(mod)
             loaded.add(name)
 
     return loaded
```

### Comparing `chemfeat-2023.9/src/chemfeat/features/calculator.py` & `chemfeat-2024.1/src/chemfeat/features/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 #!/usr/bin/env python3
 
 '''
 Base clase for feature calculators.
-
-
-TODO:
-    * Add methods for describing the features for automatically generating
-      documentation.
 '''
 
 import inspect
 import logging
 from collections import OrderedDict
 
 from docstring_parser import parse as parse_docstring
```

### Comparing `chemfeat-2023.9/src/chemfeat/features/manager.py` & `chemfeat-2024.1/src/chemfeat/features/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,22 +20,21 @@
 from chemfeat.modules import import_modules
 
 
 LOGGER = logging.getLogger(__name__)
 NAME_KEY = 'name'
 INCHI_COLUMN = FeatureDatabase.INCHI_COLUMN_NAME
 
-# Map registered names to functions that convert InChi strings to rdkit Mol
+# Map registered names to functions that convert InChI strings to rdkit Mol
 # objects.
 _INCHI_TO_MOL = {
     None: Chem.inchi.MolFromInchi
 }
 
 
-
 def import_calculators(paths=None):
     '''
     Import the feature calculator subclasses.
 
     Args:
         paths:
             An optional list of paths to external modules with feature
@@ -64,63 +63,71 @@
 
 def _calculate_features(inchi_and_feat_calcs_and_func_name):
     '''
     Internal function for calculating features with a multiprocessing pool.
 
     Args:
         inchi_and_feat_calcs_and_func_name:
-            A 3-tuple consisting of an InChi string, a list of feature
-            calculators, and a function name for converting InChi string to
+            A 3-tuple consisting of an InChI string, a list of feature
+            calculators, and a function name for converting InChI string to
             rdkit Mol objects..
 
     Returns:
-        The InChi and the dict of features.
+        The InChI and the dict of features.
     '''
     inchi, feat_calcs, func_name = inchi_and_feat_calcs_and_func_name
     features = {}
     try:
         func = _INCHI_TO_MOL[func_name]
     except KeyError:
         LOGGER.error(
-            'The name "%s" is not a registered function to convert InChi to molecule',
+            'The name "%s" is not a registered function to convert InChI to molecule',
             func_name
         )
         return None, features
     LOGGER.debug('Converting %s to molecule with %s', inchi, func.__qualname__)
-    molecule = func(inchi)
-    if molecule is None:
-        LOGGER.error('Failed to convert InChi to molecule object: %s', inchi)
+    try:
+        molecule = func(inchi)
+        if molecule is None:
+            raise RuntimeError(f'{func_name} returned None')
+    except Exception as err:  # pylint: disable=broad-exception-caught
+        LOGGER.error(
+            'Failed to convert InChI to molecule object with %s: %s [%s]',
+            func_name,
+            inchi,
+            err
+        )
         return None, features
     for calc in feat_calcs:
         # TODO
         # If there is a problem using the same FeatureCalculator objects with
         # multiprocessing, instantiate new objects using the class and
         # parameters.
         calc.add_features(features, molecule)
     return inchi, features
 
 
 class FeatureManager():
     '''
-    Calculate features from InChis and save the results to a database.
+    Calculate features from InChIs and save the results to a database.
     '''
     def __init__(self, feature_database, features, inchi_to_mol=None):
         '''
         Args:
             feature_database:
                 A FeatureDatabase object.
 
             features:
                 An iterable of dicts. Each dict must contain the key "name"
                 which designates the feature set to use. All other key-value
                 pairs in the dict will be interpretted as parameters for the
                 designated feature set.
 
             inchi_to_mol:
-                The name of the function to use to convert InChi strings to
+                The name of the function to use to convert InChI strings to
                 molecule objects. It must be a name registed with
                 :meth:`register_inchi_to_mol`. If None,
                 rdkit.Chem.inchi.MolFromInchi will be used.
 
         Raises:
             See parse().
         '''
@@ -129,31 +136,31 @@
         self.inchis = None
         self.molecules = None
         self.inchi_to_mol = inchi_to_mol
 
     @staticmethod
     def register_inchi_to_mol(name, func):
         '''
-        Register a function so that it can be used to convert an InChi to a
+        Register a function so that it can be used to convert an InChI to a
         molecule object. The registered name can be passed to :meth:`__init__`
         with the `inchi_to_mol` parameter.
 
         Args:
             name:
                 The name under which to register the function. This can also be
                 None to change the default function.
 
             func:
-                The function. It must accept the InChi string as its sole
+                The function. It must accept the InChI string as its sole
                 argument and return an rdkit Mol object.
         '''
         old_func = _INCHI_TO_MOL.get(name)
         if old_func is not None:
             LOGGER.warning(
-                'Re-registering InChi to molecule function %s: %s -> %s',
+                'Re-registering InChI to molecule function %s: %s -> %s',
                 name,
                 old_func.__qualname__,
                 func.__qualname__
             )
         _INCHI_TO_MOL[name] = func
 
     def parse(self, features):
@@ -244,31 +251,31 @@
         '''
         Filter feature specifications based on what is already in the database.
         This assumes that the existing database tables contain the expected
         data, which may not be the case if the feature sets have changed.
 
         Args:
             inchis:
-                An iterable of target InChis.
+                An iterable of target InChIs.
 
         Returns:
-            A filtered list of 2-tuples mapping InChis to the missing feature
+            A filtered list of 2-tuples mapping InChIs to the missing feature
             specifications.
         '''
         precalculated = []
         for calc in self.feature_calculators.values():
             existing_inchis = set(self.feature_database.inchis_in_table(calc.identifier))
             precalculated.append((existing_inchis, calc))
 
         for inchi in inchis:
             feat_calcs = []
             for existing_inchis, calc in precalculated:
                 if inchi not in existing_inchis:
                     feat_calcs.append(calc)
-            # Only yield the InChi if there are uncalculated features.
+            # Only yield the InChI if there are uncalculated features.
             if feat_calcs:
                 yield inchi, feat_calcs
 
     def calculate_features(
         self,
         inchis,
         output_path=None,
@@ -277,15 +284,15 @@
     ):
         '''
         Get the path to a CSV file with the current feature set. If the file
         does not exist, it will be created.
 
         Args:
             inchis:
-                An iterable of InChi strings.
+                An iterable of InChI strings.
 
             output_path:
                 An optional output path for saving the results to a CSV file.
 
             return_dataframe:
                 If True, return a Pandas dataframe with the results.
```

### Comparing `chemfeat-2023.9/src/chemfeat/features/calculators/ecfp.py` & `chemfeat-2024.1/src/chemfeat/features/calculators/ecfp.py`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/src/chemfeat/features/calculators/padel.py` & `chemfeat-2024.1/src/chemfeat/features/calculators/padel.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 '''
 PaDEL feature calculators.
 
 Given the number of PaDEL descriptors and fingerprints, this module generates
 the corresponding classes programmatically.
 '''
 
+import inspect
 import logging
 import sys
 import textwrap
 from typing import Optional
 
 from PaDEL_pywrapper import PaDEL
 from PaDEL_pywrapper.descriptor import descriptors, _fingerprints
@@ -40,30 +41,28 @@
 
 
 class _PaDELCommonFeatureCalculator(FeatureCalculator):  # pylint: disable=abstract-method
     '''
     Abstract base class for other PaDEL feature calculators.
     '''
     _IS_3D = False
+    _PADEL_DESC = NotImplemented
+
+    def __init__(self, *args, **kwargs):
+        self.padel = PaDEL([self._PADEL_DESC], *args, ignore_3D=not self._IS_3D, **kwargs)
 
     @property
     def is_3D(self):
         return self._IS_3D
 
 
 class PaDELDescFeatureCalculator(_PaDELCommonFeatureCalculator):
     '''
     Base class for PaDEL feature calculator subclasses.
     '''
-    _PADEL_DESC = NotImplemented
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.padel = PaDEL([self._PADEL_DESC])
-
     def is_numeric(self, _name):
         return True
 
     def add_features(self, features, molecule):
         try:
             values = self.padel.calculate([molecule], show_banner=False)
         except Exception as err:
@@ -73,41 +72,51 @@
         return features
 
 
 class PaDELFPFeatureCalculator(_PaDELCommonFeatureCalculator):
     '''
     Base class for PaDEL fingerprint calculator subclasses.
     '''
-    _PADEL_DESC = NotImplemented
 
     def __init__(
         self,
         *args,
         size: Optional[int] = None,
         search_depth: Optional[int] = None,
         **kwargs
     ):
-        super().__init__(*args, **kwargs)
-        self._padel_kwargs = {}
+        if self._PADEL_DESC.name.startswith('CDK '):  # pylint: disable=no-member
+            signature = inspect.signature(self._PADEL_DESC.__call__)  # pylint: disable=no-member
+            self._padel_kwargs = {
+                name: value.default
+                for (name, value) in signature.parameters.items()
+                if value.default is not inspect.Parameter.empty
+            }
+        else:
+            self._padel_kwargs = {}
         if size is not None:
             self._padel_kwargs['size'] = int(size)
         if search_depth is not None:
             self._padel_kwargs['searchDepth'] = int(search_depth)
-        self.padel = PaDEL([self._PADEL_DESC], **self._padel_kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def parameters(self):
         return self._padel_kwargs.copy()
 
     def is_numeric(self, _name):
         return False
 
     def add_features(self, features, molecule):
         try:
-            fingerprint = self.padel.calculate([molecule], show_banner=False).iloc[0]
+            fingerprint = self.padel.calculate(
+                [molecule],
+                show_banner=False,
+                **self._padel_kwargs
+            ).iloc[0]
         except Exception as err:
             raise PadelError(f'{self.identifier}: {err}') from err
         return self.add_fingerprint_features(features, fingerprint)
 
 
 def _add_docstring_and_class(cls, name, docstring, features):
     citation_blurb = '''
```

### Comparing `chemfeat-2023.9/src/chemfeat/features/calculators/qed.py` & `chemfeat-2024.1/src/chemfeat/features/calculators/qed.py`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/src/chemfeat/features/calculators/rdkdesc.py` & `chemfeat-2024.1/src/chemfeat/features/calculators/rdkdesc.py`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/src/chemfeat/features/calculators/rdkfp.py` & `chemfeat-2024.1/src/chemfeat/features/calculators/rdkfp.py`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/src/chemfeat/features/calculators/secfp.py` & `chemfeat-2024.1/src/chemfeat/features/calculators/secfp.py`

 * *Files identical despite different names*

### Comparing `chemfeat-2023.9/LICENSE.txt` & `chemfeat-2024.1/LICENSE.txt`

 * *Files identical despite different names*

