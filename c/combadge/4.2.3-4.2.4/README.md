# Comparing `tmp/combadge-4.2.3.tar.gz` & `tmp/combadge-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combadge-4.2.3.tar", max compression
+gzip compressed data, was "combadge-4.2.4.tar", max compression
```

## Comparing `combadge-4.2.3.tar` & `combadge-4.2.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11350 2024-04-08 14:44:23.788561 combadge-4.2.3/LICENSE
--rw-r--r--   0        0        0     2135 2024-04-08 14:44:23.788561 combadge-4.2.3/README.md
--rw-r--r--   0        0        0        0 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/_helpers/__init__.py
--rw-r--r--   0        0        0       89 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/_helpers/dataclasses.py
--rw-r--r--   0        0        0      254 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/_helpers/pydantic.py
--rw-r--r--   0        0        0        0 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/__init__.py
--rw-r--r--   0        0        0     1259 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/backend.py
--rw-r--r--   0        0        0     2962 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/binder.py
--rw-r--r--   0        0        0      887 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/errors.py
--rw-r--r--   0        0        0     2777 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/interfaces.py
--rw-r--r--   0        0        0      113 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/markers/__init__.py
--rw-r--r--   0        0        0      828 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/markers/base.py
--rw-r--r--   0        0        0     2934 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/markers/method.py
--rw-r--r--   0        0        0      636 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/markers/parameter.py
--rw-r--r--   0        0        0     2022 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/markers/response.py
--rw-r--r--   0        0        0     6857 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/response.py
--rw-r--r--   0        0        0     1683 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/service.py
--rw-r--r--   0        0        0     5445 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/signature.py
--rw-r--r--   0        0        0      585 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/core/typevars.py
--rw-r--r--   0        0        0        0 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/py.typed
--rw-r--r--   0        0        0       50 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/__init__.py
--rw-r--r--   0        0        0       40 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/__init__.py
--rw-r--r--   0        0        0       80 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/abc/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/abc/containers.py
--rw-r--r--   0        0        0      693 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/abc/interfaces.py
--rw-r--r--   0        0        0       75 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/markers/__init__.py
--rw-r--r--   0        0        0     7678 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/markers/request.py
--rw-r--r--   0        0        0     2010 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/markers/response.py
--rw-r--r--   0        0        0      553 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/http/request.py
--rw-r--r--   0        0        0      112 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/httpx/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/httpx/backends/__init__.py
--rw-r--r--   0        0        0     2587 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/httpx/backends/async_.py
--rw-r--r--   0        0        0      814 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/httpx/backends/base.py
--rw-r--r--   0        0        0     2531 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/httpx/backends/sync.py
--rw-r--r--   0        0        0        0 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/shared/__init__.py
--rw-r--r--   0        0        0      224 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/shared/request.py
--rw-r--r--   0        0        0      216 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/soap/__init__.py
--rw-r--r--   0        0        0      520 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/soap/abc.py
--rw-r--r--   0        0        0     1207 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/soap/markers.py
--rw-r--r--   0        0        0      398 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/soap/request.py
--rw-r--r--   0        0        0     1117 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/soap/response.py
--rw-r--r--   0        0        0      110 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/zeep/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/zeep/backends/__init__.py
--rw-r--r--   0        0        0     4957 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/zeep/backends/async_.py
--rw-r--r--   0        0        0     4011 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/zeep/backends/base.py
--rw-r--r--   0        0        0     4220 2024-04-08 14:44:23.788561 combadge-4.2.3/combadge/support/zeep/backends/sync.py
--rw-r--r--   0        0        0     3412 2024-04-08 14:44:35.064646 combadge-4.2.3/pyproject.toml
--rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 combadge-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11350 2024-05-27 11:01:46.018339 combadge-4.2.4/LICENSE
+-rw-r--r--   0        0        0     2135 2024-05-27 11:01:46.018339 combadge-4.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/_helpers/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/_helpers/dataclasses.py
+-rw-r--r--   0        0        0      254 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/_helpers/pydantic.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/__init__.py
+-rw-r--r--   0        0        0     1259 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/backend.py
+-rw-r--r--   0        0        0     2962 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/binder.py
+-rw-r--r--   0        0        0      887 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/errors.py
+-rw-r--r--   0        0        0     2777 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/interfaces.py
+-rw-r--r--   0        0        0      113 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/markers/__init__.py
+-rw-r--r--   0        0        0      828 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/markers/base.py
+-rw-r--r--   0        0        0     2934 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/markers/method.py
+-rw-r--r--   0        0        0      636 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/markers/parameter.py
+-rw-r--r--   0        0        0     2022 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/markers/response.py
+-rw-r--r--   0        0        0     6857 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/response.py
+-rw-r--r--   0        0        0     1683 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/service.py
+-rw-r--r--   0        0        0     5445 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/signature.py
+-rw-r--r--   0        0        0      585 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/core/typevars.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/py.typed
+-rw-r--r--   0        0        0       50 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/abc/__init__.py
+-rw-r--r--   0        0        0     1707 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/abc/containers.py
+-rw-r--r--   0        0        0      693 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/abc/interfaces.py
+-rw-r--r--   0        0        0       75 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/markers/__init__.py
+-rw-r--r--   0        0        0     7678 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/markers/request.py
+-rw-r--r--   0        0        0     2010 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/markers/response.py
+-rw-r--r--   0        0        0      553 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/http/request.py
+-rw-r--r--   0        0        0      112 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/httpx/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/httpx/backends/__init__.py
+-rw-r--r--   0        0        0     2587 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/httpx/backends/async_.py
+-rw-r--r--   0        0        0      814 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/httpx/backends/base.py
+-rw-r--r--   0        0        0     2531 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/httpx/backends/sync.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/shared/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/shared/request.py
+-rw-r--r--   0        0        0      216 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/soap/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/soap/abc.py
+-rw-r--r--   0        0        0     1207 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/soap/markers.py
+-rw-r--r--   0        0        0      398 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/soap/request.py
+-rw-r--r--   0        0        0     1117 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/soap/response.py
+-rw-r--r--   0        0        0      110 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/zeep/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/zeep/backends/__init__.py
+-rw-r--r--   0        0        0     4957 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/zeep/backends/async_.py
+-rw-r--r--   0        0        0     4011 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/zeep/backends/base.py
+-rw-r--r--   0        0        0     4220 2024-05-27 11:01:46.018339 combadge-4.2.4/combadge/support/zeep/backends/sync.py
+-rw-r--r--   0        0        0     3440 2024-05-27 11:01:55.202431 combadge-4.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 combadge-4.2.4/PKG-INFO
```

### Comparing `combadge-4.2.3/LICENSE` & `combadge-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/README.md` & `combadge-4.2.4/README.md`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/backend.py` & `combadge-4.2.4/combadge/core/backend.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/binder.py` & `combadge-4.2.4/combadge/core/binder.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/errors.py` & `combadge-4.2.4/combadge/core/errors.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/interfaces.py` & `combadge-4.2.4/combadge/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/markers/base.py` & `combadge-4.2.4/combadge/core/markers/base.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/markers/method.py` & `combadge-4.2.4/combadge/core/markers/method.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/markers/parameter.py` & `combadge-4.2.4/combadge/core/markers/parameter.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/markers/response.py` & `combadge-4.2.4/combadge/core/markers/response.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/response.py` & `combadge-4.2.4/combadge/core/response.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/service.py` & `combadge-4.2.4/combadge/core/service.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/signature.py` & `combadge-4.2.4/combadge/core/signature.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/core/typevars.py` & `combadge-4.2.4/combadge/core/typevars.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/http/abc/interfaces.py` & `combadge-4.2.4/combadge/support/http/abc/interfaces.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/http/markers/request.py` & `combadge-4.2.4/combadge/support/http/markers/request.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/http/markers/response.py` & `combadge-4.2.4/combadge/support/http/markers/response.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/http/request.py` & `combadge-4.2.4/combadge/support/http/request.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/httpx/backends/async_.py` & `combadge-4.2.4/combadge/support/httpx/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/httpx/backends/base.py` & `combadge-4.2.4/combadge/support/httpx/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/httpx/backends/sync.py` & `combadge-4.2.4/combadge/support/httpx/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/soap/markers.py` & `combadge-4.2.4/combadge/support/soap/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/soap/response.py` & `combadge-4.2.4/combadge/support/soap/response.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/zeep/backends/async_.py` & `combadge-4.2.4/combadge/support/zeep/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/zeep/backends/base.py` & `combadge-4.2.4/combadge/support/zeep/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/combadge/support/zeep/backends/sync.py` & `combadge-4.2.4/combadge/support/zeep/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-4.2.3/pyproject.toml` & `combadge-4.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 description = "Generic API client based on Pydantic"
 keywords = ["api", "api-client", "pydantic"]
 license = "Apache-2.0"
 name = "combadge"
 readme = "README.md"
 repository = "https://github.com/kpn/combadge"
-version = "4.2.3"
+version = "4.2.4"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -40,14 +40,16 @@
 pretty = true
 warn_unused_configs = true
 warn_redundant_casts = true
 
 [tool.ruff]
 line-length = 120
 target-version = "py38"
+
+[tool.ruff.lint]
 select = [
     "A",
     "ANN",
     "B",
     "C4",
     "COM",
     "D",
@@ -81,18 +83,18 @@
     "D407",
     "D413",
     "TRY003",
     "UP006", # Python 3.9+
 ]
 unfixable = ["B"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["D101", "D102", "D106"]
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.pytest.ini_options]
 addopts = "--block-network --cov=./ --cov-report=xml"
 asyncio_mode = "auto"
 
 [tool.coverage.run]
@@ -126,17 +128,17 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 mypy = "1.9.0"
 pytest = "8.1.1"
-pytest-cov = "4.1.0"
+pytest-cov = "5.0.0"
 types-requests = "^2.28.11.8"
-ruff = "0.3.5"
+ruff = "0.4.5"
 pytest-recording = "0.13.1"
 pytest-asyncio = "0.23.6"
 urllib3 = "1.26.18"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `combadge-4.2.3/PKG-INFO` & `combadge-4.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combadge
-Version: 4.2.3
+Version: 4.2.4
 Summary: Generic API client based on Pydantic
 Home-page: https://github.com/kpn/combadge
 License: Apache-2.0
 Keywords: api,api-client,pydantic
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.1,<4.0.0
```

