# Comparing `tmp/json_schema_tool-0.2.0.tar.gz` & `tmp/json_schema_tool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_schema_tool-0.2.0.tar", last modified: Wed Jan 31 23:33:07 2024, max compression
+gzip compressed data, was "json_schema_tool-0.3.0.tar", last modified: Mon May 27 17:39:17 2024, max compression
```

## Comparing `json_schema_tool-0.2.0.tar` & `json_schema_tool-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 23:33:07.823900 json_schema_tool-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-01-31 23:33:07.823900 json_schema_tool-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 23:33:07.823900 json_schema_tool-0.2.0/json_schema_tool/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/json_schema_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/json_schema_tool/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/json_schema_tool/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/json_schema_tool/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/json_schema_tool/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52143 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/json_schema_tool/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/json_schema_tool/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 23:33:07.823900 json_schema_tool-0.2.0/json_schema_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-01-31 23:33:07.000000 json_schema_tool-0.2.0/json_schema_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-31 23:33:07.000000 json_schema_tool-0.2.0/json_schema_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 23:33:07.000000 json_schema_tool-0.2.0/json_schema_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-31 23:33:07.000000 json_schema_tool-0.2.0/json_schema_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-31 23:33:07.000000 json_schema_tool-0.2.0/json_schema_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-31 23:33:02.000000 json_schema_tool-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 23:33:07.823900 json_schema_tool-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 23:33:07.823900 json_schema_tool-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/test/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/test/test_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-01-31 23:32:58.000000 json_schema_tool-0.2.0/test/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:39:17.918569 json_schema_tool-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-27 17:39:17.918569 json_schema_tool-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:39:17.918569 json_schema_tool-0.3.0/json_schema_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/json_schema_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/json_schema_tool/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/json_schema_tool/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/json_schema_tool/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/json_schema_tool/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56042 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/json_schema_tool/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/json_schema_tool/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:39:17.918569 json_schema_tool-0.3.0/json_schema_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-27 17:39:17.000000 json_schema_tool-0.3.0/json_schema_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 17:39:17.000000 json_schema_tool-0.3.0/json_schema_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 17:39:17.000000 json_schema_tool-0.3.0/json_schema_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 17:39:17.000000 json_schema_tool-0.3.0/json_schema_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 17:39:17.000000 json_schema_tool-0.3.0/json_schema_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-27 17:39:15.000000 json_schema_tool-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 17:39:17.918569 json_schema_tool-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 17:39:17.918569 json_schema_tool-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/test/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/test/test_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-05-27 17:39:10.000000 json_schema_tool-0.3.0/test/test_types.py
```

### Comparing `json_schema_tool-0.2.0/LICENSE` & `json_schema_tool-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_schema_tool-0.2.0/PKG-INFO` & `json_schema_tool-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_schema_tool
-Version: 0.2.0
+Version: 0.3.0
 Summary: JSON Schema validation with various additional features
 License: MIT License
         
         Copyright (c) 2023 Institut für Automation und Kommunikation e.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `json_schema_tool-0.2.0/README.md` & `json_schema_tool-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `json_schema_tool-0.2.0/json_schema_tool/coverage.py` & `json_schema_tool-0.3.0/json_schema_tool/coverage.py`

 * *Files identical despite different names*

### Comparing `json_schema_tool-0.2.0/json_schema_tool/pointer.py` & `json_schema_tool-0.3.0/json_schema_tool/pointer.py`

 * *Files identical despite different names*

### Comparing `json_schema_tool-0.2.0/json_schema_tool/schema.py` & `json_schema_tool-0.3.0/json_schema_tool/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from json_schema_tool.types import JsonType, JsonValue
-from .types import from_typename, JsonType, from_instance, values_are_equal, JsonTypes, ALL_JSON_TYPES
+from .types import from_typename, JsonValue, from_instance, values_are_equal, JsonTypes, ALL_JSON_TYPES, JsonType
 from .pointer import JsonPointer
-
 from typing import Dict, List, Optional, Set, Callable, Pattern, Tuple
 from .exception import InvalidSchemaException, TypeException, JsonPointerException, PreprocessorException
 
 import re
 from dataclasses import dataclass, field
 import warnings
 import operator
@@ -193,14 +191,89 @@
             if self.then_validator:
                 self._types |= self.then_validator.get_types()
             if self.else_validator:
                 self._types |= self.else_validator.get_types()
         return self._types
 
 
+class DiscriminatorValidator(KeywordsValidator):
+    def __init__(self, parent: "DictSchemaValidator", unparsed_keys: Set[str], config: ParseConfig):
+        super().__init__(parent, unparsed_keys, config)
+        data = parent._read_dict('discriminator', unparsed_keys)
+        self.property_name = data.get('propertyName')
+        if not isinstance(self.property_name, str):
+            raise InvalidSchemaException(f"propertyName must be a string, got {self.property_name} at {parent.pointer}")
+        _remove_if_exists(unparsed_keys, 'anyOf')
+        _remove_if_exists(unparsed_keys, 'oneOf')
+        self.mapping: Dict[str, "ReferenceValidator"] = {}
+        self._collect_refs(False, self.parent.schema, self.parent.pointer, self.mapping, config)
+
+    def _collect_refs(self, is_child: bool, schema: dict, pointer: JsonPointer, refs: Dict[str, "ReferenceValidator"], config: ParseConfig):
+        aggregators = []
+        for key in ['anyOf', 'oneOf']:
+            try:
+                aggregators.append((key, schema[key]))
+            except KeyError:
+                pass
+        if len(aggregators) != 1:
+            if is_child:
+                return
+            else:
+                raise InvalidSchemaException("discriminator requires either anyOf or oneOf")
+        keyword, entries = aggregators[0]
+        if not isinstance(entries, list):
+            raise InvalidSchemaException("Entries must be a list")
+        for idx, entry in enumerate(entries):
+            if not isinstance(entry, dict):
+                raise InvalidSchemaException(f"Entry {idx} is invalid")
+            if len(entry.keys()) != 1:
+                if is_child:
+                    continue
+                else:
+                    raise InvalidSchemaException(f"Entry {idx} must contain exactly one key: $ref")
+            key, value = next(iter(entry.items()))
+            if key == '$ref':
+                sub_pointer = pointer + keyword + idx
+                # TODO: construct ReferenceValidator directly?
+                validator = _construct(entry, sub_pointer, self.parent.globals, config)
+                assert isinstance(validator, DictSchemaValidator)
+                assert len(validator.kw_validators) == 1
+                ref_validator = validator.kw_validators[0]
+                assert isinstance(ref_validator, ReferenceValidator)
+                refs[value] = ref_validator
+                self._collect_refs(True, ref_validator.ref_validator.schema, sub_pointer, refs, config)
+            else:
+                raise InvalidSchemaException(f"Entry {idx}: expected $ref, oneOf or anyOf, got {value}")
+
+    def invoke(self, instance: JsonValue, config: ValidationConfig) -> List[KeywordValidationResult]:
+        if not isinstance(instance, dict):
+            return [KeywordValidationResult(['discriminator'], [], 'Expected an object')]
+        try:
+            property_value = instance[self.property_name]
+        except KeyError:
+            return [KeywordValidationResult(['discriminator'], [], f"Property '{self.property_name}' is missing")]
+        if not isinstance(property_value, str):
+            return [KeywordValidationResult(['discriminator'], [], f"Property '{self.property_name}' must be a string")]
+
+        property_value = '/' + property_value  # to avoid conflicts with duplicate suffixes
+        for key, validator in self.mapping.items():
+            if key.endswith(property_value):
+                return validator.invoke(instance, config)
+        return [KeywordValidationResult(['discriminator'], [], f"Property '{self.property_name}' has invalid value '{property_value}'")]
+
+    def get_types(self) -> JsonTypes:
+        return set([JsonType.OBJECT])
+
+    def sub_pointers(self) -> List[List[str]]:
+        return [[]] # TODO
+
+    def sub_schemas(self) -> List["SchemaValidator"]:
+        return [[]] # TODO
+
+
 class AggregatingValidator(KeywordsValidator):
     """
     Base class for allOf, anyOf and oneOf validators
     """
     keyword = ''
 
     def __init__(self, parent: "DictSchemaValidator", unparsed_keys: Set[str], config: ParseConfig):
@@ -1159,14 +1232,15 @@
 
     validators_by_key = [
         ('not', NotValidator),
         ('if', IfThenElseValidator),
         ('then', IfThenElseValidator),
         ('else', IfThenElseValidator),
         ('allOf', AllOfValidator),
+        ('discriminator', DiscriminatorValidator),  # overwrites anyOf / oneOf
         ('anyOf', AnyOfValidator),
         ('oneOf', OneOfValidator),
         ('$ref', ReferenceValidator),
         ('prefixItems', ArrayItemsValidator),
         ('items', ArrayItemsValidator),
         ('minItems', ArrayMinItemsValidator),
         ('maxItems', ArrayMaxItemsValidator),
@@ -1332,8 +1406,8 @@
     if schema is False:
         return NothingValidator(pointer, globals)
     elif schema is True:
         return AnyValidator(pointer, globals)
     elif isinstance(schema, dict):
         return DictSchemaValidator(schema, pointer, globals, config)
     else:
-        raise InvalidSchemaException(f"Schema must be a bool or dict, got {type(schema)}")
+        raise InvalidSchemaException(f"Schema must be a bool or dict, got {type(schema)} at {pointer}")
```

### Comparing `json_schema_tool-0.2.0/json_schema_tool/types.py` & `json_schema_tool-0.3.0/json_schema_tool/types.py`

 * *Files identical despite different names*

### Comparing `json_schema_tool-0.2.0/json_schema_tool.egg-info/PKG-INFO` & `json_schema_tool-0.3.0/json_schema_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_schema_tool
-Version: 0.2.0
+Version: 0.3.0
 Summary: JSON Schema validation with various additional features
 License: MIT License
         
         Copyright (c) 2023 Institut für Automation und Kommunikation e.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `json_schema_tool-0.2.0/json_schema_tool.egg-info/SOURCES.txt` & `json_schema_tool-0.3.0/json_schema_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json_schema_tool-0.2.0/pyproject.toml` & `json_schema_tool-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "json_schema_tool"
-version = "0.2.0"
+version = "0.3.0"
 description = "JSON Schema validation with various additional features"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `json_schema_tool-0.2.0/test/test_coverage.py` & `json_schema_tool-0.3.0/test/test_coverage.py`

 * *Files identical despite different names*

### Comparing `json_schema_tool-0.2.0/test/test_types.py` & `json_schema_tool-0.3.0/test/test_types.py`

 * *Files identical despite different names*

