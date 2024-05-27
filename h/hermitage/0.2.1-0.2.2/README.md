# Comparing `tmp/hermitage-0.2.1.tar.gz` & `tmp/hermitage-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.2.1.tar", max compression
+gzip compressed data, was "hermitage-0.2.2.tar", max compression
```

## Comparing `hermitage-0.2.1.tar` & `hermitage-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       46 2024-05-24 13:40:38.562808 hermitage-0.2.1/README.md
--rw-r--r--   0        0        0      109 2024-05-25 13:54:06.658975 hermitage-0.2.1/hermitage/__init__.py
--rw-r--r--   0        0        0       86 2024-05-25 13:54:06.659245 hermitage-0.2.1/hermitage/adapters/__init__.py
--rw-r--r--   0        0        0      194 2024-05-25 13:54:06.659630 hermitage-0.2.1/hermitage/adapters/constraints.py
--rw-r--r--   0        0        0     4731 2024-05-25 13:54:06.659834 hermitage-0.2.1/hermitage/adapters/cqea.py
--rw-r--r--   0        0        0     1093 2024-05-25 13:54:06.660002 hermitage-0.2.1/hermitage/adapters/transformers.py
--rw-r--r--   0        0        0       24 2024-05-25 13:54:06.660098 hermitage-0.2.1/hermitage/definitions/__init__.py
--rw-r--r--   0        0        0       23 2024-05-25 13:54:06.660260 hermitage-0.2.1/hermitage/definitions/contracts/__init__.py
--rw-r--r--   0        0        0      825 2024-05-26 14:35:33.621440 hermitage-0.2.1/hermitage/definitions/contracts/adapters.py
--rw-r--r--   0        0        0      103 2024-05-25 13:54:06.660580 hermitage-0.2.1/hermitage/notation/__init__.py
--rw-r--r--   0        0        0     4462 2024-05-25 13:54:06.660840 hermitage-0.2.1/hermitage/notation/default.py
--rw-r--r--   0        0        0      418 2024-05-26 14:35:33.602943 hermitage-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-05-24 13:40:38.562808 hermitage-0.2.2/README.md
+-rw-r--r--   0        0        0      109 2024-05-25 13:54:06.658975 hermitage-0.2.2/hermitage/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-25 13:54:06.659245 hermitage-0.2.2/hermitage/adapters/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-25 13:54:06.659630 hermitage-0.2.2/hermitage/adapters/constraints.py
+-rw-r--r--   0        0        0     4731 2024-05-25 13:54:06.659834 hermitage-0.2.2/hermitage/adapters/cqea.py
+-rw-r--r--   0        0        0     1159 2024-05-27 13:18:02.202307 hermitage-0.2.2/hermitage/adapters/transformers.py
+-rw-r--r--   0        0        0       24 2024-05-25 13:54:06.660098 hermitage-0.2.2/hermitage/definitions/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-25 13:54:06.660260 hermitage-0.2.2/hermitage/definitions/contracts/__init__.py
+-rw-r--r--   0        0        0      825 2024-05-26 14:35:33.621440 hermitage-0.2.2/hermitage/definitions/contracts/adapters.py
+-rw-r--r--   0        0        0      103 2024-05-25 13:54:06.660580 hermitage-0.2.2/hermitage/notation/__init__.py
+-rw-r--r--   0        0        0     4462 2024-05-25 13:54:06.660840 hermitage-0.2.2/hermitage/notation/default.py
+-rw-r--r--   0        0        0      418 2024-05-27 13:18:46.795472 hermitage-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 hermitage-0.2.2/PKG-INFO
```

### Comparing `hermitage-0.2.1/hermitage/adapters/cqea.py` & `hermitage-0.2.2/hermitage/adapters/cqea.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.2.1/hermitage/adapters/transformers.py` & `hermitage-0.2.2/hermitage/adapters/transformers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import typing
 
 import zodchy
 from ..notation.default import Clause
 from ..definitions.contracts.adapters import TransformerContract
 
 
-class Inject(TransformerContract):
+class Replace(TransformerContract):
     def __init__(
         self,
-        field_name: str,
-        injection_entity: typing.Any,
-        injection_field: str | None = None
+        search_field: str,
+        replace_field: str | None = None,
+        replace_entity: typing.Any = None,
     ):
-        super().__init__(field_name)
-        self._injection_field = injection_field or field_name
-        self._injection_entity = injection_entity
+        super().__init__(search_field)
+        self._replace_field = replace_field or search_field
+        self._replace_entity = replace_entity
 
     def _apply_value(self, value: typing.Any):
-        if callable(self._injection_entity):
-            return self._injection_entity(value)
+        if callable(self._replace_entity):
+            return self._replace_entity(value)
         return value
 
     def __call__(self, clause: Clause):
         operation = clause.operation
-        if isinstance(operation, zodchy.codex.query.SET):
-            operation = zodchy.codex.query.SET(
-                *[self._apply_value(v) for v in operation.value]
-            )
-        else:
-            operation = type(operation)(self._apply_value(operation.value))
+        if self._replace_entity is not None:
+            if isinstance(operation, zodchy.codex.query.SET):
+                operation = zodchy.codex.query.SET(
+                    *[self._apply_value(v) for v in operation.value]
+                )
+            else:
+                operation = type(operation)(self._apply_value(operation.value))
         clause = Clause(
-            self._injection_field,
+            self._replace_field,
             operation
         )
         return clause
```

### Comparing `hermitage-0.2.1/hermitage/definitions/contracts/adapters.py` & `hermitage-0.2.2/hermitage/definitions/contracts/adapters.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.2.1/hermitage/notation/default.py` & `hermitage-0.2.2/hermitage/notation/default.py`

 * *Files identical despite different names*

### Comparing `hermitage-0.2.1/PKG-INFO` & `hermitage-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermitage
-Version: 0.2.1
+Version: 0.2.2
 Summary: Universal storage access framework
 Home-page: https://github.com/smairon/hermitage
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

