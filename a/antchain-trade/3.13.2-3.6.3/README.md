# Comparing `tmp/antchain_trade-3.13.2.tar.gz` & `tmp/antchain_trade-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_trade-3.13.2.tar", last modified: Mon May 27 10:09:19 2024, max compression
+gzip compressed data, was "dist/antchain_trade-3.6.3.tar", last modified: Mon Sep 13 02:21:05 2021, max compression
```

## Comparing `antchain_trade-3.13.2.tar` & `antchain_trade-3.6.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2175 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      810 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      996 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/antchain_sdk_trade/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/antchain_sdk_trade/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49148 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/antchain_sdk_trade/client.py
--rw-r--r--   0 root         (0) root         (0)   132061 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/antchain_sdk_trade/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/antchain_trade.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2175 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/antchain_trade.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      339 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/antchain_trade.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/antchain_trade.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/antchain_trade.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/antchain_trade.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-27 10:09:19.000000 antchain_trade-3.13.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2499 2024-05-27 10:09:18.000000 antchain_trade-3.13.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2182 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      818 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1004 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/antchain_sdk_trade/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/antchain_sdk_trade/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44486 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/antchain_sdk_trade/client.py
+-rw-r--r--   0 root         (0) root         (0)   114033 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/antchain_sdk_trade/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/antchain_trade.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2182 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/antchain_trade.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      339 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/antchain_trade.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/antchain_trade.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/antchain_trade.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/antchain_trade.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-09-13 02:21:05.000000 antchain_trade-3.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2498 2021-09-13 02:21:04.000000 antchain_trade-3.6.3/setup.py
```

### Comparing `antchain_trade-3.13.2/LICENSE` & `antchain_trade-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_trade-3.13.2/PKG-INFO` & `antchain_trade-3.6.3/antchain_trade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_trade
-Version: 3.13.2
+Name: antchain-trade
+Version: 3.6.3
 Summary: Ant Chain TRADE SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain-trade
-        pip install antchain-trade
+        # Install the antchain_sdk_trade
+        pip install antchain_sdk_trade
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_trade-3.13.2/README-CN.md` & `antchain_trade-3.6.3/README-CN.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain-trade
-pip install antchain-trade
+# 安装 antchain_sdk_trade
+pip install antchain_sdk_trade
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_trade-3.13.2/README.md` & `antchain_trade-3.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain-trade
-pip install antchain-trade
+# Install the antchain_sdk_trade
+pip install antchain_sdk_trade
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_trade-3.13.2/antchain_sdk_trade/client.py` & `antchain_trade-3.6.3/antchain_sdk_trade/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDuration': self._keep_alive_duration_millis,
+            'keepAliveDurationMillis': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,17 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '3.13.2',
-                    '_prod_code': 'TRADE',
-                    '_prod_channel': 'undefined'
+                    'sdk_version': '3.6.3'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -198,15 +196,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDuration': self._keep_alive_duration_millis,
+            'keepAliveDurationMillis': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -235,17 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '3.13.2',
-                    '_prod_code': 'TRADE',
-                    '_prod_channel': 'undefined'
+                    'sdk_version': '3.6.3'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -306,32 +302,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryInstanceCapacityResponse:
         """
         Description: 查询租户实例容量信息
         Summary: 查询租户实例容量信息
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryInstanceCapacityResponse(),
+        return trade_models.QueryInstanceCapacityResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.instance.capacity.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_instance_capacity_ex_async(
         self,
         request: trade_models.QueryInstanceCapacityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryInstanceCapacityResponse:
         """
         Description: 查询租户实例容量信息
         Summary: 查询租户实例容量信息
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryInstanceCapacityResponse(),
+        return trade_models.QueryInstanceCapacityResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.instance.capacity.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_marketing_coupon(
         self,
         request: trade_models.QueryMarketingCouponRequest,
     ) -> trade_models.QueryMarketingCouponResponse:
@@ -362,32 +356,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryMarketingCouponResponse:
         """
         Description: 优惠券列表查询接口
         Summary: 优惠券列表查询接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryMarketingCouponResponse(),
+        return trade_models.QueryMarketingCouponResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.marketing.coupon.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_marketing_coupon_ex_async(
         self,
         request: trade_models.QueryMarketingCouponRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryMarketingCouponResponse:
         """
         Description: 优惠券列表查询接口
         Summary: 优惠券列表查询接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryMarketingCouponResponse(),
+        return trade_models.QueryMarketingCouponResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.marketing.coupon.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def send_marketing_coupon(
         self,
         request: trade_models.SendMarketingCouponRequest,
     ) -> trade_models.SendMarketingCouponResponse:
@@ -418,32 +410,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.SendMarketingCouponResponse:
         """
         Description: 优惠券发放接口，基于模板ID发送优惠券
         Summary: 优惠券发放接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.SendMarketingCouponResponse(),
+        return trade_models.SendMarketingCouponResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.marketing.coupon.send', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def send_marketing_coupon_ex_async(
         self,
         request: trade_models.SendMarketingCouponRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.SendMarketingCouponResponse:
         """
         Description: 优惠券发放接口，基于模板ID发送优惠券
         Summary: 优惠券发放接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.SendMarketingCouponResponse(),
+        return trade_models.SendMarketingCouponResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.marketing.coupon.send', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_order_after(
         self,
         request: trade_models.CreateOrderAfterRequest,
     ) -> trade_models.CreateOrderAfterResponse:
@@ -474,32 +464,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateOrderAfterResponse:
         """
         Description: 开通类商品自动下单接口，仅仅针对其下后付开通类商品。预付等涉及金额暂不支持。
         Summary: 开通类商品自动下单接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateOrderAfterResponse(),
+        return trade_models.CreateOrderAfterResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.order.after.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_order_after_ex_async(
         self,
         request: trade_models.CreateOrderAfterRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateOrderAfterResponse:
         """
         Description: 开通类商品自动下单接口，仅仅针对其下后付开通类商品。预付等涉及金额暂不支持。
         Summary: 开通类商品自动下单接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateOrderAfterResponse(),
+        return trade_models.CreateOrderAfterResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.order.after.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_order_workflow(
         self,
         request: trade_models.CreateOrderWorkflowRequest,
     ) -> trade_models.CreateOrderWorkflowResponse:
@@ -530,32 +518,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateOrderWorkflowResponse:
         """
         Description: 流程编排，创建商品开通接口
         Summary: 能力编排-商品开通
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateOrderWorkflowResponse(),
+        return trade_models.CreateOrderWorkflowResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.order.workflow.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_order_workflow_ex_async(
         self,
         request: trade_models.CreateOrderWorkflowRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateOrderWorkflowResponse:
         """
         Description: 流程编排，创建商品开通接口
         Summary: 能力编排-商品开通
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateOrderWorkflowResponse(),
+        return trade_models.CreateOrderWorkflowResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.order.workflow.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def get_combo(
         self,
         request: trade_models.GetComboRequest,
     ) -> trade_models.GetComboResponse:
@@ -586,32 +572,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.GetComboResponse:
         """
         Description: 获取套餐详情接口
         Summary: 获取套餐详情
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.GetComboResponse(),
+        return trade_models.GetComboResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.combo.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def get_combo_ex_async(
         self,
         request: trade_models.GetComboRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.GetComboResponse:
         """
         Description: 获取套餐详情接口
         Summary: 获取套餐详情
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.GetComboResponse(),
+        return trade_models.GetComboResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.combo.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_combo_price(
         self,
         request: trade_models.QueryComboPriceRequest,
     ) -> trade_models.QueryComboPriceResponse:
@@ -642,32 +626,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryComboPriceResponse:
         """
         Description: 套餐询价接口
         Summary: 套餐询价接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryComboPriceResponse(),
+        return trade_models.QueryComboPriceResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.combo.price.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_combo_price_ex_async(
         self,
         request: trade_models.QueryComboPriceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryComboPriceResponse:
         """
         Description: 套餐询价接口
         Summary: 套餐询价接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryComboPriceResponse(),
+        return trade_models.QueryComboPriceResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.combo.price.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_combo_order(
         self,
         request: trade_models.CreateComboOrderRequest,
     ) -> trade_models.CreateComboOrderResponse:
@@ -698,32 +680,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateComboOrderResponse:
         """
         Description: 套餐下单接口，支持部分渠道的自动支付
         Summary: 套餐下单接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateComboOrderResponse(),
+        return trade_models.CreateComboOrderResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.combo.order.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_combo_order_ex_async(
         self,
         request: trade_models.CreateComboOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateComboOrderResponse:
         """
         Description: 套餐下单接口，支持部分渠道的自动支付
         Summary: 套餐下单接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateComboOrderResponse(),
+        return trade_models.CreateComboOrderResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.combo.order.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_combo_order(
         self,
         request: trade_models.QueryComboOrderRequest,
     ) -> trade_models.QueryComboOrderResponse:
@@ -754,32 +734,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryComboOrderResponse:
         """
         Description: 套餐订单列表分页查询接口
         Summary: 套餐订单列表分页查询接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryComboOrderResponse(),
+        return trade_models.QueryComboOrderResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.combo.order.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_combo_order_ex_async(
         self,
         request: trade_models.QueryComboOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryComboOrderResponse:
         """
         Description: 套餐订单列表分页查询接口
         Summary: 套餐订单列表分页查询接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryComboOrderResponse(),
+        return trade_models.QueryComboOrderResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.combo.order.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_combo(
         self,
         request: trade_models.QueryComboRequest,
     ) -> trade_models.QueryComboResponse:
@@ -810,32 +788,30 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryComboResponse:
         """
         Description: 查询套餐列表，支持分页查询
         Summary: 查询套餐列表
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryComboResponse(),
+        return trade_models.QueryComboResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.combo.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_combo_ex_async(
         self,
         request: trade_models.QueryComboRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryComboResponse:
         """
         Description: 查询套餐列表，支持分页查询
         Summary: 查询套餐列表
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryComboResponse(),
+        return trade_models.QueryComboResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.combo.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def pay_combo_order(
         self,
         request: trade_models.PayComboOrderRequest,
     ) -> trade_models.PayComboOrderResponse:
@@ -866,203 +842,87 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.PayComboOrderResponse:
         """
         Description: 套餐订单支付接口
         Summary: 套餐订单支付接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.PayComboOrderResponse(),
+        return trade_models.PayComboOrderResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.combo.order.pay', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def pay_combo_order_ex_async(
         self,
         request: trade_models.PayComboOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.PayComboOrderResponse:
         """
         Description: 套餐订单支付接口
         Summary: 套餐订单支付接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.PayComboOrderResponse(),
+        return trade_models.PayComboOrderResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.combo.order.pay', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_order(
         self,
         request: trade_models.CreateOrderRequest,
     ) -> trade_models.CreateOrderResponse:
         """
-        Description: 单商品通用下单接口
+        Description: 通用下单接口，支持单商品下单，支持0元订单自动支付
         Summary: 通用下单接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_order_ex(request, headers, runtime)
 
     async def create_order_async(
         self,
         request: trade_models.CreateOrderRequest,
     ) -> trade_models.CreateOrderResponse:
         """
-        Description: 单商品通用下单接口
+        Description: 通用下单接口，支持单商品下单，支持0元订单自动支付
         Summary: 通用下单接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_order_ex_async(request, headers, runtime)
 
     def create_order_ex(
         self,
         request: trade_models.CreateOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateOrderResponse:
         """
-        Description: 单商品通用下单接口
+        Description: 通用下单接口，支持单商品下单，支持0元订单自动支付
         Summary: 通用下单接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateOrderResponse(),
+        return trade_models.CreateOrderResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.order.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def create_order_ex_async(
         self,
         request: trade_models.CreateOrderRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.CreateOrderResponse:
         """
-        Description: 单商品通用下单接口
+        Description: 通用下单接口，支持单商品下单，支持0元订单自动支付
         Summary: 通用下单接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CreateOrderResponse(),
+        return trade_models.CreateOrderResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.order.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def get_combo_order(
-        self,
-        request: trade_models.GetComboOrderRequest,
-    ) -> trade_models.GetComboOrderResponse:
-        """
-        Description: 套餐订单详情查询接口
-        Summary: 套餐订单详情查询接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.get_combo_order_ex(request, headers, runtime)
-
-    async def get_combo_order_async(
-        self,
-        request: trade_models.GetComboOrderRequest,
-    ) -> trade_models.GetComboOrderResponse:
-        """
-        Description: 套餐订单详情查询接口
-        Summary: 套餐订单详情查询接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.get_combo_order_ex_async(request, headers, runtime)
-
-    def get_combo_order_ex(
-        self,
-        request: trade_models.GetComboOrderRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> trade_models.GetComboOrderResponse:
-        """
-        Description: 套餐订单详情查询接口
-        Summary: 套餐订单详情查询接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.GetComboOrderResponse(),
-            self.do_request('1.0', 'antcloud.trade.combo.order.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def get_combo_order_ex_async(
-        self,
-        request: trade_models.GetComboOrderRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> trade_models.GetComboOrderResponse:
-        """
-        Description: 套餐订单详情查询接口
-        Summary: 套餐订单详情查询接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.GetComboOrderResponse(),
-            await self.do_request_async('1.0', 'antcloud.trade.combo.order.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def cancel_order(
-        self,
-        request: trade_models.CancelOrderRequest,
-    ) -> trade_models.CancelOrderResponse:
-        """
-        Description: 取消下单接口
-        Summary: 取消下单接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.cancel_order_ex(request, headers, runtime)
-
-    async def cancel_order_async(
-        self,
-        request: trade_models.CancelOrderRequest,
-    ) -> trade_models.CancelOrderResponse:
-        """
-        Description: 取消下单接口
-        Summary: 取消下单接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.cancel_order_ex_async(request, headers, runtime)
-
-    def cancel_order_ex(
-        self,
-        request: trade_models.CancelOrderRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> trade_models.CancelOrderResponse:
-        """
-        Description: 取消下单接口
-        Summary: 取消下单接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CancelOrderResponse(),
-            self.do_request('1.0', 'antcloud.trade.order.cancel', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def cancel_order_ex_async(
-        self,
-        request: trade_models.CancelOrderRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> trade_models.CancelOrderResponse:
-        """
-        Description: 取消下单接口
-        Summary: 取消下单接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.CancelOrderResponse(),
-            await self.do_request_async('1.0', 'antcloud.trade.order.cancel', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
     def exist_price_personalized(
         self,
         request: trade_models.ExistPricePersonalizedRequest,
     ) -> trade_models.ExistPricePersonalizedResponse:
         """
         Description: 仅支持查询租户在后付费商品下，是否存在个性化定价
         Summary: 判断租户是否存在个性化定价
@@ -1090,88 +950,84 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.ExistPricePersonalizedResponse:
         """
         Description: 仅支持查询租户在后付费商品下，是否存在个性化定价
         Summary: 判断租户是否存在个性化定价
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.ExistPricePersonalizedResponse(),
+        return trade_models.ExistPricePersonalizedResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.price.personalized.exist', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def exist_price_personalized_ex_async(
         self,
         request: trade_models.ExistPricePersonalizedRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.ExistPricePersonalizedResponse:
         """
         Description: 仅支持查询租户在后付费商品下，是否存在个性化定价
         Summary: 判断租户是否存在个性化定价
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.ExistPricePersonalizedResponse(),
+        return trade_models.ExistPricePersonalizedResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.price.personalized.exist', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_price(
         self,
         request: trade_models.QueryPriceRequest,
     ) -> trade_models.QueryPriceResponse:
         """
-        Description: 单商品询价接口，支持抵扣优惠券和命中折扣活动
+        Description: 单商品询价接口，支持抵扣优惠券和命中优惠券
         Summary: 商品询价接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.query_price_ex(request, headers, runtime)
 
     async def query_price_async(
         self,
         request: trade_models.QueryPriceRequest,
     ) -> trade_models.QueryPriceResponse:
         """
-        Description: 单商品询价接口，支持抵扣优惠券和命中折扣活动
+        Description: 单商品询价接口，支持抵扣优惠券和命中优惠券
         Summary: 商品询价接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.query_price_ex_async(request, headers, runtime)
 
     def query_price_ex(
         self,
         request: trade_models.QueryPriceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryPriceResponse:
         """
-        Description: 单商品询价接口，支持抵扣优惠券和命中折扣活动
+        Description: 单商品询价接口，支持抵扣优惠券和命中优惠券
         Summary: 商品询价接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryPriceResponse(),
+        return trade_models.QueryPriceResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.price.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_price_ex_async(
         self,
         request: trade_models.QueryPriceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryPriceResponse:
         """
-        Description: 单商品询价接口，支持抵扣优惠券和命中折扣活动
+        Description: 单商品询价接口，支持抵扣优惠券和命中优惠券
         Summary: 商品询价接口
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryPriceResponse(),
+        return trade_models.QueryPriceResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.price.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_wareslife_instance(
         self,
         request: trade_models.QueryWareslifeInstanceRequest,
     ) -> trade_models.QueryWareslifeInstanceResponse:
@@ -1202,27 +1058,25 @@
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryWareslifeInstanceResponse:
         """
         Description: 实例接口查询
         Summary: 实例接口查询
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryWareslifeInstanceResponse(),
+        return trade_models.QueryWareslifeInstanceResponse().from_map(
             self.do_request('1.0', 'antcloud.trade.wareslife.instance.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_wareslife_instance_ex_async(
         self,
         request: trade_models.QueryWareslifeInstanceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> trade_models.QueryWareslifeInstanceResponse:
         """
         Description: 实例接口查询
         Summary: 实例接口查询
         """
         UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            trade_models.QueryWareslifeInstanceResponse(),
+        return trade_models.QueryWareslifeInstanceResponse().from_map(
             await self.do_request_async('1.0', 'antcloud.trade.wareslife.instance.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

### Comparing `antchain_trade-3.13.2/antchain_sdk_trade/models.py` & `antchain_trade-3.6.3/antchain_sdk_trade/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,18 +66,14 @@
         # 每个目标主机的最大连接数（分主机域名的长链接最大总数
         self.max_requests_per_host = max_requests_per_host
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.access_key_id is not None:
             result['accessKeyId'] = self.access_key_id
         if self.access_key_secret is not None:
             result['accessKeySecret'] = self.access_key_secret
         if self.security_token is not None:
             result['securityToken'] = self.security_token
@@ -191,18 +187,14 @@
         self.validate_required(self.value_type, 'value_type')
         self.validate_required(self.value_range, 'value_range')
         self.validate_required(self.display_type, 'display_type')
         self.validate_required(self.tips, 'tips')
         self.validate_required(self.unit, 'unit')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.code is not None:
             result['code'] = self.code
         if self.name is not None:
             result['name'] = self.name
         if self.default_value is not None:
             result['default_value'] = self.default_value
@@ -235,14 +227,54 @@
         if m.get('tips') is not None:
             self.tips = m.get('tips')
         if m.get('unit') is not None:
             self.unit = m.get('unit')
         return self
 
 
+class ComboCommodityOrder(TeaModel):
+    def __init__(
+        self,
+        commodity_code: str = None,
+        status: str = None,
+        instance_ids: List[str] = None,
+    ):
+        # 商品编码
+        self.commodity_code = commodity_code
+        # 状态
+        self.status = status
+        # 实例ID列表
+        self.instance_ids = instance_ids
+
+    def validate(self):
+        self.validate_required(self.commodity_code, 'commodity_code')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.instance_ids, 'instance_ids')
+
+    def to_map(self):
+        result = dict()
+        if self.commodity_code is not None:
+            result['commodity_code'] = self.commodity_code
+        if self.status is not None:
+            result['status'] = self.status
+        if self.instance_ids is not None:
+            result['instance_ids'] = self.instance_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commodity_code') is not None:
+            self.commodity_code = m.get('commodity_code')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('instance_ids') is not None:
+            self.instance_ids = m.get('instance_ids')
+        return self
+
+
 class ComboCommodity(TeaModel):
     def __init__(
         self,
         name: str = None,
         unique_code: str = None,
         inner_code: str = None,
         type: str = None,
@@ -279,18 +311,14 @@
             for k in self.attrs:
                 if k:
                     k.validate()
         self.validate_required(self.quantity, 'quantity')
         self.validate_required(self.extends_config, 'extends_config')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.name is not None:
             result['name'] = self.name
         if self.unique_code is not None:
             result['unique_code'] = self.unique_code
         if self.inner_code is not None:
             result['inner_code'] = self.inner_code
@@ -328,478 +356,14 @@
         if m.get('quantity') is not None:
             self.quantity = m.get('quantity')
         if m.get('extends_config') is not None:
             self.extends_config = m.get('extends_config')
         return self
 
 
-class OrderDuration(TeaModel):
-    def __init__(
-        self,
-        duration_type: str = None,
-        duration_value: int = None,
-    ):
-        # 周期类型，YEAR：年；MONTH：月；DAY：日
-        self.duration_type = duration_type
-        # 订购周期值
-        self.duration_value = duration_value
-
-    def validate(self):
-        self.validate_required(self.duration_type, 'duration_type')
-        self.validate_required(self.duration_value, 'duration_value')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.duration_type is not None:
-            result['duration_type'] = self.duration_type
-        if self.duration_value is not None:
-            result['duration_value'] = self.duration_value
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('duration_type') is not None:
-            self.duration_type = m.get('duration_type')
-        if m.get('duration_value') is not None:
-            self.duration_value = m.get('duration_value')
-        return self
-
-
-class ComboCommodityOrder(TeaModel):
-    def __init__(
-        self,
-        commodity_code: str = None,
-        status: str = None,
-        instance_ids: List[str] = None,
-    ):
-        # 商品编码
-        self.commodity_code = commodity_code
-        # 状态
-        self.status = status
-        # 实例ID列表
-        self.instance_ids = instance_ids
-
-    def validate(self):
-        self.validate_required(self.commodity_code, 'commodity_code')
-        self.validate_required(self.status, 'status')
-        self.validate_required(self.instance_ids, 'instance_ids')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.commodity_code is not None:
-            result['commodity_code'] = self.commodity_code
-        if self.status is not None:
-            result['status'] = self.status
-        if self.instance_ids is not None:
-            result['instance_ids'] = self.instance_ids
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('commodity_code') is not None:
-            self.commodity_code = m.get('commodity_code')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        if m.get('instance_ids') is not None:
-            self.instance_ids = m.get('instance_ids')
-        return self
-
-
-class CommodityPricing(TeaModel):
-    def __init__(self):
-        pass
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        return self
-
-
-class InstanceLabel(TeaModel):
-    def __init__(
-        self,
-        instance_key: str = None,
-        instance_value: str = None,
-    ):
-        # 标签名。
-        # 传递isvId
-        self.instance_key = instance_key
-        # 标签值
-        self.instance_value = instance_value
-
-    def validate(self):
-        self.validate_required(self.instance_key, 'instance_key')
-        self.validate_required(self.instance_value, 'instance_value')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.instance_key is not None:
-            result['instance_key'] = self.instance_key
-        if self.instance_value is not None:
-            result['instance_value'] = self.instance_value
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('instance_key') is not None:
-            self.instance_key = m.get('instance_key')
-        if m.get('instance_value') is not None:
-            self.instance_value = m.get('instance_value')
-        return self
-
-
-class PayOptions(TeaModel):
-    def __init__(
-        self,
-        pay_channel: str = None,
-    ):
-        # 系统自动会根据账号类型、当前OU进行付费渠道判定；如果传入的付款渠道不满足，则报错
-        self.pay_channel = pay_channel
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.pay_channel is not None:
-            result['pay_channel'] = self.pay_channel
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('pay_channel') is not None:
-            self.pay_channel = m.get('pay_channel')
-        return self
-
-
-class PriceStrategy(TeaModel):
-    def __init__(
-        self,
-        follow_tenant_id: str = None,
-    ):
-        # 继承租户在商品下的价格，仅后付费商品生效
-        self.follow_tenant_id = follow_tenant_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.follow_tenant_id is not None:
-            result['follow_tenant_id'] = self.follow_tenant_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('follow_tenant_id') is not None:
-            self.follow_tenant_id = m.get('follow_tenant_id')
-        return self
-
-
-class CommodityOrderAttribute(TeaModel):
-    def __init__(
-        self,
-        code: str = None,
-        value: str = None,
-        value_unit: str = None,
-    ):
-        # 属性编码
-        self.code = code
-        # 属性值
-        self.value = value
-        # 属性值单位，部分数值型属性有多种单位，需要填入；其他情况不需要填
-        self.value_unit = value_unit
-
-    def validate(self):
-        self.validate_required(self.code, 'code')
-        self.validate_required(self.value, 'value')
-        self.validate_required(self.value_unit, 'value_unit')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['code'] = self.code
-        if self.value is not None:
-            result['value'] = self.value
-        if self.value_unit is not None:
-            result['value_unit'] = self.value_unit
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('code') is not None:
-            self.code = m.get('code')
-        if m.get('value') is not None:
-            self.value = m.get('value')
-        if m.get('value_unit') is not None:
-            self.value_unit = m.get('value_unit')
-        return self
-
-
-class PrepayAmount(TeaModel):
-    def __init__(
-        self,
-        amount: str = None,
-        currency: str = None,
-    ):
-        # 指定预付费金额
-        self.amount = amount
-        # 币种单位，CNY\USD等标准币种单位编码
-        self.currency = currency
-
-    def validate(self):
-        self.validate_required(self.amount, 'amount')
-        self.validate_required(self.currency, 'currency')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.amount is not None:
-            result['amount'] = self.amount
-        if self.currency is not None:
-            result['currency'] = self.currency
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('amount') is not None:
-            self.amount = m.get('amount')
-        if m.get('currency') is not None:
-            self.currency = m.get('currency')
-        return self
-
-
-class FulfillmentOptions(TeaModel):
-    def __init__(
-        self,
-        deplay: bool = None,
-        start_time: str = None,
-        spi_skip: bool = None,
-    ):
-        # 是否延迟履约，默认false
-        self.deplay = deplay
-        # 实际履约开始时间，默认支付完成时间；只有deplay=true时，start_time才生效
-        self.start_time = start_time
-        # 跳过SPI回调，默认false，优先级高于商品上默认的接入属性
-        self.spi_skip = spi_skip
-
-    def validate(self):
-        if self.start_time is not None:
-            self.validate_pattern(self.start_time, 'start_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.deplay is not None:
-            result['deplay'] = self.deplay
-        if self.start_time is not None:
-            result['start_time'] = self.start_time
-        if self.spi_skip is not None:
-            result['spi_skip'] = self.spi_skip
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('deplay') is not None:
-            self.deplay = m.get('deplay')
-        if m.get('start_time') is not None:
-            self.start_time = m.get('start_time')
-        if m.get('spi_skip') is not None:
-            self.spi_skip = m.get('spi_skip')
-        return self
-
-
-class CommodityEnquiryPrice(TeaModel):
-    def __init__(
-        self,
-        commodity_code: str = None,
-        commodity_name: str = None,
-        pay_amount: str = None,
-        original_amount: str = None,
-        discount_amount: str = None,
-        coupon_amount: str = None,
-        subscription_unused_amount: str = None,
-        activity_code: str = None,
-        activity_name: str = None,
-        price_plan_id: int = None,
-        price_constraint_id: int = None,
-        currency: str = None,
-        min_duration_of_valid_pay_amount: OrderDuration = None,
-        discount_rate: str = None,
-        original_bd_amount: str = None,
-        original_cost_amount: str = None,
-    ):
-        # 商品主数据编码
-        self.commodity_code = commodity_code
-        # 商品名称
-        self.commodity_name = commodity_name
-        # 预付-支付金额
-        self.pay_amount = pay_amount
-        # 预付费-原始金额
-        self.original_amount = original_amount
-        # 预付费-折扣金额
-        self.discount_amount = discount_amount
-        # 预付费-优惠券抵扣金额
-        self.coupon_amount = coupon_amount
-        # 原订购剩余价值，用于变配场景
-        self.subscription_unused_amount = subscription_unused_amount
-        # 命中的活动编码
-        self.activity_code = activity_code
-        # 命中的活动名称
-        self.activity_name = activity_name
-        # 命中的定价计划ID
-        self.price_plan_id = price_plan_id
-        # 命中的定价约束ID
-        self.price_constraint_id = price_constraint_id
-        # 币种，元：CNY
-        self.currency = currency
-        # 基于剩余价值变配场景下，预测的支付金额正常的最小订购周期
-        self.min_duration_of_valid_pay_amount = min_duration_of_valid_pay_amount
-        # 预付费-折扣率
-        self.discount_rate = discount_rate
-        # 原始BD权限价金额，白名单商品会返回此价格
-        self.original_bd_amount = original_bd_amount
-        # 原始成本价金额，白名单商品会返回此价格
-        self.original_cost_amount = original_cost_amount
-
-    def validate(self):
-        self.validate_required(self.commodity_code, 'commodity_code')
-        self.validate_required(self.commodity_name, 'commodity_name')
-        self.validate_required(self.pay_amount, 'pay_amount')
-        self.validate_required(self.original_amount, 'original_amount')
-        self.validate_required(self.discount_amount, 'discount_amount')
-        self.validate_required(self.coupon_amount, 'coupon_amount')
-        self.validate_required(self.subscription_unused_amount, 'subscription_unused_amount')
-        self.validate_required(self.activity_code, 'activity_code')
-        self.validate_required(self.activity_name, 'activity_name')
-        self.validate_required(self.price_plan_id, 'price_plan_id')
-        self.validate_required(self.price_constraint_id, 'price_constraint_id')
-        self.validate_required(self.currency, 'currency')
-        if self.min_duration_of_valid_pay_amount:
-            self.min_duration_of_valid_pay_amount.validate()
-        self.validate_required(self.discount_rate, 'discount_rate')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.commodity_code is not None:
-            result['commodity_code'] = self.commodity_code
-        if self.commodity_name is not None:
-            result['commodity_name'] = self.commodity_name
-        if self.pay_amount is not None:
-            result['pay_amount'] = self.pay_amount
-        if self.original_amount is not None:
-            result['original_amount'] = self.original_amount
-        if self.discount_amount is not None:
-            result['discount_amount'] = self.discount_amount
-        if self.coupon_amount is not None:
-            result['coupon_amount'] = self.coupon_amount
-        if self.subscription_unused_amount is not None:
-            result['subscription_unused_amount'] = self.subscription_unused_amount
-        if self.activity_code is not None:
-            result['activity_code'] = self.activity_code
-        if self.activity_name is not None:
-            result['activity_name'] = self.activity_name
-        if self.price_plan_id is not None:
-            result['price_plan_id'] = self.price_plan_id
-        if self.price_constraint_id is not None:
-            result['price_constraint_id'] = self.price_constraint_id
-        if self.currency is not None:
-            result['currency'] = self.currency
-        if self.min_duration_of_valid_pay_amount is not None:
-            result['min_duration_of_valid_pay_amount'] = self.min_duration_of_valid_pay_amount.to_map()
-        if self.discount_rate is not None:
-            result['discount_rate'] = self.discount_rate
-        if self.original_bd_amount is not None:
-            result['original_bd_amount'] = self.original_bd_amount
-        if self.original_cost_amount is not None:
-            result['original_cost_amount'] = self.original_cost_amount
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('commodity_code') is not None:
-            self.commodity_code = m.get('commodity_code')
-        if m.get('commodity_name') is not None:
-            self.commodity_name = m.get('commodity_name')
-        if m.get('pay_amount') is not None:
-            self.pay_amount = m.get('pay_amount')
-        if m.get('original_amount') is not None:
-            self.original_amount = m.get('original_amount')
-        if m.get('discount_amount') is not None:
-            self.discount_amount = m.get('discount_amount')
-        if m.get('coupon_amount') is not None:
-            self.coupon_amount = m.get('coupon_amount')
-        if m.get('subscription_unused_amount') is not None:
-            self.subscription_unused_amount = m.get('subscription_unused_amount')
-        if m.get('activity_code') is not None:
-            self.activity_code = m.get('activity_code')
-        if m.get('activity_name') is not None:
-            self.activity_name = m.get('activity_name')
-        if m.get('price_plan_id') is not None:
-            self.price_plan_id = m.get('price_plan_id')
-        if m.get('price_constraint_id') is not None:
-            self.price_constraint_id = m.get('price_constraint_id')
-        if m.get('currency') is not None:
-            self.currency = m.get('currency')
-        if m.get('min_duration_of_valid_pay_amount') is not None:
-            temp_model = OrderDuration()
-            self.min_duration_of_valid_pay_amount = temp_model.from_map(m['min_duration_of_valid_pay_amount'])
-        if m.get('discount_rate') is not None:
-            self.discount_rate = m.get('discount_rate')
-        if m.get('original_bd_amount') is not None:
-            self.original_bd_amount = m.get('original_bd_amount')
-        if m.get('original_cost_amount') is not None:
-            self.original_cost_amount = m.get('original_cost_amount')
-        return self
-
-
 class Combo(TeaModel):
     def __init__(
         self,
         code: str = None,
         name: str = None,
         vid: str = None,
         description: str = None,
@@ -832,18 +396,14 @@
         self.validate_required(self.commodities, 'commodities')
         if self.commodities:
             for k in self.commodities:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.code is not None:
             result['code'] = self.code
         if self.name is not None:
             result['name'] = self.name
         if self.vid is not None:
             result['vid'] = self.vid
@@ -921,18 +481,14 @@
         if self.end_time is not None:
             self.validate_pattern(self.end_time, 'end_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         self.validate_required(self.status, 'status')
         self.validate_required(self.commodity_code, 'commodity_code')
         self.validate_required(self.rel_postpay_commodity, 'rel_postpay_commodity')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.instance_id is not None:
             result['instance_id'] = self.instance_id
         if self.current_capacity is not None:
             result['current_capacity'] = self.current_capacity
         if self.initial_capacity is not None:
             result['initial_capacity'] = self.initial_capacity
@@ -965,147 +521,27 @@
         if m.get('commodity_code') is not None:
             self.commodity_code = m.get('commodity_code')
         if m.get('rel_postpay_commodity') is not None:
             self.rel_postpay_commodity = m.get('rel_postpay_commodity')
         return self
 
 
-class Instance(TeaModel):
-    def __init__(
-        self,
-        tenant_id: str = None,
-        instance_id: str = None,
-        product_name: str = None,
-        charge_type: str = None,
-        status: str = None,
-    ):
-        # 租户id
-        self.tenant_id = tenant_id
-        # 实例id
-        self.instance_id = instance_id
-        # 商品code
-        self.product_name = product_name
-        # 付费类型 PREPAY_BY_MONTH 预付 AFTER_PAY_BY_HOUR 后付 MIX_PAY 混合付
-        self.charge_type = charge_type
-        # 状态 CREATING 创建中 FAILED 创建失败  STARTED 运行中 STOPPED 已停服  RELEASED 已释放
-        self.status = status
-
-    def validate(self):
-        self.validate_required(self.tenant_id, 'tenant_id')
-        self.validate_required(self.instance_id, 'instance_id')
-        self.validate_required(self.product_name, 'product_name')
-        self.validate_required(self.charge_type, 'charge_type')
-        self.validate_required(self.status, 'status')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.tenant_id is not None:
-            result['tenant_id'] = self.tenant_id
-        if self.instance_id is not None:
-            result['instance_id'] = self.instance_id
-        if self.product_name is not None:
-            result['product_name'] = self.product_name
-        if self.charge_type is not None:
-            result['charge_type'] = self.charge_type
-        if self.status is not None:
-            result['status'] = self.status
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('tenant_id') is not None:
-            self.tenant_id = m.get('tenant_id')
-        if m.get('instance_id') is not None:
-            self.instance_id = m.get('instance_id')
-        if m.get('product_name') is not None:
-            self.product_name = m.get('product_name')
-        if m.get('charge_type') is not None:
-            self.charge_type = m.get('charge_type')
-        if m.get('status') is not None:
-            self.status = m.get('status')
-        return self
-
-
-class CreateOrderResult(TeaModel):
-    def __init__(
-        self,
-        bsn_no: str = None,
-        order_id: str = None,
-        normal_order_line_id: str = None,
-        order_status: str = None,
-        instance_ids: str = None,
-        order_error_code: str = None,
-        order_error_description: str = None,
-    ):
-        # 下单时指定的业务流水号。二级订单号
-        self.bsn_no = bsn_no
-        # 一级订单号
-        self.order_id = order_id
-        # 二级订单号
-        self.normal_order_line_id = normal_order_line_id
-        # 订单状态
-        self.order_status = order_status
-        # 实例列表
-        self.instance_ids = instance_ids
-        # 订购错误码
-        self.order_error_code = order_error_code
-        # 订购错误描述
-        self.order_error_description = order_error_description
+class CommodityPricing(TeaModel):
+    def __init__(self):
+        pass
 
     def validate(self):
-        self.validate_required(self.bsn_no, 'bsn_no')
-        self.validate_required(self.order_id, 'order_id')
-        self.validate_required(self.normal_order_line_id, 'normal_order_line_id')
-        self.validate_required(self.order_status, 'order_status')
-        self.validate_required(self.instance_ids, 'instance_ids')
-        self.validate_required(self.order_error_code, 'order_error_code')
-        self.validate_required(self.order_error_description, 'order_error_description')
+        pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
-        if self.bsn_no is not None:
-            result['bsn_no'] = self.bsn_no
-        if self.order_id is not None:
-            result['order_id'] = self.order_id
-        if self.normal_order_line_id is not None:
-            result['normal_order_line_id'] = self.normal_order_line_id
-        if self.order_status is not None:
-            result['order_status'] = self.order_status
-        if self.instance_ids is not None:
-            result['instance_ids'] = self.instance_ids
-        if self.order_error_code is not None:
-            result['order_error_code'] = self.order_error_code
-        if self.order_error_description is not None:
-            result['order_error_description'] = self.order_error_description
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('bsn_no') is not None:
-            self.bsn_no = m.get('bsn_no')
-        if m.get('order_id') is not None:
-            self.order_id = m.get('order_id')
-        if m.get('normal_order_line_id') is not None:
-            self.normal_order_line_id = m.get('normal_order_line_id')
-        if m.get('order_status') is not None:
-            self.order_status = m.get('order_status')
-        if m.get('instance_ids') is not None:
-            self.instance_ids = m.get('instance_ids')
-        if m.get('order_error_code') is not None:
-            self.order_error_code = m.get('order_error_code')
-        if m.get('order_error_description') is not None:
-            self.order_error_description = m.get('order_error_description')
         return self
 
 
 class Coupon(TeaModel):
     def __init__(
         self,
         id: int = None,
@@ -1133,15 +569,15 @@
         self.display_name = display_name
         # 优惠券模板名称
         # 
         self.name = name
         # 优惠券类型，VOUCHER：抵用券;CERTAIN：满减券；DISCOUNT：折扣券
         # 
         self.type = type
-        # 优惠券总金额，单位（分）。可使用金额需要根据 amount - usedAmount 得出
+        # 优惠券金额，单位（分）
         # 
         self.amount_in_cent = amount_in_cent
         # 已使用金额，单位(分）
         # 
         self.used_amount_in_cent = used_amount_in_cent
         # 状态，AVAILABLE-有效/EXPIRED-已过期/EXHAUSTED-已用完/ABANDONED-已作废
         # 
@@ -1188,18 +624,14 @@
         self.validate_required(self.youhui_template_id, 'youhui_template_id')
         self.validate_required(self.usage_count, 'usage_count')
         self.validate_required(self.used_count, 'used_count')
         self.validate_required(self.product_list, 'product_list')
         self.validate_required(self.order_type_list, 'order_type_list')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.id is not None:
             result['id'] = self.id
         if self.display_name is not None:
             result['display_name'] = self.display_name
         if self.name is not None:
             result['name'] = self.name
@@ -1264,14 +696,350 @@
         if m.get('product_list') is not None:
             self.product_list = m.get('product_list')
         if m.get('order_type_list') is not None:
             self.order_type_list = m.get('order_type_list')
         return self
 
 
+class CommodityEnquiryPrice(TeaModel):
+    def __init__(
+        self,
+        commodity_code: str = None,
+        commodity_name: str = None,
+        pay_amount: str = None,
+        original_amount: str = None,
+        discount_amount: str = None,
+        activity_code: str = None,
+        activity_name: str = None,
+        price_plan_id: int = None,
+        price_constraint_id: int = None,
+        currency: str = None,
+    ):
+        # 商品主数据编码
+        self.commodity_code = commodity_code
+        # 商品名称
+        self.commodity_name = commodity_name
+        # 预付-支付金额
+        self.pay_amount = pay_amount
+        # 预付费-原始金额
+        self.original_amount = original_amount
+        # 预付费-折扣金额
+        self.discount_amount = discount_amount
+        # 命中的活动编码
+        self.activity_code = activity_code
+        # 命中的活动名称
+        self.activity_name = activity_name
+        # 命中的定价计划ID
+        self.price_plan_id = price_plan_id
+        # 命中的定价约束ID
+        self.price_constraint_id = price_constraint_id
+        # 币种，元：CNY
+        self.currency = currency
+
+    def validate(self):
+        self.validate_required(self.commodity_code, 'commodity_code')
+        self.validate_required(self.commodity_name, 'commodity_name')
+        self.validate_required(self.pay_amount, 'pay_amount')
+        self.validate_required(self.original_amount, 'original_amount')
+        self.validate_required(self.discount_amount, 'discount_amount')
+        self.validate_required(self.activity_code, 'activity_code')
+        self.validate_required(self.activity_name, 'activity_name')
+        self.validate_required(self.price_plan_id, 'price_plan_id')
+        self.validate_required(self.price_constraint_id, 'price_constraint_id')
+        self.validate_required(self.currency, 'currency')
+
+    def to_map(self):
+        result = dict()
+        if self.commodity_code is not None:
+            result['commodity_code'] = self.commodity_code
+        if self.commodity_name is not None:
+            result['commodity_name'] = self.commodity_name
+        if self.pay_amount is not None:
+            result['pay_amount'] = self.pay_amount
+        if self.original_amount is not None:
+            result['original_amount'] = self.original_amount
+        if self.discount_amount is not None:
+            result['discount_amount'] = self.discount_amount
+        if self.activity_code is not None:
+            result['activity_code'] = self.activity_code
+        if self.activity_name is not None:
+            result['activity_name'] = self.activity_name
+        if self.price_plan_id is not None:
+            result['price_plan_id'] = self.price_plan_id
+        if self.price_constraint_id is not None:
+            result['price_constraint_id'] = self.price_constraint_id
+        if self.currency is not None:
+            result['currency'] = self.currency
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commodity_code') is not None:
+            self.commodity_code = m.get('commodity_code')
+        if m.get('commodity_name') is not None:
+            self.commodity_name = m.get('commodity_name')
+        if m.get('pay_amount') is not None:
+            self.pay_amount = m.get('pay_amount')
+        if m.get('original_amount') is not None:
+            self.original_amount = m.get('original_amount')
+        if m.get('discount_amount') is not None:
+            self.discount_amount = m.get('discount_amount')
+        if m.get('activity_code') is not None:
+            self.activity_code = m.get('activity_code')
+        if m.get('activity_name') is not None:
+            self.activity_name = m.get('activity_name')
+        if m.get('price_plan_id') is not None:
+            self.price_plan_id = m.get('price_plan_id')
+        if m.get('price_constraint_id') is not None:
+            self.price_constraint_id = m.get('price_constraint_id')
+        if m.get('currency') is not None:
+            self.currency = m.get('currency')
+        return self
+
+
+class PayOptions(TeaModel):
+    def __init__(
+        self,
+        pay_channel: str = None,
+    ):
+        # 系统自动会根据账号类型、当前OU进行付费渠道判定；如果传入的付款渠道不满足，则报错
+        self.pay_channel = pay_channel
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        result = dict()
+        if self.pay_channel is not None:
+            result['pay_channel'] = self.pay_channel
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('pay_channel') is not None:
+            self.pay_channel = m.get('pay_channel')
+        return self
+
+
+class CreateOrderResult(TeaModel):
+    def __init__(
+        self,
+        bsn_no: str = None,
+        order_id: str = None,
+        normal_order_line_id: str = None,
+        order_status: str = None,
+        instance_ids: str = None,
+        order_error_code: str = None,
+        order_error_description: str = None,
+    ):
+        # 下单时指定的业务流水号。二级订单号
+        self.bsn_no = bsn_no
+        # 一级订单号
+        self.order_id = order_id
+        # 二级订单号
+        self.normal_order_line_id = normal_order_line_id
+        # 订单状态
+        self.order_status = order_status
+        # 实例列表
+        self.instance_ids = instance_ids
+        # 订购错误码
+        self.order_error_code = order_error_code
+        # 订购错误描述
+        self.order_error_description = order_error_description
+
+    def validate(self):
+        self.validate_required(self.bsn_no, 'bsn_no')
+        self.validate_required(self.order_id, 'order_id')
+        self.validate_required(self.normal_order_line_id, 'normal_order_line_id')
+        self.validate_required(self.order_status, 'order_status')
+        self.validate_required(self.instance_ids, 'instance_ids')
+        self.validate_required(self.order_error_code, 'order_error_code')
+        self.validate_required(self.order_error_description, 'order_error_description')
+
+    def to_map(self):
+        result = dict()
+        if self.bsn_no is not None:
+            result['bsn_no'] = self.bsn_no
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.normal_order_line_id is not None:
+            result['normal_order_line_id'] = self.normal_order_line_id
+        if self.order_status is not None:
+            result['order_status'] = self.order_status
+        if self.instance_ids is not None:
+            result['instance_ids'] = self.instance_ids
+        if self.order_error_code is not None:
+            result['order_error_code'] = self.order_error_code
+        if self.order_error_description is not None:
+            result['order_error_description'] = self.order_error_description
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bsn_no') is not None:
+            self.bsn_no = m.get('bsn_no')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('normal_order_line_id') is not None:
+            self.normal_order_line_id = m.get('normal_order_line_id')
+        if m.get('order_status') is not None:
+            self.order_status = m.get('order_status')
+        if m.get('instance_ids') is not None:
+            self.instance_ids = m.get('instance_ids')
+        if m.get('order_error_code') is not None:
+            self.order_error_code = m.get('order_error_code')
+        if m.get('order_error_description') is not None:
+            self.order_error_description = m.get('order_error_description')
+        return self
+
+
+class OrderDuration(TeaModel):
+    def __init__(
+        self,
+        duration_type: str = None,
+        duration_value: int = None,
+    ):
+        # 周期类型，YEAR：年；MONTH：月；DAY：日
+        self.duration_type = duration_type
+        # 订购周期值
+        self.duration_value = duration_value
+
+    def validate(self):
+        self.validate_required(self.duration_type, 'duration_type')
+        self.validate_required(self.duration_value, 'duration_value')
+
+    def to_map(self):
+        result = dict()
+        if self.duration_type is not None:
+            result['duration_type'] = self.duration_type
+        if self.duration_value is not None:
+            result['duration_value'] = self.duration_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('duration_type') is not None:
+            self.duration_type = m.get('duration_type')
+        if m.get('duration_value') is not None:
+            self.duration_value = m.get('duration_value')
+        return self
+
+
+class InstanceLabel(TeaModel):
+    def __init__(
+        self,
+        instance_key: str = None,
+        instance_value: str = None,
+    ):
+        # 标签名。
+        # 传递isvId
+        self.instance_key = instance_key
+        # 标签值
+        self.instance_value = instance_value
+
+    def validate(self):
+        self.validate_required(self.instance_key, 'instance_key')
+        self.validate_required(self.instance_value, 'instance_value')
+
+    def to_map(self):
+        result = dict()
+        if self.instance_key is not None:
+            result['instance_key'] = self.instance_key
+        if self.instance_value is not None:
+            result['instance_value'] = self.instance_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('instance_key') is not None:
+            self.instance_key = m.get('instance_key')
+        if m.get('instance_value') is not None:
+            self.instance_value = m.get('instance_value')
+        return self
+
+
+class CommodityOrderAttribute(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        value: str = None,
+        value_unit: str = None,
+    ):
+        # 属性编码
+        self.code = code
+        # 属性值
+        self.value = value
+        # 属性值单位，部分数值型属性有多种单位，需要填入；其他情况不需要填
+        self.value_unit = value_unit
+
+    def validate(self):
+        self.validate_required(self.code, 'code')
+        self.validate_required(self.value, 'value')
+        self.validate_required(self.value_unit, 'value_unit')
+
+    def to_map(self):
+        result = dict()
+        if self.code is not None:
+            result['code'] = self.code
+        if self.value is not None:
+            result['value'] = self.value
+        if self.value_unit is not None:
+            result['value_unit'] = self.value_unit
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        if m.get('value_unit') is not None:
+            self.value_unit = m.get('value_unit')
+        return self
+
+
+class FulfillmentOptions(TeaModel):
+    def __init__(
+        self,
+        deplay: bool = None,
+        start_time: str = None,
+        spi_skip: bool = None,
+    ):
+        # 是否延迟履约，默认false
+        self.deplay = deplay
+        # 实际履约开始时间，默认支付完成时间；只有deplay=true时，start_time才生效
+        self.start_time = start_time
+        # 跳过SPI回调，默认false，优先级高于商品上默认的接入属性
+        self.spi_skip = spi_skip
+
+    def validate(self):
+        if self.start_time is not None:
+            self.validate_pattern(self.start_time, 'start_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+
+    def to_map(self):
+        result = dict()
+        if self.deplay is not None:
+            result['deplay'] = self.deplay
+        if self.start_time is not None:
+            result['start_time'] = self.start_time
+        if self.spi_skip is not None:
+            result['spi_skip'] = self.spi_skip
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deplay') is not None:
+            self.deplay = m.get('deplay')
+        if m.get('start_time') is not None:
+            self.start_time = m.get('start_time')
+        if m.get('spi_skip') is not None:
+            self.spi_skip = m.get('spi_skip')
+        return self
+
+
 class ComboOrder(TeaModel):
     def __init__(
         self,
         tenant_id: str = None,
         biz_no: str = None,
         order_id: str = None,
         combo_code: str = None,
@@ -1340,18 +1108,14 @@
                     k.validate()
         self.validate_required(self.pay_time, 'pay_time')
         if self.pay_time is not None:
             self.validate_pattern(self.pay_time, 'pay_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         self.validate_required(self.pay_channel, 'pay_channel')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.biz_no is not None:
             result['biz_no'] = self.biz_no
         if self.order_id is not None:
             result['order_id'] = self.order_id
@@ -1417,14 +1181,70 @@
         if m.get('pay_time') is not None:
             self.pay_time = m.get('pay_time')
         if m.get('pay_channel') is not None:
             self.pay_channel = m.get('pay_channel')
         return self
 
 
+class Instance(TeaModel):
+    def __init__(
+        self,
+        tenant_id: str = None,
+        instance_id: str = None,
+        product_name: str = None,
+        charge_type: str = None,
+        status: str = None,
+    ):
+        # 租户id
+        self.tenant_id = tenant_id
+        # 实例id
+        self.instance_id = instance_id
+        # 商品code
+        self.product_name = product_name
+        # 付费类型 PREPAY_BY_MONTH 预付 AFTER_PAY_BY_HOUR 后付 MIX_PAY 混合付
+        self.charge_type = charge_type
+        # 状态 CREATING 创建中 FAILED 创建失败  STARTED 运行中 STOPPED 已停服  RELEASED 已释放
+        self.status = status
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.instance_id, 'instance_id')
+        self.validate_required(self.product_name, 'product_name')
+        self.validate_required(self.charge_type, 'charge_type')
+        self.validate_required(self.status, 'status')
+
+    def to_map(self):
+        result = dict()
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.instance_id is not None:
+            result['instance_id'] = self.instance_id
+        if self.product_name is not None:
+            result['product_name'] = self.product_name
+        if self.charge_type is not None:
+            result['charge_type'] = self.charge_type
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('instance_id') is not None:
+            self.instance_id = m.get('instance_id')
+        if m.get('product_name') is not None:
+            self.product_name = m.get('product_name')
+        if m.get('charge_type') is not None:
+            self.charge_type = m.get('charge_type')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
 class QueryInstanceCapacityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         tenant_id: str = None,
         tenant_name: str = None,
         status: str = None,
@@ -1442,18 +1262,14 @@
         # 资源包商品码
         self.commodity_code = commodity_code
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.tenant_name is not None:
             result['tenant_name'] = self.tenant_name
@@ -1498,18 +1314,14 @@
     def validate(self):
         if self.instance_capacitys:
             for k in self.instance_capacitys:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1559,18 +1371,14 @@
         self.validate_required(self.tenant_id, 'tenant_id')
         self.validate_required(self.product_codes, 'product_codes')
         self.validate_required(self.biz_time, 'biz_time')
         if self.biz_time is not None:
             self.validate_pattern(self.biz_time, 'biz_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.product_codes is not None:
             result['product_codes'] = self.product_codes
@@ -1615,18 +1423,14 @@
     def validate(self):
         if self.coupon_list:
             for k in self.coupon_list:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1674,18 +1478,14 @@
 
     def validate(self):
         self.validate_required(self.biz_no, 'biz_no')
         self.validate_required(self.tenant_id, 'tenant_id')
         self.validate_required(self.template_id, 'template_id')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.biz_no is not None:
             result['biz_no'] = self.biz_no
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
@@ -1724,18 +1524,14 @@
         # 
         self.coupon_id = coupon_id
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1782,18 +1578,14 @@
         self.validate_required(self.biz_no, 'biz_no')
         if self.instance_labels:
             for k in self.instance_labels:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_list is not None:
             result['product_list'] = self.product_list
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
@@ -1846,18 +1638,14 @@
     def validate(self):
         if self.create_order_response_list:
             for k in self.create_order_response_list:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1914,18 +1702,14 @@
         self.validate_required(self.instance_labels, 'instance_labels')
         if self.instance_labels:
             for k in self.instance_labels:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_list is not None:
             result['product_list'] = self.product_list
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
@@ -1978,18 +1762,14 @@
     def validate(self):
         if self.create_order_response_list:
             for k in self.create_order_response_list:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2030,18 +1810,14 @@
         # 套餐编码
         self.combo_code = combo_code
 
     def validate(self):
         self.validate_required(self.combo_code, 'combo_code')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.combo_code is not None:
             result['combo_code'] = self.combo_code
         return result
 
@@ -2072,18 +1848,14 @@
         self.combo = combo
 
     def validate(self):
         if self.combo:
             self.combo.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2128,18 +1900,14 @@
         # 优惠券ID
         self.coupon_id = coupon_id
 
     def validate(self):
         self.validate_required(self.combo_code, 'combo_code')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.combo_code is not None:
             result['combo_code'] = self.combo_code
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
@@ -2203,18 +1971,14 @@
     def validate(self):
         if self.commodity_enquiry_prices:
             for k in self.commodity_enquiry_prices:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2305,18 +2069,14 @@
             self.duration.validate()
         if self.instance_labels:
             for k in self.instance_labels:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.scene_code is not None:
             result['scene_code'] = self.scene_code
         if self.biz_no is not None:
             result['biz_no'] = self.biz_no
@@ -2384,18 +2144,14 @@
         # 套餐下单订单号
         self.combo_order_id = combo_order_id
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2451,18 +2207,14 @@
     def validate(self):
         if self.begin_time is not None:
             self.validate_pattern(self.begin_time, 'begin_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         if self.end_time is not None:
             self.validate_pattern(self.end_time, 'end_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.tenant_name is not None:
             result['tenant_name'] = self.tenant_name
@@ -2532,18 +2284,14 @@
     def validate(self):
         if self.orders:
             for k in self.orders:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2592,18 +2340,14 @@
         # 类目编码
         self.category_code = category_code
 
     def validate(self):
         self.validate_required(self.category_code, 'category_code')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.category_code is not None:
             result['category_code'] = self.category_code
         return result
 
@@ -2636,18 +2380,14 @@
     def validate(self):
         if self.combos:
             for k in self.combos:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2696,18 +2436,14 @@
 
     def validate(self):
         self.validate_required(self.combo_order_id, 'combo_order_id')
         self.validate_required(self.pay_channel, 'pay_channel')
         self.validate_required(self.pay_mode, 'pay_mode')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.combo_order_id is not None:
             result['combo_order_id'] = self.combo_order_id
         if self.pay_channel is not None:
             result['pay_channel'] = self.pay_channel
@@ -2759,18 +2495,14 @@
         # CANCEL：取消支付;
         self.pay_status = pay_status
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2804,110 +2536,78 @@
         self,
         auth_token: str = None,
         biz_no: str = None,
         tenant_id: str = None,
         tenant_name: str = None,
         operator_id: str = None,
         commodity_code: str = None,
-        ou: str = None,
         order_type: str = None,
         duration: OrderDuration = None,
         coupon_id: str = None,
         quantity: int = None,
         commodity_attrs: List[CommodityOrderAttribute] = None,
         fulfillment_options: FulfillmentOptions = None,
         pay_options: PayOptions = None,
-        price_strategy: PriceStrategy = None,
-        instance_id: str = None,
-        sale_market: str = None,
-        extended_properties: str = None,
-        batch_biz_no: str = None,
-        prepay_amount: PrepayAmount = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 业务流水号，调用方指定，幂等号
         self.biz_no = biz_no
         # 租户ID，和租户名称二选一必填
         self.tenant_id = tenant_id
         # 租户名称，和租户ID二选一必填
         self.tenant_name = tenant_name
         # 操作人ID，不填则默认和租户ID一致
         self.operator_id = operator_id
         # 商品编码
         self.commodity_code = commodity_code
-        # 销售主体，不传默认ZL6
-        self.ou = ou
-        # 订单类型，NEW：新购；RENEW：续费； MODIFY：变配
+        # 订单类型，NEW：新购；RENEW：续费
         # 不填默认新购
         self.order_type = order_type
         # 订购周期对象，当商品是周期订阅类型时，必填
         self.duration = duration
         # 优惠券ID
         self.coupon_id = coupon_id
         # 数量，不填默认1
         self.quantity = quantity
         # 商品订购属性，开通型商品部需要填写
         self.commodity_attrs = commodity_attrs
         # 履约选项
         self.fulfillment_options = fulfillment_options
         # 支付选项
         self.pay_options = pay_options
-        # 价格策略
-        self.price_strategy = price_strategy
-        # 实例ID，续费/变配场景必传
-        self.instance_id = instance_id
-        # 售卖市场。10100000：鹊凿市场；12000002：国际ZAN市场；其他市场编码请联系中台获取
-        self.sale_market = sale_market
-        # 扩展属性，JSON字符串
-        self.extended_properties = extended_properties
-        # 批次流水号，外部合同下单场景，传入向中台申请的合同ID
-        self.batch_biz_no = batch_biz_no
-        # 预付费订单金额。仅白名单商品且batchBizNo是合法的合同ID的情况，才允许指定预付订单金额
-        self.prepay_amount = prepay_amount
 
     def validate(self):
         self.validate_required(self.biz_no, 'biz_no')
         self.validate_required(self.commodity_code, 'commodity_code')
         if self.duration:
             self.duration.validate()
         if self.commodity_attrs:
             for k in self.commodity_attrs:
                 if k:
                     k.validate()
         if self.fulfillment_options:
             self.fulfillment_options.validate()
         if self.pay_options:
             self.pay_options.validate()
-        if self.price_strategy:
-            self.price_strategy.validate()
-        self.validate_required(self.sale_market, 'sale_market')
-        if self.prepay_amount:
-            self.prepay_amount.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.biz_no is not None:
             result['biz_no'] = self.biz_no
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.tenant_name is not None:
             result['tenant_name'] = self.tenant_name
         if self.operator_id is not None:
             result['operator_id'] = self.operator_id
         if self.commodity_code is not None:
             result['commodity_code'] = self.commodity_code
-        if self.ou is not None:
-            result['ou'] = self.ou
         if self.order_type is not None:
             result['order_type'] = self.order_type
         if self.duration is not None:
             result['duration'] = self.duration.to_map()
         if self.coupon_id is not None:
             result['coupon_id'] = self.coupon_id
         if self.quantity is not None:
@@ -2916,26 +2616,14 @@
         if self.commodity_attrs is not None:
             for k in self.commodity_attrs:
                 result['commodity_attrs'].append(k.to_map() if k else None)
         if self.fulfillment_options is not None:
             result['fulfillment_options'] = self.fulfillment_options.to_map()
         if self.pay_options is not None:
             result['pay_options'] = self.pay_options.to_map()
-        if self.price_strategy is not None:
-            result['price_strategy'] = self.price_strategy.to_map()
-        if self.instance_id is not None:
-            result['instance_id'] = self.instance_id
-        if self.sale_market is not None:
-            result['sale_market'] = self.sale_market
-        if self.extended_properties is not None:
-            result['extended_properties'] = self.extended_properties
-        if self.batch_biz_no is not None:
-            result['batch_biz_no'] = self.batch_biz_no
-        if self.prepay_amount is not None:
-            result['prepay_amount'] = self.prepay_amount.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('biz_no') is not None:
@@ -2944,16 +2632,14 @@
             self.tenant_id = m.get('tenant_id')
         if m.get('tenant_name') is not None:
             self.tenant_name = m.get('tenant_name')
         if m.get('operator_id') is not None:
             self.operator_id = m.get('operator_id')
         if m.get('commodity_code') is not None:
             self.commodity_code = m.get('commodity_code')
-        if m.get('ou') is not None:
-            self.ou = m.get('ou')
         if m.get('order_type') is not None:
             self.order_type = m.get('order_type')
         if m.get('duration') is not None:
             temp_model = OrderDuration()
             self.duration = temp_model.from_map(m['duration'])
         if m.get('coupon_id') is not None:
             self.coupon_id = m.get('coupon_id')
@@ -2966,28 +2652,14 @@
                 self.commodity_attrs.append(temp_model.from_map(k))
         if m.get('fulfillment_options') is not None:
             temp_model = FulfillmentOptions()
             self.fulfillment_options = temp_model.from_map(m['fulfillment_options'])
         if m.get('pay_options') is not None:
             temp_model = PayOptions()
             self.pay_options = temp_model.from_map(m['pay_options'])
-        if m.get('price_strategy') is not None:
-            temp_model = PriceStrategy()
-            self.price_strategy = temp_model.from_map(m['price_strategy'])
-        if m.get('instance_id') is not None:
-            self.instance_id = m.get('instance_id')
-        if m.get('sale_market') is not None:
-            self.sale_market = m.get('sale_market')
-        if m.get('extended_properties') is not None:
-            self.extended_properties = m.get('extended_properties')
-        if m.get('batch_biz_no') is not None:
-            self.batch_biz_no = m.get('batch_biz_no')
-        if m.get('prepay_amount') is not None:
-            temp_model = PrepayAmount()
-            self.prepay_amount = temp_model.from_map(m['prepay_amount'])
         return self
 
 
 class CreateOrderResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -3010,18 +2682,14 @@
         # 支付状态
         self.pay_status = pay_status
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3046,201 +2714,14 @@
         if m.get('instance_ids') is not None:
             self.instance_ids = m.get('instance_ids')
         if m.get('pay_status') is not None:
             self.pay_status = m.get('pay_status')
         return self
 
 
-class GetComboOrderRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        combo_order_id: str = None,
-        include_fulfill_info: bool = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        # 套餐订单ID
-        self.combo_order_id = combo_order_id
-        # 是否包含履约信息
-        self.include_fulfill_info = include_fulfill_info
-
-    def validate(self):
-        self.validate_required(self.combo_order_id, 'combo_order_id')
-        self.validate_required(self.include_fulfill_info, 'include_fulfill_info')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.combo_order_id is not None:
-            result['combo_order_id'] = self.combo_order_id
-        if self.include_fulfill_info is not None:
-            result['include_fulfill_info'] = self.include_fulfill_info
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('combo_order_id') is not None:
-            self.combo_order_id = m.get('combo_order_id')
-        if m.get('include_fulfill_info') is not None:
-            self.include_fulfill_info = m.get('include_fulfill_info')
-        return self
-
-
-class GetComboOrderResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        order: ComboOrder = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 套餐订单详情
-        self.order = order
-
-    def validate(self):
-        if self.order:
-            self.order.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.order is not None:
-            result['order'] = self.order.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('order') is not None:
-            temp_model = ComboOrder()
-            self.order = temp_model.from_map(m['order'])
-        return self
-
-
-class CancelOrderRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        order_id: str = None,
-        tenant_id: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        # 订单ID
-        # 
-        self.order_id = order_id
-        # 下单时的租户ID
-        self.tenant_id = tenant_id
-
-    def validate(self):
-        self.validate_required(self.order_id, 'order_id')
-        self.validate_required(self.tenant_id, 'tenant_id')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.order_id is not None:
-            result['order_id'] = self.order_id
-        if self.tenant_id is not None:
-            result['tenant_id'] = self.tenant_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('order_id') is not None:
-            self.order_id = m.get('order_id')
-        if m.get('tenant_id') is not None:
-            self.tenant_id = m.get('tenant_id')
-        return self
-
-
-class CancelOrderResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        result: bool = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 是否取消成功
-        self.result = result
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        if self.result is not None:
-            result['result'] = self.result
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        if m.get('result') is not None:
-            self.result = m.get('result')
-        return self
-
-
 class ExistPricePersonalizedRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         tenant_id: str = None,
         product_code: str = None,
         price_object_code: str = None,
@@ -3255,18 +2736,14 @@
         self.price_object_code = price_object_code
 
     def validate(self):
         self.validate_required(self.tenant_id, 'tenant_id')
         self.validate_required(self.product_code, 'product_code')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.product_code is not None:
             result['product_code'] = self.product_code
@@ -3304,18 +2781,14 @@
         # 是否存在
         self.exist = exist
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3345,60 +2818,50 @@
         tenant_name: str = None,
         quantity: int = None,
         biz_time: str = None,
         order_duration: OrderDuration = None,
         commodity_order_attrs: List[CommodityOrderAttribute] = None,
         currency: str = None,
         coupon_id: str = None,
-        order_type: str = None,
-        instance_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 商品主数据编码
         self.commodity_code = commodity_code
         # 租户ID，和租户名称二选一必填
         self.tenant_id = tenant_id
         # 8位租户名，和租户ID二选一必选
         self.tenant_name = tenant_name
         # 商品数量，不传则默认1
         self.quantity = quantity
         # 业务发生时间，不传则默认当前时间
         self.biz_time = biz_time
-        # 订购周期，基于周期定价的商品必填
+        # 订购周期，周期型商品必填，如资源包/包年包月商品
         self.order_duration = order_duration
-        # 商品规格列表，按实际商品定义的和价格相关的属性传入
-        # 1.续费询价不需要传
-        # 2.变配询价需要传入变化的规格属性
+        # 商品规格列表
+        # 针对量价型商品，统一使用SYS_USAGE_AMOUNT
+        # 针对资源包商品，统一使用CAPACITY
         self.commodity_order_attrs = commodity_order_attrs
         # 币种，元：CNY，不传默认CNY
         self.currency = currency
         # 优惠券ID
         self.coupon_id = coupon_id
-        # 不填默认为NEW；NEW：新购；RENEW：续费；MODIFY：变配
-        self.order_type = order_type
-        # 实例ID，续费/变配场景必传
-        self.instance_id = instance_id
 
     def validate(self):
         self.validate_required(self.commodity_code, 'commodity_code')
         if self.biz_time is not None:
             self.validate_pattern(self.biz_time, 'biz_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         if self.order_duration:
             self.order_duration.validate()
         if self.commodity_order_attrs:
             for k in self.commodity_order_attrs:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.commodity_code is not None:
             result['commodity_code'] = self.commodity_code
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
@@ -3414,18 +2877,14 @@
         if self.commodity_order_attrs is not None:
             for k in self.commodity_order_attrs:
                 result['commodity_order_attrs'].append(k.to_map() if k else None)
         if self.currency is not None:
             result['currency'] = self.currency
         if self.coupon_id is not None:
             result['coupon_id'] = self.coupon_id
-        if self.order_type is not None:
-            result['order_type'] = self.order_type
-        if self.instance_id is not None:
-            result['instance_id'] = self.instance_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('commodity_code') is not None:
@@ -3446,18 +2905,14 @@
             for k in m.get('commodity_order_attrs'):
                 temp_model = CommodityOrderAttribute()
                 self.commodity_order_attrs.append(temp_model.from_map(k))
         if m.get('currency') is not None:
             self.currency = m.get('currency')
         if m.get('coupon_id') is not None:
             self.coupon_id = m.get('coupon_id')
-        if m.get('order_type') is not None:
-            self.order_type = m.get('order_type')
-        if m.get('instance_id') is not None:
-            self.instance_id = m.get('instance_id')
         return self
 
 
 class QueryPriceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -3475,18 +2930,14 @@
         self.commodity_enquiry_price = commodity_enquiry_price
 
     def validate(self):
         if self.commodity_enquiry_price:
             self.commodity_enquiry_price.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -3523,18 +2974,14 @@
         self.product_codes = product_codes
 
     def validate(self):
         self.validate_required(self.tenant_id, 'tenant_id')
         self.validate_required(self.product_codes, 'product_codes')
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.tenant_id is not None:
             result['tenant_id'] = self.tenant_id
         if self.product_codes is not None:
             result['product_codes'] = self.product_codes
@@ -3571,18 +3018,14 @@
     def validate(self):
         if self.instances:
             for k in self.instances:
                 if k:
                     k.validate()
 
     def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
```

### Comparing `antchain_trade-3.13.2/antchain_trade.egg-info/PKG-INFO` & `antchain_trade-3.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-trade
-Version: 3.13.2
+Name: antchain_trade
+Version: 3.6.3
 Summary: Ant Chain TRADE SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain-trade
-        pip install antchain-trade
+        # Install the antchain_sdk_trade
+        pip install antchain_sdk_trade
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_trade-3.13.2/setup.py` & `antchain_trade-3.6.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_trade.
 
-Created on 27/05/2024
+Created on 13/09/2021
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_trade"
 NAME = "antchain_trade" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain TRADE SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_util>=0.3.5, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

