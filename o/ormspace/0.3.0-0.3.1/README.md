# Comparing `tmp/ormspace-0.3.0.tar.gz` & `tmp/ormspace-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ormspace-0.3.0.tar", max compression
+gzip compressed data, was "ormspace-0.3.1.tar", max compression
```

## Comparing `ormspace-0.3.0.tar` & `ormspace-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1102 2023-11-06 03:14:04.669967 ormspace-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-10-30 03:22:14.039503 ormspace-0.3.0/ormspace/__init__.py
--rw-r--r--   0        0        0      911 2023-12-22 00:50:03.002684 ormspace-0.3.0/ormspace/alias.py
--rw-r--r--   0        0        0     2336 2024-01-24 15:13:51.647527 ormspace-0.3.0/ormspace/annotations.py
--rw-r--r--   0        0        0     7489 2024-01-21 18:54:05.965230 ormspace-0.3.0/ormspace/bases.py
--rw-r--r--   0        0        0     4188 2024-01-21 19:04:07.719406 ormspace-0.3.0/ormspace/containers.py
--rw-r--r--   0        0        0      434 2024-01-06 02:20:03.592508 ormspace-0.3.0/ormspace/context.py
--rw-r--r--   0        0        0    11507 2024-01-21 20:43:04.610652 ormspace-0.3.0/ormspace/database.py
--rw-r--r--   0        0        0     1532 2023-12-23 17:32:46.605145 ormspace-0.3.0/ormspace/enum.py
--rw-r--r--   0        0        0      246 2023-12-07 04:08:04.710269 ormspace-0.3.0/ormspace/exception.py
--rw-r--r--   0        0        0     9729 2024-01-26 01:59:43.639314 ormspace-0.3.0/ormspace/functions.py
--rw-r--r--   0        0        0     5656 2024-01-08 18:15:56.958386 ormspace-0.3.0/ormspace/keys.py
--rw-r--r--   0        0        0     2168 2024-01-02 13:04:03.513124 ormspace-0.3.0/ormspace/metainfo.py
--rw-r--r--   0        0        0    14927 2024-01-26 02:01:55.736534 ormspace-0.3.0/ormspace/model.py
--rw-r--r--   0        0        0     1171 2024-01-22 04:48:03.926322 ormspace-0.3.0/ormspace/settings.py
--rw-r--r--   0        0        0      570 2024-01-26 02:02:39.692106 ormspace-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1939 2024-01-26 02:02:48.067970 ormspace-0.3.0/setup.py
--rw-r--r--   0        0        0     1823 2024-01-26 02:02:48.068235 ormspace-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-11-06 03:14:04.669967 ormspace-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-10-30 03:22:14.039503 ormspace-0.3.1/ormspace/__init__.py
+-rw-r--r--   0        0        0      917 2024-05-26 23:55:52.898510 ormspace-0.3.1/ormspace/alias.py
+-rw-r--r--   0        0        0     2434 2024-05-26 23:55:54.459213 ormspace-0.3.1/ormspace/annotations.py
+-rw-r--r--   0        0        0     7489 2024-05-26 23:55:53.676380 ormspace-0.3.1/ormspace/bases.py
+-rw-r--r--   0        0        0     4188 2024-01-21 19:04:07.719406 ormspace-0.3.1/ormspace/containers.py
+-rw-r--r--   0        0        0      434 2024-01-06 02:20:03.592508 ormspace-0.3.1/ormspace/context.py
+-rw-r--r--   0        0        0    11507 2024-01-21 20:43:04.610652 ormspace-0.3.1/ormspace/database.py
+-rw-r--r--   0        0        0     1453 2024-05-26 23:29:34.140489 ormspace-0.3.1/ormspace/enum.py
+-rw-r--r--   0        0        0      246 2023-12-07 04:08:04.710269 ormspace-0.3.1/ormspace/exception.py
+-rw-r--r--   0        0        0     9937 2024-05-26 23:55:52.909008 ormspace-0.3.1/ormspace/functions.py
+-rw-r--r--   0        0        0     5656 2024-01-08 18:15:56.958386 ormspace-0.3.1/ormspace/keys.py
+-rw-r--r--   0        0        0     2168 2024-01-02 13:04:03.513124 ormspace-0.3.1/ormspace/metainfo.py
+-rw-r--r--   0        0        0    14398 2024-05-26 23:26:08.729330 ormspace-0.3.1/ormspace/model.py
+-rw-r--r--   0        0        0     1171 2024-01-22 04:48:03.926322 ormspace-0.3.1/ormspace/settings.py
+-rw-r--r--   0        0        0      570 2024-05-26 23:56:38.034597 ormspace-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1939 2024-05-26 23:59:32.024659 ormspace-0.3.1/setup.py
+-rw-r--r--   0        0        0     1823 2024-05-26 23:59:32.025569 ormspace-0.3.1/PKG-INFO
```

### Comparing `ormspace-0.3.0/README.md` & `ormspace-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ormspace-0.3.0/ormspace/alias.py` & `ormspace-0.3.1/ormspace/alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 from typing import Optional, Union
 
 from typing_extensions import TypeAlias
 
 TABLE: TypeAlias = str
 KEY: TypeAlias = Optional[str]
-DATA: TypeAlias = Union[dict, list, str, int, float, bool]
+DATA: TypeAlias = Union[dict, list, str, int, float, bool, None]
 JSONPRIMITIVE: TypeAlias = Union[str, int, float, bool, None]
 JSONLIST: TypeAlias = list[JSONPRIMITIVE]
 JSONDICT: TypeAlias = Union[str, Union[JSONPRIMITIVE, dict[str, JSONPRIMITIVE], JSONLIST]]
 JSON: TypeAlias = Union[JSONPRIMITIVE, JSONDICT, JSONLIST]
 EXPIRE_IN: TypeAlias = Optional[int]
 EXPIRE_AT: TypeAlias = Union[int, float, datetime.datetime, None]
 QUERY: TypeAlias = Union[dict[str, JSONPRIMITIVE], list[dict[str, JSONPRIMITIVE]], None]
```

### Comparing `ormspace-0.3.0/ormspace/annotations.py` & `ormspace-0.3.1/ormspace/annotations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from __future__ import annotations
 
 import datetime
-import re
 from decimal import Decimal
 from typing import Annotated, Optional
 
 from annotated_types import Ge, Le
 from pydantic import AfterValidator, BeforeValidator, Field, PlainSerializer
 
 from ormspace import functions
-from ormspace.functions import bytes_to_str, none_if_empty_string, string_to_list
 from ormspace.metainfo import MetaInfo
 
 
-BytesField = Annotated[bytes, PlainSerializer(bytes_to_str, return_type=str)]
-PasswordField = Annotated[bytes, PlainSerializer(bytes_to_str, return_type=str)]
+BytesField = Annotated[bytes, PlainSerializer(functions.bytes_to_str, return_type=str)]
+PasswordField = Annotated[bytes, PlainSerializer(functions.bytes_to_str, return_type=str)]
 TitleField = Annotated[str, AfterValidator(functions.title_caps)]
 LowerStringField = Annotated[str, AfterValidator(lambda x: x.lower() if x else '')]
 BirthDateField = Annotated[datetime.date, Ge((lambda : functions.today() - datetime.timedelta(days=365*125))()), Le(functions.today()), MetaInfo(form_field='date')]
 DateField = Annotated[datetime.date, Field(default_factory=functions.today)]
 DateTimeField = Annotated[datetime.datetime, Field(default_factory=functions.now)]
 MultiLineTextField = Annotated[str, MetaInfo(form_field='textarea', style={'height': '4rem'})]
 StringField = Annotated[str, MetaInfo(form_field='text')]
 PositiveIntegerField = Annotated[int, Ge(0), MetaInfo(form_field='number', config='min="0"')]
 PositiveDecimalField = Annotated[Decimal, Ge(0), MetaInfo(form_field='number', config='min="0"')]
 IntegerField = Annotated[int, BeforeValidator(functions.parse_number), MetaInfo(form_field='number', config='step="1"')]
 FloatField = Annotated[float, BeforeValidator(functions.parse_number), MetaInfo(form_field='number', config='step="0.01"')]
 DecimalField = Annotated[Decimal, BeforeValidator(functions.parse_number), MetaInfo(form_field='number', config='step="0.01"')]
 PositiveFloatField = Annotated[float, Ge(0), MetaInfo(form_field='number', config='step="0.01"')]
-ListOfStrings = Annotated[list[str], BeforeValidator(string_to_list), Field(default_factory=list)]
-OptionalFloat = Annotated[Optional[float], BeforeValidator(none_if_empty_string), Field(None)]
-OptionalInteger = Annotated[Optional[int], BeforeValidator(none_if_empty_string), Field(None)]
-OptionalDate = Annotated[Optional[datetime.date], BeforeValidator(none_if_empty_string), Field(None)]
-OptionalDecimal = Annotated[Optional[Decimal], BeforeValidator(none_if_empty_string), Field(None)]
+ListOfStrings = Annotated[list[str], BeforeValidator(functions.string_to_list), Field(default_factory=list)]
+OptionalFloat = Annotated[Optional[float], BeforeValidator(functions.none_if_empty_string), Field(None)]
+OptionalInteger = Annotated[Optional[int], BeforeValidator(functions.none_if_empty_string), Field(None)]
+OptionalDate = Annotated[Optional[datetime.date], BeforeValidator(functions.none_if_empty_string), Field(None)]
+OptionalDateTime = Annotated[Optional[datetime.datetime], BeforeValidator(functions.none_if_empty_string), Field(None)]
+OptionalDecimal = Annotated[Optional[Decimal], BeforeValidator(functions.none_if_empty_string), Field(None)]
```

### Comparing `ormspace-0.3.0/ormspace/bases.py` & `ormspace-0.3.1/ormspace/bases.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
     
     def __init__(self, value: str) -> None:
         self.value = value or ''
         for k, v in self.groupdict().items():
             setattr(self, f"_{k}", v)
         super().__init__(self.resolve)
 
-    
     @property
     def pattern(self) -> Pattern:
         if pattern:= self.GROUP_PATTERN or self.NON_GROUP_PATTERN:
             return pattern
         raise ValueError('No group or non-group pattern')
     
     @property
@@ -228,14 +227,15 @@
     ) -> core_schema.CoreSchema:
         return core_schema.no_info_after_validator_function(
             cls.validate,
             core_schema.str_schema(),
             serialization=core_schema.plain_serializer_function_ser_schema(lambda obj: str(obj),
                                                                            return_schema=core_schema.str_schema()),
         )
+    
     @classmethod
     def validate(cls, obj: str | None) -> Self | None:
         if obj and isinstance(obj, str):
             return cls(obj)
         elif isinstance(obj, cls):
             return obj
         return None
```

### Comparing `ormspace-0.3.0/ormspace/containers.py` & `ormspace-0.3.1/ormspace/containers.py`

 * *Files identical despite different names*

### Comparing `ormspace-0.3.0/ormspace/database.py` & `ormspace-0.3.1/ormspace/database.py`

 * *Files identical despite different names*

### Comparing `ormspace-0.3.0/ormspace/enum.py` & `ormspace-0.3.1/ormspace/enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import io
-from collections import namedtuple, UserString
-from enum import Enum
 from typing import Any, Type, TypeVar
 
 from pydantic import GetCoreSchemaHandler
 from pydantic_core import core_schema
 from typing_extensions import Self
 
 from ormspace import functions
```

### Comparing `ormspace-0.3.0/ormspace/functions.py` & `ormspace-0.3.1/ormspace/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     async with create_task_group() as tks:
         for c in coroutines:
             tks.start_soon(c)
 
 def bool_to_portuguese(v: bool) -> str:
     return 'sim' if v else 'não'
 
+def bool_to_english(v: bool) -> str:
+    return 'yes' if v else 'no'
+
 def meta_repr(self):
     fds = (i for i in fields(self) if getattr(self, i.name))
     return write_kwargs({i.name: getattr(self, i.name) for i in list(fds)})
 
 def compose(items: list[str]) -> str:
     if items:
         if len(items) == 1:
@@ -55,18 +58,29 @@
         elif len(items) == 2:
             return join(items, sep=' e ')
         else:
             data, reminescent = items[:-1], items[-1]
             return join(data, sep=', ') + ' e ' + reminescent
     return ''
 
+def concatenate(items: list[str]) -> str:
+    if items:
+        if len(items) == 1:
+            return items[0]
+        elif len(items) == 2:
+            return join(items, sep=' e ')
+        else:
+            data, reminescent = items[:-1], items[-1]
+            return join(data, sep=', ') + ' e ' + reminescent
+    return ''
+
 def years(end: datetime.date, start: datetime.date) -> float:
     days = (end - start).days
     subtract = calendar.leapdays(start.year, end.year)
-    return ((days - subtract)/365).__round__(1)
+    return ((days - subtract)/365).__round__(2)
 
 def date_from_age(age: float, bdate: datetime.date) -> datetime.date:
     around = bdate + datetime.timedelta(days=age * 365)
     return around + datetime.timedelta(days=calendar.leapdays(bdate.year, around.year))
 
 def find_numbers(string: str) -> list[str]:
     if mt:= re.findall(r'(\d+[.,]\d+|\d+)', string):
@@ -259,22 +273,14 @@
     
 def string_to_number(value: str) -> int | float:
     value = value.replace(',', '.').strip()
     if '.' in value:
         return float(value).__round__(2)
     return int(float(value))
 
-# def string_to_list(v: list[str] | str):
-#     if is_none_or_empty(v):
-#         return []
-#     elif isinstance(v, str):
-#         return filter_not_none(re.split(r'[\n;]', v))
-#     elif isinstance(v, list):
-#         return filter_not_none(v)
-#     return v
 
 def list_to_string(value, intersection: str = ', '):
     if isinstance(value, list):
         return intersection.join(value)
     return value
 
 def str_to_bytes(value):
@@ -311,14 +317,17 @@
 
 def is_list(value: Any) -> bool:
     return isinstance(value, list)
 
 def is_dict(value: Any) -> bool:
     return isinstance(value, dict)
 
+def is_tuple(value: Any) -> bool:
+    return isinstance(value, tuple)
+
 
 def bytes_to_str(value: bytes) -> str:
     return value.decode("utf-8")
 
 
 def string_to_list(value: str) -> list:
     if value:
```

### Comparing `ormspace-0.3.0/ormspace/keys.py` & `ormspace-0.3.1/ormspace/keys.py`

 * *Files identical despite different names*

### Comparing `ormspace-0.3.0/ormspace/metainfo.py` & `ormspace-0.3.1/ormspace/metainfo.py`

 * *Files identical despite different names*

### Comparing `ormspace-0.3.0/ormspace/model.py` & `ormspace-0.3.1/ormspace/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,30 @@
 class Model(bs.AbstractModel):
     EXTRA_DEPENDENTS: ClassVar[list[str]] = []
     EXIST_QUERY: ClassVar[Union[str, list[str]]] = None
     FETCH_QUERY: ClassVar[Union[dict, list[dict]]] = None
     SINGULAR: ClassVar[str] = None
     PLURAL: ClassVar[str] = None
     TABLE_NAME: ClassVar[str] = None
-    Database: ClassVar[Database] = None
     MODEL_GROUPS: ClassVar[list[str]] = None
+    Database: ClassVar[Database] = None
     Key: ClassVar[Annotated] = None
     KeyList: ClassVar[Annotated] = None
     
     
+    async def update_database_data(self, **updates: dict[str, Any]) -> Optional[Self]:
+        try:
+            await self.Database.update(updates=updates, key=self.key)
+            return await self.fetch_one(self.key)
+        except Exception as e:
+            return None
+            
+    
+    
+    
     @classmethod
     def context_data(cls) -> dict:
         return cls.Database.context_data
     
     @classmethod
     def instances_from_context(cls):
         return [cls(**i) for i in cls.context_data().values()]
@@ -318,32 +328,30 @@
 
 class ModelGroupMap(UserDict[str, ModelGroup]):
     def __init__(self, data: defaultdict):
         super().__init__({k: ModelGroup(k, ct.ListOfUniques(v)) for k, v in data.items()})
 
 
 
-
-
 class ModelMapConstructor(ChainMap[str, type[bs.ModelType]]):
         
     @property
-    def models(self) -> tuple[bs.ModelType]:
+    def models(self) -> tuple[type[bs.ModelType]]:
         return tuple([*self.values()])
     
     @property
-    def key_name_map(self):
+    def key_name_map(self) -> dict[str, type[bs.ModelType]]:
         return {f'{i.item_name()}_key': i for i in self.models}
     
     @property
-    def model_name_map(self):
+    def model_name_map(self) -> dict[str, type[bs.ModelType]]:
         return {i.classname(): i for i in self.models}
     
     @property
-    def table_name_map(self):
+    def table_name_map(self) -> dict[str, type[bs.ModelType]]:
         return {i.table(): i for i in self.models}
 
 
 ModelMap: ModelMapConstructor = ModelMapConstructor()
 
 
 @overload
@@ -364,30 +372,14 @@
     return ModelGroupMap(result)
 
 
 def models() -> list[type[bs.ModelType]]:
     return functions.filter_uniques(list(ModelMap.values()))
 
 
-# def modelmap(cls: type[bs.ModelType]):
-#     @wraps(cls)
-#     def wrapper():
-#         assert issubclass(cls, Model), 'A subclass of Model is required.'
-#         # assert cls.EXIST_QUERY, 'cadastrar "EXIST_QUERY" na classe "{}"'.format(cls.__name__)
-#         cls.Database = db.Database(cls)
-#         cls.Key = Annotated[kb.Key, mt.MetaInfo(tables=[cls.classname()], item_name=cls.item_name(), model=cls)]
-#         cls.KeyList = Annotated[kb.KeyList, mt.MetaInfo(model=cls, tables=[cls.classname()], item_name=f'{cls.item_name()}_list')]
-#         # cls.Key = Annotated[kb.Key, PlainSerializer(kb.Key.asjson, return_type=str), mt.MetaInfo(tables=[cls.classname()], item_name=cls.item_name(), model=cls)]
-#         # cls.KeyList = Annotated[kb.KeyList, PlainSerializer(kb.KeyList.asjson, return_type=list[str]), mt.MetaInfo(model=cls)]
-#         ModelMap[cls.item_name()]: cls = cls
-#         return cls
-#     return wrapper()
-
-
-
 def modelmap(cls: type[bs.ModelType], *, project_key: str = None):
     def decorator():
         @wraps(cls)
         def wrapper():
             assert issubclass(cls, Model), 'A subclass of Model is required.'
             # assert cls.EXIST_QUERY, 'cadastrar "EXIST_QUERY" na classe "{}"'.format(cls.__name__)
             cls.Database = db.Database(cls, project_key if project_key else Settings().data_key)
```

### Comparing `ormspace-0.3.0/ormspace/settings.py` & `ormspace-0.3.1/ormspace/settings.py`

 * *Files identical despite different names*

### Comparing `ormspace-0.3.0/pyproject.toml` & `ormspace-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ormspace"
-version = "0.3.0"
+version = "0.3.1"
 description = "Pydantic models working with deta.space api, including ORM features."
 authors = ["Daniel Arantes <arantesdv@me.com>"]
 license = "MIT"
 readme = 'README.md'
 exclude = ['.env', 'dev.py']
 
 [tool.poetry.dependencies]
```

### Comparing `ormspace-0.3.0/setup.py` & `ormspace-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'bcrypt>=4.0.1,<5.0.0',
  'deta[async]>=1.2.0,<2.0.0',
  'pydantic-settings>=2.0.3,<3.0.0',
  'pydantic>=2.4.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'ormspace',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Pydantic models working with deta.space api, including ORM features.',
     'long_description': "# ormspace \nORM modules powered by Pydantic for Deta Space.\n\n--- \n\n### Instructions\n\nThe package **ormspace**  will use the deta data key provides as _COLLECTION_KEY_ or will look for _DETA_PROJECT_KEY_ if the \nfirst is not provided. This way you can set a custom data key or use the project default. The sistem cannot work all is\nmissing. \n\n#### the 'modelmap' decorator \nTo include the class in the system mapping you must use the 'modelmap' decorator.  With this procedure you will get:\n- access to deta space api for read and write your data \n- create special fields for each class:\n  - Model.Key \n  - Model.KeyList\n  \n\n### Example\n    import datetime\n    import asyncio\n    from ormspace import model as md\n\n    @md.modelmap\n    class Person(md.Model):\n        first_name: str \n        last_name: str \n        birth_date: datetime.date\n\n    @md.modelmap\n    class Patient(md.Model):\n        person_key: Person.Key\n\n\n    async def main():\n        await Patient.update_references_context()\n        for item in await Patient.sorted_instances_list():\n            print(item)\n\n    asyncio.run(main())\n\n",
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `ormspace-0.3.0/PKG-INFO` & `ormspace-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormspace
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pydantic models working with deta.space api, including ORM features.
 License: MIT
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

