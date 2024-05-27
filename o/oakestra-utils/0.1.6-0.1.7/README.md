# Comparing `tmp/oakestra_utils-0.1.6.tar.gz` & `tmp/oakestra_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oakestra_utils-0.1.6.tar", max compression
+gzip compressed data, was "oakestra_utils-0.1.7.tar", max compression
```

## Comparing `oakestra_utils-0.1.6.tar` & `oakestra_utils-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.6/oakestra_utils/__init__.py
--rw-r--r--   0        0        0     1042 2024-05-27 19:24:34.771957 oakestra_utils-0.1.6/oakestra_utils/types.py
--rw-r--r--   0        0        0      360 2024-05-27 19:24:48.483956 oakestra_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-05-26 16:17:24.143594 oakestra_utils-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 16:18:54.275596 oakestra_utils-0.1.7/oakestra_utils/__init__.py
+-rw-r--r--   0        0        0     1002 2024-05-27 19:31:41.475951 oakestra_utils-0.1.7/oakestra_utils/types.py
+-rw-r--r--   0        0        0      360 2024-05-27 19:31:55.895951 oakestra_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 oakestra_utils-0.1.7/PKG-INFO
```

### Comparing `oakestra_utils-0.1.6/oakestra_utils/types.py` & `oakestra_utils-0.1.7/oakestra_utils/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,10 +22,8 @@
     # Even stranger
     TARGET_CLUSTER_NOT_FOUND = "TargetClusterNotFound"
     TARGET_CLUSTER_NOT_ACTIVE = "TargetClusterNotActive"
     TARGET_CLUSTER_NO_CAPACITY = "TargetClusterNoCapacity"
     NO_ACTIVE_CLUSTER_WITH_CAPACITY = "NoActiveClusterWithCapacity"
     # DEV note: unsure if exist in non Node-Engine code - need to check
     CREATING = "CREATING"
-    DEAD = "DEAD"
-    FAILED = "FAILED"
     UNDEPLOYED = "UNDEPLOYED"
```

