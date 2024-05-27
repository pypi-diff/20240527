# Comparing `tmp/oakestra_utils-0.1.7.tar.gz` & `tmp/oakestra_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakestra_utils-0.1.7.tar", max compression
+gzip compressed data, was "oakestra_utils-0.1.8.tar", max compression
```

## Comparing `oakestra_utils-0.1.7.tar` & `oakestra_utils-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.7/oakestra_utils/__init__.py
--rw-r--r--   0        0        0     1002 2024-05-27 19:31:41.475951 oakestra_utils-0.1.7/oakestra_utils/types.py
--rw-r--r--   0        0        0      360 2024-05-27 19:31:55.895951 oakestra_utils-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.8/oakestra_utils/__init__.py
+-rw-r--r--   0        0        0     1084 2024-05-27 19:49:29.643938 oakestra_utils-0.1.8/oakestra_utils/types.py
+-rw-r--r--   0        0        0      360 2024-05-27 19:50:02.407937 oakestra_utils-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.8/PKG-INFO
```

### Comparing `oakestra_utils-0.1.7/oakestra_utils/types.py` & `oakestra_utils-0.1.8/oakestra_utils/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,24 @@
     # DEV note: Exist for sure
     CLUSTER_SCHEDULED = "CLUSTER_SCHEDULED"
     NODE_SCHEDULED = "NODE_SCHEDULED"
     REQUESTED = "REQUESTED"
     ACTIVE = "ACTIVE"  # TODO figure out strong difference between ACTIVE and RUNNING and rename
     # if both are truly needed
     RUNNING = "RUNNING"
+    COMPLETED = "COMPLETED"
     # Exist but unsure if it fits for service (i.e. other enum might be better)
     NO_WORKER_CAPACITY = "NO_WORKER_CAPACITY"
     FAILED = "FAILED"
     # failed vs dead?
     DEAD = "DEAD"
     # Even stranger
     TARGET_CLUSTER_NOT_FOUND = "TargetClusterNotFound"
     TARGET_CLUSTER_NOT_ACTIVE = "TargetClusterNotActive"
     TARGET_CLUSTER_NO_CAPACITY = "TargetClusterNoCapacity"
     NO_ACTIVE_CLUSTER_WITH_CAPACITY = "NoActiveClusterWithCapacity"
+    # Strangest
+    LEGACY_0 = "0"
+    LEGACY_1 = "1"
     # DEV note: unsure if exist in non Node-Engine code - need to check
     CREATING = "CREATING"
     UNDEPLOYED = "UNDEPLOYED"
```

