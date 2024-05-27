# Comparing `tmp/apexdevkit-1.1.2.tar.gz` & `tmp/apexdevkit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apexdevkit-1.1.2.tar", max compression
+gzip compressed data, was "apexdevkit-1.2.1.tar", max compression
```

## Comparing `apexdevkit-1.1.2.tar` & `apexdevkit-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    35149 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/LICENSE
--rw-r--r--   0        0        0       12 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/__init__.py
--rw-r--r--   0        0        0       81 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/annotation/__init__.py
--rw-r--r--   0        0        0     1475 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/annotation/deprecate.py
--rw-r--r--   0        0        0      903 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/error.py
--rw-r--r--   0        0        0      597 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/__init__.py
--rw-r--r--   0        0        0      970 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/builder.py
--rw-r--r--   0        0        0      255 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/dependable.py
--rw-r--r--   0        0        0      233 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/docs.py
--rw-r--r--   0        0        0     1699 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/response.py
--rw-r--r--   0        0        0     7751 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/router.py
--rw-r--r--   0        0        0     3603 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/schema.py
--rw-r--r--   0        0        0     2296 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/fastapi/service.py
--rw-r--r--   0        0        0      398 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/http/__init__.py
--rw-r--r--   0        0        0     2022 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/http/fake.py
--rw-r--r--   0        0        0     3060 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/http/fluent.py
--rw-r--r--   0        0        0     2763 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/http/httpx.py
--rw-r--r--   0        0        0     1026 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/http/json.py
--rw-r--r--   0        0        0      201 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/http/url.py
--rw-r--r--   0        0        0        0 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/py.typed
--rw-r--r--   0        0        0      334 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/repository/__init__.py
--rw-r--r--   0        0        0      772 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/repository/connector.py
--rw-r--r--   0        0        0     2362 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/repository/database.py
--rw-r--r--   0        0        0     2973 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/repository/in_memory.py
--rw-r--r--   0        0        0      238 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/testing/__init__.py
--rw-r--r--   0        0        0     1305 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/testing/database.py
--rw-r--r--   0        0        0     7774 2024-05-27 14:31:07.719022 apexdevkit-1.1.2/apexdevkit/testing/rest.py
--rw-r--r--   0        0        0      992 2024-05-27 14:31:20.691028 apexdevkit-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 apexdevkit-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/LICENSE
+-rw-r--r--   0        0        0       12 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/annotation/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/annotation/deprecate.py
+-rw-r--r--   0        0        0      903 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/error.py
+-rw-r--r--   0        0        0      597 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/__init__.py
+-rw-r--r--   0        0        0      970 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/builder.py
+-rw-r--r--   0        0        0      255 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/dependable.py
+-rw-r--r--   0        0        0      233 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/docs.py
+-rw-r--r--   0        0        0     1699 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/response.py
+-rw-r--r--   0        0        0     7745 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/router.py
+-rw-r--r--   0        0        0     3603 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/schema.py
+-rw-r--r--   0        0        0     2616 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/service.py
+-rw-r--r--   0        0        0      398 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/http/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/fake.py
+-rw-r--r--   0        0        0     3060 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/fluent.py
+-rw-r--r--   0        0        0     2763 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/httpx.py
+-rw-r--r--   0        0        0     1026 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/json.py
+-rw-r--r--   0        0        0      201 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/url.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/py.typed
+-rw-r--r--   0        0        0      334 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/connector.py
+-rw-r--r--   0        0        0     2362 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/database.py
+-rw-r--r--   0        0        0     3388 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/in_memory.py
+-rw-r--r--   0        0        0      653 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/interface.py
+-rw-r--r--   0        0        0      238 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/testing/__init__.py
+-rw-r--r--   0        0        0     1305 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/testing/database.py
+-rw-r--r--   0        0        0     7774 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/testing/rest.py
+-rw-r--r--   0        0        0      992 2024-05-27 15:39:16.746025 apexdevkit-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 apexdevkit-1.2.1/PKG-INFO
```

### Comparing `apexdevkit-1.1.2/LICENSE` & `apexdevkit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/annotation/deprecate.py` & `apexdevkit-1.2.1/apexdevkit/annotation/deprecate.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/error.py` & `apexdevkit-1.2.1/apexdevkit/error.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/fastapi/__init__.py` & `apexdevkit-1.2.1/apexdevkit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/fastapi/builder.py` & `apexdevkit-1.2.1/apexdevkit/fastapi/builder.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/fastapi/response.py` & `apexdevkit-1.2.1/apexdevkit/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/fastapi/router.py` & `apexdevkit-1.2.1/apexdevkit/fastapi/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Annotated, Any, Iterable, Self, TypeVar
 
 from fastapi import APIRouter, Depends
 from fastapi.responses import JSONResponse
 
 from apexdevkit.error import DoesNotExistError, ExistsError
 from apexdevkit.fastapi.schema import RestfulSchema
-from apexdevkit.fastapi.service import RestfulService, _RawCollection, _RawItem
+from apexdevkit.fastapi.service import RawCollection, RawItem, RestfulService
 from apexdevkit.testing import RestfulName
 
 _Response = JSONResponse | dict[str, Any]
 
 
 @dataclass
 class RestfulResponse:
@@ -111,15 +111,15 @@
         @self.router.post(
             "",
             status_code=201,
             responses={409: {}},
             response_model=self.schema.for_item(),
             include_in_schema=is_documented,
         )
-        def create_one(item: Annotated[_RawItem, Depends(schema)]) -> _Response:
+        def create_one(item: Annotated[RawItem, Depends(schema)]) -> _Response:
             try:
                 item = self.service.create_one(item)
             except ExistsError as e:
                 return JSONResponse(self.response.exists(e), 409)
 
             return self.response.created_one(item)
 
@@ -131,15 +131,15 @@
         @self.router.post(
             "/batch",
             status_code=201,
             responses={409: {}},
             response_model=self.schema.for_collection(),
             include_in_schema=is_documented,
         )
-        def create_many(items: Annotated[_RawCollection, Depends(schema)]) -> _Response:
+        def create_many(items: Annotated[RawCollection, Depends(schema)]) -> _Response:
             try:
                 return self.response.created_many(self.service.create_many(items))
             except ExistsError as e:
                 return JSONResponse(self.response.exists(e), 409)
 
         return self
 
@@ -184,15 +184,15 @@
             status_code=200,
             responses={404: {}},
             response_model=self.schema.for_no_data(),
             include_in_schema=is_documented,
         )
         def update_one(
             item_id: str,
-            updates: Annotated[_RawItem, Depends(schema)],
+            updates: Annotated[RawItem, Depends(schema)],
         ) -> _Response:
             try:
                 self.service.update_one(item_id, **updates)
             except DoesNotExistError as e:
                 return JSONResponse(self.response.not_found(e), 404)
 
             return self.response.ok()
@@ -205,15 +205,15 @@
         @self.router.patch(
             "",
             status_code=200,
             responses={},
             response_model=self.schema.for_no_data(),
             include_in_schema=is_documented,
         )
-        def update_many(items: Annotated[_RawCollection, Depends(schema)]) -> _Response:
+        def update_many(items: Annotated[RawCollection, Depends(schema)]) -> _Response:
             self.service.update_many(items)
 
             return self.response.ok()
 
         return self
 
     def with_delete_one_endpoint(self, is_documented: bool = True) -> Self:
```

### Comparing `apexdevkit-1.1.2/apexdevkit/fastapi/schema.py` & `apexdevkit-1.2.1/apexdevkit/fastapi/schema.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/fastapi/service.py` & `apexdevkit-1.2.1/apexdevkit/fastapi/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,85 @@
+from abc import ABC
 from dataclasses import asdict, dataclass, replace
-from typing import Any, Iterable, Protocol
+from typing import Any, Iterable
 
-from apexdevkit.repository import InMemoryRepository
+from apexdevkit.repository.interface import Repository
 
-_RawItem = dict[str, Any]
-_RawCollection = Iterable[_RawItem]
+RawItem = dict[str, Any]
+RawCollection = Iterable[RawItem]
 
 
-class RestfulService(Protocol):
-    def create_one(self, item: _RawItem) -> _RawItem:
-        pass
+class RestfulService(ABC):
+    def create_one(self, item: RawItem) -> RawItem:
+        raise NotImplementedError(self.create_one.__name__)
 
-    def create_many(self, items: _RawCollection) -> _RawCollection:
-        pass
+    def create_many(self, items: RawCollection) -> RawCollection:
+        raise NotImplementedError(self.create_many.__name__)
 
-    def read_one(self, item_id: str) -> _RawItem:
-        pass
+    def read_one(self, item_id: str) -> RawItem:
+        raise NotImplementedError(self.read_one.__name__)
 
-    def read_all(self) -> _RawCollection:
-        pass
+    def read_all(self) -> RawCollection:
+        raise NotImplementedError(self.read_all.__name__)
 
-    def update_one(self, item_id: str, **with_fields: Any) -> _RawItem:
-        pass
+    def update_one(self, item_id: str, **with_fields: Any) -> RawItem:
+        raise NotImplementedError(self.update_one.__name__)
 
-    def update_many(self, items: _RawCollection) -> _RawCollection:
-        pass
+    def update_many(self, items: RawCollection) -> RawCollection:
+        raise NotImplementedError(self.update_many.__name__)
 
     def delete_one(self, item_id: str) -> None:
-        pass
+        raise NotImplementedError(self.delete_one.__name__)
 
 
-def _as_raw_collection(value: Iterable[Any]) -> _RawCollection:
+def _as_raw_collection(value: Iterable[Any]) -> RawCollection:
     return [_as_raw_item(item) for item in value]
 
 
-def _as_raw_item(value: Any) -> _RawItem:
+def _as_raw_item(value: Any) -> RawItem:
     return asdict(value)
 
 
 @dataclass
-class InMemoryRestfulService:
+class RestfulRepository(RestfulService):
     resource: type[Any]
-    repository: InMemoryRepository[Any]
+    repository: Repository[Any, Any]
 
-    def create_one(self, item: _RawItem) -> _RawItem:
+    def create_one(self, item: RawItem) -> RawItem:
         result = self.resource(**item)
 
         self.repository.create(result)
 
         return _as_raw_item(result)
 
-    def create_many(self, items: _RawCollection) -> _RawCollection:
+    def create_many(self, items: RawCollection) -> RawCollection:
         result = [self.resource(**fields) for fields in items]
 
         self.repository.create_many(result)
 
         return _as_raw_collection(result)
 
-    def read_one(self, item_id: str) -> _RawItem:
+    def read_one(self, item_id: str) -> RawItem:
         result = self.repository.read(item_id)
 
         return _as_raw_item(result)
 
-    def read_all(self) -> _RawCollection:
+    def read_all(self) -> RawCollection:
         result = self.repository
 
         return _as_raw_collection(result)
 
-    def update_one(self, item_id: str, **with_fields: Any) -> _RawItem:
+    def update_one(self, item_id: str, **with_fields: Any) -> RawItem:
         result = replace(self.repository.read(item_id), **with_fields)
 
         self.repository.update(result)
 
         return _as_raw_item(result)
 
-    def update_many(self, items: _RawCollection) -> _RawCollection:
+    def update_many(self, items: RawCollection) -> RawCollection:
         result = [self.resource(**fields) for fields in items]
 
         self.repository.update_many(result)
 
         return _as_raw_collection(result)
 
     def delete_one(self, item_id: str) -> None:
```

### Comparing `apexdevkit-1.1.2/apexdevkit/http/fake.py` & `apexdevkit-1.2.1/apexdevkit/http/fake.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/http/fluent.py` & `apexdevkit-1.2.1/apexdevkit/http/fluent.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/http/httpx.py` & `apexdevkit-1.2.1/apexdevkit/http/httpx.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/http/json.py` & `apexdevkit-1.2.1/apexdevkit/http/json.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/repository/connector.py` & `apexdevkit-1.2.1/apexdevkit/repository/connector.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/repository/database.py` & `apexdevkit-1.2.1/apexdevkit/repository/database.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/repository/in_memory.py` & `apexdevkit-1.2.1/apexdevkit/repository/in_memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from dataclasses import dataclass, field
+from dataclasses import asdict, dataclass, field
 from typing import Any, Generic, Iterable, Iterator, Protocol, Self, TypeVar
 
 from apexdevkit.error import Criteria, DoesNotExistError, ExistsError
 
 
 class _Item(Protocol):
     @property
@@ -19,21 +19,36 @@
         pass
 
     def dump(self, item: ItemT) -> dict[str, Any]:
         pass
 
 
 @dataclass
+class DataclassFormatter(Generic[ItemT]):
+    resource: type[ItemT]
+
+    def load(self, raw: dict[str, Any]) -> ItemT:
+        return self.resource(**raw)
+
+    def dump(self, item: ItemT) -> dict[str, Any]:
+        return asdict(item)  # type: ignore
+
+
+@dataclass
 class InMemoryRepository(Generic[ItemT]):
     formatter: _Formatter[ItemT]
     items: dict[str, dict[str, Any]] = field(default_factory=dict)
 
     _uniques: list[Criteria] = field(init=False, default_factory=list)
     _search_by: list[str] = field(init=False, default_factory=list)
 
+    @classmethod
+    def for_dataclass(cls, value: type[ItemT]) -> "InMemoryRepository[ItemT]":
+        return cls(DataclassFormatter(value))
+
     def __post_init__(self) -> None:
         self._search_by = ["id", *self._search_by]
 
     def with_searchable(self, attribute: str) -> Self:
         self._search_by.append(attribute)
 
         return self
```

### Comparing `apexdevkit-1.1.2/apexdevkit/testing/database.py` & `apexdevkit-1.2.1/apexdevkit/testing/database.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/apexdevkit/testing/rest.py` & `apexdevkit-1.2.1/apexdevkit/testing/rest.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.1.2/pyproject.toml` & `apexdevkit-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apexdevkit"
-version = "1.1.2"
+version = "1.2.1"
 description = "Apex Development Tools for python."
 authors = ["Apex Dev <dev@apex.ge>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "*"
```

