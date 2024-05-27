# Comparing `tmp/replete-2.1.0.tar.gz` & `tmp/replete-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replete-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "replete-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `replete-2.1.0.tar` & `replete-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      258 2024-03-03 23:28:26.230827 replete-2.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0       65 2024-03-03 23:28:26.230827 replete-2.1.0/.markdownlint.json
--rw-r--r--   0        0        0       61 2024-03-03 23:28:26.230827 replete-2.1.0/.taplo.toml
--rw-r--r--   0        0        0       39 2024-03-03 23:28:26.230827 replete-2.1.0/.yamllint.yaml
--rw-r--r--   0        0        0    34390 2024-03-03 23:28:26.230827 replete-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      824 2024-03-03 23:28:26.230827 replete-2.1.0/README.md
--rw-r--r--   0        0        0     2117 2024-03-03 23:28:26.230827 replete-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      551 2024-03-03 23:28:26.230827 replete-2.1.0/replete/__init__.py
--rw-r--r--   0        0        0      593 2024-03-03 23:28:26.230827 replete-2.1.0/replete/abc.py
--rw-r--r--   0        0        0     1324 2024-03-03 23:28:26.230827 replete-2.1.0/replete/aio.py
--rw-r--r--   0        0        0    17510 2024-03-03 23:28:26.230827 replete-2.1.0/replete/cli.py
--rw-r--r--   0        0        0     4017 2024-03-03 23:28:26.230827 replete-2.1.0/replete/consistent_hash.py
--rw-r--r--   0        0        0     5253 2024-03-03 23:28:26.230827 replete-2.1.0/replete/datetime.py
--rw-r--r--   0        0        0      492 2024-03-03 23:28:26.230827 replete-2.1.0/replete/enum.py
--rw-r--r--   0        0        0     4996 2024-03-03 23:28:26.230827 replete-2.1.0/replete/funcutils.py
--rw-r--r--   0        0        0     5946 2024-03-03 23:28:26.230827 replete-2.1.0/replete/logging.py
--rw-r--r--   0        0        0     3955 2024-03-03 23:28:26.230827 replete-2.1.0/replete/register.py
--rw-r--r--   0        0        0     1305 2024-03-03 23:28:26.230827 replete-2.1.0/replete/testing.py
--rw-r--r--   0        0        0     2512 2024-03-03 23:28:26.230827 replete-2.1.0/replete/timing.py
--rw-r--r--   0        0        0     6830 2024-03-03 23:28:26.230827 replete-2.1.0/replete/utils.py
--rw-r--r--   0        0        0       15 2024-03-03 23:28:26.230827 replete-2.1.0/requirements.txt
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 replete-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-05-27 15:27:23.915895 replete-2.2.0/.markdownlint.json
+-rw-r--r--   0        0        0      569 2024-05-27 15:27:23.915895 replete-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       61 2024-05-27 15:27:23.915895 replete-2.2.0/.taplo.toml
+-rw-r--r--   0        0        0       39 2024-05-27 15:27:23.915895 replete-2.2.0/.yamllint.yaml
+-rw-r--r--   0        0        0    35154 2024-05-27 15:27:23.915895 replete-2.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-27 15:27:23.915895 replete-2.2.0/LICENSE
+-rw-r--r--   0        0        0     1853 2024-05-27 15:27:23.915895 replete-2.2.0/README.md
+-rw-r--r--   0        0        0     2268 2024-05-27 15:27:23.915895 replete-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      551 2024-05-27 15:27:23.915895 replete-2.2.0/replete/__init__.py
+-rw-r--r--   0        0        0      593 2024-05-27 15:27:23.915895 replete-2.2.0/replete/abc.py
+-rw-r--r--   0        0        0     1324 2024-05-27 15:27:23.915895 replete-2.2.0/replete/aio.py
+-rw-r--r--   0        0        0    17510 2024-05-27 15:27:23.915895 replete-2.2.0/replete/cli.py
+-rw-r--r--   0        0        0     3963 2024-05-27 15:27:23.915895 replete-2.2.0/replete/consistent_hash.py
+-rw-r--r--   0        0        0     5253 2024-05-27 15:27:23.915895 replete-2.2.0/replete/datetime.py
+-rw-r--r--   0        0        0      492 2024-05-27 15:27:23.915895 replete-2.2.0/replete/enum.py
+-rw-r--r--   0        0        0     4996 2024-05-27 15:27:23.919895 replete-2.2.0/replete/funcutils.py
+-rw-r--r--   0        0        0     5946 2024-05-27 15:27:23.919895 replete-2.2.0/replete/logging.py
+-rw-r--r--   0        0        0     3955 2024-05-27 15:27:23.919895 replete-2.2.0/replete/register.py
+-rw-r--r--   0        0        0     1291 2024-05-27 15:27:23.919895 replete-2.2.0/replete/testing.py
+-rw-r--r--   0        0        0     2512 2024-05-27 15:27:23.919895 replete-2.2.0/replete/timing.py
+-rw-r--r--   0        0        0     7233 2024-05-27 15:27:23.919895 replete-2.2.0/replete/utils.py
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 replete-2.2.0/PKG-INFO
```

### Comparing `replete-2.1.0/CHANGELOG.md` & `replete-2.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # CHANGELOG
 
 
 
+## v2.2.0 (2024-05-27)
+
+### Chore
+
+* chore(test_and_version): add requests update to release ([`898b48a`](https://github.com/Rizhiy/replete/commit/898b48a4ef1f74bc6d608fa3e55a7d9bd65259cd))
+
+* chore: add LICENSE ([`c4ed272`](https://github.com/Rizhiy/replete/commit/c4ed272d814bf74a206ecc9ddb839e2402c463e2))
+
+* chore: disable S403, S404 globally ([`51ff3fa`](https://github.com/Rizhiy/replete/commit/51ff3fa1d31e66bf631b99b603db2e727f152319))
+
+### Documentation
+
+* docs: add pre-commit and add dev instructions in README ([`c2f32c5`](https://github.com/Rizhiy/replete/commit/c2f32c5b388f0668a213b26dbd452aee741d1991))
+
+### Feature
+
+* feat(utils): add convert_size ([`50572d3`](https://github.com/Rizhiy/replete/commit/50572d3bc9fb4d44b54975fd9de9a0ec09ac04a4))
+
+
 ## v2.1.0 (2024-03-03)
 
 ### Ci
 
 * ci: fix coverage ([`0e368ab`](https://github.com/Rizhiy/replete/commit/0e368ab9ebede394fe8b29ec4e94ad1745b3086c))
 
 ### Feature
```

### Comparing `replete-2.1.0/pyproject.toml` & `replete-2.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requires-python = ">=3.10"
 dynamic = ["description", "version"]
 dependencies = ["coloredlogs", "docstring-parser", "python-dateutil", "xxhash"]
 
 [project.optional-dependencies]
 testing = ["pytest<8", "pyyaml"]
 test = ["flaky", "pytest", "pytest-asyncio", "pytest-coverage", "replete[testing]", "types-python-dateutil", "types-xxhash"]
-dev = ["replete[test]", "ruff"]
+dev = ["black", "isort", "replete[test]", "ruff"]
 
 [project.entry-points.pytest11]
 replete = "replete.testing"
 
 [tool.flit.sdist]
 include = ["README.md"]
 exclude = [".github", ".gitignore", "tests/*"]
@@ -27,14 +27,22 @@
 version_variables = ["replete/__init__.py:__version__"]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--doctest-modules --no-success-flaky-report"
 asyncio_mode = "auto"
 
+[tool.black]
+line-length = 120
+# skip-magic-trailing-comma = true
+
+[tool.isort]
+profile = "black"
+line_length = 120
+
 [tool.yamlfix]
 line_length = 120
 section_whitelines = 1
 
 [tool.pyright]
 strictParameterNoneValue = false
 typeCheckingMode = "basic"
@@ -42,15 +50,15 @@
 [tool.ruff]
 target-version = "py310"
 line-length = 120
 [tool.ruff.lint]
 preview = true
 select = ["A", "ARG", "B", "BLE", "C4", "COM", "E", "ERA", "F", "FBT", "FIX", "FLY", "FURB", "I", "IC", "INP", "ISC", "LOG", "N", "NPY", "PERF", "PIE", "PT", "PTH", "Q", "R", "RET", "RSE", "S", "SIM", "SLF", "T20", "TCH", "TD", "TID", "TRY", "UP", "W"]
 fixable = ["ALL"]
-ignore = ["A003", "E203", "FIX002", "FURB113", "N817", "PTH123", "RET503", "S113", "TD002", "TD003", "TRY003", "UP007", "UP035"]
+ignore = ["A003", "E203", "FIX002", "FURB113", "N817", "PTH123", "RET503", "S113", "S403", "S404", "TD002", "TD003", "TRY003", "UP007", "UP035"]
 [tool.ruff.lint.per-file-ignores]
 "**/__init__.py" = [
     "F401", # Allow unused imports in module files
 ]
 "tests/test_cli.py" = [
     "W291", # Need to ignore it for correct formatting
 ]
```

### Comparing `replete-2.1.0/replete/__init__.py` & `replete-2.2.0/replete/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 from .datetime import date_range, datetime_range, round_dt
 from .enum import ComparableEnum
 from .logging import WarnWithTraceback, assert_with_logging, setup_logging
 from .register import Register
 from .timing import RateLimiter, Timer
 from .utils import chunks, deep_update, ensure_unique_keys, grouped, split_list
 
-__version__ = "2.1.0"
+__version__ = "2.2.0"
```

### Comparing `replete-2.1.0/replete/abc.py` & `replete-2.2.0/replete/abc.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/aio.py` & `replete-2.2.0/replete/aio.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/cli.py` & `replete-2.2.0/replete/cli.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/consistent_hash.py` & `replete-2.2.0/replete/consistent_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import collections.abc
 import contextlib
 import datetime
-import pickle  # noqa S403, not loading anything here, only dumping
+import pickle
 from typing import TYPE_CHECKING
 
 import xxhash
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Sequence
     from typing import Any
```

### Comparing `replete-2.1.0/replete/datetime.py` & `replete-2.2.0/replete/datetime.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/funcutils.py` & `replete-2.2.0/replete/funcutils.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/logging.py` & `replete-2.2.0/replete/logging.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/register.py` & `replete-2.2.0/replete/register.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/testing.py` & `replete-2.2.0/replete/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pickle  # noqa: S403
+import pickle
 import warnings
 from pathlib import Path
 
 try:
     import pytest
     import yaml
 except ModuleNotFoundError as exc:
```

### Comparing `replete-2.1.0/replete/timing.py` & `replete-2.2.0/replete/timing.py`

 * *Files identical despite different names*

### Comparing `replete-2.1.0/replete/utils.py` & `replete-2.2.0/replete/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import functools
 import itertools
 import logging
+import math
 import weakref
 from concurrent import futures
 from typing import TYPE_CHECKING, Any, Callable, Hashable, Iterable, Iterator, Mapping, Sequence, TypeVar
 
 LOGGER = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
@@ -170,14 +171,15 @@
                 while current_result_idx in cache_results:
                     yield cache_results.pop(current_result_idx)
                     current_result_idx += 1
             else:
                 yield func_result
 
 
+# TODO: This function doesn't seem to work with multiple instances of a class, need to debug
 def weak_lru_cache(maxsize: Callable | int | None = 128, *, typed=False):
     """
     LRU Cache decorator that keeps a weak reference to 'self'
     Should be used instead of functools.lru_cache on methods
     """
 
     def helper(maxsize: int, user_function: Callable, *, typed: bool) -> Callable:
@@ -195,7 +197,17 @@
         # The user_function was passed in directly via the maxsize argument
         user_function, maxsize = maxsize, 128
         return helper(maxsize, user_function, typed=typed)
     if not (type(maxsize) is int or maxsize is None):
         raise ValueError("Expected maxsize to be an integer or None")
 
     return functools.partial(helper, maxsize, typed=typed)
+
+
+def convert_size(size_bytes):
+    if size_bytes == 0:
+        return "0B"
+    size_name = ("B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB", "ZiB", "YiB")
+    i = int(math.floor(math.log(size_bytes, 1024)))
+    p = math.pow(1024, i)
+    s = round(size_bytes / p, 2)
+    return f"{s} {size_name[i]}"
```

### Comparing `replete-2.1.0/PKG-INFO` & `replete-2.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: replete
-Version: 2.1.0
+Version: 2.2.0
 Summary: Assorted utilities with minimal dependencies
 Author: Anton Vasilev, Artem Vasenin
 Maintainer-email: Artem Vasenin <vasart169@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: coloredlogs
 Requires-Dist: docstring-parser
 Requires-Dist: python-dateutil
 Requires-Dist: xxhash
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: isort ; extra == "dev"
 Requires-Dist: replete[test] ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: flaky ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ; extra == "test"
 Requires-Dist: pytest-coverage ; extra == "test"
 Requires-Dist: replete[testing] ; extra == "test"
@@ -34,7 +36,25 @@
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FRizhiy%2Freplete%2Fmaster%2Fpyproject.toml)
 [![PyPI - Version](https://img.shields.io/pypi/v/replete)](https://pypi.org/project/replete/)
 
 ## Installation
 
 Released version: `pip install replete`
 
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

