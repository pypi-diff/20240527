# Comparing `tmp/drf_pydantic-2.2.0.tar.gz` & `tmp/drf_pydantic-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic-2.2.0.tar", max compression
+gzip compressed data, was "drf_pydantic-2.3.0.tar", max compression
```

## Comparing `drf_pydantic-2.2.0.tar` & `drf_pydantic-2.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/LICENSE
--rw-r--r--   0        0        0     6195 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/README.md
--rw-r--r--   0        0        0     2732 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       66 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/src/drf_pydantic/__init__.py
--rw-r--r--   0        0        0     1810 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/src/drf_pydantic/base_model.py
--rw-r--r--   0        0        0      269 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/src/drf_pydantic/errors.py
--rw-r--r--   0        0        0    13753 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/src/drf_pydantic/parse.py
--rw-r--r--   0        0        0        0 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/src/drf_pydantic/py.typed
--rw-r--r--   0        0        0     1312 2024-02-14 05:00:54.732096 drf_pydantic-2.2.0/src/drf_pydantic/utils.py
--rw-r--r--   0        0        0     7463 1970-01-01 00:00:00.000000 drf_pydantic-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/LICENSE
+-rw-r--r--   0        0        0     6195 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/README.md
+-rw-r--r--   0        0        0     2732 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/src/drf_pydantic/__init__.py
+-rw-r--r--   0        0        0     1810 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/src/drf_pydantic/base_model.py
+-rw-r--r--   0        0        0      269 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/src/drf_pydantic/errors.py
+-rw-r--r--   0        0        0    13973 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/src/drf_pydantic/parse.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/src/drf_pydantic/py.typed
+-rw-r--r--   0        0        0     1312 2024-05-27 19:03:05.250294 drf_pydantic-2.3.0/src/drf_pydantic/utils.py
+-rw-r--r--   0        0        0     7463 1970-01-01 00:00:00.000000 drf_pydantic-2.3.0/PKG-INFO
```

### Comparing `drf_pydantic-2.2.0/LICENSE` & `drf_pydantic-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic-2.2.0/README.md` & `drf_pydantic-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `drf_pydantic-2.2.0/pyproject.toml` & `drf_pydantic-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pydantic"
-version = "2.2.0"
+version = "2.3.0"
 description = "Use pydantic with the Django REST framework"
 license = "MIT"
 authors = ["George Bocharov <bocharovgeorgii@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/georgebv/drf-pydantic"
 repository = "https://github.com/georgebv/drf-pydantic"
 keywords = ["django", "drf", "pydantic", "typing", "rest", "api"]
```

### Comparing `drf_pydantic-2.2.0/src/drf_pydantic/base_model.py` & `drf_pydantic-2.3.0/src/drf_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic-2.2.0/src/drf_pydantic/parse.py` & `drf_pydantic-2.3.0/src/drf_pydantic/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,21 @@
     drf_field_kwargs: dict[str, typing.Any] = {
         "required": field.is_required(),
     }
     _default_value = field.get_default(call_default_factory=True)
     if _default_value is not pydantic_core.PydanticUndefined:
         drf_field_kwargs["default"] = _default_value
 
+    # Adding description as help_text
+    if (
+        field.description is not pydantic_core.PydanticUndefined
+        and field.description is not None
+    ):
+        drf_field_kwargs["help_text"] = field.description
+
     # Process constraints
     for item in field.metadata:
         if isinstance(item, pydantic.StringConstraints):
             drf_field_kwargs["min_length"] = (
                 max(
                     drf_field_kwargs.get("min_length", float("-inf")),
                     item.min_length,
```

### Comparing `drf_pydantic-2.2.0/src/drf_pydantic/utils.py` & `drf_pydantic-2.3.0/src/drf_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic-2.2.0/PKG-INFO` & `drf_pydantic-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pydantic
-Version: 2.2.0
+Version: 2.3.0
 Summary: Use pydantic with the Django REST framework
 Home-page: https://github.com/georgebv/drf-pydantic
 License: MIT
 Keywords: django,drf,pydantic,typing,rest,api
 Author: George Bocharov
 Author-email: bocharovgeorgii@gmail.com
 Requires-Python: >=3.9,<4.0
```

