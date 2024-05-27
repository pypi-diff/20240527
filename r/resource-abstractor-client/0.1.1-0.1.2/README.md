# Comparing `tmp/resource_abstractor_client-0.1.1.tar.gz` & `tmp/resource_abstractor_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resource_abstractor_client-0.1.1.tar", max compression
+gzip compressed data, was "resource_abstractor_client-0.1.2.tar", max compression
```

## Comparing `resource_abstractor_client-0.1.1.tar` & `resource_abstractor_client-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-05-26 19:50:20.451580 resource_abstractor_client-0.1.1/README.md
--rw-r--r--   0        0        0      292 2024-05-27 18:00:47.548019 resource_abstractor_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 11:46:23.827924 resource_abstractor_client-0.1.1/resource_abstractor_client/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-17 11:46:23.827924 resource_abstractor_client-0.1.1/resource_abstractor_client/app_operations.py
--rw-r--r--   0        0        0      572 2024-05-26 17:53:04.055668 resource_abstractor_client-0.1.1/resource_abstractor_client/client_helper.py
--rw-r--r--   0        0        0     1048 2024-05-26 15:54:15.579567 resource_abstractor_client-0.1.1/resource_abstractor_client/cluster_operations.py
--rw-r--r--   0        0        0     1416 2024-05-27 17:58:17.764021 resource_abstractor_client-0.1.1/resource_abstractor_client/job_operations.py
--rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 resource_abstractor_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-05-26 19:50:20.451580 resource_abstractor_client-0.1.2/README.md
+-rw-r--r--   0        0        0      292 2024-05-27 18:13:48.792009 resource_abstractor_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 11:46:23.827924 resource_abstractor_client-0.1.2/resource_abstractor_client/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-17 11:46:23.827924 resource_abstractor_client-0.1.2/resource_abstractor_client/app_operations.py
+-rw-r--r--   0        0        0      572 2024-05-26 17:53:04.055668 resource_abstractor_client-0.1.2/resource_abstractor_client/client_helper.py
+-rw-r--r--   0        0        0     1048 2024-05-26 15:54:15.579567 resource_abstractor_client-0.1.2/resource_abstractor_client/cluster_operations.py
+-rw-r--r--   0        0        0     1354 2024-05-27 18:13:36.296010 resource_abstractor_client-0.1.2/resource_abstractor_client/job_operations.py
+-rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 resource_abstractor_client-0.1.2/PKG-INFO
```

### Comparing `resource_abstractor_client-0.1.1/resource_abstractor_client/app_operations.py` & `resource_abstractor_client-0.1.2/resource_abstractor_client/app_operations.py`

 * *Files identical despite different names*

### Comparing `resource_abstractor_client-0.1.1/resource_abstractor_client/client_helper.py` & `resource_abstractor_client-0.1.2/resource_abstractor_client/client_helper.py`

 * *Files identical despite different names*

### Comparing `resource_abstractor_client-0.1.1/resource_abstractor_client/cluster_operations.py` & `resource_abstractor_client-0.1.2/resource_abstractor_client/cluster_operations.py`

 * *Files identical despite different names*

### Comparing `resource_abstractor_client-0.1.1/resource_abstractor_client/job_operations.py` & `resource_abstractor_client-0.1.2/resource_abstractor_client/job_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,18 @@
 def update_job(job_id: str, data: dict) -> Optional[dict]:
     request_address = f"{JOBS_API}/{job_id}"
     return make_request(patch, request_address, json=data)
 
 
 def update_job_status(
     job_id: str,
-    # service_status: ServiceStatus,
-    service_status,
+    service_status: ServiceStatus,
     status_detail: str = None,
 ) -> Optional[dict]:
-    # data = {"status": service_status.value}
-    data = {"status": service_status}
+    data = {"status": service_status.value}
     if status_detail:
         data["status_detail"] = status_detail
 
     return update_job(job_id, data)
 
 
 def update_job_instance(job_id, instance_number, data):
```

