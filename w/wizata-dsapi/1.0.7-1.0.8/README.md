# Comparing `tmp/wizata-dsapi-1.0.7.tar.gz` & `tmp/wizata-dsapi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-1.0.7.tar", last modified: Fri May 24 09:06:11 2024, max compression
+gzip compressed data, was "wizata-dsapi-1.0.8.tar", last modified: Mon May 27 11:56:54 2024, max compression
```

## Comparing `wizata-dsapi-1.0.7.tar` & `wizata-dsapi-1.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-24 09:06:11.986016 wizata-dsapi-1.0.7/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.7/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-05-24 09:06:11.985890 wizata-dsapi-1.0.7/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.7/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-05-24 09:06:11.986061 wizata-dsapi-1.0.7/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1450 2024-05-22 09:08:26.000000 wizata-dsapi-1.0.7/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-24 09:06:11.985090 wizata-dsapi-1.0.7/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1599 2024-05-24 09:06:02.000000 wizata-dsapi-1.0.7/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3875 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/api_config.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1172 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     9270 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/api_interface.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4151 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/business_label.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10084 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8472 2024-05-16 13:17:14.000000 wizata-dsapi-1.0.7/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10822 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2089 2024-03-06 07:51:32.000000 wizata-dsapi-1.0.7/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.7/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    13229 2024-05-24 08:38:26.000000 wizata-dsapi-1.0.7/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4355 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      807 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/ilogger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    14587 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1551 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1150 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/paged_query_result.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    28788 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      207 2024-05-24 09:05:32.000000 wizata-dsapi-1.0.7/wizata_dsapi/pipeline_image.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2355 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    19308 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12710 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7625 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/solution_component.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12451 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4769 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/trigger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     6291 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12865 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-05-24 09:05:32.000000 wizata-dsapi-1.0.7/wizata_dsapi/version.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      942 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3762 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/wizard_request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    68678 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.7/wizata_dsapi/wizata_dsapi_client.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1535 2024-03-20 11:49:55.000000 wizata-dsapi-1.0.7/wizata_dsapi/words.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-24 09:06:11.985704 wizata-dsapi-1.0.7/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-05-24 09:06:11.000000 wizata-dsapi-1.0.7/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1068 2024-05-24 09:06:11.000000 wizata-dsapi-1.0.7/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-05-24 09:06:11.000000 wizata-dsapi-1.0.7/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      591 2024-05-24 09:06:11.000000 wizata-dsapi-1.0.7/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-05-24 09:06:11.000000 wizata-dsapi-1.0.7/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-27 11:56:54.322772 wizata-dsapi-1.0.8/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.8/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-05-27 11:56:54.322641 wizata-dsapi-1.0.8/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.8/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-05-27 11:56:54.322818 wizata-dsapi-1.0.8/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1450 2024-05-22 09:08:26.000000 wizata-dsapi-1.0.8/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-27 11:56:54.321786 wizata-dsapi-1.0.8/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1599 2024-05-24 09:06:02.000000 wizata-dsapi-1.0.8/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3875 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/api_config.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1172 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     9270 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/api_interface.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4151 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/business_label.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10084 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8472 2024-05-16 13:17:14.000000 wizata-dsapi-1.0.8/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10822 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2089 2024-03-06 07:51:32.000000 wizata-dsapi-1.0.8/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.8/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    13229 2024-05-24 08:38:26.000000 wizata-dsapi-1.0.8/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4355 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      807 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/ilogger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    14587 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1551 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1150 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/paged_query_result.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    28788 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3703 2024-05-27 11:43:32.000000 wizata-dsapi-1.0.8/wizata_dsapi/pipeline_image.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2355 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19308 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12710 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7625 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/solution_component.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12451 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4769 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/trigger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     6291 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12865 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-05-27 11:43:32.000000 wizata-dsapi-1.0.8/wizata_dsapi/version.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      942 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3762 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/wizard_request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    68678 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.8/wizata_dsapi/wizata_dsapi_client.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1535 2024-03-20 11:49:55.000000 wizata-dsapi-1.0.8/wizata_dsapi/words.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-27 11:56:54.322467 wizata-dsapi-1.0.8/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-05-27 11:56:54.000000 wizata-dsapi-1.0.8/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1068 2024-05-27 11:56:54.000000 wizata-dsapi-1.0.8/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-05-27 11:56:54.000000 wizata-dsapi-1.0.8/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      591 2024-05-27 11:56:54.000000 wizata-dsapi-1.0.8/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-05-27 11:56:54.000000 wizata-dsapi-1.0.8/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-1.0.7/LICENSE.txt` & `wizata-dsapi-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/setup.py` & `wizata-dsapi-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/__init__.py` & `wizata-dsapi-1.0.8/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/api_config.py` & `wizata-dsapi-1.0.8/wizata_dsapi/api_config.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/api_dto.py` & `wizata-dsapi-1.0.8/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/api_interface.py` & `wizata-dsapi-1.0.8/wizata_dsapi/api_interface.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/business_label.py` & `wizata-dsapi-1.0.8/wizata_dsapi/business_label.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/context.py` & `wizata-dsapi-1.0.8/wizata_dsapi/context.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-1.0.8/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/datapoint.py` & `wizata-dsapi-1.0.8/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-1.0.8/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-1.0.8/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/execution.py` & `wizata-dsapi-1.0.8/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/experiment.py` & `wizata-dsapi-1.0.8/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/ilogger.py` & `wizata-dsapi-1.0.8/wizata_dsapi/ilogger.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/mlmodel.py` & `wizata-dsapi-1.0.8/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-1.0.8/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/paged_query_result.py` & `wizata-dsapi-1.0.8/wizata_dsapi/paged_query_result.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/pipeline.py` & `wizata-dsapi-1.0.8/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/plot.py` & `wizata-dsapi-1.0.8/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/request.py` & `wizata-dsapi-1.0.8/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/script.py` & `wizata-dsapi-1.0.8/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/solution_component.py` & `wizata-dsapi-1.0.8/wizata_dsapi/solution_component.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/template.py` & `wizata-dsapi-1.0.8/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/trigger.py` & `wizata-dsapi-1.0.8/wizata_dsapi/trigger.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/twin.py` & `wizata-dsapi-1.0.8/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/twinregistration.py` & `wizata-dsapi-1.0.8/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/wizard_function.py` & `wizata-dsapi-1.0.8/wizata_dsapi/wizard_function.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/wizard_request.py` & `wizata-dsapi-1.0.8/wizata_dsapi/wizard_request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-1.0.8/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi/words.py` & `wizata-dsapi-1.0.8/wizata_dsapi/words.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-1.0.8/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-1.0.7/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-1.0.8/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

