# Comparing `tmp/eip712_clearsign-2.0.0rc1.tar.gz` & `tmp/eip712_clearsign-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eip712_clearsign-2.0.0rc1.tar", last modified: Wed May 22 09:30:30 2024, max compression
+gzip compressed data, was "eip712_clearsign-2.0.0rc2.tar", last modified: Mon May 27 08:20:54 2024, max compression
```

## Comparing `eip712_clearsign-2.0.0rc1.tar` & `eip712_clearsign-2.0.0rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-22 09:30:30.710498 eip712_clearsign-2.0.0rc1/
--rw-r--r--   0 runner    (1001) runner    (1001)     1063 2024-05-22 09:29:40.000000 eip712_clearsign-2.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-22 09:30:30.710498 eip712_clearsign-2.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2024-05-22 09:29:40.000000 eip712_clearsign-2.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-22 09:30:30.706498 eip712_clearsign-2.0.0rc1/eip712/
--rw-r--r--   0 runner    (1001) runner    (1001)     9929 2024-05-22 09:29:40.000000 eip712_clearsign-2.0.0rc1/eip712/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-22 09:30:30.710498 eip712_clearsign-2.0.0rc1/eip712_clearsign.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-22 09:30:30.000000 eip712_clearsign-2.0.0rc1/eip712_clearsign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      265 2024-05-22 09:30:30.000000 eip712_clearsign-2.0.0rc1/eip712_clearsign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-22 09:30:30.000000 eip712_clearsign-2.0.0rc1/eip712_clearsign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-05-22 09:30:30.000000 eip712_clearsign-2.0.0rc1/eip712_clearsign.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        7 2024-05-22 09:30:30.000000 eip712_clearsign-2.0.0rc1/eip712_clearsign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-22 09:30:30.710498 eip712_clearsign-2.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-05-22 09:29:40.000000 eip712_clearsign-2.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-22 09:30:30.710498 eip712_clearsign-2.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)    15343 2024-05-22 09:29:40.000000 eip712_clearsign-2.0.0rc1/tests/test_eip712.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1063 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/eip712/
+-rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/eip712/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2432 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      265 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        7 2024-05-27 08:20:54.000000 eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      720 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-27 08:20:54.118771 eip712_clearsign-2.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)    15343 2024-05-27 08:20:01.000000 eip712_clearsign-2.0.0rc2/tests/test_eip712.py
```

### Comparing `eip712_clearsign-2.0.0rc1/LICENSE` & `eip712_clearsign-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `eip712_clearsign-2.0.0rc1/PKG-INFO` & `eip712_clearsign-2.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712-clearsign
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Parse eip712 clear sign descriptors
 Home-page: https://github.com/LedgerHQ/python-eip712
 Author: Ledger
 Author-email: hello@ledger.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eip712_clearsign-2.0.0rc1/README.md` & `eip712_clearsign-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `eip712_clearsign-2.0.0rc1/eip712/__init__.py` & `eip712_clearsign-2.0.0rc2/eip712/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,32 @@
 from enum import Enum
 from functools import cached_property
 from typing import ClassVar, Iterator, List, Optional
 
 from pydantic import BaseModel, Field, model_validator
 
 # For more details on the serialisation spec, head over to
-# https://github.com/LedgerHQ/app-ethereum/blob/apr/feature/eip712/doc/ethapp.adoc#eip712-filtering
+# https://github.com/LedgerHQ/app-ethereum/blob/develop/doc/ethapp.adoc#eip712-filtering
 
 
 class EIP712Version(Enum):
     V1 = 1
     V2 = 2
 
     def __repr__(self):
         return "EIP712Version" + self.name
 
 
+class EIP712Format(Enum):
+    TOKEN = "token"
+    AMOUNT = "amount"
+    RAW = "raw"
+    DATETIME = "datetime"
+
+
 @dataclass
 class EIP712BaseMapper:
     chain_id: int
     contract_address: str
     schema: dict
     display_name: str
     TYPE_PREFIX: ClassVar[int]
@@ -60,14 +67,15 @@
             f"{self.additional_hash(version)}"
         )
 
 
 @dataclass
 class EIP712FieldMapper(EIP712BaseMapper):
     field_path: str
+    format: ClassVar[EIP712Format]
 
     def type_prefix_hash(self, version: EIP712Version) -> str:
         match version:
             case EIP712Version.V1:
                 return (72).to_bytes(1, byteorder="big").hex()
             case _:
                 return self.TYPE_PREFIX.to_bytes(1, byteorder="big").hex()
@@ -75,78 +83,77 @@
     def additional_hash(self, version: EIP712Version) -> str:
         return f"{self.field_path.encode('utf-8').hex()}" f"{self.display_name_hash}"
 
 
 @dataclass
 class EIP712RawFieldMapper(EIP712FieldMapper):
     TYPE_PREFIX: ClassVar[int] = 72
+    format: ClassVar[EIP712Format] = EIP712Format.RAW
 
 
 @dataclass
 class EIP712AmountJoinTokenFieldMapper(EIP712FieldMapper):
     TYPE_PREFIX: ClassVar[int] = 11
+    format: ClassVar[EIP712Format] = EIP712Format.TOKEN
+
     coin_ref: Optional[int]
 
     def additional_hash(self, version: EIP712Version) -> str:
         if version == EIP712Version.V1:
             return super().additional_hash(version)
         else:
-            coinRefHash = (
+            coin_ref_hash = (
                 self.coin_ref.to_bytes(1, byteorder="big").hex()
                 if self.coin_ref is not None
                 else ""
             )
-            return f"{self.field_path.encode('utf-8').hex()}" f"{coinRefHash}"
+            return f"{self.field_path.encode('utf-8').hex()}" f"{coin_ref_hash}"
 
 
 @dataclass
 class EIP712AmountJoinValueFieldMapper(EIP712FieldMapper):
     TYPE_PREFIX: ClassVar[int] = 22
+    format: ClassVar[EIP712Format] = EIP712Format.AMOUNT
+
     coin_ref: Optional[int]
 
     def additional_hash(self, version: EIP712Version) -> str:
         if version == EIP712Version.V1:
             return super().additional_hash(version)
         else:
-            coinRefHash = (
+            coin_ref_hash = (
                 self.coin_ref.to_bytes(1, byteorder="big").hex()
                 if self.coin_ref is not None
                 else ""
             )
             return (
                 f"{self.field_path.encode('utf-8').hex()}"
                 f"{self.display_name_hash}"
-                f"{coinRefHash}"
+                f"{coin_ref_hash}"
             )
 
 
 @dataclass
 class EIP712DatetimeFieldMapper(EIP712FieldMapper):
     TYPE_PREFIX: ClassVar[int] = 33
+    format: ClassVar[EIP712Format] = EIP712Format.DATETIME
 
 
 @dataclass
 class EIP712MessageNameMapper(EIP712BaseMapper):
     field_mappers_count: int
     TYPE_PREFIX: ClassVar[int] = 183
 
     def additional_hash(self, version: EIP712Version) -> str:
         return (
             f"{self.field_mappers_count.to_bytes(1, byteorder='big').hex()}"
             f"{self.display_name_hash}"
         )
 
 
-class EIP712Format(Enum):
-    TOKEN = "token"
-    AMOUNT = "amount"
-    RAW = "raw"
-    DATETIME = "datetime"
-
-
 class EIP712Field(BaseModel):
     path: str
     label: str
     assetPath: Optional[str] = None
     format: Optional[EIP712Format] = None
     coinRef: Optional[int] = None
 
@@ -178,15 +185,14 @@
                 )
 
 
 class EIP712Mapper(BaseModel):
     label: str
     fields: List[EIP712Field]
 
-    @model_validator(mode="after")
     def update_field_index(self):
 
         coin_refs = dict()
         idx: int = 0
 
         for field in self.fields:
             path: str | None = None
@@ -201,14 +207,18 @@
                 else:
                     coin_refs[path] = idx
                     field.coinRef = idx
                     idx += 1
 
         return self
 
+    @model_validator(mode="after")
+    def _update_field_index(self):
+        return self.update_field_index()
+
     def mappers(self, **mapper_data) -> Iterator[EIP712BaseMapper]:
         yield EIP712MessageNameMapper(
             field_mappers_count=len(self.fields),
             display_name=self.label,
             **mapper_data,
         )
         for field in self.fields:
@@ -219,15 +229,15 @@
     schema_: dict = Field(alias="schema")
     mapper: EIP712Mapper
 
     def mappers(self, **mapper_data) -> Iterator[EIP712BaseMapper]:
         return self.mapper.mappers(schema=self.schema_, **mapper_data)
 
     @classmethod
-    def __schema_top_level_type(cls, schema: dict):
+    def _schema_top_level_type(cls, schema: dict):
         """Given a schema, generate a new message descriptor"""
         filtered_schema: dict = {
             type_name: type_fields
             for type_name, type_fields in schema.items()
             if type_name != "EIP712Domain"
         }
         all_type_names = {
@@ -238,44 +248,44 @@
         return next(
             type_name
             for type_name in filtered_schema.keys()
             if type_name not in all_type_names
         )
 
     @classmethod
-    def __type_names(cls, schema: dict, target_type_name: str) -> Iterator[List[str]]:
+    def _type_names(cls, schema: dict, target_type_name: str) -> Iterator[List[str]]:
         """Recursively generate the list of fields to reach an object with a basic type"""
         for type_fields in schema[target_type_name]:
             name_list = [type_fields["name"]]
             short_type = type_fields["type"].removesuffix("[]")
             if short_type != type_fields["type"]:
                 name_list.append("[]")
             if short_type in schema:
-                for recursive_name_list in cls.__type_names(
+                for recursive_name_list in cls._type_names(
                     schema=schema, target_type_name=short_type
                 ):
                     yield name_list + recursive_name_list
             else:
                 yield name_list
 
     @classmethod
     def from_schema(cls, schema: dict):
-        top_level_type_name = cls.__schema_top_level_type(schema)
+        top_level_type_name = cls._schema_top_level_type(schema)
 
         mapper_fields = []
 
-        for name_list in cls.__type_names(
+        for name_list in cls._type_names(
             schema=schema, target_type_name=top_level_type_name
         ):
             field_label = f"{top_level_type_name} {' '.join(name_list)}"
             field_path = f"{'.'.join(name_list)}"
             mapper_fields.append(EIP712Field(path=field_path, label=field_label))
 
         mapper = EIP712Mapper(label=top_level_type_name, fields=mapper_fields)
-        mapper.update_field_index
+        mapper.update_field_index()
         clazz = cls(schema=schema, mapper=mapper)
         return clazz
 
 
 class EIP712ContractDescriptor(BaseModel):
     address: str
     name: str = Field(alias="contractName")
```

### Comparing `eip712_clearsign-2.0.0rc1/eip712_clearsign.egg-info/PKG-INFO` & `eip712_clearsign-2.0.0rc2/eip712_clearsign.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eip712-clearsign
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Parse eip712 clear sign descriptors
 Home-page: https://github.com/LedgerHQ/python-eip712
 Author: Ledger
 Author-email: hello@ledger.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eip712_clearsign-2.0.0rc1/setup.py` & `eip712_clearsign-2.0.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="eip712-clearsign",
-    version="2.0.0rc1",
+    version="2.0.0rc2",
     url="https://github.com/LedgerHQ/python-eip712",
     author="Ledger",
     author_email="hello@ledger.com",
     description="Parse eip712 clear sign descriptors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["pydantic"],
```

### Comparing `eip712_clearsign-2.0.0rc1/tests/test_eip712.py` & `eip712_clearsign-2.0.0rc2/tests/test_eip712.py`

 * *Files identical despite different names*

