# Comparing `tmp/class_cache-0.1.0.tar.gz` & `tmp/class_cache-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_cache-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "class_cache-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `class_cache-0.1.0.tar` & `class_cache-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      993 2024-05-26 18:56:24.079492 class_cache-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2024-05-26 18:56:24.079492 class_cache-0.1.0/LICENSE
--rw-r--r--   0        0        0       12 2024-05-26 18:56:24.083492 class_cache-0.1.0/README.md
--rw-r--r--   0        0        0      123 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/__init__.py
--rw-r--r--   0        0        0     3981 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/backends.py
--rw-r--r--   0        0        0     2523 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/core.py
--rw-r--r--   0        0        0      229 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/types.py
--rw-r--r--   0        0        0      225 2024-05-26 18:56:24.083492 class_cache-0.1.0/class_cache/utils.py
--rw-r--r--   0        0        0     2278 2024-05-26 18:56:24.083492 class_cache-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 class_cache-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-05-26 22:57:07.152781 class_cache-0.2.0/.markdownlint.json
+-rw-r--r--   0        0        0       61 2024-05-26 22:57:07.152781 class_cache-0.2.0/.taplo.toml
+-rw-r--r--   0        0        0     1666 2024-05-26 22:57:07.152781 class_cache-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-26 22:57:07.152781 class_cache-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2248 2024-05-26 22:57:07.152781 class_cache-0.2.0/README.md
+-rw-r--r--   0        0        0      141 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/__init__.py
+-rw-r--r--   0        0        0     3995 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/backends.py
+-rw-r--r--   0        0        0     3277 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/core.py
+-rw-r--r--   0        0        0      229 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/types.py
+-rw-r--r--   0        0        0      225 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/utils.py
+-rw-r--r--   0        0        0     2073 2024-05-26 22:57:07.152781 class_cache-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 class_cache-0.2.0/PKG-INFO
```

### Comparing `class_cache-0.1.0/CHANGELOG.md` & `class_cache-0.2.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # CHANGELOG
 
 
 
+## v0.2.0 (2024-05-26)
+
+### Documentation
+
+* docs(README): add install instructions and basic usage example ([`6572cd5`](https://github.com/Rizhiy/class-cache/commit/6572cd5476e718b4a6c04937006560a7a374b185))
+
+### Feature
+
+* feat(core): implement CacheWithDefault properly ([`b5523d1`](https://github.com/Rizhiy/class-cache/commit/b5523d1bae9e7cbed62276caad1d4bb7e62e4f0c))
+
+### Test
+
+* test(github): fix requests version ([`5052e95`](https://github.com/Rizhiy/class-cache/commit/5052e957d3dab986553f0a3eccad6e6128c647b2))
+
+* test(github): fix coverage module selection ([`8dee97d`](https://github.com/Rizhiy/class-cache/commit/8dee97d67cc66e902e0b9ca285f30649928d3605))
+
+
 ## v0.1.0 (2024-05-26)
 
 ### Chore
 
 * chore: add placeholder ([`aa69282`](https://github.com/Rizhiy/class-cache/commit/aa6928222a6152ecc0e89aba0837b86d13d51076))
 
 ### Feature
```

### Comparing `class_cache-0.1.0/LICENSE` & `class_cache-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `class_cache-0.1.0/class_cache/backends.py` & `class_cache-0.2.0/class_cache/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from replete.consistent_hash import consistent_hash
 
 from class_cache.types import KeyType, ValueType
 from class_cache.utils import get_user_cache_dir
 
 
 class BaseBackend(ABC, MutableMapping[KeyType, ValueType]):
-    def __init__(self, id_: str | int) -> None:
+    def __init__(self, id_: str | int = None) -> None:
         self._id = id_
 
     @property
-    def id(self) -> str | int:
+    def id(self) -> str | int | None:
         return self._id
 
     # Override these methods to allow getting results in a more optimal fashion
     def contains_many(self, keys: Iterable[KeyType]) -> Iterator[tuple[KeyType, bool]]:
         for key in keys:
             yield key, key in self
```

### Comparing `class_cache-0.1.0/class_cache/core.py` & `class_cache-0.2.0/class_cache/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,28 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from typing import Any, ClassVar, Iterable, MutableMapping
 
 from replete.consistent_hash import consistent_hash
 
 from class_cache.backends import BaseBackend, PickleBackend
 from class_cache.types import KeyType, ValueType
 
+DEFAULT_BACKEND_TYPE = PickleBackend
 
-class Cache(ABC, MutableMapping[KeyType, ValueType]):
-    VERSION = 0
-    NON_HASH_ATTRIBUTES: ClassVar[frozenset[str]] = frozenset(
-        {"_backend", "_backend_set", "_data", "_to_write", "_to_delete"},
-    )
 
-    def __init__(self, backend: type[BaseBackend] = PickleBackend) -> None:
-        self._backend = backend(self.id_for_backend)
-        self._backend_set = True
+class Cache(ABC, MutableMapping[KeyType, ValueType]):
+    def __init__(self, id_: str | int = None, backend: type[BaseBackend] = DEFAULT_BACKEND_TYPE) -> None:
+        self._backend = backend(id_)
         self._data: dict[KeyType, ValueType] = {}
         self._to_write = set()
         self._to_delete = set()
 
-    @property
-    def id_for_backend(self) -> int:
-        return consistent_hash(self._data_for_hash())
-
-    def _data_for_hash(self) -> dict[str, Any]:
-        attrs = dict(vars(self))
-        for attr in self.NON_HASH_ATTRIBUTES:
-            attrs.pop(attr, None)
-        return attrs
-
-    def __setattr__(self, key: str, value: Any) -> None:
-        if (
-            not isinstance(getattr(self.__class__, key, None), property)
-            and getattr(self, "_backend_set", None)
-            and key not in self.NON_HASH_ATTRIBUTES
-        ):
-            raise TypeError(f"Trying to update hash inclusive attribute after hash has been decided: {key}")
-        object.__setattr__(self, key, value)
-
     def __contains__(self, key: KeyType) -> bool:
+        if key in self._data:
+            return True
         return key not in self._to_delete and key in self._backend
 
     def __setitem__(self, key: KeyType, value: ValueType) -> None:
         self._data[key] = value
         self._to_write.add(key)
 
     def __getitem__(self, key: KeyType) -> ValueType:
@@ -66,7 +45,50 @@
 
     def write(self) -> None:
         """Write values to backend"""
         self._backend.set_many((key, self._data[key]) for key in self._to_write)
         self._to_write = set()
         self._backend.del_many(self._to_delete)
         self._to_delete = set()
+
+
+class CacheWithDefault(Cache[KeyType, ValueType]):
+    VERSION = 0
+    NON_HASH_ATTRIBUTES: ClassVar[frozenset[str]] = frozenset(
+        {"_backend", "_backend_set", "_data", "_to_write", "_to_delete"},
+    )
+
+    def __init__(self, backend: type[BaseBackend] = DEFAULT_BACKEND_TYPE):
+        super().__init__(self.id_for_backend, backend)
+        self._backend_set = True
+
+    @property
+    def id_for_backend(self) -> int:
+        return consistent_hash(self._data_for_hash())
+
+    @abstractmethod
+    def _get_data(self, key: KeyType) -> ValueType:
+        """
+        Get default data for missing key.
+        This method should always produce the same value for the same instance with same hashable attributes,
+        see NON_HASH_ATTRIBUTES.
+        """
+
+    def __getitem__(self, key: KeyType) -> ValueType:
+        if key not in self:
+            self[key] = self._get_data(key)
+        return super().__getitem__(key)
+
+    def _data_for_hash(self) -> dict[str, Any]:
+        attrs = dict(vars(self))
+        for attr in self.NON_HASH_ATTRIBUTES:
+            attrs.pop(attr, None)
+        return attrs
+
+    def __setattr__(self, key: str, value: Any) -> None:
+        if (
+            not isinstance(getattr(self.__class__, key, None), property)
+            and getattr(self, "_backend_set", None)
+            and key not in self.NON_HASH_ATTRIBUTES
+        ):
+            raise TypeError(f"Trying to update hash inclusive attribute after hash has been decided: {key}")
+        object.__setattr__(self, key, value)
```

### Comparing `class_cache-0.1.0/pyproject.toml` & `class_cache-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "class-cache"
 maintainers = [{ name = "Artem Vasenin", email = "vasart169@gmail.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dynamic = ["description", "version"]
-dependencies = ["Pympler", "replete", "marisa-trie"]
+dependencies = ["Pympler", "marisa-trie", "replete"]
 
 [project.urls]
 Home = "https://github.com/Rizhiy/class-cache"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "replete[testing]"]
 dev = ["black", "class-cache[test]", "ruff"]
@@ -42,72 +42,19 @@
 typeCheckingMode = "basic"
 
 [tool.ruff]
 target-version = "py39"
 line-length = 120
 [tool.ruff.lint]
 preview = true
-select = [
-    "A",
-    "ARG",
-    "B",
-    "BLE",
-    "C4",
-    "COM",
-    "E",
-    "ERA",
-    "F",
-    "FBT",
-    "FIX",
-    "FLY",
-    "FURB",
-    "I",
-    "IC",
-    "INP",
-    "ISC",
-    "LOG",
-    "N",
-    "NPY",
-    "PERF",
-    "PIE",
-    "PT",
-    "PTH",
-    "Q",
-    "R",
-    "RET",
-    "RSE",
-    "S",
-    "SIM",
-    "SLF",
-    "T20",
-    "TCH",
-    "TD",
-    "TID",
-    "TRY",
-    "UP",
-    "W",
-]
+select = ["A", "ARG", "B", "BLE", "C4", "COM", "E", "ERA", "F", "FBT", "FIX", "FLY", "FURB", "I", "IC", "INP", "ISC", "LOG", "N", "NPY", "PERF", "PIE", "PT", "PTH", "Q", "R", "RET", "RSE", "S", "SIM", "SLF", "T20", "TCH", "TD", "TID", "TRY", "UP", "W"]
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
-ignore = [
-    "A003",
-    "E203",
-    "FIX002",
-    "FURB113",
-    "N817",
-    "PTH123",
-    "RET503",
-    "S113",
-    "TD002",
-    "TD003",
-    "TRY003",
-    "UP007",
-    "UP035",
-]
-[tool.ruff.per-file-ignores]
+ignore = ["A003", "E203", "FIX002", "FURB113", "N817", "PTH123", "RET503", "S113", "TD002", "TD003", "TRY003", "UP007", "UP035"]
+[tool.ruff.lint.per-file-ignores]
 "**/__init__.py" = [
     "F401", # Allow unused imports in module files
 ]
 "tests/**/*.py" = [
     "E501",   # Test strings can be long
     "S101",   # Asserts in tests are fine
     "T201",   # Prints are useful for debugging
```

