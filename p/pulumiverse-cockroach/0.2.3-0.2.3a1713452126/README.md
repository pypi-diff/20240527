# Comparing `tmp/pulumiverse_cockroach-0.2.3.tar.gz` & `tmp/pulumiverse_cockroach-0.2.3a1713452126.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_cockroach-0.2.3.tar", last modified: Mon May 27 09:45:53 2024, max compression
+gzip compressed data, was "pulumiverse_cockroach-0.2.3a1713452126.tar", last modified: Thu Apr 18 14:58:41 2024, max compression
```

## Comparing `pulumiverse_cockroach-0.2.3.tar` & `pulumiverse_cockroach-0.2.3a1713452126.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:53.260993 pulumiverse_cockroach-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-27 09:45:53.260993 pulumiverse_cockroach-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:53.256993 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/api_oidc_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/ca_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/cmek.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:53.260993 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/finalize_version_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_cluster_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_cockroach_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_connection_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_person_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26512 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/log_export_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/metric_export_cloudwatch_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/metric_export_datadog_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44018 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/private_endpoint_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/private_endpoint_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/private_endpoint_trusted_owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/user_role_grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/version_deferral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:45:53.260993 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-27 09:45:53.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-27 09:45:53.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:45:53.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:45:53.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 09:45:53.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 09:45:53.000000 pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:45:53.260993 pulumiverse_cockroach-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-27 09:45:52.000000 pulumiverse_cockroach-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/api_oidc_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/ca_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13069 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cmek.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/finalize_version_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cluster_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cockroach_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_connection_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_person_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26512 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/log_export_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_cloudwatch_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12006 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_datadog_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44018 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_trusted_owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/user_role_grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/version_deferral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 14:58:41.000000 pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:58:41.179000 pulumiverse_cockroach-0.2.3a1713452126/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 14:58:40.000000 pulumiverse_cockroach-0.2.3a1713452126/setup.py
```

### Comparing `pulumiverse_cockroach-0.2.3/PKG-INFO` & `pulumiverse_cockroach-0.2.3a1713452126/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_cockroach
-Version: 0.2.3
+Version: 0.2.3a1713452126
 Summary: A Pulumi package to create and managed Cockroach DB resources in Pulumi programs.
 Home-page: https://www.cockroachlabs.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-cockroach
 Keywords: pulumi cockroach pulumiverse
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_cockroach-0.2.3/README.md` & `pulumiverse_cockroach-0.2.3a1713452126/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/__init__.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/_inputs.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/_utilities.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/allow_list.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/allow_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/api_oidc_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/api_oidc_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/ca_cert.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/ca_cert.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/cluster.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/cmek.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/cmek.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/config/vars.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/database.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/finalize_version_upgrade.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/finalize_version_upgrade.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/folder.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/folder.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_cluster_cert.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cluster_cert.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_cockroach_cluster.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_cockroach_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_connection_string.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_connection_string.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_organization.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/get_person_user.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/get_person_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/log_export_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/log_export_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/maintenance_window.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/metric_export_cloudwatch_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_cloudwatch_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/metric_export_datadog_config.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/metric_export_datadog_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/outputs.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/private_endpoint_connection.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/private_endpoint_services.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/private_endpoint_trusted_owner.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/private_endpoint_trusted_owner.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/provider.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/sql_user.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/user_role_grants.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,214 +4,180 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['SqlUserArgs', 'SqlUser']
+__all__ = ['UserRoleGrantsArgs', 'UserRoleGrants']
 
 @pulumi.input_type
-class SqlUserArgs:
+class UserRoleGrantsArgs:
     def __init__(__self__, *,
-                 cluster_id: pulumi.Input[str],
-                 name: pulumi.Input[str],
-                 password: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a SqlUser resource.
-        :param pulumi.Input[str] name: SQL user name.
-        """
-        pulumi.set(__self__, "cluster_id", cluster_id)
-        pulumi.set(__self__, "name", name)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-
-    @property
-    @pulumi.getter(name="clusterId")
-    def cluster_id(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "cluster_id")
-
-    @cluster_id.setter
-    def cluster_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "cluster_id", value)
+                 roles: pulumi.Input[Sequence[pulumi.Input['UserRoleGrantsRoleArgs']]],
+                 user_id: pulumi.Input[str]):
+        """
+        The set of arguments for constructing a UserRoleGrants resource.
+        :param pulumi.Input[str] user_id: ID of the user to grant these roles to.
+        """
+        pulumi.set(__self__, "roles", roles)
+        pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        SQL user name.
-        """
-        return pulumi.get(self, "name")
+    def roles(self) -> pulumi.Input[Sequence[pulumi.Input['UserRoleGrantsRoleArgs']]]:
+        return pulumi.get(self, "roles")
 
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+    @roles.setter
+    def roles(self, value: pulumi.Input[Sequence[pulumi.Input['UserRoleGrantsRoleArgs']]]):
+        pulumi.set(self, "roles", value)
 
     @property
-    @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password")
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Input[str]:
+        """
+        ID of the user to grant these roles to.
+        """
+        return pulumi.get(self, "user_id")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
+    @user_id.setter
+    def user_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "user_id", value)
 
 
 @pulumi.input_type
-class _SqlUserState:
+class _UserRoleGrantsState:
     def __init__(__self__, *,
-                 cluster_id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering SqlUser resources.
-        :param pulumi.Input[str] name: SQL user name.
-        """
-        if cluster_id is not None:
-            pulumi.set(__self__, "cluster_id", cluster_id)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-
-    @property
-    @pulumi.getter(name="clusterId")
-    def cluster_id(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "cluster_id")
-
-    @cluster_id.setter
-    def cluster_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cluster_id", value)
+                 roles: Optional[pulumi.Input[Sequence[pulumi.Input['UserRoleGrantsRoleArgs']]]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering UserRoleGrants resources.
+        :param pulumi.Input[str] user_id: ID of the user to grant these roles to.
+        """
+        if roles is not None:
+            pulumi.set(__self__, "roles", roles)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        SQL user name.
-        """
-        return pulumi.get(self, "name")
+    def roles(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['UserRoleGrantsRoleArgs']]]]:
+        return pulumi.get(self, "roles")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @roles.setter
+    def roles(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['UserRoleGrantsRoleArgs']]]]):
+        pulumi.set(self, "roles", value)
 
     @property
-    @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password")
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the user to grant these roles to.
+        """
+        return pulumi.get(self, "user_id")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
 
 
-class SqlUser(pulumi.CustomResource):
+class UserRoleGrants(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cluster_id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
+                 roles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserRoleGrantsRoleArgs']]]]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        CockroachDB SQL user.
+        Role grants for a single user.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: SQL user name.
+        :param pulumi.Input[str] user_id: ID of the user to grant these roles to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: SqlUserArgs,
+                 args: UserRoleGrantsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        CockroachDB SQL user.
+        Role grants for a single user.
 
         :param str resource_name: The name of the resource.
-        :param SqlUserArgs args: The arguments to use to populate this resource's properties.
+        :param UserRoleGrantsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SqlUserArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserRoleGrantsArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cluster_id: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
+                 roles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserRoleGrantsRoleArgs']]]]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SqlUserArgs.__new__(SqlUserArgs)
+            __props__ = UserRoleGrantsArgs.__new__(UserRoleGrantsArgs)
 
-            if cluster_id is None and not opts.urn:
-                raise TypeError("Missing required property 'cluster_id'")
-            __props__.__dict__["cluster_id"] = cluster_id
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
-            __props__.__dict__["name"] = name
-            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(SqlUser, __self__).__init__(
-            'cockroach:index/sqlUser:SqlUser',
+            if roles is None and not opts.urn:
+                raise TypeError("Missing required property 'roles'")
+            __props__.__dict__["roles"] = roles
+            if user_id is None and not opts.urn:
+                raise TypeError("Missing required property 'user_id'")
+            __props__.__dict__["user_id"] = user_id
+        super(UserRoleGrants, __self__).__init__(
+            'cockroach:index/userRoleGrants:UserRoleGrants',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            cluster_id: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            password: Optional[pulumi.Input[str]] = None) -> 'SqlUser':
+            roles: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserRoleGrantsRoleArgs']]]]] = None,
+            user_id: Optional[pulumi.Input[str]] = None) -> 'UserRoleGrants':
         """
-        Get an existing SqlUser resource's state with the given name, id, and optional extra
+        Get an existing UserRoleGrants resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: SQL user name.
+        :param pulumi.Input[str] user_id: ID of the user to grant these roles to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _SqlUserState.__new__(_SqlUserState)
+        __props__ = _UserRoleGrantsState.__new__(_UserRoleGrantsState)
 
-        __props__.__dict__["cluster_id"] = cluster_id
-        __props__.__dict__["name"] = name
-        __props__.__dict__["password"] = password
-        return SqlUser(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["roles"] = roles
+        __props__.__dict__["user_id"] = user_id
+        return UserRoleGrants(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="clusterId")
-    def cluster_id(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "cluster_id")
+    @pulumi.getter
+    def roles(self) -> pulumi.Output[Sequence['outputs.UserRoleGrantsRole']]:
+        return pulumi.get(self, "roles")
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Output[str]:
         """
-        SQL user name.
+        ID of the user to grant these roles to.
         """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter
-    def password(self) -> pulumi.Output[Optional[str]]:
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "user_id")
```

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach/version_deferral.py` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach/version_deferral.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/PKG-INFO` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-cockroach
-Version: 0.2.3
+Version: 0.2.3a1713452126
 Summary: A Pulumi package to create and managed Cockroach DB resources in Pulumi programs.
 Home-page: https://www.cockroachlabs.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-cockroach
 Keywords: pulumi cockroach pulumiverse
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_cockroach-0.2.3/pulumiverse_cockroach.egg-info/SOURCES.txt` & `pulumiverse_cockroach-0.2.3a1713452126/pulumiverse_cockroach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_cockroach-0.2.3/setup.py` & `pulumiverse_cockroach-0.2.3a1713452126/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
+import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.2.3"
+VERSION = "0.2.3a1713452126"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "cockroach Pulumi Package - Development Version"
```

