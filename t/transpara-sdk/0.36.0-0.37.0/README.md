# Comparing `tmp/transpara_sdk-0.36.0.tar.gz` & `tmp/transpara_sdk-0.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpara_sdk-0.36.0.tar", last modified: Mon May 27 19:47:43 2024, max compression
+gzip compressed data, was "transpara_sdk-0.37.0.tar", last modified: Mon May 27 19:54:52 2024, max compression
```

## Comparing `transpara_sdk-0.36.0.tar` & `transpara_sdk-0.37.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:47:43.860530 transpara_sdk-0.36.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.36.0/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-27 19:47:43.860530 transpara_sdk-0.36.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.36.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      862 2024-05-27 19:42:14.000000 transpara_sdk-0.36.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-27 19:47:43.860530 transpara_sdk-0.36.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:47:43.856530 transpara_sdk-0.36.0/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:47:43.856530 transpara_sdk-0.36.0/src/transpara/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.36.0/src/transpara/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:47:43.856530 transpara_sdk-0.36.0/src/transpara/internal/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:47:43.856530 transpara_sdk-0.36.0/src/transpara/internal/extra-hooks/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2024-05-21 18:17:29.000000 transpara_sdk-0.36.0/src/transpara/internal/extra-hooks/hook-opentelemetry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10930 2024-05-27 19:41:24.000000 transpara_sdk-0.36.0/src/transpara/internal/output_tstore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4677 2024-05-27 19:17:34.000000 transpara_sdk-0.36.0/src/transpara/internal/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.36.0/src/transpara/logging_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.36.0/src/transpara/tlogging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.36.0/src/transpara/tracing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:47:43.856530 transpara_sdk-0.36.0/src/transpara_sdk.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-27 19:47:43.000000 transpara_sdk-0.36.0/src/transpara_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      496 2024-05-27 19:47:43.000000 transpara_sdk-0.36.0/src/transpara_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-27 19:47:43.000000 transpara_sdk-0.36.0/src/transpara_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-27 19:47:43.000000 transpara_sdk-0.36.0/src/transpara_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-05-27 19:47:43.000000 transpara_sdk-0.36.0/src/transpara_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:47:43.856530 transpara_sdk-0.36.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.36.0/tests/tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:54:52.557853 transpara_sdk-0.37.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.37.0/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-27 19:54:52.553853 transpara_sdk-0.37.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.37.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      862 2024-05-27 19:54:46.000000 transpara_sdk-0.37.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-27 19:54:52.557853 transpara_sdk-0.37.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:54:52.553853 transpara_sdk-0.37.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:54:52.553853 transpara_sdk-0.37.0/src/transpara/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.37.0/src/transpara/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:54:52.553853 transpara_sdk-0.37.0/src/transpara/internal/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:54:52.553853 transpara_sdk-0.37.0/src/transpara/internal/extra-hooks/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2024-05-21 18:17:29.000000 transpara_sdk-0.37.0/src/transpara/internal/extra-hooks/hook-opentelemetry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11003 2024-05-27 19:54:31.000000 transpara_sdk-0.37.0/src/transpara/internal/output_tstore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4677 2024-05-27 19:17:34.000000 transpara_sdk-0.37.0/src/transpara/internal/settings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.37.0/src/transpara/logging_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.37.0/src/transpara/tlogging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.37.0/src/transpara/tracing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:54:52.553853 transpara_sdk-0.37.0/src/transpara_sdk.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-27 19:54:52.000000 transpara_sdk-0.37.0/src/transpara_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      496 2024-05-27 19:54:52.000000 transpara_sdk-0.37.0/src/transpara_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-27 19:54:52.000000 transpara_sdk-0.37.0/src/transpara_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-27 19:54:52.000000 transpara_sdk-0.37.0/src/transpara_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-05-27 19:54:52.000000 transpara_sdk-0.37.0/src/transpara_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:54:52.553853 transpara_sdk-0.37.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.37.0/tests/tests.py
```

### Comparing `transpara_sdk-0.36.0/LICENSE.txt` & `transpara_sdk-0.37.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.36.0/PKG-INFO` & `transpara_sdk-0.37.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpara-sdk
-Version: 0.36.0
+Version: 0.37.0
 Summary: Transpara Python SDK
 Project-URL: homepage, https://transpara.com
 License-File: LICENSE.txt
 Requires-Dist: jsonpickle==1.4.2
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
```

### Comparing `transpara_sdk-0.36.0/README.md` & `transpara_sdk-0.37.0/README.md`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.36.0/pyproject.toml` & `transpara_sdk-0.37.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 author = "Transpara"
 author_email = "arturo.aguilar@transpara.com"
 
 [project]
 name = "transpara-sdk"
-version = "0.36.0"
+version = "0.37.0"
 description = "Transpara Python SDK"
 dependencies = [
     "jsonpickle==1.4.2",
     "asyncio==3.4.3",
     "opentelemetry-api==1.20.0",
     "opentelemetry-sdk==1.20.0",
     "opentelemetry-exporter-otlp==1.20.0",
```

### Comparing `transpara_sdk-0.36.0/src/transpara/internal/output_tstore.py` & `transpara_sdk-0.37.0/src/transpara/internal/output_tstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,32 +230,34 @@
     for tag, value in tags.items():
         labels = add_labels(sanitize_string(tag), sanitize_string(value), labels)
         
     #we create a sample for EACH field
     #if not output_tstore.config.TREAT_FIELDS_AS_LABELS:
     for field, value in fields.items():
 
+        current_labels = labels
+
         if output_tstore.config.USE_HOST_AS_METRIC_NAME or output_tstore.config.METRIC_NAME:
 
             metric_name = metric
 
             if sanitize_string(field) == "value":
-                labels = add_labels("metric", telegraf_metric_name, labels)
+                current_labels = add_labels("metric", telegraf_metric_name, current_labels)
             else:
-                labels = add_labels("metric", f"{telegraf_metric_name}_{sanitize_string(field)}", labels)
+                current_labels = add_labels("metric", f"{telegraf_metric_name}_{sanitize_string(field)}", current_labels)
 
 
         else:
 
             if sanitize_string(field) == "value":
                 metric_name = metric
             else:
                 metric_name = f"{metric}_{sanitize_string(field)}"
 
-        await output_tstore.enqueue_data(metric_name, value, ts, labels, output_tstore.config.get_tz())
+        await output_tstore.enqueue_data(metric_name, value, ts, current_labels, output_tstore.config.get_tz())
 
     # #We treat the fields as additional labels
     # Chat with michael on15 may 24, just treat it as a lookup if it has a value and a timestamp.
     # else:
     #     for field, value in fields.items():
     #         current_labels = add_labels(sanitize_string(field), sanitize_string(value), labels)
     #         await output_tstore.enqueue_data(measurement, value, ts, current_labels, output_tstore.config.get_tz())
```

### Comparing `transpara_sdk-0.36.0/src/transpara/internal/settings.py` & `transpara_sdk-0.37.0/src/transpara/internal/settings.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.36.0/src/transpara/logging_config.py` & `transpara_sdk-0.37.0/src/transpara/logging_config.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.36.0/src/transpara/tlogging.py` & `transpara_sdk-0.37.0/src/transpara/tlogging.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.36.0/src/transpara/tracing.py` & `transpara_sdk-0.37.0/src/transpara/tracing.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.36.0/src/transpara_sdk.egg-info/PKG-INFO` & `transpara_sdk-0.37.0/src/transpara_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpara-sdk
-Version: 0.36.0
+Version: 0.37.0
 Summary: Transpara Python SDK
 Project-URL: homepage, https://transpara.com
 License-File: LICENSE.txt
 Requires-Dist: jsonpickle==1.4.2
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
```

### Comparing `transpara_sdk-0.36.0/tests/tests.py` & `transpara_sdk-0.37.0/tests/tests.py`

 * *Files identical despite different names*

