# Comparing `tmp/drf-complex-filter-1.2.1.tar.gz` & `tmp/drf_complex_filter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-complex-filter-1.2.1.tar", last modified: Thu Oct 27 08:37:53 2022, max compression
+gzip compressed data, was "drf_complex_filter-1.3.0.tar", last modified: Mon May 27 14:29:57 2024, max compression
```

## Comparing `drf-complex-filter-1.2.1.tar` & `drf_complex_filter-1.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:53.958390 drf-complex-filter-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/drf_complex_filter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/drf_complex_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/drf_complex_filter/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/drf_complex_filter/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/drf_complex_filter/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/drf_complex_filter/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4654 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/drf_complex_filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-27 08:37:53.000000 drf-complex-filter-1.2.1/drf_complex_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/runtests.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:53.962390 drf-complex-filter-1.2.1/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/test_dynamic_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    11738 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5944 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/test_related_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-27 08:37:38.000000 drf-complex-filter-1.2.1/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:57.669623 drf_complex_filter-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:57.661623 drf_complex_filter-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:57.665623 drf_complex_filter-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-27 14:29:57.669623 drf_complex_filter-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:57.665623 drf_complex_filter-1.3.0/drf_complex_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/drf_complex_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/drf_complex_filter/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/drf_complex_filter/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/drf_complex_filter/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/drf_complex_filter/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/drf_complex_filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:57.669623 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 14:29:57.000000 drf_complex_filter-1.3.0/drf_complex_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 14:29:57.669623 drf_complex_filter-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:57.669623 drf_complex_filter-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:57.669623 drf_complex_filter-1.3.0/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/test_dynamic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/test_related_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-27 14:29:48.000000 drf_complex_filter-1.3.0/tests/views.py
```

### Comparing `drf-complex-filter-1.2.1/.github/workflows/python-publish.yml` & `drf_complex_filter-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/LICENSE` & `drf_complex_filter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/PKG-INFO` & `drf_complex_filter-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-complex-filter
-Version: 1.2.1
+Version: 1.3.0
 Summary: DRF filter for complex queries.
 Home-page: https://github.com/kit-oz/drf-complex-filter
 Author: Nikita Balobanov
 Author-email: kit-oz@ya.ru
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: djangorestframework
 
 # Django Rest Framework Complex Filter
 
 [![codecov](https://codecov.io/gh/kit-oz/drf-complex-filter/branch/main/graph/badge.svg?token=B6Z1LWBXOP)](https://codecov.io/gh/kit-oz/drf-complex-filter)
 
 DRF filter for complex queries
 
@@ -45,15 +46,15 @@
       serializer_class = UserSerializer
       filter_backends = [ComplexQueryFilter]
 
 ```
 
 And get some records
 
-```HTTP
+```
 
   GET /users?filters={"type":"operator","data":{"attribute":"first_name","operator":"=","value":"John"}}
 ```
 
 ## Filter operator
 
 Operator may be one of three types
@@ -209,19 +210,19 @@
   
   # if this RelatedModelName.objects.filter(field_name="value_for_compare") return objects with ids `2, 5, 9`,
   # so this `operator_filter` is equivalent to
   
   new_filter = {
     "type": "operator",
     "data": {
-      "attribute": "RelatedModelNameField_id",
+      "attribute": "RelatedModelName_id",
       "operator": "in",
       "value": [2, 5, 9],
     }
   }
   
   # and have two selects in DB:
-  # `select id from RelatedModelNameField where field_name = 'value_for_compare'`
-  # and `select * from MainTable where RelatedModelNameField_id in (2, 5, 9)`
+  # `select id from RelatedModelName where field_name = 'value_for_compare'`
+  # and `select * from MainTable where RelatedModelName_id in (2, 5, 9)`
 
 ```
```

### Comparing `drf-complex-filter-1.2.1/Pipfile.lock` & `drf_complex_filter-1.3.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/README.md` & `drf_complex_filter-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       serializer_class = UserSerializer
       filter_backends = [ComplexQueryFilter]
 
 ```
 
 And get some records
 
-```HTTP
+```
 
   GET /users?filters={"type":"operator","data":{"attribute":"first_name","operator":"=","value":"John"}}
 ```
 
 ## Filter operator
 
 Operator may be one of three types
@@ -189,18 +189,18 @@
   
   # if this RelatedModelName.objects.filter(field_name="value_for_compare") return objects with ids `2, 5, 9`,
   # so this `operator_filter` is equivalent to
   
   new_filter = {
     "type": "operator",
     "data": {
-      "attribute": "RelatedModelNameField_id",
+      "attribute": "RelatedModelName_id",
       "operator": "in",
       "value": [2, 5, 9],
     }
   }
   
   # and have two selects in DB:
-  # `select id from RelatedModelNameField where field_name = 'value_for_compare'`
-  # and `select * from MainTable where RelatedModelNameField_id in (2, 5, 9)`
+  # `select id from RelatedModelName where field_name = 'value_for_compare'`
+  # and `select * from MainTable where RelatedModelName_id in (2, 5, 9)`
 
-```
+```
```

### Comparing `drf-complex-filter-1.2.1/drf_complex_filter/comparisons.py` & `drf_complex_filter-1.3.0/drf_complex_filter/comparisons.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/drf_complex_filter/filters.py` & `drf_complex_filter-1.3.0/drf_complex_filter/filters.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/drf_complex_filter/utils.py` & `drf_complex_filter-1.3.0/drf_complex_filter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,18 @@
             self.comparisons.update(comparison_module.get_operators())
 
         self.functions = {}
         for function_path in filter_settings["VALUE_FUNCTIONS"]:
             function_module = import_string(function_path)()
             self.functions.update(function_module.get_functions())
 
+        self.default_comparison = None
+        if filter_settings["DEFAULT_COMPARISON_FUNCTION"]:
+            self.default_comparison = import_string(filter_settings["DEFAULT_COMPARISON_FUNCTION"])
+
     def generate_from_string(self, filter_string: str, request=None) -> Optional[Q]:
         try:
             filters = json.loads(filter_string)
         except (TypeError, json.decoder.JSONDecodeError):
             return None
 
         return self.generate_query_from_dict(filters, request)
@@ -39,24 +43,29 @@
         """
         query = None
         annotation = {}
         filter_type = filters["type"]
         if filter_type == "operator":
             condition = filters["data"]
             operator = condition["operator"]
-            if operator in self.comparisons:
-                attribute = condition["attribute"].replace(".", "__")
-                if '___' in attribute:
-                    value = condition.get("value")
-                    attribute, operator, value = self._calculate_subquery(attribute, operator, value, request)
-                else:
-                    value = self.get_filter_value(condition, request)
 
+            attribute = condition["attribute"].replace(".", "__")
+            if '___' in attribute:
+                value = condition.get("value")
+                attribute, operator, value = self._calculate_subquery(attribute, operator, value, request)
+            else:
+                value = self.get_filter_value(condition, request)
+
+            if operator in self.comparisons:
                 result = self.comparisons[operator](attribute, value, request, self.model)
-                (query, annotation) = result if isinstance(result, tuple) else (result, {})
+            elif self.default_comparison:
+                result = self.default_comparison(attribute, operator, value, request, self.model)
+            else:
+                raise ValueError(f"Operator '{operator}' not found")
+            (query, annotation) = result if isinstance(result, tuple) else (result, {})
         elif filter_type == "and":
             for filter_data in filters["data"]:
                 sub_query, sub_annotation = self.generate_query_from_dict(filter_data, request)
                 if sub_query:
                     query = query & sub_query if query else sub_query
                     annotation.update(sub_annotation)
         elif filter_type == "or":
```

### Comparing `drf-complex-filter-1.2.1/drf_complex_filter.egg-info/PKG-INFO` & `drf_complex_filter-1.3.0/drf_complex_filter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-complex-filter
-Version: 1.2.1
+Version: 1.3.0
 Summary: DRF filter for complex queries.
 Home-page: https://github.com/kit-oz/drf-complex-filter
 Author: Nikita Balobanov
 Author-email: kit-oz@ya.ru
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
@@ -13,14 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: djangorestframework
 
 # Django Rest Framework Complex Filter
 
 [![codecov](https://codecov.io/gh/kit-oz/drf-complex-filter/branch/main/graph/badge.svg?token=B6Z1LWBXOP)](https://codecov.io/gh/kit-oz/drf-complex-filter)
 
 DRF filter for complex queries
 
@@ -45,15 +46,15 @@
       serializer_class = UserSerializer
       filter_backends = [ComplexQueryFilter]
 
 ```
 
 And get some records
 
-```HTTP
+```
 
   GET /users?filters={"type":"operator","data":{"attribute":"first_name","operator":"=","value":"John"}}
 ```
 
 ## Filter operator
 
 Operator may be one of three types
@@ -209,19 +210,19 @@
   
   # if this RelatedModelName.objects.filter(field_name="value_for_compare") return objects with ids `2, 5, 9`,
   # so this `operator_filter` is equivalent to
   
   new_filter = {
     "type": "operator",
     "data": {
-      "attribute": "RelatedModelNameField_id",
+      "attribute": "RelatedModelName_id",
       "operator": "in",
       "value": [2, 5, 9],
     }
   }
   
   # and have two selects in DB:
-  # `select id from RelatedModelNameField where field_name = 'value_for_compare'`
-  # and `select * from MainTable where RelatedModelNameField_id in (2, 5, 9)`
+  # `select id from RelatedModelName where field_name = 'value_for_compare'`
+  # and `select * from MainTable where RelatedModelName_id in (2, 5, 9)`
 
 ```
```

### Comparing `drf-complex-filter-1.2.1/drf_complex_filter.egg-info/SOURCES.txt` & `drf_complex_filter-1.3.0/drf_complex_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/setup.cfg` & `drf_complex_filter-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/tests/fixtures.py` & `drf_complex_filter-1.3.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/tests/migrations/0001_initial.py` & `drf_complex_filter-1.3.0/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/tests/models.py` & `drf_complex_filter-1.3.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/tests/serializer.py` & `drf_complex_filter-1.3.0/tests/serializer.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/tests/test_dynamic_filter.py` & `drf_complex_filter-1.3.0/tests/test_dynamic_filter.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/tests/test_filter.py` & `drf_complex_filter-1.3.0/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `drf-complex-filter-1.2.1/tests/test_related_query.py` & `drf_complex_filter-1.3.0/tests/test_related_query.py`

 * *Files identical despite different names*

