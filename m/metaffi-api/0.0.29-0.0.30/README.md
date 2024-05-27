# Comparing `tmp/metaffi_api-0.0.29.tar.gz` & `tmp/metaffi_api-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.29.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.30.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.29.tar` & `metaffi_api-0.0.30.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.29/CMakeLists.txt
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.29/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.29/README.md
--rw-r--r--   0        0        0      598 2024-05-20 06:45:10.304035 metaffi_api-0.0.29/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.29/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      469 2024-05-19 16:07:19.521415 metaffi_api-0.0.29/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4918 2024-05-19 13:22:54.324275 metaffi_api-0.0.29/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      484 2024-05-18 16:45:00.514372 metaffi_api-0.0.29/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4619 2024-05-19 03:25:53.676813 metaffi_api-0.0.29/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     2024 2024-05-18 16:43:11.504988 metaffi_api-0.0.29/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     5217 2024-05-19 06:50:11.445337 metaffi_api-0.0.29/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0      715 2024-05-19 13:30:17.499729 metaffi_api-0.0.29/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.29/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.29/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.30/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.30/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.30/README.md
+-rw-r--r--   0        0        0      595 2024-05-27 16:11:10.233020 metaffi_api-0.0.30/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.30/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0     4918 2024-05-19 13:22:54.324275 metaffi_api-0.0.30/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      484 2024-05-18 16:45:00.514372 metaffi_api-0.0.30/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4619 2024-05-19 03:25:53.676813 metaffi_api-0.0.30/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     1068 2024-05-27 16:10:31.483129 metaffi_api-0.0.30/metaffi/metaffihandle.py
+-rw-r--r--   0        0        0     2024 2024-05-18 16:43:11.504988 metaffi_api-0.0.30/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     5217 2024-05-19 06:50:11.445337 metaffi_api-0.0.30/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      715 2024-05-19 13:30:17.499729 metaffi_api-0.0.30/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.30/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.30/PKG-INFO
```

### Comparing `metaffi_api-0.0.29/LICENSE` & `metaffi_api-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.29/metaffi/__init__.py` & `metaffi_api-0.0.30/metaffi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Python MetaFFI API"""
 
-__version__ = "0.0.29"
+__version__ = "0.0.30"
 
-__all__ = ['metaffi', 'metaffi_types', 'metaffi_runtime', 'metaffi_module', 'metaffi_handle', 'metaffi_types', 'xllr_wrapper', 'pycdts_converter', 'metaffi_type_info', 'MetaFFITypes', 'MetaFFIEntity']
+__all__ = ['metaffi', 'metaffi_types', 'metaffi_runtime', 'metaffi_module', 'MetaFFIHandle', 'metaffi_types', 'xllr_wrapper', 'pycdts_converter', 'metaffi_type_info', 'MetaFFITypes', 'MetaFFIEntity']
 
 import metaffi
 from . import metaffi_types
 from . import metaffi_runtime
 from . import metaffi_module
-from .metaffi_handle import metaffi_handle
+from .metaffihandle import MetaFFIHandle
 from . import xllr_wrapper
 from . import pycdts_converter
 from .metaffi_types import metaffi_type_info
 from .metaffi_types import MetaFFITypes
 from .metaffi_module import MetaFFIEntity
```

### Comparing `metaffi_api-0.0.29/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.30/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.29/metaffi/metaffi_module.py` & `metaffi_api-0.0.30/metaffi/metaffi_module.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.29/metaffi/metaffi_types.py` & `metaffi_api-0.0.30/metaffi/metaffi_types.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.29/metaffi/pycdts_converter.py` & `metaffi_api-0.0.30/metaffi/pycdts_converter.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.29/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.30/metaffi/xllr_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.29/publish.ps1` & `metaffi_api-0.0.30/publish.ps1`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.29/pyproject.toml` & `metaffi_api-0.0.30/pyproject.toml`

 * *Files identical despite different names*

