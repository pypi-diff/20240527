# Comparing `tmp/aliyun-python-sdk-sls-1.1.1.tar.gz` & `tmp/aliyun-python-sdk-sls-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-sls-1.1.1.tar", last modified: Mon Nov 22 11:47:50 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-sls-1.1.2.tar", last modified: Mon May 27 08:47:05 2024, max compression
```

## Comparing `aliyun-python-sdk-sls-1.1.1.tar` & `aliyun-python-sdk-sls-1.1.2.tar`

### file list

```diff
@@ -1,50 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/
--rw-r--r--   0 root         (0) root         (0)      575 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2094 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/
--rw-r--r--   0 root         (0) root         (0)       21 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1506 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20180613/
--rw-r--r--   0 root         (0) root         (0)     2878 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20180613/AnalyzeProductLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1734 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20180613/DeleteLogResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20180613/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/
--rw-r--r--   0 root         (0) root         (0)     1774 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/AnalyzeAppLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2878 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/AnalyzeProductLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1812 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CheckResourceOrchestrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2074 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CreateAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     3284 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CreateImportIngestionJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     3272 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CreateIngestionJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1962 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CreateResourceOrchestrationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1570 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DeleteAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     1754 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DeleteImportIngestionJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1742 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DeleteIngestionJobRequest.py
--rw-r--r--   0 root         (0) root         (0)     1574 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DescribeAppRequest.py
--rw-r--r--   0 root         (0) root         (0)     1884 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DisableAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     2664 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/EnableAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     2610 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/GetAlertHistoriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1876 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/GetAlertRequest.py
--rw-r--r--   0 root         (0) root         (0)     1264 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/GetSlsServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1612 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/InitProjectAlertResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1718 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/InitUserAlertResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1266 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/OpenSlsServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1784 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/QuerySafServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1888 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SetAlertActionPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1738 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SetAlertCenterResourceByConsoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1720 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SetAlertCenterResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1546 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SyncAlertGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1538 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SyncAlertUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1896 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/UpdateAppRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2021-11-22 11:47:50.000000 aliyun-python-sdk-sls-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1477 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/AnalyzeAppLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/AnalyzeProductLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/CreateAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DataExpressionProcessRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DeleteAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DescribeAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DisableAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/EnableAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/GetAlertHistoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2167 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/GetAlertRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/GetSlsServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/InitProjectAlertResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/InitUserAlertResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/OpenSlsServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/SetAlertActionPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/SetAlertCenterResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/SyncAlertGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/SyncAlertUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/UpdateAppRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-27 08:47:05.000000 aliyun-python-sdk-sls-1.1.2/setup.py
```

### Comparing `aliyun-python-sdk-sls-1.1.1/LICENSE` & `aliyun-python-sdk-sls-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-sls-1.1.1/PKG-INFO` & `aliyun-python-sdk-sls-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-sls
-Version: 1.1.1
+Version: 1.1.2
 Summary: The sls module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-sls
```

### Comparing `aliyun-python-sdk-sls-1.1.1/README.rst` & `aliyun-python-sdk-sls-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/PKG-INFO` & `aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-sls
-Version: 1.1.1
+Version: 1.1.2
 Summary: The sls module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-sls
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyun_python_sdk_sls.egg-info/SOURCES.txt` & `aliyun-python-sdk-sls-1.1.2/aliyun_python_sdk_sls.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,37 +7,27 @@
 aliyun_python_sdk_sls.egg-info/SOURCES.txt
 aliyun_python_sdk_sls.egg-info/dependency_links.txt
 aliyun_python_sdk_sls.egg-info/requires.txt
 aliyun_python_sdk_sls.egg-info/top_level.txt
 aliyunsdksls/__init__.py
 aliyunsdksls/endpoint.py
 aliyunsdksls/request/__init__.py
-aliyunsdksls/request/v20180613/AnalyzeProductLogRequest.py
-aliyunsdksls/request/v20180613/DeleteLogResourceRequest.py
-aliyunsdksls/request/v20180613/__init__.py
 aliyunsdksls/request/v20191023/AnalyzeAppLogRequest.py
 aliyunsdksls/request/v20191023/AnalyzeProductLogRequest.py
-aliyunsdksls/request/v20191023/CheckResourceOrchestrationRequest.py
 aliyunsdksls/request/v20191023/CreateAppRequest.py
-aliyunsdksls/request/v20191023/CreateImportIngestionJobRequest.py
-aliyunsdksls/request/v20191023/CreateIngestionJobRequest.py
-aliyunsdksls/request/v20191023/CreateResourceOrchestrationRequest.py
+aliyunsdksls/request/v20191023/DataExpressionProcessRequest.py
 aliyunsdksls/request/v20191023/DeleteAppRequest.py
-aliyunsdksls/request/v20191023/DeleteImportIngestionJobRequest.py
-aliyunsdksls/request/v20191023/DeleteIngestionJobRequest.py
 aliyunsdksls/request/v20191023/DescribeAppRequest.py
 aliyunsdksls/request/v20191023/DisableAlertRequest.py
 aliyunsdksls/request/v20191023/EnableAlertRequest.py
 aliyunsdksls/request/v20191023/GetAlertHistoriesRequest.py
 aliyunsdksls/request/v20191023/GetAlertRequest.py
 aliyunsdksls/request/v20191023/GetSlsServiceRequest.py
 aliyunsdksls/request/v20191023/InitProjectAlertResourceRequest.py
 aliyunsdksls/request/v20191023/InitUserAlertResourceRequest.py
 aliyunsdksls/request/v20191023/OpenSlsServiceRequest.py
-aliyunsdksls/request/v20191023/QuerySafServiceRequest.py
 aliyunsdksls/request/v20191023/SetAlertActionPolicyRequest.py
-aliyunsdksls/request/v20191023/SetAlertCenterResourceByConsoleRequest.py
 aliyunsdksls/request/v20191023/SetAlertCenterResourceRequest.py
 aliyunsdksls/request/v20191023/SyncAlertGroupsRequest.py
 aliyunsdksls/request/v20191023/SyncAlertUsersRequest.py
 aliyunsdksls/request/v20191023/UpdateAppRequest.py
 aliyunsdksls/request/v20191023/__init__.py
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20180613/AnalyzeProductLogRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/AnalyzeProductLogRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,74 +19,75 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
 class AnalyzeProductLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2018-06-13', 'AnalyzeProductLog','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'AnalyzeProductLog','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Project(self):
+	def get_Project(self): # String
 		return self.get_query_params().get('Project')
 
-	def set_Project(self,Project):
-		self.add_query_param('Project',Project)
-
-	def get_CloudProduct(self):
+	def set_Project(self, Project):  # String
+		self.add_query_param('Project', Project)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_CloudProduct(self): # String
 		return self.get_query_params().get('CloudProduct')
 
-	def set_CloudProduct(self,CloudProduct):
-		self.add_query_param('CloudProduct',CloudProduct)
-
-	def get_ResourceQuota(self):
+	def set_CloudProduct(self, CloudProduct):  # String
+		self.add_query_param('CloudProduct', CloudProduct)
+	def get_ResourceQuota(self): # String
 		return self.get_query_params().get('ResourceQuota')
 
-	def set_ResourceQuota(self,ResourceQuota):
-		self.add_query_param('ResourceQuota',ResourceQuota)
-
-	def get_VariableMap(self):
+	def set_ResourceQuota(self, ResourceQuota):  # String
+		self.add_query_param('ResourceQuota', ResourceQuota)
+	def get_VariableMap(self): # String
 		return self.get_query_params().get('VariableMap')
 
-	def set_VariableMap(self,VariableMap):
-		self.add_query_param('VariableMap',VariableMap)
-
-	def get_TTL(self):
-		return self.get_query_params().get('TTL')
-
-	def set_TTL(self,TTL):
-		self.add_query_param('TTL',TTL)
-
-	def get_ClientIp(self):
+	def set_VariableMap(self, VariableMap):  # String
+		self.add_query_param('VariableMap', VariableMap)
+	def get_ClientIp(self): # String
 		return self.get_query_params().get('ClientIp')
 
-	def set_ClientIp(self,ClientIp):
-		self.add_query_param('ClientIp',ClientIp)
-
-	def get_Region(self):
-		return self.get_query_params().get('Region')
-
-	def set_Region(self,Region):
-		self.add_query_param('Region',Region)
-
-	def get_Lang(self):
+	def set_ClientIp(self, ClientIp):  # String
+		self.add_query_param('ClientIp', ClientIp)
+	def get_Lang(self): # String
 		return self.get_query_params().get('Lang')
 
-	def set_Lang(self,Lang):
-		self.add_query_param('Lang',Lang)
+	def set_Lang(self, Lang):  # String
+		self.add_query_param('Lang', Lang)
+	def get_Overwrite(self): # Boolean
+		return self.get_query_params().get('Overwrite')
 
-	def get_Logstore(self):
-		return self.get_query_params().get('Logstore')
+	def set_Overwrite(self, Overwrite):  # Boolean
+		self.add_query_param('Overwrite', Overwrite)
+	def get_TTL(self): # Integer
+		return self.get_query_params().get('TTL')
 
-	def set_Logstore(self,Logstore):
-		self.add_query_param('Logstore',Logstore)
+	def set_TTL(self, TTL):  # Integer
+		self.add_query_param('TTL', TTL)
+	def get_HotTTL(self): # Integer
+		return self.get_query_params().get('HotTTL')
+
+	def set_HotTTL(self, HotTTL):  # Integer
+		self.add_query_param('HotTTL', HotTTL)
+	def get_Region(self): # String
+		return self.get_query_params().get('Region')
 
-	def get_Overwrite(self):
-		return self.get_query_params().get('Overwrite')
+	def set_Region(self, Region):  # String
+		self.add_query_param('Region', Region)
+	def get_Logstore(self): # String
+		return self.get_query_params().get('Logstore')
 
-	def set_Overwrite(self,Overwrite):
-		self.add_query_param('Overwrite',Overwrite)
+	def set_Logstore(self, Logstore):  # String
+		self.add_query_param('Logstore', Logstore)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20180613/DeleteLogResourceRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/AnalyzeAppLogRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class DeleteLogResourceRequest(RpcRequest):
+class AnalyzeAppLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2018-06-13', 'DeleteLogResource','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'AnalyzeAppLog','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_AppType(self): # String
+		return self.get_query_params().get('AppType')
 
-	def get_Project(self):
-		return self.get_query_params().get('Project')
-
-	def set_Project(self,Project):
-		self.add_query_param('Project',Project)
-
-	def get_Region(self):
-		return self.get_query_params().get('Region')
-
-	def set_Region(self,Region):
-		self.add_query_param('Region',Region)
-
-	def get_Logstore(self):
-		return self.get_query_params().get('Logstore')
+	def set_AppType(self, AppType):  # String
+		self.add_query_param('AppType', AppType)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_VariableMap(self): # String
+		return self.get_query_params().get('VariableMap')
+
+	def set_VariableMap(self, VariableMap):  # String
+		self.add_query_param('VariableMap', VariableMap)
+	def get_DisplayName(self): # String
+		return self.get_query_params().get('DisplayName')
 
-	def set_Logstore(self,Logstore):
-		self.add_query_param('Logstore',Logstore)
+	def set_DisplayName(self, DisplayName):  # String
+		self.add_query_param('DisplayName', DisplayName)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/AnalyzeAppLogRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DescribeAppRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class AnalyzeAppLogRequest(RpcRequest):
+class DescribeAppRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'AnalyzeAppLog','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DescribeApp','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_AppType(self):
-		return self.get_query_params().get('AppType')
-
-	def set_AppType(self,AppType):
-		self.add_query_param('AppType',AppType)
-
-	def get_VariableMap(self):
-		return self.get_query_params().get('VariableMap')
-
-	def set_VariableMap(self,VariableMap):
-		self.add_query_param('VariableMap',VariableMap)
-
-	def get_DisplayName(self):
-		return self.get_query_params().get('DisplayName')
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_AppName(self): # String
+		return self.get_query_params().get('AppName')
+
+	def set_AppName(self, AppName):  # String
+		self.add_query_param('AppName', AppName)
+	def get_ClientIp(self): # String
+		return self.get_query_params().get('ClientIp')
 
-	def set_DisplayName(self,DisplayName):
-		self.add_query_param('DisplayName',DisplayName)
+	def set_ClientIp(self, ClientIp):  # String
+		self.add_query_param('ClientIp', ClientIp)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CheckResourceOrchestrationRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/InitProjectAlertResourceRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class CheckResourceOrchestrationRequest(RpcRequest):
+class InitProjectAlertResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'CheckResourceOrchestration','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'InitProjectAlertResource','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ProjectName(self): # String
+		return self.get_body_params().get('ProjectName')
 
-	def get_Language(self):
-		return self.get_query_params().get('Language')
-
-	def set_Language(self,Language):
-		self.add_query_param('Language',Language)
-
-	def get_OperationPolicy(self):
-		return self.get_query_params().get('OperationPolicy')
-
-	def set_OperationPolicy(self,OperationPolicy):
-		self.add_query_param('OperationPolicy',OperationPolicy)
-
-	def get_AssetsId(self):
-		return self.get_query_params().get('AssetsId')
+	def set_ProjectName(self, ProjectName):  # String
+		self.add_body_params('ProjectName', ProjectName)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Region(self): # String
+		return self.get_body_params().get('Region')
 
-	def set_AssetsId(self,AssetsId):
-		self.add_query_param('AssetsId',AssetsId)
+	def set_Region(self, Region):  # String
+		self.add_body_params('Region', Region)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CreateAppRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/CreateAppRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,43 +20,44 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
 class CreateAppRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'CreateApp','sls')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ClientToken(self):
+	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
-	def set_ClientToken(self,ClientToken):
-		self.add_query_param('ClientToken',ClientToken)
-
-	def get_AppName(self):
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_AppName(self): # String
 		return self.get_query_params().get('AppName')
 
-	def set_AppName(self,AppName):
-		self.add_query_param('AppName',AppName)
-
-	def get_DisplayName(self):
+	def set_AppName(self, AppName):  # String
+		self.add_query_param('AppName', AppName)
+	def get_DisplayName(self): # String
 		return self.get_query_params().get('DisplayName')
 
-	def set_DisplayName(self,DisplayName):
-		self.add_query_param('DisplayName',DisplayName)
-
-	def get_ClientIp(self):
+	def set_DisplayName(self, DisplayName):  # String
+		self.add_query_param('DisplayName', DisplayName)
+	def get_ClientIp(self): # String
 		return self.get_query_params().get('ClientIp')
 
-	def set_ClientIp(self,ClientIp):
-		self.add_query_param('ClientIp',ClientIp)
-
-	def get_Config(self):
+	def set_ClientIp(self, ClientIp):  # String
+		self.add_query_param('ClientIp', ClientIp)
+	def get_Config(self): # String
 		return self.get_body_params().get('Config')
 
-	def set_Config(self,Config):
-		self.add_body_params('Config', Config)
+	def set_Config(self, Config):  # String
+		self.add_body_params('Config', Config)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CreateIngestionJobRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/GetAlertHistoriesRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,89 +16,68 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class CreateIngestionJobRequest(RpcRequest):
+class GetAlertHistoriesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'CreateIngestionJob','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'GetAlertHistories','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Line(self): # Integer
+		return self.get_body_params().get('Line')
 
-	def get_Args(self):
-		return self.get_body_params().get('Args')
-
-	def set_Args(self,Args):
-		self.add_body_params('Args', Args)
-
-	def get_Image(self):
-		return self.get_body_params().get('Image')
-
-	def set_Image(self,Image):
-		self.add_body_params('Image', Image)
-
-	def get_EnvFromSecret(self):
-		return self.get_body_params().get('EnvFromSecret')
-
-	def set_EnvFromSecret(self,EnvFromSecret):
-		self.add_body_params('EnvFromSecret', EnvFromSecret)
-
-	def get_RestartPolicy(self):
-		return self.get_body_params().get('RestartPolicy')
-
-	def set_RestartPolicy(self,RestartPolicy):
-		self.add_body_params('RestartPolicy', RestartPolicy)
-
-	def get_Parallelism(self):
-		return self.get_body_params().get('Parallelism')
-
-	def set_Parallelism(self,Parallelism):
-		self.add_body_params('Parallelism', Parallelism)
-
-	def get_Namespace(self):
-		return self.get_body_params().get('Namespace')
-
-	def set_Namespace(self,Namespace):
-		self.add_body_params('Namespace', Namespace)
-
-	def get_Completions(self):
-		return self.get_body_params().get('Completions')
-
-	def set_Completions(self,Completions):
-		self.add_body_params('Completions', Completions)
-
-	def get_EnvVars(self):
-		return self.get_body_params().get('EnvVars')
-
-	def set_EnvVars(self,EnvVars):
-		self.add_body_params('EnvVars', EnvVars)
-
-	def get_ImagePullSecret(self):
-		return self.get_body_params().get('ImagePullSecret')
-
-	def set_ImagePullSecret(self,ImagePullSecret):
-		self.add_body_params('ImagePullSecret', ImagePullSecret)
-
-	def get_CallerId(self):
-		return self.get_body_params().get('CallerId')
-
-	def set_CallerId(self,CallerId):
-		self.add_body_params('CallerId', CallerId)
-
-	def get_Region(self):
+	def set_Line(self, Line):  # Integer
+		self.add_body_params('Line', Line)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_ToTs(self): # Integer
+		return self.get_body_params().get('ToTs')
+
+	def set_ToTs(self, ToTs):  # Integer
+		self.add_body_params('ToTs', ToTs)
+	def get_Endpoint(self): # String
+		return self.get_body_params().get('Endpoint')
+
+	def set_Endpoint(self, Endpoint):  # String
+		self.add_body_params('Endpoint', Endpoint)
+	def get_App(self): # String
+		return self.get_body_params().get('App')
+
+	def set_App(self, App):  # String
+		self.add_body_params('App', App)
+	def get_FromTs(self): # Integer
+		return self.get_body_params().get('FromTs')
+
+	def set_FromTs(self, FromTs):  # Integer
+		self.add_body_params('FromTs', FromTs)
+	def get_ProjectName(self): # String
+		return self.get_body_params().get('ProjectName')
+
+	def set_ProjectName(self, ProjectName):  # String
+		self.add_body_params('ProjectName', ProjectName)
+	def get_Offset(self): # Integer
+		return self.get_body_params().get('Offset')
+
+	def set_Offset(self, Offset):  # Integer
+		self.add_body_params('Offset', Offset)
+	def get_AlertId(self): # String
+		return self.get_body_params().get('AlertId')
+
+	def set_AlertId(self, AlertId):  # String
+		self.add_body_params('AlertId', AlertId)
+	def get_Region(self): # String
 		return self.get_body_params().get('Region')
 
-	def set_Region(self,Region):
+	def set_Region(self, Region):  # String
 		self.add_body_params('Region', Region)
-
-	def get_JobName(self):
-		return self.get_body_params().get('JobName')
-
-	def set_JobName(self,JobName):
-		self.add_body_params('JobName', JobName)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/CreateResourceOrchestrationRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/SetAlertActionPolicyRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,41 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class CreateResourceOrchestrationRequest(RpcRequest):
+class SetAlertActionPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'CreateResourceOrchestration','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'SetAlertActionPolicy','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_Language(self):
-		return self.get_query_params().get('Language')
-
-	def set_Language(self,Language):
-		self.add_query_param('Language',Language)
-
-	def get_OperationPolicy(self):
-		return self.get_query_params().get('OperationPolicy')
-
-	def set_OperationPolicy(self,OperationPolicy):
-		self.add_query_param('OperationPolicy',OperationPolicy)
-
-	def get_Tokens(self):
-		return self.get_query_params().get('Tokens')
-
-	def set_Tokens(self,Tokens):
-		self.add_query_param('Tokens',Tokens)
-
-	def get_AssetsId(self):
-		return self.get_query_params().get('AssetsId')
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_PolicyId(self): # String
+		return self.get_body_params().get('PolicyId')
+
+	def set_PolicyId(self, PolicyId):  # String
+		self.add_body_params('PolicyId', PolicyId)
+	def get_Policy(self): # String
+		return self.get_body_params().get('Policy')
+
+	def set_Policy(self, Policy):  # String
+		self.add_body_params('Policy', Policy)
+	def get_App(self): # String
+		return self.get_body_params().get('App')
+
+	def set_App(self, App):  # String
+		self.add_body_params('App', App)
+	def get_PolicyName(self): # String
+		return self.get_body_params().get('PolicyName')
 
-	def set_AssetsId(self,AssetsId):
-		self.add_query_param('AssetsId',AssetsId)
+	def set_PolicyName(self, PolicyName):  # String
+		self.add_body_params('PolicyName', PolicyName)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DeleteAppRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/OpenSlsServiceRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,29 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class DeleteAppRequest(RpcRequest):
+class OpenSlsServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DeleteApp','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'OpenSlsService','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_AppName(self):
-		return self.get_query_params().get('AppName')
-
-	def set_AppName(self,AppName):
-		self.add_query_param('AppName',AppName)
-
-	def get_ClientIp(self):
-		return self.get_query_params().get('ClientIp')
-
-	def set_ClientIp(self,ClientIp):
-		self.add_query_param('ClientIp',ClientIp)
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DeleteImportIngestionJobRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DataExpressionProcessRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class DeleteImportIngestionJobRequest(RpcRequest):
+class DataExpressionProcessRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DeleteImportIngestionJob','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DataExpressionProcess','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Method(self): # String
+		return self.get_query_params().get('Method')
 
-	def get_Namespace(self):
-		return self.get_body_params().get('Namespace')
-
-	def set_Namespace(self,Namespace):
-		self.add_body_params('Namespace', Namespace)
-
-	def get_Region(self):
-		return self.get_body_params().get('Region')
-
-	def set_Region(self,Region):
-		self.add_body_params('Region', Region)
-
-	def get_JobName(self):
-		return self.get_body_params().get('JobName')
+	def set_Method(self, Method):  # String
+		self.add_query_param('Method', Method)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Detail(self): # String
+		return self.get_query_params().get('Detail')
 
-	def set_JobName(self,JobName):
-		self.add_body_params('JobName', JobName)
+	def set_Detail(self, Detail):  # String
+		self.add_query_param('Detail', Detail)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DeleteIngestionJobRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/UpdateAppRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,35 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class DeleteIngestionJobRequest(RpcRequest):
+class UpdateAppRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DeleteIngestionJob','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'UpdateApp','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_Namespace(self):
-		return self.get_body_params().get('Namespace')
-
-	def set_Namespace(self,Namespace):
-		self.add_body_params('Namespace', Namespace)
-
-	def get_Region(self):
-		return self.get_body_params().get('Region')
-
-	def set_Region(self,Region):
-		self.add_body_params('Region', Region)
-
-	def get_JobName(self):
-		return self.get_body_params().get('JobName')
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_AppName(self): # String
+		return self.get_query_params().get('AppName')
+
+	def set_AppName(self, AppName):  # String
+		self.add_query_param('AppName', AppName)
+	def get_DisplayName(self): # String
+		return self.get_query_params().get('DisplayName')
+
+	def set_DisplayName(self, DisplayName):  # String
+		self.add_query_param('DisplayName', DisplayName)
+	def get_ClientIp(self): # String
+		return self.get_query_params().get('ClientIp')
+
+	def set_ClientIp(self, ClientIp):  # String
+		self.add_query_param('ClientIp', ClientIp)
+	def get_Config(self): # String
+		return self.get_body_params().get('Config')
 
-	def set_JobName(self,JobName):
-		self.add_body_params('JobName', JobName)
+	def set_Config(self, Config):  # String
+		self.add_body_params('Config', Config)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/DescribeAppRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/GetSlsServiceRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,29 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class DescribeAppRequest(RpcRequest):
+class GetSlsServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DescribeApp','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'GetSlsService','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_AppName(self):
-		return self.get_query_params().get('AppName')
-
-	def set_AppName(self,AppName):
-		self.add_query_param('AppName',AppName)
-
-	def get_ClientIp(self):
-		return self.get_query_params().get('ClientIp')
-
-	def set_ClientIp(self,ClientIp):
-		self.add_query_param('ClientIp',ClientIp)
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/EnableAlertRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/EnableAlertRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,67 +20,64 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
 class EnableAlertRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'EnableAlert','sls')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_Language(self):
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Language(self): # String
 		return self.get_body_params().get('Language')
 
-	def set_Language(self,Language):
+	def set_Language(self, Language):  # String
 		self.add_body_params('Language', Language)
-
-	def get_RuleVersion(self):
+	def get_RuleVersion(self): # String
 		return self.get_body_params().get('RuleVersion')
 
-	def set_RuleVersion(self,RuleVersion):
+	def set_RuleVersion(self, RuleVersion):  # String
 		self.add_body_params('RuleVersion', RuleVersion)
-
-	def get_Endpoint(self):
+	def get_Endpoint(self): # String
 		return self.get_body_params().get('Endpoint')
 
-	def set_Endpoint(self,Endpoint):
+	def set_Endpoint(self, Endpoint):  # String
 		self.add_body_params('Endpoint', Endpoint)
-
-	def get_Tokens(self):
+	def get_Tokens(self): # String
 		return self.get_body_params().get('Tokens')
 
-	def set_Tokens(self,Tokens):
+	def set_Tokens(self, Tokens):  # String
 		self.add_body_params('Tokens', Tokens)
-
-	def get_App(self):
+	def get_App(self): # String
 		return self.get_body_params().get('App')
 
-	def set_App(self,App):
+	def set_App(self, App):  # String
 		self.add_body_params('App', App)
-
-	def get_ProjectName(self):
+	def get_ProjectName(self): # String
 		return self.get_body_params().get('ProjectName')
 
-	def set_ProjectName(self,ProjectName):
+	def set_ProjectName(self, ProjectName):  # String
 		self.add_body_params('ProjectName', ProjectName)
-
-	def get_AlertId(self):
+	def get_AlertId(self): # String
 		return self.get_body_params().get('AlertId')
 
-	def set_AlertId(self,AlertId):
+	def set_AlertId(self, AlertId):  # String
 		self.add_body_params('AlertId', AlertId)
-
-	def get_RuleId(self):
+	def get_RuleId(self): # String
 		return self.get_body_params().get('RuleId')
 
-	def set_RuleId(self,RuleId):
+	def set_RuleId(self, RuleId):  # String
 		self.add_body_params('RuleId', RuleId)
-
-	def get_Region(self):
+	def get_Region(self): # String
 		return self.get_body_params().get('Region')
 
-	def set_Region(self,Region):
-		self.add_body_params('Region', Region)
+	def set_Region(self, Region):  # String
+		self.add_body_params('Region', Region)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/InitProjectAlertResourceRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DisableAlertRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,29 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class InitProjectAlertResourceRequest(RpcRequest):
+class DisableAlertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'InitProjectAlertResource','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DisableAlert','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_App(self): # String
+		return self.get_body_params().get('App')
 
-	def get_ProjectName(self):
+	def set_App(self, App):  # String
+		self.add_body_params('App', App)
+	def get_ProjectName(self): # String
 		return self.get_body_params().get('ProjectName')
 
-	def set_ProjectName(self,ProjectName):
+	def set_ProjectName(self, ProjectName):  # String
 		self.add_body_params('ProjectName', ProjectName)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Endpoint(self): # String
+		return self.get_body_params().get('Endpoint')
 
-	def get_Region(self):
-		return self.get_body_params().get('Region')
+	def set_Endpoint(self, Endpoint):  # String
+		self.add_body_params('Endpoint', Endpoint)
+	def get_AlertId(self): # String
+		return self.get_body_params().get('AlertId')
 
-	def set_Region(self,Region):
-		self.add_body_params('Region', Region)
+	def set_AlertId(self, AlertId):  # String
+		self.add_body_params('AlertId', AlertId)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/InitUserAlertResourceRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/SetAlertCenterResourceRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class InitUserAlertResourceRequest(RpcRequest):
+class SetAlertCenterResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'InitUserAlertResource','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'SetAlertCenterResource','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_App(self):
+	def get_App(self): # String
 		return self.get_body_params().get('App')
 
-	def set_App(self,App):
+	def set_App(self, App):  # String
 		self.add_body_params('App', App)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_Language(self):
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Language(self): # String
 		return self.get_body_params().get('Language')
 
-	def set_Language(self,Language):
+	def set_Language(self, Language):  # String
 		self.add_body_params('Language', Language)
-
-	def get_Region(self):
+	def get_Region(self): # String
 		return self.get_body_params().get('Region')
 
-	def set_Region(self,Region):
-		self.add_body_params('Region', Region)
+	def set_Region(self, Region):  # String
+		self.add_body_params('Region', Region)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/QuerySafServiceRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/GetAlertRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,35 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class QuerySafServiceRequest(RpcRequest):
+class GetAlertRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'QuerySafService','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'GetAlert','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_App(self): # String
+		return self.get_body_params().get('App')
 
-	def get_ParamType(self):
-		return self.get_query_params().get('ParamType')
-
-	def set_ParamType(self,ParamType):
-		self.add_query_param('ParamType',ParamType)
-
-	def get_ProjectName(self):
-		return self.get_query_params().get('ProjectName')
-
-	def set_ProjectName(self,ProjectName):
-		self.add_query_param('ProjectName',ProjectName)
-
-	def get_ParamValue(self):
-		return self.get_query_params().get('ParamValue')
+	def set_App(self, App):  # String
+		self.add_body_params('App', App)
+	def get_ProjectName(self): # String
+		return self.get_body_params().get('ProjectName')
+
+	def set_ProjectName(self, ProjectName):  # String
+		self.add_body_params('ProjectName', ProjectName)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Endpoint(self): # String
+		return self.get_body_params().get('Endpoint')
+
+	def set_Endpoint(self, Endpoint):  # String
+		self.add_body_params('Endpoint', Endpoint)
+	def get_AlertId(self): # String
+		return self.get_body_params().get('AlertId')
 
-	def set_ParamValue(self,ParamValue):
-		self.add_query_param('ParamValue',ParamValue)
+	def set_AlertId(self, AlertId):  # String
+		self.add_body_params('AlertId', AlertId)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SetAlertCenterResourceByConsoleRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/SyncAlertUsersRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class SetAlertCenterResourceByConsoleRequest(RpcRequest):
+class SyncAlertUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'SetAlertCenterResourceByConsole','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'SyncAlertUsers','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_App(self):
+	def get_App(self): # String
 		return self.get_body_params().get('App')
 
-	def set_App(self,App):
+	def set_App(self, App):  # String
 		self.add_body_params('App', App)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_Language(self):
-		return self.get_body_params().get('Language')
-
-	def set_Language(self,Language):
-		self.add_body_params('Language', Language)
-
-	def get_Region(self):
-		return self.get_body_params().get('Region')
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Users(self): # String
+		return self.get_body_params().get('Users')
 
-	def set_Region(self,Region):
-		self.add_body_params('Region', Region)
+	def set_Users(self, Users):  # String
+		self.add_body_params('Users', Users)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SetAlertCenterResourceRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/DeleteAppRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class SetAlertCenterResourceRequest(RpcRequest):
+class DeleteAppRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'SetAlertCenterResource','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'DeleteApp','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
 
-	def get_App(self):
-		return self.get_body_params().get('App')
-
-	def set_App(self,App):
-		self.add_body_params('App', App)
-
-	def get_Language(self):
-		return self.get_body_params().get('Language')
-
-	def set_Language(self,Language):
-		self.add_body_params('Language', Language)
-
-	def get_Region(self):
-		return self.get_body_params().get('Region')
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_AppName(self): # String
+		return self.get_query_params().get('AppName')
+
+	def set_AppName(self, AppName):  # String
+		self.add_query_param('AppName', AppName)
+	def get_ClientIp(self): # String
+		return self.get_query_params().get('ClientIp')
 
-	def set_Region(self,Region):
-		self.add_body_params('Region', Region)
+	def set_ClientIp(self, ClientIp):  # String
+		self.add_query_param('ClientIp', ClientIp)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/aliyunsdksls/request/v20191023/SyncAlertUsersRequest.py` & `aliyun-python-sdk-sls-1.1.2/aliyunsdksls/request/v20191023/InitUserAlertResourceRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,29 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdksls.endpoint import endpoint_data
 
-class SyncAlertUsersRequest(RpcRequest):
+class InitUserAlertResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'SyncAlertUsers','sls')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Sls', '2019-10-23', 'InitUserAlertResource','sls')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_App(self):
+	def get_App(self): # String
 		return self.get_body_params().get('App')
 
-	def set_App(self,App):
+	def set_App(self, App):  # String
 		self.add_body_params('App', App)
+	def get_SlsAccessToken(self): # String
+		return self.get_query_params().get('SlsAccessToken')
+
+	def set_SlsAccessToken(self, SlsAccessToken):  # String
+		self.add_query_param('SlsAccessToken', SlsAccessToken)
+	def get_Language(self): # String
+		return self.get_body_params().get('Language')
 
-	def get_Users(self):
-		return self.get_body_params().get('Users')
+	def set_Language(self, Language):  # String
+		self.add_body_params('Language', Language)
+	def get_Region(self): # String
+		return self.get_body_params().get('Region')
 
-	def set_Users(self,Users):
-		self.add_body_params('Users', Users)
+	def set_Region(self, Region):  # String
+		self.add_body_params('Region', Region)
```

### Comparing `aliyun-python-sdk-sls-1.1.1/setup.py` & `aliyun-python-sdk-sls-1.1.2/setup.py`

 * *Files identical despite different names*

