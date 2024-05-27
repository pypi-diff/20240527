# Comparing `tmp/oakestra_utils-0.1.4.tar.gz` & `tmp/oakestra_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakestra_utils-0.1.4.tar", max compression
+gzip compressed data, was "oakestra_utils-0.1.5.tar", max compression
```

## Comparing `oakestra_utils-0.1.4.tar` & `oakestra_utils-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.4/oakestra_utils/__init__.py
--rw-r--r--   0        0        0      850 2024-05-27 18:24:46.736001 oakestra_utils-0.1.4/oakestra_utils/types.py
--rw-r--r--   0        0        0      360 2024-05-27 18:25:17.780001 oakestra_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.5/oakestra_utils/__init__.py
+-rw-r--r--   0        0        0      980 2024-05-27 19:18:30.271961 oakestra_utils-0.1.5/oakestra_utils/types.py
+-rw-r--r--   0        0        0      360 2024-05-27 19:18:53.171961 oakestra_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.5/PKG-INFO
```

### Comparing `oakestra_utils-0.1.4/oakestra_utils/types.py` & `oakestra_utils-0.1.5/oakestra_utils/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class ServiceStatus(CustomEnum):
     # DEV note: Exist for sure
     CLUSTER_SCHEDULED = "CLUSTER_SCHEDULED"
     NODE_SCHEDULED = "NODE_SCHEDULED"
     REQUESTED = "REQUESTED"
-    ACTIVE = "ACTIVE"
+    ACTIVE = "ACTIVE"  # TODO figure out strong difference between ACTIVE and RUNNING and rename
+    # if both are truly needed
+    RUNNING = "RUNNING"
     # Exist but unsure if it fits for service (i.e. other enum might be better)
     NO_WORKER_CAPACITY = "NO_WORKER_CAPACITY"
     # Even stranger
     TARGET_CLUSTER_NOT_FOUND = "TargetClusterNotFound"
     TARGET_CLUSTER_NOT_ACTIVE = "TargetClusterNotActive"
     TARGET_CLUSTER_NO_CAPACITY = "TargetClusterNoCapacity"
     NO_ACTIVE_CLUSTER_WITH_CAPACITY = "NoActiveClusterWithCapacity"
```

