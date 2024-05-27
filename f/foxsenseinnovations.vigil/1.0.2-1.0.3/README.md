# Comparing `tmp/foxsenseinnovations_vigil-1.0.2.tar.gz` & `tmp/foxsenseinnovations_vigil-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxsenseinnovations_vigil-1.0.2.tar", last modified: Fri May 24 06:18:41 2024, max compression
+gzip compressed data, was "foxsenseinnovations_vigil-1.0.3.tar", last modified: Mon May 27 09:16:00 2024, max compression
```

## Comparing `foxsenseinnovations_vigil-1.0.2.tar` & `foxsenseinnovations_vigil-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.447714 foxsenseinnovations_vigil-1.0.2/
--rw-r--r--   0 haripriya   (502) staff       (20)       17 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/MANIFEST.in
--rw-r--r--   0 haripriya   (502) staff       (20)     7500 2024-05-24 06:18:41.447513 foxsenseinnovations_vigil-1.0.2/PKG-INFO
--rw-r--r--   0 haripriya   (502) staff       (20)     7125 2024-05-24 05:42:17.000000 foxsenseinnovations_vigil-1.0.2/README.md
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.442413 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/
--rw-r--r--   0 haripriya   (502) staff       (20)       33 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/__init__.py
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.444513 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/
--rw-r--r--   0 haripriya   (502) staff       (20)      803 2024-05-24 05:25:16.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/__init__.py
--rw-r--r--   0 haripriya   (502) staff       (20)     4758 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_manager_django.py
--rw-r--r--   0 haripriya   (502) staff       (20)      879 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_service.py
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.444973 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/
--rw-r--r--   0 haripriya   (502) staff       (20)       78 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/__init__.py
--rw-r--r--   0 haripriya   (502) staff       (20)      749 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/route_constants.py
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.445650 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/enums/
--rw-r--r--   0 haripriya   (502) staff       (20)       71 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/enums/__init__.py
--rw-r--r--   0 haripriya   (502) staff       (20)      444 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/enums/http_method_enum.py
--rw-r--r--   0 haripriya   (502) staff       (20)     2878 2024-05-24 05:42:44.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/error_manager.py
--rw-r--r--   0 haripriya   (502) staff       (20)     4153 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/job_manager.py
--rw-r--r--   0 haripriya   (502) staff       (20)      983 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil.py
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.446464 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/
--rw-r--r--   0 haripriya   (502) staff       (20)      313 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/__init__.py
--rw-r--r--   0 haripriya   (502) staff       (20)     6580 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py
--rw-r--r--   0 haripriya   (502) staff       (20)      664 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/exception_log_types.py
--rw-r--r--   0 haripriya   (502) staff       (20)     2459 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py
--rw-r--r--   0 haripriya   (502) staff       (20)      607 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.447090 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/
--rw-r--r--   0 haripriya   (502) staff       (20)      133 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/__init__.py
--rw-r--r--   0 haripriya   (502) staff       (20)     6893 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py
--rw-r--r--   0 haripriya   (502) staff       (20)     2167 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/common_utils.py
-drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-24 06:18:41.447286 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/
--rw-r--r--   0 haripriya   (502) staff       (20)     7500 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/PKG-INFO
--rw-r--r--   0 haripriya   (502) staff       (20)     1220 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/SOURCES.txt
--rw-r--r--   0 haripriya   (502) staff       (20)        1 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/dependency_links.txt
--rw-r--r--   0 haripriya   (502) staff       (20)       36 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/requires.txt
--rw-r--r--   0 haripriya   (502) staff       (20)       20 2024-05-24 06:18:41.000000 foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/top_level.txt
--rw-r--r--   0 haripriya   (502) staff       (20)       38 2024-05-24 06:18:41.447753 foxsenseinnovations_vigil-1.0.2/setup.cfg
--rw-r--r--   0 haripriya   (502) staff       (20)      670 2024-05-24 05:58:30.000000 foxsenseinnovations_vigil-1.0.2/setup.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.377586 foxsenseinnovations_vigil-1.0.3/
+-rw-r--r--   0 haripriya   (502) staff       (20)       17 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/MANIFEST.in
+-rw-r--r--   0 haripriya   (502) staff       (20)     7500 2024-05-27 09:16:00.377330 foxsenseinnovations_vigil-1.0.3/PKG-INFO
+-rw-r--r--   0 haripriya   (502) staff       (20)     7125 2024-05-27 08:51:59.000000 foxsenseinnovations_vigil-1.0.3/README.md
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.371715 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/
+-rw-r--r--   0 haripriya   (502) staff       (20)       33 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/__init__.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.373806 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/
+-rw-r--r--   0 haripriya   (502) staff       (20)      803 2024-05-24 05:25:16.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     4758 2024-05-27 07:57:55.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/api_manager_django.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     1148 2024-05-27 07:54:38.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/api_service.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.374324 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/constants/
+-rw-r--r--   0 haripriya   (502) staff       (20)       78 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/constants/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      749 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/constants/route_constants.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.374980 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/enums/
+-rw-r--r--   0 haripriya   (502) staff       (20)       71 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/enums/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      444 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/enums/http_method_enum.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     2895 2024-05-27 08:02:40.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/error_manager.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     4121 2024-05-27 08:33:24.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/job_manager.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      983 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.376061 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/
+-rw-r--r--   0 haripriya   (502) staff       (20)      313 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     6580 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      664 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/exception_log_types.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     2459 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py
+-rw-r--r--   0 haripriya   (502) staff       (20)      607 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.376816 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_utils/
+-rw-r--r--   0 haripriya   (502) staff       (20)      133 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_utils/__init__.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     6893 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py
+-rw-r--r--   0 haripriya   (502) staff       (20)     2167 2024-05-23 08:13:34.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_utils/common_utils.py
+drwxr-xr-x   0 haripriya   (502) staff       (20)        0 2024-05-27 09:16:00.377023 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/
+-rw-r--r--   0 haripriya   (502) staff       (20)     7500 2024-05-27 09:16:00.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/PKG-INFO
+-rw-r--r--   0 haripriya   (502) staff       (20)     1220 2024-05-27 09:16:00.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/SOURCES.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)        1 2024-05-27 09:16:00.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/dependency_links.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)       36 2024-05-27 09:16:00.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/requires.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)       20 2024-05-27 09:16:00.000000 foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/top_level.txt
+-rw-r--r--   0 haripriya   (502) staff       (20)       38 2024-05-27 09:16:00.377627 foxsenseinnovations_vigil-1.0.3/setup.cfg
+-rw-r--r--   0 haripriya   (502) staff       (20)      670 2024-05-27 08:44:35.000000 foxsenseinnovations_vigil-1.0.3/setup.py
```

### Comparing `foxsenseinnovations_vigil-1.0.2/PKG-INFO` & `foxsenseinnovations_vigil-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxsenseinnovations.vigil
-Version: 1.0.2
+Version: 1.0.3
 Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
 License: ISC
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: requests
 Requires-Dist: werkzeug
 Requires-Dist: django
```

### Comparing `foxsenseinnovations_vigil-1.0.2/README.md` & `foxsenseinnovations_vigil-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/__init__.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/__init__.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_manager_django.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/api_manager_django.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/api_service.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/api_service.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from typing import Any, Dict
 import requests
+import logging
 
+logging.basicConfig(level=logging.INFO, format='%(message)s')
 class ApiService:
     """
     ApiService is a utility class for making HTTP POST requests to external APIs. Its static method,
     make_api_call, constructs the API endpoint URL and sends a POST request with provided data and headers,
     including an API key for authorization. It abstracts away HTTP request complexity, leveraging the requests
     library, and offers a centralized interface for API interaction within applications.
     """
     @staticmethod
     def make_api_call(
         base_url: str,
         api_url: str,
         data: Dict[str, Any],
         header: str
     ) -> requests.Response:
-        actual_url = base_url + api_url
-        headers = {'x-api-key': header}
-        response = requests.post(
-            actual_url,
-            json = data,
-            headers=headers,
-        )
-        return response
+        try:
+            actual_url = base_url + api_url
+            headers = {'x-api-key': header}
+            response = requests.post(
+                actual_url,
+                json = data,
+                headers=headers,
+            )
+            response.raise_for_status()
+            return response
+        except requests.exceptions.RequestException as e:
+            logging.error(e)
+            raise e
```

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/constants/route_constants.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/constants/route_constants.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/error_manager.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/error_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,20 @@
                 "stackFrames": frames_info
             },
             "tags": extra_attributes.get('tags') if extra_attributes and extra_attributes.get('tags') is not None else None,
             "context": extra_attributes.get('context') if extra_attributes and extra_attributes.get('context') is not None else None,
             "reportedAt": datetime.now(timezone.utc).isoformat(),
         }
 
-        response = ApiService.make_api_call(
-            Vigil.instance_url,
-            RouteConstants.ERROR_MONITORING,
-            error_data,
-            Vigil.api_key
-        )
-
-        if response.ok:
+        try:
+            ApiService.make_api_call(
+                Vigil.instance_url,
+                RouteConstants.ERROR_MONITORING,
+                error_data,
+                Vigil.api_key
+            )
             logging.info('[Vigil] Exception record added successfully')
-        else:
-            logging.error(f'[Vigil] Error while creating exception log :: {response.text}')
+        except Exception as e:
+            logging.error(f"[Vigil] Error while creating exception log: {e}")
+            
 
 ErrorManager = ErrorMonitoring()
```

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/job_manager.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/job_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,10 +88,10 @@
                 Vigil.api_key
             )
             logging.info(f'[Vigil] Job event has been logged successfully for route: {route}')
             return f'[Vigil] Job event has been logged successfully for route: {route}'
         except Exception as e:
             error_message = f'[Vigil] Error while creating job record for route {route} :: {str(e)}'
             logging.error(error_message)
-            return error_message
+
 
 JobManager = JobMonitoring()
```

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/api_monitoring_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/exception_log_types.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/exception_log_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/job_monitoring_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_types/vigil_options_types.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_utils/api_monitoring_utils_django.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations/vigil/vigil_utils/common_utils.py` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations/vigil/vigil_utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/PKG-INFO` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxsenseinnovations.vigil
-Version: 1.0.2
+Version: 1.0.3
 Summary: Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability
 License: ISC
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: requests
 Requires-Dist: werkzeug
 Requires-Dist: django
```

### Comparing `foxsenseinnovations_vigil-1.0.2/foxsenseinnovations.vigil.egg-info/SOURCES.txt` & `foxsenseinnovations_vigil-1.0.3/foxsenseinnovations.vigil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foxsenseinnovations_vigil-1.0.2/setup.py` & `foxsenseinnovations_vigil-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='foxsenseinnovations.vigil',
-    version='1.0.2',
+    version='1.0.3',
     description='Official SDK for Vigil - A comprehensive solution for all your monitoring requirements, including exceptions, jobs, APIs, and website availability',
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     packages=find_packages(exclude=['foxsenseinnovations.vigil.flask']),
     install_requires=[
         'setuptools',
```

