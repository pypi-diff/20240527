# Comparing `tmp/transpara_sdk-0.32.0.tar.gz` & `tmp/transpara_sdk-0.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpara_sdk-0.32.0.tar", last modified: Wed May 22 18:50:16 2024, max compression
+gzip compressed data, was "transpara_sdk-0.33.0.tar", last modified: Mon May 27 19:11:00 2024, max compression
```

## Comparing `transpara_sdk-0.32.0.tar` & `transpara_sdk-0.33.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:50:16.924781 transpara_sdk-0.32.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.32.0/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-22 18:50:16.924781 transpara_sdk-0.32.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.32.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      862 2024-05-22 18:50:10.000000 transpara_sdk-0.32.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-22 18:50:16.924781 transpara_sdk-0.32.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:50:16.920781 transpara_sdk-0.32.0/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:50:16.920781 transpara_sdk-0.32.0/src/transpara/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.32.0/src/transpara/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:50:16.920781 transpara_sdk-0.32.0/src/transpara/internal/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:50:16.920781 transpara_sdk-0.32.0/src/transpara/internal/extra-hooks/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2024-05-21 18:17:29.000000 transpara_sdk-0.32.0/src/transpara/internal/extra-hooks/hook-opentelemetry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10132 2024-05-22 18:15:38.000000 transpara_sdk-0.32.0/src/transpara/internal/output_tstore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4555 2024-05-22 18:02:58.000000 transpara_sdk-0.32.0/src/transpara/internal/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.32.0/src/transpara/logging_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.32.0/src/transpara/tlogging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.32.0/src/transpara/tracing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:50:16.924781 transpara_sdk-0.32.0/src/transpara_sdk.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-22 18:50:16.000000 transpara_sdk-0.32.0/src/transpara_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      496 2024-05-22 18:50:16.000000 transpara_sdk-0.32.0/src/transpara_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-22 18:50:16.000000 transpara_sdk-0.32.0/src/transpara_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-22 18:50:16.000000 transpara_sdk-0.32.0/src/transpara_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-05-22 18:50:16.000000 transpara_sdk-0.32.0/src/transpara_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-22 18:50:16.924781 transpara_sdk-0.32.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.32.0/tests/tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.33.0/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.33.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      862 2024-05-27 19:10:49.000000 transpara_sdk-0.33.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:11:00.122119 transpara_sdk-0.33.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/src/transpara/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.33.0/src/transpara/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/src/transpara/internal/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/src/transpara/internal/extra-hooks/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2024-05-21 18:17:29.000000 transpara_sdk-0.33.0/src/transpara/internal/extra-hooks/hook-opentelemetry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10646 2024-05-27 19:10:14.000000 transpara_sdk-0.33.0/src/transpara/internal/output_tstore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4657 2024-05-27 19:04:25.000000 transpara_sdk-0.33.0/src/transpara/internal/settings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.33.0/src/transpara/logging_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.33.0/src/transpara/tlogging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.33.0/src/transpara/tracing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/src/transpara_sdk.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      705 2024-05-27 19:11:00.000000 transpara_sdk-0.33.0/src/transpara_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      496 2024-05-27 19:11:00.000000 transpara_sdk-0.33.0/src/transpara_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-27 19:11:00.000000 transpara_sdk-0.33.0/src/transpara_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-27 19:11:00.000000 transpara_sdk-0.33.0/src/transpara_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-05-27 19:11:00.000000 transpara_sdk-0.33.0/src/transpara_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 19:11:00.126119 transpara_sdk-0.33.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.33.0/tests/tests.py
```

### Comparing `transpara_sdk-0.32.0/LICENSE.txt` & `transpara_sdk-0.33.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.32.0/PKG-INFO` & `transpara_sdk-0.33.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpara-sdk
-Version: 0.32.0
+Version: 0.33.0
 Summary: Transpara Python SDK
 Project-URL: homepage, https://transpara.com
 License-File: LICENSE.txt
 Requires-Dist: jsonpickle==1.4.2
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
```

### Comparing `transpara_sdk-0.32.0/README.md` & `transpara_sdk-0.33.0/README.md`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.32.0/pyproject.toml` & `transpara_sdk-0.33.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 author = "Transpara"
 author_email = "arturo.aguilar@transpara.com"
 
 [project]
 name = "transpara-sdk"
-version = "0.32.0"
+version = "0.33.0"
 description = "Transpara Python SDK"
 dependencies = [
     "jsonpickle==1.4.2",
     "asyncio==3.4.3",
     "opentelemetry-api==1.20.0",
     "opentelemetry-sdk==1.20.0",
     "opentelemetry-exporter-otlp==1.20.0",
```

### Comparing `transpara_sdk-0.32.0/src/transpara/internal/output_tstore.py` & `transpara_sdk-0.33.0/src/transpara/internal/output_tstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,16 +211,26 @@
         logger.tdebug("TEXT-I-Invalid data received - {}\n\t({})".format(rawLine,ex))
         return
     
     # pick apart the line, convert to json and construct the labels, etc.
     ts = line['timestamp']
     tags:Dict = line['tags']
     fields:Dict = line['fields']
+
     measurement:str = sanitize_string(line['name'])
 
+    if output_tstore.config.METRIC_NAME:
+        labels = add_labels("metric", measurement, labels)
+        measurement = output_tstore.config.METRIC_NAME
+    elif output_tstore.config.USE_HOST_AS_METRIC_NAME and "host" in tags:
+        labels = add_labels("metric", sanitize_string(tags["host"]), labels)
+        measurement = sanitize_string(tags["host"])
+    elif output_tstore.config.USE_HOST_AS_METRIC_NAME and "host" not in tags:
+        logger.tdebug("Host tag not found, using default measurement name")
+
     # everybody treats tags as Labels
     for tag, value in tags.items():
         labels = add_labels(sanitize_string(tag), sanitize_string(value), labels)
         
     #we create a sample for EACH field
     #if not output_tstore.config.TREAT_FIELDS_AS_LABELS:
     for field, value in fields.items():
```

### Comparing `transpara_sdk-0.32.0/src/transpara/internal/settings.py` & `transpara_sdk-0.33.0/src/transpara/internal/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,18 @@
     TSTORE_API_URL: Optional[str]
     TSTORE_FLUSH_SIZE: int = 50
     OUTPUT_BATCH_SIZE: int = 5
     TSTORE_FLUSH_INTERVAL_SECONDS: Optional[int] = 10
     SOURCE_TZ: str
     LOG_ENQUEUING: bool = False
 
+    #USED on the telegraf mode
+    USE_HOST_AS_METRIC_NAME: bool = False
+    METRIC_NAME: str = None
+
     def get_tz(self) -> pytz.timezone:
         return pytz.timezone(self.SOURCE_TZ)
 
     def get_write_endpoint(self) -> str:
         return urljoin(self.TSTORE_API_URL, 'api/v1/write/write-data?overwrite_data=true')
 
 class BaseExtractorSettings(OutputTstoreSettings):
```

### Comparing `transpara_sdk-0.32.0/src/transpara/logging_config.py` & `transpara_sdk-0.33.0/src/transpara/logging_config.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.32.0/src/transpara/tlogging.py` & `transpara_sdk-0.33.0/src/transpara/tlogging.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.32.0/src/transpara/tracing.py` & `transpara_sdk-0.33.0/src/transpara/tracing.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.32.0/src/transpara_sdk.egg-info/PKG-INFO` & `transpara_sdk-0.33.0/src/transpara_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpara-sdk
-Version: 0.32.0
+Version: 0.33.0
 Summary: Transpara Python SDK
 Project-URL: homepage, https://transpara.com
 License-File: LICENSE.txt
 Requires-Dist: jsonpickle==1.4.2
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
```

### Comparing `transpara_sdk-0.32.0/tests/tests.py` & `transpara_sdk-0.33.0/tests/tests.py`

 * *Files identical despite different names*

