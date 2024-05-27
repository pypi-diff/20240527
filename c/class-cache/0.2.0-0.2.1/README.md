# Comparing `tmp/class_cache-0.2.0.tar.gz` & `tmp/class_cache-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_cache-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "class_cache-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `class_cache-0.2.0.tar` & `class_cache-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       77 2024-05-26 22:57:07.152781 class_cache-0.2.0/.markdownlint.json
--rw-r--r--   0        0        0       61 2024-05-26 22:57:07.152781 class_cache-0.2.0/.taplo.toml
--rw-r--r--   0        0        0     1666 2024-05-26 22:57:07.152781 class_cache-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2024-05-26 22:57:07.152781 class_cache-0.2.0/LICENSE
--rw-r--r--   0        0        0     2248 2024-05-26 22:57:07.152781 class_cache-0.2.0/README.md
--rw-r--r--   0        0        0      141 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/__init__.py
--rw-r--r--   0        0        0     3995 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/backends.py
--rw-r--r--   0        0        0     3277 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/core.py
--rw-r--r--   0        0        0      229 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/types.py
--rw-r--r--   0        0        0      225 2024-05-26 22:57:07.152781 class_cache-0.2.0/class_cache/utils.py
--rw-r--r--   0        0        0     2073 2024-05-26 22:57:07.152781 class_cache-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 class_cache-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-05-27 14:14:06.306109 class_cache-0.2.1/.markdownlint.json
+-rw-r--r--   0        0        0      569 2024-05-27 14:14:06.306109 class_cache-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       61 2024-05-27 14:14:06.306109 class_cache-0.2.1/.taplo.toml
+-rw-r--r--   0        0        0     2144 2024-05-27 14:14:06.310109 class_cache-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-27 14:14:06.310109 class_cache-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3277 2024-05-27 14:14:06.310109 class_cache-0.2.1/README.md
+-rw-r--r--   0        0        0      141 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/__init__.py
+-rw-r--r--   0        0        0     3941 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/backends.py
+-rw-r--r--   0        0        0     3424 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/core.py
+-rw-r--r--   0        0        0      229 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/types.py
+-rw-r--r--   0        0        0      225 2024-05-27 14:14:06.310109 class_cache-0.2.1/class_cache/utils.py
+-rw-r--r--   0        0        0     2087 2024-05-27 14:14:06.310109 class_cache-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3968 1970-01-01 00:00:00.000000 class_cache-0.2.1/PKG-INFO
```

### Comparing `class_cache-0.2.0/CHANGELOG.md` & `class_cache-0.2.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v0.2.1 (2024-05-27)
+
+### Chore
+
+* chore: add pre-commit ([`f7050eb`](https://github.com/Rizhiy/class-cache/commit/f7050eb57345a667a681e6d93233c0c49c389f3b))
+
+### Documentation
+
+* docs(README): add dev instructions ([`878a6a7`](https://github.com/Rizhiy/class-cache/commit/878a6a7441a4cfa4545b3f9fdb659798e0f6392f))
+
+### Fix
+
+* fix(core.py): fix clear() and add more tests ([`7389321`](https://github.com/Rizhiy/class-cache/commit/73893218a52d341b25fda98eea7d97638b70e0f9))
+
+
 ## v0.2.0 (2024-05-26)
 
 ### Documentation
 
 * docs(README): add install instructions and basic usage example ([`6572cd5`](https://github.com/Rizhiy/class-cache/commit/6572cd5476e718b4a6c04937006560a7a374b185))
 
 ### Feature
```

### Comparing `class_cache-0.2.0/LICENSE` & `class_cache-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `class_cache-0.2.0/README.md` & `class_cache-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -65,7 +65,25 @@
       # Define logic for defaults in _get_data
       def _get_data(self, key: str) -> str:
           return f"{self._name}_{key}"
 
   cache = MyCache("first")
   assert cache["foo"] == "first_foo"
   ```
+
+## Development
+
+- Install dev dependencies: `pip install -e ".[dev]"`
+- For linting and basic fixes [ruff](https://docs.astral.sh/ruff/) is used: `ruff check . --fix`
+- This repository follows strict formatting style which will be checked by the CI.
+  - To format the code, use the [black](https://black.readthedocs.io) format: `black .`
+  - To sort the imports, user [isort](https://pycqa.github.io/isort/) utility: `isort .`
+- To test code, use [pytest](https://pytest.org): `pytest .`
+- This repository follows semantic-release, which means all commit messages have to follow a [style](https://python-semantic-release.readthedocs.io/en/latest/commit-parsing.html).
+  You can use tools like [commitizen](https://github.com/commitizen-tools/commitizen) to write your commits.
+- You can also use [pre-commit](https://pre-commit.com/) to help verify that all changes are valid.
+  Multiple hooks are used, so use the following commands to install:
+
+  ```bash
+  pre-commit install
+  pre-commit install --hook-type commit-msg
+  ```
```

### Comparing `class_cache-0.2.0/class_cache/backends.py` & `class_cache-0.2.1/class_cache/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,17 +45,14 @@
 
     def __init__(self, id_: str | int, target_block_size=1024**2) -> None:
         super().__init__(id_)
         self._dir = self.ROOT_DIR / str(self._id)
         self._dir.mkdir(exist_ok=True, parents=True)
         self._target_block_size = target_block_size
 
-    def __hash__(self):
-        return hash(self.id)
-
     def _get_key_hash(self, key: KeyType) -> str:
         return f"{consistent_hash(key):x}"
 
     def _get_all_block_ids(self) -> Iterable[str]:
         yield from (path.name.split(".")[0] for path in self._dir.glob(f"*{self.BLOCK_SUFFIX}"))
 
     def _get_path_for_block_id(self, block_id: str) -> Path:
```

### Comparing `class_cache-0.2.0/class_cache/core.py` & `class_cache-0.2.1/class_cache/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,16 +42,22 @@
             raise KeyError(key)
         self._data.pop(key, None)
         self._to_delete.add(key)
 
     def write(self) -> None:
         """Write values to backend"""
         self._backend.set_many((key, self._data[key]) for key in self._to_write)
-        self._to_write = set()
         self._backend.del_many(self._to_delete)
+        self._to_write = set()
+        self._to_delete = set()
+
+    def clear(self) -> None:
+        self._backend.clear()
+        self._data = {}
+        self._to_write = set()
         self._to_delete = set()
 
 
 class CacheWithDefault(Cache[KeyType, ValueType]):
     VERSION = 0
     NON_HASH_ATTRIBUTES: ClassVar[frozenset[str]] = frozenset(
         {"_backend", "_backend_set", "_data", "_to_write", "_to_delete"},
```

### Comparing `class_cache-0.2.0/pyproject.toml` & `class_cache-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 dependencies = ["Pympler", "marisa-trie", "replete"]
 
 [project.urls]
 Home = "https://github.com/Rizhiy/class-cache"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "replete[testing]"]
-dev = ["black", "class-cache[test]", "ruff"]
+dev = ["black", "class-cache[test]", "pre-commit", "ruff"]
 
 [tool.flit.sdist]
 include = ["README.md"]
 exclude = [".github", ".gitignore", "tests/*"]
 
 [tool.semantic_release]
 version_variables = ["class_cache/__init__.py:__version__"]
```

### Comparing `class_cache-0.2.0/PKG-INFO` & `class_cache-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: class-cache
-Version: 0.2.0
+Version: 0.2.1
 Summary: Caching for class based generators
 Maintainer-email: Artem Vasenin <vasart169@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: Pympler
 Requires-Dist: marisa-trie
 Requires-Dist: replete
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: class-cache[test] ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: replete[testing] ; extra == "test"
 Project-URL: Home, https://github.com/Rizhiy/class-cache
 Provides-Extra: dev
 Provides-Extra: test
@@ -86,7 +87,25 @@
       def _get_data(self, key: str) -> str:
           return f"{self._name}_{key}"
 
   cache = MyCache("first")
   assert cache["foo"] == "first_foo"
   ```
 
+## Development
+
+- Install dev dependencies: `pip install -e ".[dev]"`
+- For linting and basic fixes [ruff](https://docs.astral.sh/ruff/) is used: `ruff check . --fix`
+- This repository follows strict formatting style which will be checked by the CI.
+  - To format the code, use the [black](https://black.readthedocs.io) format: `black .`
+  - To sort the imports, user [isort](https://pycqa.github.io/isort/) utility: `isort .`
+- To test code, use [pytest](https://pytest.org): `pytest .`
+- This repository follows semantic-release, which means all commit messages have to follow a [style](https://python-semantic-release.readthedocs.io/en/latest/commit-parsing.html).
+  You can use tools like [commitizen](https://github.com/commitizen-tools/commitizen) to write your commits.
+- You can also use [pre-commit](https://pre-commit.com/) to help verify that all changes are valid.
+  Multiple hooks are used, so use the following commands to install:
+
+  ```bash
+  pre-commit install
+  pre-commit install --hook-type commit-msg
+  ```
+
```

