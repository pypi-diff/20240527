# Comparing `tmp/qoa4ml-0.1.9.tar.gz` & `tmp/qoa4ml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.1.9.tar", last modified: Thu Sep 14 11:20:47 2023, max compression
+gzip compressed data, was "qoa4ml-0.2.0.tar", last modified: Mon May 27 11:30:25 2024, max compression
```

## Comparing `qoa4ml-0.1.9.tar` & `qoa4ml-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,73 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-09-14 11:20:47.769168 qoa4ml-0.1.9/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.9/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.9/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.9/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)    10843 2023-09-14 11:20:47.768712 qoa4ml-0.1.9/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)    10010 2023-09-12 19:37:23.000000 qoa4ml-0.1.9/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        5 2023-09-14 11:20:11.000000 qoa4ml-0.1.9/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.9/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-09-14 11:20:47.761497 qoa4ml-0.1.9/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    15096 2023-09-12 19:13:04.000000 qoa4ml-0.1.9/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.9/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-09-14 11:20:47.763907 qoa4ml-0.1.9/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.9/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2262 2023-08-15 13:51:38.000000 qoa4ml-0.1.9/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-09-14 11:20:47.766626 qoa4ml-0.1.9/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.9/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2054 2023-08-15 13:48:36.000000 qoa4ml-0.1.9/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.9/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1753 2023-08-15 13:51:21.000000 qoa4ml-0.1.9/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.9/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.9/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-09-14 11:20:47.768021 qoa4ml-0.1.9/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.1.9/qoa4ml/probes/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6908 2023-09-12 18:35:25.000000 qoa4ml-0.1.9/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     5250 2023-08-15 14:39:19.000000 qoa4ml-0.1.9/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6105 2023-08-15 14:44:45.000000 qoa4ml-0.1.9/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    12459 2023-08-15 14:32:15.000000 qoa4ml-0.1.9/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-09-14 11:20:47.763375 qoa4ml-0.1.9/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    10843 2023-09-14 11:20:47.000000 qoa4ml-0.1.9/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      648 2023-09-14 11:20:47.000000 qoa4ml-0.1.9/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-09-14 11:20:47.000000 qoa4ml-0.1.9/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      230 2023-09-14 11:20:47.000000 qoa4ml-0.1.9/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-09-14 11:20:47.000000 qoa4ml-0.1.9/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      230 2023-08-15 13:35:14.000000 qoa4ml-0.1.9/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-09-14 11:20:47.769269 qoa4ml-0.1.9/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      688 2023-09-14 11:20:30.000000 qoa4ml-0.1.9/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.270036 qoa4ml-0.2.0/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      641 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.2.0/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.2.0/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11535 2024-05-27 11:30:25.269395 qoa4ml-0.2.0/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    10605 2024-05-27 07:40:24.000000 qoa4ml-0.2.0/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        6 2024-05-27 07:44:18.000000 qoa4ml-0.2.0/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       35 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/dev_requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      165 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/ml_requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      176 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.243837 qoa4ml-0.2.0/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      281 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.247326 qoa4ml-0.2.0/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.2.0/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2616 2024-05-27 08:06:35.000000 qoa4ml-0.2.0/qoa4ml/collector/amqp_collector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      129 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/collector/base_collector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      153 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/collector/host_object.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1126 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/collector/socket_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.247719 qoa4ml-0.2.0/qoa4ml/config/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2872 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/config/configs.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.250227 qoa4ml-0.2.0/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.2.0/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2590 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      143 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/connector/base_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1410 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2396 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2499 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1040 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/connector/socket_connector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.252087 qoa4ml-0.2.0/qoa4ml/lang/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      655 2024-05-27 11:09:59.000000 qoa4ml-0.2.0/qoa4ml/lang/common_models.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3535 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/lang/datamodel_enum.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2242 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/lang/ml_contract.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4161 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/metric.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4046 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/metric_mananger.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.252753 qoa4ml-0.2.0/qoa4ml/observability/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/observability/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.254985 qoa4ml-0.2.0/qoa4ml/observability/odop_obs/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/observability/odop_obs/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      673 2024-05-21 11:39:02.000000 qoa4ml-0.2.0/qoa4ml/observability/odop_obs/embedded_database.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1138 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/observability/odop_obs/exporter.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     8440 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/observability/odop_obs/node_aggregator.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.258578 qoa4ml-0.2.0/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-08-06 11:19:24.000000 qoa4ml-0.2.0/qoa4ml/probes/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7859 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6060 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2248 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/probes/probe.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3717 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/probes/process_monitoring_probe.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     3801 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/probes/system_monitoring_probe.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    14377 2024-05-27 11:28:12.000000 qoa4ml-0.2.0/qoa4ml/qoa_client.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.263060 qoa4ml-0.2.0/qoa4ml/reports/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/qoa4ml/reports/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      780 2024-05-27 11:09:59.000000 qoa4ml-0.2.0/qoa4ml/reports/abstract_report.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      770 2024-05-27 11:09:59.000000 qoa4ml-0.2.0/qoa4ml/reports/general_application_report.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1851 2024-05-27 11:09:59.000000 qoa4ml-0.2.0/qoa4ml/reports/ml_report_model.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      610 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/reports/resources_report_model.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    10220 2024-05-27 11:09:59.000000 qoa4ml-0.2.0/qoa4ml/reports/rohe_reports.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.267297 qoa4ml-0.2.0/qoa4ml/utils/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1528 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/utils/gpu_utils.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    55920 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/utils/pynvml_forked.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    17074 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/utils/qoa_utils.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      805 2024-05-27 07:29:49.000000 qoa4ml-0.2.0/qoa4ml/utils/repeated_timer.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.245219 qoa4ml-0.2.0/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11535 2024-05-27 11:30:25.000000 qoa4ml-0.2.0/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1645 2024-05-27 11:30:25.000000 qoa4ml-0.2.0/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2024-05-27 11:30:25.000000 qoa4ml-0.2.0/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      483 2024-05-27 11:30:25.000000 qoa4ml-0.2.0/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2024-05-27 11:30:25.000000 qoa4ml-0.2.0/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      291 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2024-05-27 11:30:25.270163 qoa4ml-0.2.0/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      788 2024-05-21 06:42:14.000000 qoa4ml-0.2.0/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.238775 qoa4ml-0.2.0/tests/
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2024-05-27 11:30:25.267894 qoa4ml-0.2.0/tests/test_reportv1/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     5484 2024-05-27 11:09:59.000000 qoa4ml-0.2.0/tests/test_reportv1/test.py
```

### Comparing `qoa4ml-0.1.9/CHANGELOG.txt` & `qoa4ml-0.2.0/CHANGELOG.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,8 +23,12 @@
 
 0.0.64 (15/03/2022)
 ---------------------
 Add metric and modify format of system/process reports
 
 0.0.72 (22/05/2023)
 ---------------------
-Refactor source code
+Refactor source code
+
+0.0.73 (19/04/2024)
+---------------------
+Add new ODOP observability module
```

### Comparing `qoa4ml-0.1.9/LICENCE.txt` & `qoa4ml-0.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.1.9/PKG-INFO` & `qoa4ml-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: ml
+Provides-Extra: dev
 License-File: LICENCE.txt
 
 # QoA4ML - Quality of Analytics for ML
 
 ## Source code
 https://github.com/rdsea/QoA4ML
 
@@ -24,19 +25,19 @@
 
 The `configuration` contains the information about the client and its configuration in form of dictionary
 
 Example: 
 ```python
 clientConf = { 
     "client":{
-        "client_id": "aaltosea1",
+        "user_id": "aaltosea1",
         "instance_name": "ML02",
         "stage_id": "ML",
         "method": "REST",
-        "application": "test",
+        "application_name": "test",
         "role": "ml"
     },
     "connector":{
         "amqp_connector":{
             "class": "amqp",
             "conf":{
                 "end_point": "localhost",
@@ -220,14 +221,20 @@
     - `send_data`: a function to send data to specified `routing_key`/`queue` with a corresponding key `corr_id` to trace back message.
 
 
 
 ## Utilities
 A module provide some frequently used functions and some function to directly collect system metrics.
 
+## Note
+- `eva_duplicate`, `eva_erronous`, `eva_missing`, and `detect_outlier` probes are using ydata-quality library, which is only available for Python 3.8
+- For using ML quality probes, you may need to install a few more dependencies, e.g., tensorflow and Pillow.
+- QoaClient uses AMQP protocol by default. To use MQTT, you may need to install `paho-mqtt`.
+- To monitor Docker stats, you need to install [docker](https://docker-py.readthedocs.io/en/stable/) python client. 
+- To connect with Prometheus, you need to install [prometheus-client](https://pypi.org/project/prometheus-client/)
 
 
 Change Log
 ======================
 
 0.0.13 (18/04/2022)
 ---------------------
@@ -253,7 +260,10 @@
 ---------------------
 Add metric and modify format of system/process reports
 
 0.0.72 (22/05/2023)
 ---------------------
 Refactor source code
 
+0.0.73 (19/04/2024)
+---------------------
+Add new ODOP observability module
```

### Comparing `qoa4ml-0.1.9/README.md` & `qoa4ml-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 The `configuration` contains the information about the client and its configuration in form of dictionary
 
 Example: 
 ```python
 clientConf = { 
     "client":{
-        "client_id": "aaltosea1",
+        "user_id": "aaltosea1",
         "instance_name": "ML02",
         "stage_id": "ML",
         "method": "REST",
-        "application": "test",
+        "application_name": "test",
         "role": "ml"
     },
     "connector":{
         "amqp_connector":{
             "class": "amqp",
             "conf":{
                 "end_point": "localhost",
@@ -209,7 +209,13 @@
     - `send_data`: a function to send data to specified `routing_key`/`queue` with a corresponding key `corr_id` to trace back message.
 
 
 
 ## Utilities
 A module provide some frequently used functions and some function to directly collect system metrics.
 
+## Note
+- `eva_duplicate`, `eva_erronous`, `eva_missing`, and `detect_outlier` probes are using ydata-quality library, which is only available for Python 3.8
+- For using ML quality probes, you may need to install a few more dependencies, e.g., tensorflow and Pillow.
+- QoaClient uses AMQP protocol by default. To use MQTT, you may need to install `paho-mqtt`.
+- To monitor Docker stats, you need to install [docker](https://docker-py.readthedocs.io/en/stable/) python client. 
+- To connect with Prometheus, you need to install [prometheus-client](https://pypi.org/project/prometheus-client/)
```

### Comparing `qoa4ml-0.1.9/qoa4ml/QoaClient.py` & `qoa4ml-0.2.0/qoa4ml/qoa_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,381 +1,410 @@
-from typing import List
-from .connector.amqp_connector import Amqp_Connector
-from .connector.mqtt_connector import Mqtt_Connector
-from .connector.prom_connector import Prom_Connector
-from .metric import Gauge, Counter, Summary, Histogram
-import json, uuid
+import copy
+import os
+import sys
 import threading
+import time
+import traceback
+import uuid
 from threading import Thread
-import time, uuid, requests
-from datetime import datetime
-import os, sys, traceback, copy
-from .utils import get_proc_cpu, get_proc_mem, load_config, qoaLogger, set_logger_level
-from .reports import QoaReport
-from .probes.dataquality import eva_duplicate, eva_erronous, eva_missing, eva_none, image_quality
-from .probes.mlquality import *
-
-headers = {
-    'Content-Type': 'application/json'
-}
+from typing import Any, Dict, Generic, List, Optional, Type, TypeVar, Union
+
+import requests
+from pydantic import create_model
+from qoa4ml.reports.rohe_reports import RoheReport
+
+from qoa4ml.reports.abstract_report import AbstractReport
+
+# from .connector.mqtt_connector import Mqtt_Connector
+from .config.configs import (
+    AMQPConnectorConfig,
+    ClientConfig,
+    ConnectorConfig,
+    MetricConfig,
+)
+from .connector.amqp_connector import Amqp_Connector
+from .connector.base_connector import BaseConnector
+from .lang.common_models import Metric
+from .lang.datamodel_enum import (
+    MetricNameEnum,
+    ReportTypeEnum,
+    ServiceAPIEnum,
+    ServiceMetricNameEnum,
+)
+from .probes.dataquality import (
+    eva_duplicate,
+    eva_erronous,
+    eva_missing,
+    eva_none,
+    image_quality,
+)
+from .utils.qoa_utils import (
+    get_proc_cpu,
+    get_proc_mem,
+    load_config,
+    qoaLogger,
+    set_logger_level,
+)
+
+headers = {"Content-Type": "application/json"}
+
+
+# NOTE: T must be a subtype of AbstractReport
+T = TypeVar("T", bound=AbstractReport)
+
 
-class QoaClient(object):
+class QoaClient(Generic[T]):
     # Init QoA Client
-    def __init__(self, config_dict:dict=None, config_path: str=None, registration_url: str=None, logging_level=2, config_format = 0):
-        """
-        The 'config_dict' contains the information about the client and its configuration in form of dictionary
-        Example: 
-        { 
-            "client":{
-                "client_id": "aaltosea4",
-                "instance_name": "ML02",
-                "stage_id": "ML",
-                "method": "REST",
-                "application": "test",
-                "role": "ml"
-            },
-            "connector":{
-                "amqp_connector":{
-                    "class": "amqp",
-                    "conf":{
-                        "end_point": "localhost",
-                        "exchange_name": "qoa4ml",
-                        "exchange_type": "topic",
-                        "out_routing_key": "qoa.report.ml"
-                    }
-                }
-            }
-        }
-        The 'connector' is the dictionary containing multiple connector configuration (amqp, mqtt, kafka)
-        If 'connector' is not define, developer must give 'registration_url'
-        The 'registration_url' specify the service where the client register for monitoring service. If it's set, the client register with the service and receive connector configuration
-        Example: "http://127.0.0.1:5001/registration"
-        """
+    def __init__(
+        self,
+        report_cls: Type[T]= RoheReport,
+        config_dict: Optional[ClientConfig] = None,
+        config_path: Optional[str] = None,
+        registration_url: Optional[str] = None,
+        logging_level=2,
+    ):
         set_logger_level(logging_level)
-        
-        if config_dict != None:
-            self.configuration = config_dict
 
-        if config_path != None:
-            self.configuration = load_config(config_path, config_format)
+        if config_dict is not None:
+            self.configuration = config_dict
 
-        self.clientConf = self.configuration["client"]
-        
-        self.metricList = {}
-        self.connectorList = {}
-        self.timerFlag = False
-        self.method = self.clientConf["method"]
-        self.stageID = self.clientConf["stage_id"]
-        self.procMonitorFlag = 0
-        self.inferenceFlag = False
-
-        self.instanceID  = os.environ.get('INSTANCE_ID')
-        if not self.instanceID:
-            print("INSTANCE_ID is not defined")
-            self.instanceID  = str(uuid.uuid4())
+        if config_path is not None:
+            self.configuration = ClientConfig(**load_config(config_path))
 
-        self.clientConf["instances_id"] = self.instanceID
-        self.qoaReport = QoaReport(self.clientConf)
+        self.client_config = self.configuration.client
+        # self.metric_manager = MetricManager()
+        self.connector_list: Dict[str, BaseConnector] = {}
+        self.timer_flag = False
+        self.functionality = self.client_config.functionality
+        self.stage_id = self.client_config.stage_id
+        self.process_monitor_flag = 0
+        self.inference_flag = False
+
+        self.instance_id = os.environ.get("INSTANCE_ID")
+        if self.instance_id is None:
+            qoaLogger.info("INSTANCE_ID is not defined, generating random uuid")
+            self.instance_id = uuid.uuid4()
+        else:
+            self.instance_id = uuid.UUID(self.instance_id)
 
-        if "connector" in self.configuration:
+        self.client_config.id = str(self.instance_id)
+        self.qoa_report = report_cls(self.client_config)
+        if self.configuration.connector:
             # init connectors offline if it's specified
-            connector_conf = self.configuration["connector"]
+            connector_conf = self.configuration.connector
             try:
-                for key in connector_conf:
-                    self.connectorList[key] = self.initConnector(connector_conf[key])
+                for connector in connector_conf:
+                    self.connector_list[connector.name] = self.init_connector(connector)
             except Exception as e:
-                qoaLogger.error(str("[ERROR] - Error {} when configuring connector in QoaClient: {}".format(type(e),e.__traceback__)))
-        elif (registration_url != None) or ("registration_url" in self.configuration):
+                qoaLogger.error(
+                    str(
+                        "[ERROR] - Error {} when configuring connector in QoaClient: {}".format(
+                            type(e), e.__traceback__
+                        )
+                    )
+                )
+        elif registration_url or self.configuration.registration_url:
             # init connectors using configuration received from monitoring service, if it's specified
             try:
-                if registration_url == None:
-                    registration_url = self.configuration["registration_url"]
-                registration_data = self.registration(registration_url)
+                if registration_url:
+                    registration_data = self.registration(registration_url)
+                else:
+                    # NOTE: logically true
+                    registration_data = self.registration(
+                        self.configuration.registration_url
+                    )
                 json_data = registration_data.json()
                 response = json_data["response"]
-                if isinstance (response,dict):
-                    connector_conf = response["connector"]
-                    for key in connector_conf:
-                        self.connectorList[key] = self.initConnector(connector_conf[key])
-                else: 
-                    qoaLogger.warning("Unable to register Qoa Client: connector configuration must be dictionary")
+                if isinstance(response, dict):
+                    connector_configs = response["connector"]
+                    if isinstance(connector_configs, dict):
+                        connector_config = ConnectorConfig(**connector_configs)
+                        self.connector_list[connector_config.name] = (
+                            self.init_connector(connector_config)
+                        )
+                    elif isinstance(connector_configs, list):
+                        for config in connector_configs:
+                            connector_config = ConnectorConfig(**config)
+                            self.connector_list[connector_config.name] = (
+                                self.init_connector(connector_config)
+                            )
+                else:
+                    qoaLogger.warning(
+                        "Unable to register Qoa Client: connector configuration must be dictionary"
+                    )
             except Exception as e:
-                qoaLogger.error(str("[ERROR] - Error {} when registering QoA client: {}".format(type(e),e.__traceback__)))
+                qoaLogger.error(
+                    str(
+                        "[ERROR] - Error {} when registering QoA client: {}".format(
+                            type(e), e.__traceback__
+                        )
+                    )
+                )
                 traceback.print_exception(*sys.exc_info())
-  
-        if not any(self.connectorList):
+
+        if not self.connector_list:
             qoaLogger.warning("No connector initiated")
             self.default_connector = None
         else:
             # Set default connector for sending monitoring data if not specify
-            self.default_connector = list(self.connectorList.keys())[0]
-        
+            self.default_connector = list(self.connector_list.keys())[0]
+
         # lock report to guarantee consistency
         self.lock = threading.Lock()
 
-
-    def registration(self, url):
+    def registration(self, url: str):
         # get connector configuration by registering with the monitoring service
-        return requests.request("POST", url, headers=headers, data=json.dumps(self.clientConf))
-        
+        return requests.request(
+            "POST", url, headers=headers, data=self.client_config.json()
+        )
 
-    def initConnector(self, configuration: dict):
+    def init_connector(self, configuration: ConnectorConfig) -> BaseConnector:
         # init connector from configuration
-        if configuration["class"] == "amqp":
-            return Amqp_Connector(configuration["conf"])
-        if configuration["class"] == "mqtt":
-            return Mqtt_Connector(configuration["conf"])
-
-    def addMetric(self, metric_conf: dict):
-        # Add multiple metrics 
-        for key in metric_conf:
-            self.metricList[key] = self.initMetric(key, metric_conf[key])
+        if (
+            configuration.connector_class == ServiceAPIEnum.amqp
+            and type(configuration.config) is AMQPConnectorConfig
+        ):
+            return Amqp_Connector(configuration.config)
+
+        # TODO: MQTT is both connector and collector
+        #
+        # if (
+        #    configuration.connector_class == ServiceAPIEnum.mqtt
+        #    and type(configuration.config) is MQTTConnectorConfig
+        # ):
+        #    return Mqtt_Connector(configuration.config)
+        raise RuntimeError("Connector config is not of correct type")
+
+    def add_metric(self, metric_configs: List[MetricConfig]):
+        # Add multiple metrics
+        # self.metric_manager.add_metric(metric_configs)
+        pass
 
-    def initMetric(self, name, configuration: dict):
+    def init_metric(self, configuration: MetricConfig):
         # init individual metrics
-        if configuration["class"] == "Gauge":
-            return Gauge(name, configuration["description"], configuration["default"],configuration["category"])
-        elif configuration["class"] == "Counter":
-            return Counter(name, configuration["description"], configuration["default"],configuration["category"])
-        elif configuration["class"] == "Summary":
-            return Summary(name, configuration["description"], configuration["default"],configuration["category"])
-        elif configuration["class"] == "Histogram":
-            return Histogram(name, configuration["description"], configuration["default"],configuration["category"])
-
-    def getClientConfig(self):
-        # TO DO:
-        return self.clientConf
+        # self.metric_manager.init_metric(configuration)
+        pass
 
+    def get_client_config(self):
+        # TODO: what to do exactly?
+        return self.client_config
 
-    def getMetric(self, key=None):
+    def get_metric(self, key: Optional[Union[List, str]] = None):
         # TO DO:
-        try:
-            if key == None:
-                # Get all metric
-                return self.metricList
-            elif isinstance(key, list):
-                # Get a list of metrics
-                return dict((k, self.metricList[k]) for k in key)
-            else: 
-                # Get a specific metric
-                return self.metricList[key]
-        except Exception as e:
-            qoaLogger.error(str("[ERROR] - Error {} when getting metric from QoA client: {}".format(type(e),e.__traceback__)))
-    
-    def resetMetric(self, key=None):
+        pass
+        # return self.metric_manager.get_metric(key)
+
+    def reset_metric(self, key: Optional[Union[List, str]] = None):
         # TO DO:
-        try:
-            if key == None:
-                for key in self.metricList:
-                    self.metricList[key].reset()
-            elif isinstance(key, list):
-                for k in key:
-                    self.metricList[k].reset()
-            else: 
-                return self.metricList[key].reset()
-        except Exception as e:
-            qoaLogger.error(str("[ERROR] - Error {} when reseting metric in QoA client: {}".format(type(e),e.__traceback__)))
-            
-    def setConfig(self, key, value):
+        pass
+        # self.metric_manager.reset_metric(key)
+
+    def set_config(self, key, value):
         # TO DO:
         try:
-            self.clientConf[key] = value
+            self.client_config.__setattr__(key, value)
         except Exception as e:
-            qoaLogger.error(str("[ERROR] - Error {} when setConfig in QoA client: {}".format(type(e),e.__traceback__)))
-
-
-    def observeMetric(self, metric_name, value, category=0, cl="Gauge", des="", def_val=-1):
-        if metric_name not in self.metricList:
-            metric_config = {}
-            metric_config["class"] = cl
-            metric_config["default"]= def_val
-            metric_config["description"]= des
-            metric_config["category"]= category
-            self.addMetric({metric_name:metric_config})
-        self.metricList[metric_name].set(value)
-        
-        self.qoaReport.observeMetric(metric=self.metricList[metric_name])
-
+            qoaLogger.error(
+                str(
+                    "[ERROR] - Error {} when setConfig in QoA client: {}".format(
+                        type(e), e.__traceback__
+                    )
+                )
+            )
+
+    def observe_metric(
+        self,
+        metric_name: MetricNameEnum,
+        value,
+        category: int = 0,
+        description: str = "",
+    ):
+        # self.metric_manager.observe_metric(
+        #     metric_name, value, category, metric_class, description, default_value
+        # )
+        # metric = self.metric_manager.metric_list[metric_name]
+        if category == 0:
+            self.qoa_report.observe_metric(
+                ReportTypeEnum.service,
+                self.stage_id,
+                Metric(
+                    metric_name=metric_name, records=[value], description=description
+                ),
+            )
+        elif category == 1:
+            self.qoa_report.observe_metric(
+                ReportTypeEnum.data,
+                self.stage_id,
+                Metric(
+                    metric_name=metric_name, records=[value], description=description
+                ),
+            )
 
     def timer(self):
-        if self.timerFlag == False:
-            self.timerFlag = True
+        if self.timer_flag is False:
+            self.timer_flag = True
             self.timerStart = time.time()
             return {}
         else:
-            self.timerFlag = False
-            responseTime = {"startTime":self.timerStart, "responseTime":time.time()-self.timerStart}
-            self.observeMetric("Response Time", responseTime, category=0)
+            self.timer_flag = False
+            responseTime = {
+                "startTime": self.timerStart,
+                "responseTime": time.time() - self.timerStart,
+            }
+            self.observe_metric(
+                ServiceMetricNameEnum.response_time, responseTime, category=0
+            )
             return responseTime
 
-
-    def importPReport(self, reports):
-        self.qoaReport.importPReport(reports)
+    def import_previous_report(self, reports: Union[Dict, List[Dict]]):
+        if isinstance(reports, list):
+            for report in reports:
+                self.qoa_report.process_previous_report(report)
+        else:
+            self.qoa_report.process_previous_report(reports)
 
     def __str__(self):
-        return str(self.clientConf) + '\n' + str(self.connectorList)
-
+        return self.client_config.model_dump_json() + "\n" + str(self.connector_list)
 
-    def process_report(self, interval:int, pid:int = None):
+    def process_report(self, interval: int, pid: Optional[int] = None):
         report = {}
-        while self.procMonitorFlag == 1:
+        while self.process_monitor_flag == 1:
             try:
                 report["proc_cpu_stats"] = get_proc_cpu()
             except Exception as e:
-                qoaLogger.error("Error {} in process cpu stat: {}".format(type(e),e.__traceback__))
+                qoaLogger.error(
+                    "Error {} in process cpu stat: {}".format(type(e), e.__traceback__)
+                )
                 traceback.print_exception(*sys.exc_info())
             try:
                 report["proc_mem_stats"] = get_proc_mem()
             except Exception as e:
-                qoaLogger.error("Error {} in process memory stat: {}".format(type(e),e.__traceback__))
+                qoaLogger.error(
+                    "Error {} in process memory stat: {}".format(
+                        type(e), e.__traceback__
+                    )
+                )
                 traceback.print_exception(*sys.exc_info())
             try:
-                self.report(report=report,submit=True)
+                self.report(report=report, submit=True)
             except Exception as e:
-                qoaLogger.error("Error {} in send process report: {}".format(type(e),e.__traceback__))
+                qoaLogger.error(
+                    "Error {} in send process report: {}".format(
+                        type(e), e.__traceback__
+                    )
+                )
                 traceback.print_exception(*sys.exc_info())
             time.sleep(interval)
 
-
-    def process_monitor_start(self, interval:int, pid:int = None):
-        if self.procMonitorFlag == 0:
-            if (pid == None):
+    def process_monitor_start(self, interval: int, pid: Optional[int] = None):
+        if self.process_monitor_flag == 0:
+            if pid is None:
                 pid = os.getpid()
-            self.procMonitorFlag = 1
+            self.process_monitor_flag = 1
             sub_thread = Thread(target=self.process_report, args=(interval, pid))
             sub_thread.start()
-        self.procMonitorFlag = 1
-        
+        self.process_monitor_flag = 1
 
     def process_monitor_stop(self):
-        self.procMonitorFlag = 2
-    
-    def asyn_report(self, report:dict, connectors:list=None):
-        body_mess = json.dumps(report)
+        self.process_monitor_flag = 2
+
+    def asyn_report(self, body_mess: str, connectors: Optional[list] = None):
         self.lock.acquire()
-        if connectors == None:
+        if connectors is None:
             # if connectors are not specify, use default
-            self.connectorList[self.default_connector].send_data(body_mess,str(uuid.uuid4()))
+            if self.default_connector:
+                self.connector_list[self.default_connector].send_report(
+                    body_mess, corr_id=str(uuid.uuid4())
+                )
+            else:
+                qoaLogger.error(
+                    "No default connector, please specify the connector to use"
+                )
         else:
             # iterate connector to send report
-            for connector in connectors:
-                print(connector)
+            # for connector in connectors:
+            # print(connector)
+            # Todo: send by multiple connector
+            pass
+
         self.lock.release()
 
-    def report(self, metrics:list=None, report: dict = None, connectors:list=None, submit=False,reset=True):
-        if (report == None):
-            report = self.qoaReport.generateReport(metrics, reset=reset)
+    def report(
+        self,
+        report: Optional[Dict] = None,
+        connectors: Optional[list] = None,
+        submit=False,
+        reset=True,
+    ):
+        if report is None:
+            return_report = self.qoa_report.generate_report(reset)
         else:
-            report["metadata"] = copy.deepcopy(self.clientConf)
-            report["metadata"]["timestamp"] = time.time()
+            UserDefinedReportModel = create_model(
+                "UserDefinedReportModel", metadata=(dict, ...), report=(dict, ...)
+            )
+            return_report = UserDefinedReportModel(
+                report=report, metadata=copy.deepcopy(self.client_config.__dict__)
+            )
 
+            return_report.metadata["timestamp"] = time.time()
         if submit:
-            if self.default_connector != None:
-                sub_thread = Thread(target=self.asyn_report, args=(report, connectors))
+            if self.default_connector is not None:
+                sub_thread = Thread(
+                    target=self.asyn_report,
+                    args=(return_report.model_dump_json(), connectors),
+                )
                 sub_thread.start()
             else:
                 qoaLogger.warning("No connector available")
-        return report
+        return return_report.model_dump()
 
-    def observeInferenceMetric(self, metric_name, value, new_inf=False, inference_id=None, dependency=None):
-        report = {}
-        
-        if new_inf:
-            infID = str(uuid.uuid4())
-        else:
-            if inference_id != None:
-                infID = inference_id
-            else:
-                if self.inferenceFlag == False:
-                    self.infID = str(uuid.uuid4())
-                    self.inferenceFlag = True
-                infID = self.infID
-        report[infID] = {}
-        report[infID]["instance_id"] = self.instanceID
-
-        report[infID][metric_name] = {}
-        report[infID][metric_name]["value"] = value
-        
-        self.qoaReport.observeInferenceMetric(report,dependency=dependency)
-        return infID
-    
-    def observeErronous(self, data, errors=None):
+    def observe_inference(
+        self,
+        inference_value,
+    ):
+        self.qoa_report.observe_inference(inference_value)
+
+    def observe_inference_metric(
+        self,
+        metric_name: MetricNameEnum,
+        value: Any,
+    ):
+        metric = Metric(metric_name=metric_name, records=[value])
+        self.qoa_report.observe_inference_metric(metric)
+
+    def observe_erronous(self, data, errors=None):
         results = eva_erronous(data, errors=errors)
-        if results != None:
+        if results is not None:
             for key in results:
-                self.observeMetric(key,results[key],1)
+                self.observe_metric(key, results[key], 1)
 
-    def observeDuplicate(self, data):
+    def observe_duplicate(self, data):
         results = eva_duplicate(data)
-        if results != None:
+        if results is not None:
             for key in results:
-                self.observeMetric(key,results[key],1)
-    
-    def observeMissing(self, data, null_count=True, correlations=False, predict=False, random_state=0):
-        results = eva_missing(data, null_count=null_count, correlations=correlations, predict=predict, random_state=random_state)
-        if results != None:
+                self.observe_metric(key, results[key], 1)
+
+    def observe_missing(
+        self, data, null_count=True, correlations=False, predict=False, random_state=0
+    ):
+        results = eva_missing(
+            data,
+            null_count=null_count,
+            correlations=correlations,
+            predict=predict,
+            random_state=random_state,
+        )
+        if results is not None:
             for key in results:
-                self.observeMetric(key,results[key],1)
-    
-    def observeImgQuality(self, image):
+                self.observe_metric(key, results[key], 1)
+
+    def observe_image_quality(self, image):
         results = image_quality(image)
-        if results != None:
+        if results is not None:
             for key in results:
-                self.observeMetric(key,results[key],1)
+                self.observe_metric(key, results[key], 1)
 
-    def observeNone(self, data):
+    def observe_none(self, data):
         results = eva_none(data)
-        if results != None:
+        if results is not None:
             for key in results:
-                self.observeMetric(key,results[key],1)
-
-
-        # self.qoaReport = QoA_Report()
-        # self.start_time = time.time()
-        # self.clientConf = client_conf
-        # self.metricList = {}
-        # self.connectorList = {}
-        # self.timerFlag = False
-        self.timer_start = 0
-        # self.method = client_conf["method"]
-        # self.stageID = client_conf["stage_id"]
-        # self.instanceID  = os.environ.get('INSTANCE_ID')
-        # if not self.instanceID:
-        #     print("INSTANCE_ID is not defined")
-        #     self.instanceID  = str(uuid.uuid4())
-        # self.procMonitorFlag = False
-        # Init all connectors in for loop 
-        # self.registration_flag = False
-        # try:
-        #     registration_data = self.registration(registration_url)
-        #     json_data = registration_data.json()
-        #     response = json_data["response"]
-            
-        #     if isinstance (response,dict):
-        #         self.registration_flag = True
-        #         connector_conf = response["connector"]
-
-        #         for key in connector_conf:
-        #             self.connectorList[key] = self.initConnector(connector_conf[key])
-        #     else: 
-        #         print("Unable to register Qoa Client")
-        # except Exception as e:
-        #     qoaLogger.error("Error {} when register QoA client: {}".format(type(e),e.__traceback__))
-        #     traceback.print_exception(*sys.exc_info())
-        
-
-        # Set default connector for sending monitoring data if not specify
-        # self.default_connector = list(self.connectorList.keys())[0]
-        # self.addMetric(metric_conf)
-        # self.lock = threading.Lock()
-
-
-    
-
-
-
-
-
-
-
-
-    
+                self.observe_metric(key, results[key], 1)
```

### Comparing `qoa4ml-0.1.9/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.2.0/qoa4ml/collector/amqp_collector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,76 @@
-import pika, json
-import sys, pathlib
-p_dir = pathlib.Path(__file__).parent.parent.absolute()
-sys.path.append(str(p_dir))
-from utils import qoaLogger
+import json
+from typing import Optional
 
-class Amqp_Collector(object):
+from qoa4ml.collector.base_collector import BaseCollector
+
+from ..config.configs import AMQPCollectorConfig
+from ..utils.qoa_utils import qoaLogger
+from .host_object import HostObject
+
+class Amqp_Collector(BaseCollector):
     # Init an amqp client handling the connection to amqp servier
-    def __init__(self, configuration:dict, host_object:object=None):
-        self.host_object = host_object  
-        self.exchange_name = configuration["exchange_name"]
-        self.exchange_type = configuration["exchange_type"]
-        self.in_routing_key = configuration["in_routing_key"]
+    def __init__(
+        self,
+        configuration: AMQPCollectorConfig,
+        host_object: Optional[HostObject] = None,
+    ):
+        if "pika" not in globals():
+            global pika
+            import pika
+        self.host_object = host_object
+        self.exchange_name = configuration.exchange_name
+        self.exchange_type = configuration.exchange_type
+        self.in_routing_key = configuration.in_routing_key
 
         # Connect to RabbitMQ host
-        if "amqps://" in configuration["end_point"]:
-            self.in_connection = pika.BlockingConnection(pika.URLParameters(configuration["end_point"]))
+        if "amqps://" in configuration.end_point:
+            self.in_connection = pika.BlockingConnection(
+                pika.URLParameters(configuration.end_point)
+            )
         else:
-            self.in_connection = pika.BlockingConnection(pika.ConnectionParameters(host=configuration["end_point"]))
-        
+            self.in_connection = pika.BlockingConnection(
+                pika.ConnectionParameters(host=configuration.end_point)
+            )
+
         # Create a channel
         self.in_channel = self.in_connection.channel()
-        
-        # Init an Exchange 
-        self.in_channel.exchange_declare(exchange=self.exchange_name, exchange_type=self.exchange_type)
-        
+
+        # Init an Exchange
+        self.in_channel.exchange_declare(
+            exchange=self.exchange_name, exchange_type=self.exchange_type
+        )
+
         # Declare a queue to receive prediction response
-        self.queue = self.in_channel.queue_declare(queue=configuration["in_queue"], exclusive=False)
+        self.queue = self.in_channel.queue_declare(
+            queue=configuration.in_queue, exclusive=False
+        )
         self.queue_name = self.queue.method.queue
         # Binding the exchange to the queue with specific routing
-        self.in_channel.queue_bind(exchange=self.exchange_name, queue=self.queue_name, routing_key=self.in_routing_key)
-        
+        self.in_channel.queue_bind(
+            exchange=self.exchange_name,
+            queue=self.queue_name,
+            routing_key=self.in_routing_key,
+        )
 
-        
     def on_request(self, ch, method, props, body):
         # Process the data on request: sending back to host object
-        if self.host_object != None:
+        if self.host_object is not None:
             self.host_object.message_processing(ch, method, props, body)
         else:
             mess = json.loads(str(body.decode("utf-8")))
-            qoaLogger.debug(mess)
+            qoaLogger.info(mess)
 
-    def start(self):
+    def start_collecting(self):
         # Start rabbit MQ
         self.in_channel.basic_qos(prefetch_count=1)
-        self.in_channel.basic_consume(queue=self.queue_name,on_message_callback=self.on_request,auto_ack=True)
+        self.in_channel.basic_consume(
+            queue=self.queue_name, on_message_callback=self.on_request, auto_ack=True
+        )
         self.in_channel.start_consuming()
 
     def stop(self):
         self.in_channel.stop_consuming()
         self.in_channel.close()
 
     def get_queue(self):
-        return self.queue.method.queue
+        return self.queue.method.queue
```

### Comparing `qoa4ml-0.1.9/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.2.0/qoa4ml/connector/mess_logging.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import threading
 import time
+
 import pandas as pd
+
+
 class Mess_Logging(object):
     def __init__(self, log_id, cap=500):
         column_names = ["id", "request", "response"]
-        self.log = pd.DataFrame(index=range(cap),columns=column_names)
+        self.log = pd.DataFrame(index=range(cap), columns=column_names)
         self.capacity = cap
         self.log_request_count = 0
         self.log_response_count = 0
         self.log_id = log_id
         self.condition = threading.Condition()
         self.save_flag = True
-    
+
     def log_request(self, data, uuid):
         with self.condition:
             self.log.loc[self.log_request_count] = [uuid, data, ""]
-            self.log_request_count = (self.log_request_count+1)%self.capacity
-            
+            self.log_request_count = (self.log_request_count + 1) % self.capacity
 
     def log_response(self, data, uuid):
         with self.condition:
             self.log.loc[self.log["id"] == uuid] = data
-            self.log_response_count = (self.log_response_count+1)%self.capacity
-            if (self.log_response_count == (self.capacity/2)):
-                self.save_to_file(0,self.capacity/2-1)
-            elif (self.log_response_count == (self.capacity-1)):
-                self.save_to_file(self.capacity/2,self.capacity-1)
+            self.log_response_count = (self.log_response_count + 1) % self.capacity
+            if self.log_response_count == (self.capacity / 2):
+                self.save_to_file(0, self.capacity / 2 - 1)
+            elif self.log_response_count == (self.capacity - 1):
+                self.save_to_file(self.capacity / 2, self.capacity - 1)
 
     def save_to_file(self, bot_lim, top_lim):
         print(self.log)
-        self.log.loc[bot_lim:top_lim,].to_csv("./log/log_{}_{}.csv".format(self.log_id,time.time()),index=False)
+        self.log.loc[bot_lim:top_lim,].to_csv(
+            "./log/log_{}_{}.csv".format(self.log_id, time.time()), index=False
+        )
 
-    def set_capacity(self,cap):
-        self.capacity = cap
+    def set_capacity(self, cap):
+        self.capacity = cap
```

### Comparing `qoa4ml-0.1.9/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.2.0/qoa4ml/connector/mqtt_connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,55 @@
-import paho.mqtt.client as mqtt
-import sys, pathlib
-p_dir = pathlib.Path(__file__).parent.parent.absolute()
-sys.path.append(str(p_dir))
-from utils import qoaLogger
+from typing import TYPE_CHECKING
 
-class Mqtt_Connector(object):
+import lazy_import
+
+from ..collector.host_object import HostObject
+from ..config.configs import MQTTConnectorConfig
+from ..utils.qoa_utils import qoaLogger
+from .base_connector import BaseConnector
+
+if TYPE_CHECKING:
+    import paho.mqtt.client as mqtt
+else:
+    mqtt = lazy_import.lazy_module("paho.mqtt")
+
+
+# TODO: this client handle both connector and collector
+class Mqtt_Connector(BaseConnector):
     # This class will handle all the mqtt connection for each client application
-    def __init__(self, host_object, queue_info, broker_info, client_id): 
-        # Init the host object to return message 
+    # FIX: what is host object?
+    def __init__(self, host_object: HostObject, configuration: MQTTConnectorConfig):
+        # from paho.mqtt.client import Client as MqttClient
+        # from paho.mqtt.enums import CallbackAPIVersion
+        # Init the host object to return message
         self.host_object = host_object
         # Init the send/receive queue
-        self.pub_queue = queue_info["in_queue"]
-        self.sub_queue = queue_info["out_queue"]
+        self.pub_queue = configuration.in_queue
+        self.sub_queue = configuration.out_queue
         # Create the mqtt client
-        self.client = mqtt.Client(client_id=client_id, clean_session=False, userdata=None, transport="tcp")
+        self.test = mqtt
+        self.client = mqtt.Client(
+            callback_api_version=mqtt.CallbackAPIVersion.VERSION2,
+            client_id=configuration.client_id,
+            clean_session=False,
+            userdata=None,
+            transport="tcp",
+        )
         # Set some functional method
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
         # Connect to mqtt broker
-        self.client.connect(broker_info["url"], broker_info["port"], broker_info["keepalive"])
-
+        self.client.connect(
+            configuration.broker_url,
+            configuration.broker_port,
+            configuration.broker_keepalive,
+        )
 
     def on_connect(self, client, userdata, flags, rc):
-        qoaLogger.debug("Connected with result code "+str(rc))
+        qoaLogger.debug("Connected with result code " + str(rc))
         # Subscribing in on_connect() means that if we lose the connection and
         # reconnect then subscriptions will be renewed.
         client.subscribe(self.sub_queue)
 
     def on_message(self, client, userdata, msg):
         # Pass the data to the host object
         self.host_object.message_processing(client, userdata, msg)
@@ -35,10 +58,10 @@
         # stop the connection
         self.client.disconnect()
 
     def start(self):
         # Start looking for data from broker
         self.client.loop_start()
 
-    def send_data(self, body_mess):
+    def send_data(self, body_message: str):
         # Send data in form of text message
-        self.client.publish(self.pub_queue, body_mess)
+        self.client.publish(self.pub_queue, body_message)
```

### Comparing `qoa4ml-0.1.9/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.2.0/qoa4ml/connector/prom_connector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,64 @@
-import prometheus_client as pr
 _INF = float("inf")
 
+
 class Prom_Connector(object):
-    def __init__(self,info):
+    def __init__(self, info):
+        if "pr" not in globals():
+            global pr
+            import prometheus_client as pr
+
         self.info = info["metric"]
         self.port = info["port"]
         self.metrices = {}
         for key in self.info:
             self.metrices[key] = {}
             if self.info[key]["Type"] == "Gauge":
-                self.metrices[key]["metric"] = pr.Gauge(self.info[key]["Prom_name"], self.info[key]["Description"])
+                self.metrices[key]["metric"] = pr.Gauge(
+                    self.info[key]["Prom_name"], self.info[key]["Description"]
+                )
             if self.info[key]["Type"] == "Counter":
-                self.metrices[key]["metric"] = pr.Counter(self.info[key]["Prom_name"], self.info[key]["Description"])
+                self.metrices[key]["metric"] = pr.Counter(
+                    self.info[key]["Prom_name"], self.info[key]["Description"]
+                )
             if self.info[key]["Type"] == "Summary":
-                self.metrices[key]["metric"] = pr.Summary(self.info[key]["Prom_name"], self.info[key]["Description"])
+                self.metrices[key]["metric"] = pr.Summary(
+                    self.info[key]["Prom_name"], self.info[key]["Description"]
+                )
             if self.info[key]["Type"] == "Histogram":
-                self.metrices[key]["metric"] = pr.Histogram(self.info[key]["Prom_name"], self.info[key]["Description"],buckets=(tuple(self.info[key]["Buckets"])))
-            self.metrices[key]["violation"] = pr.Counter(self.info[key]["Prom_name"]+"_violation", self.info[key]["Description"]+" (violation)")
+                self.metrices[key]["metric"] = pr.Histogram(
+                    self.info[key]["Prom_name"],
+                    self.info[key]["Description"],
+                    buckets=(tuple(self.info[key]["Buckets"])),
+                )
+            self.metrices[key]["violation"] = pr.Counter(
+                self.info[key]["Prom_name"] + "_violation",
+                self.info[key]["Description"] + " (violation)",
+            )
         pr.start_http_server(int(info["port"]))
 
     def inc(self, key, num=1):
-        if (self.info[key]["Type"] in ["Gauge", "Counter"]):
+        if self.info[key]["Type"] in ["Gauge", "Counter"]:
             self.metrices[key]["metric"].inc(num)
+
     def dec(self, key, num=1):
-        if (self.info[key]["Type"] == "Gauge"):
+        if self.info[key]["Type"] == "Gauge":
             self.metrices[key]["metric"].dec(num)
+
     def set(self, key, num=1):
-        if (self.info[key]["Type"] == "Gauge"):
+        if self.info[key]["Type"] == "Gauge":
             self.metrices[key]["metric"].set(num)
-        elif (self.info[key]["Type"] == "Counter"):
+        elif self.info[key]["Type"] == "Counter":
             self.metrices[key]["metric"].inc(num)
-        elif (self.info[key]["Type"] in ["Histogram","Summary"]):
+        elif self.info[key]["Type"] in ["Histogram", "Summary"]:
             self.metrices[key]["metric"].observe(num)
+
     def observe(self, key, val):
-        if (self.info[key]["Type"] in ["Summary", "Histogram"]):
+        if self.info[key]["Type"] in ["Summary", "Histogram"]:
             self.metrices[key]["metric"].observe(val)
+
     def inc_violation(self, key, num=1):
         self.metrices[key]["violation"].inc(num)
 
     def update_violation_count(self):
         for key in self.metrices:
-            pr.generate_latest(self.metrices[key]["violation"])
+            pr.generate_latest(self.metrices[key]["violation"])
```

### Comparing `qoa4ml-0.1.9/qoa4ml/metric.py` & `qoa4ml-0.2.0/qoa4ml/metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,147 @@
 # Metrics are implemented based on these classes to be compatible with Prometheus
-import numpy as np
+from .lang.datamodel_enum import MetricNameEnum
 
-class Metric(object):
+
+class PrometheusMetric(object):
     """
     This class defines the common attribute and provide basic function for handling a metric
-    - Attribute: 
+    - Attribute:
         - name: name of the metric
         - description: describe the metric
         - value: value of the metric
         - category: group metric into specific category supporting building QoA_Report
         - others: (Developing)
 
-    - Function: 
+    - Function:
         - set: set specific value
         - get_val: return current value
         - get_name: return metric name
         - get_des: return metric description
         - other: (Developing)
 
     - Category: metrics are categorized into following groups
         0 - Quality: Performance (metrics for evaluating service performance e.g., response time, throughput)
         1 - Quality: Data (metrics for evaluating data quality e.g., missing, duplicate, erroneous)
         2 - Quality: Inference (metrics for evaluating quality of ML inference, measured from inferences e.g., accuracy, confidence)
         3 - Resource: metrics for evaluating resource utilization e.g. CPU, Memory
         Other: To do (extend more categories)
     """
-    def __init__(self, metric_name, description, default_value=-1, category=0):
+
+    def __init__(
+        self, metric_name: MetricNameEnum, description, default_value=-1, category=0
+    ):
         self.name = metric_name
         self.description = description
         self.default_value = default_value
         self.value = default_value
         self.category = category
-    
+
     def set(self, value):
         self.value = value
+
     def get_val(self):
         return self.value
+
     def get_name(self):
         return self.name
+
     def get_des(self):
         return self.description
+
     def get_category(self):
         return self.category
 
     def reset(self):
         self.value = self.default_value
+
     def __str__(self) -> str:
         return "metric_name: " + self.name + ", " + "value: " + str(self.value)
+
     def to_dict(self):
         mectric_dict = {}
         mectric_dict[self.name] = self.value
         return mectric_dict
 
-class Counter(Metric):
+
+class Counter(PrometheusMetric):
     """
     This class inherit all attributes of Metric
     - Attribute: (Developing)
 
-    - Function: 
+    - Function:
         - inc: increase its value by num
         - reset: set the value back to zero
         - others: (Developing)
     """
+
     def __init__(self, metric_name, description, default_value=0, category=0):
         super().__init__(metric_name, description, default_value, category)
 
-    def inc(self,num=1):
+    def inc(self, num=1):
         self.value += num
 
-class Gauge(Metric):
+
+class Gauge(PrometheusMetric):
     """
     This class inherit all attributes of Metric
     - Attribute: (Developing)
 
-    - Function: 
+    - Function:
         - inc: increase its value by num
         - others: (Developing)
     """
+
     def __init__(self, metric_name, description, default_value=-1, category=0):
         super().__init__(metric_name, description, default_value, category)
 
-    def inc(self,num=1):
+    def inc(self, num=1):
         self.value += num
+
     # TO DO:
     # implement other functions
-    def dec(self,num=1):
+    def dec(self, num=1):
         self.value -= num
-    def set(self,val):
-        self.value = val
 
-class Summary(Metric):
+
+class Summary(PrometheusMetric):
     """
     This class inherit all attributes of Metric
     - Attribute: (Developing)
 
-    - Function: 
+    - Function:
         - inc: increase its value by num
         - others: (Developing)
     """
+
     def __init__(self, metric_name, description, default_value=-1, category=0):
         super().__init__(metric_name, description, default_value, category)
 
-    def inc(self,num):
+    def inc(self, num):
         self.value += num
+
     # TO DO:
     # implement other functions
-    def dec(self,num):
+    def dec(self, num):
         self.value -= num
-    def set(self,val):
-        self.value = val
 
-class Histogram(Metric):
+
+class Histogram(PrometheusMetric):
     """
     This class inherit all attributes of Metric
     - Attribute: (Developing)
 
-    - Function: 
+    - Function:
         - inc: increase its value by num
         - others: (Developing)
     """
+
     def __init__(self, metric_name, description, default_value=-1, category=0):
         super().__init__(metric_name, description, default_value, category)
 
-    def inc(self,num):
+    def inc(self, num):
         self.value += num
+
     # TO DO:
     # implement other functions
-    def dec(self,num):
+    def dec(self, num):
         self.value -= num
-    def set(self,val):
-        self.value = val
-
```

### Comparing `qoa4ml-0.1.9/qoa4ml/probes/dataquality.py` & `qoa4ml-0.2.0/qoa4ml/probes/dataquality.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,171 +1,206 @@
 # This library is built based on ydata_quality: https://github.com/ydataai/ydata-quality
-import pandas as pd 
+
+import io
+import pathlib
+import sys
+import traceback
+
 import numpy as np
-import traceback, sys, pathlib
-from ydata_quality.erroneous_data import ErroneousDataIdentifier
-from ydata_quality.missings import MissingsProfiler
-from ydata_quality.labelling import LabelInspector
-from ydata_quality.duplicates import DuplicateChecker
-from PIL import Image
-import PIL, io
+import pandas as pd
+
+from ..lang.datamodel_enum import ImageQualityNameEnum
+from ..utils.qoa_utils import is_numpyarray, is_pddataframe, qoaLogger
+
 p_dir = pathlib.Path(__file__).parent.parent.absolute()
 sys.path.append(str(p_dir))
-from utils import qoaLogger, is_numpyarray, is_pddataframe
 
 # Define metric names, return formats: dictionary {metric name} {sub-element}
 # Return error/debugging
 ################################################ DATA QUALITY ########################################################
 
 
-
-
 def eva_erronous(data, errors=None):
     """
     Return number/percentage of error data
     data: numpy array or pandas data frame
     errors: list of item considered as error
     ratio: return percentage if set to True
     sum: sum the result if set to True, otherwise return errors following the categories in list of 'errors'
     """
     try:
+        if "ErroneousDataIdentifier" not in globals():
+            global ErroneousDataIdentifier
+            from ydata_quality.erroneous_data import ErroneousDataIdentifier
         if is_numpyarray(data):
             data = pd.DataFrame(data)
         if is_pddataframe(data):
             if errors and isinstance(errors, list):
-                eva_err =  ErroneousDataIdentifier(df=data,ed_extensions=errors) 
+                eva_err = ErroneousDataIdentifier(df=data, ed_extensions=errors)
             else:
-                eva_err = ErroneousDataIdentifier(df=data) 
+                eva_err = ErroneousDataIdentifier(df=data)
             error_df = eva_err.predefined_erroneous_data()
-            
+
             total_count = data.count().to_numpy().flatten().sum()
             results = {}
             results["totalErrors"] = error_df.to_numpy().flatten().sum()
-            results["errorRatio"] = 100*error_df/total_count
+            results["errorRatio"] = 100 * error_df / total_count
             return results
         else:
             qoaLogger.warning("Unsupported data: {}".format(type(data)))
             return None
     except Exception as e:
-        qoaLogger.error("Error {} in eva_erronous: {}".format(type(e),e.__traceback__))
+        qoaLogger.error("Error {} in eva_erronous: {}".format(type(e), e.__traceback__))
         traceback.print_exception(*sys.exc_info())
 
+
 def eva_duplicate(data):
     """
     Return data/percentage of duplicate
     data: numpy array or pandas data frame
     ratio: return percentage if set to True
     """
     try:
+        if "DuplicateChecker" not in globals():
+            global DuplicateChecker
+            from ydata_quality.duplicates import DuplicateChecker
         if is_numpyarray(data):
             data = pd.DataFrame(data)
         if is_pddataframe(data):
             dc = DuplicateChecker(df=data)
             dcEva = dc.exact_duplicates()
             results = {}
-            results["duplicateRatio"] = 100*len(dcEva.index)/len(data.index)
+            results["duplicateRatio"] = 100 * len(dcEva.index) / len(data.index)
             results["totalDuplicate"] = len(dcEva.index)
             return results
         else:
             qoaLogger.warning("Unsupported data: {}".format(type(data)))
             return None
     except Exception as e:
-        qoaLogger.error("Error {} in eva_duplicate: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} in eva_duplicate: {}".format(type(e), e.__traceback__)
+        )
         traceback.print_exception(*sys.exc_info())
 
-def eva_missing(data, null_count=True, correlations=False, predict=False, random_state=0):
+
+def eva_missing(
+    data, null_count=True, correlations=False, predict=False, random_state=0
+):
     try:
+        if "MissingsProfiler" not in globals():
+            global MissingsProfiler
+            from ydata_quality.missings import MissingsProfiler
         if is_numpyarray(data):
             data = pd.DataFrame(data)
         if is_pddataframe(data):
             mp = MissingsProfiler(df=data, random_state=random_state)
-            results ={}
+            results = {}
             if null_count:
                 results["nullCount"] = mp.null_count()
             if correlations:
                 results["correlations"] = mp.missing_correlations()
             if predict:
-                results["missingPrediction"]= mp.predict_missings()
+                results["missingPrediction"] = mp.predict_missings()
             return results
         else:
             qoaLogger.warning("Unsupported data: {}".format(type(data)))
             return None
     except Exception as e:
-        qoaLogger.error("Error {} in eva_erronous: {}".format(type(e),e.__traceback__))
+        qoaLogger.error("Error {} in eva_erronous: {}".format(type(e), e.__traceback__))
         traceback.print_exception(*sys.exc_info())
 
+
 class Outlier_Detector(object):
     def __init__(self, data):
         self.data = None
         self.update_data(data)
-    
+
     def detect_outlier(self, n_data, labels=[], random_state=0, n=10, cluster=False):
         if is_numpyarray(n_data):
             n_data = pd.DataFrame(n_data)
         if is_pddataframe(n_data):
             if self.data is not None:
                 data = None
                 try:
-                    data = pd.concat([self.data,n_data])
+                    data = pd.concat([self.data, n_data])
                 except Exception as e:
-                    qoaLogger.error("Error {} in concatenating data: {}".format(type(e),e.__traceback__))
+                    qoaLogger.error(
+                        "Error {} in concatenating data: {}".format(
+                            type(e), e.__traceback__
+                        )
+                    )
                     traceback.print_exception(*sys.exc_info())
                 if data is not None:
                     results = {}
                     for label in labels:
                         try:
-                            li = LabelInspector(df=data, label=label, random_state=random_state)
-                            results[label] = li.outlier_detection(th=n,use_clusters=cluster)
+                            if "LabelInspector" not in globals():
+                                global LabelInspector
+                                from ydata_quality.labelling import LabelInspector
+                            li = LabelInspector(
+                                df=data, label=label, random_state=random_state
+                            )
+                            results[label] = li.outlier_detection(
+                                th=n, use_clusters=cluster
+                            )
                         except Exception as e:
-                            qoaLogger.error("Error {} in LabelInspector: {}".format(type(e),e.__traceback__))
+                            qoaLogger.error(
+                                "Error {} in LabelInspector: {}".format(
+                                    type(e), e.__traceback__
+                                )
+                            )
                             traceback.print_exception(*sys.exc_info())
                     return results
-                else: 
+                else:
                     return {"Error": "Cannot concatenate data"}
             else:
                 return {"Error": "Historical data has not been set"}
         else:
-            return {"Error":  "Unsupported data: {}".format(type(data))}
-    
+            return {"Error": "Unsupported data: {}".format(type(data))}
+
     def update_data(self, data):
         if is_numpyarray(data):
             data = pd.DataFrame(data)
         if is_pddataframe(data):
             self.data = data
-            return {"Response":  "Success"}
+            return {"Response": "Success"}
         else:
-            return {"Error":  "Unsupported data: {}".format(type(data))}
+            return {"Error": "Unsupported data: {}".format(type(data))}
 
 
 def image_quality(image):
+    if "PIL" not in globals():
+        global PIL
+        import PIL
     quality = {}
-    if isinstance(image,bytes):
-        image = Image.open(io.BytesIO(image))
-    if isinstance(image,np.ndarray):
-        image = Image.fromarray(image)
-    if isinstance(image,PIL.JpegImagePlugin.JpegImageFile) or isinstance(image,PIL.Image.Image):
+    if isinstance(image, bytes):
+        image = PIL.Image.open(io.BytesIO(image))
+    if isinstance(image, np.ndarray):
+        image = PIL.Image.fromarray(image)
+    if isinstance(image, PIL.JpegImagePlugin.JpegImageFile) or isinstance(
+        image, PIL.Image.Image
+    ):
         # qoaLogger.debug(dir(image)
-        quality["Image Width"] = image.width
-        quality["Image Height"] = image.height
-        quality["Image Size"] = image.size
-        quality["Color Mode"] = image.mode
-        quality["Color Channel"] = len(image.getbands())
+        quality[ImageQualityNameEnum.image_size] = image.size
+        quality[ImageQualityNameEnum.color_mode] = image.mode
+        quality[ImageQualityNameEnum.color_channel] = len(image.getbands())
     return quality
 
+
 def eva_none(data):
     try:
         if is_pddataframe(data):
             data = data.to_numpy()
         if is_numpyarray(data):
             valid_count = np.count_nonzero(~np.isnan(data))
             none_count = np.count_nonzero(np.isnan(data))
             results = {}
             results["totalValid"] = valid_count
             results["totalNone"] = none_count
-            results["noneRatio"] = valid_count/(valid_count+none_count)
+            results["noneRatio"] = valid_count / (valid_count + none_count)
             return results
         else:
             qoaLogger.warning("Unsupported data: {}".format(type(data)))
             return None
     except Exception as e:
-        qoaLogger.error("Error {} in eva_none: {}".format(type(e),e.__traceback__))
+        qoaLogger.error("Error {} in eva_none: {}".format(type(e), e.__traceback__))
         traceback.print_exception(*sys.exc_info())
```

### Comparing `qoa4ml-0.1.9/qoa4ml/probes/mlquality.py` & `qoa4ml-0.2.0/qoa4ml/probes/mlquality.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,136 +1,196 @@
 # This library is built based on ydata_quality: https://github.com/ydataai/ydata-quality
-import pandas as pd 
+
+import pathlib
+import sys
+import traceback
+
 import numpy as np
-import traceback, sys, pathlib
+
+from ..qoa_utils import is_numpyarray, qoaLogger
+
 p_dir = pathlib.Path(__file__).parent.parent.absolute()
 sys.path.append(str(p_dir))
-from utils import is_numpyarray, qoaLogger
-
-try:
-    import tensorflow as tf
-except Exception as e:
-    qoaLogger.error("Error {} when importing TensorFlow: {}".format(type(e),e.__traceback__))
-    traceback.print_exception(*sys.exc_info())
 
 
 ################################################ ML QUALITY ########################################################
+def import_tf():
+    if "tf" not in globals():
+        global tf
+        try:
+            import tensorflow as tf
+        except Exception as e:
+            qoaLogger.error(
+                "Error {} when importing TensorFlow: {}".format(
+                    type(e), e.__traceback__
+                )
+            )
+            traceback.print_exception(*sys.exc_info())
+
 
 def timeseries_metric(model):
     metrics = {}
     try:
+        import_tf()
         if isinstance(model, tf.keras.Sequential):
             for metric in model.metrics:
                 metrics[metric.name] = metric.result().numpy()
         return metrics
     except Exception as e:
-        qoaLogger.error("Error {} when querying timeseries model metrics: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying timeseries model metrics: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get metrics"}
 
-def ts_inference_metric(model,name):
+
+def ts_inference_metric(model, name):
     try:
         metrics = timeseries_metric(model)
         results = {}
         if name in metrics:
             results[name] = metrics[name]
         if "Error" in metrics:
             results["Error"] = metrics["Error"]
         return results
     except Exception as e:
-        qoaLogger.error("Error {} when querying timeseries {}: {}".format(type(e),name,e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying timeseries {}: {}".format(
+                type(e), name, e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get model {}".format(name)}
-    
+
+
 def ts_inference_MAE(model):
     try:
         metrics = ts_inference_metric(model, "mean_absolute_error")
-        return {"MAE":metrics}
+        return {"MAE": metrics}
     except Exception as e:
-        qoaLogger.error("Error {} when querying timeseries mean absolute error: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying timeseries mean absolute error: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get model mean absolute error"}
-    
+
+
 def ts_inference_loss(model):
     try:
         metrics = ts_inference_metric(model, "loss")
-        return {"Loss":metrics}
+        return {"Loss": metrics}
     except Exception as e:
-        qoaLogger.error("Error {} when querying timeseries mean absolute error: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying timeseries mean absolute error: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get model mean absolute error"}
-    
+
 
 def training_metric(model):
     try:
+        import_tf()
         if isinstance(model, tf.keras.Sequential):
             return model.history.history
         else:
             return None
     except Exception as e:
-        qoaLogger.error("Error {} when querying training metrics: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying training metrics: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get training metrics"}
-    
+
+
 def training_loss(model):
     try:
+        import_tf()
         if isinstance(model, tf.keras.Sequential):
-            return {"Training Loss":model.history.history["loss"]}
+            return {"Training Loss": model.history.history["loss"]}
         else:
             return None
     except Exception as e:
-        qoaLogger.error("Error {} when querying training loss: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying training loss: {}".format(type(e), e.__traceback__)
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get training loss"}
-    
+
+
 def training_val_accuracy(model):
     try:
+        import_tf()
         if isinstance(model, tf.keras.Sequential):
-            return {"Evaluate Accuracy":model.history.history["val_accuracy"]}
+            return {"Evaluate Accuracy": model.history.history["val_accuracy"]}
         else:
             return None
     except Exception as e:
-        qoaLogger.error("Error {} when querying training validation accuracy: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying training validation accuracy: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get validation accuracy"}
 
+
 def training_accuracy(model):
     try:
+        import_tf()
         if isinstance(model, tf.keras.Sequential):
             return {"Train Accuracy": model.history.history["accuracy"]}
         else:
             return None
     except Exception as e:
-        qoaLogger.error("Error {} when querying training accuracy: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying training accuracy: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get accuracy"}
-    
+
+
 def training_val_loss(model):
     try:
+        import_tf()
         if isinstance(model, tf.keras.Sequential):
-            return {"Evaluate Loss":model.history.history["val_loss"]}
+            return {"Evaluate Loss": model.history.history["val_loss"]}
         else:
             return None
     except Exception as e:
-        qoaLogger.error("Error {} when querying training validation loss: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} when querying training validation loss: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get validation loss"}
 
+
 def classification_confidence(data, score=True):
     try:
         if score:
             return {"Confidence": 100 * np.max(data)}
         else:
             if is_numpyarray(data):
+                import_tf()
                 scores = tf.nn.softmax(data[0])
-                return {"Confidence":100 * np.max(scores)}
+                return {"Confidence": 100 * np.max(scores)}
             else:
                 return {"Error": "Unsupported data: {}".format(type(data))}
     except Exception as e:
-        qoaLogger.error("Error {} in extracting classification confidence: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} in extracting classification confidence: {}".format(
+                type(e), e.__traceback__
+            )
+        )
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get classification confidence"}
-
-
-
-
-
```

### Comparing `qoa4ml-0.1.9/qoa4ml/utils.py` & `qoa4ml-0.2.0/qoa4ml/utils/qoa_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,184 +1,281 @@
-from concurrent.futures import thread
-from email.policy import default
-import json, psutil, time, os, docker, yaml, logging
-from threading import Thread
-import traceback,sys, pathlib
-import numpy as np
-import pandas as pd
+import glob
+import json
 import logging
+import os
+import pathlib
+import re
+import shlex
+import subprocess
+import sys
+import time
+import traceback
+from threading import Thread
 
-logging.basicConfig(format='%(asctime)s:%(levelname)s -- %(message)s', level=logging.INFO)
+import psutil
+import yaml
+
+logging.basicConfig(
+    format="%(asctime)s:%(levelname)s -- %(message)s", level=logging.INFO
+)
 
 qoaLogger = logging.getLogger()
 
+
+def make_folder(temp_path):
+    try:
+        if os.path.exists(temp_path):
+            pass
+        else:
+            os.makedirs(temp_path)
+        return True
+    except Exception:
+        return False
+
+
+def get_cgroup_version() -> str:
+    proc1 = subprocess.Popen("mount", stdout=subprocess.PIPE)
+    proc2 = subprocess.Popen(
+        shlex.split("grep cgroup"),
+        stdin=proc1.stdout,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+    )
+    if proc1.stdout:
+        proc1.stdout.close()
+    out, _ = proc2.communicate()
+    if "cgroup2" in out.decode():
+        return "v2"
+    return "v1"
+
+
+if get_cgroup_version() == "v2":
+    CGROUP_VERSION = "v2"
+else:
+    CGROUP_VERSION = "v1"
+
+
 def set_logger_level(logging_level):
     if logging_level == 0:
         log_level = logging.NOTSET
     elif logging_level == 1:
         log_level = logging.DEBUG
     elif logging_level == 2:
         log_level = logging.INFO
     elif logging_level == 3:
         log_level = logging.WARNING
     elif logging_level == 4:
         log_level = logging.ERROR
     elif logging_level == 5:
         log_level = logging.CRITICAL
+    else:
+        raise ValueError(f"Error logging level {logging_level}")
     qoaLogger.setLevel(log_level)
 
+
 ###################### DEFAULT METRIC ######################
 default_docker_metric = {
-    "dock_cpu_percentage":{
+    "dock_cpu_percentage": {
         "class": "Gauge",
         "description": "monitor system cpu percentage",
         "default": -1,
-        "key": "percentage"
+        "key": "percentage",
     },
     "docker_memory_used": {
         "class": "Gauge",
         "description": "monitor system memory used",
-        "default": - 0,
-        "key": "used"
-    }
+        "default": -0,
+        "key": "used",
+    },
 }
 
 
 ###################### COMMON USED FUNCTION ######################
-def load_config(file_path:str, format=0)->dict:
+def load_config(file_path: str) -> dict:
     """
     file_path: file path to load config
-    format:
-        0 - json
-        1 - yaml
-        other - To Do
+
     """
     try:
-        if format == 0:
+        if "json" in file_path:
             with open(file_path, "r") as f:
                 return json.load(f)
-        elif format == 1:
-            with open('file_path', 'r') as f:
+        if ("yaml" in file_path) or ("yml" in file_path):
+            with open(file_path, "r") as f:
                 return yaml.safe_load(f)
         else:
             qoaLogger.warning("Unsupported format")
             return None
-    except Exception as e:
+    except Exception:
         qoaLogger.error("Unable to load configuration")
 
-def to_json(file_path:str, conf:dict):
+    return None
+
+
+def to_json(file_path: str, conf: dict):
     """
     file_path: file path to save config
     """
     with open(file_path, "w") as f:
         json.dump(conf, f)
 
-def to_yaml(file_path:str, conf:dict):
+
+def to_yaml(file_path: str, conf: dict):
     """
     file_path: file path to save config
     """
     with open(file_path, "w") as f:
         yaml.dump(conf, f)
-    
+
+
 def get_sys_cpu():
     stats = psutil.cpu_stats()
     cpu_time = psutil.cpu_times()
     info = {}
     for key in stats._fields:
-        info[key] = getattr(stats,key)
+        info[key] = getattr(stats, key)
     for key in cpu_time._fields:
-        info[key] = getattr(cpu_time,key)
+        info[key] = getattr(cpu_time, key)
+    return info
+
+
+def get_sys_cpu_util():
+    info = {}
+    core_utils = psutil.cpu_percent(percpu=True)
+    for core_num, core_util in enumerate(core_utils):
+        info[f"core_{core_num}"] = core_util
     return info
 
+
+def get_sys_cpu_metadata():
+    cpu_freq = psutil.cpu_freq()
+    frequency = {"value": cpu_freq.max / 1000, "unit": "GHz"}
+    cpu_threads = psutil.cpu_count(logical=True)
+    return {"frequency": frequency, "thread": cpu_threads}
+
+
 def get_sys_mem():
     stats = psutil.virtual_memory()
     info = {}
     for key in stats._fields:
-        info[key] = getattr(stats,key)
+        info[key] = getattr(stats, key)
     return info
 
+
 def get_sys_net():
     info = {}
     net = psutil.net_io_counters()
     for key in net._fields:
-        info[key] = getattr(net,key)
+        info[key] = getattr(net, key)
     return info
 
+
 def report_proc_cpu(process):
     report = {}
     cpu_time = process.cpu_times()
     contex = process.num_ctx_switches()
     for key in cpu_time._fields:
-        report[key] = getattr(cpu_time,key)
+        report[key] = getattr(cpu_time, key)
     for key in contex._fields:
-        report[key] = getattr(contex,key)
-    report['num_thread'] = process.num_threads()
+        report[key] = getattr(contex, key)
+    report["num_thread"] = process.num_threads()
 
     return report
-    
-def get_proc_cpu(pid = None):
-    if (pid == None):
+
+
+def report_proc_child_cpu(process: psutil.Process):
+    # WARNING: this children function takes a lot of time
+    child_processes = process.children(recursive=True)
+    child_processes_count = len(child_processes)
+    child_processes_cpu = {}
+    process_cpu_time = process.cpu_times()
+    for id, child_proc in enumerate(child_processes):
+        cpu_time = child_proc.cpu_times()
+        child_processes_cpu[f"child_{id}"] = float(cpu_time.user + cpu_time.system)
+
+    total_cpu_usage = sum(child_processes_cpu.values())
+    total_cpu_usage += float(process_cpu_time.user + process_cpu_time.system)
+    return {
+        "child_process": child_processes_count,
+        "value": child_processes_cpu,
+        "total": total_cpu_usage,
+        "unit": "cputime",
+    }
+
+
+def get_proc_cpu(pid=None):
+    if pid is None:
         pid = os.getpid()
     process = psutil.Process(pid)
     child_list = process.children()
     info = {}
     info[pid] = report_proc_cpu(process)
-    
+
     for child in child_list:
         info[child.pid + "c"] = report_proc_cpu(child)
     return info
 
-def report_proc_mem(process):
+
+def report_proc_mem(process: psutil.Process):
     report = {}
     mem_info = process.memory_info()
     for key in mem_info._fields:
-        report[key] = getattr(mem_info,key)
+        report[key] = getattr(mem_info, key)
     return report
-    
-def get_proc_mem(pid = None):
-    if (pid == None):
+
+
+def get_proc_mem(pid=None):
+    if pid is None:
         pid = os.getpid()
     process = psutil.Process(pid)
     child_list = process.children()
     info = {}
     info[pid] = report_proc_mem(process)
-    
+
     for child in child_list:
         info[child.pid + "c"] = report_proc_mem(child)
     return info
 
+
 def convert_to_gbyte(value):
-    return value/1024./1024./1024.
+    return value / 1024.0 / 1024.0 / 1024.0
+
 
 def convert_to_mbyte(value):
-    return value/1024./1024.
+    return value / 1024.0 / 1024.0
+
 
 def convert_to_kbyte(value):
-    return value/1024.
+    return value / 1024.0
+
 
 ###################### SYSTEM REPORT ######################
 
 sys_monitor_flag = False
 procMonitorFlag = False
 doc_monitor_flag = False
 
 
-def system_report(client, interval:int, to_mb=True, to_gb=False, to_kb=False):
+def system_report(client, interval: int, to_mb=True, to_gb=False, to_kb=False):
     report = {}
-    last_net_value = {"sent":0, "receive":0}  
+    last_net_value = {"sent": 0, "receive": 0}
     while sys_monitor_flag:
         try:
             report["sys_cpu_stats"] = get_sys_mem()
         except Exception as e:
-            qoaLogger.error("Error {} in report CPU stat: {}".format(type(e),e.__traceback__))
+            qoaLogger.error(
+                "Error {} in report CPU stat: {}".format(type(e), e.__traceback__)
+            )
             traceback.print_exception(*sys.exc_info())
         try:
             report["sys_mem_stats"] = get_sys_mem()
         except Exception as e:
-            qoaLogger.error("Error {} in report memory stat: {}".format(type(e),e.__traceback__))
+            qoaLogger.error(
+                "Error {} in report memory stat: {}".format(type(e), e.__traceback__)
+            )
             traceback.print_exception(*sys.exc_info())
         try:
             report["sys_net_stats"] = get_sys_net()
             sent = 0
             if to_mb:
                 sent = convert_to_mbyte(psutil.net_io_counters().bytes_sent)
                 receive = convert_to_mbyte(psutil.net_io_counters().bytes_recv)
@@ -187,35 +284,41 @@
                 receive = convert_to_gbyte(psutil.net_io_counters().bytes_recv)
             elif to_kb:
                 sent = convert_to_kbyte(psutil.net_io_counters().bytes_sent)
                 receive = convert_to_kbyte(psutil.net_io_counters().bytes_recv)
             else:
                 sent = psutil.net_io_counters().bytes_sent
                 receive = psutil.net_io_counters().bytes_recv
-            curr_net_value = {"sent": sent, "receive": receive}  
-            report["sys_net_send"]  = curr_net_value["sent"] - last_net_value["sent"]
-            report["sys_net_receive"]  = curr_net_value["receive"] - last_net_value["receive"]
+            curr_net_value = {"sent": sent, "receive": receive}
+            report["sys_net_send"] = curr_net_value["sent"] - last_net_value["sent"]
+            report["sys_net_receive"] = (
+                curr_net_value["receive"] - last_net_value["receive"]
+            )
             last_net_value = curr_net_value.copy()
         except Exception as e:
-            qoaLogger.error("Error {} in report network stat: {}".format(type(e),e.__traceback__))
+            qoaLogger.error(
+                "Error {} in report network stat: {}".format(type(e), e.__traceback__)
+            )
             traceback.print_exception(*sys.exc_info())
         try:
             client.report(report=report)
         except Exception as e:
-            qoaLogger.error("Error {} in sent system report: {}".format(type(e),e.__traceback__))
+            qoaLogger.error(
+                "Error {} in sent system report: {}".format(type(e), e.__traceback__)
+            )
             traceback.print_exception(*sys.exc_info())
         time.sleep(interval)
 
 
-def sys_monitor(client, interval:int):
+def sys_monitor(client, interval: int):
     sub_thread = Thread(target=system_report, args=(client, interval))
     sub_thread.start()
 
 
-###################### PROCESS REPORT ######################   
+###################### PROCESS REPORT ######################
 
 # def process_report(client, interval:int, pid:int = None):
 #     report = {}
 #     while procMonitorFlag:
 #         try:
 #             report["proc_cpu_stats"] = get_proc_cpu()
 #         except Exception as e:
@@ -239,136 +342,223 @@
 #         pid = os.getpid()
 #     sub_thread = Thread(target=process_report, args=(client, interval, pid))
 #     sub_thread.start()
 
 
 ###################### DOCKER REPORT ######################
 
-def get_cpu_stat(stats,key):
-    if key == 'percentage':
-        UsageDelta = stats['cpu_stats']['cpu_usage']['total_usage'] - stats['precpu_stats']['cpu_usage']['total_usage']
 
-        SystemDelta = stats['cpu_stats']['system_cpu_usage'] - stats['precpu_stats']['system_cpu_usage']
+def get_cpu_stat(stats, key):
+    if key == "percentage":
+        UsageDelta = (
+            stats["cpu_stats"]["cpu_usage"]["total_usage"]
+            - stats["precpu_stats"]["cpu_usage"]["total_usage"]
+        )
+
+        SystemDelta = (
+            stats["cpu_stats"]["system_cpu_usage"]
+            - stats["precpu_stats"]["system_cpu_usage"]
+        )
 
-        len_cpu = stats['cpu_stats']['online_cpus']
+        len_cpu = stats["cpu_stats"]["online_cpus"]
 
         percentage = (UsageDelta / SystemDelta) * len_cpu * 100
         return round(percentage, 2)
     else:
         return -1
-def get_mem_stat(stats,key):
+
+
+def get_mem_stat(stats, key):
     if key == "used":
         return stats["memory_stats"]["usage"]
     else:
         return -1
 
-        
+
 def get_docker_stats(client):
     stats = {}
     try:
         for container in client.containers.list():
             stats[container.name] = {}
             stats[container.name]["cpu"] = {}
-            stats[container.name]["mem"]= {}
+            stats[container.name]["mem"] = {}
 
-            stat = container.stats(decode=None, stream = False) 
-            stats[container.name]["cpu"]["percentage"] = get_cpu_stat(stat,"percentage")
-            stats[container.name]["mem"]["used"] = get_mem_stat(stat,"used")
+            stat = container.stats(decode=None, stream=False)
+            stats[container.name]["cpu"]["percentage"] = get_cpu_stat(
+                stat, "percentage"
+            )
+            stats[container.name]["mem"]["used"] = get_mem_stat(stat, "used")
     except Exception as e:
-        qoaLogger.error("Error {} in query docker stat: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} in query docker stat: {}".format(type(e), e.__traceback__)
+        )
         traceback.print_exception(*sys.exc_info())
     return stats
 
-def docker_report(client, interval:int, metrics:dict = None, detail = False):
+
+def docker_report(client, interval: int, metrics: dict = None, detail=False):
     try:
         client.addMetric(metrics)
     except Exception as e:
-        qoaLogger.error("Error {} in add docker metric: {}".format(type(e),e.__traceback__))
+        qoaLogger.error(
+            "Error {} in add docker metric: {}".format(type(e), e.__traceback__)
+        )
         traceback.print_exception(*sys.exc_info())
     metric_list = list(metrics.keys())
+
+    if "docker" not in globals():
+        global docker
+        import docker
     doc_client = docker.from_env()
-    
+
     while doc_monitor_flag:
         sum_cpu = 0
         sum_memory = 0
         try:
             stats = get_docker_stats(doc_client)
             for container_name in stats:
-                sum_cpu += stats[container_name]["cpu"][metrics['dock_cpu_percentage']['key']]
-                sum_memory += stats[container_name]["mem"][metrics['docker_memory_used']['key']]
-                
-            cpu_metric = client.getMetric('dock_cpu_percentage')
+                sum_cpu += stats[container_name]["cpu"][
+                    metrics["dock_cpu_percentage"]["key"]
+                ]
+                sum_memory += stats[container_name]["mem"][
+                    metrics["docker_memory_used"]["key"]
+                ]
+
+            cpu_metric = client.getMetric("dock_cpu_percentage")
             cpu_metric.set(sum_cpu)
-            mem_metric = client.getMetric('docker_memory_used')
+            mem_metric = client.getMetric("docker_memory_used")
             mem_metric.set(sum_memory)
         except Exception as e:
-            qoaLogger.error("Error {} in report docker stat: {}".format(type(e),e.__traceback__))
+            qoaLogger.error(
+                "Error {} in report docker stat: {}".format(type(e), e.__traceback__)
+            )
             traceback.print_exception(*sys.exc_info())
 
         try:
             if detail:
                 client.report(report=stats)
             else:
                 client.report(metrics=metric_list)
         except Exception as e:
-            qoaLogger.error("Error {} in send docker report: {}".format(type(e),e.__traceback__))
+            qoaLogger.error(
+                "Error {} in send docker report: {}".format(type(e), e.__traceback__)
+            )
             traceback.print_exception(*sys.exc_info())
         time.sleep(interval)
 
-def docker_monitor(client, interval:int, metrics: dict = None, detail=False):
-    if (metrics == None):
+
+def docker_monitor(client, interval: int, metrics: dict = None, detail=False):
+    if metrics is None:
         metrics = default_docker_metric
-    sub_thread = Thread(target=docker_report, args=(client, interval, metrics,detail))
+    sub_thread = Thread(target=docker_report, args=(client, interval, metrics, detail))
     sub_thread.start()
 
 
 def mergeReport(f_report, i_report, prio=True):
     try:
         if isinstance(f_report, dict) and isinstance(i_report, dict):
             key_list = tuple(f_report.keys())
             for key in key_list:
                 if key in i_report:
-                    f_report[key] = mergeReport(f_report[key],i_report[key],prio)
+                    f_report[key] = mergeReport(f_report[key], i_report[key], prio)
                     i_report.pop(key)
             f_report.update(i_report)
         else:
             if f_report != i_report:
-                if prio == True:
+                if prio is True:
                     return f_report
                 else:
                     return i_report
     except Exception as e:
-        qoaLogger.error("Error {} in mergeReport: {}".format(type(e),e.__traceback__))
+        qoaLogger.error("Error {} in mergeReport: {}".format(type(e), e.__traceback__))
         traceback.print_exception(*sys.exc_info())
     return f_report
 
+
 def get_dict_at(dict, i=0):
     try:
         keys = list(dict.keys())
-        return  keys[i], dict[keys[i]]
+        return keys[i], dict[keys[i]]
     except Exception as e:
-        qoaLogger.error("Error {} in get_dict_at: {}".format(type(e),e.__traceback__))
+        qoaLogger.error("Error {} in get_dict_at: {}".format(type(e), e.__traceback__))
         traceback.print_exception(*sys.exc_info())
 
+
 def get_file_dir(file, to_string=True):
     current_dir = pathlib.Path(file).parent.absolute()
     if to_string:
         return str(current_dir)
     else:
         return current_dir
 
+
 def get_parent_dir(file, parent_level=1, to_string=True):
     current_dir = get_file_dir(file=file, to_string=False)
     for i in range(parent_level):
         current_dir = current_dir.parent.absolute()
     if to_string:
         return str(current_dir)
     else:
         return current_dir
 
 
-
 def is_numpyarray(obj):
+    if "np" not in globals():
+        global np
+        import numpy as np
     return type(obj) == np.ndarray
 
+
 def is_pddataframe(obj):
-    return type(obj) == pd.DataFrame
+    if "pd" not in globals():
+        global pd
+        import pandas as pd
+    return type(obj) == pd.DataFrame
+
+
+def get_process_allowed_cpus():
+    # NOTE: 0 as PID represents the calling process
+    pid = 0
+    affinity = os.sched_getaffinity(pid)
+    return list(affinity)
+
+
+def get_process_allowed_memory():
+    if CGROUP_VERSION == "v1":
+        with open("/proc/self/cgroup") as file:
+            for line in file:
+                parts = line.strip().split(":")
+                if len(parts) == 3 and parts[1] == "memory":
+                    cgroup_path = parts[2]
+                    memory_limit_file = re.sub(r"/task_\d+", "", cgroup_path)
+
+                    number_of_task = len(
+                        glob.glob(f"/sys/fs/cgroup/memory{memory_limit_file}/task_*")
+                    )
+
+                    with open(
+                        f"/sys/fs/cgroup/memory{memory_limit_file}/memory.limit_in_bytes"
+                    ) as limit_file:
+                        memory_limit_str = limit_file.read().strip()
+                        try:
+                            memory_limit_int = int(memory_limit_str)
+                            return memory_limit_int / number_of_task
+                        except ValueError:
+                            return memory_limit_str
+
+    else:
+        with open("/proc/self/cgroup") as file:
+            for line in file:
+                parts = line.strip().split(":")
+                cgroup_path = parts[2]
+                pattern = r"/task_\d+"
+                cgroup_path = re.sub(pattern, "", cgroup_path)
+                with open(f"/sys/fs/cgroup{cgroup_path}/memory.max") as limit_file:
+                    number_of_task = len(
+                        glob.glob(f"/sys/fs/cgroup{cgroup_path}/task_*")
+                    )
+                    memory_limit_str = limit_file.read().strip()
+                    try:
+                        memory_limit_int = int(memory_limit_str)
+                        return memory_limit_int / number_of_task
+                    except ValueError:
+                        return memory_limit_str
```

### Comparing `qoa4ml-0.1.9/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.2.0/qoa4ml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: ml
+Provides-Extra: dev
 License-File: LICENCE.txt
 
 # QoA4ML - Quality of Analytics for ML
 
 ## Source code
 https://github.com/rdsea/QoA4ML
 
@@ -24,19 +25,19 @@
 
 The `configuration` contains the information about the client and its configuration in form of dictionary
 
 Example: 
 ```python
 clientConf = { 
     "client":{
-        "client_id": "aaltosea1",
+        "user_id": "aaltosea1",
         "instance_name": "ML02",
         "stage_id": "ML",
         "method": "REST",
-        "application": "test",
+        "application_name": "test",
         "role": "ml"
     },
     "connector":{
         "amqp_connector":{
             "class": "amqp",
             "conf":{
                 "end_point": "localhost",
@@ -220,14 +221,20 @@
     - `send_data`: a function to send data to specified `routing_key`/`queue` with a corresponding key `corr_id` to trace back message.
 
 
 
 ## Utilities
 A module provide some frequently used functions and some function to directly collect system metrics.
 
+## Note
+- `eva_duplicate`, `eva_erronous`, `eva_missing`, and `detect_outlier` probes are using ydata-quality library, which is only available for Python 3.8
+- For using ML quality probes, you may need to install a few more dependencies, e.g., tensorflow and Pillow.
+- QoaClient uses AMQP protocol by default. To use MQTT, you may need to install `paho-mqtt`.
+- To monitor Docker stats, you need to install [docker](https://docker-py.readthedocs.io/en/stable/) python client. 
+- To connect with Prometheus, you need to install [prometheus-client](https://pypi.org/project/prometheus-client/)
 
 
 Change Log
 ======================
 
 0.0.13 (18/04/2022)
 ---------------------
@@ -253,7 +260,10 @@
 ---------------------
 Add metric and modify format of system/process reports
 
 0.0.72 (22/05/2023)
 ---------------------
 Refactor source code
 
+0.0.73 (19/04/2024)
+---------------------
+Add new ODOP observability module
```

### Comparing `qoa4ml-0.1.9/setup.py` & `qoa4ml-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
-    name='qoa4ml',
-    version=open('VERSION').read(),
-    description='Quality of Analysis for Machine Learning',
-    long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
-    long_description_content_type='text/markdown',
-    url='https://rdsea.github.io/',
-    author='AaltoSEA',
-    email='tri.m.nguyen@aalto.fi',
-    keyword='Monitoring Machine Learning',
-    #install_requires=['pika','requests','paho-mqtt','prometheus-client','psutil', 'docker'],
-    install_requires=[line.strip() for line in  open('requirements.txt').readlines()], 
+    name="qoa4ml",
+    version=open("VERSION").read(),
+    description="Quality of Analysis for Machine Learning",
+    long_description=open("README.md").read() + "\n\n" + open("CHANGELOG.txt").read(),
+    long_description_content_type="text/markdown",
+    url="https://rdsea.github.io/",
+    author="AaltoSEA",
+    email="tri.m.nguyen@aalto.fi",
+    keyword="Monitoring Machine Learning",
+    install_requires=[line.strip() for line in open("requirements.txt").readlines()],
+    extras_require={
+        "ml": [line.strip() for line in open("ml_requirements.txt").readlines()],
+        "dev": [line.strip() for line in open("dev_requirements.txt").readlines()],
+    },
     packages=find_packages(),
-    license='Apache License 2.0'
-)
+    license="Apache License 2.0",
+)
```

