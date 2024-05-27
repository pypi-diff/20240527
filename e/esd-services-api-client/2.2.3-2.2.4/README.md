# Comparing `tmp/esd_services_api_client-2.2.3.tar.gz` & `tmp/esd_services_api_client-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esd_services_api_client-2.2.3.tar", max compression
+gzip compressed data, was "esd_services_api_client-2.2.4.tar", max compression
```

## Comparing `esd_services_api_client-2.2.3.tar` & `esd_services_api_client-2.2.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0    10693 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/LICENSE
--rw-r--r--   0        0        0      111 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/README.md
--rw-r--r--   0        0        0      603 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/__init__.py
--rw-r--r--   0        0        0       22 2024-05-21 14:11:38.392578 esd_services_api_client-2.2.3/esd_services_api_client/_version.py
--rw-r--r--   0        0        0      723 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/beast/__init__.py
--rw-r--r--   0        0        0      754 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/beast/v3/__init__.py
--rw-r--r--   0        0        0    11478 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/beast/v3/_connector.py
--rw-r--r--   0        0        0     6766 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/beast/v3/_models.py
--rw-r--r--   0        0        0     3618 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/boxer/README.md
--rw-r--r--   0        0        0      785 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/boxer/__init__.py
--rw-r--r--   0        0        0     7445 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/boxer/_auth.py
--rw-r--r--   0        0        0      981 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/boxer/_base.py
--rw-r--r--   0        0        0     8677 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/boxer/_connector.py
--rw-r--r--   0        0        0     1702 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/boxer/_models.py
--rw-r--r--   0        0        0      603 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/common/__init__.py
--rw-r--r--   0        0        0      792 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/crystal/__init__.py
--rw-r--r--   0        0        0      837 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/crystal/_api_versions.py
--rw-r--r--   0        0        0    13098 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/crystal/_connector.py
--rw-r--r--   0        0        0     4366 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/crystal/_models.py
--rw-r--r--   0        0        0     9393 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/README.md
--rw-r--r--   0        0        0      627 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/__init__.py
--rw-r--r--   0        0        0      627 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/__init__.py
--rw-r--r--   0        0        0     3338 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/algrorithm_cache.py
--rw-r--r--   0        0        0     1761 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/input_object.py
--rw-r--r--   0        0        0     2019 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/logger_factory.py
--rw-r--r--   0        0        0     3039 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/nexus_object.py
--rw-r--r--   0        0        0     1729 2024-05-21 14:11:26.648474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/socket_provider.py
--rw-r--r--   0        0        0      903 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/__init__.py
--rw-r--r--   0        0        0     2925 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py
--rw-r--r--   0        0        0     3900 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/_remote_algorithm.py
--rw-r--r--   0        0        0     1702 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/distributed.py
--rw-r--r--   0        0        0     4310 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/forked_algorithm.py
--rw-r--r--   0        0        0     1644 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/minimalistic.py
--rw-r--r--   0        0        0     2007 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/recursive.py
--rw-r--r--   0        0        0        0 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/configurations/__init__.py
--rw-r--r--   0        0        0     1091 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/configurations/algorithm_configuration.py
--rw-r--r--   0        0        0      627 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/core/__init__.py
--rw-r--r--   0        0        0    10037 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/core/app_core.py
--rw-r--r--   0        0        0     6674 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/core/app_dependencies.py
--rw-r--r--   0        0        0      696 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/__init__.py
--rw-r--r--   0        0        0      895 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/_nexus_error.py
--rw-r--r--   0        0        0     1622 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/cache_errors.py
--rw-r--r--   0        0        0     1765 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/input_reader_error.py
--rw-r--r--   0        0        0     1991 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/startup_error.py
--rw-r--r--   0        0        0      758 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/__init__.py
--rw-r--r--   0        0        0     3132 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/input_processor.py
--rw-r--r--   0        0        0     3505 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/input_reader.py
--rw-r--r--   0        0        0     2516 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/payload_reader.py
--rw-r--r--   0        0        0        0 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/telemetry/__init__.py
--rw-r--r--   0        0        0     3644 2024-05-21 14:11:26.652474 esd_services_api_client-2.2.3/esd_services_api_client/nexus/telemetry/recorder.py
--rw-r--r--   0        0        0     1237 2024-05-21 14:11:38.392578 esd_services_api_client-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 esd_services_api_client-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10693 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/LICENSE
+-rw-r--r--   0        0        0      111 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/README.md
+-rw-r--r--   0        0        0      603 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-27 10:42:26.932471 esd_services_api_client-2.2.4/esd_services_api_client/_version.py
+-rw-r--r--   0        0        0      723 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/beast/__init__.py
+-rw-r--r--   0        0        0      754 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/beast/v3/__init__.py
+-rw-r--r--   0        0        0    11478 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/beast/v3/_connector.py
+-rw-r--r--   0        0        0     6766 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/beast/v3/_models.py
+-rw-r--r--   0        0        0     3618 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/boxer/README.md
+-rw-r--r--   0        0        0      785 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/boxer/__init__.py
+-rw-r--r--   0        0        0     7445 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/boxer/_auth.py
+-rw-r--r--   0        0        0      981 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/boxer/_base.py
+-rw-r--r--   0        0        0     8677 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/boxer/_connector.py
+-rw-r--r--   0        0        0     1702 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/boxer/_models.py
+-rw-r--r--   0        0        0      603 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/common/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/crystal/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/crystal/_api_versions.py
+-rw-r--r--   0        0        0    13098 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/crystal/_connector.py
+-rw-r--r--   0        0        0     4366 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/crystal/_models.py
+-rw-r--r--   0        0        0     9393 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/README.md
+-rw-r--r--   0        0        0      627 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/__init__.py
+-rw-r--r--   0        0        0      627 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/__init__.py
+-rw-r--r--   0        0        0     3338 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/algrorithm_cache.py
+-rw-r--r--   0        0        0     1761 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/input_object.py
+-rw-r--r--   0        0        0     2019 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/logger_factory.py
+-rw-r--r--   0        0        0     3039 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/nexus_object.py
+-rw-r--r--   0        0        0     1729 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/socket_provider.py
+-rw-r--r--   0        0        0      903 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/__init__.py
+-rw-r--r--   0        0        0     2925 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py
+-rw-r--r--   0        0        0     3900 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/_remote_algorithm.py
+-rw-r--r--   0        0        0     1702 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/distributed.py
+-rw-r--r--   0        0        0     4310 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/forked_algorithm.py
+-rw-r--r--   0        0        0     1644 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/minimalistic.py
+-rw-r--r--   0        0        0     2007 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/recursive.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/configurations/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/configurations/algorithm_configuration.py
+-rw-r--r--   0        0        0      627 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/core/__init__.py
+-rw-r--r--   0        0        0    10211 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/core/app_core.py
+-rw-r--r--   0        0        0     8561 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/core/app_dependencies.py
+-rw-r--r--   0        0        0     2217 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/core/serializers.py
+-rw-r--r--   0        0        0      696 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/__init__.py
+-rw-r--r--   0        0        0      895 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/_nexus_error.py
+-rw-r--r--   0        0        0     1622 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/cache_errors.py
+-rw-r--r--   0        0        0     1765 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/input_reader_error.py
+-rw-r--r--   0        0        0     1991 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/startup_error.py
+-rw-r--r--   0        0        0      758 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/__init__.py
+-rw-r--r--   0        0        0     3132 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/input_processor.py
+-rw-r--r--   0        0        0     3505 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/input_reader.py
+-rw-r--r--   0        0        0     2516 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/payload_reader.py
+-rw-r--r--   0        0        0        0 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/telemetry/__init__.py
+-rw-r--r--   0        0        0     3651 2024-05-27 10:42:14.244542 esd_services_api_client-2.2.4/esd_services_api_client/nexus/telemetry/recorder.py
+-rw-r--r--   0        0        0     1237 2024-05-27 10:42:26.928471 esd_services_api_client-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 esd_services_api_client-2.2.4/PKG-INFO
```

### Comparing `esd_services_api_client-2.2.3/LICENSE` & `esd_services_api_client-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/beast/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/beast/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/beast/v3/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/beast/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/beast/v3/_connector.py` & `esd_services_api_client-2.2.4/esd_services_api_client/beast/v3/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/beast/v3/_models.py` & `esd_services_api_client-2.2.4/esd_services_api_client/beast/v3/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/boxer/README.md` & `esd_services_api_client-2.2.4/esd_services_api_client/boxer/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/boxer/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/boxer/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/boxer/_auth.py` & `esd_services_api_client-2.2.4/esd_services_api_client/boxer/_auth.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/boxer/_base.py` & `esd_services_api_client-2.2.4/esd_services_api_client/boxer/_base.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/boxer/_connector.py` & `esd_services_api_client-2.2.4/esd_services_api_client/boxer/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/boxer/_models.py` & `esd_services_api_client-2.2.4/esd_services_api_client/boxer/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/common/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/common/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/crystal/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/crystal/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/crystal/_api_versions.py` & `esd_services_api_client-2.2.4/esd_services_api_client/crystal/_api_versions.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/crystal/_connector.py` & `esd_services_api_client-2.2.4/esd_services_api_client/crystal/_connector.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/crystal/_models.py` & `esd_services_api_client-2.2.4/esd_services_api_client/crystal/_models.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/README.md` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/README.md`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/algrorithm_cache.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/algrorithm_cache.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/input_object.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/input_object.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/logger_factory.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/logger_factory.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/nexus_object.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/nexus_object.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/abstractions/socket_provider.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/abstractions/socket_provider.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/_baseline_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/_remote_algorithm.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/_remote_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/distributed.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/distributed.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/forked_algorithm.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/forked_algorithm.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/minimalistic.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/minimalistic.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/algorithms/recursive.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/algorithms/recursive.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/configurations/algorithm_configuration.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/configurations/algorithm_configuration.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/core/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/core/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/core/app_core.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/core/app_core.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from typing import final, Type, Optional, Coroutine
 
 import backoff
 import urllib3.exceptions
 import azure.core.exceptions
 from adapta.process_communication import DataSocket
 from adapta.storage.blob.base import StorageClient
-from adapta.storage.models.format import DataFrameJsonSerializationFormat
 from adapta.storage.query_enabled_store import QueryEnabledStore
 from injector import Injector
 
 import esd_services_api_client.nexus.exceptions
 from esd_services_api_client.crystal import (
     add_crystal_args,
     extract_crystal_args,
@@ -48,14 +47,17 @@
 )
 from esd_services_api_client.nexus.configurations.algorithm_configuration import (
     NexusConfiguration,
 )
 from esd_services_api_client.nexus.core.app_dependencies import (
     ServiceConfigurator,
 )
+from esd_services_api_client.nexus.core.serializers import (
+    ResultSerializer,
+)
 from esd_services_api_client.nexus.input.input_processor import InputProcessor
 from esd_services_api_client.nexus.input.input_reader import InputReader
 from esd_services_api_client.nexus.input.payload_reader import (
     AlgorithmPayloadReader,
     AlgorithmPayload,
 )
 from esd_services_api_client.nexus.telemetry.recorder import TelemetryRecorder
@@ -200,23 +202,27 @@
 
             :param: path: path to save the blob
             :param: output_consumer_df: Formatted dataframe into ECCO format
             :param: storage_client: Azure storage client
 
             :return: blob uri
             """
+            dataframe_data = data.dataframe()
+            serializer = self._injector.get(ResultSerializer)
             storage_client = self._injector.get(StorageClient)
             output_path = f"{os.getenv('NEXUS__ALGORITHM_OUTPUT_PATH')}/{self._run_args.request_id}.json"
             blob_path = DataSocket(
                 data_path=output_path, alias="output", data_format="null"
             ).parse_data_path()
             storage_client.save_data_as_blob(
-                data=data.dataframe(),
+                data=dataframe_data,
                 blob_path=blob_path,
-                serialization_format=DataFrameJsonSerializationFormat,
+                serialization_format=serializer.get_serialization_format(
+                    dataframe_data
+                ),
                 overwrite=True,
             )
             return storage_client.get_blob_uri(blob_path=blob_path)
 
         receiver = self._injector.get(CrystalConnector)
 
         match is_transient_exception(ex):
```

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/core/app_dependencies.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/core/app_dependencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 import json
 import os
+import re
 from pydoc import locate
-from typing import final, Type
+from typing import final, Type, Any
 
 from adapta.metrics import MetricsProvider
 from adapta.storage.blob.base import StorageClient
 from adapta.storage.query_enabled_store import QueryEnabledStore
 from injector import Module, singleton, provider
 
 from esd_services_api_client.crystal import CrystalConnector
@@ -41,14 +42,18 @@
 )
 from esd_services_api_client.nexus.input.input_processor import InputProcessor
 from esd_services_api_client.nexus.input.input_reader import InputReader
 from esd_services_api_client.nexus.input.payload_reader import (
     AlgorithmPayload,
 )
 from esd_services_api_client.nexus.telemetry.recorder import TelemetryRecorder
+from esd_services_api_client.nexus.core.serializers import (
+    TelemetrySerializer,
+    ResultSerializer,
+)
 
 
 @final
 class MetricsModule(Module):
     """
     Metrics provider module.
     """
@@ -164,14 +169,56 @@
 
         return ExternalSocketProvider.from_serialized(
             os.getenv("NEXUS__ALGORITHM_INPUT_EXTERNAL_DATA_SOCKETS")
         )
 
 
 @final
+class ResultSerializerModule(Module):
+    """
+    Serialization format module for results.
+    """
+
+    @singleton
+    @provider
+    def provide(self) -> ResultSerializer:
+        """
+        DI factory method.
+        """
+        serializer = ResultSerializer()
+        for serialization_format in locate_classes(
+            re.compile(r"NEXUS__RESULT_SERIALIZATION_FORMAT_(.+)_CLASS")
+        ):
+            serializer = serializer.with_format(serialization_format)
+
+        return serializer
+
+
+@final
+class TelemetrySerializerModule(Module):
+    """
+    Serialization format module for telemetry.
+    """
+
+    @singleton
+    @provider
+    def provide(self) -> TelemetrySerializer:
+        """
+        DI factory method.
+        """
+        serializer = TelemetrySerializer()
+        for serialization_format in locate_classes(
+            re.compile(r"NEXUS__TELEMETRY_SERIALIZATION_FORMAT_(.+)_CLASS")
+        ):
+            serializer = serializer.with_format(serialization_format)
+
+        return serializer
+
+
+@final
 class CacheModule(Module):
     """
     Storage client module.
     """
 
     @singleton
     @provider
@@ -191,14 +238,16 @@
     def __init__(self):
         self._injection_binds = [
             MetricsModule(),
             CrystalReceiverClientModule(),
             QueryEnabledStoreModule(),
             StorageClientModule(),
             ExternalSocketsModule(),
+            TelemetrySerializerModule(),
+            ResultSerializerModule(),
             CacheModule(),
             type(f"{TelemetryRecorder.__name__}Module", (Module,), {})(),
         ]
 
     @property
     def injection_binds(self) -> list:
         """
@@ -237,7 +286,28 @@
         """
         Adds the specified payload instance to the DI container.
         """
         self._injection_binds.append(
             lambda binder: binder.bind(config.__class__, to=config, scope=singleton)
         )
         return self
+
+
+def locate_classes(pattern: re.Pattern) -> list[Type[Any]]:
+    """
+    Locates all classes matching the pattern in the environment. Throws a start-up error if any class is not found.
+    """
+    classes = {
+        (var_name, class_path): locate(class_path)
+        for var_name, class_path in os.environ.items()
+        if pattern.match(var_name)
+    }
+
+    non_located_classes = [
+        name_and_path for name_and_path, class_ in classes.items() if class_ is None
+    ]
+    if non_located_classes:
+        raise FatalStartupConfigurationError(
+            f"Failed to locate classes: {non_located_classes}"
+        )
+
+    return list(classes.values())
```

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/_nexus_error.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/_nexus_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/cache_errors.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/cache_errors.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/input_reader_error.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/input_reader_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/exceptions/startup_error.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/exceptions/startup_error.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/__init__.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/__init__.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/input_processor.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/input_processor.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/input_reader.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/input_reader.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/input/payload_reader.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/input/payload_reader.py`

 * *Files identical despite different names*

### Comparing `esd_services_api_client-2.2.3/esd_services_api_client/nexus/telemetry/recorder.py` & `esd_services_api_client-2.2.4/esd_services_api_client/nexus/telemetry/recorder.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,21 @@
 from functools import partial
 from typing import final
 
 import pandas as pd
 from adapta.metrics import MetricsProvider
 from adapta.process_communication import DataSocket
 from adapta.storage.blob.base import StorageClient
-from adapta.storage.models.format import (
-    DictJsonSerializationFormat,
-    DataFrameParquetSerializationFormat,
-)
 from injector import inject, singleton
 
 from esd_services_api_client.nexus.abstractions.logger_factory import LoggerFactory
 from esd_services_api_client.nexus.abstractions.nexus_object import NexusCoreObject
+from esd_services_api_client.nexus.core.serializers import (
+    TelemetrySerializer,
+)
 
 
 @final
 @singleton
 class TelemetryRecorder(NexusCoreObject):
     """
     Class for instantiating a telemetry recorder that will save all algorithm inputs (run method arguments) to a persistent location.
@@ -33,20 +32,22 @@
     async def _context_close(self):
         pass
 
     @inject
     def __init__(
         self,
         storage_client: StorageClient,
+        serializer: TelemetrySerializer,
         metrics_provider: MetricsProvider,
         logger_factory: LoggerFactory,
     ):
         super().__init__(metrics_provider, logger_factory)
         self._storage_client = storage_client
         self._telemetry_base_path = os.getenv("NEXUS__TELEMETRY_PATH")
+        self._serializer = serializer
 
     async def record(self, run_id: str, **telemetry_args):
         """
         Record all data in telemetry args for the provided run_id.
         """
 
         async def _record(
@@ -70,17 +71,17 @@
                 self._storage_client.save_data_as_blob(
                     data=entity_to_record,
                     blob_path=DataSocket(
                         alias="telemetry",
                         data_path=f"{self._telemetry_base_path}/{entity_name}/{run_id}",
                         data_format="null",
                     ).parse_data_path(),
-                    serialization_format=DictJsonSerializationFormat
-                    if isinstance(entity_to_record, dict)
-                    else DataFrameParquetSerializationFormat,
+                    serialization_format=self._serializer.get_serialization_format(
+                        entity_to_record
+                    ),
                     overwrite=True,
                 )
 
         telemetry_tasks = [
             asyncio.create_task(
                 partial(
                     _record,
```

### Comparing `esd_services_api_client-2.2.3/pyproject.toml` & `esd_services_api_client-2.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esd-services-api-client"
-version = "2.2.3"
+version = "2.2.4"
 description = "Python clients for ESD services"
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>', 'VISA <visa@ecco.com>']
 readme = "README.md"
 license = 'Apache 2.0'
 repository = 'https://github.com/SneaksAndData/esd-services-api-client'
```

### Comparing `esd_services_api_client-2.2.3/PKG-INFO` & `esd_services_api_client-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esd-services-api-client
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python clients for ESD services
 Home-page: https://github.com/SneaksAndData/esd-services-api-client
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

