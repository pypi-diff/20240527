# Comparing `tmp/alibabacloud_mns-open20220119-1.0.2.tar.gz` & `tmp/alibabacloud_mns-open20220119-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mns-open20220119-1.0.2.tar", last modified: Wed May  8 17:09:39 2024, max compression
+gzip compressed data, was "dist/alibabacloud_mns-open20220119-1.0.3.tar", last modified: Mon May 27 17:12:43 2024, max compression
```

## Comparing `alibabacloud_mns-open20220119-1.0.2.tar` & `alibabacloud_mns-open20220119-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      125 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48282 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/client.py
--rw-r--r--   0 root         (0) root         (0)    96763 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2638 2024-05-08 17:09:39.000000 alibabacloud_mns-open20220119-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60872 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-05-27 17:12:43.000000 alibabacloud_mns-open20220119-1.0.3/setup.py
```

### Comparing `alibabacloud_mns-open20220119-1.0.2/LICENSE` & `alibabacloud_mns-open20220119-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.2/PKG-INFO` & `alibabacloud_mns-open20220119-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mns-open20220119
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mns-open20220119-1.0.2/README-CN.md` & `alibabacloud_mns-open20220119-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.2/README.md` & `alibabacloud_mns-open20220119-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/client.py` & `alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,28 +42,37 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def create_queue_with_options(
         self,
         request: mns_open_20220119_models.CreateQueueRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.CreateQueueResponse:
+        """
+        @summary CreateQueue
+        
+        @param request: CreateQueueRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateQueueResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.delay_seconds):
             query['DelaySeconds'] = request.delay_seconds
         if not UtilClient.is_unset(request.enable_logging):
             query['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.maximum_message_size):
             query['MaximumMessageSize'] = request.maximum_message_size
         if not UtilClient.is_unset(request.message_retention_period):
             query['MessageRetentionPeriod'] = request.message_retention_period
         if not UtilClient.is_unset(request.polling_wait_seconds):
             query['PollingWaitSeconds'] = request.polling_wait_seconds
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.visibility_timeout):
             query['VisibilityTimeout'] = request.visibility_timeout
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateQueue',
@@ -82,28 +91,37 @@
         )
 
     async def create_queue_with_options_async(
         self,
         request: mns_open_20220119_models.CreateQueueRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.CreateQueueResponse:
+        """
+        @summary CreateQueue
+        
+        @param request: CreateQueueRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateQueueResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.delay_seconds):
             query['DelaySeconds'] = request.delay_seconds
         if not UtilClient.is_unset(request.enable_logging):
             query['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.maximum_message_size):
             query['MaximumMessageSize'] = request.maximum_message_size
         if not UtilClient.is_unset(request.message_retention_period):
             query['MessageRetentionPeriod'] = request.message_retention_period
         if not UtilClient.is_unset(request.polling_wait_seconds):
             query['PollingWaitSeconds'] = request.polling_wait_seconds
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.visibility_timeout):
             query['VisibilityTimeout'] = request.visibility_timeout
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateQueue',
@@ -121,38 +139,61 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_queue(
         self,
         request: mns_open_20220119_models.CreateQueueRequest,
     ) -> mns_open_20220119_models.CreateQueueResponse:
+        """
+        @summary CreateQueue
+        
+        @param request: CreateQueueRequest
+        @return: CreateQueueResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_queue_with_options(request, runtime)
 
     async def create_queue_async(
         self,
         request: mns_open_20220119_models.CreateQueueRequest,
     ) -> mns_open_20220119_models.CreateQueueResponse:
+        """
+        @summary CreateQueue
+        
+        @param request: CreateQueueRequest
+        @return: CreateQueueResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_queue_with_options_async(request, runtime)
 
     def create_topic_with_options(
         self,
         request: mns_open_20220119_models.CreateTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.CreateTopicResponse:
+        """
+        @summary CreateTopic
+        
+        @param request: CreateTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTopicResponse
+        """
         UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         body = {}
         if not UtilClient.is_unset(request.enable_logging):
             body['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.max_message_size):
             body['MaxMessageSize'] = request.max_message_size
         if not UtilClient.is_unset(request.topic_name):
             body['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateTopic',
             version='2022-01-19',
             protocol='HTTPS',
             pathname='/',
@@ -168,23 +209,34 @@
         )
 
     async def create_topic_with_options_async(
         self,
         request: mns_open_20220119_models.CreateTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.CreateTopicResponse:
+        """
+        @summary CreateTopic
+        
+        @param request: CreateTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTopicResponse
+        """
         UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         body = {}
         if not UtilClient.is_unset(request.enable_logging):
             body['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.max_message_size):
             body['MaxMessageSize'] = request.max_message_size
         if not UtilClient.is_unset(request.topic_name):
             body['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateTopic',
             version='2022-01-19',
             protocol='HTTPS',
             pathname='/',
@@ -199,29 +251,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_topic(
         self,
         request: mns_open_20220119_models.CreateTopicRequest,
     ) -> mns_open_20220119_models.CreateTopicResponse:
+        """
+        @summary CreateTopic
+        
+        @param request: CreateTopicRequest
+        @return: CreateTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_topic_with_options(request, runtime)
 
     async def create_topic_async(
         self,
         request: mns_open_20220119_models.CreateTopicRequest,
     ) -> mns_open_20220119_models.CreateTopicResponse:
+        """
+        @summary CreateTopic
+        
+        @param request: CreateTopicRequest
+        @return: CreateTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_topic_with_options_async(request, runtime)
 
     def delete_queue_with_options(
         self,
         request: mns_open_20220119_models.DeleteQueueRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.DeleteQueueResponse:
+        """
+        @summary DeleteQueue
+        
+        @param request: DeleteQueueRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteQueueResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -242,14 +313,21 @@
         )
 
     async def delete_queue_with_options_async(
         self,
         request: mns_open_20220119_models.DeleteQueueRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.DeleteQueueResponse:
+        """
+        @summary DeleteQueue
+        
+        @param request: DeleteQueueRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteQueueResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -269,29 +347,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_queue(
         self,
         request: mns_open_20220119_models.DeleteQueueRequest,
     ) -> mns_open_20220119_models.DeleteQueueResponse:
+        """
+        @summary DeleteQueue
+        
+        @param request: DeleteQueueRequest
+        @return: DeleteQueueResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_queue_with_options(request, runtime)
 
     async def delete_queue_async(
         self,
         request: mns_open_20220119_models.DeleteQueueRequest,
     ) -> mns_open_20220119_models.DeleteQueueResponse:
+        """
+        @summary DeleteQueue
+        
+        @param request: DeleteQueueRequest
+        @return: DeleteQueueResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_queue_with_options_async(request, runtime)
 
     def delete_topic_with_options(
         self,
         request: mns_open_20220119_models.DeleteTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.DeleteTopicResponse:
+        """
+        @summary 删除订阅主题
+        
+        @param request: DeleteTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -312,14 +409,21 @@
         )
 
     async def delete_topic_with_options_async(
         self,
         request: mns_open_20220119_models.DeleteTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.DeleteTopicResponse:
+        """
+        @summary 删除订阅主题
+        
+        @param request: DeleteTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -339,33 +443,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_topic(
         self,
         request: mns_open_20220119_models.DeleteTopicRequest,
     ) -> mns_open_20220119_models.DeleteTopicResponse:
+        """
+        @summary 删除订阅主题
+        
+        @param request: DeleteTopicRequest
+        @return: DeleteTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_topic_with_options(request, runtime)
 
     async def delete_topic_async(
         self,
         request: mns_open_20220119_models.DeleteTopicRequest,
     ) -> mns_open_20220119_models.DeleteTopicResponse:
+        """
+        @summary 删除订阅主题
+        
+        @param request: DeleteTopicRequest
+        @return: DeleteTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_topic_with_options_async(request, runtime)
 
     def get_queue_attributes_with_options(
         self,
         request: mns_open_20220119_models.GetQueueAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.GetQueueAttributesResponse:
+        """
+        @summary GetQueueAttributes
+        
+        @param request: GetQueueAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetQueueAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetQueueAttributes',
             version='2022-01-19',
             protocol='HTTPS',
@@ -382,18 +507,27 @@
         )
 
     async def get_queue_attributes_with_options_async(
         self,
         request: mns_open_20220119_models.GetQueueAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.GetQueueAttributesResponse:
+        """
+        @summary GetQueueAttributes
+        
+        @param request: GetQueueAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetQueueAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetQueueAttributes',
             version='2022-01-19',
             protocol='HTTPS',
@@ -409,29 +543,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_queue_attributes(
         self,
         request: mns_open_20220119_models.GetQueueAttributesRequest,
     ) -> mns_open_20220119_models.GetQueueAttributesResponse:
+        """
+        @summary GetQueueAttributes
+        
+        @param request: GetQueueAttributesRequest
+        @return: GetQueueAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_queue_attributes_with_options(request, runtime)
 
     async def get_queue_attributes_async(
         self,
         request: mns_open_20220119_models.GetQueueAttributesRequest,
     ) -> mns_open_20220119_models.GetQueueAttributesResponse:
+        """
+        @summary GetQueueAttributes
+        
+        @param request: GetQueueAttributesRequest
+        @return: GetQueueAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_queue_attributes_with_options_async(request, runtime)
 
     def get_subscription_attributes_with_options(
         self,
         request: mns_open_20220119_models.GetSubscriptionAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.GetSubscriptionAttributesResponse:
+        """
+        @summary GetSubscription
+        
+        @param request: GetSubscriptionAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSubscriptionAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.subscription_name):
             query['SubscriptionName'] = request.subscription_name
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
@@ -454,14 +607,21 @@
         )
 
     async def get_subscription_attributes_with_options_async(
         self,
         request: mns_open_20220119_models.GetSubscriptionAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.GetSubscriptionAttributesResponse:
+        """
+        @summary GetSubscription
+        
+        @param request: GetSubscriptionAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSubscriptionAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.subscription_name):
             query['SubscriptionName'] = request.subscription_name
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
@@ -483,31 +643,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_subscription_attributes(
         self,
         request: mns_open_20220119_models.GetSubscriptionAttributesRequest,
     ) -> mns_open_20220119_models.GetSubscriptionAttributesResponse:
+        """
+        @summary GetSubscription
+        
+        @param request: GetSubscriptionAttributesRequest
+        @return: GetSubscriptionAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_subscription_attributes_with_options(request, runtime)
 
     async def get_subscription_attributes_async(
         self,
         request: mns_open_20220119_models.GetSubscriptionAttributesRequest,
     ) -> mns_open_20220119_models.GetSubscriptionAttributesResponse:
+        """
+        @summary GetSubscription
+        
+        @param request: GetSubscriptionAttributesRequest
+        @return: GetSubscriptionAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_subscription_attributes_with_options_async(request, runtime)
 
     def get_topic_attributes_with_options(
         self,
         request: mns_open_20220119_models.GetTopicAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.GetTopicAttributesResponse:
+        """
+        @summary 查询主题
+        
+        @param request: GetTopicAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetTopicAttributes',
@@ -526,16 +707,25 @@
         )
 
     async def get_topic_attributes_with_options_async(
         self,
         request: mns_open_20220119_models.GetTopicAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.GetTopicAttributesResponse:
+        """
+        @summary 查询主题
+        
+        @param request: GetTopicAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTopicAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetTopicAttributes',
@@ -553,37 +743,58 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_topic_attributes(
         self,
         request: mns_open_20220119_models.GetTopicAttributesRequest,
     ) -> mns_open_20220119_models.GetTopicAttributesResponse:
+        """
+        @summary 查询主题
+        
+        @param request: GetTopicAttributesRequest
+        @return: GetTopicAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_topic_attributes_with_options(request, runtime)
 
     async def get_topic_attributes_async(
         self,
         request: mns_open_20220119_models.GetTopicAttributesRequest,
     ) -> mns_open_20220119_models.GetTopicAttributesResponse:
+        """
+        @summary 查询主题
+        
+        @param request: GetTopicAttributesRequest
+        @return: GetTopicAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_topic_attributes_with_options_async(request, runtime)
 
     def list_queue_with_options(
         self,
         request: mns_open_20220119_models.ListQueueRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.ListQueueResponse:
+        """
+        @summary ListQueue
+        
+        @param request: ListQueueRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListQueueResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListQueue',
             version='2022-01-19',
             protocol='HTTPS',
@@ -600,22 +811,31 @@
         )
 
     async def list_queue_with_options_async(
         self,
         request: mns_open_20220119_models.ListQueueRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.ListQueueResponse:
+        """
+        @summary ListQueue
+        
+        @param request: ListQueueRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListQueueResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.queue_name):
             query['QueueName'] = request.queue_name
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListQueue',
             version='2022-01-19',
             protocol='HTTPS',
@@ -631,29 +851,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_queue(
         self,
         request: mns_open_20220119_models.ListQueueRequest,
     ) -> mns_open_20220119_models.ListQueueResponse:
+        """
+        @summary ListQueue
+        
+        @param request: ListQueueRequest
+        @return: ListQueueResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_queue_with_options(request, runtime)
 
     async def list_queue_async(
         self,
         request: mns_open_20220119_models.ListQueueRequest,
     ) -> mns_open_20220119_models.ListQueueResponse:
+        """
+        @summary ListQueue
+        
+        @param request: ListQueueRequest
+        @return: ListQueueResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_queue_with_options_async(request, runtime)
 
     def list_subscription_by_topic_with_options(
         self,
         request: mns_open_20220119_models.ListSubscriptionByTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.ListSubscriptionByTopicResponse:
+        """
+        @summary ListSubscription
+        
+        @param request: ListSubscriptionByTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSubscriptionByTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.subscription_name):
@@ -680,14 +919,21 @@
         )
 
     async def list_subscription_by_topic_with_options_async(
         self,
         request: mns_open_20220119_models.ListSubscriptionByTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.ListSubscriptionByTopicResponse:
+        """
+        @summary ListSubscription
+        
+        @param request: ListSubscriptionByTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSubscriptionByTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.subscription_name):
@@ -713,35 +959,56 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_subscription_by_topic(
         self,
         request: mns_open_20220119_models.ListSubscriptionByTopicRequest,
     ) -> mns_open_20220119_models.ListSubscriptionByTopicResponse:
+        """
+        @summary ListSubscription
+        
+        @param request: ListSubscriptionByTopicRequest
+        @return: ListSubscriptionByTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_subscription_by_topic_with_options(request, runtime)
 
     async def list_subscription_by_topic_async(
         self,
         request: mns_open_20220119_models.ListSubscriptionByTopicRequest,
     ) -> mns_open_20220119_models.ListSubscriptionByTopicResponse:
+        """
+        @summary ListSubscription
+        
+        @param request: ListSubscriptionByTopicRequest
+        @return: ListSubscriptionByTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_subscription_by_topic_with_options_async(request, runtime)
 
     def list_topic_with_options(
         self,
         request: mns_open_20220119_models.ListTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.ListTopicResponse:
+        """
+        @summary ListTopic
+        
+        @param request: ListTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTopic',
@@ -760,20 +1027,29 @@
         )
 
     async def list_topic_with_options_async(
         self,
         request: mns_open_20220119_models.ListTopicRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.ListTopicResponse:
+        """
+        @summary ListTopic
+        
+        @param request: ListTopicRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTopicResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTopic',
@@ -791,29 +1067,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_topic(
         self,
         request: mns_open_20220119_models.ListTopicRequest,
     ) -> mns_open_20220119_models.ListTopicResponse:
+        """
+        @summary ListTopic
+        
+        @param request: ListTopicRequest
+        @return: ListTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_topic_with_options(request, runtime)
 
     async def list_topic_async(
         self,
         request: mns_open_20220119_models.ListTopicRequest,
     ) -> mns_open_20220119_models.ListTopicResponse:
+        """
+        @summary ListTopic
+        
+        @param request: ListTopicRequest
+        @return: ListTopicResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_topic_with_options_async(request, runtime)
 
     def set_queue_attributes_with_options(
         self,
         request: mns_open_20220119_models.SetQueueAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SetQueueAttributesResponse:
+        """
+        @summary SetQueueAttributes
+        
+        @param request: SetQueueAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetQueueAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.delay_seconds):
             query['DelaySeconds'] = request.delay_seconds
         if not UtilClient.is_unset(request.enable_logging):
             query['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.maximum_message_size):
@@ -846,14 +1141,21 @@
         )
 
     async def set_queue_attributes_with_options_async(
         self,
         request: mns_open_20220119_models.SetQueueAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SetQueueAttributesResponse:
+        """
+        @summary SetQueueAttributes
+        
+        @param request: SetQueueAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetQueueAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.delay_seconds):
             query['DelaySeconds'] = request.delay_seconds
         if not UtilClient.is_unset(request.enable_logging):
             query['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.maximum_message_size):
@@ -885,29 +1187,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_queue_attributes(
         self,
         request: mns_open_20220119_models.SetQueueAttributesRequest,
     ) -> mns_open_20220119_models.SetQueueAttributesResponse:
+        """
+        @summary SetQueueAttributes
+        
+        @param request: SetQueueAttributesRequest
+        @return: SetQueueAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_queue_attributes_with_options(request, runtime)
 
     async def set_queue_attributes_async(
         self,
         request: mns_open_20220119_models.SetQueueAttributesRequest,
     ) -> mns_open_20220119_models.SetQueueAttributesResponse:
+        """
+        @summary SetQueueAttributes
+        
+        @param request: SetQueueAttributesRequest
+        @return: SetQueueAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_queue_attributes_with_options_async(request, runtime)
 
     def set_subscription_attributes_with_options(
         self,
         request: mns_open_20220119_models.SetSubscriptionAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SetSubscriptionAttributesResponse:
+        """
+        @summary ModifySubscription
+        
+        @param request: SetSubscriptionAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetSubscriptionAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.notify_strategy):
             query['NotifyStrategy'] = request.notify_strategy
         if not UtilClient.is_unset(request.subscription_name):
             query['SubscriptionName'] = request.subscription_name
         if not UtilClient.is_unset(request.topic_name):
@@ -932,14 +1253,21 @@
         )
 
     async def set_subscription_attributes_with_options_async(
         self,
         request: mns_open_20220119_models.SetSubscriptionAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SetSubscriptionAttributesResponse:
+        """
+        @summary ModifySubscription
+        
+        @param request: SetSubscriptionAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetSubscriptionAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.notify_strategy):
             query['NotifyStrategy'] = request.notify_strategy
         if not UtilClient.is_unset(request.subscription_name):
             query['SubscriptionName'] = request.subscription_name
         if not UtilClient.is_unset(request.topic_name):
@@ -963,29 +1291,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_subscription_attributes(
         self,
         request: mns_open_20220119_models.SetSubscriptionAttributesRequest,
     ) -> mns_open_20220119_models.SetSubscriptionAttributesResponse:
+        """
+        @summary ModifySubscription
+        
+        @param request: SetSubscriptionAttributesRequest
+        @return: SetSubscriptionAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_subscription_attributes_with_options(request, runtime)
 
     async def set_subscription_attributes_async(
         self,
         request: mns_open_20220119_models.SetSubscriptionAttributesRequest,
     ) -> mns_open_20220119_models.SetSubscriptionAttributesResponse:
+        """
+        @summary ModifySubscription
+        
+        @param request: SetSubscriptionAttributesRequest
+        @return: SetSubscriptionAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_subscription_attributes_with_options_async(request, runtime)
 
     def set_topic_attributes_with_options(
         self,
         request: mns_open_20220119_models.SetTopicAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SetTopicAttributesResponse:
+        """
+        @summary 编辑订阅主题
+        
+        @param request: SetTopicAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetTopicAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.enable_logging):
             query['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.max_message_size):
             query['MaxMessageSize'] = request.max_message_size
         if not UtilClient.is_unset(request.topic_name):
@@ -1010,14 +1357,21 @@
         )
 
     async def set_topic_attributes_with_options_async(
         self,
         request: mns_open_20220119_models.SetTopicAttributesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SetTopicAttributesResponse:
+        """
+        @summary 编辑订阅主题
+        
+        @param request: SetTopicAttributesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetTopicAttributesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.enable_logging):
             query['EnableLogging'] = request.enable_logging
         if not UtilClient.is_unset(request.max_message_size):
             query['MaxMessageSize'] = request.max_message_size
         if not UtilClient.is_unset(request.topic_name):
@@ -1041,29 +1395,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_topic_attributes(
         self,
         request: mns_open_20220119_models.SetTopicAttributesRequest,
     ) -> mns_open_20220119_models.SetTopicAttributesResponse:
+        """
+        @summary 编辑订阅主题
+        
+        @param request: SetTopicAttributesRequest
+        @return: SetTopicAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_topic_attributes_with_options(request, runtime)
 
     async def set_topic_attributes_async(
         self,
         request: mns_open_20220119_models.SetTopicAttributesRequest,
     ) -> mns_open_20220119_models.SetTopicAttributesResponse:
+        """
+        @summary 编辑订阅主题
+        
+        @param request: SetTopicAttributesRequest
+        @return: SetTopicAttributesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_topic_attributes_with_options_async(request, runtime)
 
     def subscribe_with_options(
         self,
         request: mns_open_20220119_models.SubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SubscribeResponse:
+        """
+        @summary CreateSubscription
+        
+        @param request: SubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.endpoint):
             query['Endpoint'] = request.endpoint
         if not UtilClient.is_unset(request.message_tag):
             query['MessageTag'] = request.message_tag
         if not UtilClient.is_unset(request.notify_content_format):
@@ -1096,14 +1469,21 @@
         )
 
     async def subscribe_with_options_async(
         self,
         request: mns_open_20220119_models.SubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.SubscribeResponse:
+        """
+        @summary CreateSubscription
+        
+        @param request: SubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.endpoint):
             query['Endpoint'] = request.endpoint
         if not UtilClient.is_unset(request.message_tag):
             query['MessageTag'] = request.message_tag
         if not UtilClient.is_unset(request.notify_content_format):
@@ -1135,29 +1515,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def subscribe(
         self,
         request: mns_open_20220119_models.SubscribeRequest,
     ) -> mns_open_20220119_models.SubscribeResponse:
+        """
+        @summary CreateSubscription
+        
+        @param request: SubscribeRequest
+        @return: SubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.subscribe_with_options(request, runtime)
 
     async def subscribe_async(
         self,
         request: mns_open_20220119_models.SubscribeRequest,
     ) -> mns_open_20220119_models.SubscribeResponse:
+        """
+        @summary CreateSubscription
+        
+        @param request: SubscribeRequest
+        @return: SubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.subscribe_with_options_async(request, runtime)
 
     def unsubscribe_with_options(
         self,
         request: mns_open_20220119_models.UnsubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.UnsubscribeResponse:
+        """
+        @summary DeleteSubscription
+        
+        @param request: UnsubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UnsubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.subscription_name):
             query['SubscriptionName'] = request.subscription_name
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
@@ -1180,14 +1579,21 @@
         )
 
     async def unsubscribe_with_options_async(
         self,
         request: mns_open_20220119_models.UnsubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> mns_open_20220119_models.UnsubscribeResponse:
+        """
+        @summary DeleteSubscription
+        
+        @param request: UnsubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UnsubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.subscription_name):
             query['SubscriptionName'] = request.subscription_name
         if not UtilClient.is_unset(request.topic_name):
             query['TopicName'] = request.topic_name
         req = open_api_models.OpenApiRequest(
@@ -1209,16 +1615,28 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def unsubscribe(
         self,
         request: mns_open_20220119_models.UnsubscribeRequest,
     ) -> mns_open_20220119_models.UnsubscribeResponse:
+        """
+        @summary DeleteSubscription
+        
+        @param request: UnsubscribeRequest
+        @return: UnsubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.unsubscribe_with_options(request, runtime)
 
     async def unsubscribe_async(
         self,
         request: mns_open_20220119_models.UnsubscribeRequest,
     ) -> mns_open_20220119_models.UnsubscribeResponse:
+        """
+        @summary DeleteSubscription
+        
+        @param request: UnsubscribeRequest
+        @return: UnsubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.unsubscribe_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119/models.py` & `alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,73 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, Any, List
+from typing import List, Dict, Any
+
+
+class CreateQueueRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
 
 
 class CreateQueueRequest(TeaModel):
     def __init__(
         self,
         delay_seconds: int = None,
         enable_logging: bool = None,
         maximum_message_size: int = None,
         message_retention_period: int = None,
         polling_wait_seconds: int = None,
         queue_name: str = None,
+        tag: List[CreateQueueRequestTag] = None,
         visibility_timeout: int = None,
     ):
         self.delay_seconds = delay_seconds
         self.enable_logging = enable_logging
         self.maximum_message_size = maximum_message_size
         self.message_retention_period = message_retention_period
         self.polling_wait_seconds = polling_wait_seconds
+        # This parameter is required.
         self.queue_name = queue_name
+        self.tag = tag
         self.visibility_timeout = visibility_timeout
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -40,14 +79,18 @@
             result['MaximumMessageSize'] = self.maximum_message_size
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
         if self.polling_wait_seconds is not None:
             result['PollingWaitSeconds'] = self.polling_wait_seconds
         if self.queue_name is not None:
             result['QueueName'] = self.queue_name
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.visibility_timeout is not None:
             result['VisibilityTimeout'] = self.visibility_timeout
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DelaySeconds') is not None:
@@ -58,14 +101,19 @@
             self.maximum_message_size = m.get('MaximumMessageSize')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
         if m.get('PollingWaitSeconds') is not None:
             self.polling_wait_seconds = m.get('PollingWaitSeconds')
         if m.get('QueueName') is not None:
             self.queue_name = m.get('QueueName')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateQueueRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('VisibilityTimeout') is not None:
             self.visibility_timeout = m.get('VisibilityTimeout')
         return self
 
 
 class CreateQueueResponseBodyData(TeaModel):
     def __init__(
@@ -202,48 +250,96 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateQueueResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateTopicRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateTopicRequest(TeaModel):
     def __init__(
         self,
         enable_logging: bool = None,
         max_message_size: int = None,
+        tag: List[CreateTopicRequestTag] = None,
         topic_name: str = None,
     ):
         self.enable_logging = enable_logging
         self.max_message_size = max_message_size
+        self.tag = tag
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.enable_logging is not None:
             result['EnableLogging'] = self.enable_logging
         if self.max_message_size is not None:
             result['MaxMessageSize'] = self.max_message_size
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('EnableLogging') is not None:
             self.enable_logging = m.get('EnableLogging')
         if m.get('MaxMessageSize') is not None:
             self.max_message_size = m.get('MaxMessageSize')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateTopicRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
 class CreateTopicResponseBodyData(TeaModel):
     def __init__(
@@ -385,14 +481,15 @@
 
 
 class DeleteQueueRequest(TeaModel):
     def __init__(
         self,
         queue_name: str = None,
     ):
+        # This parameter is required.
         self.queue_name = queue_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -551,14 +648,15 @@
 
 
 class DeleteTopicRequest(TeaModel):
     def __init__(
         self,
         topic_name: str = None,
     ):
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -671,38 +769,119 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteTopicResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetQueueAttributesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class GetQueueAttributesRequest(TeaModel):
     def __init__(
         self,
         queue_name: str = None,
+        tag: List[GetQueueAttributesRequestTag] = None,
     ):
+        # This parameter is required.
         self.queue_name = queue_name
+        self.tag = tag
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.queue_name is not None:
             result['QueueName'] = self.queue_name
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('QueueName') is not None:
             self.queue_name = m.get('QueueName')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = GetQueueAttributesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class GetQueueAttributesResponseBodyDataTags(TeaModel):
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
         return self
 
 
 class GetQueueAttributesResponseBodyData(TeaModel):
     def __init__(
         self,
         active_messages: int = None,
@@ -712,31 +891,36 @@
         inactive_messages: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         maximum_message_size: int = None,
         message_retention_period: int = None,
         polling_wait_seconds: int = None,
         queue_name: str = None,
+        tags: List[GetQueueAttributesResponseBodyDataTags] = None,
         visibility_timeout: int = None,
     ):
         self.active_messages = active_messages
         self.create_time = create_time
         self.delay_messages = delay_messages
         self.delay_seconds = delay_seconds
         self.inactive_messages = inactive_messages
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.maximum_message_size = maximum_message_size
         self.message_retention_period = message_retention_period
         self.polling_wait_seconds = polling_wait_seconds
         self.queue_name = queue_name
+        self.tags = tags
         self.visibility_timeout = visibility_timeout
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -758,14 +942,18 @@
             result['MaximumMessageSize'] = self.maximum_message_size
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
         if self.polling_wait_seconds is not None:
             result['PollingWaitSeconds'] = self.polling_wait_seconds
         if self.queue_name is not None:
             result['QueueName'] = self.queue_name
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         if self.visibility_timeout is not None:
             result['VisibilityTimeout'] = self.visibility_timeout
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ActiveMessages') is not None:
@@ -786,14 +974,19 @@
             self.maximum_message_size = m.get('MaximumMessageSize')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
         if m.get('PollingWaitSeconds') is not None:
             self.polling_wait_seconds = m.get('PollingWaitSeconds')
         if m.get('QueueName') is not None:
             self.queue_name = m.get('QueueName')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = GetQueueAttributesResponseBodyDataTags()
+                self.tags.append(temp_model.from_map(k))
         if m.get('VisibilityTimeout') is not None:
             self.visibility_timeout = m.get('VisibilityTimeout')
         return self
 
 
 class GetQueueAttributesResponseBody(TeaModel):
     def __init__(
@@ -897,15 +1090,17 @@
 
 class GetSubscriptionAttributesRequest(TeaModel):
     def __init__(
         self,
         subscription_name: str = None,
         topic_name: str = None,
     ):
+        # This parameter is required.
         self.subscription_name = subscription_name
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1099,62 +1294,148 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetSubscriptionAttributesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetTopicAttributesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class GetTopicAttributesRequest(TeaModel):
     def __init__(
         self,
+        tag: List[GetTopicAttributesRequestTag] = None,
         topic_name: str = None,
     ):
+        self.tag = tag
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = GetTopicAttributesRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
+class GetTopicAttributesResponseBodyDataTags(TeaModel):
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
 class GetTopicAttributesResponseBodyData(TeaModel):
     def __init__(
         self,
         create_time: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         max_message_size: int = None,
         message_count: int = None,
         message_retention_period: int = None,
+        tags: List[GetTopicAttributesResponseBodyDataTags] = None,
         topic_name: str = None,
     ):
         self.create_time = create_time
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.max_message_size = max_message_size
         self.message_count = message_count
         self.message_retention_period = message_retention_period
+        self.tags = tags
         self.topic_name = topic_name
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1166,14 +1447,18 @@
             result['LoggingEnabled'] = self.logging_enabled
         if self.max_message_size is not None:
             result['MaxMessageSize'] = self.max_message_size
         if self.message_count is not None:
             result['MessageCount'] = self.message_count
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CreateTime') is not None:
@@ -1184,14 +1469,19 @@
             self.logging_enabled = m.get('LoggingEnabled')
         if m.get('MaxMessageSize') is not None:
             self.max_message_size = m.get('MaxMessageSize')
         if m.get('MessageCount') is not None:
             self.message_count = m.get('MessageCount')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = GetTopicAttributesResponseBodyDataTags()
+                self.tags.append(temp_model.from_map(k))
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
 class GetTopicAttributesResponseBody(TeaModel):
     def __init__(
@@ -1289,50 +1579,130 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetTopicAttributesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListQueueRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class ListQueueRequest(TeaModel):
     def __init__(
         self,
         page_num: int = None,
         page_size: int = None,
         queue_name: str = None,
+        tag: List[ListQueueRequestTag] = None,
     ):
         self.page_num = page_num
         self.page_size = page_size
         self.queue_name = queue_name
+        self.tag = tag
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.page_num is not None:
             result['PageNum'] = self.page_num
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.queue_name is not None:
             result['QueueName'] = self.queue_name
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PageNum') is not None:
             self.page_num = m.get('PageNum')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('QueueName') is not None:
             self.queue_name = m.get('QueueName')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = ListQueueRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class ListQueueResponseBodyDataPageDataTags(TeaModel):
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
         return self
 
 
 class ListQueueResponseBodyDataPageData(TeaModel):
     def __init__(
         self,
         active_messages: int = None,
@@ -1342,31 +1712,36 @@
         inactive_messages: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         maximum_message_size: int = None,
         message_retention_period: int = None,
         polling_wait_seconds: int = None,
         queue_name: str = None,
+        tags: List[ListQueueResponseBodyDataPageDataTags] = None,
         visibility_timeout: int = None,
     ):
         self.active_messages = active_messages
         self.create_time = create_time
         self.delay_messages = delay_messages
         self.delay_seconds = delay_seconds
         self.inactive_messages = inactive_messages
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.maximum_message_size = maximum_message_size
         self.message_retention_period = message_retention_period
         self.polling_wait_seconds = polling_wait_seconds
         self.queue_name = queue_name
+        self.tags = tags
         self.visibility_timeout = visibility_timeout
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1388,14 +1763,18 @@
             result['MaximumMessageSize'] = self.maximum_message_size
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
         if self.polling_wait_seconds is not None:
             result['PollingWaitSeconds'] = self.polling_wait_seconds
         if self.queue_name is not None:
             result['QueueName'] = self.queue_name
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         if self.visibility_timeout is not None:
             result['VisibilityTimeout'] = self.visibility_timeout
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ActiveMessages') is not None:
@@ -1416,14 +1795,19 @@
             self.maximum_message_size = m.get('MaximumMessageSize')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
         if m.get('PollingWaitSeconds') is not None:
             self.polling_wait_seconds = m.get('PollingWaitSeconds')
         if m.get('QueueName') is not None:
             self.queue_name = m.get('QueueName')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = ListQueueResponseBodyDataPageDataTags()
+                self.tags.append(temp_model.from_map(k))
         if m.get('VisibilityTimeout') is not None:
             self.visibility_timeout = m.get('VisibilityTimeout')
         return self
 
 
 class ListQueueResponseBodyData(TeaModel):
     def __init__(
@@ -1597,14 +1981,15 @@
         page_size: int = None,
         subscription_name: str = None,
         topic_name: str = None,
     ):
         self.page_num = page_num
         self.page_size = page_size
         self.subscription_name = subscription_name
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1871,78 +2256,163 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListSubscriptionByTopicResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTopicRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class ListTopicRequest(TeaModel):
     def __init__(
         self,
         page_num: int = None,
         page_size: int = None,
+        tag: List[ListTopicRequestTag] = None,
         topic_name: str = None,
     ):
         self.page_num = page_num
         self.page_size = page_size
+        self.tag = tag
         self.topic_name = topic_name
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.page_num is not None:
             result['PageNum'] = self.page_num
         if self.page_size is not None:
             result['PageSize'] = self.page_size
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PageNum') is not None:
             self.page_num = m.get('PageNum')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = ListTopicRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         return self
 
 
+class ListTopicResponseBodyDataPageDataTags(TeaModel):
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
 class ListTopicResponseBodyDataPageData(TeaModel):
     def __init__(
         self,
         create_time: int = None,
         last_modify_time: int = None,
         logging_enabled: bool = None,
         max_message_size: int = None,
         message_count: int = None,
         message_retention_period: int = None,
+        tags: List[ListTopicResponseBodyDataPageDataTags] = None,
         topic_inner_url: str = None,
         topic_name: str = None,
         topic_url: str = None,
     ):
         self.create_time = create_time
         self.last_modify_time = last_modify_time
         self.logging_enabled = logging_enabled
         self.max_message_size = max_message_size
         self.message_count = message_count
         self.message_retention_period = message_retention_period
+        self.tags = tags
         self.topic_inner_url = topic_inner_url
         self.topic_name = topic_name
         self.topic_url = topic_url
 
     def validate(self):
-        pass
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1954,14 +2424,18 @@
             result['LoggingEnabled'] = self.logging_enabled
         if self.max_message_size is not None:
             result['MaxMessageSize'] = self.max_message_size
         if self.message_count is not None:
             result['MessageCount'] = self.message_count
         if self.message_retention_period is not None:
             result['MessageRetentionPeriod'] = self.message_retention_period
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
         if self.topic_inner_url is not None:
             result['TopicInnerUrl'] = self.topic_inner_url
         if self.topic_name is not None:
             result['TopicName'] = self.topic_name
         if self.topic_url is not None:
             result['TopicUrl'] = self.topic_url
         return result
@@ -1976,14 +2450,19 @@
             self.logging_enabled = m.get('LoggingEnabled')
         if m.get('MaxMessageSize') is not None:
             self.max_message_size = m.get('MaxMessageSize')
         if m.get('MessageCount') is not None:
             self.message_count = m.get('MessageCount')
         if m.get('MessageRetentionPeriod') is not None:
             self.message_retention_period = m.get('MessageRetentionPeriod')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = ListTopicResponseBodyDataPageDataTags()
+                self.tags.append(temp_model.from_map(k))
         if m.get('TopicInnerUrl') is not None:
             self.topic_inner_url = m.get('TopicInnerUrl')
         if m.get('TopicName') is not None:
             self.topic_name = m.get('TopicName')
         if m.get('TopicUrl') is not None:
             self.topic_url = m.get('TopicUrl')
         return self
@@ -2154,14 +2633,15 @@
         visibility_timeout: int = None,
     ):
         self.delay_seconds = delay_seconds
         self.enable_logging = enable_logging
         self.maximum_message_size = maximum_message_size
         self.message_retention_period = message_retention_period
         self.polling_wait_seconds = polling_wait_seconds
+        # This parameter is required.
         self.queue_name = queue_name
         self.visibility_timeout = visibility_timeout
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2348,15 +2828,17 @@
     def __init__(
         self,
         notify_strategy: str = None,
         subscription_name: str = None,
         topic_name: str = None,
     ):
         self.notify_strategy = notify_strategy
+        # This parameter is required.
         self.subscription_name = subscription_name
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2527,14 +3009,15 @@
         self,
         enable_logging: bool = None,
         max_message_size: int = None,
         topic_name: str = None,
     ):
         self.enable_logging = enable_logging
         self.max_message_size = max_message_size
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2707,20 +3190,24 @@
         message_tag: str = None,
         notify_content_format: str = None,
         notify_strategy: str = None,
         push_type: str = None,
         subscription_name: str = None,
         topic_name: str = None,
     ):
+        # This parameter is required.
         self.endpoint = endpoint
         self.message_tag = message_tag
         self.notify_content_format = notify_content_format
         self.notify_strategy = notify_strategy
+        # This parameter is required.
         self.push_type = push_type
+        # This parameter is required.
         self.subscription_name = subscription_name
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2863,15 +3350,17 @@
 
 class UnsubscribeRequest(TeaModel):
     def __init__(
         self,
         subscription_name: str = None,
         topic_name: str = None,
     ):
+        # This parameter is required.
         self.subscription_name = subscription_name
+        # This parameter is required.
         self.topic_name = topic_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_mns-open20220119-1.0.2/alibabacloud_mns_open20220119.egg-info/PKG-INFO` & `alibabacloud_mns-open20220119-1.0.3/alibabacloud_mns_open20220119.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mns-open20220119
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Mns-open (20220119) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mns-open20220119-1.0.2/setup.py` & `alibabacloud_mns-open20220119-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mns-open20220119.
 
-Created on 08/05/2024
+Created on 27/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mns_open20220119"
 NAME = "alibabacloud_mns-open20220119" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Mns-open (20220119) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

