# Comparing `tmp/cap_tools-2.4.0.tar.gz` & `tmp/cap_tools-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cap_tools-2.4.0.tar", max compression
+gzip compressed data, was "cap_tools-2.5.0.tar", max compression
```

## Comparing `cap_tools-2.4.0.tar` & `cap_tools-2.5.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-27 19:41:22.929494 cap_tools-2.4.0/LICENSE
--rw-r--r--   0        0        0     4900 2024-05-27 19:41:22.929494 cap_tools-2.4.0/README.md
--rw-r--r--   0        0        0     1937 2024-05-27 19:41:22.933494 cap_tools-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      530 2024-05-27 19:41:22.933494 cap_tools-2.4.0/src/cap_tools/__init__.py
--rw-r--r--   0        0        0    15087 2024-05-27 19:41:22.933494 cap_tools-2.4.0/src/cap_tools/models.py
--rw-r--r--   0        0        0     5431 1970-01-01 00:00:00.000000 cap_tools-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-27 19:41:22.721122 cap_tools-2.5.0/LICENSE
+-rw-r--r--   0        0        0     5301 2024-05-27 19:41:22.721122 cap_tools-2.5.0/README.md
+-rw-r--r--   0        0        0     1978 2024-05-27 19:41:22.721122 cap_tools-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      530 2024-05-27 19:41:22.721122 cap_tools-2.5.0/src/cap_tools/__init__.py
+-rw-r--r--   0        0        0    15865 2024-05-27 19:41:22.721122 cap_tools-2.5.0/src/cap_tools/models.py
+-rw-r--r--   0        0        0      321 2024-05-27 19:41:22.725122 cap_tools-2.5.0/src/cap_tools/utils.py
+-rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 cap_tools-2.5.0/PKG-INFO
```

### Comparing `cap_tools-2.4.0/LICENSE` & `cap_tools-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cap_tools-2.4.0/README.md` & `cap_tools-2.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -66,14 +66,18 @@
 >>> area.geocodes_from_dict({"foo": "bar", "lorem": "ipsum"})
 >>> area.geocodes
 [Geocode(value_name=ValueName(value='foo'), value=Value(value='bar')), Geocode(value_name=ValueName(value='lorem'), value=Value(value='ipsum'))]
 ```
 
 The MultiDicts do not retain any connection to the model. In all cases, the internal state is always represented by the list of containers of key-value-pairs.
 
+#### Splitting group listings
+
+The attributes `addresses`, `references` and `incidents` of `Alert` store multiple values as "group listings", i.e. multiple values are space-delimited. You can split these attributes by using `Alert.addresses_to_list()`, `Alert.references_to_list()` and `Alert.incidents_to_list()` and write back to them with corresponding `Alert.*_from_list()` methods respectively.
+
 #### Awareness of "en-US" as the default language
 
 When no language is explicitly defined on an Info element, "en-US" is assumed per CAP spec. This library implements this behavior neither by using default values nor by using descriptor fields.
 
 ```python
 >>> alert.infos[0].language = "en-US"
 >>> alert.infos[0].language
```

### Comparing `cap_tools-2.4.0/pyproject.toml` & `cap_tools-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 version_scheme = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 
 [tool.coverage.run]
 source = ["src", "tests"]
 
+[tool.mypy]
+strict = true
+files = "src"
+
 [tool.poetry]
 name = "cap-tools"
-version = "2.4.0"
+version = "2.5.0"
 description = "Python data bindings for the Common Alerting Protocol Version."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "cap_tools", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cap_tools-2.4.0/src/cap_tools/__init__.py` & `cap_tools-2.5.0/src/cap_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cap_tools-2.4.0/src/cap_tools/models.py` & `cap_tools-2.5.0/src/cap_tools/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from dataclasses import dataclass, field
 from decimal import Decimal
 from enum import Enum
 
 from multidict import MultiDict
 from xsdata.models.datatype import XmlDateTime
 
+from cap_tools.utils import join_and_maybe_add_quotes, split_and_remove_quotes
+
 __NAMESPACE__ = "urn:oasis:names:tc:emergency:cap:1.2"
 DEFAULT_LANGUAGE = "en-US"
 
 
 class Category(Enum):
     GEO = "Geo"
     MET = "Met"
@@ -597,7 +599,25 @@
     _signatures: list[object] = field(
         default_factory=list,
         metadata={
             "type": "Wildcard",
             "namespace": "http://www.w3.org/2000/09/xmldsig#",
         },
     )
+
+    def addresses_to_list(self) -> list[str]:
+        return split_and_remove_quotes(self.addresses)
+
+    def addresses_from_list(self, addressees: list[str]) -> None:
+        self.addresses = join_and_maybe_add_quotes(addressees)
+
+    def references_to_list(self) -> list[str]:
+        return split_and_remove_quotes(self.references)
+
+    def references_from_list(self, references: list[str]) -> None:
+        self.references = join_and_maybe_add_quotes(references)
+
+    def incidents_to_list(self) -> list[str]:
+        return split_and_remove_quotes(self.incidents)
+
+    def incidents_from_list(self, incidents: list[str]) -> None:
+        self.incidents = join_and_maybe_add_quotes(incidents)
```

### Comparing `cap_tools-2.4.0/PKG-INFO` & `cap_tools-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cap-tools
-Version: 2.4.0
+Version: 2.5.0
 Summary: Python data bindings for the Common Alerting Protocol Version.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -81,14 +81,18 @@
 >>> area.geocodes_from_dict({"foo": "bar", "lorem": "ipsum"})
 >>> area.geocodes
 [Geocode(value_name=ValueName(value='foo'), value=Value(value='bar')), Geocode(value_name=ValueName(value='lorem'), value=Value(value='ipsum'))]
 ```
 
 The MultiDicts do not retain any connection to the model. In all cases, the internal state is always represented by the list of containers of key-value-pairs.
 
+#### Splitting group listings
+
+The attributes `addresses`, `references` and `incidents` of `Alert` store multiple values as "group listings", i.e. multiple values are space-delimited. You can split these attributes by using `Alert.addresses_to_list()`, `Alert.references_to_list()` and `Alert.incidents_to_list()` and write back to them with corresponding `Alert.*_from_list()` methods respectively.
+
 #### Awareness of "en-US" as the default language
 
 When no language is explicitly defined on an Info element, "en-US" is assumed per CAP spec. This library implements this behavior neither by using default values nor by using descriptor fields.
 
 ```python
 >>> alert.infos[0].language = "en-US"
 >>> alert.infos[0].language
```

