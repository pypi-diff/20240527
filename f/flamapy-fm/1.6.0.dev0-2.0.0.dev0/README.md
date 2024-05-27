# Comparing `tmp/flamapy-fm-1.6.0.dev0.tar.gz` & `tmp/flamapy-fm-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-fm-1.6.0.dev0.tar", last modified: Mon Jan  8 10:31:27 2024, max compression
+gzip compressed data, was "flamapy-fm-2.0.0.dev0.tar", last modified: Mon May 27 15:17:46 2024, max compression
```

## Comparing `flamapy-fm-1.6.0.dev0.tar` & `flamapy-fm-2.0.0.dev0.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.498437 flamapy-fm-1.6.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-08 10:31:27.498437 flamapy-fm-1.6.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.494437 flamapy-fm-1.6.0.dev0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.494437 flamapy-fm-1.6.0.dev0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.494437 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.494437 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19963 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/models/feature_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.498437 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_atomic_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_average_branching_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_estimated_products_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    27850 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.498437 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/json_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15177 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-01-08 10:31:16.000000 flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:31:27.498437 flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-08 10:31:27.000000 flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-08 10:31:27.000000 flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-08 10:31:27.000000 flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-08 10:31:27.000000 flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-08 10:31:27.000000 flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 10:31:27.498437 flamapy-fm-1.6.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-08 10:31:17.000000 flamapy-fm-1.6.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.233325 flamapy-fm-2.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-27 15:17:46.233325 flamapy-fm-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.229325 flamapy-fm-2.0.0.dev0/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.229325 flamapy-fm-2.0.0.dev0/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.229325 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.229325 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20747 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/models/feature_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.229325 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_atomic_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_average_branching_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_estimated_configurations_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_generate_random_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28965 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.233325 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/clafer_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/featureide_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/json_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/pysat_to_fm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-27 15:17:32.000000 flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:17:46.233325 flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-27 15:17:46.000000 flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-27 15:17:46.000000 flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 15:17:46.000000 flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 15:17:46.000000 flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 15:17:46.000000 flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:17:46.233325 flamapy-fm-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-27 15:17:33.000000 flamapy-fm-2.0.0.dev0/setup.py
```

### Comparing `flamapy-fm-1.6.0.dev0/PKG-INFO` & `flamapy-fm-2.0.0.dev0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fm
-Version: 1.6.0.dev0
+Version: 2.0.0.dev0
 Summary: flamapy-fm is a plugin to Flamapy module
 Home-page: https://github.com/flamapy/fm_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/models/feature_model.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/models/feature_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 from typing import Any, Optional
 from functools import total_ordering
 
 from flamapy.core.exceptions import FlamaException
 from flamapy.core.models import AST, VariabilityModel, VariabilityElement, ASTOperation
 from flamapy.core.models.ast import simplify_formula, propagate_negation, to_cnf
-class Relation:
 
+
+class Relation:
     def __init__(
-        self,
-        parent: 'Feature',
-        children: list['Feature'],
-        card_min: int,
-        card_max: int
+        self, parent: "Feature", children: list["Feature"], card_min: int, card_max: int
     ) -> None:
-
         self.parent = parent
         self.children = children
         self.card_min = card_min
         self.card_max = card_max
 
-    def add_child(self, feature: 'Feature') -> None:
+    def add_child(self, feature: "Feature") -> None:
         self.children.append(feature)
 
     def is_mandatory(self) -> bool:
         return self.card_min == 1 and self.card_max == 1 and len(self.children) == 1
 
     def is_optional(self) -> bool:
         return self.card_min == 0 and self.card_max == 1 and len(self.children) == 1
 
     def is_or(self) -> bool:
         return (
-            self.card_min == 1 and
-            self.card_max == len(self.children) and
-            len(self.children) > 1
+            self.card_min == 1
+            and self.card_max == len(self.children)
+            and len(self.children) > 1
         )
 
     def is_alternative(self) -> bool:
         return self.card_min == 1 and self.card_max == 1 and len(self.children) > 1
 
     def is_mutex(self) -> bool:
         return self.card_min == 0 and self.card_max == 1 and len(self.children) > 1
@@ -49,109 +45,113 @@
             and not self.is_mutex()
         )
 
     def is_group(self) -> bool:
         return len(self.children) > 1
 
     def __str__(self) -> str:
-        parent_name = self.parent.name if self.parent else ''
-        res = f'{parent_name}[{self.card_min},{self.card_max}]'
+        parent_name = self.parent.name if self.parent else ""
+        res = f"{parent_name}[{self.card_min},{self.card_max}]"
         for _child in self.children:
-            res += _child.name + ' '
+            res += _child.name + " "
         if self.is_alternative():
-            relation_type = 'alternative'
+            relation_type = "alternative"
         elif self.is_or():
-            relation_type = 'or'
+            relation_type = "or"
         elif self.is_mandatory():
-            relation_type = 'mandatory'
+            relation_type = "mandatory"
         elif self.is_optional():
-            relation_type = 'optional'
+            relation_type = "optional"
         elif self.is_mutex():
-            relation_type = 'mutex'
+            relation_type = "mutex"
         elif self.is_cardinal():
-            relation_type = 'cardinality'
+            relation_type = "cardinality"
         else:
-            relation_type = 'Other'
-        res = f'({relation_type}) ' + res
+            relation_type = "Other"
+        res = f"({relation_type}) " + res
         return res
 
     def __hash__(self) -> int:
-        return hash((self.parent, frozenset(self.children), self.card_min, self.card_max))
+        return hash(
+            (self.parent, frozenset(self.children), self.card_min, self.card_max)
+        )
 
     def __eq__(self, other: Any) -> bool:
-        return (isinstance(other, Relation)
-                and self.parent == other.parent
-                and sorted(self.children) == sorted(other.children)
-                and self.card_min == other.card_min
-                and self.card_max == other.card_max)
+        return (
+            isinstance(other, Relation)
+            and self.parent == other.parent
+            and sorted(self.children) == sorted(other.children)
+            and self.card_min == other.card_min
+            and self.card_max == other.card_max
+        )
 
     def __lt__(self, other: Any) -> bool:
         return str(self) < str(other)
 
 
 @total_ordering
 class Feature(VariabilityElement):
 
     def __init__(
         self,
         name: str,
-        relations: Optional[list['Relation']] = None,
-        parent: Optional['Feature'] = None,
-        is_abstract: bool = False
+        relations: Optional[list["Relation"]] = None,
+        parent: Optional["Feature"] = None,
+        is_abstract: bool = False,
     ):
-
+        super().__init__(name)
         self.name = name
         self.relations = [] if relations is None else relations
         self.parent = self._get_parent() if parent is None else parent
         self.is_abstract = is_abstract
-        self.attributes = list['Attribute']([])
+        self.attributes = list["Attribute"]([])
 
     def is_empty(self) -> bool:
         return self.parent is None and self.relations == []
 
-    def add_relation(self, relation: 'Relation') -> None:
+    def add_relation(self, relation: "Relation") -> None:
         self.relations.append(relation)
         for child in relation.children:
             child.parent = self
 
-    def add_attribute(self, attribute: 'Attribute') -> None:
-        attribute.parent=self
+    def add_attribute(self, attribute: "Attribute") -> None:
+        attribute.parent = self
         self.attributes.append(attribute)
 
-    def get_attributes(self) -> list['Attribute']:
+    def get_attributes(self) -> list["Attribute"]:
         return self.attributes
 
-    def set_attributes(self, attributes: list['Attribute']) -> None:
+    def set_attributes(self, attributes: list["Attribute"]) -> None:
         self.attributes = attributes
 
-    def get_relations(self) -> list['Relation']:
+    def get_relations(self) -> list["Relation"]:
         return self.relations
 
-    def get_parent(self) -> Optional['Feature']:
+    def get_parent(self) -> Optional["Feature"]:
         return self.parent
 
-    def _get_parent(self) -> Optional['Feature']:
+    def _get_parent(self) -> Optional["Feature"]:
         return next((r.parent for r in self.get_relations() if not r.children), None)
 
-    def get_children(self) -> list['Feature']:
+    def get_children(self) -> list["Feature"]:
         """Direct children of the feature regardless the relation type."""
         return [f for r in self.get_relations() for f in r.children]
 
     def is_root(self) -> bool:
         return self.parent is None
 
     def is_mandatory(self) -> bool:
-        return (self.parent is not None
-                and any(r.is_mandatory() and self in r.children
-                        for r in self.parent.get_relations()))
+        return self.parent is not None and any(
+            r.is_mandatory() and self in r.children for r in self.parent.get_relations()
+        )
 
     def is_optional(self) -> bool:
-        return (self.parent is not None
-                and any(r.is_optional() and self in r.children
-                        for r in self.parent.get_relations()))
+        return self.parent is not None and any(
+            r.is_optional() and self in r.children for r in self.parent.get_relations()
+        )
 
     def is_or_group(self) -> bool:
         return any(r.is_or() for r in self.get_relations())
 
     def is_alternative_group(self) -> bool:
         return any(r.is_alternative() for r in self.get_relations())
 
@@ -180,15 +180,14 @@
         return isinstance(other, Feature) and self.name == other.name
 
     def __lt__(self, other: Any) -> bool:
         return str(self) < str(other)
 
 
 class Constraint:
-
     def __init__(self, name: str, ast: AST):
         self.name = name
         self._ast = ast
 
     @property
     def ast(self) -> AST:
         return self._ast
@@ -212,216 +211,244 @@
                 stack.append(node.left)
         return list(features)
 
     def is_simple_constraint(self) -> bool:
         """Return true if the constraint is a simple constraint (requires or excludes)."""
         return self.is_requires_constraint() or self.is_excludes_constraint()
 
-
     def is_complex_constraint(self) -> bool:
-        """Return true if the constraint is a complex constraint 
+        """Return true if the constraint is a complex constraint
         (i.e., it is not a simple constraint)."""
         return not self.is_simple_constraint()
 
-
     def is_requires_constraint(self) -> bool:
         """Return true if the constraint is a requires constraint."""
         root_op = self._ast.root
         if root_op.is_binary_op():
             if root_op.data in [ASTOperation.REQUIRES, ASTOperation.IMPLIES]:
                 return root_op.left.is_term() and root_op.right.is_term()
-            elif root_op.data == ASTOperation.OR:
-                neg_left = root_op.left.data == ASTOperation.NOT and root_op.left.left.is_term()
-                neg_right = root_op.right.data == ASTOperation.NOT and root_op.right.left.is_term()
-                return neg_left and root_op.right.is_term() or neg_right and root_op.left.is_term()
-        return False
 
+            if root_op.data == ASTOperation.OR:
+                neg_left = (
+                    root_op.left.data == ASTOperation.NOT
+                    and root_op.left.left.is_term()
+                )
+                neg_right = (
+                    root_op.right.data == ASTOperation.NOT
+                    and root_op.right.left.is_term()
+                )
+                return (
+                    neg_left
+                    and root_op.right.is_term()
+                    or neg_right
+                    and root_op.left.is_term()
+                )
+        return False
 
     def is_excludes_constraint(self) -> bool:
         """Return true if the constraint is an excludes constraint."""
         root_op = self._ast.root
         if root_op.is_binary_op():
             if root_op.data in [ASTOperation.EXCLUDES, ASTOperation.XOR]:
                 return root_op.left.is_term() and root_op.right.is_term()
-            elif root_op.data in [ASTOperation.REQUIRES, ASTOperation.IMPLIES]:
-                neg_right = root_op.right.data == ASTOperation.NOT and root_op.right.left.is_term()
+
+            if root_op.data in [ASTOperation.REQUIRES, ASTOperation.IMPLIES]:
+                neg_right = (
+                    root_op.right.data == ASTOperation.NOT
+                    and root_op.right.left.is_term()
+                )
                 return root_op.left.is_term() and neg_right
-            elif root_op.data == ASTOperation.OR:
-                neg_left = root_op.left.data == ASTOperation.NOT and root_op.left.left.is_term()
-                neg_right = root_op.right.data == ASTOperation.NOT and root_op.right.left.is_term()
+
+            if root_op.data == ASTOperation.OR:
+                neg_left = (
+                    root_op.left.data == ASTOperation.NOT
+                    and root_op.left.left.is_term()
+                )
+                neg_right = (
+                    root_op.right.data == ASTOperation.NOT
+                    and root_op.right.left.is_term()
+                )
                 return neg_left and neg_right
         return False
 
-    def is_pseudo_complex_constraint(self) -> bool:
-        """Return true if the constraint is a pseudo-complex constraint 
+    def is_pseudocomplex_constraint(self) -> bool:
+        """Return true if the constraint is a pseudo-complex constraint
         (i.e., it can be transformed to a set of simple constraints)."""
         split_ctcs = split_constraint(self)
-        return len(split_ctcs) > 1 and all(self.is_simple_constraint() for ctc in split_ctcs)
-
+        return len(split_ctcs) > 1 and all(
+            self.is_simple_constraint() for ctc in split_ctcs
+        )
 
-    def is_strict_complex_constraint(self) -> bool:
-        """Return true if the constraint is a strict-complex constraint 
+    def is_strictcomplex_constraint(self) -> bool:
+        """Return true if the constraint is a strict-complex constraint
         (i.e., it cannot be transformed to a set of simple constraints)."""
         split_ctcs = split_constraint(self)
-        return any(self.is_complex_constraint(ctc) for ctc in split_ctcs)
-    
+        return any(self.is_complex_constraint() for ctc in split_ctcs)
+
     def __str__(self) -> str:
-        return f'({self.name}) {str(self.ast)}'
+        return f"({self.name}) {str(self.ast)}"
 
     def __hash__(self) -> int:
         return hash(str(self.ast).lower())
 
     def __eq__(self, other: Any) -> bool:
-        return isinstance(other, Constraint) and str(self.ast).lower() == str(other.ast).lower()
+        return (
+            isinstance(other, Constraint)
+            and str(self.ast).lower() == str(other.ast).lower()
+        )
 
     def __lt__(self, other: Any) -> bool:
         return str(self.ast).lower() < str(other.ast).lower()
 
 
 class FeatureModel(VariabilityModel):
-
     @staticmethod
     def get_extension() -> str:
-        return 'fm'
+        return "fm"
 
     def __init__(
-        self,
-        root: 'Feature',
-        constraints: Optional[list['Constraint']] = None
+        self, root: "Feature", constraints: Optional[list["Constraint"]] = None
     ) -> None:
         self.root = root
         self.ctcs = [] if constraints is None else constraints
 
-    def get_relations(self, feature: Optional['Feature'] = None) -> list['Relation']:
+    def get_relations(self, feature: Optional["Feature"] = None) -> list["Relation"]:
         if self.root is None or self.root.is_empty():
             return []
         if feature is None:
             feature = self.root
         relations = []
         for relation in feature.relations:
             relations.append(relation)
             for _feature in relation.children:
                 relations.extend(self.get_relations(_feature))
         return relations
 
-    def get_features(self) -> list['Feature']:
-        features: list['Feature'] = []
+    def get_features(self) -> list["Feature"]:
+        features: list["Feature"] = []
         if self.root is not None:
             features.append(self.root)
             for relation in self.get_relations():
                 features.extend(relation.children)
         return features
 
-    def get_constraints(self) -> list['Constraint']:
+    def get_constraints(self) -> list["Constraint"]:
         return self.ctcs
 
-    def get_mandatory_features(self) -> list['Feature']:
+    def get_mandatory_features(self) -> list["Feature"]:
         return [f for f in self.get_features() if f.is_mandatory()]
 
-    def get_optional_features(self) -> list['Feature']:
+    def get_optional_features(self) -> list["Feature"]:
         return [f for f in self.get_features() if f.is_optional()]
 
-    def get_alternative_group_features(self) -> list['Feature']:
+    def get_alternative_group_features(self) -> list["Feature"]:
         return [f for f in self.get_features() if f.is_alternative_group()]
 
-    def get_or_group_features(self) -> list['Feature']:
+    def get_or_group_features(self) -> list["Feature"]:
         return [f for f in self.get_features() if f.is_or_group()]
 
-    def get_feature_by_name(self, feature_name: str) -> Optional['Feature']:
+    def get_feature_by_name(self, feature_name: str) -> Optional["Feature"]:
         return next((f for f in self.get_features() if f.name == feature_name), None)
 
-    def get_complex_constraints(self):
+    def get_complex_constraints(self) -> list["Constraint"]:
         return [c for c in self.get_constraints() if c.is_complex_constraint()]
-    
-    def get_simple_constraints(self):
+
+    def get_simple_constraints(self) -> list["Constraint"]:
         return [c for c in self.get_constraints() if c.is_simple_constraint()]
-    
-    def get_pseudocomplex_constraints(self):
-        return [c for c in self.get_constraints() if c.is_pseudo_complex_constraint()]
-    
-    def get_excludes_constraints(self):
+
+    def get_pseudocomplex_constraints(self) -> list["Constraint"]:
+        return [c for c in self.get_constraints() if c.is_pseudocomplex_constraint()]
+
+    def get_strictcomplex_constraints(self) -> list["Constraint"]:
+        return [c for c in self.get_constraints() if c.is_strictcomplex_constraint()]
+
+    def get_excludes_constraints(self) -> list["Constraint"]:
         return [c for c in self.get_constraints() if c.is_excludes_constraint()]
-    
-    def get_requires_constraints(self):
+
+    def get_requires_constraints(self) -> list["Constraint"]:
         return [c for c in self.get_constraints() if c.is_requires_constraint()]
-    
-    def import_model(self, root: Feature, parent: Feature, ctcs: list[Constraint]) -> None:
+
+    def import_model(
+        self, root: Feature, parent: Feature, ctcs: list[Constraint]
+    ) -> None:
         root.parent = parent
         for ctc in ctcs:
             if ctc not in self.ctcs:
                 self.ctcs.append(ctc)
 
     def __str__(self) -> str:
-        res = 'root: ' + ('None' if self.root is None else self.root.name) + '\r\n'
-        res += 'Relations:\r\n'
+        res = "root: " + ("None" if self.root is None else self.root.name) + "\r\n"
+        res += "Relations:\r\n"
         for i, relation in enumerate(self.get_relations()):
-            res += f'R{i}: {relation}\r\n'
+            res += f"R{i}: {relation}\r\n"
         for i, ctc in enumerate(self.ctcs):
-            res += f'CTC{i}: {ctc}\r\n'
-        attributes_res = ''
+            res += f"CTC{i}: {ctc}\r\n"
+        attributes_res = ""
         for feature in self.get_features():
             for attribute in feature.get_attributes():
-                attributes_res += f'{attribute}' + '\r\n'
-        if attributes_res != '':
-            res += 'Attributes:\r\n' + attributes_res
+                attributes_res += f"{attribute}" + "\r\n"
+        if attributes_res != "":
+            res += "Attributes:\r\n" + attributes_res
         return res
 
     def __hash__(self) -> int:
-        return hash((
-            self.root,
-            frozenset(self.get_features()),
-            frozenset(self.get_relations()),
-            frozenset(self.ctcs)
-        ))
+        return hash(
+            (
+                self.root,
+                frozenset(self.get_features()),
+                frozenset(self.get_relations()),
+                frozenset(self.ctcs),
+            )
+        )
 
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, FeatureModel) and
-            self.root == other.root and
-            sorted(self.get_features()) == sorted(other.get_features()) and
-            sorted(self.get_relations()) == sorted(other.get_relations()) and
-            sorted(self.get_constraints()) == sorted(other.get_constraints())
+            isinstance(other, FeatureModel)
+            and self.root == other.root
+            and sorted(self.get_features()) == sorted(other.get_features())
+            and sorted(self.get_relations()) == sorted(other.get_relations())
+            and sorted(self.get_constraints()) == sorted(other.get_constraints())
         )
 
 
 class Range:
     def __init__(self, min_value: int, max_value: int):
         self.min_value: int = min_value
         self.max_value: int = max_value
 
     def __str__(self) -> str:
-        return "[ " + str(self.min_value) + " to " + \
-            str(self.max_value) + "]"
+        return "[ " + str(self.min_value) + " to " + str(self.max_value) + "]"
 
 
 class Domain:
-    def __init__(self, ranges: Optional[list['Range']], elements: Optional[list['Any']]):
+    def __init__(
+        self, ranges: Optional[list["Range"]], elements: Optional[list["Any"]]
+    ):
         self.range_list = [] if ranges is None else ranges
         self.element_list = [] if elements is None else elements
 
-    def get_range_list(self) -> list['Range']:
+    def get_range_list(self) -> list["Range"]:
         return self.range_list
 
-    def get_element_list(self) -> list['Any']:
+    def get_element_list(self) -> list["Any"]:
         return self.element_list
 
     def add_range(self, new_range: Range) -> None:
         self.range_list.append(new_range)
 
     def add_element(self, element: Any) -> None:
         self.element_list.append(element)
 
-    def set_range_list(self, range_list: list['Range']) -> None:
+    def set_range_list(self, range_list: list["Range"]) -> None:
         self.range_list = range_list
 
-    def set_element_list(self, element_list: list['Any']) -> None:
+    def set_element_list(self, element_list: list["Any"]) -> None:
         self.element_list = element_list
 
     def __str__(self) -> str:
-
         result = ""
         element_list = self.element_list
         if len(element_list) > 0:
             result = str(element_list)
 
         range_list = self.range_list
         if len(range_list) > 0:
@@ -429,30 +456,36 @@
             for rng in range_list:
                 result = result + str(rng)
 
         return result
 
 
 class Attribute:
-    def __init__(self, name: str, domain: Optional[Domain] = None, default_value: Any = None, null_value: Optional['Any']=None):
-        self.name: 'str' = name
-        self.parent: Optional['Feature'] = None
-        self.domain: Optional['Domain'] = domain
-        self.default_value: 'Any' = default_value
+    def __init__(
+        self,
+        name: str,
+        domain: Optional[Domain] = None,
+        default_value: Any = None,
+        null_value: Optional["Any"] = None,
+    ):
+        self.name: "str" = name
+        self.parent: Optional["Feature"] = None
+        self.domain: Optional["Domain"] = domain
+        self.default_value: "Any" = default_value
         self.null_value: Optional[Any] = null_value
 
     def get_name(self) -> str:
         return self.name
 
-    def get_parent(self) -> Optional['Feature']:
+    def get_parent(self) -> Optional["Feature"]:
         return self.parent
 
     def get_domain(self) -> Domain:
         if self.domain is None:
-            raise FlamaException('Attribute domain is not defined')
+            raise FlamaException("Attribute domain is not defined")
         return self.domain
 
     def get_default_value(self) -> Any:
         return self.default_value
 
     def get_null_value(self) -> Any:
         return self.null_value
@@ -470,55 +503,62 @@
         self.default_value = default_value
 
     def set_null_value(self, null_value: Any) -> None:
         self.null_value = null_value
 
     def __str__(self) -> str:
         if self.parent is None:
-            raise TypeError('self.parent is None, expected Feature type')
+            raise TypeError("self.parent is None, expected Feature type")
 
         result = "[" + self.parent.name + "." + self.name + "]"
         if self.domain is not None:
             result = result + "Domain: " + str(self.domain)
         if self.default_value is not None:
             result = result + "Default value: " + str(self.default_value)
         if self.null_value is not None:
             result = result + "Null value: " + str(self.null_value)
 
         return result
 
-#This is a list of ultils to work with constraints
+
+# This is a list of ultils to work with constraints
 def get_new_ctc_name(ctcs_names: list[str], prefix_name: str) -> str:
-    """Return a new name for a constraint (based on the provided prefix) that is not already 
+    """Return a new name for a constraint (based on the provided prefix) that is not already
     in the given list of constraints' names."""
     count = 1
-    new_name = f'{prefix_name}'
+    new_name = f"{prefix_name}"
     while new_name in ctcs_names:
-        new_name = f'{prefix_name}{count}'
+        new_name = f"{prefix_name}{count}"
         count += 1
     return new_name
 
 
-def left_right_features_from_simple_constraint(simple_ctc: Constraint) -> tuple[str, str]:
+def left_right_features_from_simple_constraint(
+    simple_ctc: Constraint,
+) -> tuple[str, str]:
     """Return the names of the features involved in a simple constraint.
-    
+
     A simple constraint can be a requires constraint or an excludes constraint.
-    A requires constraint can be represented in the AST of the constraint with one of the 
+    A requires constraint can be represented in the AST of the constraint with one of the
     following structures:
         A requires B
         A => B
         !A v B
-    An excludes constraint can be represented in the AST of the constraint with one of the 
+    An excludes constraint can be represented in the AST of the constraint with one of the
     following structures:
         A excludes B
         A => !B
         !A v !B
     """
     root_op = simple_ctc.ast.root
-    if root_op.data in [ASTOperation.REQUIRES, ASTOperation.IMPLIES, ASTOperation.EXCLUDES]:
+    if root_op.data in [
+        ASTOperation.REQUIRES,
+        ASTOperation.IMPLIES,
+        ASTOperation.EXCLUDES,
+    ]:
         left = root_op.left.data
         right = root_op.right.data
         if right == ASTOperation.NOT:
             right = root_op.right.left.data
     elif root_op.data == ASTOperation.OR:
         left = root_op.left.data
         right = root_op.right.data
@@ -537,30 +577,30 @@
 def split_constraint(constraint: Constraint) -> list[Constraint]:
     """Given a constraint, split it in multiple constraints separated by the AND operator."""
     asts = split_formula(constraint.ast)
     asts_simplified = [simplify_formula(ast) for ast in asts]
     asts = []
     for ctc in asts_simplified:
         asts.extend(split_formula(ctc))
-        
+
     asts_negation_propagated = [propagate_negation(ast.root) for ast in asts]
     asts = []
     for ctc in asts_negation_propagated:
         asts.extend(split_formula(ctc))
 
     asts_cnf = [to_cnf(ast) for ast in asts]
     asts = []
     for ctc in asts_cnf:
         asts.extend(split_formula(ctc))
-    return [Constraint(f'{constraint.name}{i}', ast) for i, ast in enumerate(asts)]
+    return [Constraint(f"{constraint.name}{i}", ast) for i, ast in enumerate(asts)]
 
 
 def split_formula(formula: AST) -> list[AST]:
     """Given a formula, returns a list of formulas separated by the AND operator."""
     res = []
     node = formula.root
     if node.data == ASTOperation.AND:
         res.extend(split_formula(AST(node.left)))
         res.extend(split_formula(AST(node.right)))
     else:
         res.append(formula)
-    return res
+    return res
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/__init__.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from .fm_core_features import FMCoreFeatures, get_core_features
 from .fm_count_leafs import FMCountLeafs, count_leaf_features
 from .fm_leaf_features import FMLeafFeatures, get_leaf_features
 from .fm_average_branching_factor import FMAverageBranchingFactor, average_branching_factor
 from .fm_feature_ancestors import FMFeatureAncestors, get_feature_ancestors
 from .fm_max_depth_tree import FMMaxDepthTree, max_depth_tree
-from .fm_estimated_products_number import FMEstimatedProductsNumber, count_configurations
+from .fm_estimated_configurations_number import FMEstimatedConfigurationsNumber, count_configurations
 from .fm_atomic_sets import FMAtomicSets, get_atomic_sets
 from .fm_metrics import FMMetrics
+from .fm_generate_random_attribute import GenerateRandomAttribute
 
 __all__ = ['FMCoreFeatures', 'get_core_features',
            'FMCountLeafs', 'count_leaf_features',
            'FMLeafFeatures', 'get_leaf_features',
            'FMAverageBranchingFactor', 'average_branching_factor',
            'FMFeatureAncestors', 'get_feature_ancestors',
            'FMMaxDepthTree', 'max_depth_tree',
-           'FMEstimatedProductsNumber', 'count_configurations',
-           'FMAtomicSets', 'get_atomic_sets', 'FMMetrics']
+           'count_configurations',
+           'FMAtomicSets', 'get_atomic_sets', 'FMMetrics',
+           'GenerateRandomAttribute', 'FMEstimatedConfigurationsNumber']
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from flamapy.core.operations import CoreFeatures
+from typing import cast
 
+from flamapy.core.models import VariabilityModel
+from flamapy.core.operations import CoreFeatures
 from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature
 
 
 class FMCoreFeatures(CoreFeatures):
     """Core features are features that are present in all configurations of the feature model.
 
     This implementation assumes that:
@@ -18,16 +20,17 @@
 
     def __init__(self) -> None:
         self.result: list[Feature] = []
 
     def get_result(self) -> list[Feature]:
         return self.result
 
-    def execute(self, model: FeatureModel) -> 'FMCoreFeatures':
-        self.result = get_core_features(model)
+    def execute(self, model: VariabilityModel) -> 'FMCoreFeatures':
+        fm_model = cast(FeatureModel, model)
+        self.result = get_core_features(fm_model)
         return self
 
     def get_core_features(self) -> list[Feature]:
         return self.get_result()
 
 
 def get_core_features(feature_model: FeatureModel) -> list[Feature]:
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_estimated_products_number.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_estimated_configurations_number.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import math
-from typing import Optional
+from typing import Optional, cast
 
+from flamapy.core.models import VariabilityModel
 from flamapy.core.exceptions import FlamaException
-from flamapy.core.operations import EstimatedProductsNumber
+from flamapy.core.operations import EstimatedConfigurationsNumber
 from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature
 
 
-class FMEstimatedProductsNumber(EstimatedProductsNumber):
+class FMEstimatedConfigurationsNumber(EstimatedConfigurationsNumber):
     """It computes an estimation of the number of products of the feature model.
 
     It only uses the structure of the feature model,
     without taking into account the cross-tree constraints,
     and thus, the number is an upper limit of the real number of products.
     """
 
     def __init__(self) -> None:
         self.result = 0
         self.feature_model: Optional[FeatureModel] = None
 
-    def execute(self, model: FeatureModel) -> 'FMEstimatedProductsNumber':
-        self.feature_model = model
-        self.result = self.get_products_number()
+    def execute(self, model: VariabilityModel) -> 'FMEstimatedProductsNumber':
+        self.feature_model = cast(FeatureModel, model)
+        self.result = self.get_configurations_number()
         return self
 
     def get_result(self) -> int:
         return self.result
 
-    def get_products_number(self) -> int:
+    def get_configurations_number(self) -> int:
         if self.feature_model is None:
-            raise FlamaException("Feature is not defined")
+            raise FlamaException("The feature model is not defined")
 
         return count_configurations(self.feature_model)
 
 
 def count_configurations(feature_model: FeatureModel) -> int:
     return count_configurations_rec(feature_model.root)
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional
 
+from flamapy.core.models import VariabilityModel
 from flamapy.core.exceptions import FlamaException
 from flamapy.core.operations import Operation
-from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature
+from flamapy.metamodels.fm_metamodel.models import Feature
 
 
 class FMFeatureAncestors(Operation):
     """
     This operation returns the list of ancestors of a given feature
     (i.e., all parents recursively up to the root feature).
     """
@@ -17,18 +18,17 @@
 
     def set_feature(self, feature: Feature) -> None:
         self.feature = feature
 
     def get_result(self) -> list[Feature]:
         return self.result
 
-    def execute(self, model: FeatureModel) -> 'FMFeatureAncestors':
+    def execute(self, model: VariabilityModel) -> 'FMFeatureAncestors':
         if self.feature is None:
-            raise FlamaException("Feature is not defined")
-
+            raise FlamaException("The feature is not defined")
         self.result = get_feature_ancestors(self.feature)
         return self
 
 
 def get_feature_ancestors(feature: Feature) -> list[Feature]:
     features = []
     parent = feature.get_parent()
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from flamapy.core.operations import Operation
+from typing import cast
 
+from flamapy.core.models import VariabilityModel
+from flamapy.core.operations import Operation
 from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature
 
 
 class FMLeafFeatures(Operation):
     """
     This operation returns the list of features that are leaves of the feature model tree
     (i.e., they have not children).
@@ -11,14 +13,15 @@
 
     def __init__(self) -> None:
         self.result: list[Feature] = []
 
     def get_result(self) -> list[Feature]:
         return self.result
 
-    def execute(self, model: FeatureModel) -> 'FMLeafFeatures':
-        self.result = get_leaf_features(model)
+    def execute(self, model: VariabilityModel) -> 'FMLeafFeatures':
+        fm_model = cast(FeatureModel, model)
+        self.result = get_leaf_features(fm_model)
         return self
 
 
 def get_leaf_features(feature_model: FeatureModel) -> list[Feature]:
     return [f for f in feature_model.get_features() if len(f.get_relations()) == 0]
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from flamapy.core.operations import Operation
+from typing import cast
 
+from flamapy.core.models import VariabilityModel
+from flamapy.core.operations import CountLeafs
 from flamapy.metamodels.fm_metamodel.models import FeatureModel
-from flamapy.metamodels.fm_metamodel.operations import get_feature_ancestors, get_leaf_features
 
 
-class FMMaxDepthTree(Operation):
-    """This operation returns the maximum depth of the feature model tree."""
+class FMCountLeafs(CountLeafs):
 
     def __init__(self) -> None:
         self.result = 0
 
     def get_result(self) -> int:
         return self.result
 
-    def execute(self, model: FeatureModel) -> 'FMMaxDepthTree':
-        self.result = max_depth_tree(model)
+    def execute(self, model: VariabilityModel) -> 'FMCountLeafs':
+        fm_model = cast(FeatureModel, model)
+        self.result = count_leaf_features(fm_model)
         return self
 
+    def get_number_of_leafs(self) -> int:
+        return self.get_result()
 
-def max_depth_tree(feature_model: FeatureModel) -> int:
-    return max(len(get_feature_ancestors(f)) for f in get_leaf_features(feature_model))
+
+def count_leaf_features(feature_model: FeatureModel) -> int:
+    return sum(f.is_leaf() for f in feature_model.get_features())
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_metrics.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/operations/fm_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,538 +1,770 @@
-from typing import List, Tuple, Union, Optional, cast, Callable, Dict, Any
+from typing import Any, Callable, Optional, cast
 import statistics
 
-from flamapy.core.operations.metrics_operation import Metrics
+from flamapy.core.exceptions import FlamaException
 from flamapy.core.models.variability_model import VariabilityModel
-
+from flamapy.core.operations.metrics_operation import Metrics
 from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature
 from flamapy.metamodels.fm_metamodel import operations as fm_operations
 
 
+def metric_method(func: Callable[..., dict[str, Any]]) -> Callable[..., dict[str, Any]]:
+    """Decorator to mark a method as a metric method.
+    It has the value of the measure, it can also have a size and a ratio.
+    Example:
+        property name: Abstract Features.
+        description: The description of the property
+        value (optional): the list of abstract features.
+        size (optional): the length of the list.
+        ratio (optional): the percentage of abstract features with regards the total
+        number of features.
+    """
+    if not hasattr(func, "_is_metric_method"):
+        setattr(func, "_is_metric_method", True)
+    return func
 
-def metric_method(func: Callable) -> Callable:
-        """Decorator to mark a method as a metric method.
-        It has the value of the measure, it can also have a size and a ratio.
-        Example:
-            property name: Abstract Features.
-            description: The description of the property
-            value (optional): the list of abstract features.
-            size (optional): the length of the list.
-            ratio (optional): the percentage of abstract features with regards the total number of features.
-        """
-        if not hasattr(func, '_is_metric_method'):
-            setattr(func, '_is_metric_method', True)
-        return func
 
-class FMMetrics(Metrics):
+class FMMetrics(Metrics):  # pylint: disable=too-many-instance-attributes
 
     def __init__(self) -> None:
-        self.model = None
-        self.result: List[Dict[str, Any]] = []
-        self.model_type_extension="fm"
+        super().__init__()
+        self.model: Optional[FeatureModel] = None
+        self.result: list[dict[str, Any]] = []
+        self.model_type_extension = "fm"
+        self._features: list[Feature] = []
+        self._features_by_name: dict[str, Feature] = {}
+        self._abstract_features: dict[str, Feature] = {}
+        self._concrete_features: dict[str, Feature] = {}
+        self._leaf_features: list[str] = []
+        self._constraints_per_features: list[int] = []
+        self._feature_ancestors: list[int] = []
 
-    def get_result(self) -> Dict[str, Any]:
+    def get_result(self) -> list[dict[str, Any]]:
         return self.result
 
-
-
-    def calculate_metamodel_metrics(self,model) -> Dict[str, Any]:
+    def calculate_metamodel_metrics(self, model: VariabilityModel) -> list[dict[str, Any]]:
         self.model = cast(FeatureModel, model)
 
-        #Do some basic calculations to speedup the rest
+        # Do some basic calculations to speedup the rest
         self._features = self.model.get_features()
         self._features_by_name = {f.name: f for f in self._features}
         self._abstract_features = {f.name: f for f in self._features if f.is_abstract}
-        self._concrete_features = {f.name: f for f in self._features if not f.is_abstract}
-        self._leaf_features = [f.name for f in self._features if len(f.get_relations()) == 0]
-        self._constraints_per_features = self.constraints_per_features(model, self._features)
-        self._feature_ancestors = [len(self.get_feature_ancestors(self._features_by_name[f])) for f in self._leaf_features]
-       
+        self._concrete_features = {
+            f.name: f for f in self._features if not f.is_abstract
+        }
+        self._leaf_features = [
+            f.name for f in self._features if len(f.get_relations()) == 0
+        ]
+        self._constraints_per_features = self.constraints_per_features(
+            self.model, self._features
+        )
+        self._feature_ancestors = [
+            len(self.get_feature_ancestors(self._features_by_name[f]))
+            for f in self._leaf_features
+        ]
+
         # Get all methods that are marked with the metric_method decorator
-        metric_methods = [getattr(self, method_name) for method_name in dir(self) 
-                          if callable(getattr(self, method_name)) and hasattr(getattr(self, method_name), '_is_metric_method')]
+        metric_methods = [
+            getattr(self, method_name)
+            for method_name in dir(self)
+            if callable(getattr(self, method_name))
+            and hasattr(getattr(self, method_name), "_is_metric_method")
+        ]
         if self.filter is not None:
-            metric_methods = [method for method in metric_methods if method.__name__ in self.filter]
-          
+            metric_methods = [
+                method for method in metric_methods if method.__name__ in self.filter
+            ]
+
         return [method() for method in metric_methods]
 
-    ##Auxiliary methods
-    def constraints_per_features(self,fm: FeatureModel, features: list[Feature]) -> list[int]:
+    # Auxiliary methods
+    def constraints_per_features(
+        self, fm: FeatureModel, features: list[Feature]  # pylint: disable=invalid-name
+    ) -> list[int]:
         _features_per_constraints = []
         _constraints_per_feature = []
         for ctc in fm.get_constraints():
-            _features_per_constraints.append([f for f in ctc.get_features()])
+            _features_per_constraints.append(list(ctc.get_features()))
 
         for feature in features:
-            cpf = sum(feature.name in l for l in _features_per_constraints)
+            cpf = sum(feature.name in feat for feat in _features_per_constraints)
             _constraints_per_feature.append(cpf)
         return _constraints_per_feature
 
     def get_feature_ancestors(self, feature: Feature) -> list[Feature]:
         features = []
         parent = feature.get_parent()
         while parent is not None:
             features.append(parent)
             parent = parent.get_parent()
         return features
 
-    ##List of methods that returns a feature
+    # List of methods that returns a feature
     @metric_method
-    def features(self) -> Dict[str, Any]:
+    def features(self) -> dict[str, Any]:
         """Set of features in the feature model."""
         name = "Features"
         _features = list(self._features_by_name.keys())
-        result = self.construct_result(name=name,
-                                       doc=self.features.__doc__,
-                                       result=_features,
-                                       size=len(_features))
+        result = self.construct_result(
+            name=name, doc=self.features.__doc__, result=_features, size=len(_features)
+        )
         return result
 
-    #@metric_method
-    def abstract_features(self) -> Dict[str, Any]:
-        """Features used to structure the feature model that, however, do not have any impact at implementation level."""
+    @metric_method
+    def abstract_features(self) -> dict[str, Any]:
+        """Features used to structure the feature model that, however, do not have any
+        impact at implementation level."""
         name = "Abstract features"
         _abstract_features = list(self._abstract_features.keys())
-        result = self.construct_result( name=name,
-                                        doc=self.abstract_features.__doc__,
-                                        result=_abstract_features,
-                                        size=len(_abstract_features),
-                                        ratio=self.get_ratio(_abstract_features, self._features))
+        result = self.construct_result(
+            name=name,
+            doc=self.abstract_features.__doc__,
+            result=_abstract_features,
+            size=len(_abstract_features),
+            ratio=self.get_ratio(_abstract_features, self._features),
+        )
         return result
 
     @metric_method
-    def concrete_features(self) -> Dict[str, Any]:
+    def concrete_features(self) -> dict[str, Any]:
         """Features that are mapped to at least one implementation artifact."""
         name = "Concrete features"
         _concrete_features = list(self._concrete_features.keys())
-        result = self.construct_result( name=name,
-                                        doc=self.concrete_features.__doc__,
-                                        result=_concrete_features,
-                                        size=len(_concrete_features),
-                                        ratio=self.get_ratio(_concrete_features, self._features))
+        result = self.construct_result(
+            name=name,
+            doc=self.concrete_features.__doc__,
+            result=_concrete_features,
+            size=len(_concrete_features),
+            ratio=self.get_ratio(_concrete_features, self._features),
+        )
         return result
 
     @metric_method
-    def leaf_features(self) -> Dict[str, Any]:
+    def leaf_features(self) -> dict[str, Any]:
         """Features that have not subfeatures (aka 'primitive features' or 'terminal features')."""
         name = "Leaf features"
         _leaf_features = self._leaf_features
-        result = self.construct_result( name=name,
-                                        doc=self.leaf_features.__doc__,
-                                        result=_leaf_features,
-                                        size=len(_leaf_features),
-                                        ratio=self.get_ratio(_leaf_features, self._features))
+        result = self.construct_result(
+            name=name,
+            doc=self.leaf_features.__doc__,
+            result=_leaf_features,
+            size=len(_leaf_features),
+            ratio=self.get_ratio(_leaf_features, self._features),
+        )
         return result
 
-    #@metric_method
-    def compound_features(self) -> Dict[str, Any]:
+    @metric_method
+    def compound_features(self) -> dict[str, Any]:
         """Features that have subfeatures."""
         name = "Compound features"
-        _compound_features = [f.name for f in self._features if len(f.get_relations()) > 0]
-        result = self.construct_result( name=name,
-                                doc=self.compound_features.__doc__,
-                                result=_compound_features,
-                                size=len(_compound_features),
-                                ratio=self.get_ratio(_compound_features, self._features))
+        _compound_features = [
+            f.name for f in self._features if len(f.get_relations()) > 0
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.compound_features.__doc__,
+            result=_compound_features,
+            size=len(_compound_features),
+            ratio=self.get_ratio(_compound_features, self._features),
+        )
         return result
 
     @metric_method
-    def concrete_compound_features(self) -> Dict[str, Any]:
+    def concrete_compound_features(self) -> dict[str, Any]:
         """Concrete and compound features."""
         name = "Concrete compound features"
-        _concrete_compound_features = [name for name, f in self._concrete_features.items() if len(f.get_relations()) > 0]
-        result = self.construct_result( name=name,
-                                doc=self.concrete_compound_features.__doc__,
-                                result=_concrete_compound_features,
-                                size=len(_concrete_compound_features),
-                                ratio=self.get_ratio(_concrete_compound_features, self.concrete_features()["result"]))
+        _concrete_compound_features = [
+            name
+            for name, f in self._concrete_features.items()
+            if len(f.get_relations()) > 0
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.concrete_compound_features.__doc__,
+            result=_concrete_compound_features,
+            size=len(_concrete_compound_features),
+            ratio=self.get_ratio(
+                _concrete_compound_features, self.concrete_features()["result"]
+            ),
+        )
         return result
 
     @metric_method
-    def concrete_leaf_features(self) -> Dict[str, Any]:
+    def concrete_leaf_features(self) -> dict[str, Any]:
         """Concrete and leaf features."""
         name = "Concrete leaf features"
-        _concrete_leaf_features = [name for name, f in self._concrete_features.items() if len(f.get_relations()) == 0]
-        result = self.construct_result( name=name,
-                                doc=self.concrete_leaf_features.__doc__,
-                                result=_concrete_leaf_features,
-                                size=len(_concrete_leaf_features),
-                                ratio=self.get_ratio(_concrete_leaf_features, self.concrete_features()["result"]))
-        return result       
+        _concrete_leaf_features = [
+            name
+            for name, f in self._concrete_features.items()
+            if len(f.get_relations()) == 0
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.concrete_leaf_features.__doc__,
+            result=_concrete_leaf_features,
+            size=len(_concrete_leaf_features),
+            ratio=self.get_ratio(
+                _concrete_leaf_features, self.concrete_features()["result"]
+            ),
+        )
+        return result
 
     @metric_method
-    def abstract_compound_features(self) -> Dict[str, Any]:
+    def abstract_compound_features(self) -> dict[str, Any]:
         """Abstract and compound features."""
         name = "Abstract compound features"
-        _abstract_compound_features = [name for name, f in self._abstract_features.items() if len(f.get_relations()) > 0]
-        result = self.construct_result( name=name,
-                                doc=self.abstract_compound_features.__doc__,
-                                result=_abstract_compound_features,
-                                size=len(_abstract_compound_features),
-                                ratio=self.get_ratio(_abstract_compound_features, self._abstract_features.keys()))
+        _abstract_compound_features = [
+            name
+            for name, f in self._abstract_features.items()
+            if len(f.get_relations()) > 0
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.abstract_compound_features.__doc__,
+            result=_abstract_compound_features,
+            size=len(_abstract_compound_features),
+            ratio=self.get_ratio(
+                _abstract_compound_features, self._abstract_features.keys()
+            ),
+        )
         return result
 
     @metric_method
-    def abstract_leaf_features(self) -> Dict[str, Any]:
+    def abstract_leaf_features(self) -> dict[str, Any]:
         """Abstract and leaf features."""
         name = "Abstract leaf features"
-        _abstract_leaf_features = [name for name, f in self._abstract_features.items() if len(f.get_relations()) == 0]
-        result = self.construct_result( name=name,
-                                doc=self.abstract_leaf_features.__doc__,
-                                result=_abstract_leaf_features,
-                                size=len(_abstract_leaf_features),
-                                ratio=self.get_ratio(_abstract_leaf_features, self._abstract_features.keys()))
+        _abstract_leaf_features = [
+            name
+            for name, f in self._abstract_features.items()
+            if len(f.get_relations()) == 0
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.abstract_leaf_features.__doc__,
+            result=_abstract_leaf_features,
+            size=len(_abstract_leaf_features),
+            ratio=self.get_ratio(
+                _abstract_leaf_features, self._abstract_features.keys()
+            ),
+        )
         return result
 
     @metric_method
-    def tree_relationships(self) -> Dict[str, Any]:
+    def tree_relationships(self) -> dict[str, Any]:
         """Number of relationships (edges) of the feature model."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Tree relationships"
         _tree_relationships = [str(r) for r in self.model.get_relations()]
-        result = self.construct_result(name=name,
-                                doc=self.tree_relationships.__doc__,
-                                result=_tree_relationships,
-                                size=len(_tree_relationships))
+        result = self.construct_result(
+            name=name,
+            doc=self.tree_relationships.__doc__,
+            result=_tree_relationships,
+            size=len(_tree_relationships),
+        )
         return result
 
     @metric_method
-    def root_feature(self) -> Dict[str, Any]:
+    def root_feature(self) -> dict[str, Any]:
         """The root of the feature model."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Root feature"
         _root_feature = self.model.root.name
-        result = self.construct_result( name=name,
-                        doc=self.root_feature.__doc__,
-                        result=_root_feature,
-                        size=1,
-                        ratio=self.get_ratio([_root_feature], self._features))
+        result = self.construct_result(
+            name=name,
+            doc=self.root_feature.__doc__,
+            result=_root_feature,
+            size=1,
+            ratio=self.get_ratio([_root_feature], self._features),
+        )
         return result
-    
+
     @metric_method
-    def top_features(self) -> Dict[str, Any]:
+    def top_features(self) -> dict[str, Any]:
         """Features that are first descendants of the root."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Top features"
-        _top_features = [f.name for r in self.model.root.get_relations() for f in r.children]
-        result = self.construct_result( name=name,
-                        doc=self.top_features.__doc__,
-                        result=_top_features,
-                        size=len(_top_features),
-                        ratio=self.get_ratio(_top_features, self._features))
+        _top_features = [
+            f.name for r in self.model.root.get_relations() for f in r.children
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.top_features.__doc__,
+            result=_top_features,
+            size=len(_top_features),
+            ratio=self.get_ratio(_top_features, self._features),
+        )
         return result
 
     @metric_method
-    def solitary_features(self) -> Dict[str, Any]:
+    def solitary_features(self) -> dict[str, Any]:
         """Features that are not grouped in a feature group."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Solitary features"
-        _solitary_features = [f.name for f in self._features if not f.is_root() and not f.parent.is_group()]
-        result = self.construct_result( name=name,
-                doc=self.solitary_features.__doc__,
-                result=_solitary_features,
-                size=len(_solitary_features),
-                ratio=self.get_ratio(_solitary_features, self._features))
+        _solitary_features = [
+            f.name
+            for f in self._features
+            if not f.is_root() and f.parent is not None and not f.parent.is_group()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.solitary_features.__doc__,
+            result=_solitary_features,
+            size=len(_solitary_features),
+            ratio=self.get_ratio(_solitary_features, self._features),
+        )
         return result
 
     @metric_method
-    def grouped_features(self) -> Dict[str, Any]:
+    def grouped_features(self) -> dict[str, Any]:
         """Features that occurs in a feature group."""
         name = "Grouped features"
-        _grouped_features = [f.name for f in self._features if not f.is_root() and f.parent.is_group()]
-        result = self.construct_result( name=name,
-                doc=self.grouped_features.__doc__,
-                result=_grouped_features,
-                size=len(_grouped_features),
-                ratio=self.get_ratio(_grouped_features, self._features))
+        _grouped_features = [
+            f.name
+            for f in self._features
+            if not f.is_root() and f.parent is not None and f.parent.is_group()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.grouped_features.__doc__,
+            result=_grouped_features,
+            size=len(_grouped_features),
+            ratio=self.get_ratio(_grouped_features, self._features),
+        )
         return result
 
     @metric_method
-    def mandatory_features(self) -> Dict[str, Any]:
+    def mandatory_features(self) -> dict[str, Any]:
         """Features marked as mandatory that need to be selected if its parent is selected."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Mandatory features"
         _mandatory_features = [f.name for f in self.model.get_mandatory_features()]
-        result = self.construct_result( name=name,
-                                        doc=self.mandatory_features.__doc__,
-                                        result=_mandatory_features,
-                                        size=len(_mandatory_features),
-                                        ratio=self.get_ratio(_mandatory_features, self.solitary_features()["result"]))
+        result = self.construct_result(
+            name=name,
+            doc=self.mandatory_features.__doc__,
+            result=_mandatory_features,
+            size=len(_mandatory_features),
+            ratio=self.get_ratio(
+                _mandatory_features, self.solitary_features()["result"]
+            ),
+        )
         return result
 
     @metric_method
-    def optional_features(self) -> Dict[str, Any]:
+    def optional_features(self) -> dict[str, Any]:
         """Feature marked as optional."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Optional features"
         _optional_features = [f.name for f in self.model.get_optional_features()]
-        result = self.construct_result( name=name,
-                                doc=self.optional_features.__doc__,
-                                result=_optional_features,
-                                size=len(_optional_features),
-                                ratio=self.get_ratio(_optional_features, self.solitary_features()["result"]))
+        result = self.construct_result(
+            name=name,
+            doc=self.optional_features.__doc__,
+            result=_optional_features,
+            size=len(_optional_features),
+            ratio=self.get_ratio(
+                _optional_features, self.solitary_features()["result"]
+            ),
+        )
         return result
 
     @metric_method
-    def feature_groups(self) -> Dict[str, Any]:
+    def feature_groups(self) -> dict[str, Any]:
         """Features that express a choice over the grouped features in a group."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Feature groups"
-        _tree_relationships = [r for r in self.model.get_relations()]
+        _tree_relationships = list(self.model.get_relations())
         _feature_groups = [f.name for f in self._features if f.is_group()]
-        result = self.construct_result( name=name,
-                                        doc=self.feature_groups.__doc__,
-                                        result=_feature_groups,
-                                        size=len(_feature_groups),
-                                        ratio=self.get_ratio(_feature_groups, _tree_relationships))
+        result = self.construct_result(
+            name=name,
+            doc=self.feature_groups.__doc__,
+            result=_feature_groups,
+            size=len(_feature_groups),
+            ratio=self.get_ratio(_feature_groups, _tree_relationships),
+        )
         return result
 
-    #@metric_method
-    def alternative_groups(self) -> Dict[str, Any]:
-        """Feature groups that require the selection of just one child (i.e., [1..1] cardinality)."""
+    @metric_method
+    def alternative_groups(self) -> dict[str, Any]:
+        """Feature groups that require the selection of just one child (i.e., [1..1]
+        cardinality)."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Alternative groups"
         _group_features = [f.name for f in self._features if f.is_group()]
-        _alternative_groups = [f.name for f in self.model.get_alternative_group_features()]
-        result = self.construct_result( name=name,
-                                        doc=self.alternative_groups.__doc__,
-                                        result=_alternative_groups,
-                                        size=len(_alternative_groups),
-                                        ratio=self.get_ratio(_alternative_groups, _group_features))
+        _alternative_groups = [
+            f.name for f in self.model.get_alternative_group_features()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.alternative_groups.__doc__,
+            result=_alternative_groups,
+            size=len(_alternative_groups),
+            ratio=self.get_ratio(_alternative_groups, _group_features),
+        )
         return result
 
     @metric_method
-    def or_groups(self) -> Dict[str, Any]:
-        """Feature groups that require the selection of at least one child (i.e., [1..*] cardinality)."""
+    def or_groups(self) -> dict[str, Any]:
+        """Feature groups that require the selection of at least one child (i.e., [1..*]
+        cardinality)."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Or groups"
         _group_features = [f.name for f in self._features if f.is_group()]
         _or_groups = [f.name for f in self.model.get_or_group_features()]
-        result = self.construct_result( name=name,
-                                        doc=self.or_groups.__doc__,
-                                        result=_or_groups,
-                                        size=len(_or_groups),
-                                        ratio=self.get_ratio(_or_groups, _group_features))
+        result = self.construct_result(
+            name=name,
+            doc=self.or_groups.__doc__,
+            result=_or_groups,
+            size=len(_or_groups),
+            ratio=self.get_ratio(_or_groups, _group_features),
+        )
         return result
 
     @metric_method
-    def mutex_groups(self) -> Dict[str, Any]:
-        """Feature groups that require the selection of zero or just one child (i.e., [0..1] cardinality)."""
+    def mutex_groups(self) -> dict[str, Any]:
+        """Feature groups that require the selection of zero or just one child (i.e.,
+        [0..1] cardinality)."""
         name = "Mutex groups"
         _group_features = [f.name for f in self._features if f.is_group()]
         _mutex_groups = [f.name for f in self._features if f.is_mutex_group()]
-        result = self.construct_result( name=name,
-                                        doc=self.mutex_groups.__doc__,
-                                        result=_mutex_groups,
-                                        size=len(_mutex_groups),
-                                        ratio=self.get_ratio(_mutex_groups, _group_features))
+        result = self.construct_result(
+            name=name,
+            doc=self.mutex_groups.__doc__,
+            result=_mutex_groups,
+            size=len(_mutex_groups),
+            ratio=self.get_ratio(_mutex_groups, _group_features),
+        )
         return result
 
     @metric_method
-    def cardinality_groups(self) -> Dict[str, Any]:
-        """Feature groups with arbitrary cardinality [a..b] that require the selection of a minimum and a maximum number of children."""
+    def cardinality_groups(self) -> dict[str, Any]:
+        """Feature groups with arbitrary cardinality [a..b] that require the selection
+        of a minimum and a maximum number of children."""
         name = "Cardinality groups"
         _group_features = [f.name for f in self._features if f.is_group()]
-        _cardinality_groups = [f.name for f in self._features if f.is_cardinality_group()]
-        result = self.construct_result( name=name,
-                                        doc=self.cardinality_groups.__doc__,
-                                        result=_cardinality_groups,
-                                        size=len(_cardinality_groups),
-                                        ratio=self.get_ratio(_cardinality_groups, _group_features))
+        _cardinality_groups = [
+            f.name for f in self._features if f.is_cardinality_group()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.cardinality_groups.__doc__,
+            result=_cardinality_groups,
+            size=len(_cardinality_groups),
+            ratio=self.get_ratio(_cardinality_groups, _group_features),
+        )
         return result
 
     @metric_method
-    def branching_factor(self) -> Dict[str, Any]:
+    def branching_factor(self) -> dict[str, Any]:
         """Average number of children per non-leaf feature (aka 'Ratio of Variability')."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Branching factor"
         _avg_branching_factor = fm_operations.average_branching_factor(self.model)
-        result = self.construct_result( name=name,
-                                        doc=self.branching_factor.__doc__,
-                                        result=_avg_branching_factor)
+        result = self.construct_result(
+            name=name, doc=self.branching_factor.__doc__, result=_avg_branching_factor
+        )
         return result
-    
+
     @metric_method
-    def min_children_per_feature(self) -> Dict[str, Any]:
+    def min_children_per_feature(self) -> dict[str, Any]:
         """Minimal number of children per non-leaf feature."""
         name = "Min children per feature"
-        _min_children_per_feature = min(sum(len(r.children) for r in feature.get_relations()) for feature in self._features if not feature.is_leaf())
-        result = self.construct_result( name=name,
-                                        doc=self.min_children_per_feature.__doc__,
-                                        result=_min_children_per_feature)
+        _min_children_per_feature = min(
+            sum(len(r.children) for r in feature.get_relations())
+            for feature in self._features
+            if not feature.is_leaf()
+        )
+        result = self.construct_result(
+            name=name,
+            doc=self.min_children_per_feature.__doc__,
+            result=_min_children_per_feature,
+        )
         return result
 
     @metric_method
-    def max_children_per_feature(self) -> Dict[str, Any]:
+    def max_children_per_feature(self) -> dict[str, Any]:
         """Maximal number of children per feature."""
         name = "Max children per feature"
-        _max_children_per_feature = max(sum(len(r.children) for r in feature.get_relations()) for feature in self._features)
-        result = self.construct_result( name=name,
-                                        doc=self.max_children_per_feature.__doc__,
-                                        result=_max_children_per_feature)
+        _max_children_per_feature = max(
+            sum(len(r.children) for r in feature.get_relations())
+            for feature in self._features
+        )
+        result = self.construct_result(
+            name=name,
+            doc=self.max_children_per_feature.__doc__,
+            result=_max_children_per_feature,
+        )
         return result
 
     @metric_method
-    def avg_children_per_feature(self) -> Dict[str, Any]:
+    def avg_children_per_feature(self) -> dict[str, Any]:
         """Average number of children per feature."""
         name = "Avg children per feature"
-        nof_children = sum(len(r.children) for feature in self._features for r in feature.get_relations())
+        nof_children = sum(
+            len(r.children)
+            for feature in self._features
+            for r in feature.get_relations()
+        )
         _avg_children_per_feature = round(nof_children / len(self._features), 2)
-        result = self.construct_result( name=name,
-                                        doc=self.avg_children_per_feature.__doc__,
-                                        result=_avg_children_per_feature)
+        result = self.construct_result(
+            name=name,
+            doc=self.avg_children_per_feature.__doc__,
+            result=_avg_children_per_feature,
+        )
         return result
 
     @metric_method
-    def depth_tree(self) -> Dict[str, Any]:
+    def depth_tree(self) -> dict[str, Any]:
         """Number of features of the longest path from the root to the leaf features."""
         name = "Depth of tree"
         _max_depth_tree = max(self._feature_ancestors)
-        result = self.construct_result( name=name,
-                                doc=self.depth_tree.__doc__,
-                                result=_max_depth_tree)
+        result = self.construct_result(
+            name=name, doc=self.depth_tree.__doc__, result=_max_depth_tree
+        )
         return result
 
     @metric_method
-    def max_depth_tree(self) -> Dict[str, Any]:
+    def max_depth_tree(self) -> dict[str, Any]:
         """Number of features of the longest path from the root to the leaf features."""
         name = "Max depth of tree"
         _max_depth_tree = max(self._feature_ancestors)
-        result = self.construct_result( name=name,
-                                        doc=self.max_depth_tree.__doc__,
-                                        result=_max_depth_tree)
+        result = self.construct_result(
+            name=name, doc=self.max_depth_tree.__doc__, result=_max_depth_tree
+        )
         return result
 
     @metric_method
-    def mean_depth_tree(self) -> Dict[str, Any]:
+    def mean_depth_tree(self) -> dict[str, Any]:
         """Number of features of the mean path from the root to the leaf features."""
         name = "Mean depth of tree"
         _mean_depth_tree = statistics.mean(self._feature_ancestors)
-        result = self.construct_result( name=name,
-                                        doc=self.mean_depth_tree.__doc__,
-                                        result=round(_mean_depth_tree, 2))
+        result = self.construct_result(
+            name=name,
+            doc=self.mean_depth_tree.__doc__,
+            result=round(_mean_depth_tree, 2),
+        )
         return result
 
     @metric_method
-    def median_depth_tree(self) -> Dict[str, Any]:
+    def median_depth_tree(self) -> dict[str, Any]:
         """Number of features of the median path from the root to the leaf features."""
         name = "Median depth of tree"
         _median_depth_tree = statistics.median(self._feature_ancestors)
-        result = self.construct_result( name=name,
-                                        doc=self.median_depth_tree.__doc__,
-                                        result=round(_median_depth_tree, 2))
+        result = self.construct_result(
+            name=name,
+            doc=self.median_depth_tree.__doc__,
+            result=round(_median_depth_tree, 2),
+        )
         return result
 
     @metric_method
-    def cross_tree_constraints(self) -> Dict[str, Any]:
+    def cross_tree_constraints(self) -> dict[str, Any]:
         """Textual cross-tree constraints."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Cross-tree constraints"
         _cross_tree_constraints = [str(ctc) for ctc in self.model.get_constraints()]
-        result = self.construct_result( name=name,
-                                        doc=self.cross_tree_constraints.__doc__,
-                                        result=_cross_tree_constraints,
-                                        size=len(_cross_tree_constraints))
+        result = self.construct_result(
+            name=name,
+            doc=self.cross_tree_constraints.__doc__,
+            result=_cross_tree_constraints,
+            size=len(_cross_tree_constraints),
+        )
         return result
 
     @metric_method
-    def simple_constraints(self) -> Dict[str, Any]:
+    def simple_constraints(self) -> dict[str, Any]:
         """Requires and Excludes constraints."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Simple constraints"
         _simple_constraints = [str(ctc) for ctc in self.model.get_simple_constraints()]
-        result = self.construct_result( name=name,
-                                        doc=self.simple_constraints.__doc__,
-                                        result=_simple_constraints,
-                                        size=len(_simple_constraints),
-                                        ratio=self.get_ratio(_simple_constraints, self.model.get_constraints()))
-        return result    
+        result = self.construct_result(
+            name=name,
+            doc=self.simple_constraints.__doc__,
+            result=_simple_constraints,
+            size=len(_simple_constraints),
+            ratio=self.get_ratio(_simple_constraints, self.model.get_constraints()),
+        )
+        return result
 
     @metric_method
-    def requires_constraints(self) -> Dict[str, Any]:
-        """Constraints modeling that the activation of a feature f1 implies the activation of a feature f2."""
+    def requires_constraints(self) -> dict[str, Any]:
+        """Constraints modeling that the activation of a feature f1 implies the
+        activation of a feature f2."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Requires constraints"
-        _requires_constraints = [str(ctc) for ctc in self.model.get_requires_constraints()]
-        result = self.construct_result( name=name,
-                                        doc=self.requires_constraints.__doc__,
-                                        result=_requires_constraints,
-                                        size=len(_requires_constraints),
-                                        ratio=self.get_ratio(_requires_constraints, self.model.get_simple_constraints()))
-        return result  
+        _requires_constraints = [
+            str(ctc) for ctc in self.model.get_requires_constraints()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.requires_constraints.__doc__,
+            result=_requires_constraints,
+            size=len(_requires_constraints),
+            ratio=self.get_ratio(
+                _requires_constraints, self.model.get_simple_constraints()
+            ),
+        )
+        return result
 
     @metric_method
-    def excludes_constraints(self) -> Dict[str, Any]:
-        """Constraints modeling that two features are mutually exclusive and cannot be activated together."""
+    def excludes_constraints(self) -> dict[str, Any]:
+        """Constraints modeling that two features are mutually exclusive and cannot be
+        activated together."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Excludes constraints"
-        _excludes_constraints = [str(ctc) for ctc in self.model.get_excludes_constraints()]
-        result = self.construct_result( name=name,
-                                        doc=self.excludes_constraints.__doc__,
-                                        result=_excludes_constraints,
-                                        size=len(_excludes_constraints),
-                                        ratio=self.get_ratio(_excludes_constraints, self.model.get_simple_constraints()))
-        return result  
+        _excludes_constraints = [
+            str(ctc) for ctc in self.model.get_excludes_constraints()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.excludes_constraints.__doc__,
+            result=_excludes_constraints,
+            size=len(_excludes_constraints),
+            ratio=self.get_ratio(
+                _excludes_constraints, self.model.get_simple_constraints()
+            ),
+        )
+        return result
 
     @metric_method
-    def complex_constraints(self) -> Dict[str, Any]:
+    def complex_constraints(self) -> dict[str, Any]:
         """Constraints in arbitrary propositional logic formulae."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Complex constraints"
-        _complex_constraints = [str(ctc) for ctc in self.model.get_complex_constraints()]
-        result = self.construct_result( name=name,
-                                        doc=self.complex_constraints.__doc__,
-                                        result=_complex_constraints,
-                                        size=len(_complex_constraints),
-                                        ratio=self.get_ratio(_complex_constraints, self.model.get_constraints()))
-        return result    
+        _complex_constraints = [
+            str(ctc) for ctc in self.model.get_complex_constraints()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.complex_constraints.__doc__,
+            result=_complex_constraints,
+            size=len(_complex_constraints),
+            ratio=self.get_ratio(_complex_constraints, self.model.get_constraints()),
+        )
+        return result
 
     @metric_method
-    def pseudo_complex_constraints(self) -> Dict[str, Any]:
+    def pseudo_complex_constraints(self) -> dict[str, Any]:
         """Constraints that are convertible to a set of simple constraints."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Pseudo-complex constraints"
-        _pseudocomplex_constraints = [str(ctc) for ctc in self.model.get_pseudocomplex_constraints()]
-        result = self.construct_result( name=name,
-                                        doc=self.pseudo_complex_constraints.__doc__,
-                                        result=_pseudocomplex_constraints,
-                                        size=len(_pseudocomplex_constraints),
-                                        ratio=self.get_ratio(_pseudocomplex_constraints, self.model.get_complex_constraints()))
-        return result    
+        _pseudocomplex_constraints = [
+            str(ctc) for ctc in self.model.get_pseudocomplex_constraints()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.pseudo_complex_constraints.__doc__,
+            result=_pseudocomplex_constraints,
+            size=len(_pseudocomplex_constraints),
+            ratio=self.get_ratio(
+                _pseudocomplex_constraints, self.model.get_complex_constraints()
+            ),
+        )
+        return result
 
-    #@metric_method
-    def strict_complex_constraints(self) -> Dict[str, Any]:
+    @metric_method
+    def strict_complex_constraints(self) -> dict[str, Any]:
         """Constraints that cannot be converted to a set of simple constraints."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Strict-complex constraints"
-        _strictcomplex_constraints = [str(ctc) for ctc in self.fm.get_strictcomplex_constraints()]
-        result = self.construct_result( name=name,
-                                        doc=self.strict_complex_constraints.__doc__,
-                                        result=_strictcomplex_constraints,
-                                        size=len(_strictcomplex_constraints),
-                                        ratio=self.get_ratio(_strictcomplex_constraints, self.model.get_complex_constraints()))
-        return result    
+        _strictcomplex_constraints = [
+            str(ctc) for ctc in self.model.get_strictcomplex_constraints()
+        ]
+        result = self.construct_result(
+            name=name,
+            doc=self.strict_complex_constraints.__doc__,
+            result=_strictcomplex_constraints,
+            size=len(_strictcomplex_constraints),
+            ratio=self.get_ratio(
+                _strictcomplex_constraints, self.model.get_complex_constraints()
+            ),
+        )
+        return result
 
     @metric_method
-    def min_constraints_per_feature(self) -> Dict[str, Any]:
+    def min_constraints_per_feature(self) -> dict[str, Any]:
         """The minimal number of constraints per feature."""
         name = "Min constraints per feature"
         _constraints_per_feature = self._constraints_per_features
-        result = self.construct_result( name=name,
-                                        doc=self.min_constraints_per_feature.__doc__,
-                                        result=min(_constraints_per_feature))
-        return result    
+        result = self.construct_result(
+            name=name,
+            doc=self.min_constraints_per_feature.__doc__,
+            result=min(_constraints_per_feature),
+        )
+        return result
 
     @metric_method
-    def max_constraints_per_feature(self) -> Dict[str, Any]:
+    def max_constraints_per_feature(self) -> dict[str, Any]:
         """The maximal number of constraints per feature."""
         name = "Max constraints per feature"
         _constraints_per_feature = self._constraints_per_features
-        result = self.construct_result( name=name,
-                                doc=self.max_constraints_per_feature.__doc__,
-                                result=max(_constraints_per_feature))
-        return result    
+        result = self.construct_result(
+            name=name,
+            doc=self.max_constraints_per_feature.__doc__,
+            result=max(_constraints_per_feature),
+        )
+        return result
 
     @metric_method
-    def avg_constraints_per_feature(self) -> Dict[str, Any]:
+    def avg_constraints_per_feature(self) -> dict[str, Any]:
         """The average number of constraints per feature."""
         name = "Avg constraints per feature"
         _constraints_per_feature = self._constraints_per_features
-        result = self.construct_result( name=name,
-                        doc=self.avg_constraints_per_feature.__doc__,
-                        result=round(statistics.mean(_constraints_per_feature), 2))
-        return result    
+        result = self.construct_result(
+            name=name,
+            doc=self.avg_constraints_per_feature.__doc__,
+            result=round(statistics.mean(_constraints_per_feature), 2),
+        )
+        return result
 
     @metric_method
-    def extra_constraint_representativeness(self) -> Dict[str, Any]:
-        """Features involved in cross-tree constraints. The ratio to the total number of features is called 'Extra constraint representativeness (ECR)'."""
+    def extra_constraint_representativeness(self) -> dict[str, Any]:
+        """Features involved in cross-tree constraints. The ratio to the total number of
+        features is called 'Extra constraint representativeness (ECR)'."""
+        if self.model is None:
+            raise FlamaException("Feature model is not defined.")
+
         name = "Features in constraints"
-        _features_in_constraints = list({f for ctc in self.model.get_constraints() for f in ctc.get_features()})
-        result = self.construct_result( name=name,
-                        doc=self.extra_constraint_representativeness.__doc__,
-                        result=_features_in_constraints,
-                        size=len(_features_in_constraints),
-                        ratio=self.get_ratio(_features_in_constraints, self._features, 2))
-        return result
+        _features_in_constraints = list(
+            {f for ctc in self.model.get_constraints() for f in ctc.get_features()}
+        )
+        result = self.construct_result(
+            name=name,
+            doc=self.extra_constraint_representativeness.__doc__,
+            result=_features_in_constraints,
+            size=len(_features_in_constraints),
+            ratio=self.get_ratio(_features_in_constraints, self._features, 2),
+        )
+        return result
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 from flamapy.metamodels.fm_metamodel.models import (
     Constraint,
     Domain,
     Feature,
     FeatureModel,
     Range,
     Relation,
-    Attribute
+    Attribute,
 )
 
 
 class AFMReader(TextToModel):
-
     @staticmethod
     def get_source_extension() -> str:
-        return 'afm'
+        return "afm"
 
     def __init__(self, path: str) -> None:
         self.path: str = path
         self.parse_tree: AFMParser.Feature_modelContext = None
         self.model: Optional[FeatureModel] = None
 
     def set_parse_tree(self) -> None:
@@ -35,47 +34,55 @@
         self.parse_tree = get_tree(absolute_path)
 
     def transform(self) -> FeatureModel:
         self.set_parse_tree()
         self.set_relations()
         self.set_attributes()
         self.set_constraints()
+        if self.model is None:
+            raise FlamaException("FeatureModel is not defined.")
         return self.model
+
     def set_relations(self) -> None:
         root_feature_node = self.parse_tree
         relationships_block = root_feature_node.relationships_block()
         self.set_root_feature(relationships_block)
         self.set_child_features(relationships_block)
 
-    def set_root_feature(self, relationships_block: AFMParser.Relationships_blockContext) -> None:
+    def set_root_feature(
+        self, relationships_block: AFMParser.Relationships_blockContext
+    ) -> None:
         root_feature_spec = relationships_block.relationship_spec()[0]
         root_feature_name = root_feature_spec.init_spec().WORD().getText()
         root_feature = Feature(root_feature_name, [])
 
         self.model = FeatureModel(root_feature, None)
 
         self.read_children(root_feature_spec)
 
-    def set_child_features(self, relationship_block: AFMParser.Relationships_blockContext) -> None:
+    def set_child_features(
+        self, relationship_block: AFMParser.Relationships_blockContext
+    ) -> None:
         relationship_spec_list = relationship_block.relationship_spec()
         if len(relationship_spec_list) == 1:
             pass
         else:
             for relationship_spec in relationship_spec_list[1:]:
                 self.read_children(relationship_spec)
 
     def read_children(self, feature_spec: AFMParser.Relationship_specContext) -> None:
         if self.model is None:
-            raise TypeError('self.model is None, expected FeatureModel type')
+            raise TypeError("self.model is None, expected FeatureModel type")
 
         parent_feature = self.model.get_feature_by_name(
-            feature_spec.init_spec().WORD().getText())
+            feature_spec.init_spec().WORD().getText()
+        )
 
         if parent_feature is None:
-            raise FlamaException('parent_feature is not defined')
+            raise FlamaException("parent_feature is not defined")
 
         for non_cardinal_spec in feature_spec.non_cardinal_spec():
             child_node = non_cardinal_spec.getChild(0)
 
             if isinstance(child_node, AFMParser.Obligatory_specContext):
                 feature = Feature(child_node.WORD().getText(), [])
                 relation = Relation(parent_feature, [feature], 1, 1)
@@ -108,109 +115,115 @@
                 self.read_attribute(attribute_spec)
 
     def read_attribute(self, attribute_spec: AFMParser.Attribute_specContext) -> None:
         attribute_name_node = attribute_spec.attribute_name()
         attribute_name = attribute_name_node.LOWERCASE().getText()
 
         if self.model is None:
-            raise TypeError('self.model is None, expected FeatureModel type')
+            raise TypeError("self.model is None, expected FeatureModel type")
 
         attribute_feature = self.model.get_feature_by_name(
-            attribute_name_node.WORD().getText())
+            attribute_name_node.WORD().getText()
+        )
 
         if attribute_feature is None:
-            raise FlamaException('attribute_feature is not defined')
+            raise FlamaException("attribute_feature is not defined")
 
-        discrete_domain_node = attribute_spec.attribute_domain(
-        ).discrete_domain_spec()
+        discrete_domain_node = attribute_spec.attribute_domain().discrete_domain_spec()
         if discrete_domain_node is not None:
             values = []
             for value in discrete_domain_node.value_spec():
                 values.append(value.getText())
             domain = Domain(None, values)
 
         range_domain_node = attribute_spec.attribute_domain().range_domain_spec()
         if range_domain_node is not None:
             range_list = []
             for domain_range in range_domain_node.domain_range():
-                range_list.append(Range(domain_range.INT()[
-                    0], domain_range.INT()[1]))
+                range_list.append(Range(domain_range.INT()[0], domain_range.INT()[1]))
             domain = Domain(range_list, None)
 
         default_value = attribute_spec.attribute_default_value().value_spec().getText()
         null_value = attribute_spec.attribute_null_value().value_spec().getText()
 
-        attribute = Attribute(attribute_name, domain,
-                              default_value, null_value)
+        attribute = Attribute(attribute_name, domain, default_value, null_value)
         attribute.set_parent(attribute_feature)
         attribute_feature.add_attribute(attribute)
 
     def set_constraints(self) -> None:
         constraints_block = self.parse_tree.constraints_block()
         if constraints_block is not None:
             for constraint_spec in constraints_block.constraint_spec():
-
                 simple_spec = constraint_spec.simple_spec()
                 if simple_spec is not None:
                     prefix = ""
                     self.read_expression(simple_spec.expression(), prefix)
 
                 brackets_spec = constraint_spec.brackets_spec()
                 if brackets_spec is not None:
                     prefix = brackets_spec.WORD().getText() + "."
                     for spec in brackets_spec.simple_spec():
                         self.read_expression(spec.expression(), prefix)
 
-    def read_expression(self, expression: AFMParser.ExpressionContext, prefix: str) -> None:
-
+    def read_expression(
+        self, expression: AFMParser.ExpressionContext, prefix: str
+    ) -> None:
         root_node = self.build_ast_node(expression, prefix)
         ast = AST(root_node)
         cst = Constraint(expression.getText(), ast)
 
         if self.model is None:
-            raise TypeError('self.model is None, expected FeatureModel type')
+            raise TypeError("self.model is None, expected FeatureModel type")
 
         self.model.ctcs.append(cst)
 
-    def build_ast_node(self, expression: AFMParser.ExpressionContext, prefix: str) -> Node:
+    def build_ast_node(
+        self, expression: AFMParser.ExpressionContext, prefix: str
+    ) -> Node:
         if isinstance(expression, AFMParser.AtomContext):
             if expression.variable() is not None:
                 var_name = prefix + expression.variable().getText()
             if expression.number() is not None:
                 var_name = expression.number().getText()
             result = Node(var_name)
 
-        binary_operation_types = [AFMParser.LogicalExpContext,
-                                  AFMParser.OrExpContext,
-                                  AFMParser.AndExpContext,
-                                  AFMParser.RelationalExpContext,
-                                  AFMParser.ArithmeticExpContext]
-        binary_operations_map = {'REQUIRES': ASTOperation.REQUIRES,
-                                 'EXCLUDES': ASTOperation.EXCLUDES,
-                                 'OR': ASTOperation.OR,
-                                 'AND': ASTOperation.AND,
-                                 'IFF': ASTOperation.EQUIVALENCE}
+        binary_operation_types = [
+            AFMParser.LogicalExpContext,
+            AFMParser.OrExpContext,
+            AFMParser.AndExpContext,
+            AFMParser.RelationalExpContext,
+            AFMParser.ArithmeticExpContext,
+        ]
+        binary_operations_map = {
+            "REQUIRES": ASTOperation.REQUIRES,
+            "EXCLUDES": ASTOperation.EXCLUDES,
+            "OR": ASTOperation.OR,
+            "AND": ASTOperation.AND,
+            "IFF": ASTOperation.EQUIVALENCE,
+        }
 
         if expression.__class__ in binary_operation_types:
             binary_operation = expression.getChild(1).getText()
             ast_operation = binary_operations_map.get(binary_operation)
 
             # TODO: provide support for arithmetic and relational operations.
             if ast_operation is None:
                 raise FlamaException(
-                    f'Constraints not supported in AFM Reader: {binary_operation}.')
+                    f"Constraints not supported in AFM Reader: {binary_operation}."
+                )
             result = Node(ast_operation)
             result.left = self.build_ast_node(expression.expression()[0], prefix)
             result.right = self.build_ast_node(expression.expression()[1], prefix)
 
         if isinstance(expression, AFMParser.NotExpContext):
             result = Node(ASTOperation.NOT)
             result.right = self.build_ast_node(expression.expression(), prefix)
 
         if isinstance(expression, AFMParser.ParenthesisExpContext):
             result = self.build_ast_node(expression.expression(), prefix)
 
         if result is None:
             raise FlamaException(
-                f'Constraint not support in AFM Reader: {expression}, {prefix}')
+                f"Constraint not support in AFM Reader: {expression}, {prefix}"
+            )
 
         return result
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 class AFMWriter(ModelToText):
 
     @staticmethod
     def get_destination_extension() -> str:
         return 'afm'
 
-    def __init__(self, source_model: FeatureModel, path: str):
+    def __init__(self, path: str, source_model: FeatureModel):
         self.path = path
         self.model = source_model
 
     def transform(self) -> str:
         serialized_model = ""
         serialized_model += self.serialize_relationships()
         serialized_model += self.serialize_attributes()
         serialized_model += self.serialize_constraints()
 
-        with open(self.path, 'w', encoding='utf8') as file:
-            file.write(serialized_model)
+        if self.path is not None:
+            with open(self.path, 'w', encoding='utf8') as file:
+                file.write(serialized_model)
 
         return serialized_model
 
     def serialize_relationships(self) -> str:
         result = "%Relationships\n"
 
         root_feature = self.model.root
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,112 +13,125 @@
 )
 
 
 class FeatureIDEReader(TextToModel):
     """Reader for FeatureIDE models (.xml)."""
 
     # Main tags
-    TAG_STRUCT = 'struct'
-    TAG_CONSTRAINTS = 'constraints'
-    TAG_GRAPHICS = 'graphics'
+    TAG_FEATUREMODEL = "featureModel"
+    TAG_STRUCT = "struct"
+    TAG_FEATURE = "feature"
+    TAG_CONSTRAINTS = "constraints"
+    TAG_GRAPHICS = "graphics"
 
     # Feature tags
-    TAG_AND = 'and'
-    TAG_OR = 'or'
-    TAG_ALT = 'alt'
+    TAG_AND = "and"
+    TAG_OR = "or"
+    TAG_ALT = "alt"
 
     # Constraints tags
-    TAG_VAR = 'var'
-    TAG_NOT = 'not'
-    TAG_IMP = 'imp'
-    TAG_DISJ = 'disj'
-    TAG_CONJ = 'conj'
-    TAG_EQ = 'eq'
+    TAG_RULE = "rule"
+    TAG_VAR = "var"
+    TAG_NOT = "not"
+    TAG_IMP = "imp"
+    TAG_IMPN = "impn"
+    TAG_DISJ = "disj"
+    TAG_CONJ = "conj"
+    TAG_EQ = "eq"
 
     # Feature attributes
-    ATTRIB_NAME = 'name'
-    ATTRIB_ABSTRACT = 'abstract'
-    ATTRIB_MANDATORY = 'mandatory'
+    ATTRIB_NAME = "name"
+    ATTRIB_ABSTRACT = "abstract"
+    ATTRIB_MANDATORY = "mandatory"
 
     @staticmethod
     def get_source_extension() -> str:
-        return 'fide'
+        return "fide"
 
     def __init__(self, path: str) -> None:
         self._path = path
 
     def transform(self) -> FeatureModel:
         return self._read_feature_model(self._path)
 
     def _read_feature_model(self, filepath: str) -> FeatureModel:
         tree = ElementTree.parse(filepath)
         root = None
-        constraints = []
+        constraints_list = []
         for child in tree.getroot():
             if child.tag == FeatureIDEReader.TAG_STRUCT:
-                # TODO: _read_features tiene como segundo parámetro None, si lo
-                # permitimos, que hacemos luego en _read_features ??
                 (root_feature, _) = self._read_features(child, None)
                 root = root_feature
             elif child.tag == FeatureIDEReader.TAG_CONSTRAINTS:
                 constraints = self._read_constraints(child)
-                constraints.extend(constraints)
+                constraints_list.extend(constraints)
 
         if root is None:
-            raise FlamaException('No root feature found')
+            raise FlamaException("No root feature found")
 
         return FeatureModel(root=root, constraints=constraints)
 
     def _read_features(
         self,
         root_tree: Element,
         parent: Optional[Feature],
     ) -> tuple[Feature, list[Feature]]:
         children = []
         feature = None
 
         for child in root_tree:
             if not child.tag == FeatureIDEReader.TAG_GRAPHICS:
                 is_abstract = (
-                    FeatureIDEReader.ATTRIB_ABSTRACT in child.attrib and
-                    child.attrib[FeatureIDEReader.ATTRIB_ABSTRACT] == "true"
+                    FeatureIDEReader.ATTRIB_ABSTRACT in child.attrib
+                    and child.attrib[FeatureIDEReader.ATTRIB_ABSTRACT] == "true"
                 )
 
                 feature = Feature(
                     name=child.attrib[FeatureIDEReader.ATTRIB_NAME],
                     relations=[],
                     parent=parent,
-                    is_abstract=is_abstract
+                    is_abstract=is_abstract,
                 )
 
                 children.append(feature)
 
-                if root_tree.tag == FeatureIDEReader.TAG_AND:
-                    if FeatureIDEReader.ATTRIB_MANDATORY in child.attrib:  # Mandatory feature
-                        rel = Relation(parent=parent, children=[feature], card_min=1, card_max=1)
+                if root_tree.tag == FeatureIDEReader.TAG_AND and parent is not None:
+                    if (
+                        FeatureIDEReader.ATTRIB_MANDATORY in child.attrib
+                    ):  # Mandatory feature
+                        rel = Relation(
+                            parent=parent, children=[feature], card_min=1, card_max=1
+                        )
                         parent.add_relation(rel)
                     else:  # Optional feature
-                        rel = Relation(parent=parent, children=[feature], card_min=0, card_max=1)
+                        rel = Relation(
+                            parent=parent, children=[feature], card_min=0, card_max=1
+                        )
                         parent.add_relation(rel)
 
                 if child.tag == FeatureIDEReader.TAG_ALT:
                     (_, direct_children) = self._read_features(child, feature)
-                    rel = Relation(parent=feature, children=direct_children,
-                                    card_min=1, card_max=1)
+                    rel = Relation(
+                        parent=feature, children=direct_children, card_min=1, card_max=1
+                    )
                     feature.add_relation(rel)
                 elif child.tag == FeatureIDEReader.TAG_OR:
                     (_, direct_children) = self._read_features(child, feature)
-                    rel = Relation(parent=feature, children=direct_children, card_min=1,
-                                    card_max=len(direct_children))
+                    rel = Relation(
+                        parent=feature,
+                        children=direct_children,
+                        card_min=1,
+                        card_max=len(direct_children),
+                    )
                     feature.add_relation(rel)
                 elif child.tag == FeatureIDEReader.TAG_AND:
                     (_, direct_children) = self._read_features(child, feature)
-                    
+
         if feature is None:
-            raise FlamaException('No feature found')
+            raise FlamaException("No feature found")
 
         return (feature, children)
 
     def _read_constraints(self, ctcs_root: Element) -> list[Constraint]:
         number = 1
         constraints = []
         for ctc in ctcs_root:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,114 +2,135 @@
 import json
 from typing import Any, Optional
 
 from flamapy.core.exceptions import FlamaException
 from flamapy.core.models.ast import AST, Node, ASTOperation
 from flamapy.core.transformations import TextToModel
 
-from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature, Relation, Constraint
+from flamapy.metamodels.fm_metamodel.models import (
+    FeatureModel,
+    Feature,
+    Relation,
+    Constraint,
+)
 
 
 class GlencoeReader(TextToModel):
-
     @staticmethod
     def get_source_extension() -> str:
-        return 'gfm.json'
+        return "gfm.json"
 
     def __init__(self, path: str) -> None:
         self.path = path
 
     def transform(self) -> FeatureModel:
-        with open(self.path, 'r', encoding='utf-8') as file:
+        with open(self.path, "r", encoding="utf-8") as file:
             data = json.load(file)
-            features_info = data['features']
-            root_node = data['tree']
-            constraints_info = data['constraints']
+            features_info = data["features"]
+            root_node = data["tree"]
+            constraints_info = data["constraints"]
             root_feature = self._parse_tree(None, root_node, features_info)
             constraints = self._parse_constraints(constraints_info, features_info)
             return FeatureModel(root_feature, constraints)
 
-    def _parse_tree(self, parent: Optional[Feature], feature_node: dict[str, Any],
-                    features_info: dict[str, Any]) -> Feature:
+    def _parse_tree(
+        self,
+        parent: Optional[Feature],
+        feature_node: dict[str, Any],
+        features_info: dict[str, Any],
+    ) -> Feature:
         """Parse the tree structure and returns the root feature."""
-        feature_id = feature_node['id']
-        feature_type = features_info[feature_id]['type']
-        #optional = features_info[feature_id]['optional']
-        feature = Feature(name=features_info[feature_id]['name'], parent=parent)
+        feature_id = feature_node["id"]
+        feature_type = features_info[feature_id]["type"]
+        # optional = features_info[feature_id]['optional']
+        feature = Feature(name=features_info[feature_id]["name"], parent=parent)
 
-        if 'children' in feature_node:
+        if "children" in feature_node:
             children = []
-            for child in feature_node['children']:
+            for child in feature_node["children"]:
                 child_feature = self._parse_tree(feature, child, features_info)
-                optional = features_info[child['id']]['optional'] 
-                if feature_type == 'FEATURE':  # simple feature (not group)
+                optional = features_info[child["id"]]["optional"]
+                if feature_type == "FEATURE":  # simple feature (not group)
                     card_min = 0 if optional else 1
                     relation = Relation(feature, [child_feature], card_min, 1)
                     feature.add_relation(relation)
                 elif not optional:
                     # Additional relation because Glencoe supports mandatory features in groups
                     relation = Relation(feature, [child_feature], 1, 1)
                     feature.add_relation(relation)
-                    #children.append(child_feature)  # NOTE: may be needed for mandatory in groups
+                    # children.append(child_feature)  # NOTE: may be needed for mandatory in groups
                 else:
                     children.append(child_feature)
-            if feature_type != 'FEATURE':  # group
-                if feature_type == 'XOR':
+            if feature_type != "FEATURE":  # group
+                if feature_type == "XOR":
                     relation = Relation(feature, children, 1, 1)
-                elif feature_type == 'OR':
+                elif feature_type == "OR":
                     relation = Relation(feature, children, 1, len(children))
-                elif feature_type == 'GENOR':  # Group Cardinality
-                    card_min = features_info[feature_id]['min']
-                    card_max = features_info[feature_id]['max']
+                elif feature_type == "GENOR":  # Group Cardinality
+                    card_min = features_info[feature_id]["min"]
+                    card_max = features_info[feature_id]["max"]
                     relation = Relation(feature, children, card_min, card_max)
                 feature.add_relation(relation)
         # Create an attribute for the 'note' parameter
         # note = features_info[feature_id]['note']
         # if note:
         #     pass
         return feature
 
-    def _parse_constraints(self, ctcs_info: dict[str, Any],
-                           features_info: dict[str, Any]) -> list[Constraint]:
+    def _parse_constraints(
+        self, ctcs_info: dict[str, Any], features_info: dict[str, Any]
+    ) -> list[Constraint]:
         constraints = []
         for ctc_name, ctc_info in ctcs_info.items():
             ctc_node = self._parse_ast_constraint(ctc_info, features_info)
             constraints.append(Constraint(ctc_name, AST(ctc_node)))
         return constraints
 
-    def _parse_ast_constraint(self, ctc_info: dict[str, Any],
-                              features_info: dict[str, Any]) -> Node:
-        
-        ctc_type = ctc_info['type']
-        ctc_operands = ctc_info['operands']
+    def _parse_ast_constraint(
+        self, ctc_info: dict[str, Any], features_info: dict[str, Any]
+    ) -> Node:
+        ctc_type = ctc_info["type"]
+        ctc_operands = ctc_info["operands"]
         node = None
-        if ctc_type == 'FeatureTerm':
-            feature_id = ctc_info['operands'][0]
-            feature_name = features_info[feature_id]['name']
+        if ctc_type == "FeatureTerm":
+            feature_id = ctc_info["operands"][0]
+            feature_name = features_info[feature_id]["name"]
             node = Node(feature_name)
-        elif ctc_type == 'NotTerm':
+        elif ctc_type == "NotTerm":
             left = self._parse_ast_constraint(ctc_operands[0], features_info)
             node = Node(ASTOperation.NOT, left)
-        elif ctc_type == 'ImpliesTerm':
+        elif ctc_type == "ImpliesTerm":
             left = self._parse_ast_constraint(ctc_operands[0], features_info)
             right = self._parse_ast_constraint(ctc_operands[1], features_info)
             node = Node(ASTOperation.IMPLIES, left, right)
-        elif ctc_type == 'ExcludesTerm':
+        elif ctc_type == "ExcludesTerm":
             left = self._parse_ast_constraint(ctc_operands[0], features_info)
             right = self._parse_ast_constraint(ctc_operands[1], features_info)
             node = Node(ASTOperation.EXCLUDES, left, right)
-        elif ctc_type == 'EquivalentTerm':
+        elif ctc_type == "EquivalentTerm":
             left = self._parse_ast_constraint(ctc_operands[0], features_info)
             right = self._parse_ast_constraint(ctc_operands[1], features_info)
             node = Node(ASTOperation.EQUIVALENCE, left, right)
-        elif ctc_type == 'AndTerm':
-            op_list = [self._parse_ast_constraint(op, features_info) for op in ctc_operands]
-            node = functools.reduce(lambda lamb, r: Node(ASTOperation.AND, lamb, r), op_list)
-        elif ctc_type == 'OrTerm':
-            op_list = [self._parse_ast_constraint(op, features_info) for op in ctc_operands]
-            node = functools.reduce(lambda lamb, r: Node(ASTOperation.OR, lamb, r), op_list)
-        elif ctc_type == 'XorTerm':
-            op_list = [self._parse_ast_constraint(op, features_info) for op in ctc_operands]
-            node = functools.reduce(lambda lamb, r: Node(ASTOperation.XOR, lamb, r), op_list)
+        elif ctc_type == "AndTerm":
+            op_list = [
+                self._parse_ast_constraint(op, features_info) for op in ctc_operands
+            ]
+            node = functools.reduce(
+                lambda lamb, r: Node(ASTOperation.AND, lamb, r), op_list
+            )
+        elif ctc_type == "OrTerm":
+            op_list = [
+                self._parse_ast_constraint(op, features_info) for op in ctc_operands
+            ]
+            node = functools.reduce(
+                lambda lamb, r: Node(ASTOperation.OR, lamb, r), op_list
+            )
+        elif ctc_type == "XorTerm":
+            op_list = [
+                self._parse_ast_constraint(op, features_info) for op in ctc_operands
+            ]
+            node = functools.reduce(
+                lambda lamb, r: Node(ASTOperation.XOR, lamb, r), op_list
+            )
         else:
-            raise FlamaException(f'Invalid constraint: {ctc_info}')
+            raise FlamaException(f"Invalid constraint: {ctc_info}")
         return node
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,99 +3,103 @@
 
 from flamapy.core.models.ast import Node, ASTOperation
 from flamapy.core.transformations import ModelToText
 from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature, Constraint
 
 
 class GlencoeWriter(ModelToText):
-
-    CTC_TYPES = {ASTOperation.NOT: 'NotTerm',
-                 ASTOperation.AND: 'AndTerm',
-                 ASTOperation.OR: 'OrTerm',
-                 ASTOperation.XOR: 'XorTerm',
-                 ASTOperation.IMPLIES: 'ImpliesTerm',
-                 ASTOperation.REQUIRES: 'ImpliesTerm',
-                 ASTOperation.EXCLUDES: 'ExcludesTerm',
-                 ASTOperation.EQUIVALENCE: 'EquivalentTerm'}
+    CTC_TYPES = {
+        ASTOperation.NOT: "NotTerm",
+        ASTOperation.AND: "AndTerm",
+        ASTOperation.OR: "OrTerm",
+        ASTOperation.XOR: "XorTerm",
+        ASTOperation.IMPLIES: "ImpliesTerm",
+        ASTOperation.REQUIRES: "ImpliesTerm",
+        ASTOperation.EXCLUDES: "ExcludesTerm",
+        ASTOperation.EQUIVALENCE: "EquivalentTerm",
+    }
 
     @staticmethod
     def get_destination_extension() -> str:
-        return 'gfm.json'
+        return "gfm.json"
 
     def __init__(self, path: str, source_model: FeatureModel) -> None:
         self.path = path
         self.source_model = source_model
 
     def transform(self) -> str:
         json_object = _to_json(self.source_model)
         if self.path is not None:
-            with open(self.path, 'w', encoding='utf8') as file:
+            with open(self.path, "w", encoding="utf8") as file:
                 json.dump(json_object, file, indent=4)
         return json.dumps(json_object, indent=4)
 
 
 def _to_json(feature_model: FeatureModel) -> dict[str, Any]:
     result: dict[str, Any] = {}
-    result['id'] = f'FM_{feature_model.root.name}'
-    result['name'] = f'FM_{feature_model.root.name}'
-    result['features'] = _get_features_info(feature_model.get_features())
-    result['tree'] = _get_tree_info(feature_model.root)
-    result['constraints'] = _get_constraints_info(feature_model.get_constraints())
+    result["id"] = f"FM_{feature_model.root.name}"
+    result["name"] = f"FM_{feature_model.root.name}"
+    result["features"] = _get_features_info(feature_model.get_features())
+    result["tree"] = _get_tree_info(feature_model.root)
+    result["constraints"] = _get_constraints_info(feature_model.get_constraints())
     return result
 
 
 def _get_features_info(features: list[Feature]) -> dict[str, Any]:
     features_info = {}
-    for feature in sorted(features, key=lambda f:f.name):
-        feature_type = 'FEATURE'
+    for feature in sorted(features, key=lambda f: f.name):
+        feature_type = "FEATURE"
         if feature.is_alternative_group():
-            feature_type = 'XOR'
+            feature_type = "XOR"
         elif feature.is_or_group():
-            feature_type = 'OR'
+            feature_type = "OR"
         elif feature.is_cardinality_group():
-            feature_type = 'GENOR'
+            feature_type = "GENOR"
 
         features_info[feature.name] = {
-            'name': feature.name,
-            'optional': not feature.is_mandatory(), 
-            'type': feature_type,
-            'note': ''  # ToDo: add 'note' attribute information
+            "name": feature.name,
+            "optional": not feature.is_mandatory(),
+            "type": feature_type,
+            "note": "",  # ToDo: add 'note' attribute information
         }
 
-        if feature_type == 'GENOR':
+        if feature_type == "GENOR":
             relation = next(r for r in feature.get_relations() if r.is_cardinal())
-            features_info[feature.name]['min'] = relation.card_min
-            features_info[feature.name]['max'] = relation.card_max
+            features_info[feature.name]["min"] = relation.card_min
+            features_info[feature.name]["max"] = relation.card_max
     return features_info
 
 
 def _get_tree_info(feature: Feature) -> dict[str, Any]:
     feature_info: dict[str, Any] = {}
-    feature_info['id'] = feature.name
-    children = [_get_tree_info(child) for child in sorted(feature.get_children(),key=lambda f: f.name)]
+    feature_info["id"] = feature.name
+    children = [
+        _get_tree_info(child)
+        for child in sorted(feature.get_children(), key=lambda f: f.name)
+    ]
     if children:
-        feature_info['children'] = children
+        feature_info["children"] = children
     return feature_info
 
 
 def _get_constraints_info(constraints: list[Constraint]) -> dict[str, Any]:
     constraints_info = {}
     for ctc in constraints:
         constraints_info[ctc.name] = _get_ctc_info(ctc.ast.root)
     return constraints_info
 
 
 def _get_ctc_info(ast_node: Node) -> dict[str, Any]:
     ctc_info: dict[str, Any] = {}
     if ast_node.is_term():
-        ctc_info['type'] = 'FeatureTerm'
-        ctc_info['operands'] = [ast_node.data]
+        ctc_info["type"] = "FeatureTerm"
+        ctc_info["operands"] = [ast_node.data]
     else:
-        ctc_info['type'] = GlencoeWriter.CTC_TYPES[ast_node.data]
+        ctc_info["type"] = GlencoeWriter.CTC_TYPES[ast_node.data]
         operands = []
         left = _get_ctc_info(ast_node.left)
         operands.append(left)
         if ast_node.right is not None:
             right = _get_ctc_info(ast_node.right)
             operands.append(right)
-        ctc_info['operands'] = operands
+        ctc_info["operands"] = operands
     return ctc_info
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 class SPLOTWriter(ModelToText):
 
     @staticmethod
     def get_destination_extension() -> str:
         return 'sxfm'
 
     def __init__(self, path: str, source_model: FeatureModel) -> None:
-        self.path = path + '.' + SPLOTWriter.get_destination_extension()
+        self.path = path
         self.source_model = source_model
 
     def transform(self) -> str:
         splot_str = fm_to_splot(self.source_model)
-        with open(self.path, 'w', encoding='utf8') as file:
-            file.write(splot_str)
+        if self.path is not None:
+            with open(self.path, 'w', encoding='utf8') as file:
+                file.write(splot_str)
         return splot_str
 
 
 def fm_to_splot(model: FeatureModel) -> str:
     lines = []
     lines.append('<?xml version="1.0" encoding="UTF-8" standalone="no"?>')
     lines.append(f'<feature_model name="{model.root.name}">')
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,334 +1,427 @@
 import os
 import logging
 from typing import Any, Optional
 
 from antlr4 import CommonTokenStream, FileStream
+from antlr4.error.ErrorListener import ErrorListener
 from uvl.UVLCustomLexer import UVLCustomLexer
 from uvl.UVLPythonParser import UVLPythonParser
 
 from flamapy.core.exceptions import FlamaException
 from flamapy.core.transformations import TextToModel
 from flamapy.core.models.ast import AST, ASTOperation, Node
 from flamapy.metamodels.fm_metamodel.models import (
     Constraint,
     Feature,
     FeatureModel,
     Relation,
     Attribute,
 )
 
-from antlr4.error.ErrorListener import ErrorListener
 
 class CustomErrorListener(ErrorListener):
-    def __init__(self):
-        super(CustomErrorListener, self).__init__()
-        self.errors = []
-
-    def syntaxError(self, recognizer, offendingSymbol, line, column, msg, e):
+    def __init__(self) -> None:
+        super().__init__()
+        self.errors: list[str] = []
+
+    def syntaxError(  # noqa: N802
+        self,
+        recognizer: Any,
+        offendingSymbol: Any,  # noqa: N803
+        line: Any,
+        column: Any,
+        msg: Any,
+        e: Any,
+    ) -> None:
         error_msg = f"Syntax error at line {line}, column {column}: {msg}"
         self.errors.append(error_msg)
 
-class UVLReader(TextToModel):
 
+class UVLReader(TextToModel):
     @staticmethod
     def get_source_extension() -> str:
-        return 'uvl'
+        return "uvl"
 
     def __init__(self, path: str) -> None:
         self.path: str = os.sep.join(path.split(os.sep)[:-1])
         self.file: str = path.split(os.sep)[-1]
-        self.namespace: str = ''
+        self.namespace: str = ""
         self.parse_tree: Any = None
         self.model: Optional[FeatureModel] = None
         self.imports: dict[str, FeatureModel] = {}
         self.import_root: dict[str, str] = {}
 
     def set_parse_tree(self) -> None:
         absolute_path = os.path.abspath(os.path.join(self.path, self.file))
         input_stream = FileStream(absolute_path)
         lexer = UVLCustomLexer(input_stream)
 
         stream = CommonTokenStream(lexer)
         parser = UVLPythonParser(stream)
-    
+
         # Attach custom error listener
         error_listener = CustomErrorListener()
         parser.removeErrorListeners()
         parser.addErrorListener(error_listener)
 
         self.parse_tree = parser.featureModel()
 
         if error_listener.errors:
             for error in error_listener.errors:
                 logging.error(error)
             raise FlamaException("Parsing failed due to syntax errors.")
-        
-    def process_attributes(self, attributes_node):
+
+    def process_attributes(
+        self, attributes_node: UVLPythonParser.AttributeContext
+    ) -> dict[str, Any]:
         attributes_list = attributes_node.attribute()
         attributes_dict = {}
-        
+
         for attribute_context in attributes_list:
             # First, check which kind of attribute we're dealing with
             value_attribute = attribute_context.valueAttribute()
             constraint_attribute = attribute_context.constraintAttribute()
 
             if value_attribute:
                 key = value_attribute.key().getText()
                 if value_attribute.value():
                     value = self.process_value(value_attribute.value())
                 else:
                     value = None  # or some default value
-           
+
             elif constraint_attribute:
                 # Here you can handle constraint attributes if you need them
                 # If they should be processed differently, provide methods similar to process_value
                 logging.warning("This attributes are not yet supported in flama.")
-                pass  # Adjust accordingly
             else:
                 # Handle unexpected case
-                raise ValueError(f"Unknown attribute type for: {attribute_context.getText()}")
+                raise ValueError(
+                    f"Unknown attribute type for: {attribute_context.getText()}"
+                )
 
             attributes_dict[key] = value
         return attributes_dict
 
-
-   
-
-    def process_value(self, value_context):
+    def process_value(self, value_context: UVLPythonParser.ValueContext) -> Any:
+        value = None
         if value_context.BOOLEAN():
-            return value_context.BOOLEAN().getText() == 'true'
+            value = value_context.BOOLEAN().getText() == "true"
         elif value_context.FLOAT():
-            return float(value_context.FLOAT().getText())
+            value = float(value_context.FLOAT().getText())
         elif value_context.INTEGER():
-            return int(value_context.INTEGER().getText())
+            value = int(value_context.INTEGER().getText())
         elif value_context.STRING():
-            return value_context.STRING().getText()[1:-1]  # Removing quotes
+            value = value_context.STRING().getText()[1:-1]  # Removing quotes
         elif value_context.attributes():
-            return self.process_attributes(value_context.attributes())
+            value = self.process_attributes(value_context.attributes())
         elif value_context.vector():
-            return [self.process_value(val) for val in value_context.vector().value()]
+            value = [self.process_value(val) for val in value_context.vector().value()]
+        return value
 
-    def process_feature(self, feature:Feature, feature_node: UVLPythonParser.FeatureContext) -> Feature:
-        
-        #See if there is a feature cardinality and attributes (TODO)
+    def _check_feature_cardinality(
+        self, feature: Feature, feature_node: UVLPythonParser.FeatureContext
+    ) -> None:
+        # See if there is a feature cardinality and attributes (TODO)
         if feature_node.featureCardinality():
             cardinality_text = feature_node.featureCardinality().CARDINALITY().getText()
             min_val, max_val = self.parse_cardinality(cardinality_text)
             feature.card_min = min_val
             feature.card_max = max_val
-        
+
+    def _check_attributes(
+        self, feature: Feature, feature_node: UVLPythonParser.FeatureContext
+    ) -> None:
         if feature_node.attributes():
             attributes = self.process_attributes(feature_node.attributes())
+
             for key, value in attributes.items():
-                if key == 'abstract':
-                    feature.abstract = True
+                if key == "abstract" and (value is None or value):
+                    feature.is_abstract = True
                 else:
                     feature.add_attribute(Attribute(name=key, default_value=value))
-                    
+
+    def process_feature(
+        self, feature: Feature, feature_node: UVLPythonParser.FeatureContext
+    ) -> Feature:
+        self._check_feature_cardinality(feature, feature_node)
+        self._check_attributes(feature, feature_node)
+
         # Get the relationship type
         for relationship in feature_node.group():
-            childs=self.process_group(relationship.groupSpec())
+            childs = self.process_group(relationship.groupSpec())
             if isinstance(relationship, UVLPythonParser.AlternativeGroupContext):
                 feature.add_relation(Relation(feature, childs, 1, 1))
             elif isinstance(relationship, UVLPythonParser.OptionalGroupContext):
                 for child in childs:
                     feature.add_relation(Relation(feature, [child], 0, 1))
             elif isinstance(relationship, UVLPythonParser.OrGroupContext):
                 feature.add_relation(Relation(feature, childs, 1, len(childs)))
             elif isinstance(relationship, UVLPythonParser.MandatoryGroupContext):
                 for child in childs:
                     feature.add_relation(Relation(feature, [child], 1, 1))
             elif isinstance(relationship, UVLPythonParser.CardinalityGroupContext):
                 # Access the CARDINALITY token text.
                 cardinality_text = relationship.CARDINALITY().getText()
-                
-                min_value, max_value=self.parse_cardinality(cardinality_text)
-                feature.add_relation(Relation(feature, childs,min_value, max_value))
-                
-                if(max_value>len(childs)):
-                    logging.warning("Cardinality error: max value is greater than the number of childs")
+
+                min_value, max_value = self.parse_cardinality(cardinality_text)
+                feature.add_relation(Relation(feature, childs, min_value, max_value))
+
+                if max_value > len(childs):
+                    logging.warning(
+                        "Cardinality error: max value is greater than the number of childs"
+                    )
 
         return feature
 
     def parse_cardinality(self, cardinality_text: str) -> tuple[int, int]:
         # Extract the minimum and maximum values.
         # This assumes a format like "[min..max]" or "[min]" or "[min..*]"
-        min_value = None
-        max_value = None
+        min_value: str = ""
+        max_value: str = ""
 
         # Remove brackets.
         cardinality_text = cardinality_text[1:-1]
 
-        if '..' in cardinality_text:
-            parts = cardinality_text.split('..')
+        if ".." in cardinality_text:
+            parts = cardinality_text.split("..")
             min_value = parts[0]
             max_value = parts[1]
         else:
             min_value = cardinality_text
             max_value = min_value  # Assuming max is the same as min if not specified.
 
-        min_value=(int)(min_value)
-        max_value=(int)(max_value)
-        return min_value, max_value
-    
-    def process_group(self, groupSpec_node) ->list[Feature]:
-        list_features=[]
-        for feature_context in groupSpec_node.feature():
+        try:
+            return int(min_value), int(max_value)
+        except Exception as exc:
+            raise exc
+
+    def process_group(
+        self, group_spec_node: UVLPythonParser.GroupSpecContext
+    ) -> list[Feature]:
+        list_features = []
+        for feature_context in group_spec_node.feature():
             feature_name = feature_context.reference().getText()
             feature = Feature(feature_name, [])
             self.process_feature(feature, feature_context)
             list_features.append(feature)
         return list_features
-    
-    def process_constraints(self, constraint_node) -> Node:
-        n = None
+
+    def process_constraints(
+        self, constraint_node: UVLPythonParser.ConstraintContext
+    ) -> Node:
+        process = None
         if isinstance(constraint_node, UVLPythonParser.EquationConstraintContext):
-            n = self.process_equation_constraint(constraint_node)
-        elif isinstance(constraint_node, UVLPythonParser.LiteralConstraintContext) :
-            n = self.process_literal_constraint(constraint_node)
+            process = self.process_equation_constraint(constraint_node)
+        elif isinstance(constraint_node, UVLPythonParser.LiteralConstraintContext):
+            process = self.process_literal_constraint(constraint_node)
         elif isinstance(constraint_node, UVLPythonParser.ParenthesisConstraintContext):
-            n = self.process_parenthesis_constraint(constraint_node)
+            process = self.process_parenthesis_constraint(constraint_node)
         elif isinstance(constraint_node, UVLPythonParser.NotConstraintContext):
-            n = self.process_not_constraint(constraint_node)
+            process = self.process_not_constraint(constraint_node)
         elif isinstance(constraint_node, UVLPythonParser.AndConstraintContext):
-            n = self.process_and_constraint(constraint_node)
+            process = self.process_and_constraint(constraint_node)
         elif isinstance(constraint_node, UVLPythonParser.OrConstraintContext):
-            n = self.process_or_constraint(constraint_node)
+            process = self.process_or_constraint(constraint_node)
         elif isinstance(constraint_node, UVLPythonParser.ImplicationConstraintContext):
-            n = self.process_implication_constraint(constraint_node)
+            process = self.process_implication_constraint(constraint_node)
         elif isinstance(constraint_node, UVLPythonParser.EquivalenceConstraintContext):
-            n = self.process_equivalence_constraint(constraint_node)
-            
+            process = self.process_equivalence_constraint(constraint_node)
+
         else:
             # Handle unexpected constraint types
-            raise NotImplementedError(f"Constraint of type {type(constraint_node)} not handled")
-
-        return n
-
-    def process_equation_constraint(self, equation_context: UVLPythonParser.EquationConstraintContext) -> Node:
+            raise NotImplementedError(
+                f"Constraint of type {type(constraint_node)} not handled"
+            )
+
+        return process
+
+    def process_equation_constraint(
+        self, equation_context: UVLPythonParser.EquationConstraintContext
+    ) -> Node:
         """Process an equation constraint."""
         left_expr = equation_context.expression(0)  # Gets the left expression text
-        right_expr = equation_context.expression(1) # Gets the right expression text
-        operator = equation_context.getChild(1).getText()     # Gets the operator
-        return Node(operator, self.process_constraints(left_expr), self.process_constraints(right_expr))
-
-    def process_literal_constraint(self, literal_context: UVLPythonParser.LiteralConstraintContext)-> Node:
+        right_expr = equation_context.expression(1)  # Gets the right expression text
+        operator = equation_context.getChild(1).getText()  # Gets the operator
+        return Node(
+            operator,
+            self.process_constraints(left_expr),
+            self.process_constraints(right_expr),
+        )
+
+    def process_literal_constraint(
+        self, literal_context: UVLPythonParser.LiteralConstraintContext
+    ) -> Node:
         """Process a literal constraint."""
         literal = literal_context.reference()
         return Node(literal.getText())
 
-    def process_parenthesis_constraint(self, parenthesis_context: UVLPythonParser.ParenthesisConstraintContext)-> Node:
+    def process_parenthesis_constraint(
+        self, parenthesis_context: UVLPythonParser.ParenthesisConstraintContext
+    ) -> Node:
         """Process a parenthesis constraint."""
         inner_constraint = parenthesis_context.constraint()
         return self.process_constraints(inner_constraint)
 
-    def process_not_constraint(self, not_context: UVLPythonParser.NotConstraintContext)-> Node:
+    def process_not_constraint(
+        self, not_context: UVLPythonParser.NotConstraintContext
+    ) -> Node:
         """Process a not constraint."""
         inner_constraint = not_context.constraint()
         return Node(ASTOperation.NOT, self.process_constraints(inner_constraint))
 
-    def process_and_constraint(self, and_context: UVLPythonParser.AndConstraintContext)-> Node:
+    def process_and_constraint(
+        self, and_context: UVLPythonParser.AndConstraintContext
+    ) -> Node:
         """Process an and constraint."""
         left_constraint = and_context.constraint(0)
         right_constraint = and_context.constraint(1)
-        return Node(ASTOperation.AND, self.process_constraints(left_constraint), self.process_constraints(right_constraint))
-
-    def process_or_constraint(self, or_context: UVLPythonParser.OrConstraintContext)-> Node:
+        return Node(
+            ASTOperation.AND,
+            self.process_constraints(left_constraint),
+            self.process_constraints(right_constraint),
+        )
+
+    def process_or_constraint(
+        self, or_context: UVLPythonParser.OrConstraintContext
+    ) -> Node:
         """Process an or constraint."""
         left_constraint = or_context.constraint(0)
         right_constraint = or_context.constraint(1)
-        return Node(ASTOperation.OR, self.process_constraints(left_constraint), self.process_constraints(right_constraint))
-
-    def process_implication_constraint(self, implication_context: UVLPythonParser.ImplicationConstraintContext)-> Node:
+        return Node(
+            ASTOperation.OR,
+            self.process_constraints(left_constraint),
+            self.process_constraints(right_constraint),
+        )
+
+    def process_implication_constraint(
+        self, implication_context: UVLPythonParser.ImplicationConstraintContext
+    ) -> Node:
         """Process an implication constraint."""
         left_constraint = implication_context.constraint(0)
         right_constraint = implication_context.constraint(1)
-        return Node(ASTOperation.IMPLIES, self.process_constraints(left_constraint), self.process_constraints(right_constraint))
-
-    def process_equivalence_constraint(self, equivalence_context: UVLPythonParser.EquivalenceConstraintContext)-> Node:
+        return Node(
+            ASTOperation.IMPLIES,
+            self.process_constraints(left_constraint),
+            self.process_constraints(right_constraint),
+        )
+
+    def process_equivalence_constraint(
+        self, equivalence_context: UVLPythonParser.EquivalenceConstraintContext
+    ) -> Node:
         """Process an equivalence constraint."""
         left_constraint = equivalence_context.constraint(0)
         right_constraint = equivalence_context.constraint(1)
-        return Node(ASTOperation.EQUIVALENCE, self.process_constraints(left_constraint), self.process_constraints(right_constraint))
-    
-    def process_includes(self, includes_node):
+        return Node(
+            ASTOperation.EQUIVALENCE,
+            self.process_constraints(left_constraint),
+            self.process_constraints(right_constraint),
+        )
+
+    def process_includes(
+        self, includes_node: UVLPythonParser.IncludesContext
+    ) -> list[str]:
         include_lines = includes_node.includeLine()
 
         # This will hold the processed includes
         includes_list = []
 
         for include_line in include_lines:
             language_level_node = include_line.languageLevel()
             includes_list.append(self.process_language_level(language_level_node))
 
         return includes_list
 
-    def process_language_level(self, language_level_node):
+    def process_language_level(
+        self, language_level_node: UVLPythonParser.LanguageLevelContext
+    ) -> str:
         major_level = language_level_node.majorLevel().getText()
-        
+
         # Check if there's a minor level or a wildcard
         if language_level_node.minorLevel():
             minor_level = language_level_node.minorLevel().getText()
             return f"{major_level}.{minor_level}"
-        elif language_level_node.getChildCount() > 1 and language_level_node.getChild(1).getText() == '*':
+
+        if (
+            language_level_node.getChildCount() > 1
+            and language_level_node.getChild(1).getText() == "*"
+        ):
             return f"{major_level}.*"
-        else:
-            return major_level
 
-    def process_namespace(self, namespace_node):
+        return major_level
+
+    def process_namespace(
+        self, namespace_node: UVLPythonParser.NamespaceContext
+    ) -> str:
         return namespace_node.reference().getText()
 
-    def process_imports(self, imports_node):
+    def process_imports(
+        self, imports_node: UVLPythonParser.ImportsContext
+    ) -> list[tuple[str, Optional[str]]]:
         import_lines = imports_node.importLine()
 
         # This will hold the processed imports
         imports_list = []
 
         for import_line in import_lines:
             namespace = import_line.ns.getText()
-            
+
             # Check if there's an alias
             alias = import_line.alias.getText() if import_line.alias else None
-            
+
             imports_list.append((namespace, alias))
 
         return imports_list
 
     def transform(self) -> FeatureModel:
         self.set_parse_tree()
-        
+
         # Processing the namespace
         namespace_node = self.parse_tree.namespace()
         if namespace_node:
             namespace_value = self.process_namespace(namespace_node)
-            logging.warning("Namespaces are not meningful for Flama.This model has the following namespaces: %s ",namespace_value)
+            logging.warning(
+                "Namespaces are not meningful for Flama."
+                "This model has the following namespaces: %s ",
+                namespace_value,
+            )
 
         # Processing the imports
         imports_node = self.parse_tree.imports()
         if imports_node:
             imports_list = self.process_imports(imports_node)
-            logging.warning("Imports are not yet supported in flama.This model has the following imports: %s", imports_list)
-            
-            
+            logging.warning(
+                "Imports are not yet supported in flama."
+                "This model has the following imports: %s",
+                imports_list,
+            )
+
         includes_node = self.parse_tree.includes()
         if includes_node:
             includes_list = self.process_includes(includes_node)
-            logging.warning("Includes are not yet supported in flama.This model has the following imports: %s", includes_list)
+            logging.warning(
+                "Includes are not yet supported in flama."
+                "This model has the following imports: %s",
+                includes_list,
+            )
 
         # Find ParseTree node of root feature
         root_feature_ast = self.parse_tree.features().feature()
-        #Get the root and process it
+        # Get the root and process it
         feature_text = root_feature_ast.reference().getText()
         feature = Feature(feature_text, [])
-        root=self.process_feature(feature,root_feature_ast)
-        
-        feature_model=FeatureModel(root, [])
-        
+        root = self.process_feature(feature, root_feature_ast)
+
+        feature_model = FeatureModel(root, [])
+
         if self.parse_tree.constraints():  # Check if constraints exist
             contraint_counter = 0
             for constraint_line in self.parse_tree.constraints().constraintLine():
                 node = self.process_constraints(constraint_line.constraint())
-                feature_model.ctcs.append(Constraint(name='Constraint '+str(contraint_counter),ast=AST(node)))
+                feature_model.ctcs.append(
+                    Constraint(
+                        name="Constraint " + str(contraint_counter), ast=AST(node)
+                    )
+                )
                 contraint_counter = contraint_counter + 1
-        self.model=feature_model
-        return self.model
+        self.model = feature_model
+        return self.model
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,55 +9,67 @@
     Relation,
 )
 
 
 class UVLWriter(ModelToText):
     @staticmethod
     def get_destination_extension() -> str:
-        return 'uvl'
+        return "uvl"
 
-    def __init__(self, source_model: FeatureModel, path: str):
+    def __init__(self, path: str, source_model: FeatureModel):
         self.path = path
         self.model = source_model
 
     def transform(self) -> str:
         model = self.model
         root = model.root
 
-        serialized_model = self.read_features(
-            root, "features", 0) + "\n" + self.read_constraints()
+        serialized_model = (
+            self.read_features(root, "features", 0) + "\n" + self.read_constraints()
+        )
 
         if self.path is not None:
-            with open(self.path, 'w', encoding='utf8') as file:
+            with open(self.path, "w", encoding="utf8") as file:
                 file.write(serialized_model)
         return serialized_model
 
     def read_features(self, feature: Feature, result: str, tab_count: int) -> str:
         tab_count = tab_count + 1
-        result = result + "\n" + tab_count * "\t" + \
-             feature.name + " " + self.read_attributes(feature)
+        result = (
+            result
+            + "\n"
+            + tab_count * "\t"
+            + feature.name
+            + " "
+            + self.read_attributes(feature)
+        )
         tab_count = tab_count + 1
         for relation in feature.relations:
             relation_name = self.serialize_relation(relation)
             result = result + "\n" + tab_count * "\t" + relation_name
             for feature_node in relation.children:
                 result = self.read_features(feature_node, result, tab_count)
         return result
 
     @classmethod
     def read_attributes(cls, feature: Feature) -> str:
         attributes = []
         if feature.is_abstract:
-            attributes.append('abstract')
+            attributes.append("abstract")
         for attribute in feature.get_attributes():
             attribute_str = attribute.name
             if attribute.default_value is not None:
-                attribute_str += f' "{attribute.default_value}"'
+                if isinstance(attribute.default_value, str):
+                    attribute_str += f" '{attribute.default_value}'"
+                elif isinstance(attribute.default_value, bool):
+                    attribute_str += f" {str(attribute.default_value).lower()}"
+                else:
+                    attribute_str += f" {attribute.default_value}"
             attributes.append(attribute_str)
-        return f'{{{", ".join(attributes)}}}' if attributes else ''
+        return f'{{{", ".join(attributes)}}}' if attributes else ""
 
     @staticmethod
     def serialize_relation(rel: Relation) -> str:
         result = ""
 
         if rel.is_alternative():
             result = "alternative"
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py` & `flamapy-fm-2.0.0.dev0/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/PKG-INFO` & `flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-fm
-Version: 1.6.0.dev0
+Version: 2.0.0.dev0
 Summary: flamapy-fm is a plugin to Flamapy module
 Home-page: https://github.com/flamapy/fm_metamodel
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-fm-1.6.0.dev0/flamapy_fm.egg-info/SOURCES.txt` & `flamapy-fm-2.0.0.dev0/flamapy_fm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 flamapy/metamodels/fm_metamodel/models/__init__.py
 flamapy/metamodels/fm_metamodel/models/feature_model.py
 flamapy/metamodels/fm_metamodel/operations/__init__.py
 flamapy/metamodels/fm_metamodel/operations/fm_atomic_sets.py
 flamapy/metamodels/fm_metamodel/operations/fm_average_branching_factor.py
 flamapy/metamodels/fm_metamodel/operations/fm_core_features.py
 flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py
-flamapy/metamodels/fm_metamodel/operations/fm_estimated_products_number.py
+flamapy/metamodels/fm_metamodel/operations/fm_estimated_configurations_number.py
 flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py
+flamapy/metamodels/fm_metamodel/operations/fm_generate_random_attribute.py
 flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py
 flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py
 flamapy/metamodels/fm_metamodel/operations/fm_metrics.py
 flamapy/metamodels/fm_metamodel/transformations/__init__.py
 flamapy/metamodels/fm_metamodel/transformations/afm_reader.py
 flamapy/metamodels/fm_metamodel/transformations/afm_writer.py
+flamapy/metamodels/fm_metamodel/transformations/clafer_writer.py
 flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py
+flamapy/metamodels/fm_metamodel/transformations/featureide_writer.py
 flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py
 flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py
+flamapy/metamodels/fm_metamodel/transformations/json_reader.py
 flamapy/metamodels/fm_metamodel/transformations/json_writer.py
+flamapy/metamodels/fm_metamodel/transformations/pysat_to_fm.py
 flamapy/metamodels/fm_metamodel/transformations/splot_writer.py
 flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py
 flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py
 flamapy/metamodels/fm_metamodel/transformations/xml_reader.py
 flamapy_fm.egg-info/PKG-INFO
 flamapy_fm.egg-info/SOURCES.txt
 flamapy_fm.egg-info/dependency_links.txt
```

### Comparing `flamapy-fm-1.6.0.dev0/setup.py` & `flamapy-fm-2.0.0.dev0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-fm",
-    version="1.6.0.dev0",
+    version="2.0.0.dev0",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="flamapy-fm is a plugin to Flamapy module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/fm_metamodel",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
-        'flamapy~=1.6.0.dev0',
+        'flamapy-fw~=2.0.0.dev0',
         'uvlparser~=2.0.1',
         'afmparser~=1.0.3',
     ],
     extras_require={
         'dev': [
             'pytest',
             'pytest-mock',
```

