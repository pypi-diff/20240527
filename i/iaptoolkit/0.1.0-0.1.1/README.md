# Comparing `tmp/iaptoolkit-0.1.0.tar.gz` & `tmp/iaptoolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaptoolkit-0.1.0.tar", max compression
+gzip compressed data, was "iaptoolkit-0.1.1.tar", max compression
```

## Comparing `iaptoolkit-0.1.0.tar` & `iaptoolkit-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-05-13 01:02:13.498532 iaptoolkit-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     1343 2024-05-13 01:02:13.498532 iaptoolkit-0.1.0/README.md
--rwxr-xr-x   0        0        0     1010 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4742 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/__init__.py
--rw-r--r--   0        0        0      522 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/constants.py
--rw-r--r--   0        0        0     1507 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/exceptions.py
--rw-r--r--   0        0        0     2896 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/headers.py
--rw-r--r--   0        0        0      673 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/__init__.py
--rw-r--r--   0        0        0     8036 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/service_account.py
--rw-r--r--   0        0        0     1330 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/structs.py
--rw-r--r--   0        0        0     2699 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/tokens/token_datastore.py
--rw-r--r--   0        0        0        0 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/utils/__init__.py
--rw-r--r--   0        0        0     1477 2024-05-13 01:02:13.502532 iaptoolkit-0.1.0/src/iaptoolkit/utils/urls.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 iaptoolkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-27 02:36:21.036247 iaptoolkit-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     1856 2024-05-27 02:36:21.036247 iaptoolkit-0.1.1/README.md
+-rwxr-xr-x   0        0        0     1010 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4742 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/__init__.py
+-rw-r--r--   0        0        0      522 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/constants.py
+-rw-r--r--   0        0        0     1507 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/exceptions.py
+-rw-r--r--   0        0        0     2896 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/headers.py
+-rw-r--r--   0        0        0      673 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/tokens/__init__.py
+-rw-r--r--   0        0        0     8036 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/tokens/service_account.py
+-rw-r--r--   0        0        0     1330 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/tokens/structs.py
+-rw-r--r--   0        0        0     2699 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/tokens/token_datastore.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     1477 2024-05-27 02:36:21.040247 iaptoolkit-0.1.1/src/iaptoolkit/utils/urls.py
+-rw-r--r--   0        0        0     2412 1970-01-01 00:00:00.000000 iaptoolkit-0.1.1/PKG-INFO
```

### Comparing `iaptoolkit-0.1.0/LICENSE` & `iaptoolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/pyproject.toml` & `iaptoolkit-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iaptoolkit"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library of common utils for interacting with Identity-Aware Proxies"
 authors = ["Rob Voigt <code@ravoigt.com>"]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/__init__.py` & `iaptoolkit-0.1.1/src/iaptoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/constants.py` & `iaptoolkit-0.1.1/src/iaptoolkit/constants.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/exceptions.py` & `iaptoolkit-0.1.1/src/iaptoolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/headers.py` & `iaptoolkit-0.1.1/src/iaptoolkit/headers.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/tokens/__init__.py` & `iaptoolkit-0.1.1/src/iaptoolkit/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/tokens/service_account.py` & `iaptoolkit-0.1.1/src/iaptoolkit/tokens/service_account.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/tokens/structs.py` & `iaptoolkit-0.1.1/src/iaptoolkit/tokens/structs.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/tokens/token_datastore.py` & `iaptoolkit-0.1.1/src/iaptoolkit/tokens/token_datastore.py`

 * *Files identical despite different names*

### Comparing `iaptoolkit-0.1.0/src/iaptoolkit/utils/urls.py` & `iaptoolkit-0.1.1/src/iaptoolkit/utils/urls.py`

 * *Files identical despite different names*

