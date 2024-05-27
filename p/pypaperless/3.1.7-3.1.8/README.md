# Comparing `tmp/pypaperless-3.1.7.tar.gz` & `tmp/pypaperless-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaperless-3.1.7.tar", max compression
+gzip compressed data, was "pypaperless-3.1.8.tar", max compression
```

## Comparing `pypaperless-3.1.7.tar` & `pypaperless-3.1.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2024-05-22 11:19:26.620070 pypaperless-3.1.7/LICENSE.md
--rw-r--r--   0        0        0     2605 2024-05-22 11:19:26.620070 pypaperless-3.1.7/README.md
--rw-r--r--   0        0        0     3720 2024-05-22 11:19:37.891985 pypaperless-3.1.7/pyproject.toml
--rw-r--r--   0        0        0       73 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/__init__.py
--rw-r--r--   0        0        0    11483 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/api.py
--rw-r--r--   0        0        0     3876 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/const.py
--rw-r--r--   0        0        0     1741 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/exceptions.py
--rw-r--r--   0        0        0      899 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/helpers.py
--rw-r--r--   0        0        0     1260 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/__init__.py
--rw-r--r--   0        0        0     3797 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/base.py
--rw-r--r--   0        0        0     6766 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/classifiers.py
--rw-r--r--   0        0        0     5891 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/common.py
--rw-r--r--   0        0        0     1500 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/config.py
--rw-r--r--   0        0        0     1654 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/custom_fields.py
--rw-r--r--   0        0        0    19769 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/documents.py
--rw-r--r--   0        0        0       93 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/generators/__init__.py
--rw-r--r--   0        0        0     2112 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/generators/page.py
--rw-r--r--   0        0        0     3041 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mails.py
--rw-r--r--   0        0        0       37 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/__init__.py
--rw-r--r--   0        0        0      288 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/__init__.py
--rw-r--r--   0        0        0     1009 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/callable.py
--rw-r--r--   0        0        0      916 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/draftable.py
--rw-r--r--   0        0        0     2893 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/iterable.py
--rw-r--r--   0        0        0      765 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/securable.py
--rw-r--r--   0        0        0      413 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/__init__.py
--rw-r--r--   0        0        0     2169 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/creatable.py
--rw-r--r--   0        0        0      382 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/data_fields.py
--rw-r--r--   0        0        0      755 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/deletable.py
--rw-r--r--   0        0        0      742 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/securable.py
--rw-r--r--   0        0        0     2641 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/updatable.py
--rw-r--r--   0        0        0     2660 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/pages.py
--rw-r--r--   0        0        0     2201 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/permissions.py
--rw-r--r--   0        0        0     1390 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/saved_views.py
--rw-r--r--   0        0        0     1856 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/share_links.py
--rw-r--r--   0        0        0     1802 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/status.py
--rw-r--r--   0        0        0     2735 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/tasks.py
--rw-r--r--   0        0        0     7307 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/utils/__init__.py
--rw-r--r--   0        0        0     4564 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/workflows.py
--rw-r--r--   0        0        0        0 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/py.typed
--rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 pypaperless-3.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-27 17:44:37.808008 pypaperless-3.1.8/LICENSE.md
+-rw-r--r--   0        0        0     2605 2024-05-27 17:44:37.808008 pypaperless-3.1.8/README.md
+-rw-r--r--   0        0        0     3720 2024-05-27 17:44:49.615950 pypaperless-3.1.8/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/__init__.py
+-rw-r--r--   0        0        0    11501 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/api.py
+-rw-r--r--   0        0        0     3876 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/const.py
+-rw-r--r--   0        0        0     1741 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/exceptions.py
+-rw-r--r--   0        0        0      899 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/helpers.py
+-rw-r--r--   0        0        0     1260 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/__init__.py
+-rw-r--r--   0        0        0     3797 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/base.py
+-rw-r--r--   0        0        0     6766 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/classifiers.py
+-rw-r--r--   0        0        0     5891 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/common.py
+-rw-r--r--   0        0        0     1500 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/config.py
+-rw-r--r--   0        0        0     1654 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/custom_fields.py
+-rw-r--r--   0        0        0    19769 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/documents.py
+-rw-r--r--   0        0        0       93 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/generators/__init__.py
+-rw-r--r--   0        0        0     2112 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/generators/page.py
+-rw-r--r--   0        0        0     3041 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mails.py
+-rw-r--r--   0        0        0       37 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mixins/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/__init__.py
+-rw-r--r--   0        0        0     1009 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/callable.py
+-rw-r--r--   0        0        0      916 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/draftable.py
+-rw-r--r--   0        0        0     2893 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/iterable.py
+-rw-r--r--   0        0        0      765 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/securable.py
+-rw-r--r--   0        0        0      413 2024-05-27 17:44:37.808008 pypaperless-3.1.8/src/pypaperless/models/mixins/models/__init__.py
+-rw-r--r--   0        0        0     2169 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/mixins/models/creatable.py
+-rw-r--r--   0        0        0      382 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/mixins/models/data_fields.py
+-rw-r--r--   0        0        0      755 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/mixins/models/deletable.py
+-rw-r--r--   0        0        0      742 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/mixins/models/securable.py
+-rw-r--r--   0        0        0     2641 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/mixins/models/updatable.py
+-rw-r--r--   0        0        0     2660 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/pages.py
+-rw-r--r--   0        0        0     2201 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/permissions.py
+-rw-r--r--   0        0        0     1390 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/saved_views.py
+-rw-r--r--   0        0        0     1856 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/share_links.py
+-rw-r--r--   0        0        0     1802 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/status.py
+-rw-r--r--   0        0        0     2735 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/tasks.py
+-rw-r--r--   0        0        0     7307 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/utils/__init__.py
+-rw-r--r--   0        0        0     4564 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/models/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:37.812008 pypaperless-3.1.8/src/pypaperless/py.typed
+-rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 pypaperless-3.1.8/PKG-INFO
```

### Comparing `pypaperless-3.1.7/LICENSE.md` & `pypaperless-3.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/README.md` & `pypaperless-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/pyproject.toml` & `pypaperless-3.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.poetry]
 name = "pypaperless"
-version = "3.1.7"
+version = "3.1.8"
 description = "Little api client for paperless(-ngx)."
 authors = ["Tobias Schulz <public.dev@tbsch.de>"]
 maintainers = ["Tobias Schulz <public.dev@tbsch.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tb1337/paperless-api"
 repository = "https://github.com/tb1337/paperless-api"
```

### Comparing `pypaperless-3.1.7/src/pypaperless/api.py` & `pypaperless-3.1.8/src/pypaperless/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     @staticmethod
     def _process_form(data: dict[str, Any]) -> aiohttp.FormData:
         """Process form data and create a `aiohttp.FormData` object.
 
         Every field item gets converted to a string-like object.
         """
-        form = aiohttp.FormData()
+        form = aiohttp.FormData(quote_fields=False)
 
         def _add_form_value(name: str | None, value: Any) -> Any:
             if value is None:
                 return
             params = {}
             if isinstance(value, dict):
                 for dict_key, dict_value in value.items():
```

### Comparing `pypaperless-3.1.7/src/pypaperless/const.py` & `pypaperless-3.1.8/src/pypaperless/const.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/exceptions.py` & `pypaperless-3.1.8/src/pypaperless/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/helpers.py` & `pypaperless-3.1.8/src/pypaperless/helpers.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/__init__.py` & `pypaperless-3.1.8/src/pypaperless/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/base.py` & `pypaperless-3.1.8/src/pypaperless/models/base.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/classifiers.py` & `pypaperless-3.1.8/src/pypaperless/models/classifiers.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/common.py` & `pypaperless-3.1.8/src/pypaperless/models/common.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/config.py` & `pypaperless-3.1.8/src/pypaperless/models/config.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/custom_fields.py` & `pypaperless-3.1.8/src/pypaperless/models/custom_fields.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/documents.py` & `pypaperless-3.1.8/src/pypaperless/models/documents.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/generators/page.py` & `pypaperless-3.1.8/src/pypaperless/models/generators/page.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mails.py` & `pypaperless-3.1.8/src/pypaperless/models/mails.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/callable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/callable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/draftable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/draftable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/iterable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/iterable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/securable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/helpers/securable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/models/creatable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/models/creatable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/models/deletable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/models/deletable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/models/securable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/models/securable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/mixins/models/updatable.py` & `pypaperless-3.1.8/src/pypaperless/models/mixins/models/updatable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/pages.py` & `pypaperless-3.1.8/src/pypaperless/models/pages.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/permissions.py` & `pypaperless-3.1.8/src/pypaperless/models/permissions.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/saved_views.py` & `pypaperless-3.1.8/src/pypaperless/models/saved_views.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/share_links.py` & `pypaperless-3.1.8/src/pypaperless/models/share_links.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/status.py` & `pypaperless-3.1.8/src/pypaperless/models/status.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/tasks.py` & `pypaperless-3.1.8/src/pypaperless/models/tasks.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/utils/__init__.py` & `pypaperless-3.1.8/src/pypaperless/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/src/pypaperless/models/workflows.py` & `pypaperless-3.1.8/src/pypaperless/models/workflows.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.7/PKG-INFO` & `pypaperless-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypaperless
-Version: 3.1.7
+Version: 3.1.8
 Summary: Little api client for paperless(-ngx).
 Home-page: https://github.com/tb1337/paperless-api
 License: MIT
 Keywords: library,async,api-client,python3,paperless-ngx
 Author: Tobias Schulz
 Author-email: public.dev@tbsch.de
 Maintainer: Tobias Schulz
```

