# Comparing `tmp/apexdevkit-1.2.1.tar.gz` & `tmp/apexdevkit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apexdevkit-1.2.1.tar", max compression
+gzip compressed data, was "apexdevkit-1.2.2.tar", max compression
```

## Comparing `apexdevkit-1.2.1.tar` & `apexdevkit-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/LICENSE
--rw-r--r--   0        0        0       12 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/__init__.py
--rw-r--r--   0        0        0       81 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/annotation/__init__.py
--rw-r--r--   0        0        0     1475 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/annotation/deprecate.py
--rw-r--r--   0        0        0      903 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/error.py
--rw-r--r--   0        0        0      597 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/__init__.py
--rw-r--r--   0        0        0      970 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/builder.py
--rw-r--r--   0        0        0      255 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/dependable.py
--rw-r--r--   0        0        0      233 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/docs.py
--rw-r--r--   0        0        0     1699 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/response.py
--rw-r--r--   0        0        0     7745 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/router.py
--rw-r--r--   0        0        0     3603 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/schema.py
--rw-r--r--   0        0        0     2616 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/fastapi/service.py
--rw-r--r--   0        0        0      398 2024-05-27 15:39:04.153942 apexdevkit-1.2.1/apexdevkit/http/__init__.py
--rw-r--r--   0        0        0     2022 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/fake.py
--rw-r--r--   0        0        0     3060 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/fluent.py
--rw-r--r--   0        0        0     2763 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/httpx.py
--rw-r--r--   0        0        0     1026 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/json.py
--rw-r--r--   0        0        0      201 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/http/url.py
--rw-r--r--   0        0        0        0 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/py.typed
--rw-r--r--   0        0        0      334 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/__init__.py
--rw-r--r--   0        0        0      772 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/connector.py
--rw-r--r--   0        0        0     2362 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/database.py
--rw-r--r--   0        0        0     3388 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/in_memory.py
--rw-r--r--   0        0        0      653 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/repository/interface.py
--rw-r--r--   0        0        0      238 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/testing/__init__.py
--rw-r--r--   0        0        0     1305 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/testing/database.py
--rw-r--r--   0        0        0     7774 2024-05-27 15:39:04.157942 apexdevkit-1.2.1/apexdevkit/testing/rest.py
--rw-r--r--   0        0        0      992 2024-05-27 15:39:16.746025 apexdevkit-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 apexdevkit-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-27 16:06:49.816435 apexdevkit-1.2.2/LICENSE
+-rw-r--r--   0        0        0       12 2024-05-27 16:06:49.816435 apexdevkit-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 16:06:49.816435 apexdevkit-1.2.2/apexdevkit/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-27 16:06:49.816435 apexdevkit-1.2.2/apexdevkit/annotation/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-27 16:06:49.816435 apexdevkit-1.2.2/apexdevkit/annotation/deprecate.py
+-rw-r--r--   0        0        0      903 2024-05-27 16:06:49.816435 apexdevkit-1.2.2/apexdevkit/error.py
+-rw-r--r--   0        0        0      597 2024-05-27 16:06:49.816435 apexdevkit-1.2.2/apexdevkit/fastapi/__init__.py
+-rw-r--r--   0        0        0      970 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/fastapi/builder.py
+-rw-r--r--   0        0        0      255 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/fastapi/dependable.py
+-rw-r--r--   0        0        0      233 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/fastapi/docs.py
+-rw-r--r--   0        0        0     1699 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/fastapi/response.py
+-rw-r--r--   0        0        0     7745 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/fastapi/router.py
+-rw-r--r--   0        0        0     3603 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/fastapi/schema.py
+-rw-r--r--   0        0        0     2616 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/fastapi/service.py
+-rw-r--r--   0        0        0      398 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/http/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/http/fake.py
+-rw-r--r--   0        0        0     3060 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/http/fluent.py
+-rw-r--r--   0        0        0     2763 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/http/httpx.py
+-rw-r--r--   0        0        0     1026 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/http/json.py
+-rw-r--r--   0        0        0      201 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/http/url.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/py.typed
+-rw-r--r--   0        0        0      334 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/repository/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/repository/connector.py
+-rw-r--r--   0        0        0     2362 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/repository/database.py
+-rw-r--r--   0        0        0     3388 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/repository/in_memory.py
+-rw-r--r--   0        0        0      653 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/repository/interface.py
+-rw-r--r--   0        0        0      238 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/testing/__init__.py
+-rw-r--r--   0        0        0     1305 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/testing/database.py
+-rw-r--r--   0        0        0     7774 2024-05-27 16:06:49.820436 apexdevkit-1.2.2/apexdevkit/testing/rest.py
+-rw-r--r--   0        0        0      992 2024-05-27 16:07:02.648444 apexdevkit-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 apexdevkit-1.2.2/PKG-INFO
```

### Comparing `apexdevkit-1.2.1/LICENSE` & `apexdevkit-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/annotation/deprecate.py` & `apexdevkit-1.2.2/apexdevkit/annotation/deprecate.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/error.py` & `apexdevkit-1.2.2/apexdevkit/error.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/fastapi/__init__.py` & `apexdevkit-1.2.2/apexdevkit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/fastapi/builder.py` & `apexdevkit-1.2.2/apexdevkit/fastapi/builder.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/fastapi/response.py` & `apexdevkit-1.2.2/apexdevkit/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/fastapi/router.py` & `apexdevkit-1.2.2/apexdevkit/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/fastapi/schema.py` & `apexdevkit-1.2.2/apexdevkit/fastapi/schema.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/fastapi/service.py` & `apexdevkit-1.2.2/apexdevkit/fastapi/service.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/http/fake.py` & `apexdevkit-1.2.2/apexdevkit/http/fake.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/http/fluent.py` & `apexdevkit-1.2.2/apexdevkit/http/fluent.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/http/httpx.py` & `apexdevkit-1.2.2/apexdevkit/http/httpx.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/http/json.py` & `apexdevkit-1.2.2/apexdevkit/http/json.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/repository/connector.py` & `apexdevkit-1.2.2/apexdevkit/repository/connector.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/repository/database.py` & `apexdevkit-1.2.2/apexdevkit/repository/database.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/repository/in_memory.py` & `apexdevkit-1.2.2/apexdevkit/repository/in_memory.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/repository/interface.py` & `apexdevkit-1.2.2/apexdevkit/repository/interface.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/testing/database.py` & `apexdevkit-1.2.2/apexdevkit/testing/database.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/apexdevkit/testing/rest.py` & `apexdevkit-1.2.2/apexdevkit/testing/rest.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.1/pyproject.toml` & `apexdevkit-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apexdevkit"
-version = "1.2.1"
+version = "1.2.2"
 description = "Apex Development Tools for python."
 authors = ["Apex Dev <dev@apex.ge>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "*"
```

