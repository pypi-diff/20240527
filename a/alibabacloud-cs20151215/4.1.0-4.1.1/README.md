# Comparing `tmp/alibabacloud_cs20151215-4.1.0.tar.gz` & `tmp/alibabacloud_cs20151215-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cs20151215-4.1.0.tar", last modified: Fri May 24 17:09:09 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cs20151215-4.1.1.tar", last modified: Mon May 27 17:14:17 2024, max compression
```

## Comparing `alibabacloud_cs20151215-4.1.0.tar` & `alibabacloud_cs20151215-4.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/
--rw-r--r--   0 root         (0) root         (0)     6816 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1091 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215/__init__.py
--rw-r--r--   0 root         (0) root         (0)   630720 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215/client.py
--rw-r--r--   0 root         (0) root         (0)   988187 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-24 17:09:09.000000 alibabacloud_cs20151215-4.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2606 2024-05-24 17:09:08.000000 alibabacloud_cs20151215-4.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/
+-rw-r--r--   0 root         (0) root         (0)     6876 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   630936 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215/client.py
+-rw-r--r--   0 root         (0) root         (0)   989689 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-05-27 17:14:17.000000 alibabacloud_cs20151215-4.1.1/setup.py
```

### Comparing `alibabacloud_cs20151215-4.1.0/ChangeLog.md` & `alibabacloud_cs20151215-4.1.1/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-05-24 Version: 4.1.0
+- Support API CheckServiceRole.
+
+
 2024-05-15 Version: 4.0.10
 - Generated python 2015-12-15 for CS.
 
 2024-05-15 Version: 4.0.9
 - Update API DescribeKubernetesVersionMetadata: add param QueryUpgradableVersion.
 - Update API DescribeKubernetesVersionMetadata: update response param.
```

### Comparing `alibabacloud_cs20151215-4.1.0/LICENSE` & `alibabacloud_cs20151215-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215-4.1.0/PKG-INFO` & `alibabacloud_cs20151215-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cs20151215
-Version: 4.1.0
+Version: 4.1.1
 Summary: Alibaba Cloud CS (20151215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cs20151215-4.1.0/README-CN.md` & `alibabacloud_cs20151215-4.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215-4.1.0/README.md` & `alibabacloud_cs20151215-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215/client.py` & `alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11478,14 +11478,16 @@
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.auto_restart):
             body['auto_restart'] = request.auto_restart
         if not UtilClient.is_unset(request.nodes):
             body['nodes'] = request.nodes
+        if not UtilClient.is_unset(request.operations):
+            body['operations'] = request.operations
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='RepairClusterNodePool',
             version='2015-12-15',
@@ -11520,14 +11522,16 @@
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.auto_restart):
             body['auto_restart'] = request.auto_restart
         if not UtilClient.is_unset(request.nodes):
             body['nodes'] = request.nodes
+        if not UtilClient.is_unset(request.operations):
+            body['operations'] = request.operations
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='RepairClusterNodePool',
             version='2015-12-15',
```

### Comparing `alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215/models.py` & `alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -55287,6476 +55287,6570 @@
 000d7f60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
 000d7f70: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
 000d7f80: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
 000d7f90: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
 000d7fa0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
 000d7fb0: 660a 0a0a 636c 6173 7320 5265 7061 6972  f...class Repair
 000d7fc0: 436c 7573 7465 724e 6f64 6550 6f6f 6c52  ClusterNodePoolR
-000d7fd0: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-000d7fe0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000d7ff0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000d8000: 2c0a 2020 2020 2020 2020 6175 746f 5f72  ,.        auto_r
-000d8010: 6573 7461 7274 3a20 626f 6f6c 203d 204e  estart: bool = N
-000d8020: 6f6e 652c 0a20 2020 2020 2020 206e 6f64  one,.        nod
-000d8030: 6573 3a20 4c69 7374 5b73 7472 5d20 3d20  es: List[str] = 
-000d8040: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000d8050: 2020 2020 2073 656c 662e 6175 746f 5f72       self.auto_r
-000d8060: 6573 7461 7274 203d 2061 7574 6f5f 7265  estart = auto_re
-000d8070: 7374 6172 740a 2020 2020 2020 2020 2320  start.        # 
-000d8080: 5468 6520 6c69 7374 206f 6620 6e6f 6465  The list of node
-000d8090: 732e 2049 6620 796f 7520 646f 206e 6f74  s. If you do not
-000d80a0: 2073 7065 6369 6679 206e 6f64 6573 2c20   specify nodes, 
-000d80b0: 616c 6c20 6e6f 6465 7320 696e 2074 6865  all nodes in the
-000d80c0: 206e 6f64 6520 706f 6f6c 2061 7265 2073   node pool are s
-000d80d0: 656c 6563 7465 642e 0a20 2020 2020 2020  elected..       
-000d80e0: 2073 656c 662e 6e6f 6465 7320 3d20 6e6f   self.nodes = no
-000d80f0: 6465 730a 0a20 2020 2064 6566 2076 616c  des..    def val
-000d8100: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000d8110: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000d8120: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000d8130: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-000d8140: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-000d8150: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-000d8160: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000d8170: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000d8180: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-000d8190: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-000d81a0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-000d81b0: 7574 6f5f 7265 7374 6172 7420 6973 206e  uto_restart is n
-000d81c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000d81d0: 2020 2020 2072 6573 756c 745b 2761 7574       result['aut
-000d81e0: 6f5f 7265 7374 6172 7427 5d20 3d20 7365  o_restart'] = se
-000d81f0: 6c66 2e61 7574 6f5f 7265 7374 6172 740a  lf.auto_restart.
-000d8200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000d8210: 6e6f 6465 7320 6973 206e 6f74 204e 6f6e  nodes is not Non
-000d8220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000d8230: 6573 756c 745b 276e 6f64 6573 275d 203d  esult['nodes'] =
-000d8240: 2073 656c 662e 6e6f 6465 730a 2020 2020   self.nodes.    
-000d8250: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000d8260: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000d8270: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000d8280: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000d8290: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000d82a0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000d82b0: 6765 7428 2761 7574 6f5f 7265 7374 6172  get('auto_restar
-000d82c0: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
-000d82d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000d82e0: 662e 6175 746f 5f72 6573 7461 7274 203d  f.auto_restart =
-000d82f0: 206d 2e67 6574 2827 6175 746f 5f72 6573   m.get('auto_res
-000d8300: 7461 7274 2729 0a20 2020 2020 2020 2069  tart').        i
-000d8310: 6620 6d2e 6765 7428 276e 6f64 6573 2729  f m.get('nodes')
-000d8320: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000d8330: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000d8340: 6f64 6573 203d 206d 2e67 6574 2827 6e6f  odes = m.get('no
-000d8350: 6465 7327 290a 2020 2020 2020 2020 7265  des').        re
-000d8360: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000d8370: 7320 5265 7061 6972 436c 7573 7465 724e  s RepairClusterN
-000d8380: 6f64 6550 6f6f 6c52 6573 706f 6e73 6542  odePoolResponseB
-000d8390: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-000d83a0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000d83b0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000d83c0: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
-000d83d0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-000d83e0: 2020 2020 2020 2074 6173 6b5f 6964 3a20         task_id: 
-000d83f0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000d8400: 293a 0a20 2020 2020 2020 2023 2054 6865  ):.        # The
-000d8410: 2072 6571 7565 7374 2049 442e 0a20 2020   request ID..   
-000d8420: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-000d8430: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-000d8440: 640a 2020 2020 2020 2020 2320 5468 6520  d.        # The 
-000d8450: 4944 206f 6620 7468 6520 7461 736b 2e0a  ID of the task..
-000d8460: 2020 2020 2020 2020 7365 6c66 2e74 6173          self.tas
-000d8470: 6b5f 6964 203d 2074 6173 6b5f 6964 0a0a  k_id = task_id..
-000d8480: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000d8490: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000d84a0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-000d84b0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-000d84c0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-000d84d0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-000d84e0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-000d84f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000d8500: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-000d8510: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000d8520: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000d8530: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-000d8540: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-000d8550: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000d8560: 7375 6c74 5b27 7265 7175 6573 745f 6964  sult['request_id
-000d8570: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-000d8580: 745f 6964 0a20 2020 2020 2020 2069 6620  t_id.        if 
-000d8590: 7365 6c66 2e74 6173 6b5f 6964 2069 7320  self.task_id is 
-000d85a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000d85b0: 2020 2020 2020 7265 7375 6c74 5b27 7461        result['ta
-000d85c0: 736b 5f69 6427 5d20 3d20 7365 6c66 2e74  sk_id'] = self.t
-000d85d0: 6173 6b5f 6964 0a20 2020 2020 2020 2072  ask_id.        r
-000d85e0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000d85f0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000d8600: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000d8610: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000d8620: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000d8630: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000d8640: 7265 7175 6573 745f 6964 2729 2069 7320  request_id') is 
-000d8650: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000d8660: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-000d8670: 7374 5f69 6420 3d20 6d2e 6765 7428 2772  st_id = m.get('r
-000d8680: 6571 7565 7374 5f69 6427 290a 2020 2020  equest_id').    
-000d8690: 2020 2020 6966 206d 2e67 6574 2827 7461      if m.get('ta
-000d86a0: 736b 5f69 6427 2920 6973 206e 6f74 204e  sk_id') is not N
-000d86b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000d86c0: 2073 656c 662e 7461 736b 5f69 6420 3d20   self.task_id = 
-000d86d0: 6d2e 6765 7428 2774 6173 6b5f 6964 2729  m.get('task_id')
-000d86e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000d86f0: 7365 6c66 0a0a 0a63 6c61 7373 2052 6570  self...class Rep
-000d8700: 6169 7243 6c75 7374 6572 4e6f 6465 506f  airClusterNodePo
-000d8710: 6f6c 5265 7370 6f6e 7365 2854 6561 4d6f  olResponse(TeaMo
-000d8720: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-000d8730: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000d8740: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
-000d8750: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
-000d8760: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
-000d8770: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
-000d8780: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
-000d8790: 2020 2020 2020 2062 6f64 793a 2052 6570         body: Rep
-000d87a0: 6169 7243 6c75 7374 6572 4e6f 6465 506f  airClusterNodePo
-000d87b0: 6f6c 5265 7370 6f6e 7365 426f 6479 203d  olResponseBody =
-000d87c0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-000d87d0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-000d87e0: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-000d87f0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000d8800: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-000d8810: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-000d8820: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-000d8830: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-000d8840: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-000d8850: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-000d8860: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-000d8870: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-000d8880: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000d8890: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-000d88a0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-000d88b0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-000d88c0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-000d88d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000d88e0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-000d88f0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-000d8900: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000d8910: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-000d8920: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000d8930: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-000d8940: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-000d8950: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-000d8960: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-000d8970: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000d8980: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000d8990: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-000d89a0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000d89b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000d89c0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-000d89d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000d89e0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-000d89f0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-000d8a00: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-000d8a10: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000d8a20: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000d8a30: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000d8a40: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000d8a50: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000d8a60: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-000d8a70: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-000d8a80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000d8a90: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-000d8aa0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-000d8ab0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000d8ac0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-000d8ad0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000d8ae0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000d8af0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-000d8b00: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-000d8b10: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000d8b20: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-000d8b30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000d8b40: 7465 6d70 5f6d 6f64 656c 203d 2052 6570  temp_model = Rep
-000d8b50: 6169 7243 6c75 7374 6572 4e6f 6465 506f  airClusterNodePo
-000d8b60: 6f6c 5265 7370 6f6e 7365 426f 6479 2829  olResponseBody()
-000d8b70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000d8b80: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-000d8b90: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-000d8ba0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-000d8bb0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-000d8bc0: 6173 7320 5265 7375 6d65 436f 6d70 6f6e  ass ResumeCompon
-000d8bd0: 656e 7455 7067 7261 6465 5265 7370 6f6e  entUpgradeRespon
-000d8be0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-000d8bf0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000d8c00: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000d8c10: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-000d8c20: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-000d8c30: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-000d8c40: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
-000d8c50: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-000d8c60: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-000d8c70: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-000d8c80: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000d8c90: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-000d8ca0: 6f64 650a 0a20 2020 2064 6566 2076 616c  ode..    def val
-000d8cb0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000d8cc0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000d8cd0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000d8ce0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-000d8cf0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-000d8d00: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-000d8d10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000d8d20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000d8d30: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-000d8d40: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-000d8d50: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-000d8d60: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-000d8d70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000d8d80: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-000d8d90: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-000d8da0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000d8db0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-000d8dc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000d8dd0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-000d8de0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-000d8df0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-000d8e00: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000d8e10: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-000d8e20: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-000d8e30: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-000d8e40: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-000d8e50: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000d8e60: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000d8e70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000d8e80: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-000d8e90: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-000d8ea0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-000d8eb0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-000d8ec0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-000d8ed0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000d8ee0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-000d8ef0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-000d8f00: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-000d8f10: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000d8f20: 6c61 7373 2052 6573 756d 6554 6173 6b52  lass ResumeTaskR
-000d8f30: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-000d8f40: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-000d8f50: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000d8f60: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
-000d8f70: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
-000d8f80: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-000d8f90: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
-000d8fa0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-000d8fb0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000d8fc0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-000d8fd0: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-000d8fe0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-000d8ff0: 7475 735f 636f 6465 0a0a 2020 2020 6465  tus_code..    de
-000d9000: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000d9010: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-000d9020: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000d9030: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000d9040: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000d9050: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000d9060: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000d9070: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000d9080: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000d9090: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000d90a0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000d90b0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-000d90c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000d90d0: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-000d90e0: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-000d90f0: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-000d9100: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000d9110: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000d9120: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000d9130: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-000d9140: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-000d9150: 6465 0a20 2020 2020 2020 2072 6574 7572  de.        retur
-000d9160: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000d9170: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000d9180: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000d9190: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000d91a0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000d91b0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-000d91c0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-000d91d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000d91e0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-000d91f0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-000d9200: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000d9210: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-000d9220: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000d9230: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000d9240: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-000d9250: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-000d9260: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000d9270: 660a 0a0a 636c 6173 7320 5265 7375 6d65  f...class Resume
-000d9280: 5570 6772 6164 6543 6c75 7374 6572 5265  UpgradeClusterRe
-000d9290: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-000d92a0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000d92b0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000d92c0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-000d92d0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-000d92e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000d92f0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-000d9300: 6e74 203d 204e 6f6e 652c 0a20 2020 2029  nt = None,.    )
-000d9310: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-000d9320: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-000d9330: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-000d9340: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
-000d9350: 7573 5f63 6f64 650a 0a20 2020 2064 6566  us_code..    def
-000d9360: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000d9370: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000d9380: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-000d9390: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-000d93a0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-000d93b0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-000d93c0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-000d93d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000d93e0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-000d93f0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-000d9400: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-000d9410: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-000d9420: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000d9430: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-000d9440: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-000d9450: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-000d9460: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000d9470: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000d9480: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000d9490: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-000d94a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000d94b0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-000d94c0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-000d94d0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-000d94e0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-000d94f0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000d9500: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000d9510: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-000d9520: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-000d9530: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000d9540: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-000d9550: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-000d9560: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000d9570: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-000d9580: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000d9590: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-000d95a0: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-000d95b0: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-000d95c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000d95d0: 0a0a 0a63 6c61 7373 2052 756e 436c 7573  ...class RunClus
-000d95e0: 7465 7243 6865 636b 5265 7175 6573 7428  terCheckRequest(
-000d95f0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-000d9600: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000d9610: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000d9620: 2020 206f 7074 696f 6e73 3a20 4469 6374     options: Dict
-000d9630: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-000d9640: 652c 0a20 2020 2020 2020 2074 6172 6765  e,.        targe
-000d9650: 743a 2073 7472 203d 204e 6f6e 652c 0a20  t: str = None,. 
-000d9660: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-000d9670: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000d9680: 2020 2020 2020 2020 2320 5468 6520 636c          # The cl
-000d9690: 7573 7465 7220 6368 6563 6b20 6974 656d  uster check item
-000d96a0: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-000d96b0: 6f70 7469 6f6e 7320 3d20 6f70 7469 6f6e  options = option
-000d96c0: 730a 2020 2020 2020 2020 7365 6c66 2e74  s.        self.t
-000d96d0: 6172 6765 7420 3d20 7461 7267 6574 0a20  arget = target. 
-000d96e0: 2020 2020 2020 2023 2054 6865 2063 6865         # The che
-000d96f0: 636b 206d 6574 686f 642e 0a20 2020 2020  ck method..     
-000d9700: 2020 2023 200a 2020 2020 2020 2020 2320     # .        # 
-000d9710: 5468 6973 2070 6172 616d 6574 6572 2069  This parameter i
-000d9720: 7320 7265 7175 6972 6564 2e0a 2020 2020  s required..    
-000d9730: 2020 2020 7365 6c66 2e74 7970 6520 3d20      self.type = 
-000d9740: 7479 7065 0a0a 2020 2020 6465 6620 7661  type..    def va
-000d9750: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000d9760: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000d9770: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000d9780: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000d9790: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-000d97a0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-000d97b0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000d97c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000d97d0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-000d97e0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000d97f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000d9800: 6f70 7469 6f6e 7320 6973 206e 6f74 204e  options is not N
-000d9810: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000d9820: 2072 6573 756c 745b 276f 7074 696f 6e73   result['options
-000d9830: 275d 203d 2073 656c 662e 6f70 7469 6f6e  '] = self.option
-000d9840: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-000d9850: 662e 7461 7267 6574 2069 7320 6e6f 7420  f.target is not 
-000d9860: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000d9870: 2020 7265 7375 6c74 5b27 7461 7267 6574    result['target
-000d9880: 275d 203d 2073 656c 662e 7461 7267 6574  '] = self.target
-000d9890: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000d98a0: 2e74 7970 6520 6973 206e 6f74 204e 6f6e  .type is not Non
-000d98b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000d98c0: 6573 756c 745b 2774 7970 6527 5d20 3d20  esult['type'] = 
-000d98d0: 7365 6c66 2e74 7970 650a 2020 2020 2020  self.type.      
-000d98e0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-000d98f0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-000d9900: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-000d9910: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-000d9920: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-000d9930: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000d9940: 7428 276f 7074 696f 6e73 2729 2069 7320  t('options') is 
-000d9950: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000d9960: 2020 2020 2020 7365 6c66 2e6f 7074 696f        self.optio
-000d9970: 6e73 203d 206d 2e67 6574 2827 6f70 7469  ns = m.get('opti
-000d9980: 6f6e 7327 290a 2020 2020 2020 2020 6966  ons').        if
-000d9990: 206d 2e67 6574 2827 7461 7267 6574 2729   m.get('target')
-000d99a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000d99b0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000d99c0: 6172 6765 7420 3d20 6d2e 6765 7428 2774  arget = m.get('t
-000d99d0: 6172 6765 7427 290a 2020 2020 2020 2020  arget').        
-000d99e0: 6966 206d 2e67 6574 2827 7479 7065 2729  if m.get('type')
-000d99f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000d9a00: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000d9a10: 7970 6520 3d20 6d2e 6765 7428 2774 7970  ype = m.get('typ
-000d9a20: 6527 290a 2020 2020 2020 2020 7265 7475  e').        retu
-000d9a30: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000d9a40: 5275 6e43 6c75 7374 6572 4368 6563 6b52  RunClusterCheckR
-000d9a50: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-000d9a60: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000d9a70: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000d9a80: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
-000d9a90: 6865 636b 5f69 643a 2073 7472 203d 204e  heck_id: str = N
-000d9aa0: 6f6e 652c 0a20 2020 2020 2020 2072 6571  one,.        req
-000d9ab0: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
-000d9ac0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000d9ad0: 2020 2020 2320 5468 6520 4944 206f 6620      # The ID of 
-000d9ae0: 7468 6520 636c 7573 7465 7220 6368 6563  the cluster chec
-000d9af0: 6b20 7461 736b 2e0a 2020 2020 2020 2020  k task..        
-000d9b00: 7365 6c66 2e63 6865 636b 5f69 6420 3d20  self.check_id = 
-000d9b10: 6368 6563 6b5f 6964 0a20 2020 2020 2020  check_id.       
-000d9b20: 2023 2049 6420 6f66 2074 6865 2072 6571   # Id of the req
-000d9b30: 7565 7374 0a20 2020 2020 2020 2073 656c  uest.        sel
-000d9b40: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
-000d9b50: 6571 7565 7374 5f69 640a 0a20 2020 2064  equest_id..    d
-000d9b60: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000d9b70: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000d9b80: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000d9b90: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000d9ba0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-000d9bb0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000d9bc0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000d9bd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000d9be0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000d9bf0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000d9c00: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000d9c10: 7365 6c66 2e63 6865 636b 5f69 6420 6973  self.check_id is
-000d9c20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000d9c30: 2020 2020 2020 2072 6573 756c 745b 2763         result['c
-000d9c40: 6865 636b 5f69 6427 5d20 3d20 7365 6c66  heck_id'] = self
-000d9c50: 2e63 6865 636b 5f69 640a 2020 2020 2020  .check_id.      
-000d9c60: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-000d9c70: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-000d9c80: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000d9c90: 7375 6c74 5b27 7265 7175 6573 745f 6964  sult['request_id
-000d9ca0: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-000d9cb0: 745f 6964 0a20 2020 2020 2020 2072 6574  t_id.        ret
-000d9cc0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000d9cd0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000d9ce0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000d9cf0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000d9d00: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000d9d10: 2020 2020 6966 206d 2e67 6574 2827 6368      if m.get('ch
-000d9d20: 6563 6b5f 6964 2729 2069 7320 6e6f 7420  eck_id') is not 
-000d9d30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000d9d40: 2020 7365 6c66 2e63 6865 636b 5f69 6420    self.check_id 
-000d9d50: 3d20 6d2e 6765 7428 2763 6865 636b 5f69  = m.get('check_i
-000d9d60: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-000d9d70: 2e67 6574 2827 7265 7175 6573 745f 6964  .get('request_id
-000d9d80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000d9d90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000d9da0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
-000d9db0: 6765 7428 2772 6571 7565 7374 5f69 6427  get('request_id'
-000d9dc0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000d9dd0: 2073 656c 660a 0a0a 636c 6173 7320 5275   self...class Ru
-000d9de0: 6e43 6c75 7374 6572 4368 6563 6b52 6573  nClusterCheckRes
-000d9df0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-000d9e00: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000d9e10: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-000d9e20: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-000d9e30: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-000d9e40: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000d9e50: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-000d9e60: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-000d9e70: 2020 626f 6479 3a20 5275 6e43 6c75 7374    body: RunClust
-000d9e80: 6572 4368 6563 6b52 6573 706f 6e73 6542  erCheckResponseB
-000d9e90: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
-000d9ea0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000d9eb0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-000d9ec0: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-000d9ed0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-000d9ee0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-000d9ef0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-000d9f00: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-000d9f10: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000d9f20: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-000d9f30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000d9f40: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-000d9f50: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000d9f60: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000d9f70: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000d9f80: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000d9f90: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000d9fa0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000d9fb0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000d9fc0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000d9fd0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000d9fe0: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-000d9ff0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000da000: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000da010: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-000da020: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-000da030: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-000da040: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-000da050: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000da060: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-000da070: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-000da080: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-000da090: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-000da0a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000da0b0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-000da0c0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-000da0d0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000da0e0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000da0f0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000da100: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-000da110: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-000da120: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000da130: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000da140: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-000da150: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000da160: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-000da170: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-000da180: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-000da190: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-000da1a0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000da1b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000da1c0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-000da1d0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-000da1e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000da1f0: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+000d7fd0: 6571 7565 7374 4f70 6572 6174 696f 6e73  equestOperations
+000d7fe0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000d7ff0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000d8000: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000d8010: 2020 2020 6172 6773 3a20 4c69 7374 5b73      args: List[s
+000d8020: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+000d8030: 2020 2020 6f70 6572 6174 696f 6e5f 6964      operation_id
+000d8040: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000d8050: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+000d8060: 662e 6172 6773 203d 2061 7267 730a 2020  f.args = args.  
+000d8070: 2020 2020 2020 7365 6c66 2e6f 7065 7261        self.opera
+000d8080: 7469 6f6e 5f69 6420 3d20 6f70 6572 6174  tion_id = operat
+000d8090: 696f 6e5f 6964 0a0a 2020 2020 6465 6620  ion_id..    def 
+000d80a0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000d80b0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000d80c0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000d80d0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000d80e0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000d80f0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000d8100: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000d8110: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000d8120: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000d8130: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000d8140: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000d8150: 662e 6172 6773 2069 7320 6e6f 7420 4e6f  f.args is not No
+000d8160: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000d8170: 7265 7375 6c74 5b27 6172 6773 275d 203d  result['args'] =
+000d8180: 2073 656c 662e 6172 6773 0a20 2020 2020   self.args.     
+000d8190: 2020 2069 6620 7365 6c66 2e6f 7065 7261     if self.opera
+000d81a0: 7469 6f6e 5f69 6420 6973 206e 6f74 204e  tion_id is not N
+000d81b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000d81c0: 2072 6573 756c 745b 276f 7065 7261 7469   result['operati
+000d81d0: 6f6e 5f69 6427 5d20 3d20 7365 6c66 2e6f  on_id'] = self.o
+000d81e0: 7065 7261 7469 6f6e 5f69 640a 2020 2020  peration_id.    
+000d81f0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000d8200: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000d8210: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000d8220: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000d8230: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000d8240: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+000d8250: 6765 7428 2761 7267 7327 2920 6973 206e  get('args') is n
+000d8260: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000d8270: 2020 2020 2073 656c 662e 6172 6773 203d       self.args =
+000d8280: 206d 2e67 6574 2827 6172 6773 2729 0a20   m.get('args'). 
+000d8290: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000d82a0: 276f 7065 7261 7469 6f6e 5f69 6427 2920  'operation_id') 
+000d82b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000d82c0: 2020 2020 2020 2020 2073 656c 662e 6f70           self.op
+000d82d0: 6572 6174 696f 6e5f 6964 203d 206d 2e67  eration_id = m.g
+000d82e0: 6574 2827 6f70 6572 6174 696f 6e5f 6964  et('operation_id
+000d82f0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+000d8300: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2052  n self...class R
+000d8310: 6570 6169 7243 6c75 7374 6572 4e6f 6465  epairClusterNode
+000d8320: 506f 6f6c 5265 7175 6573 7428 5465 614d  PoolRequest(TeaM
+000d8330: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+000d8340: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000d8350: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
+000d8360: 7574 6f5f 7265 7374 6172 743a 2062 6f6f  uto_restart: boo
+000d8370: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
+000d8380: 2020 6e6f 6465 733a 204c 6973 745b 7374    nodes: List[st
+000d8390: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+000d83a0: 2020 206f 7065 7261 7469 6f6e 733a 204c     operations: L
+000d83b0: 6973 745b 5265 7061 6972 436c 7573 7465  ist[RepairCluste
+000d83c0: 724e 6f64 6550 6f6f 6c52 6571 7565 7374  rNodePoolRequest
+000d83d0: 4f70 6572 6174 696f 6e73 5d20 3d20 4e6f  Operations] = No
+000d83e0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000d83f0: 2020 2073 656c 662e 6175 746f 5f72 6573     self.auto_res
+000d8400: 7461 7274 203d 2061 7574 6f5f 7265 7374  tart = auto_rest
+000d8410: 6172 740a 2020 2020 2020 2020 2320 5468  art.        # Th
+000d8420: 6520 6c69 7374 206f 6620 6e6f 6465 732e  e list of nodes.
+000d8430: 2049 6620 796f 7520 646f 206e 6f74 2073   If you do not s
+000d8440: 7065 6369 6679 206e 6f64 6573 2c20 616c  pecify nodes, al
+000d8450: 6c20 6e6f 6465 7320 696e 2074 6865 206e  l nodes in the n
+000d8460: 6f64 6520 706f 6f6c 2061 7265 2073 656c  ode pool are sel
+000d8470: 6563 7465 642e 0a20 2020 2020 2020 2073  ected..        s
+000d8480: 656c 662e 6e6f 6465 7320 3d20 6e6f 6465  elf.nodes = node
+000d8490: 730a 2020 2020 2020 2020 7365 6c66 2e6f  s.        self.o
+000d84a0: 7065 7261 7469 6f6e 7320 3d20 6f70 6572  perations = oper
+000d84b0: 6174 696f 6e73 0a0a 2020 2020 6465 6620  ations..    def 
+000d84c0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000d84d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000d84e0: 6f70 6572 6174 696f 6e73 3a0a 2020 2020  operations:.    
+000d84f0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+000d8500: 2073 656c 662e 6f70 6572 6174 696f 6e73   self.operations
+000d8510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000d8520: 2020 6966 206b 3a0a 2020 2020 2020 2020    if k:.        
+000d8530: 2020 2020 2020 2020 2020 2020 6b2e 7661              k.va
+000d8540: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+000d8550: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000d8560: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000d8570: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000d8580: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000d8590: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000d85a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000d85b0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000d85c0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000d85d0: 2020 2020 2020 6966 2073 656c 662e 6175        if self.au
+000d85e0: 746f 5f72 6573 7461 7274 2069 7320 6e6f  to_restart is no
+000d85f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000d8600: 2020 2020 7265 7375 6c74 5b27 6175 746f      result['auto
+000d8610: 5f72 6573 7461 7274 275d 203d 2073 656c  _restart'] = sel
+000d8620: 662e 6175 746f 5f72 6573 7461 7274 0a20  f.auto_restart. 
+000d8630: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+000d8640: 6f64 6573 2069 7320 6e6f 7420 4e6f 6e65  odes is not None
+000d8650: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000d8660: 7375 6c74 5b27 6e6f 6465 7327 5d20 3d20  sult['nodes'] = 
+000d8670: 7365 6c66 2e6e 6f64 6573 0a20 2020 2020  self.nodes.     
+000d8680: 2020 2072 6573 756c 745b 276f 7065 7261     result['opera
+000d8690: 7469 6f6e 7327 5d20 3d20 5b5d 0a20 2020  tions'] = [].   
+000d86a0: 2020 2020 2069 6620 7365 6c66 2e6f 7065       if self.ope
+000d86b0: 7261 7469 6f6e 7320 6973 206e 6f74 204e  rations is not N
+000d86c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000d86d0: 2066 6f72 206b 2069 6e20 7365 6c66 2e6f   for k in self.o
+000d86e0: 7065 7261 7469 6f6e 733a 0a20 2020 2020  perations:.     
+000d86f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000d8700: 745b 276f 7065 7261 7469 6f6e 7327 5d2e  t['operations'].
+000d8710: 6170 7065 6e64 286b 2e74 6f5f 6d61 7028  append(k.to_map(
+000d8720: 2920 6966 206b 2065 6c73 6520 4e6f 6e65  ) if k else None
+000d8730: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000d8740: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+000d8750: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+000d8760: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+000d8770: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+000d8780: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+000d8790: 2069 6620 6d2e 6765 7428 2761 7574 6f5f   if m.get('auto_
+000d87a0: 7265 7374 6172 7427 2920 6973 206e 6f74  restart') is not
+000d87b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000d87c0: 2020 2073 656c 662e 6175 746f 5f72 6573     self.auto_res
+000d87d0: 7461 7274 203d 206d 2e67 6574 2827 6175  tart = m.get('au
+000d87e0: 746f 5f72 6573 7461 7274 2729 0a20 2020  to_restart').   
+000d87f0: 2020 2020 2069 6620 6d2e 6765 7428 276e       if m.get('n
+000d8800: 6f64 6573 2729 2069 7320 6e6f 7420 4e6f  odes') is not No
+000d8810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000d8820: 7365 6c66 2e6e 6f64 6573 203d 206d 2e67  self.nodes = m.g
+000d8830: 6574 2827 6e6f 6465 7327 290a 2020 2020  et('nodes').    
+000d8840: 2020 2020 7365 6c66 2e6f 7065 7261 7469      self.operati
+000d8850: 6f6e 7320 3d20 5b5d 0a20 2020 2020 2020  ons = [].       
+000d8860: 2069 6620 6d2e 6765 7428 276f 7065 7261   if m.get('opera
+000d8870: 7469 6f6e 7327 2920 6973 206e 6f74 204e  tions') is not N
+000d8880: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000d8890: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
+000d88a0: 276f 7065 7261 7469 6f6e 7327 293a 0a20  'operations'):. 
+000d88b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000d88c0: 656d 705f 6d6f 6465 6c20 3d20 5265 7061  emp_model = Repa
+000d88d0: 6972 436c 7573 7465 724e 6f64 6550 6f6f  irClusterNodePoo
+000d88e0: 6c52 6571 7565 7374 4f70 6572 6174 696f  lRequestOperatio
+000d88f0: 6e73 2829 0a20 2020 2020 2020 2020 2020  ns().           
+000d8900: 2020 2020 2073 656c 662e 6f70 6572 6174       self.operat
+000d8910: 696f 6e73 2e61 7070 656e 6428 7465 6d70  ions.append(temp
+000d8920: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+000d8930: 6b29 290a 2020 2020 2020 2020 7265 7475  k)).        retu
+000d8940: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000d8950: 5265 7061 6972 436c 7573 7465 724e 6f64  RepairClusterNod
+000d8960: 6550 6f6f 6c52 6573 706f 6e73 6542 6f64  ePoolResponseBod
+000d8970: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+000d8980: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000d8990: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000d89a0: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
+000d89b0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000d89c0: 2020 2020 2074 6173 6b5f 6964 3a20 7374       task_id: st
+000d89d0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
+000d89e0: 0a20 2020 2020 2020 2023 2054 6865 2072  .        # The r
+000d89f0: 6571 7565 7374 2049 442e 0a20 2020 2020  equest ID..     
+000d8a00: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+000d8a10: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
+000d8a20: 2020 2020 2020 2020 2320 5468 6520 4944          # The ID
+000d8a30: 206f 6620 7468 6520 7461 736b 2e0a 2020   of the task..  
+000d8a40: 2020 2020 2020 7365 6c66 2e74 6173 6b5f        self.task_
+000d8a50: 6964 203d 2074 6173 6b5f 6964 0a0a 2020  id = task_id..  
+000d8a60: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000d8a70: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+000d8a80: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+000d8a90: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+000d8aa0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+000d8ab0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000d8ac0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+000d8ad0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000d8ae0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000d8af0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000d8b00: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000d8b10: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+000d8b20: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000d8b30: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000d8b40: 6c74 5b27 7265 7175 6573 745f 6964 275d  lt['request_id']
+000d8b50: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+000d8b60: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+000d8b70: 6c66 2e74 6173 6b5f 6964 2069 7320 6e6f  lf.task_id is no
+000d8b80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000d8b90: 2020 2020 7265 7375 6c74 5b27 7461 736b      result['task
+000d8ba0: 5f69 6427 5d20 3d20 7365 6c66 2e74 6173  _id'] = self.tas
+000d8bb0: 6b5f 6964 0a20 2020 2020 2020 2072 6574  k_id.        ret
+000d8bc0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000d8bd0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000d8be0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000d8bf0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000d8c00: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000d8c10: 2020 2020 6966 206d 2e67 6574 2827 7265      if m.get('re
+000d8c20: 7175 6573 745f 6964 2729 2069 7320 6e6f  quest_id') is no
+000d8c30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000d8c40: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+000d8c50: 5f69 6420 3d20 6d2e 6765 7428 2772 6571  _id = m.get('req
+000d8c60: 7565 7374 5f69 6427 290a 2020 2020 2020  uest_id').      
+000d8c70: 2020 6966 206d 2e67 6574 2827 7461 736b    if m.get('task
+000d8c80: 5f69 6427 2920 6973 206e 6f74 204e 6f6e  _id') is not Non
+000d8c90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000d8ca0: 656c 662e 7461 736b 5f69 6420 3d20 6d2e  elf.task_id = m.
+000d8cb0: 6765 7428 2774 6173 6b5f 6964 2729 0a20  get('task_id'). 
+000d8cc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000d8cd0: 6c66 0a0a 0a63 6c61 7373 2052 6570 6169  lf...class Repai
+000d8ce0: 7243 6c75 7374 6572 4e6f 6465 506f 6f6c  rClusterNodePool
+000d8cf0: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+000d8d00: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000d8d10: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000d8d20: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
+000d8d30: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
+000d8d40: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+000d8d50: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
+000d8d60: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+000d8d70: 2020 2020 2062 6f64 793a 2052 6570 6169       body: Repai
+000d8d80: 7243 6c75 7374 6572 4e6f 6465 506f 6f6c  rClusterNodePool
+000d8d90: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
+000d8da0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+000d8db0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000d8dc0: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+000d8dd0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000d8de0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+000d8df0: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
+000d8e00: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
+000d8e10: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+000d8e20: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+000d8e30: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+000d8e40: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+000d8e50: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+000d8e60: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000d8e70: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000d8e80: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+000d8e90: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000d8ea0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000d8eb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000d8ec0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000d8ed0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000d8ee0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000d8ef0: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+000d8f00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000d8f10: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+000d8f20: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+000d8f30: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+000d8f40: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+000d8f50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000d8f60: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+000d8f70: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+000d8f80: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+000d8f90: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+000d8fa0: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+000d8fb0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000d8fc0: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+000d8fd0: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+000d8fe0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000d8ff0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000d9000: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000d9010: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000d9020: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000d9030: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000d9040: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+000d9050: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+000d9060: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000d9070: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+000d9080: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+000d9090: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+000d90a0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+000d90b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000d90c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000d90d0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+000d90e0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+000d90f0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+000d9100: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+000d9110: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+000d9120: 6d70 5f6d 6f64 656c 203d 2052 6570 6169  mp_model = Repai
+000d9130: 7243 6c75 7374 6572 4e6f 6465 506f 6f6c  rClusterNodePool
+000d9140: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
+000d9150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000d9160: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+000d9170: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+000d9180: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+000d9190: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+000d91a0: 7320 5265 7375 6d65 436f 6d70 6f6e 656e  s ResumeComponen
+000d91b0: 7455 7067 7261 6465 5265 7370 6f6e 7365  tUpgradeResponse
+000d91c0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000d91d0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000d91e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000d91f0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+000d9200: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+000d9210: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+000d9220: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+000d9230: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+000d9240: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000d9250: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+000d9260: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000d9270: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+000d9280: 650a 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
+000d9290: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000d92a0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000d92b0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000d92c0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000d92d0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000d92e0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000d92f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000d9300: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000d9310: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000d9320: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000d9330: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+000d9340: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+000d9350: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000d9360: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+000d9370: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+000d9380: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000d9390: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+000d93a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000d93b0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+000d93c0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+000d93d0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+000d93e0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000d93f0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000d9400: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000d9410: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000d9420: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000d9430: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+000d9440: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+000d9450: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000d9460: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000d9470: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+000d9480: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+000d9490: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+000d94a0: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+000d94b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000d94c0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000d94d0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+000d94e0: 436f 6465 2729 0a20 2020 2020 2020 2072  Code').        r
+000d94f0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000d9500: 7373 2052 6573 756d 6554 6173 6b52 6573  ss ResumeTaskRes
+000d9510: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
+000d9520: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000d9530: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+000d9540: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+000d9550: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
+000d9560: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000d9570: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
+000d9580: 7420 3d20 4e6f 6e65 2c0a 2020 2020 293a  t = None,.    ):
+000d9590: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000d95a0: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+000d95b0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000d95c0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+000d95d0: 735f 636f 6465 0a0a 2020 2020 6465 6620  s_code..    def 
+000d95e0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000d95f0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000d9600: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000d9610: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000d9620: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000d9630: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000d9640: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000d9650: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000d9660: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000d9670: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000d9680: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000d9690: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+000d96a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000d96b0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+000d96c0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+000d96d0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+000d96e0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+000d96f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000d9700: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000d9710: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+000d9720: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000d9730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000d9740: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000d9750: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000d9760: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000d9770: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000d9780: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000d9790: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+000d97a0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+000d97b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000d97c0: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+000d97d0: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+000d97e0: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+000d97f0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+000d9800: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000d9810: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000d9820: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+000d9830: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+000d9840: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000d9850: 0a0a 636c 6173 7320 5265 7375 6d65 5570  ..class ResumeUp
+000d9860: 6772 6164 6543 6c75 7374 6572 5265 7370  gradeClusterResp
+000d9870: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+000d9880: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000d9890: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000d98a0: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+000d98b0: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
+000d98c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000d98d0: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
+000d98e0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+000d98f0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000d9900: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+000d9910: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000d9920: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+000d9930: 5f63 6f64 650a 0a20 2020 2064 6566 2076  _code..    def v
+000d9940: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000d9950: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000d9960: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000d9970: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000d9980: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000d9990: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000d99a0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+000d99b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000d99c0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+000d99d0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+000d99e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000d99f0: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+000d9a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000d9a10: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+000d9a20: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+000d9a30: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+000d9a40: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+000d9a50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000d9a60: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000d9a70: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+000d9a80: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+000d9a90: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000d9aa0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+000d9ab0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+000d9ac0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+000d9ad0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+000d9ae0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000d9af0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+000d9b00: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000d9b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000d9b20: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+000d9b30: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+000d9b40: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+000d9b50: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+000d9b60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000d9b70: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+000d9b80: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+000d9b90: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+000d9ba0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+000d9bb0: 0a63 6c61 7373 2052 756e 436c 7573 7465  .class RunCluste
+000d9bc0: 7243 6865 636b 5265 7175 6573 7428 5465  rCheckRequest(Te
+000d9bd0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+000d9be0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000d9bf0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000d9c00: 206f 7074 696f 6e73 3a20 4469 6374 5b73   options: Dict[s
+000d9c10: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
+000d9c20: 0a20 2020 2020 2020 2074 6172 6765 743a  .        target:
+000d9c30: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000d9c40: 2020 2020 2074 7970 653a 2073 7472 203d       type: str =
+000d9c50: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000d9c60: 2020 2020 2020 2320 5468 6520 636c 7573        # The clus
+000d9c70: 7465 7220 6368 6563 6b20 6974 656d 732e  ter check items.
+000d9c80: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+000d9c90: 7469 6f6e 7320 3d20 6f70 7469 6f6e 730a  tions = options.
+000d9ca0: 2020 2020 2020 2020 7365 6c66 2e74 6172          self.tar
+000d9cb0: 6765 7420 3d20 7461 7267 6574 0a20 2020  get = target.   
+000d9cc0: 2020 2020 2023 2054 6865 2063 6865 636b       # The check
+000d9cd0: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
+000d9ce0: 2023 200a 2020 2020 2020 2020 2320 5468   # .        # Th
+000d9cf0: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
+000d9d00: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
+000d9d10: 2020 7365 6c66 2e74 7970 6520 3d20 7479    self.type = ty
+000d9d20: 7065 0a0a 2020 2020 6465 6620 7661 6c69  pe..    def vali
+000d9d30: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000d9d40: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000d9d50: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000d9d60: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000d9d70: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000d9d80: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000d9d90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000d9da0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000d9db0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000d9dc0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000d9dd0: 2020 2020 2020 6966 2073 656c 662e 6f70        if self.op
+000d9de0: 7469 6f6e 7320 6973 206e 6f74 204e 6f6e  tions is not Non
+000d9df0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000d9e00: 6573 756c 745b 276f 7074 696f 6e73 275d  esult['options']
+000d9e10: 203d 2073 656c 662e 6f70 7469 6f6e 730a   = self.options.
+000d9e20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000d9e30: 7461 7267 6574 2069 7320 6e6f 7420 4e6f  target is not No
+000d9e40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000d9e50: 7265 7375 6c74 5b27 7461 7267 6574 275d  result['target']
+000d9e60: 203d 2073 656c 662e 7461 7267 6574 0a20   = self.target. 
+000d9e70: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+000d9e80: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
+000d9e90: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000d9ea0: 756c 745b 2774 7970 6527 5d20 3d20 7365  ult['type'] = se
+000d9eb0: 6c66 2e74 7970 650a 2020 2020 2020 2020  lf.type.        
+000d9ec0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+000d9ed0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+000d9ee0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+000d9ef0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+000d9f00: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000d9f10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000d9f20: 276f 7074 696f 6e73 2729 2069 7320 6e6f  'options') is no
+000d9f30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000d9f40: 2020 2020 7365 6c66 2e6f 7074 696f 6e73      self.options
+000d9f50: 203d 206d 2e67 6574 2827 6f70 7469 6f6e   = m.get('option
+000d9f60: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000d9f70: 2e67 6574 2827 7461 7267 6574 2729 2069  .get('target') i
+000d9f80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000d9f90: 2020 2020 2020 2020 7365 6c66 2e74 6172          self.tar
+000d9fa0: 6765 7420 3d20 6d2e 6765 7428 2774 6172  get = m.get('tar
+000d9fb0: 6765 7427 290a 2020 2020 2020 2020 6966  get').        if
+000d9fc0: 206d 2e67 6574 2827 7479 7065 2729 2069   m.get('type') i
+000d9fd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000d9fe0: 2020 2020 2020 2020 7365 6c66 2e74 7970          self.typ
+000d9ff0: 6520 3d20 6d2e 6765 7428 2774 7970 6527  e = m.get('type'
+000da000: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000da010: 2073 656c 660a 0a0a 636c 6173 7320 5275   self...class Ru
+000da020: 6e43 6c75 7374 6572 4368 6563 6b52 6573  nClusterCheckRes
+000da030: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+000da040: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000da050: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000da060: 656c 662c 0a20 2020 2020 2020 2063 6865  elf,.        che
+000da070: 636b 5f69 643a 2073 7472 203d 204e 6f6e  ck_id: str = Non
+000da080: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
+000da090: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+000da0a0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000da0b0: 2020 2320 5468 6520 4944 206f 6620 7468    # The ID of th
+000da0c0: 6520 636c 7573 7465 7220 6368 6563 6b20  e cluster check 
+000da0d0: 7461 736b 2e0a 2020 2020 2020 2020 7365  task..        se
+000da0e0: 6c66 2e63 6865 636b 5f69 6420 3d20 6368  lf.check_id = ch
+000da0f0: 6563 6b5f 6964 0a20 2020 2020 2020 2023  eck_id.        #
+000da100: 2049 6420 6f66 2074 6865 2072 6571 7565   Id of the reque
+000da110: 7374 0a20 2020 2020 2020 2073 656c 662e  st.        self.
+000da120: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+000da130: 7565 7374 5f69 640a 0a20 2020 2064 6566  uest_id..    def
+000da140: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+000da150: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000da160: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000da170: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000da180: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+000da190: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+000da1a0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+000da1b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000da1c0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+000da1d0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+000da1e0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+000da1f0: 6c66 2e63 6865 636b 5f69 6420 6973 206e  lf.check_id is n
 000da200: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000da210: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-000da220: 3d20 5275 6e43 6c75 7374 6572 4368 6563  = RunClusterChec
-000da230: 6b52 6573 706f 6e73 6542 6f64 7928 290a  kResponseBody().
-000da240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000da250: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-000da260: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-000da270: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-000da280: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-000da290: 7373 2053 6361 6c65 436c 7573 7465 7252  ss ScaleClusterR
-000da2a0: 6571 7565 7374 5461 6773 2854 6561 4d6f  equestTags(TeaMo
-000da2b0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-000da2c0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000da2d0: 7365 6c66 2c0a 2020 2020 2020 2020 6b65  self,.        ke
-000da2e0: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
-000da2f0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-000da300: 6c66 2e6b 6579 203d 206b 6579 0a0a 2020  lf.key = key..  
-000da310: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-000da320: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000da330: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-000da340: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-000da350: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-000da360: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-000da370: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-000da380: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000da390: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-000da3a0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000da3b0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000da3c0: 6966 2073 656c 662e 6b65 7920 6973 206e  if self.key is n
-000da3d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000da3e0: 2020 2020 2072 6573 756c 745b 276b 6579       result['key
-000da3f0: 275d 203d 2073 656c 662e 6b65 790a 2020  '] = self.key.  
-000da400: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000da410: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-000da420: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-000da430: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-000da440: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-000da450: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000da460: 6d2e 6765 7428 276b 6579 2729 2069 7320  m.get('key') is 
-000da470: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000da480: 2020 2020 2020 7365 6c66 2e6b 6579 203d        self.key =
-000da490: 206d 2e67 6574 2827 6b65 7927 290a 2020   m.get('key').  
-000da4a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000da4b0: 660a 0a0a 636c 6173 7320 5363 616c 6543  f...class ScaleC
-000da4c0: 6c75 7374 6572 5265 7175 6573 7454 6169  lusterRequestTai
-000da4d0: 6e74 7328 5465 614d 6f64 656c 293a 0a20  nts(TeaModel):. 
-000da4e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000da4f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000da500: 2020 2020 2020 2065 6666 6563 743a 2073         effect: s
-000da510: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000da520: 2020 206b 6579 3a20 7374 7220 3d20 4e6f     key: str = No
-000da530: 6e65 2c0a 2020 2020 2020 2020 7661 6c75  ne,.        valu
-000da540: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-000da550: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-000da560: 6c66 2e65 6666 6563 7420 3d20 6566 6665  lf.effect = effe
-000da570: 6374 0a20 2020 2020 2020 2073 656c 662e  ct.        self.
-000da580: 6b65 7920 3d20 6b65 790a 2020 2020 2020  key = key.      
-000da590: 2020 7365 6c66 2e76 616c 7565 203d 2076    self.value = v
-000da5a0: 616c 7565 0a0a 2020 2020 6465 6620 7661  alue..    def va
-000da5b0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000da5c0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000da5d0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000da5e0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000da5f0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-000da600: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-000da610: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000da620: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000da630: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-000da640: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000da650: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000da660: 6566 6665 6374 2069 7320 6e6f 7420 4e6f  effect is not No
-000da670: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000da680: 7265 7375 6c74 5b27 6566 6665 6374 275d  result['effect']
-000da690: 203d 2073 656c 662e 6566 6665 6374 0a20   = self.effect. 
-000da6a0: 2020 2020 2020 2069 6620 7365 6c66 2e6b         if self.k
-000da6b0: 6579 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ey is not None:.
-000da6c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000da6d0: 6c74 5b27 6b65 7927 5d20 3d20 7365 6c66  lt['key'] = self
-000da6e0: 2e6b 6579 0a20 2020 2020 2020 2069 6620  .key.        if 
-000da6f0: 7365 6c66 2e76 616c 7565 2069 7320 6e6f  self.value is no
-000da700: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000da710: 2020 2020 7265 7375 6c74 5b27 7661 6c75      result['valu
-000da720: 6527 5d20 3d20 7365 6c66 2e76 616c 7565  e'] = self.value
-000da730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000da740: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-000da750: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-000da760: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-000da770: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000da780: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000da790: 6966 206d 2e67 6574 2827 6566 6665 6374  if m.get('effect
-000da7a0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000da7b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000da7c0: 2e65 6666 6563 7420 3d20 6d2e 6765 7428  .effect = m.get(
-000da7d0: 2765 6666 6563 7427 290a 2020 2020 2020  'effect').      
-000da7e0: 2020 6966 206d 2e67 6574 2827 6b65 7927    if m.get('key'
-000da7f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000da800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000da810: 6b65 7920 3d20 6d2e 6765 7428 276b 6579  key = m.get('key
-000da820: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000da830: 6765 7428 2776 616c 7565 2729 2069 7320  get('value') is 
-000da840: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000da850: 2020 2020 2020 7365 6c66 2e76 616c 7565        self.value
-000da860: 203d 206d 2e67 6574 2827 7661 6c75 6527   = m.get('value'
-000da870: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000da880: 2073 656c 660a 0a0a 636c 6173 7320 5363   self...class Sc
-000da890: 616c 6543 6c75 7374 6572 5265 7175 6573  aleClusterReques
-000da8a0: 7457 6f72 6b65 7244 6174 6144 6973 6b73  tWorkerDataDisks
-000da8b0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-000da8c0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-000da8d0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000da8e0: 2020 2020 6361 7465 676f 7279 3a20 7374      category: st
-000da8f0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000da900: 2020 656e 6372 7970 7465 643a 2073 7472    encrypted: str
-000da910: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000da920: 2073 697a 653a 2073 7472 203d 204e 6f6e   size: str = Non
-000da930: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-000da940: 2020 7365 6c66 2e63 6174 6567 6f72 7920    self.category 
-000da950: 3d20 6361 7465 676f 7279 0a20 2020 2020  = category.     
-000da960: 2020 2073 656c 662e 656e 6372 7970 7465     self.encrypte
-000da970: 6420 3d20 656e 6372 7970 7465 640a 2020  d = encrypted.  
-000da980: 2020 2020 2020 7365 6c66 2e73 697a 6520        self.size 
-000da990: 3d20 7369 7a65 0a0a 2020 2020 6465 6620  = size..    def 
-000da9a0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000da9b0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000da9c0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000da9d0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-000da9e0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-000da9f0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-000daa00: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-000daa10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000daa20: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-000daa30: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-000daa40: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000daa50: 662e 6361 7465 676f 7279 2069 7320 6e6f  f.category is no
-000daa60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000daa70: 2020 2020 7265 7375 6c74 5b27 6361 7465      result['cate
-000daa80: 676f 7279 275d 203d 2073 656c 662e 6361  gory'] = self.ca
-000daa90: 7465 676f 7279 0a20 2020 2020 2020 2069  tegory.        i
-000daaa0: 6620 7365 6c66 2e65 6e63 7279 7074 6564  f self.encrypted
-000daab0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000daac0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000daad0: 5b27 656e 6372 7970 7465 6427 5d20 3d20  ['encrypted'] = 
-000daae0: 7365 6c66 2e65 6e63 7279 7074 6564 0a20  self.encrypted. 
-000daaf0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000dab00: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
-000dab10: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000dab20: 756c 745b 2773 697a 6527 5d20 3d20 7365  ult['size'] = se
-000dab30: 6c66 2e73 697a 650a 2020 2020 2020 2020  lf.size.        
-000dab40: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000dab50: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000dab60: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-000dab70: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-000dab80: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000dab90: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000daba0: 2763 6174 6567 6f72 7927 2920 6973 206e  'category') is n
-000dabb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000dabc0: 2020 2020 2073 656c 662e 6361 7465 676f       self.catego
-000dabd0: 7279 203d 206d 2e67 6574 2827 6361 7465  ry = m.get('cate
-000dabe0: 676f 7279 2729 0a20 2020 2020 2020 2069  gory').        i
-000dabf0: 6620 6d2e 6765 7428 2765 6e63 7279 7074  f m.get('encrypt
-000dac00: 6564 2729 2069 7320 6e6f 7420 4e6f 6e65  ed') is not None
-000dac10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000dac20: 6c66 2e65 6e63 7279 7074 6564 203d 206d  lf.encrypted = m
-000dac30: 2e67 6574 2827 656e 6372 7970 7465 6427  .get('encrypted'
-000dac40: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000dac50: 6574 2827 7369 7a65 2729 2069 7320 6e6f  et('size') is no
-000dac60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000dac70: 2020 2020 7365 6c66 2e73 697a 6520 3d20      self.size = 
-000dac80: 6d2e 6765 7428 2773 697a 6527 290a 2020  m.get('size').  
-000dac90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000daca0: 660a 0a0a 636c 6173 7320 5363 616c 6543  f...class ScaleC
-000dacb0: 6c75 7374 6572 5265 7175 6573 7428 5465  lusterRequest(Te
-000dacc0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-000dacd0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-000dace0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000dacf0: 2063 6c6f 7564 5f6d 6f6e 6974 6f72 5f66   cloud_monitor_f
-000dad00: 6c61 6773 3a20 626f 6f6c 203d 204e 6f6e  lags: bool = Non
-000dad10: 652c 0a20 2020 2020 2020 2063 6f75 6e74  e,.        count
-000dad20: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-000dad30: 2020 2020 2020 6370 755f 706f 6c69 6379        cpu_policy
-000dad40: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000dad50: 2020 2020 2020 6469 7361 626c 655f 726f        disable_ro
-000dad60: 6c6c 6261 636b 3a20 626f 6f6c 203d 204e  llback: bool = N
-000dad70: 6f6e 652c 0a20 2020 2020 2020 206b 6579  one,.        key
-000dad80: 5f70 6169 723a 2073 7472 203d 204e 6f6e  _pair: str = Non
-000dad90: 652c 0a20 2020 2020 2020 206c 6f67 696e  e,.        login
-000dada0: 5f70 6173 7377 6f72 643a 2073 7472 203d  _password: str =
-000dadb0: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
-000dadc0: 6167 733a 204c 6973 745b 5363 616c 6543  ags: List[ScaleC
-000dadd0: 6c75 7374 6572 5265 7175 6573 7454 6167  lusterRequestTag
-000dade0: 735d 203d 204e 6f6e 652c 0a20 2020 2020  s] = None,.     
-000dadf0: 2020 2074 6169 6e74 733a 204c 6973 745b     taints: List[
-000dae00: 5363 616c 6543 6c75 7374 6572 5265 7175  ScaleClusterRequ
-000dae10: 6573 7454 6169 6e74 735d 203d 204e 6f6e  estTaints] = Non
-000dae20: 652c 0a20 2020 2020 2020 2076 7377 6974  e,.        vswit
-000dae30: 6368 5f69 6473 3a20 4c69 7374 5b73 7472  ch_ids: List[str
-000dae40: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000dae50: 2020 776f 726b 6572 5f61 7574 6f5f 7265    worker_auto_re
-000dae60: 6e65 773a 2062 6f6f 6c20 3d20 4e6f 6e65  new: bool = None
-000dae70: 2c0a 2020 2020 2020 2020 776f 726b 6572  ,.        worker
-000dae80: 5f61 7574 6f5f 7265 6e65 775f 7065 7269  _auto_renew_peri
-000dae90: 6f64 3a20 696e 7420 3d20 4e6f 6e65 2c0a  od: int = None,.
-000daea0: 2020 2020 2020 2020 776f 726b 6572 5f64          worker_d
-000daeb0: 6174 615f 6469 736b 3a20 626f 6f6c 203d  ata_disk: bool =
-000daec0: 204e 6f6e 652c 0a20 2020 2020 2020 2077   None,.        w
-000daed0: 6f72 6b65 725f 6461 7461 5f64 6973 6b73  orker_data_disks
-000daee0: 3a20 4c69 7374 5b53 6361 6c65 436c 7573  : List[ScaleClus
-000daef0: 7465 7252 6571 7565 7374 576f 726b 6572  terRequestWorker
-000daf00: 4461 7461 4469 736b 735d 203d 204e 6f6e  DataDisks] = Non
-000daf10: 652c 0a20 2020 2020 2020 2077 6f72 6b65  e,.        worke
-000daf20: 725f 696e 7374 616e 6365 5f63 6861 7267  r_instance_charg
-000daf30: 655f 7479 7065 3a20 7374 7220 3d20 4e6f  e_type: str = No
-000daf40: 6e65 2c0a 2020 2020 2020 2020 776f 726b  ne,.        work
-000daf50: 6572 5f69 6e73 7461 6e63 655f 7479 7065  er_instance_type
-000daf60: 733a 204c 6973 745b 7374 725d 203d 204e  s: List[str] = N
-000daf70: 6f6e 652c 0a20 2020 2020 2020 2077 6f72  one,.        wor
-000daf80: 6b65 725f 7065 7269 6f64 3a20 696e 7420  ker_period: int 
-000daf90: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000dafa0: 776f 726b 6572 5f70 6572 696f 645f 756e  worker_period_un
-000dafb0: 6974 3a20 7374 7220 3d20 4e6f 6e65 2c0a  it: str = None,.
-000dafc0: 2020 2020 2020 2020 776f 726b 6572 5f73          worker_s
-000dafd0: 7973 7465 6d5f 6469 736b 5f63 6174 6567  ystem_disk_categ
-000dafe0: 6f72 793a 2073 7472 203d 204e 6f6e 652c  ory: str = None,
-000daff0: 0a20 2020 2020 2020 2077 6f72 6b65 725f  .        worker_
-000db000: 7379 7374 656d 5f64 6973 6b5f 7369 7a65  system_disk_size
-000db010: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-000db020: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-000db030: 662e 636c 6f75 645f 6d6f 6e69 746f 725f  f.cloud_monitor_
-000db040: 666c 6167 7320 3d20 636c 6f75 645f 6d6f  flags = cloud_mo
-000db050: 6e69 746f 725f 666c 6167 730a 2020 2020  nitor_flags.    
-000db060: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-000db070: 2063 6f75 6e74 0a20 2020 2020 2020 2073   count.        s
-000db080: 656c 662e 6370 755f 706f 6c69 6379 203d  elf.cpu_policy =
-000db090: 2063 7075 5f70 6f6c 6963 790a 2020 2020   cpu_policy.    
-000db0a0: 2020 2020 7365 6c66 2e64 6973 6162 6c65      self.disable
-000db0b0: 5f72 6f6c 6c62 6163 6b20 3d20 6469 7361  _rollback = disa
-000db0c0: 626c 655f 726f 6c6c 6261 636b 0a20 2020  ble_rollback.   
-000db0d0: 2020 2020 2073 656c 662e 6b65 795f 7061       self.key_pa
-000db0e0: 6972 203d 206b 6579 5f70 6169 720a 2020  ir = key_pair.  
-000db0f0: 2020 2020 2020 7365 6c66 2e6c 6f67 696e        self.login
-000db100: 5f70 6173 7377 6f72 6420 3d20 6c6f 6769  _password = logi
-000db110: 6e5f 7061 7373 776f 7264 0a20 2020 2020  n_password.     
-000db120: 2020 2073 656c 662e 7461 6773 203d 2074     self.tags = t
-000db130: 6167 730a 2020 2020 2020 2020 7365 6c66  ags.        self
-000db140: 2e74 6169 6e74 7320 3d20 7461 696e 7473  .taints = taints
-000db150: 0a20 2020 2020 2020 2073 656c 662e 7673  .        self.vs
-000db160: 7769 7463 685f 6964 7320 3d20 7673 7769  witch_ids = vswi
-000db170: 7463 685f 6964 730a 2020 2020 2020 2020  tch_ids.        
-000db180: 7365 6c66 2e77 6f72 6b65 725f 6175 746f  self.worker_auto
-000db190: 5f72 656e 6577 203d 2077 6f72 6b65 725f  _renew = worker_
-000db1a0: 6175 746f 5f72 656e 6577 0a20 2020 2020  auto_renew.     
-000db1b0: 2020 2073 656c 662e 776f 726b 6572 5f61     self.worker_a
-000db1c0: 7574 6f5f 7265 6e65 775f 7065 7269 6f64  uto_renew_period
-000db1d0: 203d 2077 6f72 6b65 725f 6175 746f 5f72   = worker_auto_r
-000db1e0: 656e 6577 5f70 6572 696f 640a 2020 2020  enew_period.    
-000db1f0: 2020 2020 7365 6c66 2e77 6f72 6b65 725f      self.worker_
-000db200: 6461 7461 5f64 6973 6b20 3d20 776f 726b  data_disk = work
-000db210: 6572 5f64 6174 615f 6469 736b 0a20 2020  er_data_disk.   
-000db220: 2020 2020 2073 656c 662e 776f 726b 6572       self.worker
-000db230: 5f64 6174 615f 6469 736b 7320 3d20 776f  _data_disks = wo
-000db240: 726b 6572 5f64 6174 615f 6469 736b 730a  rker_data_disks.
-000db250: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-000db260: 6b65 725f 696e 7374 616e 6365 5f63 6861  ker_instance_cha
-000db270: 7267 655f 7479 7065 203d 2077 6f72 6b65  rge_type = worke
-000db280: 725f 696e 7374 616e 6365 5f63 6861 7267  r_instance_charg
-000db290: 655f 7479 7065 0a20 2020 2020 2020 2073  e_type.        s
-000db2a0: 656c 662e 776f 726b 6572 5f69 6e73 7461  elf.worker_insta
-000db2b0: 6e63 655f 7479 7065 7320 3d20 776f 726b  nce_types = work
-000db2c0: 6572 5f69 6e73 7461 6e63 655f 7479 7065  er_instance_type
-000db2d0: 730a 2020 2020 2020 2020 7365 6c66 2e77  s.        self.w
-000db2e0: 6f72 6b65 725f 7065 7269 6f64 203d 2077  orker_period = w
-000db2f0: 6f72 6b65 725f 7065 7269 6f64 0a20 2020  orker_period.   
-000db300: 2020 2020 2073 656c 662e 776f 726b 6572       self.worker
-000db310: 5f70 6572 696f 645f 756e 6974 203d 2077  _period_unit = w
-000db320: 6f72 6b65 725f 7065 7269 6f64 5f75 6e69  orker_period_uni
-000db330: 740a 2020 2020 2020 2020 7365 6c66 2e77  t.        self.w
-000db340: 6f72 6b65 725f 7379 7374 656d 5f64 6973  orker_system_dis
-000db350: 6b5f 6361 7465 676f 7279 203d 2077 6f72  k_category = wor
-000db360: 6b65 725f 7379 7374 656d 5f64 6973 6b5f  ker_system_disk_
-000db370: 6361 7465 676f 7279 0a20 2020 2020 2020  category.       
-000db380: 2073 656c 662e 776f 726b 6572 5f73 7973   self.worker_sys
-000db390: 7465 6d5f 6469 736b 5f73 697a 6520 3d20  tem_disk_size = 
-000db3a0: 776f 726b 6572 5f73 7973 7465 6d5f 6469  worker_system_di
-000db3b0: 736b 5f73 697a 650a 0a20 2020 2064 6566  sk_size..    def
-000db3c0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000db3d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000db3e0: 2e74 6167 733a 0a20 2020 2020 2020 2020  .tags:.         
-000db3f0: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
-000db400: 2e74 6167 733a 0a20 2020 2020 2020 2020  .tags:.         
-000db410: 2020 2020 2020 2069 6620 6b3a 0a20 2020         if k:.   
-000db420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000db430: 206b 2e76 616c 6964 6174 6528 290a 2020   k.validate().  
-000db440: 2020 2020 2020 6966 2073 656c 662e 7461        if self.ta
-000db450: 696e 7473 3a0a 2020 2020 2020 2020 2020  ints:.          
-000db460: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-000db470: 7461 696e 7473 3a0a 2020 2020 2020 2020  taints:.        
-000db480: 2020 2020 2020 2020 6966 206b 3a0a 2020          if k:.  
-000db490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000db4a0: 2020 6b2e 7661 6c69 6461 7465 2829 0a20    k.validate(). 
-000db4b0: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-000db4c0: 6f72 6b65 725f 6461 7461 5f64 6973 6b73  orker_data_disks
-000db4d0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-000db4e0: 7220 6b20 696e 2073 656c 662e 776f 726b  r k in self.work
-000db4f0: 6572 5f64 6174 615f 6469 736b 733a 0a20  er_data_disks:. 
-000db500: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000db510: 6620 6b3a 0a20 2020 2020 2020 2020 2020  f k:.           
-000db520: 2020 2020 2020 2020 206b 2e76 616c 6964           k.valid
-000db530: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-000db540: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-000db550: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-000db560: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-000db570: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000db580: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000db590: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000db5a0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000db5b0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000db5c0: 2020 2069 6620 7365 6c66 2e63 6c6f 7564     if self.cloud
-000db5d0: 5f6d 6f6e 6974 6f72 5f66 6c61 6773 2069  _monitor_flags i
-000db5e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000db5f0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000db600: 636c 6f75 645f 6d6f 6e69 746f 725f 666c  cloud_monitor_fl
-000db610: 6167 7327 5d20 3d20 7365 6c66 2e63 6c6f  ags'] = self.clo
-000db620: 7564 5f6d 6f6e 6974 6f72 5f66 6c61 6773  ud_monitor_flags
-000db630: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000db640: 2e63 6f75 6e74 2069 7320 6e6f 7420 4e6f  .count is not No
-000db650: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000db660: 7265 7375 6c74 5b27 636f 756e 7427 5d20  result['count'] 
-000db670: 3d20 7365 6c66 2e63 6f75 6e74 0a20 2020  = self.count.   
-000db680: 2020 2020 2069 6620 7365 6c66 2e63 7075       if self.cpu
-000db690: 5f70 6f6c 6963 7920 6973 206e 6f74 204e  _policy is not N
-000db6a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000db6b0: 2072 6573 756c 745b 2763 7075 5f70 6f6c   result['cpu_pol
-000db6c0: 6963 7927 5d20 3d20 7365 6c66 2e63 7075  icy'] = self.cpu
-000db6d0: 5f70 6f6c 6963 790a 2020 2020 2020 2020  _policy.        
-000db6e0: 6966 2073 656c 662e 6469 7361 626c 655f  if self.disable_
-000db6f0: 726f 6c6c 6261 636b 2069 7320 6e6f 7420  rollback is not 
-000db700: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000db710: 2020 7265 7375 6c74 5b27 6469 7361 626c    result['disabl
-000db720: 655f 726f 6c6c 6261 636b 275d 203d 2073  e_rollback'] = s
-000db730: 656c 662e 6469 7361 626c 655f 726f 6c6c  elf.disable_roll
-000db740: 6261 636b 0a20 2020 2020 2020 2069 6620  back.        if 
-000db750: 7365 6c66 2e6b 6579 5f70 6169 7220 6973  self.key_pair is
-000db760: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000db770: 2020 2020 2020 2072 6573 756c 745b 276b         result['k
-000db780: 6579 5f70 6169 7227 5d20 3d20 7365 6c66  ey_pair'] = self
-000db790: 2e6b 6579 5f70 6169 720a 2020 2020 2020  .key_pair.      
-000db7a0: 2020 6966 2073 656c 662e 6c6f 6769 6e5f    if self.login_
-000db7b0: 7061 7373 776f 7264 2069 7320 6e6f 7420  password is not 
-000db7c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000db7d0: 2020 7265 7375 6c74 5b27 6c6f 6769 6e5f    result['login_
-000db7e0: 7061 7373 776f 7264 275d 203d 2073 656c  password'] = sel
-000db7f0: 662e 6c6f 6769 6e5f 7061 7373 776f 7264  f.login_password
-000db800: 0a20 2020 2020 2020 2072 6573 756c 745b  .        result[
-000db810: 2774 6167 7327 5d20 3d20 5b5d 0a20 2020  'tags'] = [].   
-000db820: 2020 2020 2069 6620 7365 6c66 2e74 6167       if self.tag
-000db830: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-000db840: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-000db850: 2069 6e20 7365 6c66 2e74 6167 733a 0a20   in self.tags:. 
-000db860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000db870: 6573 756c 745b 2774 6167 7327 5d2e 6170  esult['tags'].ap
-000db880: 7065 6e64 286b 2e74 6f5f 6d61 7028 2920  pend(k.to_map() 
-000db890: 6966 206b 2065 6c73 6520 4e6f 6e65 290a  if k else None).
-000db8a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000db8b0: 7461 696e 7473 275d 203d 205b 5d0a 2020  taints'] = [].  
-000db8c0: 2020 2020 2020 6966 2073 656c 662e 7461        if self.ta
-000db8d0: 696e 7473 2069 7320 6e6f 7420 4e6f 6e65  ints is not None
-000db8e0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-000db8f0: 7220 6b20 696e 2073 656c 662e 7461 696e  r k in self.tain
-000db900: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-000db910: 2020 2020 7265 7375 6c74 5b27 7461 696e      result['tain
-000db920: 7473 275d 2e61 7070 656e 6428 6b2e 746f  ts'].append(k.to
-000db930: 5f6d 6170 2829 2069 6620 6b20 656c 7365  _map() if k else
-000db940: 204e 6f6e 6529 0a20 2020 2020 2020 2069   None).        i
-000db950: 6620 7365 6c66 2e76 7377 6974 6368 5f69  f self.vswitch_i
-000db960: 6473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ds is not None:.
-000db970: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000db980: 6c74 5b27 7673 7769 7463 685f 6964 7327  lt['vswitch_ids'
-000db990: 5d20 3d20 7365 6c66 2e76 7377 6974 6368  ] = self.vswitch
-000db9a0: 5f69 6473 0a20 2020 2020 2020 2069 6620  _ids.        if 
-000db9b0: 7365 6c66 2e77 6f72 6b65 725f 6175 746f  self.worker_auto
-000db9c0: 5f72 656e 6577 2069 7320 6e6f 7420 4e6f  _renew is not No
-000db9d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000db9e0: 7265 7375 6c74 5b27 776f 726b 6572 5f61  result['worker_a
-000db9f0: 7574 6f5f 7265 6e65 7727 5d20 3d20 7365  uto_renew'] = se
-000dba00: 6c66 2e77 6f72 6b65 725f 6175 746f 5f72  lf.worker_auto_r
-000dba10: 656e 6577 0a20 2020 2020 2020 2069 6620  enew.        if 
-000dba20: 7365 6c66 2e77 6f72 6b65 725f 6175 746f  self.worker_auto
-000dba30: 5f72 656e 6577 5f70 6572 696f 6420 6973  _renew_period is
-000dba40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000dba50: 2020 2020 2020 2072 6573 756c 745b 2777         result['w
-000dba60: 6f72 6b65 725f 6175 746f 5f72 656e 6577  orker_auto_renew
-000dba70: 5f70 6572 696f 6427 5d20 3d20 7365 6c66  _period'] = self
-000dba80: 2e77 6f72 6b65 725f 6175 746f 5f72 656e  .worker_auto_ren
-000dba90: 6577 5f70 6572 696f 640a 2020 2020 2020  ew_period.      
-000dbaa0: 2020 6966 2073 656c 662e 776f 726b 6572    if self.worker
-000dbab0: 5f64 6174 615f 6469 736b 2069 7320 6e6f  _data_disk is no
-000dbac0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000dbad0: 2020 2020 7265 7375 6c74 5b27 776f 726b      result['work
-000dbae0: 6572 5f64 6174 615f 6469 736b 275d 203d  er_data_disk'] =
-000dbaf0: 2073 656c 662e 776f 726b 6572 5f64 6174   self.worker_dat
-000dbb00: 615f 6469 736b 0a20 2020 2020 2020 2072  a_disk.        r
-000dbb10: 6573 756c 745b 2777 6f72 6b65 725f 6461  esult['worker_da
-000dbb20: 7461 5f64 6973 6b73 275d 203d 205b 5d0a  ta_disks'] = [].
-000dbb30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000dbb40: 776f 726b 6572 5f64 6174 615f 6469 736b  worker_data_disk
-000dbb50: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-000dbb60: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-000dbb70: 2069 6e20 7365 6c66 2e77 6f72 6b65 725f   in self.worker_
-000dbb80: 6461 7461 5f64 6973 6b73 3a0a 2020 2020  data_disks:.    
-000dbb90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000dbba0: 6c74 5b27 776f 726b 6572 5f64 6174 615f  lt['worker_data_
-000dbbb0: 6469 736b 7327 5d2e 6170 7065 6e64 286b  disks'].append(k
-000dbbc0: 2e74 6f5f 6d61 7028 2920 6966 206b 2065  .to_map() if k e
-000dbbd0: 6c73 6520 4e6f 6e65 290a 2020 2020 2020  lse None).      
-000dbbe0: 2020 6966 2073 656c 662e 776f 726b 6572    if self.worker
-000dbbf0: 5f69 6e73 7461 6e63 655f 6368 6172 6765  _instance_charge
-000dbc00: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
-000dbc10: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000dbc20: 6573 756c 745b 2777 6f72 6b65 725f 696e  esult['worker_in
-000dbc30: 7374 616e 6365 5f63 6861 7267 655f 7479  stance_charge_ty
-000dbc40: 7065 275d 203d 2073 656c 662e 776f 726b  pe'] = self.work
-000dbc50: 6572 5f69 6e73 7461 6e63 655f 6368 6172  er_instance_char
-000dbc60: 6765 5f74 7970 650a 2020 2020 2020 2020  ge_type.        
-000dbc70: 6966 2073 656c 662e 776f 726b 6572 5f69  if self.worker_i
-000dbc80: 6e73 7461 6e63 655f 7479 7065 7320 6973  nstance_types is
-000dbc90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000dbca0: 2020 2020 2020 2072 6573 756c 745b 2777         result['w
-000dbcb0: 6f72 6b65 725f 696e 7374 616e 6365 5f74  orker_instance_t
-000dbcc0: 7970 6573 275d 203d 2073 656c 662e 776f  ypes'] = self.wo
-000dbcd0: 726b 6572 5f69 6e73 7461 6e63 655f 7479  rker_instance_ty
-000dbce0: 7065 730a 2020 2020 2020 2020 6966 2073  pes.        if s
-000dbcf0: 656c 662e 776f 726b 6572 5f70 6572 696f  elf.worker_perio
-000dbd00: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000dbd10: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000dbd20: 745b 2777 6f72 6b65 725f 7065 7269 6f64  t['worker_period
-000dbd30: 275d 203d 2073 656c 662e 776f 726b 6572  '] = self.worker
-000dbd40: 5f70 6572 696f 640a 2020 2020 2020 2020  _period.        
-000dbd50: 6966 2073 656c 662e 776f 726b 6572 5f70  if self.worker_p
-000dbd60: 6572 696f 645f 756e 6974 2069 7320 6e6f  eriod_unit is no
-000dbd70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000dbd80: 2020 2020 7265 7375 6c74 5b27 776f 726b      result['work
-000dbd90: 6572 5f70 6572 696f 645f 756e 6974 275d  er_period_unit']
-000dbda0: 203d 2073 656c 662e 776f 726b 6572 5f70   = self.worker_p
-000dbdb0: 6572 696f 645f 756e 6974 0a20 2020 2020  eriod_unit.     
-000dbdc0: 2020 2069 6620 7365 6c66 2e77 6f72 6b65     if self.worke
-000dbdd0: 725f 7379 7374 656d 5f64 6973 6b5f 6361  r_system_disk_ca
-000dbde0: 7465 676f 7279 2069 7320 6e6f 7420 4e6f  tegory is not No
-000dbdf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000dbe00: 7265 7375 6c74 5b27 776f 726b 6572 5f73  result['worker_s
-000dbe10: 7973 7465 6d5f 6469 736b 5f63 6174 6567  ystem_disk_categ
-000dbe20: 6f72 7927 5d20 3d20 7365 6c66 2e77 6f72  ory'] = self.wor
-000dbe30: 6b65 725f 7379 7374 656d 5f64 6973 6b5f  ker_system_disk_
-000dbe40: 6361 7465 676f 7279 0a20 2020 2020 2020  category.       
-000dbe50: 2069 6620 7365 6c66 2e77 6f72 6b65 725f   if self.worker_
-000dbe60: 7379 7374 656d 5f64 6973 6b5f 7369 7a65  system_disk_size
-000dbe70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000dbe80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000dbe90: 5b27 776f 726b 6572 5f73 7973 7465 6d5f  ['worker_system_
-000dbea0: 6469 736b 5f73 697a 6527 5d20 3d20 7365  disk_size'] = se
-000dbeb0: 6c66 2e77 6f72 6b65 725f 7379 7374 656d  lf.worker_system
-000dbec0: 5f64 6973 6b5f 7369 7a65 0a20 2020 2020  _disk_size.     
-000dbed0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000dbee0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000dbef0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000dbf00: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000dbf10: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000dbf20: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000dbf30: 6574 2827 636c 6f75 645f 6d6f 6e69 746f  et('cloud_monito
-000dbf40: 725f 666c 6167 7327 2920 6973 206e 6f74  r_flags') is not
-000dbf50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000dbf60: 2020 2073 656c 662e 636c 6f75 645f 6d6f     self.cloud_mo
-000dbf70: 6e69 746f 725f 666c 6167 7320 3d20 6d2e  nitor_flags = m.
-000dbf80: 6765 7428 2763 6c6f 7564 5f6d 6f6e 6974  get('cloud_monit
-000dbf90: 6f72 5f66 6c61 6773 2729 0a20 2020 2020  or_flags').     
-000dbfa0: 2020 2069 6620 6d2e 6765 7428 2763 6f75     if m.get('cou
-000dbfb0: 6e74 2729 2069 7320 6e6f 7420 4e6f 6e65  nt') is not None
-000dbfc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000dbfd0: 6c66 2e63 6f75 6e74 203d 206d 2e67 6574  lf.count = m.get
-000dbfe0: 2827 636f 756e 7427 290a 2020 2020 2020  ('count').      
-000dbff0: 2020 6966 206d 2e67 6574 2827 6370 755f    if m.get('cpu_
-000dc000: 706f 6c69 6379 2729 2069 7320 6e6f 7420  policy') is not 
-000dc010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000dc020: 2020 7365 6c66 2e63 7075 5f70 6f6c 6963    self.cpu_polic
-000dc030: 7920 3d20 6d2e 6765 7428 2763 7075 5f70  y = m.get('cpu_p
-000dc040: 6f6c 6963 7927 290a 2020 2020 2020 2020  olicy').        
-000dc050: 6966 206d 2e67 6574 2827 6469 7361 626c  if m.get('disabl
-000dc060: 655f 726f 6c6c 6261 636b 2729 2069 7320  e_rollback') is 
-000dc070: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000dc080: 2020 2020 2020 7365 6c66 2e64 6973 6162        self.disab
-000dc090: 6c65 5f72 6f6c 6c62 6163 6b20 3d20 6d2e  le_rollback = m.
-000dc0a0: 6765 7428 2764 6973 6162 6c65 5f72 6f6c  get('disable_rol
-000dc0b0: 6c62 6163 6b27 290a 2020 2020 2020 2020  lback').        
-000dc0c0: 6966 206d 2e67 6574 2827 6b65 795f 7061  if m.get('key_pa
-000dc0d0: 6972 2729 2069 7320 6e6f 7420 4e6f 6e65  ir') is not None
-000dc0e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000dc0f0: 6c66 2e6b 6579 5f70 6169 7220 3d20 6d2e  lf.key_pair = m.
-000dc100: 6765 7428 276b 6579 5f70 6169 7227 290a  get('key_pair').
-000dc110: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000dc120: 2827 6c6f 6769 6e5f 7061 7373 776f 7264  ('login_password
-000dc130: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000dc140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000dc150: 2e6c 6f67 696e 5f70 6173 7377 6f72 6420  .login_password 
-000dc160: 3d20 6d2e 6765 7428 276c 6f67 696e 5f70  = m.get('login_p
-000dc170: 6173 7377 6f72 6427 290a 2020 2020 2020  assword').      
-000dc180: 2020 7365 6c66 2e74 6167 7320 3d20 5b5d    self.tags = []
-000dc190: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000dc1a0: 7428 2774 6167 7327 2920 6973 206e 6f74  t('tags') is not
-000dc1b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000dc1c0: 2020 2066 6f72 206b 2069 6e20 6d2e 6765     for k in m.ge
-000dc1d0: 7428 2774 6167 7327 293a 0a20 2020 2020  t('tags'):.     
-000dc1e0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-000dc1f0: 6d6f 6465 6c20 3d20 5363 616c 6543 6c75  model = ScaleClu
-000dc200: 7374 6572 5265 7175 6573 7454 6167 7328  sterRequestTags(
-000dc210: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000dc220: 2020 7365 6c66 2e74 6167 732e 6170 7065    self.tags.appe
-000dc230: 6e64 2874 656d 705f 6d6f 6465 6c2e 6672  nd(temp_model.fr
-000dc240: 6f6d 5f6d 6170 286b 2929 0a20 2020 2020  om_map(k)).     
-000dc250: 2020 2073 656c 662e 7461 696e 7473 203d     self.taints =
-000dc260: 205b 5d0a 2020 2020 2020 2020 6966 206d   [].        if m
-000dc270: 2e67 6574 2827 7461 696e 7473 2729 2069  .get('taints') i
-000dc280: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000dc290: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-000dc2a0: 206d 2e67 6574 2827 7461 696e 7473 2729   m.get('taints')
-000dc2b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000dc2c0: 2020 7465 6d70 5f6d 6f64 656c 203d 2053    temp_model = S
-000dc2d0: 6361 6c65 436c 7573 7465 7252 6571 7565  caleClusterReque
-000dc2e0: 7374 5461 696e 7473 2829 0a20 2020 2020  stTaints().     
-000dc2f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000dc300: 7461 696e 7473 2e61 7070 656e 6428 7465  taints.append(te
-000dc310: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-000dc320: 7028 6b29 290a 2020 2020 2020 2020 6966  p(k)).        if
-000dc330: 206d 2e67 6574 2827 7673 7769 7463 685f   m.get('vswitch_
-000dc340: 6964 7327 2920 6973 206e 6f74 204e 6f6e  ids') is not Non
-000dc350: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000dc360: 656c 662e 7673 7769 7463 685f 6964 7320  elf.vswitch_ids 
-000dc370: 3d20 6d2e 6765 7428 2776 7377 6974 6368  = m.get('vswitch
-000dc380: 5f69 6473 2729 0a20 2020 2020 2020 2069  _ids').        i
-000dc390: 6620 6d2e 6765 7428 2777 6f72 6b65 725f  f m.get('worker_
-000dc3a0: 6175 746f 5f72 656e 6577 2729 2069 7320  auto_renew') is 
-000dc3b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000dc3c0: 2020 2020 2020 7365 6c66 2e77 6f72 6b65        self.worke
-000dc3d0: 725f 6175 746f 5f72 656e 6577 203d 206d  r_auto_renew = m
-000dc3e0: 2e67 6574 2827 776f 726b 6572 5f61 7574  .get('worker_aut
-000dc3f0: 6f5f 7265 6e65 7727 290a 2020 2020 2020  o_renew').      
-000dc400: 2020 6966 206d 2e67 6574 2827 776f 726b    if m.get('work
-000dc410: 6572 5f61 7574 6f5f 7265 6e65 775f 7065  er_auto_renew_pe
-000dc420: 7269 6f64 2729 2069 7320 6e6f 7420 4e6f  riod') is not No
-000dc430: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000dc440: 7365 6c66 2e77 6f72 6b65 725f 6175 746f  self.worker_auto
-000dc450: 5f72 656e 6577 5f70 6572 696f 6420 3d20  _renew_period = 
-000dc460: 6d2e 6765 7428 2777 6f72 6b65 725f 6175  m.get('worker_au
-000dc470: 746f 5f72 656e 6577 5f70 6572 696f 6427  to_renew_period'
-000dc480: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000dc490: 6574 2827 776f 726b 6572 5f64 6174 615f  et('worker_data_
-000dc4a0: 6469 736b 2729 2069 7320 6e6f 7420 4e6f  disk') is not No
-000dc4b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000dc4c0: 7365 6c66 2e77 6f72 6b65 725f 6461 7461  self.worker_data
-000dc4d0: 5f64 6973 6b20 3d20 6d2e 6765 7428 2777  _disk = m.get('w
-000dc4e0: 6f72 6b65 725f 6461 7461 5f64 6973 6b27  orker_data_disk'
-000dc4f0: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
-000dc500: 6f72 6b65 725f 6461 7461 5f64 6973 6b73  orker_data_disks
-000dc510: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-000dc520: 206d 2e67 6574 2827 776f 726b 6572 5f64   m.get('worker_d
-000dc530: 6174 615f 6469 736b 7327 2920 6973 206e  ata_disks') is n
-000dc540: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000dc550: 2020 2020 2066 6f72 206b 2069 6e20 6d2e       for k in m.
-000dc560: 6765 7428 2777 6f72 6b65 725f 6461 7461  get('worker_data
-000dc570: 5f64 6973 6b73 2729 3a0a 2020 2020 2020  _disks'):.      
-000dc580: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-000dc590: 6f64 656c 203d 2053 6361 6c65 436c 7573  odel = ScaleClus
-000dc5a0: 7465 7252 6571 7565 7374 576f 726b 6572  terRequestWorker
-000dc5b0: 4461 7461 4469 736b 7328 290a 2020 2020  DataDisks().    
-000dc5c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000dc5d0: 2e77 6f72 6b65 725f 6461 7461 5f64 6973  .worker_data_dis
-000dc5e0: 6b73 2e61 7070 656e 6428 7465 6d70 5f6d  ks.append(temp_m
-000dc5f0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6b29  odel.from_map(k)
-000dc600: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000dc610: 6574 2827 776f 726b 6572 5f69 6e73 7461  et('worker_insta
-000dc620: 6e63 655f 6368 6172 6765 5f74 7970 6527  nce_charge_type'
-000dc630: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000dc640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000dc650: 776f 726b 6572 5f69 6e73 7461 6e63 655f  worker_instance_
-000dc660: 6368 6172 6765 5f74 7970 6520 3d20 6d2e  charge_type = m.
-000dc670: 6765 7428 2777 6f72 6b65 725f 696e 7374  get('worker_inst
-000dc680: 616e 6365 5f63 6861 7267 655f 7479 7065  ance_charge_type
-000dc690: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000dc6a0: 6765 7428 2777 6f72 6b65 725f 696e 7374  get('worker_inst
-000dc6b0: 616e 6365 5f74 7970 6573 2729 2069 7320  ance_types') is 
-000dc6c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000dc6d0: 2020 2020 2020 7365 6c66 2e77 6f72 6b65        self.worke
-000dc6e0: 725f 696e 7374 616e 6365 5f74 7970 6573  r_instance_types
-000dc6f0: 203d 206d 2e67 6574 2827 776f 726b 6572   = m.get('worker
-000dc700: 5f69 6e73 7461 6e63 655f 7479 7065 7327  _instance_types'
-000dc710: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000dc720: 6574 2827 776f 726b 6572 5f70 6572 696f  et('worker_perio
-000dc730: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-000dc740: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000dc750: 662e 776f 726b 6572 5f70 6572 696f 6420  f.worker_period 
-000dc760: 3d20 6d2e 6765 7428 2777 6f72 6b65 725f  = m.get('worker_
-000dc770: 7065 7269 6f64 2729 0a20 2020 2020 2020  period').       
-000dc780: 2069 6620 6d2e 6765 7428 2777 6f72 6b65   if m.get('worke
-000dc790: 725f 7065 7269 6f64 5f75 6e69 7427 2920  r_period_unit') 
-000dc7a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000dc7b0: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
-000dc7c0: 726b 6572 5f70 6572 696f 645f 756e 6974  rker_period_unit
-000dc7d0: 203d 206d 2e67 6574 2827 776f 726b 6572   = m.get('worker
-000dc7e0: 5f70 6572 696f 645f 756e 6974 2729 0a20  _period_unit'). 
-000dc7f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000dc800: 2777 6f72 6b65 725f 7379 7374 656d 5f64  'worker_system_d
-000dc810: 6973 6b5f 6361 7465 676f 7279 2729 2069  isk_category') i
-000dc820: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000dc830: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-000dc840: 6b65 725f 7379 7374 656d 5f64 6973 6b5f  ker_system_disk_
-000dc850: 6361 7465 676f 7279 203d 206d 2e67 6574  category = m.get
-000dc860: 2827 776f 726b 6572 5f73 7973 7465 6d5f  ('worker_system_
-000dc870: 6469 736b 5f63 6174 6567 6f72 7927 290a  disk_category').
-000dc880: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000dc890: 2827 776f 726b 6572 5f73 7973 7465 6d5f  ('worker_system_
-000dc8a0: 6469 736b 5f73 697a 6527 2920 6973 206e  disk_size') is n
-000dc8b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000dc8c0: 2020 2020 2073 656c 662e 776f 726b 6572       self.worker
-000dc8d0: 5f73 7973 7465 6d5f 6469 736b 5f73 697a  _system_disk_siz
-000dc8e0: 6520 3d20 6d2e 6765 7428 2777 6f72 6b65  e = m.get('worke
-000dc8f0: 725f 7379 7374 656d 5f64 6973 6b5f 7369  r_system_disk_si
-000dc900: 7a65 2729 0a20 2020 2020 2020 2072 6574  ze').        ret
-000dc910: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-000dc920: 2053 6361 6c65 436c 7573 7465 7252 6573   ScaleClusterRes
-000dc930: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
-000dc940: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000dc950: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000dc960: 656c 662c 0a20 2020 2020 2020 2063 6c75  elf,.        clu
-000dc970: 7374 6572 5f69 643a 2073 7472 203d 204e  ster_id: str = N
-000dc980: 6f6e 652c 0a20 2020 2020 2020 2072 6571  one,.        req
-000dc990: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
-000dc9a0: 6f6e 652c 0a20 2020 2020 2020 2074 6173  one,.        tas
-000dc9b0: 6b5f 6964 3a20 7374 7220 3d20 4e6f 6e65  k_id: str = None
-000dc9c0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-000dc9d0: 2073 656c 662e 636c 7573 7465 725f 6964   self.cluster_id
-000dc9e0: 203d 2063 6c75 7374 6572 5f69 640a 2020   = cluster_id.  
-000dc9f0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-000dca00: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
-000dca10: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-000dca20: 7461 736b 5f69 6420 3d20 7461 736b 5f69  task_id = task_i
-000dca30: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
-000dca40: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000dca50: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-000dca60: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-000dca70: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-000dca80: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-000dca90: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-000dcaa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000dcab0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000dcac0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-000dcad0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-000dcae0: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
-000dcaf0: 7374 6572 5f69 6420 6973 206e 6f74 204e  ster_id is not N
-000dcb00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000dcb10: 2072 6573 756c 745b 2763 6c75 7374 6572   result['cluster
-000dcb20: 5f69 6427 5d20 3d20 7365 6c66 2e63 6c75  _id'] = self.clu
-000dcb30: 7374 6572 5f69 640a 2020 2020 2020 2020  ster_id.        
-000dcb40: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
-000dcb50: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-000dcb60: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000dcb70: 6c74 5b27 7265 7175 6573 745f 6964 275d  lt['request_id']
-000dcb80: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-000dcb90: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-000dcba0: 6c66 2e74 6173 6b5f 6964 2069 7320 6e6f  lf.task_id is no
-000dcbb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000dcbc0: 2020 2020 7265 7375 6c74 5b27 7461 736b      result['task
-000dcbd0: 5f69 6427 5d20 3d20 7365 6c66 2e74 6173  _id'] = self.tas
-000dcbe0: 6b5f 6964 0a20 2020 2020 2020 2072 6574  k_id.        ret
-000dcbf0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000dcc00: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000dcc10: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000dcc20: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000dcc30: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000dcc40: 2020 2020 6966 206d 2e67 6574 2827 636c      if m.get('cl
-000dcc50: 7573 7465 725f 6964 2729 2069 7320 6e6f  uster_id') is no
-000dcc60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000dcc70: 2020 2020 7365 6c66 2e63 6c75 7374 6572      self.cluster
-000dcc80: 5f69 6420 3d20 6d2e 6765 7428 2763 6c75  _id = m.get('clu
-000dcc90: 7374 6572 5f69 6427 290a 2020 2020 2020  ster_id').      
-000dcca0: 2020 6966 206d 2e67 6574 2827 7265 7175    if m.get('requ
-000dccb0: 6573 745f 6964 2729 2069 7320 6e6f 7420  est_id') is not 
-000dccc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000dccd0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-000dcce0: 6420 3d20 6d2e 6765 7428 2772 6571 7565  d = m.get('reque
-000dccf0: 7374 5f69 6427 290a 2020 2020 2020 2020  st_id').        
-000dcd00: 6966 206d 2e67 6574 2827 7461 736b 5f69  if m.get('task_i
-000dcd10: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-000dcd20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000dcd30: 662e 7461 736b 5f69 6420 3d20 6d2e 6765  f.task_id = m.ge
-000dcd40: 7428 2774 6173 6b5f 6964 2729 0a20 2020  t('task_id').   
-000dcd50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000dcd60: 0a0a 0a63 6c61 7373 2053 6361 6c65 436c  ...class ScaleCl
-000dcd70: 7573 7465 7252 6573 706f 6e73 6528 5465  usterResponse(Te
-000dcd80: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-000dcd90: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-000dcda0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000dcdb0: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
-000dcdc0: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
-000dcdd0: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
-000dcde0: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
-000dcdf0: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-000dce00: 5363 616c 6543 6c75 7374 6572 5265 7370  ScaleClusterResp
-000dce10: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
-000dce20: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000dce30: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
-000dce40: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
-000dce50: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-000dce60: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
-000dce70: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-000dce80: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
-000dce90: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000dcea0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000dceb0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-000dcec0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-000dced0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-000dcee0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-000dcef0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000dcf00: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-000dcf10: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-000dcf20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000dcf30: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000dcf40: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000dcf50: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000dcf60: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-000dcf70: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-000dcf80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000dcf90: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-000dcfa0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-000dcfb0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-000dcfc0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-000dcfd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000dcfe0: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-000dcff0: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-000dd000: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-000dd010: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-000dd020: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000dd030: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000dd040: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-000dd050: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-000dd060: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000dd070: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-000dd080: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-000dd090: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-000dd0a0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-000dd0b0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-000dd0c0: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-000dd0d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000dd0e0: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-000dd0f0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-000dd100: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-000dd110: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-000dd120: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-000dd130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000dd140: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000dd150: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-000dd160: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-000dd170: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-000dd180: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000dd190: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-000dd1a0: 6f64 656c 203d 2053 6361 6c65 436c 7573  odel = ScaleClus
-000dd1b0: 7465 7252 6573 706f 6e73 6542 6f64 7928  terResponseBody(
-000dd1c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000dd1d0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-000dd1e0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-000dd1f0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-000dd200: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000dd210: 6c61 7373 2053 6361 6c65 436c 7573 7465  lass ScaleCluste
-000dd220: 724e 6f64 6550 6f6f 6c52 6571 7565 7374  rNodePoolRequest
-000dd230: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-000dd240: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-000dd250: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000dd260: 2020 2020 636f 756e 743a 2069 6e74 203d      count: int =
-000dd270: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-000dd280: 2020 2020 2020 2320 5468 6520 6e75 6d62        # The numb
-000dd290: 6572 206f 6620 776f 726b 6572 206e 6f64  er of worker nod
-000dd2a0: 6573 2074 6861 7420 796f 7520 7761 6e74  es that you want
-000dd2b0: 2074 6f20 6164 642e 2059 6f75 2063 616e   to add. You can
-000dd2c0: 2061 6464 2061 7420 6d6f 7374 2035 3030   add at most 500
-000dd2d0: 206e 6f64 6573 2069 6e20 6f6e 6520 4150   nodes in one AP
-000dd2e0: 4920 6361 6c6c 2e20 5468 6520 6d61 7869  I call. The maxi
-000dd2f0: 6d75 6d20 6e75 6d62 6572 206f 6620 6e6f  mum number of no
-000dd300: 6465 7320 7468 6174 2063 616e 2062 6520  des that can be 
-000dd310: 6164 6465 6420 6973 206c 696d 6974 6564  added is limited
-000dd320: 2062 7920 7468 6520 7175 6f74 6120 6f66   by the quota of
-000dd330: 206e 6f64 6573 2069 6e20 7468 6520 636c   nodes in the cl
-000dd340: 7573 7465 722e 0a20 2020 2020 2020 2073  uster..        s
-000dd350: 656c 662e 636f 756e 7420 3d20 636f 756e  elf.count = coun
-000dd360: 740a 0a20 2020 2064 6566 2076 616c 6964  t..    def valid
-000dd370: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000dd380: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-000dd390: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-000dd3a0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-000dd3b0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-000dd3c0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-000dd3d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000dd3e0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000dd3f0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-000dd400: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-000dd410: 2020 2020 2069 6620 7365 6c66 2e63 6f75       if self.cou
-000dd420: 6e74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nt is not None:.
-000dd430: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000dd440: 6c74 5b27 636f 756e 7427 5d20 3d20 7365  lt['count'] = se
-000dd450: 6c66 2e63 6f75 6e74 0a20 2020 2020 2020  lf.count.       
-000dd460: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000dd470: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000dd480: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-000dd490: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-000dd4a0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-000dd4b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000dd4c0: 2827 636f 756e 7427 2920 6973 206e 6f74  ('count') is not
-000dd4d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000dd4e0: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-000dd4f0: 6d2e 6765 7428 2763 6f75 6e74 2729 0a20  m.get('count'). 
-000dd500: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000dd510: 6c66 0a0a 0a63 6c61 7373 2053 6361 6c65  lf...class Scale
-000dd520: 436c 7573 7465 724e 6f64 6550 6f6f 6c52  ClusterNodePoolR
-000dd530: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-000dd540: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000dd550: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000dd560: 2073 656c 662c 0a20 2020 2020 2020 2074   self,.        t
-000dd570: 6173 6b5f 6964 3a20 7374 7220 3d20 4e6f  ask_id: str = No
-000dd580: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-000dd590: 2020 2023 2054 6865 2074 6173 6b20 4944     # The task ID
-000dd5a0: 2e0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-000dd5b0: 6173 6b5f 6964 203d 2074 6173 6b5f 6964  ask_id = task_id
-000dd5c0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000dd5d0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000dd5e0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-000dd5f0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-000dd600: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000dd610: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-000dd620: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-000dd630: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000dd640: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000dd650: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000dd660: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000dd670: 2020 2020 6966 2073 656c 662e 7461 736b      if self.task
-000dd680: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-000dd690: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000dd6a0: 756c 745b 2774 6173 6b5f 6964 275d 203d  ult['task_id'] =
-000dd6b0: 2073 656c 662e 7461 736b 5f69 640a 2020   self.task_id.  
-000dd6c0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000dd6d0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-000dd6e0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-000dd6f0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-000dd700: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-000dd710: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000dd720: 6d2e 6765 7428 2774 6173 6b5f 6964 2729  m.get('task_id')
-000dd730: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000dd740: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000dd750: 6173 6b5f 6964 203d 206d 2e67 6574 2827  ask_id = m.get('
-000dd760: 7461 736b 5f69 6427 290a 2020 2020 2020  task_id').      
-000dd770: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000dd780: 636c 6173 7320 5363 616c 6543 6c75 7374  class ScaleClust
-000dd790: 6572 4e6f 6465 506f 6f6c 5265 7370 6f6e  erNodePoolRespon
-000dd7a0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-000dd7b0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000dd7c0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000dd7d0: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-000dd7e0: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-000dd7f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-000dd800: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
-000dd810: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
-000dd820: 6f64 793a 2053 6361 6c65 436c 7573 7465  ody: ScaleCluste
-000dd830: 724e 6f64 6550 6f6f 6c52 6573 706f 6e73  rNodePoolRespons
-000dd840: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
-000dd850: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-000dd860: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-000dd870: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-000dd880: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-000dd890: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-000dd8a0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-000dd8b0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-000dd8c0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000dd8d0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-000dd8e0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-000dd8f0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-000dd900: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-000dd910: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-000dd920: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-000dd930: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-000dd940: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000dd950: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000dd960: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000dd970: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000dd980: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000dd990: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-000dd9a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000dd9b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000dd9c0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-000dd9d0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-000dd9e0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-000dd9f0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-000dda00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000dda10: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-000dda20: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-000dda30: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-000dda40: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-000dda50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000dda60: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-000dda70: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-000dda80: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-000dda90: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-000ddaa0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-000ddab0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-000ddac0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-000ddad0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-000ddae0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000ddaf0: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
-000ddb00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ddb10: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-000ddb20: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
-000ddb30: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
-000ddb40: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-000ddb50: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
-000ddb60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000ddb70: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-000ddb80: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-000ddb90: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
-000ddba0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-000ddbb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000ddbc0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-000ddbd0: 6c20 3d20 5363 616c 6543 6c75 7374 6572  l = ScaleCluster
-000ddbe0: 4e6f 6465 506f 6f6c 5265 7370 6f6e 7365  NodePoolResponse
-000ddbf0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-000ddc00: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-000ddc10: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-000ddc20: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-000ddc30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000ddc40: 660a 0a0a 636c 6173 7320 5363 616c 654f  f...class ScaleO
-000ddc50: 7574 436c 7573 7465 7252 6571 7565 7374  utClusterRequest
-000ddc60: 576f 726b 6572 4461 7461 4469 736b 7328  WorkerDataDisks(
-000ddc70: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-000ddc80: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000ddc90: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000ddca0: 2020 2061 7574 6f5f 736e 6170 7368 6f74     auto_snapshot
-000ddcb0: 5f70 6f6c 6963 795f 6964 3a20 7374 7220  _policy_id: str 
-000ddcc0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000ddcd0: 6361 7465 676f 7279 3a20 7374 7220 3d20  category: str = 
-000ddce0: 4e6f 6e65 2c0a 2020 2020 2020 2020 656e  None,.        en
-000ddcf0: 6372 7970 7465 643a 2073 7472 203d 204e  crypted: str = N
-000ddd00: 6f6e 652c 0a20 2020 2020 2020 2073 697a  one,.        siz
-000ddd10: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-000ddd20: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000ddd30: 5468 6520 4944 206f 6620 616e 2061 7574  The ID of an aut
-000ddd40: 6f6d 6174 6963 2073 6e61 7073 686f 7420  omatic snapshot 
-000ddd50: 706f 6c69 6379 2e20 4175 746f 6d61 7469  policy. Automati
-000ddd60: 6320 6261 636b 7570 2069 7320 7065 7266  c backup is perf
-000ddd70: 6f72 6d65 6420 666f 7220 6120 6469 736b  ormed for a disk
-000ddd80: 2062 6173 6564 206f 6e20 7468 6520 7370   based on the sp
-000ddd90: 6563 6966 6965 6420 6175 746f 6d61 7469  ecified automati
-000ddda0: 6320 736e 6170 7368 6f74 2070 6f6c 6963  c snapshot polic
-000dddb0: 792e 0a20 2020 2020 2020 2023 200a 2020  y..        # .  
-000dddc0: 2020 2020 2020 2320 4279 2064 6566 6175        # By defau
-000dddd0: 6c74 2c20 7468 6973 2070 6172 616d 6574  lt, this paramet
-000ddde0: 6572 2069 7320 656d 7074 792c 2077 6869  er is empty, whi
-000dddf0: 6368 2069 6e64 6963 6174 6573 2074 6861  ch indicates tha
-000dde00: 7420 6175 746f 6d61 7469 6320 6261 636b  t automatic back
-000dde10: 7570 2069 7320 6469 7361 626c 6564 2e0a  up is disabled..
-000dde20: 2020 2020 2020 2020 7365 6c66 2e61 7574          self.aut
-000dde30: 6f5f 736e 6170 7368 6f74 5f70 6f6c 6963  o_snapshot_polic
-000dde40: 795f 6964 203d 2061 7574 6f5f 736e 6170  y_id = auto_snap
-000dde50: 7368 6f74 5f70 6f6c 6963 795f 6964 0a20  shot_policy_id. 
-000dde60: 2020 2020 2020 2023 2054 6865 2064 6174         # The dat
-000dde70: 6120 6469 736b 2074 7970 652e 0a20 2020  a disk type..   
-000dde80: 2020 2020 2073 656c 662e 6361 7465 676f       self.catego
-000dde90: 7279 203d 2063 6174 6567 6f72 790a 2020  ry = category.  
-000ddea0: 2020 2020 2020 2320 5370 6563 6966 6965        # Specifie
-000ddeb0: 7320 7768 6574 6865 7220 746f 2065 6e63  s whether to enc
-000ddec0: 7279 7074 2074 6865 2064 6174 6120 6469  rypt the data di
-000dded0: 736b 732e 2056 616c 6964 2076 616c 7565  sks. Valid value
-000ddee0: 733a 0a20 2020 2020 2020 2023 200a 2020  s:.        # .  
-000ddef0: 2020 2020 2020 2320 2a20 2020 6074 7275        # *   `tru
-000ddf00: 6560 3a20 656e 6372 7970 7473 2064 6174  e`: encrypts dat
-000ddf10: 6120 6469 736b 732e 0a20 2020 2020 2020  a disks..       
-000ddf20: 2023 202a 2020 2060 6661 6c73 6560 3a20   # *   `false`: 
-000ddf30: 646f 6573 206e 6f74 2065 6e63 7279 7074  does not encrypt
-000ddf40: 2064 6174 6120 6469 736b 732e 0a20 2020   data disks..   
-000ddf50: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
-000ddf60: 2320 4465 6661 756c 7420 7661 6c75 653a  # Default value:
-000ddf70: 2060 6661 6c73 6560 2e0a 2020 2020 2020   `false`..      
-000ddf80: 2020 7365 6c66 2e65 6e63 7279 7074 6564    self.encrypted
-000ddf90: 203d 2065 6e63 7279 7074 6564 0a20 2020   = encrypted.   
-000ddfa0: 2020 2020 2023 2054 6865 2073 697a 6520       # The size 
-000ddfb0: 6f66 2074 6865 2064 6174 6120 6469 736b  of the data disk
-000ddfc0: 2e20 5661 6c69 6420 7661 6c75 6573 3a20  . Valid values: 
-000ddfd0: 3430 2074 6f20 3332 3736 372e 0a20 2020  40 to 32767..   
-000ddfe0: 2020 2020 2073 656c 662e 7369 7a65 203d       self.size =
-000ddff0: 2073 697a 650a 0a20 2020 2064 6566 2076   size..    def v
-000de000: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000de010: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-000de020: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-000de030: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-000de040: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-000de050: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-000de060: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-000de070: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000de080: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-000de090: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-000de0a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000de0b0: 2e61 7574 6f5f 736e 6170 7368 6f74 5f70  .auto_snapshot_p
-000de0c0: 6f6c 6963 795f 6964 2069 7320 6e6f 7420  olicy_id is not 
-000de0d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000de0e0: 2020 7265 7375 6c74 5b27 6175 746f 5f73    result['auto_s
-000de0f0: 6e61 7073 686f 745f 706f 6c69 6379 5f69  napshot_policy_i
-000de100: 6427 5d20 3d20 7365 6c66 2e61 7574 6f5f  d'] = self.auto_
-000de110: 736e 6170 7368 6f74 5f70 6f6c 6963 795f  snapshot_policy_
-000de120: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-000de130: 6c66 2e63 6174 6567 6f72 7920 6973 206e  lf.category is n
-000de140: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000de150: 2020 2020 2072 6573 756c 745b 2763 6174       result['cat
-000de160: 6567 6f72 7927 5d20 3d20 7365 6c66 2e63  egory'] = self.c
-000de170: 6174 6567 6f72 790a 2020 2020 2020 2020  ategory.        
-000de180: 6966 2073 656c 662e 656e 6372 7970 7465  if self.encrypte
-000de190: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000de1a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000de1b0: 745b 2765 6e63 7279 7074 6564 275d 203d  t['encrypted'] =
-000de1c0: 2073 656c 662e 656e 6372 7970 7465 640a   self.encrypted.
-000de1d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000de1e0: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
-000de1f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000de200: 7375 6c74 5b27 7369 7a65 275d 203d 2073  sult['size'] = s
-000de210: 656c 662e 7369 7a65 0a20 2020 2020 2020  elf.size.       
-000de220: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000de230: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000de240: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-000de250: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-000de260: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-000de270: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000de280: 2827 6175 746f 5f73 6e61 7073 686f 745f  ('auto_snapshot_
-000de290: 706f 6c69 6379 5f69 6427 2920 6973 206e  policy_id') is n
-000de2a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000de2b0: 2020 2020 2073 656c 662e 6175 746f 5f73       self.auto_s
-000de2c0: 6e61 7073 686f 745f 706f 6c69 6379 5f69  napshot_policy_i
-000de2d0: 6420 3d20 6d2e 6765 7428 2761 7574 6f5f  d = m.get('auto_
-000de2e0: 736e 6170 7368 6f74 5f70 6f6c 6963 795f  snapshot_policy_
-000de2f0: 6964 2729 0a20 2020 2020 2020 2069 6620  id').        if 
-000de300: 6d2e 6765 7428 2763 6174 6567 6f72 7927  m.get('category'
-000de310: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000de320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000de330: 6361 7465 676f 7279 203d 206d 2e67 6574  category = m.get
-000de340: 2827 6361 7465 676f 7279 2729 0a20 2020  ('category').   
-000de350: 2020 2020 2069 6620 6d2e 6765 7428 2765       if m.get('e
-000de360: 6e63 7279 7074 6564 2729 2069 7320 6e6f  ncrypted') is no
-000de370: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000de380: 2020 2020 7365 6c66 2e65 6e63 7279 7074      self.encrypt
-000de390: 6564 203d 206d 2e67 6574 2827 656e 6372  ed = m.get('encr
-000de3a0: 7970 7465 6427 290a 2020 2020 2020 2020  ypted').        
-000de3b0: 6966 206d 2e67 6574 2827 7369 7a65 2729  if m.get('size')
-000de3c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000de3d0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000de3e0: 697a 6520 3d20 6d2e 6765 7428 2773 697a  ize = m.get('siz
-000de3f0: 6527 290a 2020 2020 2020 2020 7265 7475  e').        retu
-000de400: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000de410: 5363 616c 654f 7574 436c 7573 7465 7252  ScaleOutClusterR
-000de420: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-000de430: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000de440: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000de450: 2c0a 2020 2020 2020 2020 636c 6f75 645f  ,.        cloud_
-000de460: 6d6f 6e69 746f 725f 666c 6167 733a 2062  monitor_flags: b
-000de470: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-000de480: 2020 2020 636f 756e 743a 2069 6e74 203d      count: int =
-000de490: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-000de4a0: 7075 5f70 6f6c 6963 793a 2073 7472 203d  pu_policy: str =
-000de4b0: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
-000de4c0: 6d61 6765 5f69 643a 2073 7472 203d 204e  mage_id: str = N
-000de4d0: 6f6e 652c 0a20 2020 2020 2020 206b 6579  one,.        key
-000de4e0: 5f70 6169 723a 2073 7472 203d 204e 6f6e  _pair: str = Non
-000de4f0: 652c 0a20 2020 2020 2020 206c 6f67 696e  e,.        login
-000de500: 5f70 6173 7377 6f72 643a 2073 7472 203d  _password: str =
-000de510: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-000de520: 6473 5f69 6e73 7461 6e63 6573 3a20 4c69  ds_instances: Li
-000de530: 7374 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  st[str] = None,.
-000de540: 2020 2020 2020 2020 7275 6e74 696d 653a          runtime:
-000de550: 2052 756e 7469 6d65 203d 204e 6f6e 652c   Runtime = None,
-000de560: 0a20 2020 2020 2020 2074 6167 733a 204c  .        tags: L
-000de570: 6973 745b 5461 675d 203d 204e 6f6e 652c  ist[Tag] = None,
-000de580: 0a20 2020 2020 2020 2074 6169 6e74 733a  .        taints:
-000de590: 204c 6973 745b 5461 696e 745d 203d 204e   List[Taint] = N
-000de5a0: 6f6e 652c 0a20 2020 2020 2020 2075 7365  one,.        use
-000de5b0: 725f 6461 7461 3a20 7374 7220 3d20 4e6f  r_data: str = No
-000de5c0: 6e65 2c0a 2020 2020 2020 2020 7673 7769  ne,.        vswi
-000de5d0: 7463 685f 6964 733a 204c 6973 745b 7374  tch_ids: List[st
-000de5e0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-000de5f0: 2020 2077 6f72 6b65 725f 6175 746f 5f72     worker_auto_r
-000de600: 656e 6577 3a20 626f 6f6c 203d 204e 6f6e  enew: bool = Non
-000de610: 652c 0a20 2020 2020 2020 2077 6f72 6b65  e,.        worke
-000de620: 725f 6175 746f 5f72 656e 6577 5f70 6572  r_auto_renew_per
-000de630: 696f 643a 2069 6e74 203d 204e 6f6e 652c  iod: int = None,
-000de640: 0a20 2020 2020 2020 2077 6f72 6b65 725f  .        worker_
-000de650: 6461 7461 5f64 6973 6b73 3a20 4c69 7374  data_disks: List
-000de660: 5b53 6361 6c65 4f75 7443 6c75 7374 6572  [ScaleOutCluster
-000de670: 5265 7175 6573 7457 6f72 6b65 7244 6174  RequestWorkerDat
-000de680: 6144 6973 6b73 5d20 3d20 4e6f 6e65 2c0a  aDisks] = None,.
-000de690: 2020 2020 2020 2020 776f 726b 6572 5f69          worker_i
-000de6a0: 6e73 7461 6e63 655f 6368 6172 6765 5f74  nstance_charge_t
-000de6b0: 7970 653a 2073 7472 203d 204e 6f6e 652c  ype: str = None,
-000de6c0: 0a20 2020 2020 2020 2077 6f72 6b65 725f  .        worker_
-000de6d0: 696e 7374 616e 6365 5f74 7970 6573 3a20  instance_types: 
-000de6e0: 4c69 7374 5b73 7472 5d20 3d20 4e6f 6e65  List[str] = None
-000de6f0: 2c0a 2020 2020 2020 2020 776f 726b 6572  ,.        worker
-000de700: 5f70 6572 696f 643a 2069 6e74 203d 204e  _period: int = N
-000de710: 6f6e 652c 0a20 2020 2020 2020 2077 6f72  one,.        wor
-000de720: 6b65 725f 7065 7269 6f64 5f75 6e69 743a  ker_period_unit:
-000de730: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000de740: 2020 2020 2077 6f72 6b65 725f 7379 7374       worker_syst
-000de750: 656d 5f64 6973 6b5f 6361 7465 676f 7279  em_disk_category
-000de760: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000de770: 2020 2020 2020 776f 726b 6572 5f73 7973        worker_sys
-000de780: 7465 6d5f 6469 736b 5f73 697a 653a 2069  tem_disk_size: i
-000de790: 6e74 203d 204e 6f6e 652c 0a20 2020 2029  nt = None,.    )
-000de7a0: 3a0a 2020 2020 2020 2020 2320 5370 6563  :.        # Spec
-000de7b0: 6966 6965 7320 7768 6574 6865 7220 746f  ifies whether to
-000de7c0: 2069 6e73 7461 6c6c 2074 6865 2043 6c6f   install the Clo
-000de7d0: 7564 4d6f 6e69 746f 7220 6167 656e 742e  udMonitor agent.
-000de7e0: 2056 616c 6964 2076 616c 7565 733a 0a20   Valid values:. 
-000de7f0: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
-000de800: 2020 2320 2a20 2020 6074 7275 6560 3a20    # *   `true`: 
-000de810: 696e 7374 616c 6c73 2074 6865 2043 6c6f  installs the Clo
-000de820: 7564 4d6f 6e69 746f 7220 6167 656e 742e  udMonitor agent.
-000de830: 0a20 2020 2020 2020 2023 202a 2020 2060  .        # *   `
-000de840: 6661 6c73 6560 3a20 646f 6573 206e 6f74  false`: does not
-000de850: 2069 6e73 7461 6c6c 2074 6865 2043 6c6f   install the Clo
-000de860: 7564 4d6f 6e69 746f 7220 6167 656e 742e  udMonitor agent.
-000de870: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
-000de880: 2020 2020 2320 4465 6661 756c 7420 7661      # Default va
-000de890: 6c75 653a 2060 6661 6c73 6560 2e0a 2020  lue: `false`..  
-000de8a0: 2020 2020 2020 7365 6c66 2e63 6c6f 7564        self.cloud
-000de8b0: 5f6d 6f6e 6974 6f72 5f66 6c61 6773 203d  _monitor_flags =
-000de8c0: 2063 6c6f 7564 5f6d 6f6e 6974 6f72 5f66   cloud_monitor_f
-000de8d0: 6c61 6773 0a20 2020 2020 2020 2023 2054  lags.        # T
-000de8e0: 6865 206e 756d 6265 7220 6f66 2077 6f72  he number of wor
-000de8f0: 6b65 7220 6e6f 6465 7320 7468 6174 2079  ker nodes that y
-000de900: 6f75 2077 616e 7420 746f 2061 6464 2e0a  ou want to add..
-000de910: 2020 2020 2020 2020 2320 0a20 2020 2020          # .     
-000de920: 2020 2023 2054 6869 7320 7061 7261 6d65     # This parame
-000de930: 7465 7220 6973 2072 6571 7569 7265 642e  ter is required.
-000de940: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-000de950: 756e 7420 3d20 636f 756e 740a 2020 2020  unt = count.    
-000de960: 2020 2020 2320 5468 6520 4350 5520 6d61      # The CPU ma
-000de970: 6e61 6765 6d65 6e74 2070 6f6c 6963 7920  nagement policy 
-000de980: 6f66 2074 6865 206e 6f64 6573 2069 6e20  of the nodes in 
-000de990: 6120 6e6f 6465 2070 6f6f 6c2e 2054 6865  a node pool. The
-000de9a0: 2066 6f6c 6c6f 7769 6e67 2070 6f6c 6963   following polic
-000de9b0: 6965 7320 6172 6520 7375 7070 6f72 7465  ies are supporte
-000de9c0: 6420 6966 2074 6865 204b 7562 6572 6e65  d if the Kuberne
-000de9d0: 7465 7320 7665 7273 696f 6e20 6f66 2074  tes version of t
-000de9e0: 6865 2063 6c75 7374 6572 2069 7320 312e  he cluster is 1.
-000de9f0: 3132 2e36 206f 7220 6c61 7465 722e 0a20  12.6 or later.. 
-000dea00: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
-000dea10: 2020 2320 2a20 2020 6073 7461 7469 6360    # *   `static`
-000dea20: 3a20 5468 6973 2070 6f6c 6963 7920 616c  : This policy al
-000dea30: 6c6f 7773 2070 6f64 7320 7769 7468 2073  lows pods with s
-000dea40: 7065 6369 6669 6320 7265 736f 7572 6365  pecific resource
-000dea50: 2063 6861 7261 6374 6572 6973 7469 6373   characteristics
-000dea60: 206f 6e20 7468 6520 6e6f 6465 2074 6f20   on the node to 
-000dea70: 6265 2067 7261 6e74 6564 2077 6974 6820  be granted with 
-000dea80: 656e 6861 6e63 6564 2043 5055 2061 6666  enhanced CPU aff
-000dea90: 696e 6974 7920 616e 6420 6578 636c 7573  inity and exclus
-000deaa0: 6976 6974 792e 0a20 2020 2020 2020 2023  ivity..        #
-000deab0: 202a 2020 2060 6e6f 6e65 603a 2054 6865   *   `none`: The
-000deac0: 2064 6566 6175 6c74 2043 5055 2061 6666   default CPU aff
-000dead0: 696e 6974 7920 6973 2075 7365 642e 0a20  inity is used.. 
-000deae0: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
-000deaf0: 2020 2320 4465 6661 756c 7420 7661 6c75    # Default valu
-000deb00: 653a 2060 6e6f 6e65 602e 0a20 2020 2020  e: `none`..     
-000deb10: 2020 2073 656c 662e 6370 755f 706f 6c69     self.cpu_poli
-000deb20: 6379 203d 2063 7075 5f70 6f6c 6963 790a  cy = cpu_policy.
-000deb30: 2020 2020 2020 2020 2320 5370 6563 6966          # Specif
-000deb40: 6965 7320 6120 6375 7374 6f6d 2069 6d61  ies a custom ima
-000deb50: 6765 2066 6f72 206e 6f64 6573 2e20 4279  ge for nodes. By
-000deb60: 2064 6566 6175 6c74 2c20 7468 6520 696d   default, the im
-000deb70: 6167 6520 7072 6f76 6964 6564 2062 7920  age provided by 
-000deb80: 436f 6e74 6169 6e65 7220 5365 7276 6963  Container Servic
-000deb90: 6520 666f 7220 4b75 6265 726e 6574 6573  e for Kubernetes
-000deba0: 2028 4143 4b29 2069 7320 7573 6564 2e20   (ACK) is used. 
-000debb0: 596f 7520 6361 6e20 7365 6c65 6374 2061  You can select a
-000debc0: 2063 7573 746f 6d20 696d 6167 6520 746f   custom image to
-000debd0: 2072 6570 6c61 6365 2074 6865 2064 6566   replace the def
-000debe0: 6175 6c74 2069 6d61 6765 2e20 466f 7220  ault image. For 
-000debf0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-000dec00: 2c20 7365 6520 5b43 7573 746f 6d20 696d  , see [Custom im
-000dec10: 6167 6573 5d28 6874 7470 733a 2f2f 6865  ages](https://he
-000dec20: 6c70 2e61 6c69 7975 6e2e 636f 6d2f 646f  lp.aliyun.com/do
-000dec30: 6375 6d65 6e74 5f64 6574 6169 6c2f 3134  cument_detail/14
-000dec40: 3636 3437 2e68 746d 6c29 2e0a 2020 2020  6647.html)..    
-000dec50: 2020 2020 7365 6c66 2e69 6d61 6765 5f69      self.image_i
-000dec60: 6420 3d20 696d 6167 655f 6964 0a20 2020  d = image_id.   
-000dec70: 2020 2020 2023 2054 6865 206e 616d 6520       # The name 
-000dec80: 6f66 2074 6865 206b 6579 2070 6169 722e  of the key pair.
-000dec90: 2059 6f75 206d 7573 7420 7365 7420 7468   You must set th
-000deca0: 6973 2070 6172 616d 6574 6572 206f 7220  is parameter or 
-000decb0: 7468 6520 606c 6f67 696e 5f70 6173 7377  the `login_passw
-000decc0: 6f72 6460 2070 6172 616d 6574 6572 2e0a  ord` parameter..
-000decd0: 2020 2020 2020 2020 2320 0a20 2020 2020          # .     
-000dece0: 2020 2023 2054 6869 7320 7061 7261 6d65     # This parame
-000decf0: 7465 7220 6973 2072 6571 7569 7265 642e  ter is required.
-000ded00: 0a20 2020 2020 2020 2073 656c 662e 6b65  .        self.ke
-000ded10: 795f 7061 6972 203d 206b 6579 5f70 6169  y_pair = key_pai
-000ded20: 720a 2020 2020 2020 2020 2320 5468 6520  r.        # The 
-000ded30: 7061 7373 776f 7264 2066 6f72 2053 5348  password for SSH
-000ded40: 206c 6f67 6f6e 2e20 596f 7520 6d75 7374   logon. You must
-000ded50: 2073 6574 2074 6869 7320 7061 7261 6d65   set this parame
-000ded60: 7465 7220 6f72 2074 6865 2060 6b65 795f  ter or the `key_
-000ded70: 7061 6972 6020 7061 7261 6d65 7465 722e  pair` parameter.
-000ded80: 2054 6865 2070 6173 7377 6f72 6420 6d75   The password mu
-000ded90: 7374 2062 6520 3820 746f 2033 3020 6368  st be 8 to 30 ch
-000deda0: 6172 6163 7465 7273 2069 6e20 6c65 6e67  aracters in leng
-000dedb0: 7468 2c20 616e 6420 6d75 7374 2063 6f6e  th, and must con
-000dedc0: 7461 696e 2061 7420 6c65 6173 7420 7468  tain at least th
-000dedd0: 7265 6520 6f66 2074 6865 2066 6f6c 6c6f  ree of the follo
-000dede0: 7769 6e67 2063 6861 7261 6374 6572 2074  wing character t
-000dedf0: 7970 6573 3a20 7570 7065 7263 6173 6520  ypes: uppercase 
-000dee00: 6c65 7474 6572 732c 206c 6f77 6572 6361  letters, lowerca
-000dee10: 7365 206c 6574 7465 7273 2c20 6469 6769  se letters, digi
-000dee20: 7473 2c20 616e 6420 7370 6563 6961 6c20  ts, and special 
-000dee30: 6368 6172 6163 7465 7273 2e0a 2020 2020  characters..    
-000dee40: 2020 2020 2320 0a20 2020 2020 2020 2023      # .        #
-000dee50: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
-000dee60: 6973 2072 6571 7569 7265 642e 0a20 2020  is required..   
-000dee70: 2020 2020 2073 656c 662e 6c6f 6769 6e5f       self.login_
-000dee80: 7061 7373 776f 7264 203d 206c 6f67 696e  password = login
-000dee90: 5f70 6173 7377 6f72 640a 2020 2020 2020  _password.      
-000deea0: 2020 2320 4166 7465 7220 796f 7520 7370    # After you sp
-000deeb0: 6563 6966 7920 7468 6520 6c69 7374 206f  ecify the list o
-000deec0: 6620 4170 7361 7261 4442 2052 4453 2069  f ApsaraDB RDS i
-000deed0: 6e73 7461 6e63 6573 2c20 7468 6520 4543  nstances, the EC
-000deee0: 5320 696e 7374 616e 6365 7320 696e 2074  S instances in t
-000deef0: 6865 2063 6c75 7374 6572 2061 7265 2061  he cluster are a
-000def00: 7574 6f6d 6174 6963 616c 6c79 2061 6464  utomatically add
-000def10: 6564 2074 6f20 7468 6520 7768 6974 656c  ed to the whitel
-000def20: 6973 7420 6f66 2074 6865 2041 7073 6172  ist of the Apsar
-000def30: 6144 4220 5244 5320 696e 7374 616e 6365  aDB RDS instance
-000def40: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-000def50: 7264 735f 696e 7374 616e 6365 7320 3d20  rds_instances = 
-000def60: 7264 735f 696e 7374 616e 6365 730a 2020  rds_instances.  
-000def70: 2020 2020 2020 2320 5468 6520 636f 6e74        # The cont
-000def80: 6169 6e65 7220 7275 6e74 696d 652e 0a20  ainer runtime.. 
-000def90: 2020 2020 2020 2073 656c 662e 7275 6e74         self.runt
-000defa0: 696d 6520 3d20 7275 6e74 696d 650a 2020  ime = runtime.  
-000defb0: 2020 2020 2020 2320 5468 6520 6c61 6265        # The labe
-000defc0: 6c73 2074 6861 7420 796f 7520 7761 6e74  ls that you want
-000defd0: 2074 6f20 6164 6420 746f 206e 6f64 6573   to add to nodes
-000defe0: 2e20 596f 7520 6d75 7374 2061 6464 206c  . You must add l
-000deff0: 6162 656c 7320 6261 7365 6420 6f6e 2074  abels based on t
-000df000: 6865 2066 6f6c 6c6f 7769 6e67 2072 756c  he following rul
-000df010: 6573 3a0a 2020 2020 2020 2020 2320 0a20  es:.        # . 
-000df020: 2020 2020 2020 2023 202a 2020 2045 6163         # *   Eac
-000df030: 6820 6c61 6265 6c20 6973 2061 2063 6173  h label is a cas
-000df040: 652d 7365 6e73 6974 6976 6520 6b65 792d  e-sensitive key-
-000df050: 7661 6c75 6520 7061 6972 2e20 596f 7520  value pair. You 
-000df060: 6361 6e20 6164 6420 7570 2074 6f20 3230  can add up to 20
-000df070: 206c 6162 656c 732e 0a20 2020 2020 2020   labels..       
-000df080: 2023 202a 2020 2041 206b 6579 206d 7573   # *   A key mus
-000df090: 7420 6265 2075 6e69 7175 6520 616e 6420  t be unique and 
-000df0a0: 6361 6e6e 6f74 2065 7863 6565 6420 3634  cannot exceed 64
-000df0b0: 2063 6861 7261 6374 6572 7320 696e 206c   characters in l
-000df0c0: 656e 6774 682e 2041 2076 616c 7565 2063  ength. A value c
-000df0d0: 616e 2062 6520 656d 7074 7920 616e 6420  an be empty and 
-000df0e0: 6361 6e6e 6f74 2065 7863 6565 6420 3132  cannot exceed 12
-000df0f0: 3820 6368 6172 6163 7465 7273 2069 6e20  8 characters in 
-000df100: 6c65 6e67 7468 2e20 4b65 7973 2061 6e64  length. Keys and
-000df110: 2076 616c 7565 7320 6361 6e6e 6f74 2073   values cannot s
-000df120: 7461 7274 2077 6974 6820 616c 6979 756e  tart with aliyun
-000df130: 2c20 6163 733a 2c20 6874 7470 733a 2f2f  , acs:, https://
-000df140: 2c20 6f72 2068 7474 703a 2f2f 2e20 466f  , or http://. Fo
-000df150: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-000df160: 6f6e 2c20 7365 6520 5b4c 6162 656c 7320  on, see [Labels 
-000df170: 616e 6420 5365 6c65 6374 6f72 735d 2868  and Selectors](h
-000df180: 7474 7073 3a2f 2f6b 7562 6572 6e65 7465  ttps://kubernete
-000df190: 732e 696f 2f64 6f63 732f 636f 6e63 6570  s.io/docs/concep
-000df1a0: 7473 2f6f 7665 7276 6965 772f 776f 726b  ts/overview/work
-000df1b0: 696e 672d 7769 7468 2d6f 626a 6563 7473  ing-with-objects
-000df1c0: 2f6c 6162 656c 732f 2373 796e 7461 782d  /labels/#syntax-
-000df1d0: 616e 642d 6368 6172 6163 7465 722d 7365  and-character-se
-000df1e0: 7429 2e0a 2020 2020 2020 2020 7365 6c66  t)..        self
-000df1f0: 2e74 6167 7320 3d20 7461 6773 0a20 2020  .tags = tags.   
-000df200: 2020 2020 2023 2054 6865 2074 6169 6e74       # The taint
-000df210: 7320 7468 6174 2079 6f75 2077 616e 7420  s that you want 
-000df220: 746f 2061 6464 2074 6f20 6e6f 6465 732e  to add to nodes.
-000df230: 2054 6169 6e74 7320 6172 6520 6164 6465   Taints are adde
-000df240: 6420 746f 206e 6f64 6573 2074 6f20 7072  d to nodes to pr
-000df250: 6576 656e 7420 706f 6473 2066 726f 6d20  event pods from 
-000df260: 6265 696e 6720 7363 6865 6475 6c65 6420  being scheduled 
-000df270: 746f 2069 6e61 7070 726f 7072 6961 7465  to inappropriate
-000df280: 206e 6f64 6573 2e20 486f 7765 7665 722c   nodes. However,
-000df290: 2074 6f6c 6572 6174 696f 6e73 2061 6c6c   tolerations all
-000df2a0: 6f77 2070 6f64 7320 746f 2062 6520 7363  ow pods to be sc
-000df2b0: 6865 6475 6c65 6420 746f 206e 6f64 6573  heduled to nodes
-000df2c0: 2077 6974 6820 6d61 7463 6869 6e67 2074   with matching t
-000df2d0: 6169 6e74 732e 2046 6f72 206d 6f72 6520  aints. For more 
-000df2e0: 696e 666f 726d 6174 696f 6e2c 2073 6565  information, see
-000df2f0: 205b 5461 696e 7473 2061 6e64 2054 6f6c   [Taints and Tol
-000df300: 6572 6174 696f 6e73 5d28 6874 7470 733a  erations](https:
-000df310: 2f2f 6b75 6265 726e 6574 6573 2e69 6f2f  //kubernetes.io/
-000df320: 7a68 2f64 6f63 732f 636f 6e63 6570 7473  zh/docs/concepts
-000df330: 2f73 6368 6564 756c 696e 672d 6576 6963  /scheduling-evic
-000df340: 7469 6f6e 2f74 6169 6e74 2d61 6e64 2d74  tion/taint-and-t
-000df350: 6f6c 6572 6174 696f 6e2f 292e 0a20 2020  oleration/)..   
-000df360: 2020 2020 2073 656c 662e 7461 696e 7473       self.taints
-000df370: 203d 2074 6169 6e74 730a 2020 2020 2020   = taints.      
-000df380: 2020 2320 5468 6520 7573 6572 2064 6174    # The user dat
-000df390: 6120 6f66 2074 6865 206e 6f64 6520 706f  a of the node po
-000df3a0: 6f6c 2e20 466f 7220 6d6f 7265 2069 6e66  ol. For more inf
-000df3b0: 6f72 6d61 7469 6f6e 2c20 7365 6520 5b47  ormation, see [G
-000df3c0: 656e 6572 6174 6520 7573 6572 2d64 6566  enerate user-def
-000df3d0: 696e 6564 2064 6174 615d 2868 7474 7073  ined data](https
-000df3e0: 3a2f 2f68 656c 702e 616c 6979 756e 2e63  ://help.aliyun.c
-000df3f0: 6f6d 2f64 6f63 756d 656e 745f 6465 7461  om/document_deta
-000df400: 696c 2f34 3931 3231 2e68 746d 6c29 2e0a  il/49121.html)..
-000df410: 2020 2020 2020 2020 7365 6c66 2e75 7365          self.use
-000df420: 725f 6461 7461 203d 2075 7365 725f 6461  r_data = user_da
-000df430: 7461 0a20 2020 2020 2020 2023 2054 6865  ta.        # The
-000df440: 2049 4473 206f 6620 7468 6520 7653 7769   IDs of the vSwi
-000df450: 7463 6865 732e 2059 6f75 2063 616e 2073  tches. You can s
-000df460: 656c 6563 7420 6f6e 6520 746f 2074 6872  elect one to thr
-000df470: 6565 2076 5377 6974 6368 6573 2077 6865  ee vSwitches whe
-000df480: 6e20 796f 7520 6372 6561 7465 2061 2063  n you create a c
-000df490: 6c75 7374 6572 2e20 5765 2072 6563 6f6d  luster. We recom
-000df4a0: 6d65 6e64 2074 6861 7420 796f 7520 7365  mend that you se
-000df4b0: 6c65 6374 2076 5377 6974 6368 6573 2069  lect vSwitches i
-000df4c0: 6e20 6469 6666 6572 656e 7420 7a6f 6e65  n different zone
-000df4d0: 7320 746f 2065 6e73 7572 6520 6869 6768  s to ensure high
-000df4e0: 2061 7661 696c 6162 696c 6974 792e 0a20   availability.. 
-000df4f0: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
-000df500: 2020 2320 5468 6973 2070 6172 616d 6574    # This paramet
-000df510: 6572 2069 7320 7265 7175 6972 6564 2e0a  er is required..
-000df520: 2020 2020 2020 2020 7365 6c66 2e76 7377          self.vsw
-000df530: 6974 6368 5f69 6473 203d 2076 7377 6974  itch_ids = vswit
-000df540: 6368 5f69 6473 0a20 2020 2020 2020 2023  ch_ids.        #
-000df550: 2053 7065 6369 6669 6573 2077 6865 7468   Specifies wheth
-000df560: 6572 2074 6f20 656e 6162 6c65 2061 7574  er to enable aut
-000df570: 6f2d 7265 6e65 7761 6c20 666f 7220 776f  o-renewal for wo
-000df580: 726b 6572 206e 6f64 6573 2e20 5468 6973  rker nodes. This
-000df590: 2070 6172 616d 6574 6572 2074 616b 6573   parameter takes
-000df5a0: 2065 6666 6563 7420 6f6e 6c79 2069 6620   effect only if 
-000df5b0: 6077 6f72 6b65 725f 696e 7374 616e 6365  `worker_instance
-000df5c0: 5f63 6861 7267 655f 7479 7065 6020 6973  _charge_type` is
-000df5d0: 2073 6574 2074 6f20 6050 7265 5061 6964   set to `PrePaid
-000df5e0: 602e 2056 616c 6964 2076 616c 7565 733a  `. Valid values:
-000df5f0: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
-000df600: 2020 2020 2320 2a20 2020 6074 7275 6560      # *   `true`
-000df610: 3a20 656e 6162 6c65 7320 6175 746f 2d72  : enables auto-r
-000df620: 656e 6577 616c 2e0a 2020 2020 2020 2020  enewal..        
-000df630: 2320 2a20 2020 6066 616c 7365 603a 2064  # *   `false`: d
-000df640: 6973 6162 6c65 7320 6175 746f 2d72 656e  isables auto-ren
-000df650: 6577 616c 2e0a 2020 2020 2020 2020 2320  ewal..        # 
-000df660: 0a20 2020 2020 2020 2023 2044 6566 6175  .        # Defau
-000df670: 6c74 2076 616c 7565 3a20 6074 7275 6560  lt value: `true`
-000df680: 2e0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-000df690: 6f72 6b65 725f 6175 746f 5f72 656e 6577  orker_auto_renew
-000df6a0: 203d 2077 6f72 6b65 725f 6175 746f 5f72   = worker_auto_r
-000df6b0: 656e 6577 0a20 2020 2020 2020 2023 2054  enew.        # T
-000df6c0: 6865 2061 7574 6f2d 7265 6e65 7761 6c20  he auto-renewal 
-000df6d0: 7065 7269 6f64 2066 6f72 2077 6f72 6b65  period for worke
-000df6e0: 7220 6e6f 6465 7320 6166 7465 7220 7468  r nodes after th
-000df6f0: 6520 7375 6273 6372 6970 7469 6f6e 7320  e subscriptions 
-000df700: 6f66 2077 6f72 6b65 7220 6e6f 6465 7320  of worker nodes 
-000df710: 6578 7069 7265 2e20 5468 6973 2070 6172  expire. This par
-000df720: 616d 6574 6572 2074 616b 6573 2065 6666  ameter takes eff
-000df730: 6563 7420 616e 6420 6973 2072 6571 7569  ect and is requi
-000df740: 7265 6420 6f6e 6c79 2069 6620 7468 6520  red only if the 
-000df750: 7375 6273 6372 6970 7469 6f6e 2062 696c  subscription bil
-000df760: 6c69 6e67 206d 6574 686f 6420 6973 2073  ling method is s
-000df770: 656c 6563 7465 6420 666f 7220 776f 726b  elected for work
-000df780: 6572 206e 6f64 6573 2e0a 2020 2020 2020  er nodes..      
-000df790: 2020 2320 0a20 2020 2020 2020 2023 2056    # .        # V
-000df7a0: 616c 6964 2076 616c 7565 733a 2031 2c20  alid values: 1, 
-000df7b0: 322c 2033 2c20 362c 2061 6e64 2031 322e  2, 3, 6, and 12.
-000df7c0: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
-000df7d0: 2020 2020 2320 4465 6661 756c 7420 7661      # Default va
-000df7e0: 6c75 653a 2060 3160 2e0a 2020 2020 2020  lue: `1`..      
-000df7f0: 2020 7365 6c66 2e77 6f72 6b65 725f 6175    self.worker_au
-000df800: 746f 5f72 656e 6577 5f70 6572 696f 6420  to_renew_period 
-000df810: 3d20 776f 726b 6572 5f61 7574 6f5f 7265  = worker_auto_re
-000df820: 6e65 775f 7065 7269 6f64 0a20 2020 2020  new_period.     
-000df830: 2020 2023 2054 6865 2063 6f6e 6669 6775     # The configu
-000df840: 7261 7469 6f6e 206f 6620 7468 6520 6461  ration of the da
-000df850: 7461 2064 6973 6b20 7468 6174 2069 7320  ta disk that is 
-000df860: 6d6f 756e 7465 6420 746f 2077 6f72 6b65  mounted to worke
-000df870: 7220 6e6f 6465 732e 2054 6865 2063 6f6e  r nodes. The con
-000df880: 6669 6775 7261 7469 6f6e 2069 6e63 6c75  figuration inclu
-000df890: 6465 7320 7468 6520 6469 736b 2074 7970  des the disk typ
-000df8a0: 6520 616e 6420 6469 736b 2073 697a 652e  e and disk size.
-000df8b0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-000df8c0: 726b 6572 5f64 6174 615f 6469 736b 7320  rker_data_disks 
-000df8d0: 3d20 776f 726b 6572 5f64 6174 615f 6469  = worker_data_di
-000df8e0: 736b 730a 2020 2020 2020 2020 2320 5468  sks.        # Th
-000df8f0: 6520 6269 6c6c 696e 6720 6d65 7468 6f64  e billing method
-000df900: 206f 6620 776f 726b 6572 206e 6f64 6573   of worker nodes
-000df910: 2e20 5661 6c69 6420 7661 6c75 6573 3a0a  . Valid values:.
-000df920: 2020 2020 2020 2020 2320 0a20 2020 2020          # .     
-000df930: 2020 2023 202a 2020 2060 5072 6550 6169     # *   `PrePai
-000df940: 6460 3a20 7375 6273 6372 6970 7469 6f6e  d`: subscription
-000df950: 2e0a 2020 2020 2020 2020 2320 2a20 2020  ..        # *   
-000df960: 6050 6f73 7450 6169 6460 3a20 7061 792d  `PostPaid`: pay-
-000df970: 6173 2d79 6f75 2d67 6f2e 0a20 2020 2020  as-you-go..     
-000df980: 2020 2023 200a 2020 2020 2020 2020 2320     # .        # 
-000df990: 4465 6661 756c 7420 7661 6c75 653a 2060  Default value: `
-000df9a0: 506f 7374 5061 6964 602e 0a20 2020 2020  PostPaid`..     
-000df9b0: 2020 2073 656c 662e 776f 726b 6572 5f69     self.worker_i
-000df9c0: 6e73 7461 6e63 655f 6368 6172 6765 5f74  nstance_charge_t
-000df9d0: 7970 6520 3d20 776f 726b 6572 5f69 6e73  ype = worker_ins
-000df9e0: 7461 6e63 655f 6368 6172 6765 5f74 7970  tance_charge_typ
-000df9f0: 650a 2020 2020 2020 2020 2320 5468 6520  e.        # The 
-000dfa00: 696e 7374 616e 6365 2063 6f6e 6669 6775  instance configu
-000dfa10: 7261 7469 6f6e 7320 6f66 2077 6f72 6b65  rations of worke
-000dfa20: 7220 6e6f 6465 732e 0a20 2020 2020 2020  r nodes..       
-000dfa30: 2023 200a 2020 2020 2020 2020 2320 5468   # .        # Th
-000dfa40: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
-000dfa50: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
-000dfa60: 2020 7365 6c66 2e77 6f72 6b65 725f 696e    self.worker_in
-000dfa70: 7374 616e 6365 5f74 7970 6573 203d 2077  stance_types = w
-000dfa80: 6f72 6b65 725f 696e 7374 616e 6365 5f74  orker_instance_t
-000dfa90: 7970 6573 0a20 2020 2020 2020 2023 2054  ypes.        # T
-000dfaa0: 6865 2073 7562 7363 7269 7074 696f 6e20  he subscription 
-000dfab0: 6475 7261 7469 6f6e 206f 6620 776f 726b  duration of work
-000dfac0: 6572 206e 6f64 6573 2e20 5468 6973 2070  er nodes. This p
-000dfad0: 6172 616d 6574 6572 2074 616b 6573 2065  arameter takes e
-000dfae0: 6666 6563 7420 616e 6420 6973 2072 6571  ffect and is req
-000dfaf0: 7569 7265 6420 6f6e 6c79 2069 6620 6077  uired only if `w
-000dfb00: 6f72 6b65 725f 696e 7374 616e 6365 5f63  orker_instance_c
-000dfb10: 6861 7267 655f 7479 7065 6020 6973 2073  harge_type` is s
-000dfb20: 6574 2074 6f20 6050 7265 5061 6964 602e  et to `PrePaid`.
-000dfb30: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
-000dfb40: 2020 2020 2320 5661 6c69 6420 7661 6c75      # Valid valu
-000dfb50: 6573 3a20 312c 2032 2c20 332c 2036 2c20  es: 1, 2, 3, 6, 
-000dfb60: 3132 2c20 3234 2c20 3336 2c20 3438 2c20  12, 24, 36, 48, 
-000dfb70: 616e 6420 3630 2e0a 2020 2020 2020 2020  and 60..        
-000dfb80: 2320 0a20 2020 2020 2020 2023 2044 6566  # .        # Def
-000dfb90: 6175 6c74 2076 616c 7565 3a20 312e 0a20  ault value: 1.. 
-000dfba0: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
-000dfbb0: 6572 5f70 6572 696f 6420 3d20 776f 726b  er_period = work
-000dfbc0: 6572 5f70 6572 696f 640a 2020 2020 2020  er_period.      
-000dfbd0: 2020 2320 5468 6520 6269 6c6c 696e 6720    # The billing 
-000dfbe0: 6379 636c 6520 6f66 2077 6f72 6b65 7220  cycle of worker 
-000dfbf0: 6e6f 6465 732e 2054 6869 7320 7061 7261  nodes. This para
-000dfc00: 6d65 7465 7220 6973 2072 6571 7569 7265  meter is require
-000dfc10: 6420 6966 2077 6f72 6b65 725f 696e 7374  d if worker_inst
-000dfc20: 616e 6365 5f63 6861 7267 655f 7479 7065  ance_charge_type
-000dfc30: 2069 7320 7365 7420 746f 2060 5072 6550   is set to `PreP
-000dfc40: 6169 6460 2e0a 2020 2020 2020 2020 2320  aid`..        # 
-000dfc50: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
-000dfc60: 6865 2076 616c 7565 2074 6f20 604d 6f6e  he value to `Mon
-000dfc70: 7468 602e 2057 6f72 6b65 7220 6e6f 6465  th`. Worker node
-000dfc80: 7320 6172 6520 6269 6c6c 6564 206f 6e6c  s are billed onl
-000dfc90: 7920 6f6e 2061 206d 6f6e 7468 6c79 2062  y on a monthly b
-000dfca0: 6173 6973 2e0a 2020 2020 2020 2020 7365  asis..        se
-000dfcb0: 6c66 2e77 6f72 6b65 725f 7065 7269 6f64  lf.worker_period
-000dfcc0: 5f75 6e69 7420 3d20 776f 726b 6572 5f70  _unit = worker_p
-000dfcd0: 6572 696f 645f 756e 6974 0a20 2020 2020  eriod_unit.     
-000dfce0: 2020 2023 2054 6865 2074 7970 6520 6f66     # The type of
-000dfcf0: 2073 7973 7465 6d20 6469 736b 2074 6861   system disk tha
-000dfd00: 7420 796f 7520 7761 6e74 2074 6f20 7573  t you want to us
-000dfd10: 6520 666f 7220 776f 726b 6572 206e 6f64  e for worker nod
-000dfd20: 6573 2e20 5661 6c69 6420 7661 6c75 6573  es. Valid values
-000dfd30: 3a0a 2020 2020 2020 2020 2320 0a20 2020  :.        # .   
-000dfd40: 2020 2020 2023 202a 2020 2060 636c 6f75       # *   `clou
-000dfd50: 645f 6566 6669 6369 656e 6379 603a 2075  d_efficiency`: u
-000dfd60: 6c74 7261 2064 6973 6b2e 0a20 2020 2020  ltra disk..     
-000dfd70: 2020 2023 202a 2020 2060 636c 6f75 645f     # *   `cloud_
-000dfd80: 7373 6460 3a20 7374 616e 6461 7264 2053  ssd`: standard S
-000dfd90: 5344 2e0a 2020 2020 2020 2020 2320 2a20  SD..        # * 
-000dfda0: 2020 6063 6c6f 7564 5f65 7373 6460 3a20    `cloud_essd`: 
-000dfdb0: 656e 6861 6e63 6564 2053 5344 2028 4553  enhanced SSD (ES
-000dfdc0: 5344 292e 0a20 2020 2020 2020 2023 200a  SD)..        # .
-000dfdd0: 2020 2020 2020 2020 2320 4465 6661 756c          # Defaul
-000dfde0: 7420 7661 6c75 653a 2060 636c 6f75 645f  t value: `cloud_
-000dfdf0: 7373 6460 2e0a 2020 2020 2020 2020 2320  ssd`..        # 
-000dfe00: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
-000dfe10: 7061 7261 6d65 7465 7220 6973 2072 6571  parameter is req
-000dfe20: 7569 7265 642e 0a20 2020 2020 2020 2073  uired..        s
-000dfe30: 656c 662e 776f 726b 6572 5f73 7973 7465  elf.worker_syste
-000dfe40: 6d5f 6469 736b 5f63 6174 6567 6f72 7920  m_disk_category 
-000dfe50: 3d20 776f 726b 6572 5f73 7973 7465 6d5f  = worker_system_
-000dfe60: 6469 736b 5f63 6174 6567 6f72 790a 2020  disk_category.  
-000dfe70: 2020 2020 2020 2320 5468 6520 7369 7a65        # The size
-000dfe80: 206f 6620 7468 6520 7379 7374 656d 2064   of the system d
-000dfe90: 6973 6b20 7468 6174 2079 6f75 2077 616e  isk that you wan
-000dfea0: 7420 746f 2075 7365 2066 6f72 2077 6f72  t to use for wor
-000dfeb0: 6b65 7220 6e6f 6465 732e 2055 6e69 743a  ker nodes. Unit:
-000dfec0: 2047 6942 2e0a 2020 2020 2020 2020 2320   GiB..        # 
-000dfed0: 0a20 2020 2020 2020 2023 2056 616c 6964  .        # Valid
-000dfee0: 2076 616c 7565 733a 2034 3020 746f 2035   values: 40 to 5
-000dfef0: 3030 2e0a 2020 2020 2020 2020 2320 0a20  00..        # . 
-000dff00: 2020 2020 2020 2023 2044 6566 6175 6c74         # Default
-000dff10: 2076 616c 7565 3a20 6031 3230 602e 0a20   value: `120`.. 
-000dff20: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
-000dff30: 2020 2320 5468 6973 2070 6172 616d 6574    # This paramet
-000dff40: 6572 2069 7320 7265 7175 6972 6564 2e0a  er is required..
-000dff50: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-000dff60: 6b65 725f 7379 7374 656d 5f64 6973 6b5f  ker_system_disk_
-000dff70: 7369 7a65 203d 2077 6f72 6b65 725f 7379  size = worker_sy
-000dff80: 7374 656d 5f64 6973 6b5f 7369 7a65 0a0a  stem_disk_size..
-000dff90: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000dffa0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000dffb0: 6966 2073 656c 662e 7275 6e74 696d 653a  if self.runtime:
-000dffc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000dffd0: 662e 7275 6e74 696d 652e 7661 6c69 6461  f.runtime.valida
-000dffe0: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
-000dfff0: 7365 6c66 2e74 6167 733a 0a20 2020 2020  self.tags:.     
-000e0000: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-000e0010: 7365 6c66 2e74 6167 733a 0a20 2020 2020  self.tags:.     
-000e0020: 2020 2020 2020 2020 2020 2069 6620 6b3a             if k:
-000e0030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000e0040: 2020 2020 206b 2e76 616c 6964 6174 6528       k.validate(
-000e0050: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000e0060: 662e 7461 696e 7473 3a0a 2020 2020 2020  f.taints:.      
-000e0070: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
-000e0080: 656c 662e 7461 696e 7473 3a0a 2020 2020  elf.taints:.    
-000e0090: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-000e00a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000e00b0: 2020 2020 2020 6b2e 7661 6c69 6461 7465        k.validate
-000e00c0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-000e00d0: 6c66 2e77 6f72 6b65 725f 6461 7461 5f64  lf.worker_data_d
-000e00e0: 6973 6b73 3a0a 2020 2020 2020 2020 2020  isks:.          
-000e00f0: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-000e0100: 776f 726b 6572 5f64 6174 615f 6469 736b  worker_data_disk
-000e0110: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000e0120: 2020 2069 6620 6b3a 0a20 2020 2020 2020     if k:.       
-000e0130: 2020 2020 2020 2020 2020 2020 206b 2e76               k.v
-000e0140: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-000e0150: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000e0160: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-000e0170: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-000e0180: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-000e0190: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e01a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000e01b0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-000e01c0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-000e01d0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-000e01e0: 6c6f 7564 5f6d 6f6e 6974 6f72 5f66 6c61  loud_monitor_fla
-000e01f0: 6773 2069 7320 6e6f 7420 4e6f 6e65 3a0a  gs is not None:.
-000e0200: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000e0210: 6c74 5b27 636c 6f75 645f 6d6f 6e69 746f  lt['cloud_monito
-000e0220: 725f 666c 6167 7327 5d20 3d20 7365 6c66  r_flags'] = self
-000e0230: 2e63 6c6f 7564 5f6d 6f6e 6974 6f72 5f66  .cloud_monitor_f
-000e0240: 6c61 6773 0a20 2020 2020 2020 2069 6620  lags.        if 
-000e0250: 7365 6c66 2e63 6f75 6e74 2069 7320 6e6f  self.count is no
-000e0260: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e0270: 2020 2020 7265 7375 6c74 5b27 636f 756e      result['coun
-000e0280: 7427 5d20 3d20 7365 6c66 2e63 6f75 6e74  t'] = self.count
-000e0290: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e02a0: 2e63 7075 5f70 6f6c 6963 7920 6973 206e  .cpu_policy is n
-000e02b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e02c0: 2020 2020 2072 6573 756c 745b 2763 7075       result['cpu
-000e02d0: 5f70 6f6c 6963 7927 5d20 3d20 7365 6c66  _policy'] = self
-000e02e0: 2e63 7075 5f70 6f6c 6963 790a 2020 2020  .cpu_policy.    
-000e02f0: 2020 2020 6966 2073 656c 662e 696d 6167      if self.imag
-000e0300: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
-000e0310: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e0320: 7375 6c74 5b27 696d 6167 655f 6964 275d  sult['image_id']
-000e0330: 203d 2073 656c 662e 696d 6167 655f 6964   = self.image_id
-000e0340: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e0350: 2e6b 6579 5f70 6169 7220 6973 206e 6f74  .key_pair is not
-000e0360: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e0370: 2020 2072 6573 756c 745b 276b 6579 5f70     result['key_p
-000e0380: 6169 7227 5d20 3d20 7365 6c66 2e6b 6579  air'] = self.key
-000e0390: 5f70 6169 720a 2020 2020 2020 2020 6966  _pair.        if
-000e03a0: 2073 656c 662e 6c6f 6769 6e5f 7061 7373   self.login_pass
-000e03b0: 776f 7264 2069 7320 6e6f 7420 4e6f 6e65  word is not None
-000e03c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e03d0: 7375 6c74 5b27 6c6f 6769 6e5f 7061 7373  sult['login_pass
-000e03e0: 776f 7264 275d 203d 2073 656c 662e 6c6f  word'] = self.lo
-000e03f0: 6769 6e5f 7061 7373 776f 7264 0a20 2020  gin_password.   
-000e0400: 2020 2020 2069 6620 7365 6c66 2e72 6473       if self.rds
-000e0410: 5f69 6e73 7461 6e63 6573 2069 7320 6e6f  _instances is no
-000e0420: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e0430: 2020 2020 7265 7375 6c74 5b27 7264 735f      result['rds_
-000e0440: 696e 7374 616e 6365 7327 5d20 3d20 7365  instances'] = se
-000e0450: 6c66 2e72 6473 5f69 6e73 7461 6e63 6573  lf.rds_instances
-000e0460: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e0470: 2e72 756e 7469 6d65 2069 7320 6e6f 7420  .runtime is not 
-000e0480: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e0490: 2020 7265 7375 6c74 5b27 7275 6e74 696d    result['runtim
-000e04a0: 6527 5d20 3d20 7365 6c66 2e72 756e 7469  e'] = self.runti
-000e04b0: 6d65 2e74 6f5f 6d61 7028 290a 2020 2020  me.to_map().    
-000e04c0: 2020 2020 7265 7375 6c74 5b27 7461 6773      result['tags
-000e04d0: 275d 203d 205b 5d0a 2020 2020 2020 2020  '] = [].        
-000e04e0: 6966 2073 656c 662e 7461 6773 2069 7320  if self.tags is 
-000e04f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e0500: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
-000e0510: 656c 662e 7461 6773 3a0a 2020 2020 2020  elf.tags:.      
-000e0520: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e0530: 5b27 7461 6773 275d 2e61 7070 656e 6428  ['tags'].append(
-000e0540: 6b2e 746f 5f6d 6170 2829 2069 6620 6b20  k.to_map() if k 
-000e0550: 656c 7365 204e 6f6e 6529 0a20 2020 2020  else None).     
-000e0560: 2020 2072 6573 756c 745b 2774 6169 6e74     result['taint
-000e0570: 7327 5d20 3d20 5b5d 0a20 2020 2020 2020  s'] = [].       
-000e0580: 2069 6620 7365 6c66 2e74 6169 6e74 7320   if self.taints 
-000e0590: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e05a0: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-000e05b0: 6e20 7365 6c66 2e74 6169 6e74 733a 0a20  n self.taints:. 
-000e05c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000e05d0: 6573 756c 745b 2774 6169 6e74 7327 5d2e  esult['taints'].
-000e05e0: 6170 7065 6e64 286b 2e74 6f5f 6d61 7028  append(k.to_map(
-000e05f0: 2920 6966 206b 2065 6c73 6520 4e6f 6e65  ) if k else None
-000e0600: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000e0610: 662e 7573 6572 5f64 6174 6120 6973 206e  f.user_data is n
-000e0620: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e0630: 2020 2020 2072 6573 756c 745b 2775 7365       result['use
-000e0640: 725f 6461 7461 275d 203d 2073 656c 662e  r_data'] = self.
-000e0650: 7573 6572 5f64 6174 610a 2020 2020 2020  user_data.      
-000e0660: 2020 6966 2073 656c 662e 7673 7769 7463    if self.vswitc
-000e0670: 685f 6964 7320 6973 206e 6f74 204e 6f6e  h_ids is not Non
-000e0680: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e0690: 6573 756c 745b 2776 7377 6974 6368 5f69  esult['vswitch_i
-000e06a0: 6473 275d 203d 2073 656c 662e 7673 7769  ds'] = self.vswi
-000e06b0: 7463 685f 6964 730a 2020 2020 2020 2020  tch_ids.        
-000e06c0: 6966 2073 656c 662e 776f 726b 6572 5f61  if self.worker_a
-000e06d0: 7574 6f5f 7265 6e65 7720 6973 206e 6f74  uto_renew is not
-000e06e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e06f0: 2020 2072 6573 756c 745b 2777 6f72 6b65     result['worke
-000e0700: 725f 6175 746f 5f72 656e 6577 275d 203d  r_auto_renew'] =
-000e0710: 2073 656c 662e 776f 726b 6572 5f61 7574   self.worker_aut
-000e0720: 6f5f 7265 6e65 770a 2020 2020 2020 2020  o_renew.        
-000e0730: 6966 2073 656c 662e 776f 726b 6572 5f61  if self.worker_a
-000e0740: 7574 6f5f 7265 6e65 775f 7065 7269 6f64  uto_renew_period
-000e0750: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e0760: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e0770: 5b27 776f 726b 6572 5f61 7574 6f5f 7265  ['worker_auto_re
-000e0780: 6e65 775f 7065 7269 6f64 275d 203d 2073  new_period'] = s
-000e0790: 656c 662e 776f 726b 6572 5f61 7574 6f5f  elf.worker_auto_
-000e07a0: 7265 6e65 775f 7065 7269 6f64 0a20 2020  renew_period.   
-000e07b0: 2020 2020 2072 6573 756c 745b 2777 6f72       result['wor
-000e07c0: 6b65 725f 6461 7461 5f64 6973 6b73 275d  ker_data_disks']
-000e07d0: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-000e07e0: 2073 656c 662e 776f 726b 6572 5f64 6174   self.worker_dat
-000e07f0: 615f 6469 736b 7320 6973 206e 6f74 204e  a_disks is not N
-000e0800: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e0810: 2066 6f72 206b 2069 6e20 7365 6c66 2e77   for k in self.w
-000e0820: 6f72 6b65 725f 6461 7461 5f64 6973 6b73  orker_data_disks
-000e0830: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000e0840: 2020 7265 7375 6c74 5b27 776f 726b 6572    result['worker
-000e0850: 5f64 6174 615f 6469 736b 7327 5d2e 6170  _data_disks'].ap
-000e0860: 7065 6e64 286b 2e74 6f5f 6d61 7028 2920  pend(k.to_map() 
-000e0870: 6966 206b 2065 6c73 6520 4e6f 6e65 290a  if k else None).
-000e0880: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000e0890: 776f 726b 6572 5f69 6e73 7461 6e63 655f  worker_instance_
-000e08a0: 6368 6172 6765 5f74 7970 6520 6973 206e  charge_type is n
-000e08b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e08c0: 2020 2020 2072 6573 756c 745b 2777 6f72       result['wor
-000e08d0: 6b65 725f 696e 7374 616e 6365 5f63 6861  ker_instance_cha
-000e08e0: 7267 655f 7479 7065 275d 203d 2073 656c  rge_type'] = sel
-000e08f0: 662e 776f 726b 6572 5f69 6e73 7461 6e63  f.worker_instanc
-000e0900: 655f 6368 6172 6765 5f74 7970 650a 2020  e_charge_type.  
-000e0910: 2020 2020 2020 6966 2073 656c 662e 776f        if self.wo
-000e0920: 726b 6572 5f69 6e73 7461 6e63 655f 7479  rker_instance_ty
-000e0930: 7065 7320 6973 206e 6f74 204e 6f6e 653a  pes is not None:
-000e0940: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000e0950: 756c 745b 2777 6f72 6b65 725f 696e 7374  ult['worker_inst
-000e0960: 616e 6365 5f74 7970 6573 275d 203d 2073  ance_types'] = s
-000e0970: 656c 662e 776f 726b 6572 5f69 6e73 7461  elf.worker_insta
-000e0980: 6e63 655f 7479 7065 730a 2020 2020 2020  nce_types.      
-000e0990: 2020 6966 2073 656c 662e 776f 726b 6572    if self.worker
-000e09a0: 5f70 6572 696f 6420 6973 206e 6f74 204e  _period is not N
-000e09b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e09c0: 2072 6573 756c 745b 2777 6f72 6b65 725f   result['worker_
-000e09d0: 7065 7269 6f64 275d 203d 2073 656c 662e  period'] = self.
-000e09e0: 776f 726b 6572 5f70 6572 696f 640a 2020  worker_period.  
-000e09f0: 2020 2020 2020 6966 2073 656c 662e 776f        if self.wo
-000e0a00: 726b 6572 5f70 6572 696f 645f 756e 6974  rker_period_unit
-000e0a10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e0a20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e0a30: 5b27 776f 726b 6572 5f70 6572 696f 645f  ['worker_period_
-000e0a40: 756e 6974 275d 203d 2073 656c 662e 776f  unit'] = self.wo
-000e0a50: 726b 6572 5f70 6572 696f 645f 756e 6974  rker_period_unit
-000e0a60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e0a70: 2e77 6f72 6b65 725f 7379 7374 656d 5f64  .worker_system_d
-000e0a80: 6973 6b5f 6361 7465 676f 7279 2069 7320  isk_category is 
-000e0a90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e0aa0: 2020 2020 2020 7265 7375 6c74 5b27 776f        result['wo
-000e0ab0: 726b 6572 5f73 7973 7465 6d5f 6469 736b  rker_system_disk
-000e0ac0: 5f63 6174 6567 6f72 7927 5d20 3d20 7365  _category'] = se
-000e0ad0: 6c66 2e77 6f72 6b65 725f 7379 7374 656d  lf.worker_system
-000e0ae0: 5f64 6973 6b5f 6361 7465 676f 7279 0a20  _disk_category. 
-000e0af0: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-000e0b00: 6f72 6b65 725f 7379 7374 656d 5f64 6973  orker_system_dis
-000e0b10: 6b5f 7369 7a65 2069 7320 6e6f 7420 4e6f  k_size is not No
-000e0b20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e0b30: 7265 7375 6c74 5b27 776f 726b 6572 5f73  result['worker_s
-000e0b40: 7973 7465 6d5f 6469 736b 5f73 697a 6527  ystem_disk_size'
-000e0b50: 5d20 3d20 7365 6c66 2e77 6f72 6b65 725f  ] = self.worker_
-000e0b60: 7379 7374 656d 5f64 6973 6b5f 7369 7a65  system_disk_size
-000e0b70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000e0b80: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-000e0b90: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-000e0ba0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-000e0bb0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000e0bc0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000e0bd0: 6966 206d 2e67 6574 2827 636c 6f75 645f  if m.get('cloud_
-000e0be0: 6d6f 6e69 746f 725f 666c 6167 7327 2920  monitor_flags') 
-000e0bf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e0c00: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-000e0c10: 6f75 645f 6d6f 6e69 746f 725f 666c 6167  oud_monitor_flag
-000e0c20: 7320 3d20 6d2e 6765 7428 2763 6c6f 7564  s = m.get('cloud
-000e0c30: 5f6d 6f6e 6974 6f72 5f66 6c61 6773 2729  _monitor_flags')
-000e0c40: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000e0c50: 7428 2763 6f75 6e74 2729 2069 7320 6e6f  t('count') is no
-000e0c60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e0c70: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-000e0c80: 206d 2e67 6574 2827 636f 756e 7427 290a   m.get('count').
-000e0c90: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000e0ca0: 2827 6370 755f 706f 6c69 6379 2729 2069  ('cpu_policy') i
-000e0cb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e0cc0: 2020 2020 2020 2020 7365 6c66 2e63 7075          self.cpu
-000e0cd0: 5f70 6f6c 6963 7920 3d20 6d2e 6765 7428  _policy = m.get(
-000e0ce0: 2763 7075 5f70 6f6c 6963 7927 290a 2020  'cpu_policy').  
-000e0cf0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e0d00: 696d 6167 655f 6964 2729 2069 7320 6e6f  image_id') is no
-000e0d10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e0d20: 2020 2020 7365 6c66 2e69 6d61 6765 5f69      self.image_i
-000e0d30: 6420 3d20 6d2e 6765 7428 2769 6d61 6765  d = m.get('image
-000e0d40: 5f69 6427 290a 2020 2020 2020 2020 6966  _id').        if
-000e0d50: 206d 2e67 6574 2827 6b65 795f 7061 6972   m.get('key_pair
-000e0d60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000e0d70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e0d80: 2e6b 6579 5f70 6169 7220 3d20 6d2e 6765  .key_pair = m.ge
-000e0d90: 7428 276b 6579 5f70 6169 7227 290a 2020  t('key_pair').  
-000e0da0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e0db0: 6c6f 6769 6e5f 7061 7373 776f 7264 2729  login_password')
-000e0dc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e0dd0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-000e0de0: 6f67 696e 5f70 6173 7377 6f72 6420 3d20  ogin_password = 
-000e0df0: 6d2e 6765 7428 276c 6f67 696e 5f70 6173  m.get('login_pas
-000e0e00: 7377 6f72 6427 290a 2020 2020 2020 2020  sword').        
-000e0e10: 6966 206d 2e67 6574 2827 7264 735f 696e  if m.get('rds_in
-000e0e20: 7374 616e 6365 7327 2920 6973 206e 6f74  stances') is not
-000e0e30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e0e40: 2020 2073 656c 662e 7264 735f 696e 7374     self.rds_inst
-000e0e50: 616e 6365 7320 3d20 6d2e 6765 7428 2772  ances = m.get('r
-000e0e60: 6473 5f69 6e73 7461 6e63 6573 2729 0a20  ds_instances'). 
-000e0e70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000e0e80: 2772 756e 7469 6d65 2729 2069 7320 6e6f  'runtime') is no
-000e0e90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e0ea0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-000e0eb0: 2052 756e 7469 6d65 2829 0a20 2020 2020   Runtime().     
-000e0ec0: 2020 2020 2020 2073 656c 662e 7275 6e74         self.runt
-000e0ed0: 696d 6520 3d20 7465 6d70 5f6d 6f64 656c  ime = temp_model
-000e0ee0: 2e66 726f 6d5f 6d61 7028 6d5b 2772 756e  .from_map(m['run
-000e0ef0: 7469 6d65 275d 290a 2020 2020 2020 2020  time']).        
-000e0f00: 7365 6c66 2e74 6167 7320 3d20 5b5d 0a20  self.tags = []. 
-000e0f10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000e0f20: 2774 6167 7327 2920 6973 206e 6f74 204e  'tags') is not N
-000e0f30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e0f40: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
-000e0f50: 2774 6167 7327 293a 0a20 2020 2020 2020  'tags'):.       
-000e0f60: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000e0f70: 6465 6c20 3d20 5461 6728 290a 2020 2020  del = Tag().    
-000e0f80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e0f90: 2e74 6167 732e 6170 7065 6e64 2874 656d  .tags.append(tem
-000e0fa0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-000e0fb0: 286b 2929 0a20 2020 2020 2020 2073 656c  (k)).        sel
-000e0fc0: 662e 7461 696e 7473 203d 205b 5d0a 2020  f.taints = [].  
-000e0fd0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e0fe0: 7461 696e 7473 2729 2069 7320 6e6f 7420  taints') is not 
-000e0ff0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e1000: 2020 666f 7220 6b20 696e 206d 2e67 6574    for k in m.get
-000e1010: 2827 7461 696e 7473 2729 3a0a 2020 2020  ('taints'):.    
-000e1020: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000e1030: 5f6d 6f64 656c 203d 2054 6169 6e74 2829  _model = Taint()
-000e1040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000e1050: 2073 656c 662e 7461 696e 7473 2e61 7070   self.taints.app
-000e1060: 656e 6428 7465 6d70 5f6d 6f64 656c 2e66  end(temp_model.f
-000e1070: 726f 6d5f 6d61 7028 6b29 290a 2020 2020  rom_map(k)).    
-000e1080: 2020 2020 6966 206d 2e67 6574 2827 7573      if m.get('us
-000e1090: 6572 5f64 6174 6127 2920 6973 206e 6f74  er_data') is not
-000e10a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e10b0: 2020 2073 656c 662e 7573 6572 5f64 6174     self.user_dat
-000e10c0: 6120 3d20 6d2e 6765 7428 2775 7365 725f  a = m.get('user_
-000e10d0: 6461 7461 2729 0a20 2020 2020 2020 2069  data').        i
-000e10e0: 6620 6d2e 6765 7428 2776 7377 6974 6368  f m.get('vswitch
-000e10f0: 5f69 6473 2729 2069 7320 6e6f 7420 4e6f  _ids') is not No
-000e1100: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e1110: 7365 6c66 2e76 7377 6974 6368 5f69 6473  self.vswitch_ids
-000e1120: 203d 206d 2e67 6574 2827 7673 7769 7463   = m.get('vswitc
-000e1130: 685f 6964 7327 290a 2020 2020 2020 2020  h_ids').        
-000e1140: 6966 206d 2e67 6574 2827 776f 726b 6572  if m.get('worker
-000e1150: 5f61 7574 6f5f 7265 6e65 7727 2920 6973  _auto_renew') is
-000e1160: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e1170: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
-000e1180: 6572 5f61 7574 6f5f 7265 6e65 7720 3d20  er_auto_renew = 
-000e1190: 6d2e 6765 7428 2777 6f72 6b65 725f 6175  m.get('worker_au
-000e11a0: 746f 5f72 656e 6577 2729 0a20 2020 2020  to_renew').     
-000e11b0: 2020 2069 6620 6d2e 6765 7428 2777 6f72     if m.get('wor
-000e11c0: 6b65 725f 6175 746f 5f72 656e 6577 5f70  ker_auto_renew_p
-000e11d0: 6572 696f 6427 2920 6973 206e 6f74 204e  eriod') is not N
-000e11e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e11f0: 2073 656c 662e 776f 726b 6572 5f61 7574   self.worker_aut
-000e1200: 6f5f 7265 6e65 775f 7065 7269 6f64 203d  o_renew_period =
-000e1210: 206d 2e67 6574 2827 776f 726b 6572 5f61   m.get('worker_a
-000e1220: 7574 6f5f 7265 6e65 775f 7065 7269 6f64  uto_renew_period
-000e1230: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-000e1240: 776f 726b 6572 5f64 6174 615f 6469 736b  worker_data_disk
-000e1250: 7320 3d20 5b5d 0a20 2020 2020 2020 2069  s = [].        i
-000e1260: 6620 6d2e 6765 7428 2777 6f72 6b65 725f  f m.get('worker_
-000e1270: 6461 7461 5f64 6973 6b73 2729 2069 7320  data_disks') is 
-000e1280: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e1290: 2020 2020 2020 666f 7220 6b20 696e 206d        for k in m
-000e12a0: 2e67 6574 2827 776f 726b 6572 5f64 6174  .get('worker_dat
-000e12b0: 615f 6469 736b 7327 293a 0a20 2020 2020  a_disks'):.     
-000e12c0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-000e12d0: 6d6f 6465 6c20 3d20 5363 616c 654f 7574  model = ScaleOut
-000e12e0: 436c 7573 7465 7252 6571 7565 7374 576f  ClusterRequestWo
-000e12f0: 726b 6572 4461 7461 4469 736b 7328 290a  rkerDataDisks().
-000e1300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000e1310: 7365 6c66 2e77 6f72 6b65 725f 6461 7461  self.worker_data
-000e1320: 5f64 6973 6b73 2e61 7070 656e 6428 7465  _disks.append(te
-000e1330: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-000e1340: 7028 6b29 290a 2020 2020 2020 2020 6966  p(k)).        if
-000e1350: 206d 2e67 6574 2827 776f 726b 6572 5f69   m.get('worker_i
-000e1360: 6e73 7461 6e63 655f 6368 6172 6765 5f74  nstance_charge_t
-000e1370: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
-000e1380: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000e1390: 656c 662e 776f 726b 6572 5f69 6e73 7461  elf.worker_insta
-000e13a0: 6e63 655f 6368 6172 6765 5f74 7970 6520  nce_charge_type 
-000e13b0: 3d20 6d2e 6765 7428 2777 6f72 6b65 725f  = m.get('worker_
-000e13c0: 696e 7374 616e 6365 5f63 6861 7267 655f  instance_charge_
-000e13d0: 7479 7065 2729 0a20 2020 2020 2020 2069  type').        i
-000e13e0: 6620 6d2e 6765 7428 2777 6f72 6b65 725f  f m.get('worker_
-000e13f0: 696e 7374 616e 6365 5f74 7970 6573 2729  instance_types')
-000e1400: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e1410: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-000e1420: 6f72 6b65 725f 696e 7374 616e 6365 5f74  orker_instance_t
-000e1430: 7970 6573 203d 206d 2e67 6574 2827 776f  ypes = m.get('wo
-000e1440: 726b 6572 5f69 6e73 7461 6e63 655f 7479  rker_instance_ty
-000e1450: 7065 7327 290a 2020 2020 2020 2020 6966  pes').        if
-000e1460: 206d 2e67 6574 2827 776f 726b 6572 5f70   m.get('worker_p
-000e1470: 6572 696f 6427 2920 6973 206e 6f74 204e  eriod') is not N
-000e1480: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e1490: 2073 656c 662e 776f 726b 6572 5f70 6572   self.worker_per
-000e14a0: 696f 6420 3d20 6d2e 6765 7428 2777 6f72  iod = m.get('wor
-000e14b0: 6b65 725f 7065 7269 6f64 2729 0a20 2020  ker_period').   
-000e14c0: 2020 2020 2069 6620 6d2e 6765 7428 2777       if m.get('w
-000e14d0: 6f72 6b65 725f 7065 7269 6f64 5f75 6e69  orker_period_uni
-000e14e0: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
-000e14f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000e1500: 662e 776f 726b 6572 5f70 6572 696f 645f  f.worker_period_
-000e1510: 756e 6974 203d 206d 2e67 6574 2827 776f  unit = m.get('wo
-000e1520: 726b 6572 5f70 6572 696f 645f 756e 6974  rker_period_unit
-000e1530: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000e1540: 6765 7428 2777 6f72 6b65 725f 7379 7374  get('worker_syst
-000e1550: 656d 5f64 6973 6b5f 6361 7465 676f 7279  em_disk_category
-000e1560: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000e1570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e1580: 2e77 6f72 6b65 725f 7379 7374 656d 5f64  .worker_system_d
-000e1590: 6973 6b5f 6361 7465 676f 7279 203d 206d  isk_category = m
-000e15a0: 2e67 6574 2827 776f 726b 6572 5f73 7973  .get('worker_sys
-000e15b0: 7465 6d5f 6469 736b 5f63 6174 6567 6f72  tem_disk_categor
-000e15c0: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
-000e15d0: 2e67 6574 2827 776f 726b 6572 5f73 7973  .get('worker_sys
-000e15e0: 7465 6d5f 6469 736b 5f73 697a 6527 2920  tem_disk_size') 
-000e15f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e1600: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
-000e1610: 726b 6572 5f73 7973 7465 6d5f 6469 736b  rker_system_disk
-000e1620: 5f73 697a 6520 3d20 6d2e 6765 7428 2777  _size = m.get('w
-000e1630: 6f72 6b65 725f 7379 7374 656d 5f64 6973  orker_system_dis
-000e1640: 6b5f 7369 7a65 2729 0a20 2020 2020 2020  k_size').       
-000e1650: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000e1660: 6c61 7373 2053 6361 6c65 4f75 7443 6c75  lass ScaleOutClu
-000e1670: 7374 6572 5265 7370 6f6e 7365 426f 6479  sterResponseBody
-000e1680: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-000e1690: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-000e16a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000e16b0: 2020 2020 636c 7573 7465 725f 6964 3a20      cluster_id: 
-000e16c0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000e16d0: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-000e16e0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000e16f0: 2020 2020 7461 736b 5f69 643a 2073 7472      task_id: str
-000e1700: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000e1710: 2020 2020 2020 2020 2320 5468 6520 636c          # The cl
-000e1720: 7573 7465 7220 4944 2e0a 2020 2020 2020  uster ID..      
-000e1730: 2020 7365 6c66 2e63 6c75 7374 6572 5f69    self.cluster_i
-000e1740: 6420 3d20 636c 7573 7465 725f 6964 0a20  d = cluster_id. 
-000e1750: 2020 2020 2020 2023 2054 6865 2072 6571         # The req
-000e1760: 7565 7374 2049 442e 0a20 2020 2020 2020  uest ID..       
-000e1770: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-000e1780: 203d 2072 6571 7565 7374 5f69 640a 2020   = request_id.  
-000e1790: 2020 2020 2020 2320 5468 6520 7461 736b        # The task
-000e17a0: 2049 442e 0a20 2020 2020 2020 2073 656c   ID..        sel
-000e17b0: 662e 7461 736b 5f69 6420 3d20 7461 736b  f.task_id = task
-000e17c0: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-000e17d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000e17e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000e17f0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000e1800: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-000e1810: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-000e1820: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-000e1830: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e1840: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000e1850: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-000e1860: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-000e1870: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-000e1880: 6c75 7374 6572 5f69 6420 6973 206e 6f74  luster_id is not
-000e1890: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e18a0: 2020 2072 6573 756c 745b 2763 6c75 7374     result['clust
-000e18b0: 6572 5f69 6427 5d20 3d20 7365 6c66 2e63  er_id'] = self.c
-000e18c0: 6c75 7374 6572 5f69 640a 2020 2020 2020  luster_id.      
-000e18d0: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-000e18e0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-000e18f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e1900: 7375 6c74 5b27 7265 7175 6573 745f 6964  sult['request_id
-000e1910: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-000e1920: 745f 6964 0a20 2020 2020 2020 2069 6620  t_id.        if 
-000e1930: 7365 6c66 2e74 6173 6b5f 6964 2069 7320  self.task_id is 
-000e1940: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e1950: 2020 2020 2020 7265 7375 6c74 5b27 7461        result['ta
-000e1960: 736b 5f69 6427 5d20 3d20 7365 6c66 2e74  sk_id'] = self.t
-000e1970: 6173 6b5f 6964 0a20 2020 2020 2020 2072  ask_id.        r
-000e1980: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000e1990: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000e19a0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000e19b0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000e19c0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000e19d0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e19e0: 636c 7573 7465 725f 6964 2729 2069 7320  cluster_id') is 
-000e19f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e1a00: 2020 2020 2020 7365 6c66 2e63 6c75 7374        self.clust
-000e1a10: 6572 5f69 6420 3d20 6d2e 6765 7428 2763  er_id = m.get('c
-000e1a20: 6c75 7374 6572 5f69 6427 290a 2020 2020  luster_id').    
-000e1a30: 2020 2020 6966 206d 2e67 6574 2827 7265      if m.get('re
-000e1a40: 7175 6573 745f 6964 2729 2069 7320 6e6f  quest_id') is no
-000e1a50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e1a60: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-000e1a70: 5f69 6420 3d20 6d2e 6765 7428 2772 6571  _id = m.get('req
-000e1a80: 7565 7374 5f69 6427 290a 2020 2020 2020  uest_id').      
-000e1a90: 2020 6966 206d 2e67 6574 2827 7461 736b    if m.get('task
-000e1aa0: 5f69 6427 2920 6973 206e 6f74 204e 6f6e  _id') is not Non
-000e1ab0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000e1ac0: 656c 662e 7461 736b 5f69 6420 3d20 6d2e  elf.task_id = m.
-000e1ad0: 6765 7428 2774 6173 6b5f 6964 2729 0a20  get('task_id'). 
-000e1ae0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000e1af0: 6c66 0a0a 0a63 6c61 7373 2053 6361 6c65  lf...class Scale
-000e1b00: 4f75 7443 6c75 7374 6572 5265 7370 6f6e  OutClusterRespon
-000e1b10: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-000e1b20: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000e1b30: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000e1b40: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-000e1b50: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-000e1b60: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-000e1b70: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
-000e1b80: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
-000e1b90: 6f64 793a 2053 6361 6c65 4f75 7443 6c75  ody: ScaleOutClu
-000e1ba0: 7374 6572 5265 7370 6f6e 7365 426f 6479  sterResponseBody
-000e1bb0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000e1bc0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000e1bd0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-000e1be0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000e1bf0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-000e1c00: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-000e1c10: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-000e1c20: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000e1c30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e1c40: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-000e1c50: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000e1c60: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-000e1c70: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000e1c80: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000e1c90: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000e1ca0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000e1cb0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000e1cc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e1cd0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000e1ce0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000e1cf0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000e1d00: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-000e1d10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e1d20: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-000e1d30: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-000e1d40: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-000e1d50: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000e1d60: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000e1d70: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000e1d80: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-000e1d90: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-000e1da0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-000e1db0: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-000e1dc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e1dd0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-000e1de0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-000e1df0: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-000e1e00: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000e1e10: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000e1e20: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000e1e30: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000e1e40: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000e1e50: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-000e1e60: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+000da210: 2020 2020 2072 6573 756c 745b 2763 6865       result['che
+000da220: 636b 5f69 6427 5d20 3d20 7365 6c66 2e63  ck_id'] = self.c
+000da230: 6865 636b 5f69 640a 2020 2020 2020 2020  heck_id.        
+000da240: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+000da250: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000da260: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000da270: 6c74 5b27 7265 7175 6573 745f 6964 275d  lt['request_id']
+000da280: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+000da290: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+000da2a0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000da2b0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000da2c0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+000da2d0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000da2e0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+000da2f0: 2020 6966 206d 2e67 6574 2827 6368 6563    if m.get('chec
+000da300: 6b5f 6964 2729 2069 7320 6e6f 7420 4e6f  k_id') is not No
+000da310: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000da320: 7365 6c66 2e63 6865 636b 5f69 6420 3d20  self.check_id = 
+000da330: 6d2e 6765 7428 2763 6865 636b 5f69 6427  m.get('check_id'
+000da340: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000da350: 6574 2827 7265 7175 6573 745f 6964 2729  et('request_id')
+000da360: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000da370: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000da380: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+000da390: 7428 2772 6571 7565 7374 5f69 6427 290a  t('request_id').
+000da3a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000da3b0: 656c 660a 0a0a 636c 6173 7320 5275 6e43  elf...class RunC
+000da3c0: 6c75 7374 6572 4368 6563 6b52 6573 706f  lusterCheckRespo
+000da3d0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+000da3e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000da3f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000da400: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+000da410: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+000da420: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000da430: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
+000da440: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000da450: 626f 6479 3a20 5275 6e43 6c75 7374 6572  body: RunCluster
+000da460: 4368 6563 6b52 6573 706f 6e73 6542 6f64  CheckResponseBod
+000da470: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+000da480: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000da490: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+000da4a0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000da4b0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+000da4c0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+000da4d0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+000da4e0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000da4f0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000da500: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+000da510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000da520: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+000da530: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000da540: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000da550: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000da560: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000da570: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000da580: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000da590: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000da5a0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000da5b0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000da5c0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+000da5d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000da5e0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+000da5f0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+000da600: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+000da610: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+000da620: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+000da630: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000da640: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+000da650: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+000da660: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+000da670: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+000da680: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000da690: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+000da6a0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+000da6b0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+000da6c0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000da6d0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000da6e0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000da6f0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000da700: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000da710: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+000da720: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+000da730: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000da740: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+000da750: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+000da760: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000da770: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000da780: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000da790: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000da7a0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+000da7b0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000da7c0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000da7d0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+000da7e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000da7f0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+000da800: 5275 6e43 6c75 7374 6572 4368 6563 6b52  RunClusterCheckR
+000da810: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+000da820: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000da830: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+000da840: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+000da850: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+000da860: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+000da870: 2053 6361 6c65 436c 7573 7465 7252 6571   ScaleClusterReq
+000da880: 7565 7374 5461 6773 2854 6561 4d6f 6465  uestTags(TeaMode
+000da890: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000da8a0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000da8b0: 6c66 2c0a 2020 2020 2020 2020 6b65 793a  lf,.        key:
+000da8c0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000da8d0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+000da8e0: 2e6b 6579 203d 206b 6579 0a0a 2020 2020  .key = key..    
+000da8f0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+000da900: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+000da910: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000da920: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000da930: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+000da940: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000da950: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000da960: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000da970: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+000da980: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+000da990: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000da9a0: 2073 656c 662e 6b65 7920 6973 206e 6f74   self.key is not
+000da9b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000da9c0: 2020 2072 6573 756c 745b 276b 6579 275d     result['key']
+000da9d0: 203d 2073 656c 662e 6b65 790a 2020 2020   = self.key.    
+000da9e0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000da9f0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000daa00: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000daa10: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000daa20: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000daa30: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+000daa40: 6765 7428 276b 6579 2729 2069 7320 6e6f  get('key') is no
+000daa50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000daa60: 2020 2020 7365 6c66 2e6b 6579 203d 206d      self.key = m
+000daa70: 2e67 6574 2827 6b65 7927 290a 2020 2020  .get('key').    
+000daa80: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000daa90: 0a0a 636c 6173 7320 5363 616c 6543 6c75  ..class ScaleClu
+000daaa0: 7374 6572 5265 7175 6573 7454 6169 6e74  sterRequestTaint
+000daab0: 7328 5465 614d 6f64 656c 293a 0a20 2020  s(TeaModel):.   
+000daac0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000daad0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000daae0: 2020 2020 2065 6666 6563 743a 2073 7472       effect: str
+000daaf0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000dab00: 206b 6579 3a20 7374 7220 3d20 4e6f 6e65   key: str = None
+000dab10: 2c0a 2020 2020 2020 2020 7661 6c75 653a  ,.        value:
+000dab20: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000dab30: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+000dab40: 2e65 6666 6563 7420 3d20 6566 6665 6374  .effect = effect
+000dab50: 0a20 2020 2020 2020 2073 656c 662e 6b65  .        self.ke
+000dab60: 7920 3d20 6b65 790a 2020 2020 2020 2020  y = key.        
+000dab70: 7365 6c66 2e76 616c 7565 203d 2076 616c  self.value = val
+000dab80: 7565 0a0a 2020 2020 6465 6620 7661 6c69  ue..    def vali
+000dab90: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000daba0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000dabb0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000dabc0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000dabd0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000dabe0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000dabf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000dac00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000dac10: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000dac20: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000dac30: 2020 2020 2020 6966 2073 656c 662e 6566        if self.ef
+000dac40: 6665 6374 2069 7320 6e6f 7420 4e6f 6e65  fect is not None
+000dac50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000dac60: 7375 6c74 5b27 6566 6665 6374 275d 203d  sult['effect'] =
+000dac70: 2073 656c 662e 6566 6665 6374 0a20 2020   self.effect.   
+000dac80: 2020 2020 2069 6620 7365 6c66 2e6b 6579       if self.key
+000dac90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000daca0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000dacb0: 5b27 6b65 7927 5d20 3d20 7365 6c66 2e6b  ['key'] = self.k
+000dacc0: 6579 0a20 2020 2020 2020 2069 6620 7365  ey.        if se
+000dacd0: 6c66 2e76 616c 7565 2069 7320 6e6f 7420  lf.value is not 
+000dace0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000dacf0: 2020 7265 7375 6c74 5b27 7661 6c75 6527    result['value'
+000dad00: 5d20 3d20 7365 6c66 2e76 616c 7565 0a20  ] = self.value. 
+000dad10: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000dad20: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000dad30: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000dad40: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000dad50: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000dad60: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000dad70: 206d 2e67 6574 2827 6566 6665 6374 2729   m.get('effect')
+000dad80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000dad90: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+000dada0: 6666 6563 7420 3d20 6d2e 6765 7428 2765  ffect = m.get('e
+000dadb0: 6666 6563 7427 290a 2020 2020 2020 2020  ffect').        
+000dadc0: 6966 206d 2e67 6574 2827 6b65 7927 2920  if m.get('key') 
+000dadd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000dade0: 2020 2020 2020 2020 2073 656c 662e 6b65           self.ke
+000dadf0: 7920 3d20 6d2e 6765 7428 276b 6579 2729  y = m.get('key')
+000dae00: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000dae10: 7428 2776 616c 7565 2729 2069 7320 6e6f  t('value') is no
+000dae20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000dae30: 2020 2020 7365 6c66 2e76 616c 7565 203d      self.value =
+000dae40: 206d 2e67 6574 2827 7661 6c75 6527 290a   m.get('value').
+000dae50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000dae60: 656c 660a 0a0a 636c 6173 7320 5363 616c  elf...class Scal
+000dae70: 6543 6c75 7374 6572 5265 7175 6573 7457  eClusterRequestW
+000dae80: 6f72 6b65 7244 6174 6144 6973 6b73 2854  orkerDataDisks(T
+000dae90: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000daea0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000daeb0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000daec0: 2020 6361 7465 676f 7279 3a20 7374 7220    category: str 
+000daed0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000daee0: 656e 6372 7970 7465 643a 2073 7472 203d  encrypted: str =
+000daef0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000daf00: 697a 653a 2073 7472 203d 204e 6f6e 652c  ize: str = None,
+000daf10: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000daf20: 7365 6c66 2e63 6174 6567 6f72 7920 3d20  self.category = 
+000daf30: 6361 7465 676f 7279 0a20 2020 2020 2020  category.       
+000daf40: 2073 656c 662e 656e 6372 7970 7465 6420   self.encrypted 
+000daf50: 3d20 656e 6372 7970 7465 640a 2020 2020  = encrypted.    
+000daf60: 2020 2020 7365 6c66 2e73 697a 6520 3d20      self.size = 
+000daf70: 7369 7a65 0a0a 2020 2020 6465 6620 7661  size..    def va
+000daf80: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000daf90: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000dafa0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000dafb0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000dafc0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+000dafd0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000dafe0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000daff0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000db000: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000db010: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000db020: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000db030: 6361 7465 676f 7279 2069 7320 6e6f 7420  category is not 
+000db040: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000db050: 2020 7265 7375 6c74 5b27 6361 7465 676f    result['catego
+000db060: 7279 275d 203d 2073 656c 662e 6361 7465  ry'] = self.cate
+000db070: 676f 7279 0a20 2020 2020 2020 2069 6620  gory.        if 
+000db080: 7365 6c66 2e65 6e63 7279 7074 6564 2069  self.encrypted i
+000db090: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000db0a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000db0b0: 656e 6372 7970 7465 6427 5d20 3d20 7365  encrypted'] = se
+000db0c0: 6c66 2e65 6e63 7279 7074 6564 0a20 2020  lf.encrypted.   
+000db0d0: 2020 2020 2069 6620 7365 6c66 2e73 697a       if self.siz
+000db0e0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000db0f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000db100: 745b 2773 697a 6527 5d20 3d20 7365 6c66  t['size'] = self
+000db110: 2e73 697a 650a 2020 2020 2020 2020 7265  .size.        re
+000db120: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000db130: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000db140: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000db150: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000db160: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000db170: 2020 2020 2069 6620 6d2e 6765 7428 2763       if m.get('c
+000db180: 6174 6567 6f72 7927 2920 6973 206e 6f74  ategory') is not
+000db190: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000db1a0: 2020 2073 656c 662e 6361 7465 676f 7279     self.category
+000db1b0: 203d 206d 2e67 6574 2827 6361 7465 676f   = m.get('catego
+000db1c0: 7279 2729 0a20 2020 2020 2020 2069 6620  ry').        if 
+000db1d0: 6d2e 6765 7428 2765 6e63 7279 7074 6564  m.get('encrypted
+000db1e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000db1f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000db200: 2e65 6e63 7279 7074 6564 203d 206d 2e67  .encrypted = m.g
+000db210: 6574 2827 656e 6372 7970 7465 6427 290a  et('encrypted').
+000db220: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000db230: 2827 7369 7a65 2729 2069 7320 6e6f 7420  ('size') is not 
+000db240: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000db250: 2020 7365 6c66 2e73 697a 6520 3d20 6d2e    self.size = m.
+000db260: 6765 7428 2773 697a 6527 290a 2020 2020  get('size').    
+000db270: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000db280: 0a0a 636c 6173 7320 5363 616c 6543 6c75  ..class ScaleClu
+000db290: 7374 6572 5265 7175 6573 7428 5465 614d  sterRequest(TeaM
+000db2a0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+000db2b0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000db2c0: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
+000db2d0: 6c6f 7564 5f6d 6f6e 6974 6f72 5f66 6c61  loud_monitor_fla
+000db2e0: 6773 3a20 626f 6f6c 203d 204e 6f6e 652c  gs: bool = None,
+000db2f0: 0a20 2020 2020 2020 2063 6f75 6e74 3a20  .        count: 
+000db300: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+000db310: 2020 2020 6370 755f 706f 6c69 6379 3a20      cpu_policy: 
+000db320: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000db330: 2020 2020 6469 7361 626c 655f 726f 6c6c      disable_roll
+000db340: 6261 636b 3a20 626f 6f6c 203d 204e 6f6e  back: bool = Non
+000db350: 652c 0a20 2020 2020 2020 206b 6579 5f70  e,.        key_p
+000db360: 6169 723a 2073 7472 203d 204e 6f6e 652c  air: str = None,
+000db370: 0a20 2020 2020 2020 206c 6f67 696e 5f70  .        login_p
+000db380: 6173 7377 6f72 643a 2073 7472 203d 204e  assword: str = N
+000db390: 6f6e 652c 0a20 2020 2020 2020 2074 6167  one,.        tag
+000db3a0: 733a 204c 6973 745b 5363 616c 6543 6c75  s: List[ScaleClu
+000db3b0: 7374 6572 5265 7175 6573 7454 6167 735d  sterRequestTags]
+000db3c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000db3d0: 2074 6169 6e74 733a 204c 6973 745b 5363   taints: List[Sc
+000db3e0: 616c 6543 6c75 7374 6572 5265 7175 6573  aleClusterReques
+000db3f0: 7454 6169 6e74 735d 203d 204e 6f6e 652c  tTaints] = None,
+000db400: 0a20 2020 2020 2020 2076 7377 6974 6368  .        vswitch
+000db410: 5f69 6473 3a20 4c69 7374 5b73 7472 5d20  _ids: List[str] 
+000db420: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000db430: 776f 726b 6572 5f61 7574 6f5f 7265 6e65  worker_auto_rene
+000db440: 773a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  w: bool = None,.
+000db450: 2020 2020 2020 2020 776f 726b 6572 5f61          worker_a
+000db460: 7574 6f5f 7265 6e65 775f 7065 7269 6f64  uto_renew_period
+000db470: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+000db480: 2020 2020 2020 776f 726b 6572 5f64 6174        worker_dat
+000db490: 615f 6469 736b 3a20 626f 6f6c 203d 204e  a_disk: bool = N
+000db4a0: 6f6e 652c 0a20 2020 2020 2020 2077 6f72  one,.        wor
+000db4b0: 6b65 725f 6461 7461 5f64 6973 6b73 3a20  ker_data_disks: 
+000db4c0: 4c69 7374 5b53 6361 6c65 436c 7573 7465  List[ScaleCluste
+000db4d0: 7252 6571 7565 7374 576f 726b 6572 4461  rRequestWorkerDa
+000db4e0: 7461 4469 736b 735d 203d 204e 6f6e 652c  taDisks] = None,
+000db4f0: 0a20 2020 2020 2020 2077 6f72 6b65 725f  .        worker_
+000db500: 696e 7374 616e 6365 5f63 6861 7267 655f  instance_charge_
+000db510: 7479 7065 3a20 7374 7220 3d20 4e6f 6e65  type: str = None
+000db520: 2c0a 2020 2020 2020 2020 776f 726b 6572  ,.        worker
+000db530: 5f69 6e73 7461 6e63 655f 7479 7065 733a  _instance_types:
+000db540: 204c 6973 745b 7374 725d 203d 204e 6f6e   List[str] = Non
+000db550: 652c 0a20 2020 2020 2020 2077 6f72 6b65  e,.        worke
+000db560: 725f 7065 7269 6f64 3a20 696e 7420 3d20  r_period: int = 
+000db570: 4e6f 6e65 2c0a 2020 2020 2020 2020 776f  None,.        wo
+000db580: 726b 6572 5f70 6572 696f 645f 756e 6974  rker_period_unit
+000db590: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000db5a0: 2020 2020 2020 776f 726b 6572 5f73 7973        worker_sys
+000db5b0: 7465 6d5f 6469 736b 5f63 6174 6567 6f72  tem_disk_categor
+000db5c0: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
+000db5d0: 2020 2020 2020 2077 6f72 6b65 725f 7379         worker_sy
+000db5e0: 7374 656d 5f64 6973 6b5f 7369 7a65 3a20  stem_disk_size: 
+000db5f0: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+000db600: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000db610: 636c 6f75 645f 6d6f 6e69 746f 725f 666c  cloud_monitor_fl
+000db620: 6167 7320 3d20 636c 6f75 645f 6d6f 6e69  ags = cloud_moni
+000db630: 746f 725f 666c 6167 730a 2020 2020 2020  tor_flags.      
+000db640: 2020 7365 6c66 2e63 6f75 6e74 203d 2063    self.count = c
+000db650: 6f75 6e74 0a20 2020 2020 2020 2073 656c  ount.        sel
+000db660: 662e 6370 755f 706f 6c69 6379 203d 2063  f.cpu_policy = c
+000db670: 7075 5f70 6f6c 6963 790a 2020 2020 2020  pu_policy.      
+000db680: 2020 7365 6c66 2e64 6973 6162 6c65 5f72    self.disable_r
+000db690: 6f6c 6c62 6163 6b20 3d20 6469 7361 626c  ollback = disabl
+000db6a0: 655f 726f 6c6c 6261 636b 0a20 2020 2020  e_rollback.     
+000db6b0: 2020 2073 656c 662e 6b65 795f 7061 6972     self.key_pair
+000db6c0: 203d 206b 6579 5f70 6169 720a 2020 2020   = key_pair.    
+000db6d0: 2020 2020 7365 6c66 2e6c 6f67 696e 5f70      self.login_p
+000db6e0: 6173 7377 6f72 6420 3d20 6c6f 6769 6e5f  assword = login_
+000db6f0: 7061 7373 776f 7264 0a20 2020 2020 2020  password.       
+000db700: 2073 656c 662e 7461 6773 203d 2074 6167   self.tags = tag
+000db710: 730a 2020 2020 2020 2020 7365 6c66 2e74  s.        self.t
+000db720: 6169 6e74 7320 3d20 7461 696e 7473 0a20  aints = taints. 
+000db730: 2020 2020 2020 2073 656c 662e 7673 7769         self.vswi
+000db740: 7463 685f 6964 7320 3d20 7673 7769 7463  tch_ids = vswitc
+000db750: 685f 6964 730a 2020 2020 2020 2020 7365  h_ids.        se
+000db760: 6c66 2e77 6f72 6b65 725f 6175 746f 5f72  lf.worker_auto_r
+000db770: 656e 6577 203d 2077 6f72 6b65 725f 6175  enew = worker_au
+000db780: 746f 5f72 656e 6577 0a20 2020 2020 2020  to_renew.       
+000db790: 2073 656c 662e 776f 726b 6572 5f61 7574   self.worker_aut
+000db7a0: 6f5f 7265 6e65 775f 7065 7269 6f64 203d  o_renew_period =
+000db7b0: 2077 6f72 6b65 725f 6175 746f 5f72 656e   worker_auto_ren
+000db7c0: 6577 5f70 6572 696f 640a 2020 2020 2020  ew_period.      
+000db7d0: 2020 7365 6c66 2e77 6f72 6b65 725f 6461    self.worker_da
+000db7e0: 7461 5f64 6973 6b20 3d20 776f 726b 6572  ta_disk = worker
+000db7f0: 5f64 6174 615f 6469 736b 0a20 2020 2020  _data_disk.     
+000db800: 2020 2073 656c 662e 776f 726b 6572 5f64     self.worker_d
+000db810: 6174 615f 6469 736b 7320 3d20 776f 726b  ata_disks = work
+000db820: 6572 5f64 6174 615f 6469 736b 730a 2020  er_data_disks.  
+000db830: 2020 2020 2020 7365 6c66 2e77 6f72 6b65        self.worke
+000db840: 725f 696e 7374 616e 6365 5f63 6861 7267  r_instance_charg
+000db850: 655f 7479 7065 203d 2077 6f72 6b65 725f  e_type = worker_
+000db860: 696e 7374 616e 6365 5f63 6861 7267 655f  instance_charge_
+000db870: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
+000db880: 662e 776f 726b 6572 5f69 6e73 7461 6e63  f.worker_instanc
+000db890: 655f 7479 7065 7320 3d20 776f 726b 6572  e_types = worker
+000db8a0: 5f69 6e73 7461 6e63 655f 7479 7065 730a  _instance_types.
+000db8b0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+000db8c0: 6b65 725f 7065 7269 6f64 203d 2077 6f72  ker_period = wor
+000db8d0: 6b65 725f 7065 7269 6f64 0a20 2020 2020  ker_period.     
+000db8e0: 2020 2073 656c 662e 776f 726b 6572 5f70     self.worker_p
+000db8f0: 6572 696f 645f 756e 6974 203d 2077 6f72  eriod_unit = wor
+000db900: 6b65 725f 7065 7269 6f64 5f75 6e69 740a  ker_period_unit.
+000db910: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+000db920: 6b65 725f 7379 7374 656d 5f64 6973 6b5f  ker_system_disk_
+000db930: 6361 7465 676f 7279 203d 2077 6f72 6b65  category = worke
+000db940: 725f 7379 7374 656d 5f64 6973 6b5f 6361  r_system_disk_ca
+000db950: 7465 676f 7279 0a20 2020 2020 2020 2073  tegory.        s
+000db960: 656c 662e 776f 726b 6572 5f73 7973 7465  elf.worker_syste
+000db970: 6d5f 6469 736b 5f73 697a 6520 3d20 776f  m_disk_size = wo
+000db980: 726b 6572 5f73 7973 7465 6d5f 6469 736b  rker_system_disk
+000db990: 5f73 697a 650a 0a20 2020 2064 6566 2076  _size..    def v
+000db9a0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000db9b0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+000db9c0: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
+000db9d0: 2066 6f72 206b 2069 6e20 7365 6c66 2e74   for k in self.t
+000db9e0: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
+000db9f0: 2020 2020 2069 6620 6b3a 0a20 2020 2020       if k:.     
+000dba00: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+000dba10: 2e76 616c 6964 6174 6528 290a 2020 2020  .validate().    
+000dba20: 2020 2020 6966 2073 656c 662e 7461 696e      if self.tain
+000dba30: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+000dba40: 666f 7220 6b20 696e 2073 656c 662e 7461  for k in self.ta
+000dba50: 696e 7473 3a0a 2020 2020 2020 2020 2020  ints:.          
+000dba60: 2020 2020 2020 6966 206b 3a0a 2020 2020        if k:.    
+000dba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000dba80: 6b2e 7661 6c69 6461 7465 2829 0a20 2020  k.validate().   
+000dba90: 2020 2020 2069 6620 7365 6c66 2e77 6f72       if self.wor
+000dbaa0: 6b65 725f 6461 7461 5f64 6973 6b73 3a0a  ker_data_disks:.
+000dbab0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000dbac0: 6b20 696e 2073 656c 662e 776f 726b 6572  k in self.worker
+000dbad0: 5f64 6174 615f 6469 736b 733a 0a20 2020  _data_disks:.   
+000dbae0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000dbaf0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+000dbb00: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
+000dbb10: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+000dbb20: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+000dbb30: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000dbb40: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+000dbb50: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+000dbb60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000dbb70: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000dbb80: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000dbb90: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000dbba0: 2069 6620 7365 6c66 2e63 6c6f 7564 5f6d   if self.cloud_m
+000dbbb0: 6f6e 6974 6f72 5f66 6c61 6773 2069 7320  onitor_flags is 
+000dbbc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000dbbd0: 2020 2020 2020 7265 7375 6c74 5b27 636c        result['cl
+000dbbe0: 6f75 645f 6d6f 6e69 746f 725f 666c 6167  oud_monitor_flag
+000dbbf0: 7327 5d20 3d20 7365 6c66 2e63 6c6f 7564  s'] = self.cloud
+000dbc00: 5f6d 6f6e 6974 6f72 5f66 6c61 6773 0a20  _monitor_flags. 
+000dbc10: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000dbc20: 6f75 6e74 2069 7320 6e6f 7420 4e6f 6e65  ount is not None
+000dbc30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000dbc40: 7375 6c74 5b27 636f 756e 7427 5d20 3d20  sult['count'] = 
+000dbc50: 7365 6c66 2e63 6f75 6e74 0a20 2020 2020  self.count.     
+000dbc60: 2020 2069 6620 7365 6c66 2e63 7075 5f70     if self.cpu_p
+000dbc70: 6f6c 6963 7920 6973 206e 6f74 204e 6f6e  olicy is not Non
+000dbc80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000dbc90: 6573 756c 745b 2763 7075 5f70 6f6c 6963  esult['cpu_polic
+000dbca0: 7927 5d20 3d20 7365 6c66 2e63 7075 5f70  y'] = self.cpu_p
+000dbcb0: 6f6c 6963 790a 2020 2020 2020 2020 6966  olicy.        if
+000dbcc0: 2073 656c 662e 6469 7361 626c 655f 726f   self.disable_ro
+000dbcd0: 6c6c 6261 636b 2069 7320 6e6f 7420 4e6f  llback is not No
+000dbce0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000dbcf0: 7265 7375 6c74 5b27 6469 7361 626c 655f  result['disable_
+000dbd00: 726f 6c6c 6261 636b 275d 203d 2073 656c  rollback'] = sel
+000dbd10: 662e 6469 7361 626c 655f 726f 6c6c 6261  f.disable_rollba
+000dbd20: 636b 0a20 2020 2020 2020 2069 6620 7365  ck.        if se
+000dbd30: 6c66 2e6b 6579 5f70 6169 7220 6973 206e  lf.key_pair is n
+000dbd40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000dbd50: 2020 2020 2072 6573 756c 745b 276b 6579       result['key
+000dbd60: 5f70 6169 7227 5d20 3d20 7365 6c66 2e6b  _pair'] = self.k
+000dbd70: 6579 5f70 6169 720a 2020 2020 2020 2020  ey_pair.        
+000dbd80: 6966 2073 656c 662e 6c6f 6769 6e5f 7061  if self.login_pa
+000dbd90: 7373 776f 7264 2069 7320 6e6f 7420 4e6f  ssword is not No
+000dbda0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000dbdb0: 7265 7375 6c74 5b27 6c6f 6769 6e5f 7061  result['login_pa
+000dbdc0: 7373 776f 7264 275d 203d 2073 656c 662e  ssword'] = self.
+000dbdd0: 6c6f 6769 6e5f 7061 7373 776f 7264 0a20  login_password. 
+000dbde0: 2020 2020 2020 2072 6573 756c 745b 2774         result['t
+000dbdf0: 6167 7327 5d20 3d20 5b5d 0a20 2020 2020  ags'] = [].     
+000dbe00: 2020 2069 6620 7365 6c66 2e74 6167 7320     if self.tags 
+000dbe10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000dbe20: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+000dbe30: 6e20 7365 6c66 2e74 6167 733a 0a20 2020  n self.tags:.   
+000dbe40: 2020 2020 2020 2020 2020 2020 2072 6573               res
+000dbe50: 756c 745b 2774 6167 7327 5d2e 6170 7065  ult['tags'].appe
+000dbe60: 6e64 286b 2e74 6f5f 6d61 7028 2920 6966  nd(k.to_map() if
+000dbe70: 206b 2065 6c73 6520 4e6f 6e65 290a 2020   k else None).  
+000dbe80: 2020 2020 2020 7265 7375 6c74 5b27 7461        result['ta
+000dbe90: 696e 7473 275d 203d 205b 5d0a 2020 2020  ints'] = [].    
+000dbea0: 2020 2020 6966 2073 656c 662e 7461 696e      if self.tain
+000dbeb0: 7473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ts is not None:.
+000dbec0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000dbed0: 6b20 696e 2073 656c 662e 7461 696e 7473  k in self.taints
+000dbee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000dbef0: 2020 7265 7375 6c74 5b27 7461 696e 7473    result['taints
+000dbf00: 275d 2e61 7070 656e 6428 6b2e 746f 5f6d  '].append(k.to_m
+000dbf10: 6170 2829 2069 6620 6b20 656c 7365 204e  ap() if k else N
+000dbf20: 6f6e 6529 0a20 2020 2020 2020 2069 6620  one).        if 
+000dbf30: 7365 6c66 2e76 7377 6974 6368 5f69 6473  self.vswitch_ids
+000dbf40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000dbf50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000dbf60: 5b27 7673 7769 7463 685f 6964 7327 5d20  ['vswitch_ids'] 
+000dbf70: 3d20 7365 6c66 2e76 7377 6974 6368 5f69  = self.vswitch_i
+000dbf80: 6473 0a20 2020 2020 2020 2069 6620 7365  ds.        if se
+000dbf90: 6c66 2e77 6f72 6b65 725f 6175 746f 5f72  lf.worker_auto_r
+000dbfa0: 656e 6577 2069 7320 6e6f 7420 4e6f 6e65  enew is not None
+000dbfb0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000dbfc0: 7375 6c74 5b27 776f 726b 6572 5f61 7574  sult['worker_aut
+000dbfd0: 6f5f 7265 6e65 7727 5d20 3d20 7365 6c66  o_renew'] = self
+000dbfe0: 2e77 6f72 6b65 725f 6175 746f 5f72 656e  .worker_auto_ren
+000dbff0: 6577 0a20 2020 2020 2020 2069 6620 7365  ew.        if se
+000dc000: 6c66 2e77 6f72 6b65 725f 6175 746f 5f72  lf.worker_auto_r
+000dc010: 656e 6577 5f70 6572 696f 6420 6973 206e  enew_period is n
+000dc020: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000dc030: 2020 2020 2072 6573 756c 745b 2777 6f72       result['wor
+000dc040: 6b65 725f 6175 746f 5f72 656e 6577 5f70  ker_auto_renew_p
+000dc050: 6572 696f 6427 5d20 3d20 7365 6c66 2e77  eriod'] = self.w
+000dc060: 6f72 6b65 725f 6175 746f 5f72 656e 6577  orker_auto_renew
+000dc070: 5f70 6572 696f 640a 2020 2020 2020 2020  _period.        
+000dc080: 6966 2073 656c 662e 776f 726b 6572 5f64  if self.worker_d
+000dc090: 6174 615f 6469 736b 2069 7320 6e6f 7420  ata_disk is not 
+000dc0a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000dc0b0: 2020 7265 7375 6c74 5b27 776f 726b 6572    result['worker
+000dc0c0: 5f64 6174 615f 6469 736b 275d 203d 2073  _data_disk'] = s
+000dc0d0: 656c 662e 776f 726b 6572 5f64 6174 615f  elf.worker_data_
+000dc0e0: 6469 736b 0a20 2020 2020 2020 2072 6573  disk.        res
+000dc0f0: 756c 745b 2777 6f72 6b65 725f 6461 7461  ult['worker_data
+000dc100: 5f64 6973 6b73 275d 203d 205b 5d0a 2020  _disks'] = [].  
+000dc110: 2020 2020 2020 6966 2073 656c 662e 776f        if self.wo
+000dc120: 726b 6572 5f64 6174 615f 6469 736b 7320  rker_data_disks 
+000dc130: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000dc140: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+000dc150: 6e20 7365 6c66 2e77 6f72 6b65 725f 6461  n self.worker_da
+000dc160: 7461 5f64 6973 6b73 3a0a 2020 2020 2020  ta_disks:.      
+000dc170: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000dc180: 5b27 776f 726b 6572 5f64 6174 615f 6469  ['worker_data_di
+000dc190: 736b 7327 5d2e 6170 7065 6e64 286b 2e74  sks'].append(k.t
+000dc1a0: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
+000dc1b0: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
+000dc1c0: 6966 2073 656c 662e 776f 726b 6572 5f69  if self.worker_i
+000dc1d0: 6e73 7461 6e63 655f 6368 6172 6765 5f74  nstance_charge_t
+000dc1e0: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
+000dc1f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000dc200: 756c 745b 2777 6f72 6b65 725f 696e 7374  ult['worker_inst
+000dc210: 616e 6365 5f63 6861 7267 655f 7479 7065  ance_charge_type
+000dc220: 275d 203d 2073 656c 662e 776f 726b 6572  '] = self.worker
+000dc230: 5f69 6e73 7461 6e63 655f 6368 6172 6765  _instance_charge
+000dc240: 5f74 7970 650a 2020 2020 2020 2020 6966  _type.        if
+000dc250: 2073 656c 662e 776f 726b 6572 5f69 6e73   self.worker_ins
+000dc260: 7461 6e63 655f 7479 7065 7320 6973 206e  tance_types is n
+000dc270: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000dc280: 2020 2020 2072 6573 756c 745b 2777 6f72       result['wor
+000dc290: 6b65 725f 696e 7374 616e 6365 5f74 7970  ker_instance_typ
+000dc2a0: 6573 275d 203d 2073 656c 662e 776f 726b  es'] = self.work
+000dc2b0: 6572 5f69 6e73 7461 6e63 655f 7479 7065  er_instance_type
+000dc2c0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+000dc2d0: 662e 776f 726b 6572 5f70 6572 696f 6420  f.worker_period 
+000dc2e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000dc2f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000dc300: 2777 6f72 6b65 725f 7065 7269 6f64 275d  'worker_period']
+000dc310: 203d 2073 656c 662e 776f 726b 6572 5f70   = self.worker_p
+000dc320: 6572 696f 640a 2020 2020 2020 2020 6966  eriod.        if
+000dc330: 2073 656c 662e 776f 726b 6572 5f70 6572   self.worker_per
+000dc340: 696f 645f 756e 6974 2069 7320 6e6f 7420  iod_unit is not 
+000dc350: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000dc360: 2020 7265 7375 6c74 5b27 776f 726b 6572    result['worker
+000dc370: 5f70 6572 696f 645f 756e 6974 275d 203d  _period_unit'] =
+000dc380: 2073 656c 662e 776f 726b 6572 5f70 6572   self.worker_per
+000dc390: 696f 645f 756e 6974 0a20 2020 2020 2020  iod_unit.       
+000dc3a0: 2069 6620 7365 6c66 2e77 6f72 6b65 725f   if self.worker_
+000dc3b0: 7379 7374 656d 5f64 6973 6b5f 6361 7465  system_disk_cate
+000dc3c0: 676f 7279 2069 7320 6e6f 7420 4e6f 6e65  gory is not None
+000dc3d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000dc3e0: 7375 6c74 5b27 776f 726b 6572 5f73 7973  sult['worker_sys
+000dc3f0: 7465 6d5f 6469 736b 5f63 6174 6567 6f72  tem_disk_categor
+000dc400: 7927 5d20 3d20 7365 6c66 2e77 6f72 6b65  y'] = self.worke
+000dc410: 725f 7379 7374 656d 5f64 6973 6b5f 6361  r_system_disk_ca
+000dc420: 7465 676f 7279 0a20 2020 2020 2020 2069  tegory.        i
+000dc430: 6620 7365 6c66 2e77 6f72 6b65 725f 7379  f self.worker_sy
+000dc440: 7374 656d 5f64 6973 6b5f 7369 7a65 2069  stem_disk_size i
+000dc450: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000dc460: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000dc470: 776f 726b 6572 5f73 7973 7465 6d5f 6469  worker_system_di
+000dc480: 736b 5f73 697a 6527 5d20 3d20 7365 6c66  sk_size'] = self
+000dc490: 2e77 6f72 6b65 725f 7379 7374 656d 5f64  .worker_system_d
+000dc4a0: 6973 6b5f 7369 7a65 0a20 2020 2020 2020  isk_size.       
+000dc4b0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000dc4c0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000dc4d0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+000dc4e0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+000dc4f0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+000dc500: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000dc510: 2827 636c 6f75 645f 6d6f 6e69 746f 725f  ('cloud_monitor_
+000dc520: 666c 6167 7327 2920 6973 206e 6f74 204e  flags') is not N
+000dc530: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000dc540: 2073 656c 662e 636c 6f75 645f 6d6f 6e69   self.cloud_moni
+000dc550: 746f 725f 666c 6167 7320 3d20 6d2e 6765  tor_flags = m.ge
+000dc560: 7428 2763 6c6f 7564 5f6d 6f6e 6974 6f72  t('cloud_monitor
+000dc570: 5f66 6c61 6773 2729 0a20 2020 2020 2020  _flags').       
+000dc580: 2069 6620 6d2e 6765 7428 2763 6f75 6e74   if m.get('count
+000dc590: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000dc5a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000dc5b0: 2e63 6f75 6e74 203d 206d 2e67 6574 2827  .count = m.get('
+000dc5c0: 636f 756e 7427 290a 2020 2020 2020 2020  count').        
+000dc5d0: 6966 206d 2e67 6574 2827 6370 755f 706f  if m.get('cpu_po
+000dc5e0: 6c69 6379 2729 2069 7320 6e6f 7420 4e6f  licy') is not No
+000dc5f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000dc600: 7365 6c66 2e63 7075 5f70 6f6c 6963 7920  self.cpu_policy 
+000dc610: 3d20 6d2e 6765 7428 2763 7075 5f70 6f6c  = m.get('cpu_pol
+000dc620: 6963 7927 290a 2020 2020 2020 2020 6966  icy').        if
+000dc630: 206d 2e67 6574 2827 6469 7361 626c 655f   m.get('disable_
+000dc640: 726f 6c6c 6261 636b 2729 2069 7320 6e6f  rollback') is no
+000dc650: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000dc660: 2020 2020 7365 6c66 2e64 6973 6162 6c65      self.disable
+000dc670: 5f72 6f6c 6c62 6163 6b20 3d20 6d2e 6765  _rollback = m.ge
+000dc680: 7428 2764 6973 6162 6c65 5f72 6f6c 6c62  t('disable_rollb
+000dc690: 6163 6b27 290a 2020 2020 2020 2020 6966  ack').        if
+000dc6a0: 206d 2e67 6574 2827 6b65 795f 7061 6972   m.get('key_pair
+000dc6b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000dc6c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000dc6d0: 2e6b 6579 5f70 6169 7220 3d20 6d2e 6765  .key_pair = m.ge
+000dc6e0: 7428 276b 6579 5f70 6169 7227 290a 2020  t('key_pair').  
+000dc6f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000dc700: 6c6f 6769 6e5f 7061 7373 776f 7264 2729  login_password')
+000dc710: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000dc720: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+000dc730: 6f67 696e 5f70 6173 7377 6f72 6420 3d20  ogin_password = 
+000dc740: 6d2e 6765 7428 276c 6f67 696e 5f70 6173  m.get('login_pas
+000dc750: 7377 6f72 6427 290a 2020 2020 2020 2020  sword').        
+000dc760: 7365 6c66 2e74 6167 7320 3d20 5b5d 0a20  self.tags = []. 
+000dc770: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000dc780: 2774 6167 7327 2920 6973 206e 6f74 204e  'tags') is not N
+000dc790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000dc7a0: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
+000dc7b0: 2774 6167 7327 293a 0a20 2020 2020 2020  'tags'):.       
+000dc7c0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+000dc7d0: 6465 6c20 3d20 5363 616c 6543 6c75 7374  del = ScaleClust
+000dc7e0: 6572 5265 7175 6573 7454 6167 7328 290a  erRequestTags().
+000dc7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000dc800: 7365 6c66 2e74 6167 732e 6170 7065 6e64  self.tags.append
+000dc810: 2874 656d 705f 6d6f 6465 6c2e 6672 6f6d  (temp_model.from
+000dc820: 5f6d 6170 286b 2929 0a20 2020 2020 2020  _map(k)).       
+000dc830: 2073 656c 662e 7461 696e 7473 203d 205b   self.taints = [
+000dc840: 5d0a 2020 2020 2020 2020 6966 206d 2e67  ].        if m.g
+000dc850: 6574 2827 7461 696e 7473 2729 2069 7320  et('taints') is 
+000dc860: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000dc870: 2020 2020 2020 666f 7220 6b20 696e 206d        for k in m
+000dc880: 2e67 6574 2827 7461 696e 7473 2729 3a0a  .get('taints'):.
+000dc890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000dc8a0: 7465 6d70 5f6d 6f64 656c 203d 2053 6361  temp_model = Sca
+000dc8b0: 6c65 436c 7573 7465 7252 6571 7565 7374  leClusterRequest
+000dc8c0: 5461 696e 7473 2829 0a20 2020 2020 2020  Taints().       
+000dc8d0: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
+000dc8e0: 696e 7473 2e61 7070 656e 6428 7465 6d70  ints.append(temp
+000dc8f0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+000dc900: 6b29 290a 2020 2020 2020 2020 6966 206d  k)).        if m
+000dc910: 2e67 6574 2827 7673 7769 7463 685f 6964  .get('vswitch_id
+000dc920: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+000dc930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000dc940: 662e 7673 7769 7463 685f 6964 7320 3d20  f.vswitch_ids = 
+000dc950: 6d2e 6765 7428 2776 7377 6974 6368 5f69  m.get('vswitch_i
+000dc960: 6473 2729 0a20 2020 2020 2020 2069 6620  ds').        if 
+000dc970: 6d2e 6765 7428 2777 6f72 6b65 725f 6175  m.get('worker_au
+000dc980: 746f 5f72 656e 6577 2729 2069 7320 6e6f  to_renew') is no
+000dc990: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000dc9a0: 2020 2020 7365 6c66 2e77 6f72 6b65 725f      self.worker_
+000dc9b0: 6175 746f 5f72 656e 6577 203d 206d 2e67  auto_renew = m.g
+000dc9c0: 6574 2827 776f 726b 6572 5f61 7574 6f5f  et('worker_auto_
+000dc9d0: 7265 6e65 7727 290a 2020 2020 2020 2020  renew').        
+000dc9e0: 6966 206d 2e67 6574 2827 776f 726b 6572  if m.get('worker
+000dc9f0: 5f61 7574 6f5f 7265 6e65 775f 7065 7269  _auto_renew_peri
+000dca00: 6f64 2729 2069 7320 6e6f 7420 4e6f 6e65  od') is not None
+000dca10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000dca20: 6c66 2e77 6f72 6b65 725f 6175 746f 5f72  lf.worker_auto_r
+000dca30: 656e 6577 5f70 6572 696f 6420 3d20 6d2e  enew_period = m.
+000dca40: 6765 7428 2777 6f72 6b65 725f 6175 746f  get('worker_auto
+000dca50: 5f72 656e 6577 5f70 6572 696f 6427 290a  _renew_period').
+000dca60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000dca70: 2827 776f 726b 6572 5f64 6174 615f 6469  ('worker_data_di
+000dca80: 736b 2729 2069 7320 6e6f 7420 4e6f 6e65  sk') is not None
+000dca90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000dcaa0: 6c66 2e77 6f72 6b65 725f 6461 7461 5f64  lf.worker_data_d
+000dcab0: 6973 6b20 3d20 6d2e 6765 7428 2777 6f72  isk = m.get('wor
+000dcac0: 6b65 725f 6461 7461 5f64 6973 6b27 290a  ker_data_disk').
+000dcad0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+000dcae0: 6b65 725f 6461 7461 5f64 6973 6b73 203d  ker_data_disks =
+000dcaf0: 205b 5d0a 2020 2020 2020 2020 6966 206d   [].        if m
+000dcb00: 2e67 6574 2827 776f 726b 6572 5f64 6174  .get('worker_dat
+000dcb10: 615f 6469 736b 7327 2920 6973 206e 6f74  a_disks') is not
+000dcb20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000dcb30: 2020 2066 6f72 206b 2069 6e20 6d2e 6765     for k in m.ge
+000dcb40: 7428 2777 6f72 6b65 725f 6461 7461 5f64  t('worker_data_d
+000dcb50: 6973 6b73 2729 3a0a 2020 2020 2020 2020  isks'):.        
+000dcb60: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+000dcb70: 656c 203d 2053 6361 6c65 436c 7573 7465  el = ScaleCluste
+000dcb80: 7252 6571 7565 7374 576f 726b 6572 4461  rRequestWorkerDa
+000dcb90: 7461 4469 736b 7328 290a 2020 2020 2020  taDisks().      
+000dcba0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+000dcbb0: 6f72 6b65 725f 6461 7461 5f64 6973 6b73  orker_data_disks
+000dcbc0: 2e61 7070 656e 6428 7465 6d70 5f6d 6f64  .append(temp_mod
+000dcbd0: 656c 2e66 726f 6d5f 6d61 7028 6b29 290a  el.from_map(k)).
+000dcbe0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000dcbf0: 2827 776f 726b 6572 5f69 6e73 7461 6e63  ('worker_instanc
+000dcc00: 655f 6368 6172 6765 5f74 7970 6527 2920  e_charge_type') 
+000dcc10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000dcc20: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
+000dcc30: 726b 6572 5f69 6e73 7461 6e63 655f 6368  rker_instance_ch
+000dcc40: 6172 6765 5f74 7970 6520 3d20 6d2e 6765  arge_type = m.ge
+000dcc50: 7428 2777 6f72 6b65 725f 696e 7374 616e  t('worker_instan
+000dcc60: 6365 5f63 6861 7267 655f 7479 7065 2729  ce_charge_type')
+000dcc70: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000dcc80: 7428 2777 6f72 6b65 725f 696e 7374 616e  t('worker_instan
+000dcc90: 6365 5f74 7970 6573 2729 2069 7320 6e6f  ce_types') is no
+000dcca0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000dccb0: 2020 2020 7365 6c66 2e77 6f72 6b65 725f      self.worker_
+000dccc0: 696e 7374 616e 6365 5f74 7970 6573 203d  instance_types =
+000dccd0: 206d 2e67 6574 2827 776f 726b 6572 5f69   m.get('worker_i
+000dcce0: 6e73 7461 6e63 655f 7479 7065 7327 290a  nstance_types').
+000dccf0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000dcd00: 2827 776f 726b 6572 5f70 6572 696f 6427  ('worker_period'
+000dcd10: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000dcd20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000dcd30: 776f 726b 6572 5f70 6572 696f 6420 3d20  worker_period = 
+000dcd40: 6d2e 6765 7428 2777 6f72 6b65 725f 7065  m.get('worker_pe
+000dcd50: 7269 6f64 2729 0a20 2020 2020 2020 2069  riod').        i
+000dcd60: 6620 6d2e 6765 7428 2777 6f72 6b65 725f  f m.get('worker_
+000dcd70: 7065 7269 6f64 5f75 6e69 7427 2920 6973  period_unit') is
+000dcd80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000dcd90: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
+000dcda0: 6572 5f70 6572 696f 645f 756e 6974 203d  er_period_unit =
+000dcdb0: 206d 2e67 6574 2827 776f 726b 6572 5f70   m.get('worker_p
+000dcdc0: 6572 696f 645f 756e 6974 2729 0a20 2020  eriod_unit').   
+000dcdd0: 2020 2020 2069 6620 6d2e 6765 7428 2777       if m.get('w
+000dcde0: 6f72 6b65 725f 7379 7374 656d 5f64 6973  orker_system_dis
+000dcdf0: 6b5f 6361 7465 676f 7279 2729 2069 7320  k_category') is 
+000dce00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000dce10: 2020 2020 2020 7365 6c66 2e77 6f72 6b65        self.worke
+000dce20: 725f 7379 7374 656d 5f64 6973 6b5f 6361  r_system_disk_ca
+000dce30: 7465 676f 7279 203d 206d 2e67 6574 2827  tegory = m.get('
+000dce40: 776f 726b 6572 5f73 7973 7465 6d5f 6469  worker_system_di
+000dce50: 736b 5f63 6174 6567 6f72 7927 290a 2020  sk_category').  
+000dce60: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000dce70: 776f 726b 6572 5f73 7973 7465 6d5f 6469  worker_system_di
+000dce80: 736b 5f73 697a 6527 2920 6973 206e 6f74  sk_size') is not
+000dce90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000dcea0: 2020 2073 656c 662e 776f 726b 6572 5f73     self.worker_s
+000dceb0: 7973 7465 6d5f 6469 736b 5f73 697a 6520  ystem_disk_size 
+000dcec0: 3d20 6d2e 6765 7428 2777 6f72 6b65 725f  = m.get('worker_
+000dced0: 7379 7374 656d 5f64 6973 6b5f 7369 7a65  system_disk_size
+000dcee0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+000dcef0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+000dcf00: 6361 6c65 436c 7573 7465 7252 6573 706f  caleClusterRespo
+000dcf10: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+000dcf20: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000dcf30: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000dcf40: 662c 0a20 2020 2020 2020 2063 6c75 7374  f,.        clust
+000dcf50: 6572 5f69 643a 2073 7472 203d 204e 6f6e  er_id: str = Non
+000dcf60: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
+000dcf70: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+000dcf80: 652c 0a20 2020 2020 2020 2074 6173 6b5f  e,.        task_
+000dcf90: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+000dcfa0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+000dcfb0: 656c 662e 636c 7573 7465 725f 6964 203d  elf.cluster_id =
+000dcfc0: 2063 6c75 7374 6572 5f69 640a 2020 2020   cluster_id.    
+000dcfd0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+000dcfe0: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+000dcff0: 0a20 2020 2020 2020 2073 656c 662e 7461  .        self.ta
+000dd000: 736b 5f69 6420 3d20 7461 736b 5f69 640a  sk_id = task_id.
+000dd010: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000dd020: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000dd030: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+000dd040: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+000dd050: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+000dd060: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+000dd070: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+000dd080: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000dd090: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+000dd0a0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+000dd0b0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+000dd0c0: 2020 2069 6620 7365 6c66 2e63 6c75 7374     if self.clust
+000dd0d0: 6572 5f69 6420 6973 206e 6f74 204e 6f6e  er_id is not Non
+000dd0e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000dd0f0: 6573 756c 745b 2763 6c75 7374 6572 5f69  esult['cluster_i
+000dd100: 6427 5d20 3d20 7365 6c66 2e63 6c75 7374  d'] = self.clust
+000dd110: 6572 5f69 640a 2020 2020 2020 2020 6966  er_id.        if
+000dd120: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+000dd130: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000dd140: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000dd150: 5b27 7265 7175 6573 745f 6964 275d 203d  ['request_id'] =
+000dd160: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+000dd170: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000dd180: 2e74 6173 6b5f 6964 2069 7320 6e6f 7420  .task_id is not 
+000dd190: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000dd1a0: 2020 7265 7375 6c74 5b27 7461 736b 5f69    result['task_i
+000dd1b0: 6427 5d20 3d20 7365 6c66 2e74 6173 6b5f  d'] = self.task_
+000dd1c0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+000dd1d0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000dd1e0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000dd1f0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+000dd200: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000dd210: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+000dd220: 2020 6966 206d 2e67 6574 2827 636c 7573    if m.get('clus
+000dd230: 7465 725f 6964 2729 2069 7320 6e6f 7420  ter_id') is not 
+000dd240: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000dd250: 2020 7365 6c66 2e63 6c75 7374 6572 5f69    self.cluster_i
+000dd260: 6420 3d20 6d2e 6765 7428 2763 6c75 7374  d = m.get('clust
+000dd270: 6572 5f69 6427 290a 2020 2020 2020 2020  er_id').        
+000dd280: 6966 206d 2e67 6574 2827 7265 7175 6573  if m.get('reques
+000dd290: 745f 6964 2729 2069 7320 6e6f 7420 4e6f  t_id') is not No
+000dd2a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000dd2b0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+000dd2c0: 3d20 6d2e 6765 7428 2772 6571 7565 7374  = m.get('request
+000dd2d0: 5f69 6427 290a 2020 2020 2020 2020 6966  _id').        if
+000dd2e0: 206d 2e67 6574 2827 7461 736b 5f69 6427   m.get('task_id'
+000dd2f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000dd300: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000dd310: 7461 736b 5f69 6420 3d20 6d2e 6765 7428  task_id = m.get(
+000dd320: 2774 6173 6b5f 6964 2729 0a20 2020 2020  'task_id').     
+000dd330: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+000dd340: 0a63 6c61 7373 2053 6361 6c65 436c 7573  .class ScaleClus
+000dd350: 7465 7252 6573 706f 6e73 6528 5465 614d  terResponse(TeaM
+000dd360: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+000dd370: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000dd380: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
+000dd390: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
+000dd3a0: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
+000dd3b0: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
+000dd3c0: 6465 3a20 696e 7420 3d20 4e6f 6e65 2c0a  de: int = None,.
+000dd3d0: 2020 2020 2020 2020 626f 6479 3a20 5363          body: Sc
+000dd3e0: 616c 6543 6c75 7374 6572 5265 7370 6f6e  aleClusterRespon
+000dd3f0: 7365 426f 6479 203d 204e 6f6e 652c 0a20  seBody = None,. 
+000dd400: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+000dd410: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+000dd420: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
+000dd430: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+000dd440: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+000dd450: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+000dd460: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
+000dd470: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000dd480: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+000dd490: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+000dd4a0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+000dd4b0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+000dd4c0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000dd4d0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000dd4e0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+000dd4f0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000dd500: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000dd510: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000dd520: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000dd530: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000dd540: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+000dd550: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+000dd560: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000dd570: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+000dd580: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+000dd590: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+000dd5a0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+000dd5b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000dd5c0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+000dd5d0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+000dd5e0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000dd5f0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+000dd600: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000dd610: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+000dd620: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+000dd630: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+000dd640: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+000dd650: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000dd660: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+000dd670: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+000dd680: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000dd690: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000dd6a0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+000dd6b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000dd6c0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+000dd6d0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+000dd6e0: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+000dd6f0: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+000dd700: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+000dd710: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000dd720: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+000dd730: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+000dd740: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+000dd750: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+000dd760: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000dd770: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+000dd780: 656c 203d 2053 6361 6c65 436c 7573 7465  el = ScaleCluste
+000dd790: 7252 6573 706f 6e73 6542 6f64 7928 290a  rResponseBody().
+000dd7a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000dd7b0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+000dd7c0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+000dd7d0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+000dd7e0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000dd7f0: 7373 2053 6361 6c65 436c 7573 7465 724e  ss ScaleClusterN
+000dd800: 6f64 6550 6f6f 6c52 6571 7565 7374 2854  odePoolRequest(T
+000dd810: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000dd820: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000dd830: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000dd840: 2020 636f 756e 743a 2069 6e74 203d 204e    count: int = N
+000dd850: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+000dd860: 2020 2020 2320 5468 6520 6e75 6d62 6572      # The number
+000dd870: 206f 6620 776f 726b 6572 206e 6f64 6573   of worker nodes
+000dd880: 2074 6861 7420 796f 7520 7761 6e74 2074   that you want t
+000dd890: 6f20 6164 642e 2059 6f75 2063 616e 2061  o add. You can a
+000dd8a0: 6464 2061 7420 6d6f 7374 2035 3030 206e  dd at most 500 n
+000dd8b0: 6f64 6573 2069 6e20 6f6e 6520 4150 4920  odes in one API 
+000dd8c0: 6361 6c6c 2e20 5468 6520 6d61 7869 6d75  call. The maximu
+000dd8d0: 6d20 6e75 6d62 6572 206f 6620 6e6f 6465  m number of node
+000dd8e0: 7320 7468 6174 2063 616e 2062 6520 6164  s that can be ad
+000dd8f0: 6465 6420 6973 206c 696d 6974 6564 2062  ded is limited b
+000dd900: 7920 7468 6520 7175 6f74 6120 6f66 206e  y the quota of n
+000dd910: 6f64 6573 2069 6e20 7468 6520 636c 7573  odes in the clus
+000dd920: 7465 722e 0a20 2020 2020 2020 2073 656c  ter..        sel
+000dd930: 662e 636f 756e 7420 3d20 636f 756e 740a  f.count = count.
+000dd940: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000dd950: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000dd960: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+000dd970: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+000dd980: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+000dd990: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+000dd9a0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+000dd9b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000dd9c0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+000dd9d0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+000dd9e0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+000dd9f0: 2020 2069 6620 7365 6c66 2e63 6f75 6e74     if self.count
+000dda00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000dda10: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000dda20: 5b27 636f 756e 7427 5d20 3d20 7365 6c66  ['count'] = self
+000dda30: 2e63 6f75 6e74 0a20 2020 2020 2020 2072  .count.        r
+000dda40: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+000dda50: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+000dda60: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+000dda70: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+000dda80: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+000dda90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000ddaa0: 636f 756e 7427 2920 6973 206e 6f74 204e  count') is not N
+000ddab0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ddac0: 2073 656c 662e 636f 756e 7420 3d20 6d2e   self.count = m.
+000ddad0: 6765 7428 2763 6f75 6e74 2729 0a20 2020  get('count').   
+000ddae0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000ddaf0: 0a0a 0a63 6c61 7373 2053 6361 6c65 436c  ...class ScaleCl
+000ddb00: 7573 7465 724e 6f64 6550 6f6f 6c52 6573  usterNodePoolRes
+000ddb10: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+000ddb20: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000ddb30: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000ddb40: 656c 662c 0a20 2020 2020 2020 2074 6173  elf,.        tas
+000ddb50: 6b5f 6964 3a20 7374 7220 3d20 4e6f 6e65  k_id: str = None
+000ddb60: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+000ddb70: 2023 2054 6865 2074 6173 6b20 4944 2e0a   # The task ID..
+000ddb80: 2020 2020 2020 2020 7365 6c66 2e74 6173          self.tas
+000ddb90: 6b5f 6964 203d 2074 6173 6b5f 6964 0a0a  k_id = task_id..
+000ddba0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000ddbb0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000ddbc0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+000ddbd0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000ddbe0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000ddbf0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+000ddc00: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000ddc10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000ddc20: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000ddc30: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000ddc40: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000ddc50: 2020 6966 2073 656c 662e 7461 736b 5f69    if self.task_i
+000ddc60: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+000ddc70: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000ddc80: 745b 2774 6173 6b5f 6964 275d 203d 2073  t['task_id'] = s
+000ddc90: 656c 662e 7461 736b 5f69 640a 2020 2020  elf.task_id.    
+000ddca0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000ddcb0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000ddcc0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000ddcd0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000ddce0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000ddcf0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+000ddd00: 6765 7428 2774 6173 6b5f 6964 2729 2069  get('task_id') i
+000ddd10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000ddd20: 2020 2020 2020 2020 7365 6c66 2e74 6173          self.tas
+000ddd30: 6b5f 6964 203d 206d 2e67 6574 2827 7461  k_id = m.get('ta
+000ddd40: 736b 5f69 6427 290a 2020 2020 2020 2020  sk_id').        
+000ddd50: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000ddd60: 6173 7320 5363 616c 6543 6c75 7374 6572  ass ScaleCluster
+000ddd70: 4e6f 6465 506f 6f6c 5265 7370 6f6e 7365  NodePoolResponse
+000ddd80: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000ddd90: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000ddda0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000dddb0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+000dddc0: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+000dddd0: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+000ddde0: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+000dddf0: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+000dde00: 793a 2053 6361 6c65 436c 7573 7465 724e  y: ScaleClusterN
+000dde10: 6f64 6550 6f6f 6c52 6573 706f 6e73 6542  odePoolResponseB
+000dde20: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
+000dde30: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000dde40: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+000dde50: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+000dde60: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+000dde70: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000dde80: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+000dde90: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+000ddea0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000ddeb0: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+000ddec0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000dded0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+000ddee0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+000ddef0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000ddf00: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+000ddf10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000ddf20: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+000ddf30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000ddf40: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+000ddf50: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000ddf60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000ddf70: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+000ddf80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000ddf90: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000ddfa0: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+000ddfb0: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+000ddfc0: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+000ddfd0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+000ddfe0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000ddff0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+000de000: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+000de010: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+000de020: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+000de030: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000de040: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+000de050: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+000de060: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000de070: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+000de080: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+000de090: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+000de0a0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+000de0b0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000de0c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000de0d0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+000de0e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000de0f0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000de100: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+000de110: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000de120: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+000de130: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000de140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000de150: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+000de160: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+000de170: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000de180: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+000de190: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000de1a0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+000de1b0: 3d20 5363 616c 6543 6c75 7374 6572 4e6f  = ScaleClusterNo
+000de1c0: 6465 506f 6f6c 5265 7370 6f6e 7365 426f  dePoolResponseBo
+000de1d0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+000de1e0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+000de1f0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+000de200: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+000de210: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000de220: 0a0a 636c 6173 7320 5363 616c 654f 7574  ..class ScaleOut
+000de230: 436c 7573 7465 7252 6571 7565 7374 576f  ClusterRequestWo
+000de240: 726b 6572 4461 7461 4469 736b 7328 5465  rkerDataDisks(Te
+000de250: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+000de260: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000de270: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000de280: 2061 7574 6f5f 736e 6170 7368 6f74 5f70   auto_snapshot_p
+000de290: 6f6c 6963 795f 6964 3a20 7374 7220 3d20  olicy_id: str = 
+000de2a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6361  None,.        ca
+000de2b0: 7465 676f 7279 3a20 7374 7220 3d20 4e6f  tegory: str = No
+000de2c0: 6e65 2c0a 2020 2020 2020 2020 656e 6372  ne,.        encr
+000de2d0: 7970 7465 643a 2073 7472 203d 204e 6f6e  ypted: str = Non
+000de2e0: 652c 0a20 2020 2020 2020 2073 697a 653a  e,.        size:
+000de2f0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000de300: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
+000de310: 6520 4944 206f 6620 616e 2061 7574 6f6d  e ID of an autom
+000de320: 6174 6963 2073 6e61 7073 686f 7420 706f  atic snapshot po
+000de330: 6c69 6379 2e20 4175 746f 6d61 7469 6320  licy. Automatic 
+000de340: 6261 636b 7570 2069 7320 7065 7266 6f72  backup is perfor
+000de350: 6d65 6420 666f 7220 6120 6469 736b 2062  med for a disk b
+000de360: 6173 6564 206f 6e20 7468 6520 7370 6563  ased on the spec
+000de370: 6966 6965 6420 6175 746f 6d61 7469 6320  ified automatic 
+000de380: 736e 6170 7368 6f74 2070 6f6c 6963 792e  snapshot policy.
+000de390: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
+000de3a0: 2020 2020 2320 4279 2064 6566 6175 6c74      # By default
+000de3b0: 2c20 7468 6973 2070 6172 616d 6574 6572  , this parameter
+000de3c0: 2069 7320 656d 7074 792c 2077 6869 6368   is empty, which
+000de3d0: 2069 6e64 6963 6174 6573 2074 6861 7420   indicates that 
+000de3e0: 6175 746f 6d61 7469 6320 6261 636b 7570  automatic backup
+000de3f0: 2069 7320 6469 7361 626c 6564 2e0a 2020   is disabled..  
+000de400: 2020 2020 2020 7365 6c66 2e61 7574 6f5f        self.auto_
+000de410: 736e 6170 7368 6f74 5f70 6f6c 6963 795f  snapshot_policy_
+000de420: 6964 203d 2061 7574 6f5f 736e 6170 7368  id = auto_snapsh
+000de430: 6f74 5f70 6f6c 6963 795f 6964 0a20 2020  ot_policy_id.   
+000de440: 2020 2020 2023 2054 6865 2064 6174 6120       # The data 
+000de450: 6469 736b 2074 7970 652e 0a20 2020 2020  disk type..     
+000de460: 2020 2073 656c 662e 6361 7465 676f 7279     self.category
+000de470: 203d 2063 6174 6567 6f72 790a 2020 2020   = category.    
+000de480: 2020 2020 2320 5370 6563 6966 6965 7320      # Specifies 
+000de490: 7768 6574 6865 7220 746f 2065 6e63 7279  whether to encry
+000de4a0: 7074 2074 6865 2064 6174 6120 6469 736b  pt the data disk
+000de4b0: 732e 2056 616c 6964 2076 616c 7565 733a  s. Valid values:
+000de4c0: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
+000de4d0: 2020 2020 2320 2a20 2020 6074 7275 6560      # *   `true`
+000de4e0: 3a20 656e 6372 7970 7473 2064 6174 6120  : encrypts data 
+000de4f0: 6469 736b 732e 0a20 2020 2020 2020 2023  disks..        #
+000de500: 202a 2020 2060 6661 6c73 6560 3a20 646f   *   `false`: do
+000de510: 6573 206e 6f74 2065 6e63 7279 7074 2064  es not encrypt d
+000de520: 6174 6120 6469 736b 732e 0a20 2020 2020  ata disks..     
+000de530: 2020 2023 200a 2020 2020 2020 2020 2320     # .        # 
+000de540: 4465 6661 756c 7420 7661 6c75 653a 2060  Default value: `
+000de550: 6661 6c73 6560 2e0a 2020 2020 2020 2020  false`..        
+000de560: 7365 6c66 2e65 6e63 7279 7074 6564 203d  self.encrypted =
+000de570: 2065 6e63 7279 7074 6564 0a20 2020 2020   encrypted.     
+000de580: 2020 2023 2054 6865 2073 697a 6520 6f66     # The size of
+000de590: 2074 6865 2064 6174 6120 6469 736b 2e20   the data disk. 
+000de5a0: 5661 6c69 6420 7661 6c75 6573 3a20 3430  Valid values: 40
+000de5b0: 2074 6f20 3332 3736 372e 0a20 2020 2020   to 32767..     
+000de5c0: 2020 2073 656c 662e 7369 7a65 203d 2073     self.size = s
+000de5d0: 697a 650a 0a20 2020 2064 6566 2076 616c  ize..    def val
+000de5e0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000de5f0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000de600: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+000de610: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000de620: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+000de630: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+000de640: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000de650: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000de660: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+000de670: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+000de680: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+000de690: 7574 6f5f 736e 6170 7368 6f74 5f70 6f6c  uto_snapshot_pol
+000de6a0: 6963 795f 6964 2069 7320 6e6f 7420 4e6f  icy_id is not No
+000de6b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000de6c0: 7265 7375 6c74 5b27 6175 746f 5f73 6e61  result['auto_sna
+000de6d0: 7073 686f 745f 706f 6c69 6379 5f69 6427  pshot_policy_id'
+000de6e0: 5d20 3d20 7365 6c66 2e61 7574 6f5f 736e  ] = self.auto_sn
+000de6f0: 6170 7368 6f74 5f70 6f6c 6963 795f 6964  apshot_policy_id
+000de700: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000de710: 2e63 6174 6567 6f72 7920 6973 206e 6f74  .category is not
+000de720: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000de730: 2020 2072 6573 756c 745b 2763 6174 6567     result['categ
+000de740: 6f72 7927 5d20 3d20 7365 6c66 2e63 6174  ory'] = self.cat
+000de750: 6567 6f72 790a 2020 2020 2020 2020 6966  egory.        if
+000de760: 2073 656c 662e 656e 6372 7970 7465 6420   self.encrypted 
+000de770: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000de780: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000de790: 2765 6e63 7279 7074 6564 275d 203d 2073  'encrypted'] = s
+000de7a0: 656c 662e 656e 6372 7970 7465 640a 2020  elf.encrypted.  
+000de7b0: 2020 2020 2020 6966 2073 656c 662e 7369        if self.si
+000de7c0: 7a65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ze is not None:.
+000de7d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000de7e0: 6c74 5b27 7369 7a65 275d 203d 2073 656c  lt['size'] = sel
+000de7f0: 662e 7369 7a65 0a20 2020 2020 2020 2072  f.size.        r
+000de800: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+000de810: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+000de820: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+000de830: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+000de840: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+000de850: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000de860: 6175 746f 5f73 6e61 7073 686f 745f 706f  auto_snapshot_po
+000de870: 6c69 6379 5f69 6427 2920 6973 206e 6f74  licy_id') is not
+000de880: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000de890: 2020 2073 656c 662e 6175 746f 5f73 6e61     self.auto_sna
+000de8a0: 7073 686f 745f 706f 6c69 6379 5f69 6420  pshot_policy_id 
+000de8b0: 3d20 6d2e 6765 7428 2761 7574 6f5f 736e  = m.get('auto_sn
+000de8c0: 6170 7368 6f74 5f70 6f6c 6963 795f 6964  apshot_policy_id
+000de8d0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000de8e0: 6765 7428 2763 6174 6567 6f72 7927 2920  get('category') 
+000de8f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000de900: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+000de910: 7465 676f 7279 203d 206d 2e67 6574 2827  tegory = m.get('
+000de920: 6361 7465 676f 7279 2729 0a20 2020 2020  category').     
+000de930: 2020 2069 6620 6d2e 6765 7428 2765 6e63     if m.get('enc
+000de940: 7279 7074 6564 2729 2069 7320 6e6f 7420  rypted') is not 
+000de950: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000de960: 2020 7365 6c66 2e65 6e63 7279 7074 6564    self.encrypted
+000de970: 203d 206d 2e67 6574 2827 656e 6372 7970   = m.get('encryp
+000de980: 7465 6427 290a 2020 2020 2020 2020 6966  ted').        if
+000de990: 206d 2e67 6574 2827 7369 7a65 2729 2069   m.get('size') i
+000de9a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000de9b0: 2020 2020 2020 2020 7365 6c66 2e73 697a          self.siz
+000de9c0: 6520 3d20 6d2e 6765 7428 2773 697a 6527  e = m.get('size'
+000de9d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000de9e0: 2073 656c 660a 0a0a 636c 6173 7320 5363   self...class Sc
+000de9f0: 616c 654f 7574 436c 7573 7465 7252 6571  aleOutClusterReq
+000dea00: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+000dea10: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000dea20: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000dea30: 2020 2020 2020 2020 636c 6f75 645f 6d6f          cloud_mo
+000dea40: 6e69 746f 725f 666c 6167 733a 2062 6f6f  nitor_flags: boo
+000dea50: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
+000dea60: 2020 636f 756e 743a 2069 6e74 203d 204e    count: int = N
+000dea70: 6f6e 652c 0a20 2020 2020 2020 2063 7075  one,.        cpu
+000dea80: 5f70 6f6c 6963 793a 2073 7472 203d 204e  _policy: str = N
+000dea90: 6f6e 652c 0a20 2020 2020 2020 2069 6d61  one,.        ima
+000deaa0: 6765 5f69 643a 2073 7472 203d 204e 6f6e  ge_id: str = Non
+000deab0: 652c 0a20 2020 2020 2020 206b 6579 5f70  e,.        key_p
+000deac0: 6169 723a 2073 7472 203d 204e 6f6e 652c  air: str = None,
+000dead0: 0a20 2020 2020 2020 206c 6f67 696e 5f70  .        login_p
+000deae0: 6173 7377 6f72 643a 2073 7472 203d 204e  assword: str = N
+000deaf0: 6f6e 652c 0a20 2020 2020 2020 2072 6473  one,.        rds
+000deb00: 5f69 6e73 7461 6e63 6573 3a20 4c69 7374  _instances: List
+000deb10: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+000deb20: 2020 2020 2020 7275 6e74 696d 653a 2052        runtime: R
+000deb30: 756e 7469 6d65 203d 204e 6f6e 652c 0a20  untime = None,. 
+000deb40: 2020 2020 2020 2074 6167 733a 204c 6973         tags: Lis
+000deb50: 745b 5461 675d 203d 204e 6f6e 652c 0a20  t[Tag] = None,. 
+000deb60: 2020 2020 2020 2074 6169 6e74 733a 204c         taints: L
+000deb70: 6973 745b 5461 696e 745d 203d 204e 6f6e  ist[Taint] = Non
+000deb80: 652c 0a20 2020 2020 2020 2075 7365 725f  e,.        user_
+000deb90: 6461 7461 3a20 7374 7220 3d20 4e6f 6e65  data: str = None
+000deba0: 2c0a 2020 2020 2020 2020 7673 7769 7463  ,.        vswitc
+000debb0: 685f 6964 733a 204c 6973 745b 7374 725d  h_ids: List[str]
+000debc0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000debd0: 2077 6f72 6b65 725f 6175 746f 5f72 656e   worker_auto_ren
+000debe0: 6577 3a20 626f 6f6c 203d 204e 6f6e 652c  ew: bool = None,
+000debf0: 0a20 2020 2020 2020 2077 6f72 6b65 725f  .        worker_
+000dec00: 6175 746f 5f72 656e 6577 5f70 6572 696f  auto_renew_perio
+000dec10: 643a 2069 6e74 203d 204e 6f6e 652c 0a20  d: int = None,. 
+000dec20: 2020 2020 2020 2077 6f72 6b65 725f 6461         worker_da
+000dec30: 7461 5f64 6973 6b73 3a20 4c69 7374 5b53  ta_disks: List[S
+000dec40: 6361 6c65 4f75 7443 6c75 7374 6572 5265  caleOutClusterRe
+000dec50: 7175 6573 7457 6f72 6b65 7244 6174 6144  questWorkerDataD
+000dec60: 6973 6b73 5d20 3d20 4e6f 6e65 2c0a 2020  isks] = None,.  
+000dec70: 2020 2020 2020 776f 726b 6572 5f69 6e73        worker_ins
+000dec80: 7461 6e63 655f 6368 6172 6765 5f74 7970  tance_charge_typ
+000dec90: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+000deca0: 2020 2020 2020 2077 6f72 6b65 725f 696e         worker_in
+000decb0: 7374 616e 6365 5f74 7970 6573 3a20 4c69  stance_types: Li
+000decc0: 7374 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  st[str] = None,.
+000decd0: 2020 2020 2020 2020 776f 726b 6572 5f70          worker_p
+000dece0: 6572 696f 643a 2069 6e74 203d 204e 6f6e  eriod: int = Non
+000decf0: 652c 0a20 2020 2020 2020 2077 6f72 6b65  e,.        worke
+000ded00: 725f 7065 7269 6f64 5f75 6e69 743a 2073  r_period_unit: s
+000ded10: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000ded20: 2020 2077 6f72 6b65 725f 7379 7374 656d     worker_system
+000ded30: 5f64 6973 6b5f 6361 7465 676f 7279 3a20  _disk_category: 
+000ded40: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000ded50: 2020 2020 776f 726b 6572 5f73 7973 7465      worker_syste
+000ded60: 6d5f 6469 736b 5f73 697a 653a 2069 6e74  m_disk_size: int
+000ded70: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+000ded80: 2020 2020 2020 2020 2320 5370 6563 6966          # Specif
+000ded90: 6965 7320 7768 6574 6865 7220 746f 2069  ies whether to i
+000deda0: 6e73 7461 6c6c 2074 6865 2043 6c6f 7564  nstall the Cloud
+000dedb0: 4d6f 6e69 746f 7220 6167 656e 742e 2056  Monitor agent. V
+000dedc0: 616c 6964 2076 616c 7565 733a 0a20 2020  alid values:.   
+000dedd0: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+000dede0: 2320 2a20 2020 6074 7275 6560 3a20 696e  # *   `true`: in
+000dedf0: 7374 616c 6c73 2074 6865 2043 6c6f 7564  stalls the Cloud
+000dee00: 4d6f 6e69 746f 7220 6167 656e 742e 0a20  Monitor agent.. 
+000dee10: 2020 2020 2020 2023 202a 2020 2060 6661         # *   `fa
+000dee20: 6c73 6560 3a20 646f 6573 206e 6f74 2069  lse`: does not i
+000dee30: 6e73 7461 6c6c 2074 6865 2043 6c6f 7564  nstall the Cloud
+000dee40: 4d6f 6e69 746f 7220 6167 656e 742e 0a20  Monitor agent.. 
+000dee50: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+000dee60: 2020 2320 4465 6661 756c 7420 7661 6c75    # Default valu
+000dee70: 653a 2060 6661 6c73 6560 2e0a 2020 2020  e: `false`..    
+000dee80: 2020 2020 7365 6c66 2e63 6c6f 7564 5f6d      self.cloud_m
+000dee90: 6f6e 6974 6f72 5f66 6c61 6773 203d 2063  onitor_flags = c
+000deea0: 6c6f 7564 5f6d 6f6e 6974 6f72 5f66 6c61  loud_monitor_fla
+000deeb0: 6773 0a20 2020 2020 2020 2023 2054 6865  gs.        # The
+000deec0: 206e 756d 6265 7220 6f66 2077 6f72 6b65   number of worke
+000deed0: 7220 6e6f 6465 7320 7468 6174 2079 6f75  r nodes that you
+000deee0: 2077 616e 7420 746f 2061 6464 2e0a 2020   want to add..  
+000deef0: 2020 2020 2020 2320 0a20 2020 2020 2020        # .       
+000def00: 2023 2054 6869 7320 7061 7261 6d65 7465   # This paramete
+000def10: 7220 6973 2072 6571 7569 7265 642e 0a20  r is required.. 
+000def20: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+000def30: 7420 3d20 636f 756e 740a 2020 2020 2020  t = count.      
+000def40: 2020 2320 5468 6520 4350 5520 6d61 6e61    # The CPU mana
+000def50: 6765 6d65 6e74 2070 6f6c 6963 7920 6f66  gement policy of
+000def60: 2074 6865 206e 6f64 6573 2069 6e20 6120   the nodes in a 
+000def70: 6e6f 6465 2070 6f6f 6c2e 2054 6865 2066  node pool. The f
+000def80: 6f6c 6c6f 7769 6e67 2070 6f6c 6963 6965  ollowing policie
+000def90: 7320 6172 6520 7375 7070 6f72 7465 6420  s are supported 
+000defa0: 6966 2074 6865 204b 7562 6572 6e65 7465  if the Kubernete
+000defb0: 7320 7665 7273 696f 6e20 6f66 2074 6865  s version of the
+000defc0: 2063 6c75 7374 6572 2069 7320 312e 3132   cluster is 1.12
+000defd0: 2e36 206f 7220 6c61 7465 722e 0a20 2020  .6 or later..   
+000defe0: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+000deff0: 2320 2a20 2020 6073 7461 7469 6360 3a20  # *   `static`: 
+000df000: 5468 6973 2070 6f6c 6963 7920 616c 6c6f  This policy allo
+000df010: 7773 2070 6f64 7320 7769 7468 2073 7065  ws pods with spe
+000df020: 6369 6669 6320 7265 736f 7572 6365 2063  cific resource c
+000df030: 6861 7261 6374 6572 6973 7469 6373 206f  haracteristics o
+000df040: 6e20 7468 6520 6e6f 6465 2074 6f20 6265  n the node to be
+000df050: 2067 7261 6e74 6564 2077 6974 6820 656e   granted with en
+000df060: 6861 6e63 6564 2043 5055 2061 6666 696e  hanced CPU affin
+000df070: 6974 7920 616e 6420 6578 636c 7573 6976  ity and exclusiv
+000df080: 6974 792e 0a20 2020 2020 2020 2023 202a  ity..        # *
+000df090: 2020 2060 6e6f 6e65 603a 2054 6865 2064     `none`: The d
+000df0a0: 6566 6175 6c74 2043 5055 2061 6666 696e  efault CPU affin
+000df0b0: 6974 7920 6973 2075 7365 642e 0a20 2020  ity is used..   
+000df0c0: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+000df0d0: 2320 4465 6661 756c 7420 7661 6c75 653a  # Default value:
+000df0e0: 2060 6e6f 6e65 602e 0a20 2020 2020 2020   `none`..       
+000df0f0: 2073 656c 662e 6370 755f 706f 6c69 6379   self.cpu_policy
+000df100: 203d 2063 7075 5f70 6f6c 6963 790a 2020   = cpu_policy.  
+000df110: 2020 2020 2020 2320 5370 6563 6966 6965        # Specifie
+000df120: 7320 6120 6375 7374 6f6d 2069 6d61 6765  s a custom image
+000df130: 2066 6f72 206e 6f64 6573 2e20 4279 2064   for nodes. By d
+000df140: 6566 6175 6c74 2c20 7468 6520 696d 6167  efault, the imag
+000df150: 6520 7072 6f76 6964 6564 2062 7920 436f  e provided by Co
+000df160: 6e74 6169 6e65 7220 5365 7276 6963 6520  ntainer Service 
+000df170: 666f 7220 4b75 6265 726e 6574 6573 2028  for Kubernetes (
+000df180: 4143 4b29 2069 7320 7573 6564 2e20 596f  ACK) is used. Yo
+000df190: 7520 6361 6e20 7365 6c65 6374 2061 2063  u can select a c
+000df1a0: 7573 746f 6d20 696d 6167 6520 746f 2072  ustom image to r
+000df1b0: 6570 6c61 6365 2074 6865 2064 6566 6175  eplace the defau
+000df1c0: 6c74 2069 6d61 6765 2e20 466f 7220 6d6f  lt image. For mo
+000df1d0: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
+000df1e0: 7365 6520 5b43 7573 746f 6d20 696d 6167  see [Custom imag
+000df1f0: 6573 5d28 6874 7470 733a 2f2f 6865 6c70  es](https://help
+000df200: 2e61 6c69 7975 6e2e 636f 6d2f 646f 6375  .aliyun.com/docu
+000df210: 6d65 6e74 5f64 6574 6169 6c2f 3134 3636  ment_detail/1466
+000df220: 3437 2e68 746d 6c29 2e0a 2020 2020 2020  47.html)..      
+000df230: 2020 7365 6c66 2e69 6d61 6765 5f69 6420    self.image_id 
+000df240: 3d20 696d 6167 655f 6964 0a20 2020 2020  = image_id.     
+000df250: 2020 2023 2054 6865 206e 616d 6520 6f66     # The name of
+000df260: 2074 6865 206b 6579 2070 6169 722e 2059   the key pair. Y
+000df270: 6f75 206d 7573 7420 7365 7420 7468 6973  ou must set this
+000df280: 2070 6172 616d 6574 6572 206f 7220 7468   parameter or th
+000df290: 6520 606c 6f67 696e 5f70 6173 7377 6f72  e `login_passwor
+000df2a0: 6460 2070 6172 616d 6574 6572 2e0a 2020  d` parameter..  
+000df2b0: 2020 2020 2020 2320 0a20 2020 2020 2020        # .       
+000df2c0: 2023 2054 6869 7320 7061 7261 6d65 7465   # This paramete
+000df2d0: 7220 6973 2072 6571 7569 7265 642e 0a20  r is required.. 
+000df2e0: 2020 2020 2020 2073 656c 662e 6b65 795f         self.key_
+000df2f0: 7061 6972 203d 206b 6579 5f70 6169 720a  pair = key_pair.
+000df300: 2020 2020 2020 2020 2320 5468 6520 7061          # The pa
+000df310: 7373 776f 7264 2066 6f72 2053 5348 206c  ssword for SSH l
+000df320: 6f67 6f6e 2e20 596f 7520 6d75 7374 2073  ogon. You must s
+000df330: 6574 2074 6869 7320 7061 7261 6d65 7465  et this paramete
+000df340: 7220 6f72 2074 6865 2060 6b65 795f 7061  r or the `key_pa
+000df350: 6972 6020 7061 7261 6d65 7465 722e 2054  ir` parameter. T
+000df360: 6865 2070 6173 7377 6f72 6420 6d75 7374  he password must
+000df370: 2062 6520 3820 746f 2033 3020 6368 6172   be 8 to 30 char
+000df380: 6163 7465 7273 2069 6e20 6c65 6e67 7468  acters in length
+000df390: 2c20 616e 6420 6d75 7374 2063 6f6e 7461  , and must conta
+000df3a0: 696e 2061 7420 6c65 6173 7420 7468 7265  in at least thre
+000df3b0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+000df3c0: 6e67 2063 6861 7261 6374 6572 2074 7970  ng character typ
+000df3d0: 6573 3a20 7570 7065 7263 6173 6520 6c65  es: uppercase le
+000df3e0: 7474 6572 732c 206c 6f77 6572 6361 7365  tters, lowercase
+000df3f0: 206c 6574 7465 7273 2c20 6469 6769 7473   letters, digits
+000df400: 2c20 616e 6420 7370 6563 6961 6c20 6368  , and special ch
+000df410: 6172 6163 7465 7273 2e0a 2020 2020 2020  aracters..      
+000df420: 2020 2320 0a20 2020 2020 2020 2023 2054    # .        # T
+000df430: 6869 7320 7061 7261 6d65 7465 7220 6973  his parameter is
+000df440: 2072 6571 7569 7265 642e 0a20 2020 2020   required..     
+000df450: 2020 2073 656c 662e 6c6f 6769 6e5f 7061     self.login_pa
+000df460: 7373 776f 7264 203d 206c 6f67 696e 5f70  ssword = login_p
+000df470: 6173 7377 6f72 640a 2020 2020 2020 2020  assword.        
+000df480: 2320 4166 7465 7220 796f 7520 7370 6563  # After you spec
+000df490: 6966 7920 7468 6520 6c69 7374 206f 6620  ify the list of 
+000df4a0: 4170 7361 7261 4442 2052 4453 2069 6e73  ApsaraDB RDS ins
+000df4b0: 7461 6e63 6573 2c20 7468 6520 4543 5320  tances, the ECS 
+000df4c0: 696e 7374 616e 6365 7320 696e 2074 6865  instances in the
+000df4d0: 2063 6c75 7374 6572 2061 7265 2061 7574   cluster are aut
+000df4e0: 6f6d 6174 6963 616c 6c79 2061 6464 6564  omatically added
+000df4f0: 2074 6f20 7468 6520 7768 6974 656c 6973   to the whitelis
+000df500: 7420 6f66 2074 6865 2041 7073 6172 6144  t of the ApsaraD
+000df510: 4220 5244 5320 696e 7374 616e 6365 732e  B RDS instances.
+000df520: 0a20 2020 2020 2020 2073 656c 662e 7264  .        self.rd
+000df530: 735f 696e 7374 616e 6365 7320 3d20 7264  s_instances = rd
+000df540: 735f 696e 7374 616e 6365 730a 2020 2020  s_instances.    
+000df550: 2020 2020 2320 5468 6520 636f 6e74 6169      # The contai
+000df560: 6e65 7220 7275 6e74 696d 652e 0a20 2020  ner runtime..   
+000df570: 2020 2020 2073 656c 662e 7275 6e74 696d       self.runtim
+000df580: 6520 3d20 7275 6e74 696d 650a 2020 2020  e = runtime.    
+000df590: 2020 2020 2320 5468 6520 6c61 6265 6c73      # The labels
+000df5a0: 2074 6861 7420 796f 7520 7761 6e74 2074   that you want t
+000df5b0: 6f20 6164 6420 746f 206e 6f64 6573 2e20  o add to nodes. 
+000df5c0: 596f 7520 6d75 7374 2061 6464 206c 6162  You must add lab
+000df5d0: 656c 7320 6261 7365 6420 6f6e 2074 6865  els based on the
+000df5e0: 2066 6f6c 6c6f 7769 6e67 2072 756c 6573   following rules
+000df5f0: 3a0a 2020 2020 2020 2020 2320 0a20 2020  :.        # .   
+000df600: 2020 2020 2023 202a 2020 2045 6163 6820       # *   Each 
+000df610: 6c61 6265 6c20 6973 2061 2063 6173 652d  label is a case-
+000df620: 7365 6e73 6974 6976 6520 6b65 792d 7661  sensitive key-va
+000df630: 6c75 6520 7061 6972 2e20 596f 7520 6361  lue pair. You ca
+000df640: 6e20 6164 6420 7570 2074 6f20 3230 206c  n add up to 20 l
+000df650: 6162 656c 732e 0a20 2020 2020 2020 2023  abels..        #
+000df660: 202a 2020 2041 206b 6579 206d 7573 7420   *   A key must 
+000df670: 6265 2075 6e69 7175 6520 616e 6420 6361  be unique and ca
+000df680: 6e6e 6f74 2065 7863 6565 6420 3634 2063  nnot exceed 64 c
+000df690: 6861 7261 6374 6572 7320 696e 206c 656e  haracters in len
+000df6a0: 6774 682e 2041 2076 616c 7565 2063 616e  gth. A value can
+000df6b0: 2062 6520 656d 7074 7920 616e 6420 6361   be empty and ca
+000df6c0: 6e6e 6f74 2065 7863 6565 6420 3132 3820  nnot exceed 128 
+000df6d0: 6368 6172 6163 7465 7273 2069 6e20 6c65  characters in le
+000df6e0: 6e67 7468 2e20 4b65 7973 2061 6e64 2076  ngth. Keys and v
+000df6f0: 616c 7565 7320 6361 6e6e 6f74 2073 7461  alues cannot sta
+000df700: 7274 2077 6974 6820 616c 6979 756e 2c20  rt with aliyun, 
+000df710: 6163 733a 2c20 6874 7470 733a 2f2f 2c20  acs:, https://, 
+000df720: 6f72 2068 7474 703a 2f2f 2e20 466f 7220  or http://. For 
+000df730: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+000df740: 2c20 7365 6520 5b4c 6162 656c 7320 616e  , see [Labels an
+000df750: 6420 5365 6c65 6374 6f72 735d 2868 7474  d Selectors](htt
+000df760: 7073 3a2f 2f6b 7562 6572 6e65 7465 732e  ps://kubernetes.
+000df770: 696f 2f64 6f63 732f 636f 6e63 6570 7473  io/docs/concepts
+000df780: 2f6f 7665 7276 6965 772f 776f 726b 696e  /overview/workin
+000df790: 672d 7769 7468 2d6f 626a 6563 7473 2f6c  g-with-objects/l
+000df7a0: 6162 656c 732f 2373 796e 7461 782d 616e  abels/#syntax-an
+000df7b0: 642d 6368 6172 6163 7465 722d 7365 7429  d-character-set)
+000df7c0: 2e0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+000df7d0: 6167 7320 3d20 7461 6773 0a20 2020 2020  ags = tags.     
+000df7e0: 2020 2023 2054 6865 2074 6169 6e74 7320     # The taints 
+000df7f0: 7468 6174 2079 6f75 2077 616e 7420 746f  that you want to
+000df800: 2061 6464 2074 6f20 6e6f 6465 732e 2054   add to nodes. T
+000df810: 6169 6e74 7320 6172 6520 6164 6465 6420  aints are added 
+000df820: 746f 206e 6f64 6573 2074 6f20 7072 6576  to nodes to prev
+000df830: 656e 7420 706f 6473 2066 726f 6d20 6265  ent pods from be
+000df840: 696e 6720 7363 6865 6475 6c65 6420 746f  ing scheduled to
+000df850: 2069 6e61 7070 726f 7072 6961 7465 206e   inappropriate n
+000df860: 6f64 6573 2e20 486f 7765 7665 722c 2074  odes. However, t
+000df870: 6f6c 6572 6174 696f 6e73 2061 6c6c 6f77  olerations allow
+000df880: 2070 6f64 7320 746f 2062 6520 7363 6865   pods to be sche
+000df890: 6475 6c65 6420 746f 206e 6f64 6573 2077  duled to nodes w
+000df8a0: 6974 6820 6d61 7463 6869 6e67 2074 6169  ith matching tai
+000df8b0: 6e74 732e 2046 6f72 206d 6f72 6520 696e  nts. For more in
+000df8c0: 666f 726d 6174 696f 6e2c 2073 6565 205b  formation, see [
+000df8d0: 5461 696e 7473 2061 6e64 2054 6f6c 6572  Taints and Toler
+000df8e0: 6174 696f 6e73 5d28 6874 7470 733a 2f2f  ations](https://
+000df8f0: 6b75 6265 726e 6574 6573 2e69 6f2f 7a68  kubernetes.io/zh
+000df900: 2f64 6f63 732f 636f 6e63 6570 7473 2f73  /docs/concepts/s
+000df910: 6368 6564 756c 696e 672d 6576 6963 7469  cheduling-evicti
+000df920: 6f6e 2f74 6169 6e74 2d61 6e64 2d74 6f6c  on/taint-and-tol
+000df930: 6572 6174 696f 6e2f 292e 0a20 2020 2020  eration/)..     
+000df940: 2020 2073 656c 662e 7461 696e 7473 203d     self.taints =
+000df950: 2074 6169 6e74 730a 2020 2020 2020 2020   taints.        
+000df960: 2320 5468 6520 7573 6572 2064 6174 6120  # The user data 
+000df970: 6f66 2074 6865 206e 6f64 6520 706f 6f6c  of the node pool
+000df980: 2e20 466f 7220 6d6f 7265 2069 6e66 6f72  . For more infor
+000df990: 6d61 7469 6f6e 2c20 7365 6520 5b47 656e  mation, see [Gen
+000df9a0: 6572 6174 6520 7573 6572 2d64 6566 696e  erate user-defin
+000df9b0: 6564 2064 6174 615d 2868 7474 7073 3a2f  ed data](https:/
+000df9c0: 2f68 656c 702e 616c 6979 756e 2e63 6f6d  /help.aliyun.com
+000df9d0: 2f64 6f63 756d 656e 745f 6465 7461 696c  /document_detail
+000df9e0: 2f34 3931 3231 2e68 746d 6c29 2e0a 2020  /49121.html)..  
+000df9f0: 2020 2020 2020 7365 6c66 2e75 7365 725f        self.user_
+000dfa00: 6461 7461 203d 2075 7365 725f 6461 7461  data = user_data
+000dfa10: 0a20 2020 2020 2020 2023 2054 6865 2049  .        # The I
+000dfa20: 4473 206f 6620 7468 6520 7653 7769 7463  Ds of the vSwitc
+000dfa30: 6865 732e 2059 6f75 2063 616e 2073 656c  hes. You can sel
+000dfa40: 6563 7420 6f6e 6520 746f 2074 6872 6565  ect one to three
+000dfa50: 2076 5377 6974 6368 6573 2077 6865 6e20   vSwitches when 
+000dfa60: 796f 7520 6372 6561 7465 2061 2063 6c75  you create a clu
+000dfa70: 7374 6572 2e20 5765 2072 6563 6f6d 6d65  ster. We recomme
+000dfa80: 6e64 2074 6861 7420 796f 7520 7365 6c65  nd that you sele
+000dfa90: 6374 2076 5377 6974 6368 6573 2069 6e20  ct vSwitches in 
+000dfaa0: 6469 6666 6572 656e 7420 7a6f 6e65 7320  different zones 
+000dfab0: 746f 2065 6e73 7572 6520 6869 6768 2061  to ensure high a
+000dfac0: 7661 696c 6162 696c 6974 792e 0a20 2020  vailability..   
+000dfad0: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+000dfae0: 2320 5468 6973 2070 6172 616d 6574 6572  # This parameter
+000dfaf0: 2069 7320 7265 7175 6972 6564 2e0a 2020   is required..  
+000dfb00: 2020 2020 2020 7365 6c66 2e76 7377 6974        self.vswit
+000dfb10: 6368 5f69 6473 203d 2076 7377 6974 6368  ch_ids = vswitch
+000dfb20: 5f69 6473 0a20 2020 2020 2020 2023 2053  _ids.        # S
+000dfb30: 7065 6369 6669 6573 2077 6865 7468 6572  pecifies whether
+000dfb40: 2074 6f20 656e 6162 6c65 2061 7574 6f2d   to enable auto-
+000dfb50: 7265 6e65 7761 6c20 666f 7220 776f 726b  renewal for work
+000dfb60: 6572 206e 6f64 6573 2e20 5468 6973 2070  er nodes. This p
+000dfb70: 6172 616d 6574 6572 2074 616b 6573 2065  arameter takes e
+000dfb80: 6666 6563 7420 6f6e 6c79 2069 6620 6077  ffect only if `w
+000dfb90: 6f72 6b65 725f 696e 7374 616e 6365 5f63  orker_instance_c
+000dfba0: 6861 7267 655f 7479 7065 6020 6973 2073  harge_type` is s
+000dfbb0: 6574 2074 6f20 6050 7265 5061 6964 602e  et to `PrePaid`.
+000dfbc0: 2056 616c 6964 2076 616c 7565 733a 0a20   Valid values:. 
+000dfbd0: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+000dfbe0: 2020 2320 2a20 2020 6074 7275 6560 3a20    # *   `true`: 
+000dfbf0: 656e 6162 6c65 7320 6175 746f 2d72 656e  enables auto-ren
+000dfc00: 6577 616c 2e0a 2020 2020 2020 2020 2320  ewal..        # 
+000dfc10: 2a20 2020 6066 616c 7365 603a 2064 6973  *   `false`: dis
+000dfc20: 6162 6c65 7320 6175 746f 2d72 656e 6577  ables auto-renew
+000dfc30: 616c 2e0a 2020 2020 2020 2020 2320 0a20  al..        # . 
+000dfc40: 2020 2020 2020 2023 2044 6566 6175 6c74         # Default
+000dfc50: 2076 616c 7565 3a20 6074 7275 6560 2e0a   value: `true`..
+000dfc60: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+000dfc70: 6b65 725f 6175 746f 5f72 656e 6577 203d  ker_auto_renew =
+000dfc80: 2077 6f72 6b65 725f 6175 746f 5f72 656e   worker_auto_ren
+000dfc90: 6577 0a20 2020 2020 2020 2023 2054 6865  ew.        # The
+000dfca0: 2061 7574 6f2d 7265 6e65 7761 6c20 7065   auto-renewal pe
+000dfcb0: 7269 6f64 2066 6f72 2077 6f72 6b65 7220  riod for worker 
+000dfcc0: 6e6f 6465 7320 6166 7465 7220 7468 6520  nodes after the 
+000dfcd0: 7375 6273 6372 6970 7469 6f6e 7320 6f66  subscriptions of
+000dfce0: 2077 6f72 6b65 7220 6e6f 6465 7320 6578   worker nodes ex
+000dfcf0: 7069 7265 2e20 5468 6973 2070 6172 616d  pire. This param
+000dfd00: 6574 6572 2074 616b 6573 2065 6666 6563  eter takes effec
+000dfd10: 7420 616e 6420 6973 2072 6571 7569 7265  t and is require
+000dfd20: 6420 6f6e 6c79 2069 6620 7468 6520 7375  d only if the su
+000dfd30: 6273 6372 6970 7469 6f6e 2062 696c 6c69  bscription billi
+000dfd40: 6e67 206d 6574 686f 6420 6973 2073 656c  ng method is sel
+000dfd50: 6563 7465 6420 666f 7220 776f 726b 6572  ected for worker
+000dfd60: 206e 6f64 6573 2e0a 2020 2020 2020 2020   nodes..        
+000dfd70: 2320 0a20 2020 2020 2020 2023 2056 616c  # .        # Val
+000dfd80: 6964 2076 616c 7565 733a 2031 2c20 322c  id values: 1, 2,
+000dfd90: 2033 2c20 362c 2061 6e64 2031 322e 0a20   3, 6, and 12.. 
+000dfda0: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+000dfdb0: 2020 2320 4465 6661 756c 7420 7661 6c75    # Default valu
+000dfdc0: 653a 2060 3160 2e0a 2020 2020 2020 2020  e: `1`..        
+000dfdd0: 7365 6c66 2e77 6f72 6b65 725f 6175 746f  self.worker_auto
+000dfde0: 5f72 656e 6577 5f70 6572 696f 6420 3d20  _renew_period = 
+000dfdf0: 776f 726b 6572 5f61 7574 6f5f 7265 6e65  worker_auto_rene
+000dfe00: 775f 7065 7269 6f64 0a20 2020 2020 2020  w_period.       
+000dfe10: 2023 2054 6865 2063 6f6e 6669 6775 7261   # The configura
+000dfe20: 7469 6f6e 206f 6620 7468 6520 6461 7461  tion of the data
+000dfe30: 2064 6973 6b20 7468 6174 2069 7320 6d6f   disk that is mo
+000dfe40: 756e 7465 6420 746f 2077 6f72 6b65 7220  unted to worker 
+000dfe50: 6e6f 6465 732e 2054 6865 2063 6f6e 6669  nodes. The confi
+000dfe60: 6775 7261 7469 6f6e 2069 6e63 6c75 6465  guration include
+000dfe70: 7320 7468 6520 6469 736b 2074 7970 6520  s the disk type 
+000dfe80: 616e 6420 6469 736b 2073 697a 652e 0a20  and disk size.. 
+000dfe90: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
+000dfea0: 6572 5f64 6174 615f 6469 736b 7320 3d20  er_data_disks = 
+000dfeb0: 776f 726b 6572 5f64 6174 615f 6469 736b  worker_data_disk
+000dfec0: 730a 2020 2020 2020 2020 2320 5468 6520  s.        # The 
+000dfed0: 6269 6c6c 696e 6720 6d65 7468 6f64 206f  billing method o
+000dfee0: 6620 776f 726b 6572 206e 6f64 6573 2e20  f worker nodes. 
+000dfef0: 5661 6c69 6420 7661 6c75 6573 3a0a 2020  Valid values:.  
+000dff00: 2020 2020 2020 2320 0a20 2020 2020 2020        # .       
+000dff10: 2023 202a 2020 2060 5072 6550 6169 6460   # *   `PrePaid`
+000dff20: 3a20 7375 6273 6372 6970 7469 6f6e 2e0a  : subscription..
+000dff30: 2020 2020 2020 2020 2320 2a20 2020 6050          # *   `P
+000dff40: 6f73 7450 6169 6460 3a20 7061 792d 6173  ostPaid`: pay-as
+000dff50: 2d79 6f75 2d67 6f2e 0a20 2020 2020 2020  -you-go..       
+000dff60: 2023 200a 2020 2020 2020 2020 2320 4465   # .        # De
+000dff70: 6661 756c 7420 7661 6c75 653a 2060 506f  fault value: `Po
+000dff80: 7374 5061 6964 602e 0a20 2020 2020 2020  stPaid`..       
+000dff90: 2073 656c 662e 776f 726b 6572 5f69 6e73   self.worker_ins
+000dffa0: 7461 6e63 655f 6368 6172 6765 5f74 7970  tance_charge_typ
+000dffb0: 6520 3d20 776f 726b 6572 5f69 6e73 7461  e = worker_insta
+000dffc0: 6e63 655f 6368 6172 6765 5f74 7970 650a  nce_charge_type.
+000dffd0: 2020 2020 2020 2020 2320 5468 6520 696e          # The in
+000dffe0: 7374 616e 6365 2063 6f6e 6669 6775 7261  stance configura
+000dfff0: 7469 6f6e 7320 6f66 2077 6f72 6b65 7220  tions of worker 
+000e0000: 6e6f 6465 732e 0a20 2020 2020 2020 2023  nodes..        #
+000e0010: 200a 2020 2020 2020 2020 2320 5468 6973   .        # This
+000e0020: 2070 6172 616d 6574 6572 2069 7320 7265   parameter is re
+000e0030: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+000e0040: 7365 6c66 2e77 6f72 6b65 725f 696e 7374  self.worker_inst
+000e0050: 616e 6365 5f74 7970 6573 203d 2077 6f72  ance_types = wor
+000e0060: 6b65 725f 696e 7374 616e 6365 5f74 7970  ker_instance_typ
+000e0070: 6573 0a20 2020 2020 2020 2023 2054 6865  es.        # The
+000e0080: 2073 7562 7363 7269 7074 696f 6e20 6475   subscription du
+000e0090: 7261 7469 6f6e 206f 6620 776f 726b 6572  ration of worker
+000e00a0: 206e 6f64 6573 2e20 5468 6973 2070 6172   nodes. This par
+000e00b0: 616d 6574 6572 2074 616b 6573 2065 6666  ameter takes eff
+000e00c0: 6563 7420 616e 6420 6973 2072 6571 7569  ect and is requi
+000e00d0: 7265 6420 6f6e 6c79 2069 6620 6077 6f72  red only if `wor
+000e00e0: 6b65 725f 696e 7374 616e 6365 5f63 6861  ker_instance_cha
+000e00f0: 7267 655f 7479 7065 6020 6973 2073 6574  rge_type` is set
+000e0100: 2074 6f20 6050 7265 5061 6964 602e 0a20   to `PrePaid`.. 
+000e0110: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+000e0120: 2020 2320 5661 6c69 6420 7661 6c75 6573    # Valid values
+000e0130: 3a20 312c 2032 2c20 332c 2036 2c20 3132  : 1, 2, 3, 6, 12
+000e0140: 2c20 3234 2c20 3336 2c20 3438 2c20 616e  , 24, 36, 48, an
+000e0150: 6420 3630 2e0a 2020 2020 2020 2020 2320  d 60..        # 
+000e0160: 0a20 2020 2020 2020 2023 2044 6566 6175  .        # Defau
+000e0170: 6c74 2076 616c 7565 3a20 312e 0a20 2020  lt value: 1..   
+000e0180: 2020 2020 2073 656c 662e 776f 726b 6572       self.worker
+000e0190: 5f70 6572 696f 6420 3d20 776f 726b 6572  _period = worker
+000e01a0: 5f70 6572 696f 640a 2020 2020 2020 2020  _period.        
+000e01b0: 2320 5468 6520 6269 6c6c 696e 6720 6379  # The billing cy
+000e01c0: 636c 6520 6f66 2077 6f72 6b65 7220 6e6f  cle of worker no
+000e01d0: 6465 732e 2054 6869 7320 7061 7261 6d65  des. This parame
+000e01e0: 7465 7220 6973 2072 6571 7569 7265 6420  ter is required 
+000e01f0: 6966 2077 6f72 6b65 725f 696e 7374 616e  if worker_instan
+000e0200: 6365 5f63 6861 7267 655f 7479 7065 2069  ce_charge_type i
+000e0210: 7320 7365 7420 746f 2060 5072 6550 6169  s set to `PrePai
+000e0220: 6460 2e0a 2020 2020 2020 2020 2320 0a20  d`..        # . 
+000e0230: 2020 2020 2020 2023 2053 6574 2074 6865         # Set the
+000e0240: 2076 616c 7565 2074 6f20 604d 6f6e 7468   value to `Month
+000e0250: 602e 2057 6f72 6b65 7220 6e6f 6465 7320  `. Worker nodes 
+000e0260: 6172 6520 6269 6c6c 6564 206f 6e6c 7920  are billed only 
+000e0270: 6f6e 2061 206d 6f6e 7468 6c79 2062 6173  on a monthly bas
+000e0280: 6973 2e0a 2020 2020 2020 2020 7365 6c66  is..        self
+000e0290: 2e77 6f72 6b65 725f 7065 7269 6f64 5f75  .worker_period_u
+000e02a0: 6e69 7420 3d20 776f 726b 6572 5f70 6572  nit = worker_per
+000e02b0: 696f 645f 756e 6974 0a20 2020 2020 2020  iod_unit.       
+000e02c0: 2023 2054 6865 2074 7970 6520 6f66 2073   # The type of s
+000e02d0: 7973 7465 6d20 6469 736b 2074 6861 7420  ystem disk that 
+000e02e0: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
+000e02f0: 666f 7220 776f 726b 6572 206e 6f64 6573  for worker nodes
+000e0300: 2e20 5661 6c69 6420 7661 6c75 6573 3a0a  . Valid values:.
+000e0310: 2020 2020 2020 2020 2320 0a20 2020 2020          # .     
+000e0320: 2020 2023 202a 2020 2060 636c 6f75 645f     # *   `cloud_
+000e0330: 6566 6669 6369 656e 6379 603a 2075 6c74  efficiency`: ult
+000e0340: 7261 2064 6973 6b2e 0a20 2020 2020 2020  ra disk..       
+000e0350: 2023 202a 2020 2060 636c 6f75 645f 7373   # *   `cloud_ss
+000e0360: 6460 3a20 7374 616e 6461 7264 2053 5344  d`: standard SSD
+000e0370: 2e0a 2020 2020 2020 2020 2320 2a20 2020  ..        # *   
+000e0380: 6063 6c6f 7564 5f65 7373 6460 3a20 656e  `cloud_essd`: en
+000e0390: 6861 6e63 6564 2053 5344 2028 4553 5344  hanced SSD (ESSD
+000e03a0: 292e 0a20 2020 2020 2020 2023 200a 2020  )..        # .  
+000e03b0: 2020 2020 2020 2320 4465 6661 756c 7420        # Default 
+000e03c0: 7661 6c75 653a 2060 636c 6f75 645f 7373  value: `cloud_ss
+000e03d0: 6460 2e0a 2020 2020 2020 2020 2320 0a20  d`..        # . 
+000e03e0: 2020 2020 2020 2023 2054 6869 7320 7061         # This pa
+000e03f0: 7261 6d65 7465 7220 6973 2072 6571 7569  rameter is requi
+000e0400: 7265 642e 0a20 2020 2020 2020 2073 656c  red..        sel
+000e0410: 662e 776f 726b 6572 5f73 7973 7465 6d5f  f.worker_system_
+000e0420: 6469 736b 5f63 6174 6567 6f72 7920 3d20  disk_category = 
+000e0430: 776f 726b 6572 5f73 7973 7465 6d5f 6469  worker_system_di
+000e0440: 736b 5f63 6174 6567 6f72 790a 2020 2020  sk_category.    
+000e0450: 2020 2020 2320 5468 6520 7369 7a65 206f      # The size o
+000e0460: 6620 7468 6520 7379 7374 656d 2064 6973  f the system dis
+000e0470: 6b20 7468 6174 2079 6f75 2077 616e 7420  k that you want 
+000e0480: 746f 2075 7365 2066 6f72 2077 6f72 6b65  to use for worke
+000e0490: 7220 6e6f 6465 732e 2055 6e69 743a 2047  r nodes. Unit: G
+000e04a0: 6942 2e0a 2020 2020 2020 2020 2320 0a20  iB..        # . 
+000e04b0: 2020 2020 2020 2023 2056 616c 6964 2076         # Valid v
+000e04c0: 616c 7565 733a 2034 3020 746f 2035 3030  alues: 40 to 500
+000e04d0: 2e0a 2020 2020 2020 2020 2320 0a20 2020  ..        # .   
+000e04e0: 2020 2020 2023 2044 6566 6175 6c74 2076       # Default v
+000e04f0: 616c 7565 3a20 6031 3230 602e 0a20 2020  alue: `120`..   
+000e0500: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+000e0510: 2320 5468 6973 2070 6172 616d 6574 6572  # This parameter
+000e0520: 2069 7320 7265 7175 6972 6564 2e0a 2020   is required..  
+000e0530: 2020 2020 2020 7365 6c66 2e77 6f72 6b65        self.worke
+000e0540: 725f 7379 7374 656d 5f64 6973 6b5f 7369  r_system_disk_si
+000e0550: 7a65 203d 2077 6f72 6b65 725f 7379 7374  ze = worker_syst
+000e0560: 656d 5f64 6973 6b5f 7369 7a65 0a0a 2020  em_disk_size..  
+000e0570: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000e0580: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+000e0590: 2073 656c 662e 7275 6e74 696d 653a 0a20   self.runtime:. 
+000e05a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000e05b0: 7275 6e74 696d 652e 7661 6c69 6461 7465  runtime.validate
+000e05c0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+000e05d0: 6c66 2e74 6167 733a 0a20 2020 2020 2020  lf.tags:.       
+000e05e0: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
+000e05f0: 6c66 2e74 6167 733a 0a20 2020 2020 2020  lf.tags:.       
+000e0600: 2020 2020 2020 2020 2069 6620 6b3a 0a20           if k:. 
+000e0610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000e0620: 2020 206b 2e76 616c 6964 6174 6528 290a     k.validate().
+000e0630: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000e0640: 7461 696e 7473 3a0a 2020 2020 2020 2020  taints:.        
+000e0650: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+000e0660: 662e 7461 696e 7473 3a0a 2020 2020 2020  f.taints:.      
+000e0670: 2020 2020 2020 2020 2020 6966 206b 3a0a            if k:.
+000e0680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000e0690: 2020 2020 6b2e 7661 6c69 6461 7465 2829      k.validate()
+000e06a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000e06b0: 2e77 6f72 6b65 725f 6461 7461 5f64 6973  .worker_data_dis
+000e06c0: 6b73 3a0a 2020 2020 2020 2020 2020 2020  ks:.            
+000e06d0: 666f 7220 6b20 696e 2073 656c 662e 776f  for k in self.wo
+000e06e0: 726b 6572 5f64 6174 615f 6469 736b 733a  rker_data_disks:
+000e06f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000e0700: 2069 6620 6b3a 0a20 2020 2020 2020 2020   if k:.         
+000e0710: 2020 2020 2020 2020 2020 206b 2e76 616c             k.val
+000e0720: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+000e0730: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000e0740: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000e0750: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000e0760: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000e0770: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e0780: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000e0790: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000e07a0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000e07b0: 2020 2020 2069 6620 7365 6c66 2e63 6c6f       if self.clo
+000e07c0: 7564 5f6d 6f6e 6974 6f72 5f66 6c61 6773  ud_monitor_flags
+000e07d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e07e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000e07f0: 5b27 636c 6f75 645f 6d6f 6e69 746f 725f  ['cloud_monitor_
+000e0800: 666c 6167 7327 5d20 3d20 7365 6c66 2e63  flags'] = self.c
+000e0810: 6c6f 7564 5f6d 6f6e 6974 6f72 5f66 6c61  loud_monitor_fla
+000e0820: 6773 0a20 2020 2020 2020 2069 6620 7365  gs.        if se
+000e0830: 6c66 2e63 6f75 6e74 2069 7320 6e6f 7420  lf.count is not 
+000e0840: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e0850: 2020 7265 7375 6c74 5b27 636f 756e 7427    result['count'
+000e0860: 5d20 3d20 7365 6c66 2e63 6f75 6e74 0a20  ] = self.count. 
+000e0870: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000e0880: 7075 5f70 6f6c 6963 7920 6973 206e 6f74  pu_policy is not
+000e0890: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e08a0: 2020 2072 6573 756c 745b 2763 7075 5f70     result['cpu_p
+000e08b0: 6f6c 6963 7927 5d20 3d20 7365 6c66 2e63  olicy'] = self.c
+000e08c0: 7075 5f70 6f6c 6963 790a 2020 2020 2020  pu_policy.      
+000e08d0: 2020 6966 2073 656c 662e 696d 6167 655f    if self.image_
+000e08e0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000e08f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000e0900: 6c74 5b27 696d 6167 655f 6964 275d 203d  lt['image_id'] =
+000e0910: 2073 656c 662e 696d 6167 655f 6964 0a20   self.image_id. 
+000e0920: 2020 2020 2020 2069 6620 7365 6c66 2e6b         if self.k
+000e0930: 6579 5f70 6169 7220 6973 206e 6f74 204e  ey_pair is not N
+000e0940: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e0950: 2072 6573 756c 745b 276b 6579 5f70 6169   result['key_pai
+000e0960: 7227 5d20 3d20 7365 6c66 2e6b 6579 5f70  r'] = self.key_p
+000e0970: 6169 720a 2020 2020 2020 2020 6966 2073  air.        if s
+000e0980: 656c 662e 6c6f 6769 6e5f 7061 7373 776f  elf.login_passwo
+000e0990: 7264 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rd is not None:.
+000e09a0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000e09b0: 6c74 5b27 6c6f 6769 6e5f 7061 7373 776f  lt['login_passwo
+000e09c0: 7264 275d 203d 2073 656c 662e 6c6f 6769  rd'] = self.logi
+000e09d0: 6e5f 7061 7373 776f 7264 0a20 2020 2020  n_password.     
+000e09e0: 2020 2069 6620 7365 6c66 2e72 6473 5f69     if self.rds_i
+000e09f0: 6e73 7461 6e63 6573 2069 7320 6e6f 7420  nstances is not 
+000e0a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e0a10: 2020 7265 7375 6c74 5b27 7264 735f 696e    result['rds_in
+000e0a20: 7374 616e 6365 7327 5d20 3d20 7365 6c66  stances'] = self
+000e0a30: 2e72 6473 5f69 6e73 7461 6e63 6573 0a20  .rds_instances. 
+000e0a40: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+000e0a50: 756e 7469 6d65 2069 7320 6e6f 7420 4e6f  untime is not No
+000e0a60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e0a70: 7265 7375 6c74 5b27 7275 6e74 696d 6527  result['runtime'
+000e0a80: 5d20 3d20 7365 6c66 2e72 756e 7469 6d65  ] = self.runtime
+000e0a90: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000e0aa0: 2020 7265 7375 6c74 5b27 7461 6773 275d    result['tags']
+000e0ab0: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
+000e0ac0: 2073 656c 662e 7461 6773 2069 7320 6e6f   self.tags is no
+000e0ad0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e0ae0: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+000e0af0: 662e 7461 6773 3a0a 2020 2020 2020 2020  f.tags:.        
+000e0b00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e0b10: 7461 6773 275d 2e61 7070 656e 6428 6b2e  tags'].append(k.
+000e0b20: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
+000e0b30: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
+000e0b40: 2072 6573 756c 745b 2774 6169 6e74 7327   result['taints'
+000e0b50: 5d20 3d20 5b5d 0a20 2020 2020 2020 2069  ] = [].        i
+000e0b60: 6620 7365 6c66 2e74 6169 6e74 7320 6973  f self.taints is
+000e0b70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e0b80: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+000e0b90: 7365 6c66 2e74 6169 6e74 733a 0a20 2020  self.taints:.   
+000e0ba0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+000e0bb0: 756c 745b 2774 6169 6e74 7327 5d2e 6170  ult['taints'].ap
+000e0bc0: 7065 6e64 286b 2e74 6f5f 6d61 7028 2920  pend(k.to_map() 
+000e0bd0: 6966 206b 2065 6c73 6520 4e6f 6e65 290a  if k else None).
+000e0be0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000e0bf0: 7573 6572 5f64 6174 6120 6973 206e 6f74  user_data is not
+000e0c00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e0c10: 2020 2072 6573 756c 745b 2775 7365 725f     result['user_
+000e0c20: 6461 7461 275d 203d 2073 656c 662e 7573  data'] = self.us
+000e0c30: 6572 5f64 6174 610a 2020 2020 2020 2020  er_data.        
+000e0c40: 6966 2073 656c 662e 7673 7769 7463 685f  if self.vswitch_
+000e0c50: 6964 7320 6973 206e 6f74 204e 6f6e 653a  ids is not None:
+000e0c60: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000e0c70: 756c 745b 2776 7377 6974 6368 5f69 6473  ult['vswitch_ids
+000e0c80: 275d 203d 2073 656c 662e 7673 7769 7463  '] = self.vswitc
+000e0c90: 685f 6964 730a 2020 2020 2020 2020 6966  h_ids.        if
+000e0ca0: 2073 656c 662e 776f 726b 6572 5f61 7574   self.worker_aut
+000e0cb0: 6f5f 7265 6e65 7720 6973 206e 6f74 204e  o_renew is not N
+000e0cc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e0cd0: 2072 6573 756c 745b 2777 6f72 6b65 725f   result['worker_
+000e0ce0: 6175 746f 5f72 656e 6577 275d 203d 2073  auto_renew'] = s
+000e0cf0: 656c 662e 776f 726b 6572 5f61 7574 6f5f  elf.worker_auto_
+000e0d00: 7265 6e65 770a 2020 2020 2020 2020 6966  renew.        if
+000e0d10: 2073 656c 662e 776f 726b 6572 5f61 7574   self.worker_aut
+000e0d20: 6f5f 7265 6e65 775f 7065 7269 6f64 2069  o_renew_period i
+000e0d30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e0d40: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e0d50: 776f 726b 6572 5f61 7574 6f5f 7265 6e65  worker_auto_rene
+000e0d60: 775f 7065 7269 6f64 275d 203d 2073 656c  w_period'] = sel
+000e0d70: 662e 776f 726b 6572 5f61 7574 6f5f 7265  f.worker_auto_re
+000e0d80: 6e65 775f 7065 7269 6f64 0a20 2020 2020  new_period.     
+000e0d90: 2020 2072 6573 756c 745b 2777 6f72 6b65     result['worke
+000e0da0: 725f 6461 7461 5f64 6973 6b73 275d 203d  r_data_disks'] =
+000e0db0: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
+000e0dc0: 656c 662e 776f 726b 6572 5f64 6174 615f  elf.worker_data_
+000e0dd0: 6469 736b 7320 6973 206e 6f74 204e 6f6e  disks is not Non
+000e0de0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+000e0df0: 6f72 206b 2069 6e20 7365 6c66 2e77 6f72  or k in self.wor
+000e0e00: 6b65 725f 6461 7461 5f64 6973 6b73 3a0a  ker_data_disks:.
+000e0e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000e0e20: 7265 7375 6c74 5b27 776f 726b 6572 5f64  result['worker_d
+000e0e30: 6174 615f 6469 736b 7327 5d2e 6170 7065  ata_disks'].appe
+000e0e40: 6e64 286b 2e74 6f5f 6d61 7028 2920 6966  nd(k.to_map() if
+000e0e50: 206b 2065 6c73 6520 4e6f 6e65 290a 2020   k else None).  
+000e0e60: 2020 2020 2020 6966 2073 656c 662e 776f        if self.wo
+000e0e70: 726b 6572 5f69 6e73 7461 6e63 655f 6368  rker_instance_ch
+000e0e80: 6172 6765 5f74 7970 6520 6973 206e 6f74  arge_type is not
+000e0e90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e0ea0: 2020 2072 6573 756c 745b 2777 6f72 6b65     result['worke
+000e0eb0: 725f 696e 7374 616e 6365 5f63 6861 7267  r_instance_charg
+000e0ec0: 655f 7479 7065 275d 203d 2073 656c 662e  e_type'] = self.
+000e0ed0: 776f 726b 6572 5f69 6e73 7461 6e63 655f  worker_instance_
+000e0ee0: 6368 6172 6765 5f74 7970 650a 2020 2020  charge_type.    
+000e0ef0: 2020 2020 6966 2073 656c 662e 776f 726b      if self.work
+000e0f00: 6572 5f69 6e73 7461 6e63 655f 7479 7065  er_instance_type
+000e0f10: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+000e0f20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000e0f30: 745b 2777 6f72 6b65 725f 696e 7374 616e  t['worker_instan
+000e0f40: 6365 5f74 7970 6573 275d 203d 2073 656c  ce_types'] = sel
+000e0f50: 662e 776f 726b 6572 5f69 6e73 7461 6e63  f.worker_instanc
+000e0f60: 655f 7479 7065 730a 2020 2020 2020 2020  e_types.        
+000e0f70: 6966 2073 656c 662e 776f 726b 6572 5f70  if self.worker_p
+000e0f80: 6572 696f 6420 6973 206e 6f74 204e 6f6e  eriod is not Non
+000e0f90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e0fa0: 6573 756c 745b 2777 6f72 6b65 725f 7065  esult['worker_pe
+000e0fb0: 7269 6f64 275d 203d 2073 656c 662e 776f  riod'] = self.wo
+000e0fc0: 726b 6572 5f70 6572 696f 640a 2020 2020  rker_period.    
+000e0fd0: 2020 2020 6966 2073 656c 662e 776f 726b      if self.work
+000e0fe0: 6572 5f70 6572 696f 645f 756e 6974 2069  er_period_unit i
+000e0ff0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e1000: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e1010: 776f 726b 6572 5f70 6572 696f 645f 756e  worker_period_un
+000e1020: 6974 275d 203d 2073 656c 662e 776f 726b  it'] = self.work
+000e1030: 6572 5f70 6572 696f 645f 756e 6974 0a20  er_period_unit. 
+000e1040: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
+000e1050: 6f72 6b65 725f 7379 7374 656d 5f64 6973  orker_system_dis
+000e1060: 6b5f 6361 7465 676f 7279 2069 7320 6e6f  k_category is no
+000e1070: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e1080: 2020 2020 7265 7375 6c74 5b27 776f 726b      result['work
+000e1090: 6572 5f73 7973 7465 6d5f 6469 736b 5f63  er_system_disk_c
+000e10a0: 6174 6567 6f72 7927 5d20 3d20 7365 6c66  ategory'] = self
+000e10b0: 2e77 6f72 6b65 725f 7379 7374 656d 5f64  .worker_system_d
+000e10c0: 6973 6b5f 6361 7465 676f 7279 0a20 2020  isk_category.   
+000e10d0: 2020 2020 2069 6620 7365 6c66 2e77 6f72       if self.wor
+000e10e0: 6b65 725f 7379 7374 656d 5f64 6973 6b5f  ker_system_disk_
+000e10f0: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
+000e1100: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000e1110: 7375 6c74 5b27 776f 726b 6572 5f73 7973  sult['worker_sys
+000e1120: 7465 6d5f 6469 736b 5f73 697a 6527 5d20  tem_disk_size'] 
+000e1130: 3d20 7365 6c66 2e77 6f72 6b65 725f 7379  = self.worker_sy
+000e1140: 7374 656d 5f64 6973 6b5f 7369 7a65 0a20  stem_disk_size. 
+000e1150: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000e1160: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000e1170: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000e1180: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000e1190: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000e11a0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000e11b0: 206d 2e67 6574 2827 636c 6f75 645f 6d6f   m.get('cloud_mo
+000e11c0: 6e69 746f 725f 666c 6167 7327 2920 6973  nitor_flags') is
+000e11d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e11e0: 2020 2020 2020 2073 656c 662e 636c 6f75         self.clou
+000e11f0: 645f 6d6f 6e69 746f 725f 666c 6167 7320  d_monitor_flags 
+000e1200: 3d20 6d2e 6765 7428 2763 6c6f 7564 5f6d  = m.get('cloud_m
+000e1210: 6f6e 6974 6f72 5f66 6c61 6773 2729 0a20  onitor_flags'). 
+000e1220: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000e1230: 2763 6f75 6e74 2729 2069 7320 6e6f 7420  'count') is not 
+000e1240: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e1250: 2020 7365 6c66 2e63 6f75 6e74 203d 206d    self.count = m
+000e1260: 2e67 6574 2827 636f 756e 7427 290a 2020  .get('count').  
+000e1270: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000e1280: 6370 755f 706f 6c69 6379 2729 2069 7320  cpu_policy') is 
+000e1290: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e12a0: 2020 2020 2020 7365 6c66 2e63 7075 5f70        self.cpu_p
+000e12b0: 6f6c 6963 7920 3d20 6d2e 6765 7428 2763  olicy = m.get('c
+000e12c0: 7075 5f70 6f6c 6963 7927 290a 2020 2020  pu_policy').    
+000e12d0: 2020 2020 6966 206d 2e67 6574 2827 696d      if m.get('im
+000e12e0: 6167 655f 6964 2729 2069 7320 6e6f 7420  age_id') is not 
+000e12f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e1300: 2020 7365 6c66 2e69 6d61 6765 5f69 6420    self.image_id 
+000e1310: 3d20 6d2e 6765 7428 2769 6d61 6765 5f69  = m.get('image_i
+000e1320: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+000e1330: 2e67 6574 2827 6b65 795f 7061 6972 2729  .get('key_pair')
+000e1340: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e1350: 2020 2020 2020 2020 2020 7365 6c66 2e6b            self.k
+000e1360: 6579 5f70 6169 7220 3d20 6d2e 6765 7428  ey_pair = m.get(
+000e1370: 276b 6579 5f70 6169 7227 290a 2020 2020  'key_pair').    
+000e1380: 2020 2020 6966 206d 2e67 6574 2827 6c6f      if m.get('lo
+000e1390: 6769 6e5f 7061 7373 776f 7264 2729 2069  gin_password') i
+000e13a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e13b0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
+000e13c0: 696e 5f70 6173 7377 6f72 6420 3d20 6d2e  in_password = m.
+000e13d0: 6765 7428 276c 6f67 696e 5f70 6173 7377  get('login_passw
+000e13e0: 6f72 6427 290a 2020 2020 2020 2020 6966  ord').        if
+000e13f0: 206d 2e67 6574 2827 7264 735f 696e 7374   m.get('rds_inst
+000e1400: 616e 6365 7327 2920 6973 206e 6f74 204e  ances') is not N
+000e1410: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e1420: 2073 656c 662e 7264 735f 696e 7374 616e   self.rds_instan
+000e1430: 6365 7320 3d20 6d2e 6765 7428 2772 6473  ces = m.get('rds
+000e1440: 5f69 6e73 7461 6e63 6573 2729 0a20 2020  _instances').   
+000e1450: 2020 2020 2069 6620 6d2e 6765 7428 2772       if m.get('r
+000e1460: 756e 7469 6d65 2729 2069 7320 6e6f 7420  untime') is not 
+000e1470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e1480: 2020 7465 6d70 5f6d 6f64 656c 203d 2052    temp_model = R
+000e1490: 756e 7469 6d65 2829 0a20 2020 2020 2020  untime().       
+000e14a0: 2020 2020 2073 656c 662e 7275 6e74 696d       self.runtim
+000e14b0: 6520 3d20 7465 6d70 5f6d 6f64 656c 2e66  e = temp_model.f
+000e14c0: 726f 6d5f 6d61 7028 6d5b 2772 756e 7469  rom_map(m['runti
+000e14d0: 6d65 275d 290a 2020 2020 2020 2020 7365  me']).        se
+000e14e0: 6c66 2e74 6167 7320 3d20 5b5d 0a20 2020  lf.tags = [].   
+000e14f0: 2020 2020 2069 6620 6d2e 6765 7428 2774       if m.get('t
+000e1500: 6167 7327 2920 6973 206e 6f74 204e 6f6e  ags') is not Non
+000e1510: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+000e1520: 6f72 206b 2069 6e20 6d2e 6765 7428 2774  or k in m.get('t
+000e1530: 6167 7327 293a 0a20 2020 2020 2020 2020  ags'):.         
+000e1540: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000e1550: 6c20 3d20 5461 6728 290a 2020 2020 2020  l = Tag().      
+000e1560: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000e1570: 6167 732e 6170 7065 6e64 2874 656d 705f  ags.append(temp_
+000e1580: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286b  model.from_map(k
+000e1590: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000e15a0: 7461 696e 7473 203d 205b 5d0a 2020 2020  taints = [].    
+000e15b0: 2020 2020 6966 206d 2e67 6574 2827 7461      if m.get('ta
+000e15c0: 696e 7473 2729 2069 7320 6e6f 7420 4e6f  ints') is not No
+000e15d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e15e0: 666f 7220 6b20 696e 206d 2e67 6574 2827  for k in m.get('
+000e15f0: 7461 696e 7473 2729 3a0a 2020 2020 2020  taints'):.      
+000e1600: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+000e1610: 6f64 656c 203d 2054 6169 6e74 2829 0a20  odel = Taint(). 
+000e1620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000e1630: 656c 662e 7461 696e 7473 2e61 7070 656e  elf.taints.appen
+000e1640: 6428 7465 6d70 5f6d 6f64 656c 2e66 726f  d(temp_model.fro
+000e1650: 6d5f 6d61 7028 6b29 290a 2020 2020 2020  m_map(k)).      
+000e1660: 2020 6966 206d 2e67 6574 2827 7573 6572    if m.get('user
+000e1670: 5f64 6174 6127 2920 6973 206e 6f74 204e  _data') is not N
+000e1680: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e1690: 2073 656c 662e 7573 6572 5f64 6174 6120   self.user_data 
+000e16a0: 3d20 6d2e 6765 7428 2775 7365 725f 6461  = m.get('user_da
+000e16b0: 7461 2729 0a20 2020 2020 2020 2069 6620  ta').        if 
+000e16c0: 6d2e 6765 7428 2776 7377 6974 6368 5f69  m.get('vswitch_i
+000e16d0: 6473 2729 2069 7320 6e6f 7420 4e6f 6e65  ds') is not None
+000e16e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000e16f0: 6c66 2e76 7377 6974 6368 5f69 6473 203d  lf.vswitch_ids =
+000e1700: 206d 2e67 6574 2827 7673 7769 7463 685f   m.get('vswitch_
+000e1710: 6964 7327 290a 2020 2020 2020 2020 6966  ids').        if
+000e1720: 206d 2e67 6574 2827 776f 726b 6572 5f61   m.get('worker_a
+000e1730: 7574 6f5f 7265 6e65 7727 2920 6973 206e  uto_renew') is n
+000e1740: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e1750: 2020 2020 2073 656c 662e 776f 726b 6572       self.worker
+000e1760: 5f61 7574 6f5f 7265 6e65 7720 3d20 6d2e  _auto_renew = m.
+000e1770: 6765 7428 2777 6f72 6b65 725f 6175 746f  get('worker_auto
+000e1780: 5f72 656e 6577 2729 0a20 2020 2020 2020  _renew').       
+000e1790: 2069 6620 6d2e 6765 7428 2777 6f72 6b65   if m.get('worke
+000e17a0: 725f 6175 746f 5f72 656e 6577 5f70 6572  r_auto_renew_per
+000e17b0: 696f 6427 2920 6973 206e 6f74 204e 6f6e  iod') is not Non
+000e17c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000e17d0: 656c 662e 776f 726b 6572 5f61 7574 6f5f  elf.worker_auto_
+000e17e0: 7265 6e65 775f 7065 7269 6f64 203d 206d  renew_period = m
+000e17f0: 2e67 6574 2827 776f 726b 6572 5f61 7574  .get('worker_aut
+000e1800: 6f5f 7265 6e65 775f 7065 7269 6f64 2729  o_renew_period')
+000e1810: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
+000e1820: 726b 6572 5f64 6174 615f 6469 736b 7320  rker_data_disks 
+000e1830: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
+000e1840: 6d2e 6765 7428 2777 6f72 6b65 725f 6461  m.get('worker_da
+000e1850: 7461 5f64 6973 6b73 2729 2069 7320 6e6f  ta_disks') is no
+000e1860: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e1870: 2020 2020 666f 7220 6b20 696e 206d 2e67      for k in m.g
+000e1880: 6574 2827 776f 726b 6572 5f64 6174 615f  et('worker_data_
+000e1890: 6469 736b 7327 293a 0a20 2020 2020 2020  disks'):.       
+000e18a0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+000e18b0: 6465 6c20 3d20 5363 616c 654f 7574 436c  del = ScaleOutCl
+000e18c0: 7573 7465 7252 6571 7565 7374 576f 726b  usterRequestWork
+000e18d0: 6572 4461 7461 4469 736b 7328 290a 2020  erDataDisks().  
+000e18e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000e18f0: 6c66 2e77 6f72 6b65 725f 6461 7461 5f64  lf.worker_data_d
+000e1900: 6973 6b73 2e61 7070 656e 6428 7465 6d70  isks.append(temp
+000e1910: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+000e1920: 6b29 290a 2020 2020 2020 2020 6966 206d  k)).        if m
+000e1930: 2e67 6574 2827 776f 726b 6572 5f69 6e73  .get('worker_ins
+000e1940: 7461 6e63 655f 6368 6172 6765 5f74 7970  tance_charge_typ
+000e1950: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+000e1960: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000e1970: 662e 776f 726b 6572 5f69 6e73 7461 6e63  f.worker_instanc
+000e1980: 655f 6368 6172 6765 5f74 7970 6520 3d20  e_charge_type = 
+000e1990: 6d2e 6765 7428 2777 6f72 6b65 725f 696e  m.get('worker_in
+000e19a0: 7374 616e 6365 5f63 6861 7267 655f 7479  stance_charge_ty
+000e19b0: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
+000e19c0: 6d2e 6765 7428 2777 6f72 6b65 725f 696e  m.get('worker_in
+000e19d0: 7374 616e 6365 5f74 7970 6573 2729 2069  stance_types') i
+000e19e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e19f0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+000e1a00: 6b65 725f 696e 7374 616e 6365 5f74 7970  ker_instance_typ
+000e1a10: 6573 203d 206d 2e67 6574 2827 776f 726b  es = m.get('work
+000e1a20: 6572 5f69 6e73 7461 6e63 655f 7479 7065  er_instance_type
+000e1a30: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000e1a40: 2e67 6574 2827 776f 726b 6572 5f70 6572  .get('worker_per
+000e1a50: 696f 6427 2920 6973 206e 6f74 204e 6f6e  iod') is not Non
+000e1a60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000e1a70: 656c 662e 776f 726b 6572 5f70 6572 696f  elf.worker_perio
+000e1a80: 6420 3d20 6d2e 6765 7428 2777 6f72 6b65  d = m.get('worke
+000e1a90: 725f 7065 7269 6f64 2729 0a20 2020 2020  r_period').     
+000e1aa0: 2020 2069 6620 6d2e 6765 7428 2777 6f72     if m.get('wor
+000e1ab0: 6b65 725f 7065 7269 6f64 5f75 6e69 7427  ker_period_unit'
+000e1ac0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000e1ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000e1ae0: 776f 726b 6572 5f70 6572 696f 645f 756e  worker_period_un
+000e1af0: 6974 203d 206d 2e67 6574 2827 776f 726b  it = m.get('work
+000e1b00: 6572 5f70 6572 696f 645f 756e 6974 2729  er_period_unit')
+000e1b10: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000e1b20: 7428 2777 6f72 6b65 725f 7379 7374 656d  t('worker_system
+000e1b30: 5f64 6973 6b5f 6361 7465 676f 7279 2729  _disk_category')
+000e1b40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e1b50: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+000e1b60: 6f72 6b65 725f 7379 7374 656d 5f64 6973  orker_system_dis
+000e1b70: 6b5f 6361 7465 676f 7279 203d 206d 2e67  k_category = m.g
+000e1b80: 6574 2827 776f 726b 6572 5f73 7973 7465  et('worker_syste
+000e1b90: 6d5f 6469 736b 5f63 6174 6567 6f72 7927  m_disk_category'
+000e1ba0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000e1bb0: 6574 2827 776f 726b 6572 5f73 7973 7465  et('worker_syste
+000e1bc0: 6d5f 6469 736b 5f73 697a 6527 2920 6973  m_disk_size') is
+000e1bd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e1be0: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
+000e1bf0: 6572 5f73 7973 7465 6d5f 6469 736b 5f73  er_system_disk_s
+000e1c00: 697a 6520 3d20 6d2e 6765 7428 2777 6f72  ize = m.get('wor
+000e1c10: 6b65 725f 7379 7374 656d 5f64 6973 6b5f  ker_system_disk_
+000e1c20: 7369 7a65 2729 0a20 2020 2020 2020 2072  size').        r
+000e1c30: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000e1c40: 7373 2053 6361 6c65 4f75 7443 6c75 7374  ss ScaleOutClust
+000e1c50: 6572 5265 7370 6f6e 7365 426f 6479 2854  erResponseBody(T
+000e1c60: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000e1c70: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000e1c80: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000e1c90: 2020 636c 7573 7465 725f 6964 3a20 7374    cluster_id: st
+000e1ca0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000e1cb0: 2020 7265 7175 6573 745f 6964 3a20 7374    request_id: st
+000e1cc0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000e1cd0: 2020 7461 736b 5f69 643a 2073 7472 203d    task_id: str =
+000e1ce0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000e1cf0: 2020 2020 2020 2320 5468 6520 636c 7573        # The clus
+000e1d00: 7465 7220 4944 2e0a 2020 2020 2020 2020  ter ID..        
+000e1d10: 7365 6c66 2e63 6c75 7374 6572 5f69 6420  self.cluster_id 
+000e1d20: 3d20 636c 7573 7465 725f 6964 0a20 2020  = cluster_id.   
+000e1d30: 2020 2020 2023 2054 6865 2072 6571 7565       # The reque
+000e1d40: 7374 2049 442e 0a20 2020 2020 2020 2073  st ID..        s
+000e1d50: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+000e1d60: 2072 6571 7565 7374 5f69 640a 2020 2020   request_id.    
+000e1d70: 2020 2020 2320 5468 6520 7461 736b 2049      # The task I
+000e1d80: 442e 0a20 2020 2020 2020 2073 656c 662e  D..        self.
+000e1d90: 7461 736b 5f69 6420 3d20 7461 736b 5f69  task_id = task_i
+000e1da0: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
+000e1db0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000e1dc0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000e1dd0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000e1de0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000e1df0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000e1e00: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000e1e10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e1e20: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000e1e30: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000e1e40: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000e1e50: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
+000e1e60: 7374 6572 5f69 6420 6973 206e 6f74 204e  ster_id is not N
 000e1e70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e1e80: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-000e1e90: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000e1ea0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000e1eb0: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-000e1ec0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e1ed0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000e1ee0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-000e1ef0: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-000e1f00: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000e1f10: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-000e1f20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e1f30: 2020 7465 6d70 5f6d 6f64 656c 203d 2053    temp_model = S
-000e1f40: 6361 6c65 4f75 7443 6c75 7374 6572 5265  caleOutClusterRe
-000e1f50: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
-000e1f60: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-000e1f70: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-000e1f80: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-000e1f90: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-000e1fa0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000e1fb0: 5363 616e 436c 7573 7465 7256 756c 7352  ScanClusterVulsR
-000e1fc0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-000e1fd0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000e1fe0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000e1ff0: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-000e2000: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
-000e2010: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
-000e2020: 6173 6b5f 6964 3a20 7374 7220 3d20 4e6f  ask_id: str = No
-000e2030: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-000e2040: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-000e2050: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
-000e2060: 2020 2020 2020 2020 7365 6c66 2e74 6173          self.tas
-000e2070: 6b5f 6964 203d 2074 6173 6b5f 6964 0a0a  k_id = task_id..
-000e2080: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000e2090: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e20a0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-000e20b0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-000e20c0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-000e20d0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-000e20e0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-000e20f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e2100: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-000e2110: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000e2120: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000e2130: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-000e2140: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-000e2150: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e2160: 7375 6c74 5b27 7265 7175 6573 745f 6964  sult['request_id
-000e2170: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-000e2180: 745f 6964 0a20 2020 2020 2020 2069 6620  t_id.        if 
-000e2190: 7365 6c66 2e74 6173 6b5f 6964 2069 7320  self.task_id is 
-000e21a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e21b0: 2020 2020 2020 7265 7375 6c74 5b27 7461        result['ta
-000e21c0: 736b 5f69 6427 5d20 3d20 7365 6c66 2e74  sk_id'] = self.t
-000e21d0: 6173 6b5f 6964 0a20 2020 2020 2020 2072  ask_id.        r
-000e21e0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000e21f0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000e2200: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000e2210: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000e2220: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000e2230: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e2240: 7265 7175 6573 745f 6964 2729 2069 7320  request_id') is 
-000e2250: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e2260: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-000e2270: 7374 5f69 6420 3d20 6d2e 6765 7428 2772  st_id = m.get('r
-000e2280: 6571 7565 7374 5f69 6427 290a 2020 2020  equest_id').    
-000e2290: 2020 2020 6966 206d 2e67 6574 2827 7461      if m.get('ta
-000e22a0: 736b 5f69 6427 2920 6973 206e 6f74 204e  sk_id') is not N
-000e22b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e22c0: 2073 656c 662e 7461 736b 5f69 6420 3d20   self.task_id = 
-000e22d0: 6d2e 6765 7428 2774 6173 6b5f 6964 2729  m.get('task_id')
-000e22e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000e22f0: 7365 6c66 0a0a 0a63 6c61 7373 2053 6361  self...class Sca
-000e2300: 6e43 6c75 7374 6572 5675 6c73 5265 7370  nClusterVulsResp
-000e2310: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-000e2320: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000e2330: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000e2340: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-000e2350: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-000e2360: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000e2370: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-000e2380: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000e2390: 2062 6f64 793a 2053 6361 6e43 6c75 7374   body: ScanClust
-000e23a0: 6572 5675 6c73 5265 7370 6f6e 7365 426f  erVulsResponseBo
-000e23b0: 6479 203d 204e 6f6e 652c 0a20 2020 2029  dy = None,.    )
-000e23c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-000e23d0: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-000e23e0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-000e23f0: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
-000e2400: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-000e2410: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-000e2420: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000e2430: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000e2440: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-000e2450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e2460: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-000e2470: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000e2480: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e2490: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000e24a0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000e24b0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000e24c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e24d0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000e24e0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000e24f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000e2500: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-000e2510: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e2520: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-000e2530: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-000e2540: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-000e2550: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-000e2560: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-000e2570: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000e2580: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-000e2590: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-000e25a0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-000e25b0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-000e25c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e25d0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-000e25e0: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-000e25f0: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-000e2600: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000e2610: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000e2620: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000e2630: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000e2640: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000e2650: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e2660: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-000e2670: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e2680: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-000e2690: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-000e26a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000e26b0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-000e26c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000e26d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000e26e0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-000e26f0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-000e2700: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000e2710: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-000e2720: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e2730: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-000e2740: 2053 6361 6e43 6c75 7374 6572 5675 6c73   ScanClusterVuls
-000e2750: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
-000e2760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000e2770: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
-000e2780: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
-000e2790: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
-000e27a0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000e27b0: 7320 5374 6172 7441 6c65 7274 5265 7175  s StartAlertRequ
-000e27c0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-000e27d0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000e27e0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000e27f0: 2020 2020 2020 2061 6c65 7274 5f72 756c         alert_rul
-000e2800: 655f 6772 6f75 705f 6e61 6d65 3a20 7374  e_group_name: st
-000e2810: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000e2820: 2020 616c 6572 745f 7275 6c65 5f6e 616d    alert_rule_nam
-000e2830: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-000e2840: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000e2850: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-000e2860: 616c 6572 7420 7275 6c65 2073 6574 2074  alert rule set t
-000e2870: 6f20 6265 2065 6e61 626c 6564 2e0a 2020  o be enabled..  
-000e2880: 2020 2020 2020 7365 6c66 2e61 6c65 7274        self.alert
-000e2890: 5f72 756c 655f 6772 6f75 705f 6e61 6d65  _rule_group_name
-000e28a0: 203d 2061 6c65 7274 5f72 756c 655f 6772   = alert_rule_gr
-000e28b0: 6f75 705f 6e61 6d65 0a20 2020 2020 2020  oup_name.       
-000e28c0: 2023 2054 6865 206e 616d 6520 6f66 2074   # The name of t
-000e28d0: 6865 2061 6c65 7274 2072 756c 6520 746f  he alert rule to
-000e28e0: 2062 6520 656e 6162 6c65 642e 2049 6620   be enabled. If 
-000e28f0: 796f 7520 646f 206e 6f74 2073 7065 6369  you do not speci
-000e2900: 6679 2061 6e20 616c 6572 7420 7275 6c65  fy an alert rule
-000e2910: 206e 616d 652c 2074 6865 2061 6c65 7274   name, the alert
-000e2920: 2072 756c 6520 7365 7420 6973 2065 6e61   rule set is ena
-000e2930: 626c 6564 2e0a 2020 2020 2020 2020 7365  bled..        se
-000e2940: 6c66 2e61 6c65 7274 5f72 756c 655f 6e61  lf.alert_rule_na
-000e2950: 6d65 203d 2061 6c65 7274 5f72 756c 655f  me = alert_rule_
-000e2960: 6e61 6d65 0a0a 2020 2020 6465 6620 7661  name..    def va
-000e2970: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000e2980: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000e2990: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000e29a0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000e29b0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-000e29c0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-000e29d0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000e29e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000e29f0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-000e2a00: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000e2a10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000e2a20: 616c 6572 745f 7275 6c65 5f67 726f 7570  alert_rule_group
-000e2a30: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
-000e2a40: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e2a50: 6573 756c 745b 2761 6c65 7274 5f72 756c  esult['alert_rul
-000e2a60: 655f 6772 6f75 705f 6e61 6d65 275d 203d  e_group_name'] =
-000e2a70: 2073 656c 662e 616c 6572 745f 7275 6c65   self.alert_rule
-000e2a80: 5f67 726f 7570 5f6e 616d 650a 2020 2020  _group_name.    
-000e2a90: 2020 2020 6966 2073 656c 662e 616c 6572      if self.aler
-000e2aa0: 745f 7275 6c65 5f6e 616d 6520 6973 206e  t_rule_name is n
-000e2ab0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e2ac0: 2020 2020 2072 6573 756c 745b 2761 6c65       result['ale
-000e2ad0: 7274 5f72 756c 655f 6e61 6d65 275d 203d  rt_rule_name'] =
-000e2ae0: 2073 656c 662e 616c 6572 745f 7275 6c65   self.alert_rule
-000e2af0: 5f6e 616d 650a 2020 2020 2020 2020 7265  _name.        re
-000e2b00: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-000e2b10: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-000e2b20: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-000e2b30: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-000e2b40: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-000e2b50: 2020 2020 2069 6620 6d2e 6765 7428 2761       if m.get('a
-000e2b60: 6c65 7274 5f72 756c 655f 6772 6f75 705f  lert_rule_group_
-000e2b70: 6e61 6d65 2729 2069 7320 6e6f 7420 4e6f  name') is not No
-000e2b80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e2b90: 7365 6c66 2e61 6c65 7274 5f72 756c 655f  self.alert_rule_
-000e2ba0: 6772 6f75 705f 6e61 6d65 203d 206d 2e67  group_name = m.g
-000e2bb0: 6574 2827 616c 6572 745f 7275 6c65 5f67  et('alert_rule_g
-000e2bc0: 726f 7570 5f6e 616d 6527 290a 2020 2020  roup_name').    
-000e2bd0: 2020 2020 6966 206d 2e67 6574 2827 616c      if m.get('al
-000e2be0: 6572 745f 7275 6c65 5f6e 616d 6527 2920  ert_rule_name') 
-000e2bf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e2c00: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000e2c10: 6572 745f 7275 6c65 5f6e 616d 6520 3d20  ert_rule_name = 
-000e2c20: 6d2e 6765 7428 2761 6c65 7274 5f72 756c  m.get('alert_rul
-000e2c30: 655f 6e61 6d65 2729 0a20 2020 2020 2020  e_name').       
-000e2c40: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000e2c50: 6c61 7373 2053 7461 7274 416c 6572 7452  lass StartAlertR
-000e2c60: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-000e2c70: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000e2c80: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000e2c90: 2073 656c 662c 0a20 2020 2020 2020 206d   self,.        m
-000e2ca0: 7367 3a20 7374 7220 3d20 4e6f 6e65 2c0a  sg: str = None,.
-000e2cb0: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
-000e2cc0: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
-000e2cd0: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
-000e2ce0: 6520 6d65 7373 6167 6520 7265 7475 726e  e message return
-000e2cf0: 6564 2e0a 2020 2020 2020 2020 7365 6c66  ed..        self
-000e2d00: 2e6d 7367 203d 206d 7367 0a20 2020 2020  .msg = msg.     
-000e2d10: 2020 2023 2054 6865 2073 7461 7475 732e     # The status.
-000e2d20: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-000e2d30: 6174 7573 203d 2073 7461 7475 730a 0a20  atus = status.. 
-000e2d40: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-000e2d50: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-000e2d60: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-000e2d70: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-000e2d80: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-000e2d90: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-000e2da0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000e2db0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e2dc0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000e2dd0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000e2de0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000e2df0: 2069 6620 7365 6c66 2e6d 7367 2069 7320   if self.msg is 
-000e2e00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e2e10: 2020 2020 2020 7265 7375 6c74 5b27 6d73        result['ms
-000e2e20: 6727 5d20 3d20 7365 6c66 2e6d 7367 0a20  g'] = self.msg. 
-000e2e30: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-000e2e40: 7461 7475 7320 6973 206e 6f74 204e 6f6e  tatus is not Non
-000e2e50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e2e60: 6573 756c 745b 2773 7461 7475 7327 5d20  esult['status'] 
-000e2e70: 3d20 7365 6c66 2e73 7461 7475 730a 2020  = self.status.  
-000e2e80: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000e2e90: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-000e2ea0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-000e2eb0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-000e2ec0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-000e2ed0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000e2ee0: 6d2e 6765 7428 276d 7367 2729 2069 7320  m.get('msg') is 
-000e2ef0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e2f00: 2020 2020 2020 7365 6c66 2e6d 7367 203d        self.msg =
-000e2f10: 206d 2e67 6574 2827 6d73 6727 290a 2020   m.get('msg').  
-000e2f20: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e2f30: 7374 6174 7573 2729 2069 7320 6e6f 7420  status') is not 
-000e2f40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e2f50: 2020 7365 6c66 2e73 7461 7475 7320 3d20    self.status = 
-000e2f60: 6d2e 6765 7428 2773 7461 7475 7327 290a  m.get('status').
-000e2f70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000e2f80: 656c 660a 0a0a 636c 6173 7320 5374 6172  elf...class Star
-000e2f90: 7441 6c65 7274 5265 7370 6f6e 7365 2854  tAlertResponse(T
-000e2fa0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-000e2fb0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-000e2fc0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000e2fd0: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
-000e2fe0: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
-000e2ff0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
-000e3000: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
-000e3010: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
-000e3020: 2053 7461 7274 416c 6572 7452 6573 706f   StartAlertRespo
-000e3030: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-000e3040: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-000e3050: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-000e3060: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-000e3070: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-000e3080: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-000e3090: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-000e30a0: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-000e30b0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000e30c0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000e30d0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-000e30e0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-000e30f0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-000e3100: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-000e3110: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-000e3120: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-000e3130: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000e3140: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e3150: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000e3160: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000e3170: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000e3180: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-000e3190: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-000e31a0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000e31b0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-000e31c0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-000e31d0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-000e31e0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-000e31f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e3200: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-000e3210: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-000e3220: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-000e3230: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-000e3240: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e3250: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000e3260: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-000e3270: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-000e3280: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000e3290: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000e32a0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000e32b0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000e32c0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000e32d0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000e32e0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-000e32f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e3300: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000e3310: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-000e3320: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-000e3330: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-000e3340: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-000e3350: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e3360: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000e3370: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-000e3380: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-000e3390: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-000e33a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e33b0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000e33c0: 6465 6c20 3d20 5374 6172 7441 6c65 7274  del = StartAlert
-000e33d0: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
-000e33e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000e33f0: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
-000e3400: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
-000e3410: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
-000e3420: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000e3430: 7320 5374 6172 7457 6f72 6b66 6c6f 7752  s StartWorkflowR
-000e3440: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-000e3450: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000e3460: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000e3470: 2c0a 2020 2020 2020 2020 6d61 7070 696e  ,.        mappin
-000e3480: 675f 6261 6d5f 6f75 745f 6669 6c65 6e61  g_bam_out_filena
-000e3490: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-000e34a0: 2020 2020 2020 2020 6d61 7070 696e 675f          mapping_
-000e34b0: 6261 6d5f 6f75 745f 7061 7468 3a20 7374  bam_out_path: st
-000e34c0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000e34d0: 2020 6d61 7070 696e 675f 6275 636b 6574    mapping_bucket
-000e34e0: 5f6e 616d 653a 2073 7472 203d 204e 6f6e  _name: str = Non
-000e34f0: 652c 0a20 2020 2020 2020 206d 6170 7069  e,.        mappi
-000e3500: 6e67 5f66 6173 7471 5f66 6972 7374 5f66  ng_fastq_first_f
-000e3510: 696c 656e 616d 653a 2073 7472 203d 204e  ilename: str = N
-000e3520: 6f6e 652c 0a20 2020 2020 2020 206d 6170  one,.        map
-000e3530: 7069 6e67 5f66 6173 7471 5f70 6174 683a  ping_fastq_path:
-000e3540: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000e3550: 2020 2020 206d 6170 7069 6e67 5f66 6173       mapping_fas
-000e3560: 7471 5f73 6563 6f6e 645f 6669 6c65 6e61  tq_second_filena
-000e3570: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-000e3580: 2020 2020 2020 2020 6d61 7070 696e 675f          mapping_
-000e3590: 6973 5f6d 6172 6b5f 6475 703a 2073 7472  is_mark_dup: str
-000e35a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000e35b0: 206d 6170 7069 6e67 5f6f 7373 5f72 6567   mapping_oss_reg
-000e35c0: 696f 6e3a 2073 7472 203d 204e 6f6e 652c  ion: str = None,
-000e35d0: 0a20 2020 2020 2020 206d 6170 7069 6e67  .        mapping
-000e35e0: 5f72 6566 6572 656e 6365 5f70 6174 683a  _reference_path:
-000e35f0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000e3600: 2020 2020 2073 6572 7669 6365 3a20 7374       service: st
-000e3610: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000e3620: 2020 7767 735f 6275 636b 6574 5f6e 616d    wgs_bucket_nam
-000e3630: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-000e3640: 2020 2020 2020 2077 6773 5f66 6173 7471         wgs_fastq
-000e3650: 5f66 6972 7374 5f66 696c 656e 616d 653a  _first_filename:
-000e3660: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000e3670: 2020 2020 2077 6773 5f66 6173 7471 5f70       wgs_fastq_p
-000e3680: 6174 683a 2073 7472 203d 204e 6f6e 652c  ath: str = None,
-000e3690: 0a20 2020 2020 2020 2077 6773 5f66 6173  .        wgs_fas
-000e36a0: 7471 5f73 6563 6f6e 645f 6669 6c65 6e61  tq_second_filena
-000e36b0: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-000e36c0: 2020 2020 2020 2020 7767 735f 6f73 735f          wgs_oss_
-000e36d0: 7265 6769 6f6e 3a20 7374 7220 3d20 4e6f  region: str = No
-000e36e0: 6e65 2c0a 2020 2020 2020 2020 7767 735f  ne,.        wgs_
-000e36f0: 7265 6665 7265 6e63 655f 7061 7468 3a20  reference_path: 
-000e3700: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000e3710: 2020 2020 7767 735f 7663 665f 6f75 745f      wgs_vcf_out_
-000e3720: 6669 6c65 6e61 6d65 3a20 7374 7220 3d20  filename: str = 
-000e3730: 4e6f 6e65 2c0a 2020 2020 2020 2020 7767  None,.        wg
-000e3740: 735f 7663 665f 6f75 745f 7061 7468 3a20  s_vcf_out_path: 
-000e3750: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000e3760: 2020 2020 776f 726b 666c 6f77 5f74 7970      workflow_typ
-000e3770: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-000e3780: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000e3790: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-000e37a0: 6f75 7470 7574 2042 414d 2066 696c 652e  output BAM file.
-000e37b0: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
-000e37c0: 7070 696e 675f 6261 6d5f 6f75 745f 6669  pping_bam_out_fi
-000e37d0: 6c65 6e61 6d65 203d 206d 6170 7069 6e67  lename = mapping
-000e37e0: 5f62 616d 5f6f 7574 5f66 696c 656e 616d  _bam_out_filenam
-000e37f0: 650a 2020 2020 2020 2020 2320 5468 6520  e.        # The 
-000e3800: 6f75 7470 7574 2070 6174 6820 6f66 2074  output path of t
-000e3810: 6865 2042 696e 6172 7920 416c 6967 6e6d  he Binary Alignm
-000e3820: 656e 7420 4d61 7020 2842 414d 2920 6669  ent Map (BAM) fi
-000e3830: 6c65 2e0a 2020 2020 2020 2020 7365 6c66  le..        self
-000e3840: 2e6d 6170 7069 6e67 5f62 616d 5f6f 7574  .mapping_bam_out
-000e3850: 5f70 6174 6820 3d20 6d61 7070 696e 675f  _path = mapping_
-000e3860: 6261 6d5f 6f75 745f 7061 7468 0a20 2020  bam_out_path.   
-000e3870: 2020 2020 2023 2054 6865 206e 616d 6520       # The name 
-000e3880: 6f66 2074 6865 204f 5353 2062 7563 6b65  of the OSS bucke
-000e3890: 7420 7468 6174 2073 746f 7265 7320 7468  t that stores th
-000e38a0: 6520 6461 7461 206f 6620 7468 6520 6d61  e data of the ma
-000e38b0: 7070 696e 6720 776f 726b 666c 6f77 2e0a  pping workflow..
-000e38c0: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-000e38d0: 7069 6e67 5f62 7563 6b65 745f 6e61 6d65  ping_bucket_name
-000e38e0: 203d 206d 6170 7069 6e67 5f62 7563 6b65   = mapping_bucke
-000e38f0: 745f 6e61 6d65 0a20 2020 2020 2020 2023  t_name.        #
-000e3900: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-000e3910: 2066 6972 7374 2046 4153 5451 2066 696c   first FASTQ fil
-000e3920: 6520 6f66 2074 6865 206d 6170 7069 6e67  e of the mapping
-000e3930: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
-000e3940: 2020 2073 656c 662e 6d61 7070 696e 675f     self.mapping_
-000e3950: 6661 7374 715f 6669 7273 745f 6669 6c65  fastq_first_file
-000e3960: 6e61 6d65 203d 206d 6170 7069 6e67 5f66  name = mapping_f
-000e3970: 6173 7471 5f66 6972 7374 5f66 696c 656e  astq_first_filen
-000e3980: 616d 650a 2020 2020 2020 2020 2320 5468  ame.        # Th
-000e3990: 6520 7061 7468 206f 6620 7468 6520 4641  e path of the FA
-000e39a0: 5354 5120 6669 6c65 7320 6f66 2074 6865  STQ files of the
-000e39b0: 206d 6170 7069 6e67 2077 6f72 6b66 6c6f   mapping workflo
-000e39c0: 772e 0a20 2020 2020 2020 2073 656c 662e  w..        self.
-000e39d0: 6d61 7070 696e 675f 6661 7374 715f 7061  mapping_fastq_pa
-000e39e0: 7468 203d 206d 6170 7069 6e67 5f66 6173  th = mapping_fas
-000e39f0: 7471 5f70 6174 680a 2020 2020 2020 2020  tq_path.        
-000e3a00: 2320 5468 6520 6e61 6d65 206f 6620 7468  # The name of th
-000e3a10: 6520 7365 636f 6e64 2046 4153 5451 2066  e second FASTQ f
-000e3a20: 696c 6520 6f66 2074 6865 206d 6170 7069  ile of the mappi
-000e3a30: 6e67 2077 6f72 6b66 6c6f 772e 0a20 2020  ng workflow..   
-000e3a40: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
-000e3a50: 675f 6661 7374 715f 7365 636f 6e64 5f66  g_fastq_second_f
-000e3a60: 696c 656e 616d 6520 3d20 6d61 7070 696e  ilename = mappin
-000e3a70: 675f 6661 7374 715f 7365 636f 6e64 5f66  g_fastq_second_f
-000e3a80: 696c 656e 616d 650a 2020 2020 2020 2020  ilename.        
-000e3a90: 2320 5370 6563 6966 6965 7320 7768 6574  # Specifies whet
-000e3aa0: 6865 7220 746f 206d 6172 6b20 6475 706c  her to mark dupl
-000e3ab0: 6963 6174 6520 7661 6c75 6573 2e0a 2020  icate values..  
-000e3ac0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
-000e3ad0: 6e67 5f69 735f 6d61 726b 5f64 7570 203d  ng_is_mark_dup =
-000e3ae0: 206d 6170 7069 6e67 5f69 735f 6d61 726b   mapping_is_mark
-000e3af0: 5f64 7570 0a20 2020 2020 2020 2023 2054  _dup.        # T
-000e3b00: 6865 2072 6567 696f 6e20 7768 6572 6520  he region where 
-000e3b10: 7468 6520 4f62 6a65 6374 2053 746f 7261  the Object Stora
-000e3b20: 6765 2053 6572 7669 6365 2028 4f53 5329  ge Service (OSS)
-000e3b30: 2062 7563 6b65 7420 7468 6174 2073 746f   bucket that sto
-000e3b40: 7265 7320 7468 6520 6461 7461 206f 6620  res the data of 
-000e3b50: 7468 6520 6d61 7070 696e 6720 776f 726b  the mapping work
-000e3b60: 666c 6f77 2069 7320 6465 706c 6f79 6564  flow is deployed
-000e3b70: 2e0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000e3b80: 6170 7069 6e67 5f6f 7373 5f72 6567 696f  apping_oss_regio
-000e3b90: 6e20 3d20 6d61 7070 696e 675f 6f73 735f  n = mapping_oss_
-000e3ba0: 7265 6769 6f6e 0a20 2020 2020 2020 2023  region.        #
-000e3bb0: 2054 6865 2070 6174 6820 6f66 2074 6865   The path of the
-000e3bc0: 2072 6566 6572 656e 6365 2066 696c 6573   reference files
-000e3bd0: 206f 6620 7468 6520 6d61 7070 696e 6720   of the mapping 
-000e3be0: 776f 726b 666c 6f77 2e0a 2020 2020 2020  workflow..      
-000e3bf0: 2020 7365 6c66 2e6d 6170 7069 6e67 5f72    self.mapping_r
-000e3c00: 6566 6572 656e 6365 5f70 6174 6820 3d20  eference_path = 
-000e3c10: 6d61 7070 696e 675f 7265 6665 7265 6e63  mapping_referenc
-000e3c20: 655f 7061 7468 0a20 2020 2020 2020 2023  e_path.        #
-000e3c30: 2054 6865 2074 7970 6520 6f66 2073 6572   The type of ser
-000e3c40: 7669 6365 2d6c 6576 656c 2061 6772 6565  vice-level agree
-000e3c50: 6d65 6e74 2028 534c 4129 2e20 5661 6c69  ment (SLA). Vali
-000e3c60: 6420 7661 6c75 6573 3a0a 2020 2020 2020  d values:.      
-000e3c70: 2020 2320 0a20 2020 2020 2020 2023 202a    # .        # *
-000e3c80: 2020 2073 3a20 7468 6520 7369 6c76 6572     s: the silver
-000e3c90: 206c 6576 656c 2028 532d 6c65 7665 6c29   level (S-level)
-000e3ca0: 2e20 4974 2072 6571 7569 7265 7320 3120  . It requires 1 
-000e3cb0: 6578 7472 6120 6d69 6e75 7465 2074 6f20  extra minute to 
-000e3cc0: 7072 6f63 6573 7320 6576 6572 7920 312e  process every 1.
-000e3cd0: 3520 6269 6c6c 696f 6e20 6261 7365 2070  5 billion base p
-000e3ce0: 6169 7273 2062 6579 6f6e 6420 7468 6520  airs beyond the 
-000e3cf0: 6c69 6d69 7420 6f66 2039 3020 6269 6c6c  limit of 90 bill
-000e3d00: 696f 6e20 6261 7365 2070 6169 7273 2e0a  ion base pairs..
-000e3d10: 2020 2020 2020 2020 2320 2a20 2020 673a          # *   g:
-000e3d20: 2074 6865 2067 6f6c 6420 6c65 7665 6c20   the gold level 
-000e3d30: 2847 2d6c 6576 656c 292e 2049 7420 7265  (G-level). It re
-000e3d40: 7175 6972 6573 2031 2065 7874 7261 206d  quires 1 extra m
-000e3d50: 696e 7574 6520 746f 2070 726f 6365 7373  inute to process
-000e3d60: 2065 7665 7279 2032 2062 696c 6c69 6f6e   every 2 billion
-000e3d70: 2062 6173 6520 7061 6972 7320 6265 796f   base pairs beyo
-000e3d80: 6e64 2074 6865 206c 696d 6974 206f 6620  nd the limit of 
-000e3d90: 3930 2062 696c 6c69 6f6e 2062 6173 6520  90 billion base 
-000e3da0: 7061 6972 732e 0a20 2020 2020 2020 2023  pairs..        #
-000e3db0: 202a 2020 2070 3a20 7468 6520 706c 6174   *   p: the plat
-000e3dc0: 696e 756d 206c 6576 656c 2028 502d 6c65  inum level (P-le
-000e3dd0: 7665 6c29 2e20 4974 2072 6571 7569 7265  vel). It require
-000e3de0: 7320 3120 6578 7472 6120 6d69 6e75 7465  s 1 extra minute
-000e3df0: 2074 6f20 7072 6f63 6573 7320 6576 6572   to process ever
-000e3e00: 7920 3320 6269 6c6c 696f 6e20 6261 7365  y 3 billion base
-000e3e10: 2070 6169 7273 2062 6579 6f6e 6420 7468   pairs beyond th
-000e3e20: 6520 6c69 6d69 7420 6f66 2039 3020 6269  e limit of 90 bi
-000e3e30: 6c6c 696f 6e20 6261 7365 2070 6169 7273  llion base pairs
-000e3e40: 2e0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-000e3e50: 6572 7669 6365 203d 2073 6572 7669 6365  ervice = service
-000e3e60: 0a20 2020 2020 2020 2023 2054 6865 206e  .        # The n
-000e3e70: 616d 6520 6f66 2074 6865 204f 5353 2062  ame of the OSS b
-000e3e80: 7563 6b65 7420 7468 6174 2073 746f 7265  ucket that store
-000e3e90: 7320 7468 6520 6461 7461 206f 6620 7468  s the data of th
-000e3ea0: 6520 5747 5320 776f 726b 666c 6f77 2e0a  e WGS workflow..
-000e3eb0: 2020 2020 2020 2020 7365 6c66 2e77 6773          self.wgs
-000e3ec0: 5f62 7563 6b65 745f 6e61 6d65 203d 2077  _bucket_name = w
-000e3ed0: 6773 5f62 7563 6b65 745f 6e61 6d65 0a20  gs_bucket_name. 
-000e3ee0: 2020 2020 2020 2023 2054 6865 206e 616d         # The nam
-000e3ef0: 6520 6f66 2074 6865 2066 6972 7374 2046  e of the first F
-000e3f00: 4153 5451 2066 696c 6520 6f66 2074 6865  ASTQ file of the
-000e3f10: 2057 4753 2077 6f72 6b66 6c6f 772e 0a20   WGS workflow.. 
-000e3f20: 2020 2020 2020 2073 656c 662e 7767 735f         self.wgs_
-000e3f30: 6661 7374 715f 6669 7273 745f 6669 6c65  fastq_first_file
-000e3f40: 6e61 6d65 203d 2077 6773 5f66 6173 7471  name = wgs_fastq
-000e3f50: 5f66 6972 7374 5f66 696c 656e 616d 650a  _first_filename.
-000e3f60: 2020 2020 2020 2020 2320 5468 6520 7061          # The pa
-000e3f70: 7468 206f 6620 7468 6520 4641 5354 5120  th of the FASTQ 
-000e3f80: 6669 6c65 7320 6f66 2074 6865 2057 4753  files of the WGS
-000e3f90: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
-000e3fa0: 2020 2073 656c 662e 7767 735f 6661 7374     self.wgs_fast
-000e3fb0: 715f 7061 7468 203d 2077 6773 5f66 6173  q_path = wgs_fas
-000e3fc0: 7471 5f70 6174 680a 2020 2020 2020 2020  tq_path.        
-000e3fd0: 2320 5468 6520 6e61 6d65 206f 6620 7468  # The name of th
-000e3fe0: 6520 7365 636f 6e64 2046 4153 5451 2066  e second FASTQ f
-000e3ff0: 696c 6520 6f66 2074 6865 2057 4753 2077  ile of the WGS w
-000e4000: 6f72 6b66 6c6f 772e 0a20 2020 2020 2020  orkflow..       
-000e4010: 2073 656c 662e 7767 735f 6661 7374 715f   self.wgs_fastq_
-000e4020: 7365 636f 6e64 5f66 696c 656e 616d 6520  second_filename 
-000e4030: 3d20 7767 735f 6661 7374 715f 7365 636f  = wgs_fastq_seco
-000e4040: 6e64 5f66 696c 656e 616d 650a 2020 2020  nd_filename.    
-000e4050: 2020 2020 2320 5468 6520 7265 6769 6f6e      # The region
-000e4060: 2077 6865 7265 2074 6865 204f 5353 2062   where the OSS b
-000e4070: 7563 6b65 7420 7468 6174 2073 746f 7265  ucket that store
-000e4080: 7320 7468 6520 6461 7461 206f 6620 7468  s the data of th
-000e4090: 6520 7768 6f6c 6520 6765 6e6f 6d65 2073  e whole genome s
-000e40a0: 6571 7565 6e63 696e 6720 2857 4753 2920  equencing (WGS) 
-000e40b0: 776f 726b 666c 6f77 2069 7320 6465 706c  workflow is depl
-000e40c0: 6f79 6564 2e0a 2020 2020 2020 2020 7365  oyed..        se
-000e40d0: 6c66 2e77 6773 5f6f 7373 5f72 6567 696f  lf.wgs_oss_regio
-000e40e0: 6e20 3d20 7767 735f 6f73 735f 7265 6769  n = wgs_oss_regi
-000e40f0: 6f6e 0a20 2020 2020 2020 2023 2054 6865  on.        # The
-000e4100: 2070 6174 6820 6f66 2074 6865 2072 6566   path of the ref
-000e4110: 6572 656e 6365 2066 696c 6573 206f 6620  erence files of 
-000e4120: 7468 6520 5747 5320 776f 726b 666c 6f77  the WGS workflow
-000e4130: 2e0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-000e4140: 6773 5f72 6566 6572 656e 6365 5f70 6174  gs_reference_pat
-000e4150: 6820 3d20 7767 735f 7265 6665 7265 6e63  h = wgs_referenc
-000e4160: 655f 7061 7468 0a20 2020 2020 2020 2023  e_path.        #
-000e4170: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-000e4180: 206f 7574 7075 7420 5643 4620 6669 6c65   output VCF file
-000e4190: 2e0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-000e41a0: 6773 5f76 6366 5f6f 7574 5f66 696c 656e  gs_vcf_out_filen
-000e41b0: 616d 6520 3d20 7767 735f 7663 665f 6f75  ame = wgs_vcf_ou
-000e41c0: 745f 6669 6c65 6e61 6d65 0a20 2020 2020  t_filename.     
-000e41d0: 2020 2023 2054 6865 206f 7574 7075 7420     # The output 
-000e41e0: 7061 7468 206f 6620 7468 6520 5661 7269  path of the Vari
-000e41f0: 616e 7420 4361 6c6c 2046 6f72 6d61 7420  ant Call Format 
-000e4200: 2856 4346 2920 6669 6c65 2e0a 2020 2020  (VCF) file..    
-000e4210: 2020 2020 7365 6c66 2e77 6773 5f76 6366      self.wgs_vcf
-000e4220: 5f6f 7574 5f70 6174 6820 3d20 7767 735f  _out_path = wgs_
-000e4230: 7663 665f 6f75 745f 7061 7468 0a20 2020  vcf_out_path.   
-000e4240: 2020 2020 2023 2054 6865 2074 7970 6520       # The type 
-000e4250: 6f66 2077 6f72 6b66 6c6f 772e 2056 616c  of workflow. Val
-000e4260: 6964 2076 616c 7565 733a 2077 6773 2061  id values: wgs a
-000e4270: 6e64 206d 6170 7069 6e67 2e0a 2020 2020  nd mapping..    
-000e4280: 2020 2020 2320 0a20 2020 2020 2020 2023      # .        #
-000e4290: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
-000e42a0: 6973 2072 6571 7569 7265 642e 0a20 2020  is required..   
-000e42b0: 2020 2020 2073 656c 662e 776f 726b 666c       self.workfl
-000e42c0: 6f77 5f74 7970 6520 3d20 776f 726b 666c  ow_type = workfl
-000e42d0: 6f77 5f74 7970 650a 0a20 2020 2064 6566  ow_type..    def
-000e42e0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000e42f0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000e4300: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-000e4310: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-000e4320: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-000e4330: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-000e4340: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-000e4350: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e4360: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-000e4370: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-000e4380: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-000e4390: 6c66 2e6d 6170 7069 6e67 5f62 616d 5f6f  lf.mapping_bam_o
-000e43a0: 7574 5f66 696c 656e 616d 6520 6973 206e  ut_filename is n
-000e43b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e43c0: 2020 2020 2072 6573 756c 745b 276d 6170       result['map
-000e43d0: 7069 6e67 5f62 616d 5f6f 7574 5f66 696c  ping_bam_out_fil
-000e43e0: 656e 616d 6527 5d20 3d20 7365 6c66 2e6d  ename'] = self.m
-000e43f0: 6170 7069 6e67 5f62 616d 5f6f 7574 5f66  apping_bam_out_f
-000e4400: 696c 656e 616d 650a 2020 2020 2020 2020  ilename.        
-000e4410: 6966 2073 656c 662e 6d61 7070 696e 675f  if self.mapping_
-000e4420: 6261 6d5f 6f75 745f 7061 7468 2069 7320  bam_out_path is 
-000e4430: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e4440: 2020 2020 2020 7265 7375 6c74 5b27 6d61        result['ma
-000e4450: 7070 696e 675f 6261 6d5f 6f75 745f 7061  pping_bam_out_pa
-000e4460: 7468 275d 203d 2073 656c 662e 6d61 7070  th'] = self.mapp
-000e4470: 696e 675f 6261 6d5f 6f75 745f 7061 7468  ing_bam_out_path
-000e4480: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e4490: 2e6d 6170 7069 6e67 5f62 7563 6b65 745f  .mapping_bucket_
-000e44a0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-000e44b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e44c0: 7375 6c74 5b27 6d61 7070 696e 675f 6275  sult['mapping_bu
-000e44d0: 636b 6574 5f6e 616d 6527 5d20 3d20 7365  cket_name'] = se
-000e44e0: 6c66 2e6d 6170 7069 6e67 5f62 7563 6b65  lf.mapping_bucke
-000e44f0: 745f 6e61 6d65 0a20 2020 2020 2020 2069  t_name.        i
-000e4500: 6620 7365 6c66 2e6d 6170 7069 6e67 5f66  f self.mapping_f
-000e4510: 6173 7471 5f66 6972 7374 5f66 696c 656e  astq_first_filen
-000e4520: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-000e4530: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000e4540: 756c 745b 276d 6170 7069 6e67 5f66 6173  ult['mapping_fas
-000e4550: 7471 5f66 6972 7374 5f66 696c 656e 616d  tq_first_filenam
-000e4560: 6527 5d20 3d20 7365 6c66 2e6d 6170 7069  e'] = self.mappi
-000e4570: 6e67 5f66 6173 7471 5f66 6972 7374 5f66  ng_fastq_first_f
-000e4580: 696c 656e 616d 650a 2020 2020 2020 2020  ilename.        
-000e4590: 6966 2073 656c 662e 6d61 7070 696e 675f  if self.mapping_
-000e45a0: 6661 7374 715f 7061 7468 2069 7320 6e6f  fastq_path is no
-000e45b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e45c0: 2020 2020 7265 7375 6c74 5b27 6d61 7070      result['mapp
-000e45d0: 696e 675f 6661 7374 715f 7061 7468 275d  ing_fastq_path']
-000e45e0: 203d 2073 656c 662e 6d61 7070 696e 675f   = self.mapping_
-000e45f0: 6661 7374 715f 7061 7468 0a20 2020 2020  fastq_path.     
-000e4600: 2020 2069 6620 7365 6c66 2e6d 6170 7069     if self.mappi
-000e4610: 6e67 5f66 6173 7471 5f73 6563 6f6e 645f  ng_fastq_second_
-000e4620: 6669 6c65 6e61 6d65 2069 7320 6e6f 7420  filename is not 
-000e4630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e4640: 2020 7265 7375 6c74 5b27 6d61 7070 696e    result['mappin
-000e4650: 675f 6661 7374 715f 7365 636f 6e64 5f66  g_fastq_second_f
-000e4660: 696c 656e 616d 6527 5d20 3d20 7365 6c66  ilename'] = self
-000e4670: 2e6d 6170 7069 6e67 5f66 6173 7471 5f73  .mapping_fastq_s
-000e4680: 6563 6f6e 645f 6669 6c65 6e61 6d65 0a20  econd_filename. 
-000e4690: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-000e46a0: 6170 7069 6e67 5f69 735f 6d61 726b 5f64  apping_is_mark_d
-000e46b0: 7570 2069 7320 6e6f 7420 4e6f 6e65 3a0a  up is not None:.
-000e46c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000e46d0: 6c74 5b27 6d61 7070 696e 675f 6973 5f6d  lt['mapping_is_m
-000e46e0: 6172 6b5f 6475 7027 5d20 3d20 7365 6c66  ark_dup'] = self
-000e46f0: 2e6d 6170 7069 6e67 5f69 735f 6d61 726b  .mapping_is_mark
-000e4700: 5f64 7570 0a20 2020 2020 2020 2069 6620  _dup.        if 
-000e4710: 7365 6c66 2e6d 6170 7069 6e67 5f6f 7373  self.mapping_oss
-000e4720: 5f72 6567 696f 6e20 6973 206e 6f74 204e  _region is not N
-000e4730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e4740: 2072 6573 756c 745b 276d 6170 7069 6e67   result['mapping
-000e4750: 5f6f 7373 5f72 6567 696f 6e27 5d20 3d20  _oss_region'] = 
-000e4760: 7365 6c66 2e6d 6170 7069 6e67 5f6f 7373  self.mapping_oss
-000e4770: 5f72 6567 696f 6e0a 2020 2020 2020 2020  _region.        
-000e4780: 6966 2073 656c 662e 6d61 7070 696e 675f  if self.mapping_
-000e4790: 7265 6665 7265 6e63 655f 7061 7468 2069  reference_path i
-000e47a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e47b0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000e47c0: 6d61 7070 696e 675f 7265 6665 7265 6e63  mapping_referenc
-000e47d0: 655f 7061 7468 275d 203d 2073 656c 662e  e_path'] = self.
-000e47e0: 6d61 7070 696e 675f 7265 6665 7265 6e63  mapping_referenc
-000e47f0: 655f 7061 7468 0a20 2020 2020 2020 2069  e_path.        i
-000e4800: 6620 7365 6c66 2e73 6572 7669 6365 2069  f self.service i
-000e4810: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e4820: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000e4830: 7365 7276 6963 6527 5d20 3d20 7365 6c66  service'] = self
-000e4840: 2e73 6572 7669 6365 0a20 2020 2020 2020  .service.       
-000e4850: 2069 6620 7365 6c66 2e77 6773 5f62 7563   if self.wgs_buc
-000e4860: 6b65 745f 6e61 6d65 2069 7320 6e6f 7420  ket_name is not 
-000e4870: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e4880: 2020 7265 7375 6c74 5b27 7767 735f 6275    result['wgs_bu
-000e4890: 636b 6574 5f6e 616d 6527 5d20 3d20 7365  cket_name'] = se
-000e48a0: 6c66 2e77 6773 5f62 7563 6b65 745f 6e61  lf.wgs_bucket_na
-000e48b0: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
-000e48c0: 6c66 2e77 6773 5f66 6173 7471 5f66 6972  lf.wgs_fastq_fir
-000e48d0: 7374 5f66 696c 656e 616d 6520 6973 206e  st_filename is n
-000e48e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e48f0: 2020 2020 2072 6573 756c 745b 2777 6773       result['wgs
-000e4900: 5f66 6173 7471 5f66 6972 7374 5f66 696c  _fastq_first_fil
-000e4910: 656e 616d 6527 5d20 3d20 7365 6c66 2e77  ename'] = self.w
-000e4920: 6773 5f66 6173 7471 5f66 6972 7374 5f66  gs_fastq_first_f
-000e4930: 696c 656e 616d 650a 2020 2020 2020 2020  ilename.        
-000e4940: 6966 2073 656c 662e 7767 735f 6661 7374  if self.wgs_fast
-000e4950: 715f 7061 7468 2069 7320 6e6f 7420 4e6f  q_path is not No
-000e4960: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e4970: 7265 7375 6c74 5b27 7767 735f 6661 7374  result['wgs_fast
-000e4980: 715f 7061 7468 275d 203d 2073 656c 662e  q_path'] = self.
-000e4990: 7767 735f 6661 7374 715f 7061 7468 0a20  wgs_fastq_path. 
-000e49a0: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-000e49b0: 6773 5f66 6173 7471 5f73 6563 6f6e 645f  gs_fastq_second_
-000e49c0: 6669 6c65 6e61 6d65 2069 7320 6e6f 7420  filename is not 
-000e49d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e49e0: 2020 7265 7375 6c74 5b27 7767 735f 6661    result['wgs_fa
-000e49f0: 7374 715f 7365 636f 6e64 5f66 696c 656e  stq_second_filen
-000e4a00: 616d 6527 5d20 3d20 7365 6c66 2e77 6773  ame'] = self.wgs
-000e4a10: 5f66 6173 7471 5f73 6563 6f6e 645f 6669  _fastq_second_fi
-000e4a20: 6c65 6e61 6d65 0a20 2020 2020 2020 2069  lename.        i
-000e4a30: 6620 7365 6c66 2e77 6773 5f6f 7373 5f72  f self.wgs_oss_r
-000e4a40: 6567 696f 6e20 6973 206e 6f74 204e 6f6e  egion is not Non
-000e4a50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e4a60: 6573 756c 745b 2777 6773 5f6f 7373 5f72  esult['wgs_oss_r
-000e4a70: 6567 696f 6e27 5d20 3d20 7365 6c66 2e77  egion'] = self.w
-000e4a80: 6773 5f6f 7373 5f72 6567 696f 6e0a 2020  gs_oss_region.  
-000e4a90: 2020 2020 2020 6966 2073 656c 662e 7767        if self.wg
-000e4aa0: 735f 7265 6665 7265 6e63 655f 7061 7468  s_reference_path
-000e4ab0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e4ac0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e4ad0: 5b27 7767 735f 7265 6665 7265 6e63 655f  ['wgs_reference_
-000e4ae0: 7061 7468 275d 203d 2073 656c 662e 7767  path'] = self.wg
-000e4af0: 735f 7265 6665 7265 6e63 655f 7061 7468  s_reference_path
-000e4b00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e4b10: 2e77 6773 5f76 6366 5f6f 7574 5f66 696c  .wgs_vcf_out_fil
-000e4b20: 656e 616d 6520 6973 206e 6f74 204e 6f6e  ename is not Non
-000e4b30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e4b40: 6573 756c 745b 2777 6773 5f76 6366 5f6f  esult['wgs_vcf_o
-000e4b50: 7574 5f66 696c 656e 616d 6527 5d20 3d20  ut_filename'] = 
-000e4b60: 7365 6c66 2e77 6773 5f76 6366 5f6f 7574  self.wgs_vcf_out
-000e4b70: 5f66 696c 656e 616d 650a 2020 2020 2020  _filename.      
-000e4b80: 2020 6966 2073 656c 662e 7767 735f 7663    if self.wgs_vc
-000e4b90: 665f 6f75 745f 7061 7468 2069 7320 6e6f  f_out_path is no
-000e4ba0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e4bb0: 2020 2020 7265 7375 6c74 5b27 7767 735f      result['wgs_
-000e4bc0: 7663 665f 6f75 745f 7061 7468 275d 203d  vcf_out_path'] =
-000e4bd0: 2073 656c 662e 7767 735f 7663 665f 6f75   self.wgs_vcf_ou
-000e4be0: 745f 7061 7468 0a20 2020 2020 2020 2069  t_path.        i
-000e4bf0: 6620 7365 6c66 2e77 6f72 6b66 6c6f 775f  f self.workflow_
-000e4c00: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-000e4c10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e4c20: 7375 6c74 5b27 776f 726b 666c 6f77 5f74  sult['workflow_t
-000e4c30: 7970 6527 5d20 3d20 7365 6c66 2e77 6f72  ype'] = self.wor
-000e4c40: 6b66 6c6f 775f 7479 7065 0a20 2020 2020  kflow_type.     
-000e4c50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000e4c60: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000e4c70: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000e4c80: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000e4c90: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000e4ca0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000e4cb0: 6574 2827 6d61 7070 696e 675f 6261 6d5f  et('mapping_bam_
-000e4cc0: 6f75 745f 6669 6c65 6e61 6d65 2729 2069  out_filename') i
-000e4cd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e4ce0: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
-000e4cf0: 7069 6e67 5f62 616d 5f6f 7574 5f66 696c  ping_bam_out_fil
-000e4d00: 656e 616d 6520 3d20 6d2e 6765 7428 276d  ename = m.get('m
-000e4d10: 6170 7069 6e67 5f62 616d 5f6f 7574 5f66  apping_bam_out_f
-000e4d20: 696c 656e 616d 6527 290a 2020 2020 2020  ilename').      
-000e4d30: 2020 6966 206d 2e67 6574 2827 6d61 7070    if m.get('mapp
-000e4d40: 696e 675f 6261 6d5f 6f75 745f 7061 7468  ing_bam_out_path
-000e4d50: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000e4d60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e4d70: 2e6d 6170 7069 6e67 5f62 616d 5f6f 7574  .mapping_bam_out
-000e4d80: 5f70 6174 6820 3d20 6d2e 6765 7428 276d  _path = m.get('m
-000e4d90: 6170 7069 6e67 5f62 616d 5f6f 7574 5f70  apping_bam_out_p
-000e4da0: 6174 6827 290a 2020 2020 2020 2020 6966  ath').        if
-000e4db0: 206d 2e67 6574 2827 6d61 7070 696e 675f   m.get('mapping_
-000e4dc0: 6275 636b 6574 5f6e 616d 6527 2920 6973  bucket_name') is
-000e4dd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e4de0: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
-000e4df0: 696e 675f 6275 636b 6574 5f6e 616d 6520  ing_bucket_name 
-000e4e00: 3d20 6d2e 6765 7428 276d 6170 7069 6e67  = m.get('mapping
-000e4e10: 5f62 7563 6b65 745f 6e61 6d65 2729 0a20  _bucket_name'). 
-000e4e20: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000e4e30: 276d 6170 7069 6e67 5f66 6173 7471 5f66  'mapping_fastq_f
-000e4e40: 6972 7374 5f66 696c 656e 616d 6527 2920  irst_filename') 
-000e4e50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e4e60: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-000e4e70: 7070 696e 675f 6661 7374 715f 6669 7273  pping_fastq_firs
-000e4e80: 745f 6669 6c65 6e61 6d65 203d 206d 2e67  t_filename = m.g
-000e4e90: 6574 2827 6d61 7070 696e 675f 6661 7374  et('mapping_fast
-000e4ea0: 715f 6669 7273 745f 6669 6c65 6e61 6d65  q_first_filename
-000e4eb0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000e4ec0: 6765 7428 276d 6170 7069 6e67 5f66 6173  get('mapping_fas
-000e4ed0: 7471 5f70 6174 6827 2920 6973 206e 6f74  tq_path') is not
-000e4ee0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e4ef0: 2020 2073 656c 662e 6d61 7070 696e 675f     self.mapping_
-000e4f00: 6661 7374 715f 7061 7468 203d 206d 2e67  fastq_path = m.g
-000e4f10: 6574 2827 6d61 7070 696e 675f 6661 7374  et('mapping_fast
-000e4f20: 715f 7061 7468 2729 0a20 2020 2020 2020  q_path').       
-000e4f30: 2069 6620 6d2e 6765 7428 276d 6170 7069   if m.get('mappi
-000e4f40: 6e67 5f66 6173 7471 5f73 6563 6f6e 645f  ng_fastq_second_
-000e4f50: 6669 6c65 6e61 6d65 2729 2069 7320 6e6f  filename') is no
-000e4f60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e4f70: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
-000e4f80: 5f66 6173 7471 5f73 6563 6f6e 645f 6669  _fastq_second_fi
-000e4f90: 6c65 6e61 6d65 203d 206d 2e67 6574 2827  lename = m.get('
-000e4fa0: 6d61 7070 696e 675f 6661 7374 715f 7365  mapping_fastq_se
-000e4fb0: 636f 6e64 5f66 696c 656e 616d 6527 290a  cond_filename').
-000e4fc0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000e4fd0: 2827 6d61 7070 696e 675f 6973 5f6d 6172  ('mapping_is_mar
-000e4fe0: 6b5f 6475 7027 2920 6973 206e 6f74 204e  k_dup') is not N
-000e4ff0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e5000: 2073 656c 662e 6d61 7070 696e 675f 6973   self.mapping_is
-000e5010: 5f6d 6172 6b5f 6475 7020 3d20 6d2e 6765  _mark_dup = m.ge
-000e5020: 7428 276d 6170 7069 6e67 5f69 735f 6d61  t('mapping_is_ma
-000e5030: 726b 5f64 7570 2729 0a20 2020 2020 2020  rk_dup').       
-000e5040: 2069 6620 6d2e 6765 7428 276d 6170 7069   if m.get('mappi
-000e5050: 6e67 5f6f 7373 5f72 6567 696f 6e27 2920  ng_oss_region') 
-000e5060: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e5070: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-000e5080: 7070 696e 675f 6f73 735f 7265 6769 6f6e  pping_oss_region
-000e5090: 203d 206d 2e67 6574 2827 6d61 7070 696e   = m.get('mappin
-000e50a0: 675f 6f73 735f 7265 6769 6f6e 2729 0a20  g_oss_region'). 
-000e50b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000e50c0: 276d 6170 7069 6e67 5f72 6566 6572 656e  'mapping_referen
-000e50d0: 6365 5f70 6174 6827 2920 6973 206e 6f74  ce_path') is not
-000e50e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e50f0: 2020 2073 656c 662e 6d61 7070 696e 675f     self.mapping_
-000e5100: 7265 6665 7265 6e63 655f 7061 7468 203d  reference_path =
-000e5110: 206d 2e67 6574 2827 6d61 7070 696e 675f   m.get('mapping_
-000e5120: 7265 6665 7265 6e63 655f 7061 7468 2729  reference_path')
-000e5130: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000e5140: 7428 2773 6572 7669 6365 2729 2069 7320  t('service') is 
-000e5150: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e5160: 2020 2020 2020 7365 6c66 2e73 6572 7669        self.servi
-000e5170: 6365 203d 206d 2e67 6574 2827 7365 7276  ce = m.get('serv
-000e5180: 6963 6527 290a 2020 2020 2020 2020 6966  ice').        if
-000e5190: 206d 2e67 6574 2827 7767 735f 6275 636b   m.get('wgs_buck
-000e51a0: 6574 5f6e 616d 6527 2920 6973 206e 6f74  et_name') is not
-000e51b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e51c0: 2020 2073 656c 662e 7767 735f 6275 636b     self.wgs_buck
-000e51d0: 6574 5f6e 616d 6520 3d20 6d2e 6765 7428  et_name = m.get(
-000e51e0: 2777 6773 5f62 7563 6b65 745f 6e61 6d65  'wgs_bucket_name
-000e51f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000e5200: 6765 7428 2777 6773 5f66 6173 7471 5f66  get('wgs_fastq_f
-000e5210: 6972 7374 5f66 696c 656e 616d 6527 2920  irst_filename') 
-000e5220: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e5230: 2020 2020 2020 2020 2073 656c 662e 7767           self.wg
-000e5240: 735f 6661 7374 715f 6669 7273 745f 6669  s_fastq_first_fi
-000e5250: 6c65 6e61 6d65 203d 206d 2e67 6574 2827  lename = m.get('
-000e5260: 7767 735f 6661 7374 715f 6669 7273 745f  wgs_fastq_first_
-000e5270: 6669 6c65 6e61 6d65 2729 0a20 2020 2020  filename').     
-000e5280: 2020 2069 6620 6d2e 6765 7428 2777 6773     if m.get('wgs
-000e5290: 5f66 6173 7471 5f70 6174 6827 2920 6973  _fastq_path') is
-000e52a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e52b0: 2020 2020 2020 2073 656c 662e 7767 735f         self.wgs_
-000e52c0: 6661 7374 715f 7061 7468 203d 206d 2e67  fastq_path = m.g
-000e52d0: 6574 2827 7767 735f 6661 7374 715f 7061  et('wgs_fastq_pa
-000e52e0: 7468 2729 0a20 2020 2020 2020 2069 6620  th').        if 
-000e52f0: 6d2e 6765 7428 2777 6773 5f66 6173 7471  m.get('wgs_fastq
-000e5300: 5f73 6563 6f6e 645f 6669 6c65 6e61 6d65  _second_filename
-000e5310: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000e5320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e5330: 2e77 6773 5f66 6173 7471 5f73 6563 6f6e  .wgs_fastq_secon
-000e5340: 645f 6669 6c65 6e61 6d65 203d 206d 2e67  d_filename = m.g
-000e5350: 6574 2827 7767 735f 6661 7374 715f 7365  et('wgs_fastq_se
-000e5360: 636f 6e64 5f66 696c 656e 616d 6527 290a  cond_filename').
-000e5370: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000e5380: 2827 7767 735f 6f73 735f 7265 6769 6f6e  ('wgs_oss_region
-000e5390: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000e53a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e53b0: 2e77 6773 5f6f 7373 5f72 6567 696f 6e20  .wgs_oss_region 
-000e53c0: 3d20 6d2e 6765 7428 2777 6773 5f6f 7373  = m.get('wgs_oss
-000e53d0: 5f72 6567 696f 6e27 290a 2020 2020 2020  _region').      
-000e53e0: 2020 6966 206d 2e67 6574 2827 7767 735f    if m.get('wgs_
-000e53f0: 7265 6665 7265 6e63 655f 7061 7468 2729  reference_path')
-000e5400: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e5410: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-000e5420: 6773 5f72 6566 6572 656e 6365 5f70 6174  gs_reference_pat
-000e5430: 6820 3d20 6d2e 6765 7428 2777 6773 5f72  h = m.get('wgs_r
-000e5440: 6566 6572 656e 6365 5f70 6174 6827 290a  eference_path').
-000e5450: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000e5460: 2827 7767 735f 7663 665f 6f75 745f 6669  ('wgs_vcf_out_fi
-000e5470: 6c65 6e61 6d65 2729 2069 7320 6e6f 7420  lename') is not 
-000e5480: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e5490: 2020 7365 6c66 2e77 6773 5f76 6366 5f6f    self.wgs_vcf_o
-000e54a0: 7574 5f66 696c 656e 616d 6520 3d20 6d2e  ut_filename = m.
-000e54b0: 6765 7428 2777 6773 5f76 6366 5f6f 7574  get('wgs_vcf_out
-000e54c0: 5f66 696c 656e 616d 6527 290a 2020 2020  _filename').    
-000e54d0: 2020 2020 6966 206d 2e67 6574 2827 7767      if m.get('wg
-000e54e0: 735f 7663 665f 6f75 745f 7061 7468 2729  s_vcf_out_path')
-000e54f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e5500: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-000e5510: 6773 5f76 6366 5f6f 7574 5f70 6174 6820  gs_vcf_out_path 
-000e5520: 3d20 6d2e 6765 7428 2777 6773 5f76 6366  = m.get('wgs_vcf
-000e5530: 5f6f 7574 5f70 6174 6827 290a 2020 2020  _out_path').    
-000e5540: 2020 2020 6966 206d 2e67 6574 2827 776f      if m.get('wo
-000e5550: 726b 666c 6f77 5f74 7970 6527 2920 6973  rkflow_type') is
-000e5560: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e5570: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
-000e5580: 666c 6f77 5f74 7970 6520 3d20 6d2e 6765  flow_type = m.ge
-000e5590: 7428 2777 6f72 6b66 6c6f 775f 7479 7065  t('workflow_type
-000e55a0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-000e55b0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
-000e55c0: 7461 7274 576f 726b 666c 6f77 5265 7370  tartWorkflowResp
-000e55d0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-000e55e0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000e55f0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-000e5600: 6c66 2c0a 2020 2020 2020 2020 6a6f 625f  lf,.        job_
-000e5610: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-000e5620: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-000e5630: 2023 2054 6865 206e 616d 6520 6f66 2074   # The name of t
-000e5640: 6865 2077 6f72 6b66 6c6f 772e 0a20 2020  he workflow..   
-000e5650: 2020 2020 2073 656c 662e 6a6f 625f 6e61       self.job_na
-000e5660: 6d65 203d 206a 6f62 5f6e 616d 650a 0a20  me = job_name.. 
-000e5670: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-000e5680: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-000e5690: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-000e56a0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-000e56b0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-000e56c0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-000e56d0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000e56e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e56f0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000e5700: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000e5710: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000e5720: 2069 6620 7365 6c66 2e6a 6f62 5f6e 616d   if self.job_nam
-000e5730: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000e5740: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000e5750: 745b 274a 6f62 4e61 6d65 275d 203d 2073  t['JobName'] = s
-000e5760: 656c 662e 6a6f 625f 6e61 6d65 0a20 2020  elf.job_name.   
-000e5770: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000e5780: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-000e5790: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-000e57a0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-000e57b0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-000e57c0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-000e57d0: 2e67 6574 2827 4a6f 624e 616d 6527 2920  .get('JobName') 
-000e57e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e57f0: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-000e5800: 625f 6e61 6d65 203d 206d 2e67 6574 2827  b_name = m.get('
-000e5810: 4a6f 624e 616d 6527 290a 2020 2020 2020  JobName').      
-000e5820: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000e5830: 636c 6173 7320 5374 6172 7457 6f72 6b66  class StartWorkf
-000e5840: 6c6f 7752 6573 706f 6e73 6528 5465 614d  lowResponse(TeaM
-000e5850: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000e5860: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000e5870: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
-000e5880: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
-000e5890: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
-000e58a0: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
-000e58b0: 6465 3a20 696e 7420 3d20 4e6f 6e65 2c0a  de: int = None,.
-000e58c0: 2020 2020 2020 2020 626f 6479 3a20 5374          body: St
-000e58d0: 6172 7457 6f72 6b66 6c6f 7752 6573 706f  artWorkflowRespo
-000e58e0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-000e58f0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-000e5900: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-000e5910: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-000e5920: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-000e5930: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-000e5940: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-000e5950: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-000e5960: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000e5970: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000e5980: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-000e5990: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-000e59a0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-000e59b0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-000e59c0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-000e59d0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-000e59e0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000e59f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e5a00: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000e5a10: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000e5a20: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000e5a30: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-000e5a40: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-000e5a50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000e5a60: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-000e5a70: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-000e5a80: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-000e5a90: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-000e5aa0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e5ab0: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-000e5ac0: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-000e5ad0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-000e5ae0: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-000e5af0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e5b00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000e5b10: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-000e5b20: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-000e5b30: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000e5b40: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000e5b50: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000e5b60: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000e5b70: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000e5b80: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000e5b90: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-000e5ba0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e5bb0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000e5bc0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-000e5bd0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-000e5be0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-000e5bf0: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-000e5c00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e5c10: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000e5c20: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-000e5c30: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-000e5c40: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-000e5c50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e5c60: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000e5c70: 6465 6c20 3d20 5374 6172 7457 6f72 6b66  del = StartWorkf
-000e5c80: 6c6f 7752 6573 706f 6e73 6542 6f64 7928  lowResponseBody(
-000e5c90: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000e5ca0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-000e5cb0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-000e5cc0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-000e5cd0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000e5ce0: 6c61 7373 2053 746f 7041 6c65 7274 5265  lass StopAlertRe
-000e5cf0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-000e5d00: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000e5d10: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-000e5d20: 0a20 2020 2020 2020 2061 6c65 7274 5f72  .        alert_r
-000e5d30: 756c 655f 6772 6f75 705f 6e61 6d65 3a20  ule_group_name: 
-000e5d40: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000e5d50: 2020 2020 616c 6572 745f 7275 6c65 5f6e      alert_rule_n
-000e5d60: 616d 653a 2073 7472 203d 204e 6f6e 652c  ame: str = None,
-000e5d70: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000e5d80: 2320 5468 6520 6e61 6d65 206f 6620 7468  # The name of th
-000e5d90: 6520 616c 6572 7420 7275 6c65 2073 6574  e alert rule set
-000e5da0: 2074 6f20 6265 2064 6973 6162 6c65 642e   to be disabled.
-000e5db0: 0a20 2020 2020 2020 2073 656c 662e 616c  .        self.al
-000e5dc0: 6572 745f 7275 6c65 5f67 726f 7570 5f6e  ert_rule_group_n
-000e5dd0: 616d 6520 3d20 616c 6572 745f 7275 6c65  ame = alert_rule
-000e5de0: 5f67 726f 7570 5f6e 616d 650a 2020 2020  _group_name.    
-000e5df0: 2020 2020 2320 5468 6520 6e61 6d65 206f      # The name o
-000e5e00: 6620 7468 6520 616c 6572 7420 7275 6c65  f the alert rule
-000e5e10: 2074 6f20 6265 2064 6973 6162 6c65 642e   to be disabled.
-000e5e20: 2049 6620 796f 7520 646f 206e 6f74 2073   If you do not s
-000e5e30: 7065 6369 6679 2061 6e20 616c 6572 7420  pecify an alert 
-000e5e40: 7275 6c65 206e 616d 652c 2074 6865 2061  rule name, the a
-000e5e50: 6c65 7274 2072 756c 6520 7365 7420 6973  lert rule set is
-000e5e60: 2064 6973 6162 6c65 642e 0a20 2020 2020   disabled..     
-000e5e70: 2020 2073 656c 662e 616c 6572 745f 7275     self.alert_ru
-000e5e80: 6c65 5f6e 616d 6520 3d20 616c 6572 745f  le_name = alert_
-000e5e90: 7275 6c65 5f6e 616d 650a 0a20 2020 2064  rule_name..    d
-000e5ea0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000e5eb0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000e5ec0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000e5ed0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000e5ee0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-000e5ef0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000e5f00: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000e5f10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e5f20: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000e5f30: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000e5f40: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000e5f50: 7365 6c66 2e61 6c65 7274 5f72 756c 655f  self.alert_rule_
-000e5f60: 6772 6f75 705f 6e61 6d65 2069 7320 6e6f  group_name is no
-000e5f70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e5f80: 2020 2020 7265 7375 6c74 5b27 616c 6572      result['aler
-000e5f90: 745f 7275 6c65 5f67 726f 7570 5f6e 616d  t_rule_group_nam
-000e5fa0: 6527 5d20 3d20 7365 6c66 2e61 6c65 7274  e'] = self.alert
-000e5fb0: 5f72 756c 655f 6772 6f75 705f 6e61 6d65  _rule_group_name
-000e5fc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e5fd0: 2e61 6c65 7274 5f72 756c 655f 6e61 6d65  .alert_rule_name
-000e5fe0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e5ff0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e6000: 5b27 616c 6572 745f 7275 6c65 5f6e 616d  ['alert_rule_nam
-000e6010: 6527 5d20 3d20 7365 6c66 2e61 6c65 7274  e'] = self.alert
-000e6020: 5f72 756c 655f 6e61 6d65 0a20 2020 2020  _rule_name.     
-000e6030: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000e6040: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000e6050: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000e6060: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000e6070: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000e6080: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000e6090: 6574 2827 616c 6572 745f 7275 6c65 5f67  et('alert_rule_g
-000e60a0: 726f 7570 5f6e 616d 6527 2920 6973 206e  roup_name') is n
-000e60b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e60c0: 2020 2020 2073 656c 662e 616c 6572 745f       self.alert_
-000e60d0: 7275 6c65 5f67 726f 7570 5f6e 616d 6520  rule_group_name 
-000e60e0: 3d20 6d2e 6765 7428 2761 6c65 7274 5f72  = m.get('alert_r
-000e60f0: 756c 655f 6772 6f75 705f 6e61 6d65 2729  ule_group_name')
-000e6100: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000e6110: 7428 2761 6c65 7274 5f72 756c 655f 6e61  t('alert_rule_na
-000e6120: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-000e6130: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000e6140: 6c66 2e61 6c65 7274 5f72 756c 655f 6e61  lf.alert_rule_na
-000e6150: 6d65 203d 206d 2e67 6574 2827 616c 6572  me = m.get('aler
-000e6160: 745f 7275 6c65 5f6e 616d 6527 290a 2020  t_rule_name').  
-000e6170: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000e6180: 660a 0a0a 636c 6173 7320 5374 6f70 416c  f...class StopAl
-000e6190: 6572 7452 6573 706f 6e73 6542 6f64 7928  ertResponseBody(
-000e61a0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-000e61b0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000e61c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000e61d0: 2020 206d 7367 3a20 7374 7220 3d20 4e6f     msg: str = No
-000e61e0: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-000e61f0: 7573 3a20 626f 6f6c 203d 204e 6f6e 652c  us: bool = None,
-000e6200: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000e6210: 2320 5468 6520 6572 726f 7220 6d65 7373  # The error mess
-000e6220: 6167 6520 7265 7475 726e 6564 2069 6620  age returned if 
-000e6230: 7468 6520 6361 6c6c 2066 6169 6c73 2e0a  the call fails..
-000e6240: 2020 2020 2020 2020 7365 6c66 2e6d 7367          self.msg
-000e6250: 203d 206d 7367 0a20 2020 2020 2020 2023   = msg.        #
-000e6260: 2054 6865 206f 7065 7261 7469 6f6e 2072   The operation r
-000e6270: 6573 756c 742e 2056 616c 6964 2076 616c  esult. Valid val
-000e6280: 7565 733a 0a20 2020 2020 2020 2023 200a  ues:.        # .
-000e6290: 2020 2020 2020 2020 2320 2a20 2020 5472          # *   Tr
-000e62a0: 7565 3a20 5468 6520 6f70 6572 6174 696f  ue: The operatio
-000e62b0: 6e20 6973 2073 7563 6365 7373 6675 6c2e  n is successful.
-000e62c0: 0a20 2020 2020 2020 2023 202a 2020 2046  .        # *   F
-000e62d0: 616c 7365 3a20 5468 6520 6f70 6572 6174  alse: The operat
-000e62e0: 696f 6e20 6661 696c 6564 2e0a 2020 2020  ion failed..    
-000e62f0: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
-000e6300: 3d20 7374 6174 7573 0a0a 2020 2020 6465  = status..    de
-000e6310: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000e6320: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-000e6330: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000e6340: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000e6350: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000e6360: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000e6370: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000e6380: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e6390: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000e63a0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000e63b0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000e63c0: 656c 662e 6d73 6720 6973 206e 6f74 204e  elf.msg is not N
-000e63d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e63e0: 2072 6573 756c 745b 276d 7367 275d 203d   result['msg'] =
-000e63f0: 2073 656c 662e 6d73 670a 2020 2020 2020   self.msg.      
-000e6400: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-000e6410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e6420: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e6430: 5b27 7374 6174 7573 275d 203d 2073 656c  ['status'] = sel
-000e6440: 662e 7374 6174 7573 0a20 2020 2020 2020  f.status.       
-000e6450: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000e6460: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000e6470: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-000e6480: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-000e6490: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-000e64a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000e64b0: 2827 6d73 6727 2920 6973 206e 6f74 204e  ('msg') is not N
-000e64c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e64d0: 2073 656c 662e 6d73 6720 3d20 6d2e 6765   self.msg = m.ge
-000e64e0: 7428 276d 7367 2729 0a20 2020 2020 2020  t('msg').       
-000e64f0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-000e6500: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-000e6510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000e6520: 662e 7374 6174 7573 203d 206d 2e67 6574  f.status = m.get
-000e6530: 2827 7374 6174 7573 2729 0a20 2020 2020  ('status').     
-000e6540: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-000e6550: 0a63 6c61 7373 2053 746f 7041 6c65 7274  .class StopAlert
-000e6560: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-000e6570: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000e6580: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-000e6590: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-000e65a0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-000e65b0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-000e65c0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-000e65d0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-000e65e0: 2020 2020 2062 6f64 793a 2053 746f 7041       body: StopA
-000e65f0: 6c65 7274 5265 7370 6f6e 7365 426f 6479  lertResponseBody
-000e6600: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000e6610: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000e6620: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-000e6630: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000e6640: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-000e6650: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-000e6660: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-000e6670: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000e6680: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e6690: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-000e66a0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000e66b0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-000e66c0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000e66d0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000e66e0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000e66f0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000e6700: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000e6710: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e6720: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000e6730: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000e6740: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000e6750: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-000e6760: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e6770: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-000e6780: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-000e6790: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-000e67a0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000e67b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000e67c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000e67d0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-000e67e0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-000e67f0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-000e6800: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-000e6810: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e6820: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-000e6830: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-000e6840: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-000e6850: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000e6860: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000e6870: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000e6880: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000e6890: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000e68a0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-000e68b0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-000e68c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e68d0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-000e68e0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000e68f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000e6900: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-000e6910: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e6920: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000e6930: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-000e6940: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-000e6950: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000e6960: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-000e6970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000e6980: 2020 7465 6d70 5f6d 6f64 656c 203d 2053    temp_model = S
-000e6990: 746f 7041 6c65 7274 5265 7370 6f6e 7365  topAlertResponse
-000e69a0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-000e69b0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-000e69c0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-000e69d0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-000e69e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000e69f0: 660a 0a0a 636c 6173 7320 5379 6e63 436c  f...class SyncCl
-000e6a00: 7573 7465 724e 6f64 6550 6f6f 6c52 6573  usterNodePoolRes
-000e6a10: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
-000e6a20: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000e6a30: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000e6a40: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
-000e6a50: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
-000e6a60: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000e6a70: 2020 2020 2320 5468 6520 7265 7175 6573      # The reques
-000e6a80: 7420 4944 2e0a 2020 2020 2020 2020 7365  t ID..        se
-000e6a90: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-000e6aa0: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
-000e6ab0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-000e6ac0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-000e6ad0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000e6ae0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e6af0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000e6b00: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000e6b10: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000e6b20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e6b30: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000e6b40: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000e6b50: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000e6b60: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-000e6b70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e6b80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e6b90: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
-000e6ba0: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
-000e6bb0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000e6bc0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-000e6bd0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-000e6be0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-000e6bf0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-000e6c00: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000e6c10: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-000e6c20: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-000e6c30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000e6c40: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-000e6c50: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-000e6c60: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-000e6c70: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
-000e6c80: 796e 6343 6c75 7374 6572 4e6f 6465 506f  yncClusterNodePo
-000e6c90: 6f6c 5265 7370 6f6e 7365 2854 6561 4d6f  olResponse(TeaMo
-000e6ca0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-000e6cb0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000e6cc0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
-000e6cd0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
-000e6ce0: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
-000e6cf0: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
-000e6d00: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
-000e6d10: 2020 2020 2020 2062 6f64 793a 2053 796e         body: Syn
-000e6d20: 6343 6c75 7374 6572 4e6f 6465 506f 6f6c  cClusterNodePool
-000e6d30: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
-000e6d40: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000e6d50: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-000e6d60: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
-000e6d70: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-000e6d80: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-000e6d90: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
-000e6da0: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
-000e6db0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-000e6dc0: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-000e6dd0: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
-000e6de0: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
-000e6df0: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
-000e6e00: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000e6e10: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000e6e20: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-000e6e30: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-000e6e40: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000e6e50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000e6e60: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-000e6e70: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000e6e80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000e6e90: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
-000e6ea0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e6eb0: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
-000e6ec0: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
-000e6ed0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-000e6ee0: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+000e1e80: 2072 6573 756c 745b 2763 6c75 7374 6572   result['cluster
+000e1e90: 5f69 6427 5d20 3d20 7365 6c66 2e63 6c75  _id'] = self.clu
+000e1ea0: 7374 6572 5f69 640a 2020 2020 2020 2020  ster_id.        
+000e1eb0: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+000e1ec0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000e1ed0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000e1ee0: 6c74 5b27 7265 7175 6573 745f 6964 275d  lt['request_id']
+000e1ef0: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+000e1f00: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+000e1f10: 6c66 2e74 6173 6b5f 6964 2069 7320 6e6f  lf.task_id is no
+000e1f20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e1f30: 2020 2020 7265 7375 6c74 5b27 7461 736b      result['task
+000e1f40: 5f69 6427 5d20 3d20 7365 6c66 2e74 6173  _id'] = self.tas
+000e1f50: 6b5f 6964 0a20 2020 2020 2020 2072 6574  k_id.        ret
+000e1f60: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000e1f70: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000e1f80: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000e1f90: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000e1fa0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000e1fb0: 2020 2020 6966 206d 2e67 6574 2827 636c      if m.get('cl
+000e1fc0: 7573 7465 725f 6964 2729 2069 7320 6e6f  uster_id') is no
+000e1fd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e1fe0: 2020 2020 7365 6c66 2e63 6c75 7374 6572      self.cluster
+000e1ff0: 5f69 6420 3d20 6d2e 6765 7428 2763 6c75  _id = m.get('clu
+000e2000: 7374 6572 5f69 6427 290a 2020 2020 2020  ster_id').      
+000e2010: 2020 6966 206d 2e67 6574 2827 7265 7175    if m.get('requ
+000e2020: 6573 745f 6964 2729 2069 7320 6e6f 7420  est_id') is not 
+000e2030: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e2040: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+000e2050: 6420 3d20 6d2e 6765 7428 2772 6571 7565  d = m.get('reque
+000e2060: 7374 5f69 6427 290a 2020 2020 2020 2020  st_id').        
+000e2070: 6966 206d 2e67 6574 2827 7461 736b 5f69  if m.get('task_i
+000e2080: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+000e2090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000e20a0: 662e 7461 736b 5f69 6420 3d20 6d2e 6765  f.task_id = m.ge
+000e20b0: 7428 2774 6173 6b5f 6964 2729 0a20 2020  t('task_id').   
+000e20c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000e20d0: 0a0a 0a63 6c61 7373 2053 6361 6c65 4f75  ...class ScaleOu
+000e20e0: 7443 6c75 7374 6572 5265 7370 6f6e 7365  tClusterResponse
+000e20f0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000e2100: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000e2110: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000e2120: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+000e2130: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+000e2140: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+000e2150: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+000e2160: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+000e2170: 793a 2053 6361 6c65 4f75 7443 6c75 7374  y: ScaleOutClust
+000e2180: 6572 5265 7370 6f6e 7365 426f 6479 203d  erResponseBody =
+000e2190: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000e21a0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+000e21b0: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+000e21c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000e21d0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+000e21e0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+000e21f0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
+000e2200: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000e2210: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+000e2220: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+000e2230: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000e2240: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+000e2250: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000e2260: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000e2270: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000e2280: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000e2290: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000e22a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000e22b0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000e22c0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000e22d0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000e22e0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+000e22f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e2300: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+000e2310: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+000e2320: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+000e2330: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+000e2340: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e2350: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000e2360: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+000e2370: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000e2380: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000e2390: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+000e23a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e23b0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+000e23c0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+000e23d0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+000e23e0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000e23f0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000e2400: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+000e2410: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000e2420: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+000e2430: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+000e2440: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+000e2450: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000e2460: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000e2470: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000e2480: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000e2490: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+000e24a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e24b0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000e24c0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+000e24d0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+000e24e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000e24f0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+000e2500: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e2510: 7465 6d70 5f6d 6f64 656c 203d 2053 6361  temp_model = Sca
+000e2520: 6c65 4f75 7443 6c75 7374 6572 5265 7370  leOutClusterResp
+000e2530: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+000e2540: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000e2550: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+000e2560: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+000e2570: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000e2580: 2073 656c 660a 0a0a 636c 6173 7320 5363   self...class Sc
+000e2590: 616e 436c 7573 7465 7256 756c 7352 6573  anClusterVulsRes
+000e25a0: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+000e25b0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000e25c0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000e25d0: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
+000e25e0: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
+000e25f0: 6f6e 652c 0a20 2020 2020 2020 2074 6173  one,.        tas
+000e2600: 6b5f 6964 3a20 7374 7220 3d20 4e6f 6e65  k_id: str = None
+000e2610: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+000e2620: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+000e2630: 203d 2072 6571 7565 7374 5f69 640a 2020   = request_id.  
+000e2640: 2020 2020 2020 7365 6c66 2e74 6173 6b5f        self.task_
+000e2650: 6964 203d 2074 6173 6b5f 6964 0a0a 2020  id = task_id..  
+000e2660: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000e2670: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+000e2680: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+000e2690: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+000e26a0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+000e26b0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000e26c0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+000e26d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e26e0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000e26f0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000e2700: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000e2710: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+000e2720: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000e2730: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000e2740: 6c74 5b27 7265 7175 6573 745f 6964 275d  lt['request_id']
+000e2750: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+000e2760: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+000e2770: 6c66 2e74 6173 6b5f 6964 2069 7320 6e6f  lf.task_id is no
+000e2780: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e2790: 2020 2020 7265 7375 6c74 5b27 7461 736b      result['task
+000e27a0: 5f69 6427 5d20 3d20 7365 6c66 2e74 6173  _id'] = self.tas
+000e27b0: 6b5f 6964 0a20 2020 2020 2020 2072 6574  k_id.        ret
+000e27c0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000e27d0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000e27e0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000e27f0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000e2800: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000e2810: 2020 2020 6966 206d 2e67 6574 2827 7265      if m.get('re
+000e2820: 7175 6573 745f 6964 2729 2069 7320 6e6f  quest_id') is no
+000e2830: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e2840: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+000e2850: 5f69 6420 3d20 6d2e 6765 7428 2772 6571  _id = m.get('req
+000e2860: 7565 7374 5f69 6427 290a 2020 2020 2020  uest_id').      
+000e2870: 2020 6966 206d 2e67 6574 2827 7461 736b    if m.get('task
+000e2880: 5f69 6427 2920 6973 206e 6f74 204e 6f6e  _id') is not Non
+000e2890: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000e28a0: 656c 662e 7461 736b 5f69 6420 3d20 6d2e  elf.task_id = m.
+000e28b0: 6765 7428 2774 6173 6b5f 6964 2729 0a20  get('task_id'). 
+000e28c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000e28d0: 6c66 0a0a 0a63 6c61 7373 2053 6361 6e43  lf...class ScanC
+000e28e0: 6c75 7374 6572 5675 6c73 5265 7370 6f6e  lusterVulsRespon
+000e28f0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+000e2900: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000e2910: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000e2920: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+000e2930: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+000e2940: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+000e2950: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+000e2960: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+000e2970: 6f64 793a 2053 6361 6e43 6c75 7374 6572  ody: ScanCluster
+000e2980: 5675 6c73 5265 7370 6f6e 7365 426f 6479  VulsResponseBody
+000e2990: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+000e29a0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000e29b0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+000e29c0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000e29d0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+000e29e0: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+000e29f0: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+000e2a00: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000e2a10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000e2a20: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+000e2a30: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000e2a40: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+000e2a50: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000e2a60: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000e2a70: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000e2a80: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000e2a90: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000e2aa0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e2ab0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000e2ac0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000e2ad0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000e2ae0: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+000e2af0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e2b00: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+000e2b10: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+000e2b20: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000e2b30: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000e2b40: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000e2b50: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000e2b60: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000e2b70: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000e2b80: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+000e2b90: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+000e2ba0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e2bb0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+000e2bc0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+000e2bd0: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+000e2be0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000e2bf0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000e2c00: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000e2c10: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000e2c20: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000e2c30: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+000e2c40: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+000e2c50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e2c60: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000e2c70: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000e2c80: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000e2c90: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+000e2ca0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e2cb0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000e2cc0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+000e2cd0: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000e2ce0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000e2cf0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+000e2d00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e2d10: 2020 7465 6d70 5f6d 6f64 656c 203d 2053    temp_model = S
+000e2d20: 6361 6e43 6c75 7374 6572 5675 6c73 5265  canClusterVulsRe
+000e2d30: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
+000e2d40: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000e2d50: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+000e2d60: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+000e2d70: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+000e2d80: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000e2d90: 5374 6172 7441 6c65 7274 5265 7175 6573  StartAlertReques
+000e2da0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+000e2db0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000e2dc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000e2dd0: 2020 2020 2061 6c65 7274 5f72 756c 655f       alert_rule_
+000e2de0: 6772 6f75 705f 6e61 6d65 3a20 7374 7220  group_name: str 
+000e2df0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000e2e00: 616c 6572 745f 7275 6c65 5f6e 616d 653a  alert_rule_name:
+000e2e10: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000e2e20: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
+000e2e30: 6520 6e61 6d65 206f 6620 7468 6520 616c  e name of the al
+000e2e40: 6572 7420 7275 6c65 2073 6574 2074 6f20  ert rule set to 
+000e2e50: 6265 2065 6e61 626c 6564 2e0a 2020 2020  be enabled..    
+000e2e60: 2020 2020 7365 6c66 2e61 6c65 7274 5f72      self.alert_r
+000e2e70: 756c 655f 6772 6f75 705f 6e61 6d65 203d  ule_group_name =
+000e2e80: 2061 6c65 7274 5f72 756c 655f 6772 6f75   alert_rule_grou
+000e2e90: 705f 6e61 6d65 0a20 2020 2020 2020 2023  p_name.        #
+000e2ea0: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+000e2eb0: 2061 6c65 7274 2072 756c 6520 746f 2062   alert rule to b
+000e2ec0: 6520 656e 6162 6c65 642e 2049 6620 796f  e enabled. If yo
+000e2ed0: 7520 646f 206e 6f74 2073 7065 6369 6679  u do not specify
+000e2ee0: 2061 6e20 616c 6572 7420 7275 6c65 206e   an alert rule n
+000e2ef0: 616d 652c 2074 6865 2061 6c65 7274 2072  ame, the alert r
+000e2f00: 756c 6520 7365 7420 6973 2065 6e61 626c  ule set is enabl
+000e2f10: 6564 2e0a 2020 2020 2020 2020 7365 6c66  ed..        self
+000e2f20: 2e61 6c65 7274 5f72 756c 655f 6e61 6d65  .alert_rule_name
+000e2f30: 203d 2061 6c65 7274 5f72 756c 655f 6e61   = alert_rule_na
+000e2f40: 6d65 0a0a 2020 2020 6465 6620 7661 6c69  me..    def vali
+000e2f50: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000e2f60: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000e2f70: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000e2f80: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000e2f90: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000e2fa0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000e2fb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e2fc0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000e2fd0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000e2fe0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000e2ff0: 2020 2020 2020 6966 2073 656c 662e 616c        if self.al
+000e3000: 6572 745f 7275 6c65 5f67 726f 7570 5f6e  ert_rule_group_n
+000e3010: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+000e3020: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000e3030: 756c 745b 2761 6c65 7274 5f72 756c 655f  ult['alert_rule_
+000e3040: 6772 6f75 705f 6e61 6d65 275d 203d 2073  group_name'] = s
+000e3050: 656c 662e 616c 6572 745f 7275 6c65 5f67  elf.alert_rule_g
+000e3060: 726f 7570 5f6e 616d 650a 2020 2020 2020  roup_name.      
+000e3070: 2020 6966 2073 656c 662e 616c 6572 745f    if self.alert_
+000e3080: 7275 6c65 5f6e 616d 6520 6973 206e 6f74  rule_name is not
+000e3090: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e30a0: 2020 2072 6573 756c 745b 2761 6c65 7274     result['alert
+000e30b0: 5f72 756c 655f 6e61 6d65 275d 203d 2073  _rule_name'] = s
+000e30c0: 656c 662e 616c 6572 745f 7275 6c65 5f6e  elf.alert_rule_n
+000e30d0: 616d 650a 2020 2020 2020 2020 7265 7475  ame.        retu
+000e30e0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+000e30f0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+000e3100: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+000e3110: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+000e3120: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+000e3130: 2020 2069 6620 6d2e 6765 7428 2761 6c65     if m.get('ale
+000e3140: 7274 5f72 756c 655f 6772 6f75 705f 6e61  rt_rule_group_na
+000e3150: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
+000e3160: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000e3170: 6c66 2e61 6c65 7274 5f72 756c 655f 6772  lf.alert_rule_gr
+000e3180: 6f75 705f 6e61 6d65 203d 206d 2e67 6574  oup_name = m.get
+000e3190: 2827 616c 6572 745f 7275 6c65 5f67 726f  ('alert_rule_gro
+000e31a0: 7570 5f6e 616d 6527 290a 2020 2020 2020  up_name').      
+000e31b0: 2020 6966 206d 2e67 6574 2827 616c 6572    if m.get('aler
+000e31c0: 745f 7275 6c65 5f6e 616d 6527 2920 6973  t_rule_name') is
+000e31d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e31e0: 2020 2020 2020 2073 656c 662e 616c 6572         self.aler
+000e31f0: 745f 7275 6c65 5f6e 616d 6520 3d20 6d2e  t_rule_name = m.
+000e3200: 6765 7428 2761 6c65 7274 5f72 756c 655f  get('alert_rule_
+000e3210: 6e61 6d65 2729 0a20 2020 2020 2020 2072  name').        r
+000e3220: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000e3230: 7373 2053 7461 7274 416c 6572 7452 6573  ss StartAlertRes
+000e3240: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+000e3250: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000e3260: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000e3270: 656c 662c 0a20 2020 2020 2020 206d 7367  elf,.        msg
+000e3280: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000e3290: 2020 2020 2020 7374 6174 7573 3a20 626f        status: bo
+000e32a0: 6f6c 203d 204e 6f6e 652c 0a20 2020 2029  ol = None,.    )
+000e32b0: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
+000e32c0: 6d65 7373 6167 6520 7265 7475 726e 6564  message returned
+000e32d0: 2e0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
+000e32e0: 7367 203d 206d 7367 0a20 2020 2020 2020  sg = msg.       
+000e32f0: 2023 2054 6865 2073 7461 7475 732e 0a20   # The status.. 
+000e3300: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000e3310: 7573 203d 2073 7461 7475 730a 0a20 2020  us = status..   
+000e3320: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000e3330: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000e3340: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+000e3350: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000e3360: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+000e3370: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000e3380: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+000e3390: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e33a0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+000e33b0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000e33c0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000e33d0: 6620 7365 6c66 2e6d 7367 2069 7320 6e6f  f self.msg is no
+000e33e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e33f0: 2020 2020 7265 7375 6c74 5b27 6d73 6727      result['msg'
+000e3400: 5d20 3d20 7365 6c66 2e6d 7367 0a20 2020  ] = self.msg.   
+000e3410: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+000e3420: 7475 7320 6973 206e 6f74 204e 6f6e 653a  tus is not None:
+000e3430: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000e3440: 756c 745b 2773 7461 7475 7327 5d20 3d20  ult['status'] = 
+000e3450: 7365 6c66 2e73 7461 7475 730a 2020 2020  self.status.    
+000e3460: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000e3470: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000e3480: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000e3490: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000e34a0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000e34b0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+000e34c0: 6765 7428 276d 7367 2729 2069 7320 6e6f  get('msg') is no
+000e34d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e34e0: 2020 2020 7365 6c66 2e6d 7367 203d 206d      self.msg = m
+000e34f0: 2e67 6574 2827 6d73 6727 290a 2020 2020  .get('msg').    
+000e3500: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+000e3510: 6174 7573 2729 2069 7320 6e6f 7420 4e6f  atus') is not No
+000e3520: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e3530: 7365 6c66 2e73 7461 7475 7320 3d20 6d2e  self.status = m.
+000e3540: 6765 7428 2773 7461 7475 7327 290a 2020  get('status').  
+000e3550: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000e3560: 660a 0a0a 636c 6173 7320 5374 6172 7441  f...class StartA
+000e3570: 6c65 7274 5265 7370 6f6e 7365 2854 6561  lertResponse(Tea
+000e3580: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000e3590: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000e35a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000e35b0: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+000e35c0: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+000e35d0: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+000e35e0: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+000e35f0: 0a20 2020 2020 2020 2062 6f64 793a 2053  .        body: S
+000e3600: 7461 7274 416c 6572 7452 6573 706f 6e73  tartAlertRespons
+000e3610: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+000e3620: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+000e3630: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+000e3640: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+000e3650: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000e3660: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000e3670: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+000e3680: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+000e3690: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000e36a0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+000e36b0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+000e36c0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+000e36d0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+000e36e0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+000e36f0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000e3700: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+000e3710: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+000e3720: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e3730: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000e3740: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000e3750: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000e3760: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+000e3770: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e3780: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000e3790: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+000e37a0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+000e37b0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+000e37c0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+000e37d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e37e0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+000e37f0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+000e3800: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+000e3810: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+000e3820: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e3830: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+000e3840: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+000e3850: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000e3860: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000e3870: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000e3880: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000e3890: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+000e38a0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+000e38b0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000e38c0: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+000e38d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e38e0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+000e38f0: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+000e3900: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+000e3910: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000e3920: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+000e3930: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000e3940: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000e3950: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000e3960: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+000e3970: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+000e3980: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e3990: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000e39a0: 6c20 3d20 5374 6172 7441 6c65 7274 5265  l = StartAlertRe
+000e39b0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
+000e39c0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000e39d0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+000e39e0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+000e39f0: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+000e3a00: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000e3a10: 5374 6172 7457 6f72 6b66 6c6f 7752 6571  StartWorkflowReq
+000e3a20: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+000e3a30: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000e3a40: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000e3a50: 2020 2020 2020 2020 6d61 7070 696e 675f          mapping_
+000e3a60: 6261 6d5f 6f75 745f 6669 6c65 6e61 6d65  bam_out_filename
+000e3a70: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000e3a80: 2020 2020 2020 6d61 7070 696e 675f 6261        mapping_ba
+000e3a90: 6d5f 6f75 745f 7061 7468 3a20 7374 7220  m_out_path: str 
+000e3aa0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000e3ab0: 6d61 7070 696e 675f 6275 636b 6574 5f6e  mapping_bucket_n
+000e3ac0: 616d 653a 2073 7472 203d 204e 6f6e 652c  ame: str = None,
+000e3ad0: 0a20 2020 2020 2020 206d 6170 7069 6e67  .        mapping
+000e3ae0: 5f66 6173 7471 5f66 6972 7374 5f66 696c  _fastq_first_fil
+000e3af0: 656e 616d 653a 2073 7472 203d 204e 6f6e  ename: str = Non
+000e3b00: 652c 0a20 2020 2020 2020 206d 6170 7069  e,.        mappi
+000e3b10: 6e67 5f66 6173 7471 5f70 6174 683a 2073  ng_fastq_path: s
+000e3b20: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000e3b30: 2020 206d 6170 7069 6e67 5f66 6173 7471     mapping_fastq
+000e3b40: 5f73 6563 6f6e 645f 6669 6c65 6e61 6d65  _second_filename
+000e3b50: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000e3b60: 2020 2020 2020 6d61 7070 696e 675f 6973        mapping_is
+000e3b70: 5f6d 6172 6b5f 6475 703a 2073 7472 203d  _mark_dup: str =
+000e3b80: 204e 6f6e 652c 0a20 2020 2020 2020 206d   None,.        m
+000e3b90: 6170 7069 6e67 5f6f 7373 5f72 6567 696f  apping_oss_regio
+000e3ba0: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
+000e3bb0: 2020 2020 2020 206d 6170 7069 6e67 5f72         mapping_r
+000e3bc0: 6566 6572 656e 6365 5f70 6174 683a 2073  eference_path: s
+000e3bd0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000e3be0: 2020 2073 6572 7669 6365 3a20 7374 7220     service: str 
+000e3bf0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000e3c00: 7767 735f 6275 636b 6574 5f6e 616d 653a  wgs_bucket_name:
+000e3c10: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000e3c20: 2020 2020 2077 6773 5f66 6173 7471 5f66       wgs_fastq_f
+000e3c30: 6972 7374 5f66 696c 656e 616d 653a 2073  irst_filename: s
+000e3c40: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000e3c50: 2020 2077 6773 5f66 6173 7471 5f70 6174     wgs_fastq_pat
+000e3c60: 683a 2073 7472 203d 204e 6f6e 652c 0a20  h: str = None,. 
+000e3c70: 2020 2020 2020 2077 6773 5f66 6173 7471         wgs_fastq
+000e3c80: 5f73 6563 6f6e 645f 6669 6c65 6e61 6d65  _second_filename
+000e3c90: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000e3ca0: 2020 2020 2020 7767 735f 6f73 735f 7265        wgs_oss_re
+000e3cb0: 6769 6f6e 3a20 7374 7220 3d20 4e6f 6e65  gion: str = None
+000e3cc0: 2c0a 2020 2020 2020 2020 7767 735f 7265  ,.        wgs_re
+000e3cd0: 6665 7265 6e63 655f 7061 7468 3a20 7374  ference_path: st
+000e3ce0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000e3cf0: 2020 7767 735f 7663 665f 6f75 745f 6669    wgs_vcf_out_fi
+000e3d00: 6c65 6e61 6d65 3a20 7374 7220 3d20 4e6f  lename: str = No
+000e3d10: 6e65 2c0a 2020 2020 2020 2020 7767 735f  ne,.        wgs_
+000e3d20: 7663 665f 6f75 745f 7061 7468 3a20 7374  vcf_out_path: st
+000e3d30: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000e3d40: 2020 776f 726b 666c 6f77 5f74 7970 653a    workflow_type:
+000e3d50: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000e3d60: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
+000e3d70: 6520 6e61 6d65 206f 6620 7468 6520 6f75  e name of the ou
+000e3d80: 7470 7574 2042 414d 2066 696c 652e 0a20  tput BAM file.. 
+000e3d90: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+000e3da0: 696e 675f 6261 6d5f 6f75 745f 6669 6c65  ing_bam_out_file
+000e3db0: 6e61 6d65 203d 206d 6170 7069 6e67 5f62  name = mapping_b
+000e3dc0: 616d 5f6f 7574 5f66 696c 656e 616d 650a  am_out_filename.
+000e3dd0: 2020 2020 2020 2020 2320 5468 6520 6f75          # The ou
+000e3de0: 7470 7574 2070 6174 6820 6f66 2074 6865  tput path of the
+000e3df0: 2042 696e 6172 7920 416c 6967 6e6d 656e   Binary Alignmen
+000e3e00: 7420 4d61 7020 2842 414d 2920 6669 6c65  t Map (BAM) file
+000e3e10: 2e0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
+000e3e20: 6170 7069 6e67 5f62 616d 5f6f 7574 5f70  apping_bam_out_p
+000e3e30: 6174 6820 3d20 6d61 7070 696e 675f 6261  ath = mapping_ba
+000e3e40: 6d5f 6f75 745f 7061 7468 0a20 2020 2020  m_out_path.     
+000e3e50: 2020 2023 2054 6865 206e 616d 6520 6f66     # The name of
+000e3e60: 2074 6865 204f 5353 2062 7563 6b65 7420   the OSS bucket 
+000e3e70: 7468 6174 2073 746f 7265 7320 7468 6520  that stores the 
+000e3e80: 6461 7461 206f 6620 7468 6520 6d61 7070  data of the mapp
+000e3e90: 696e 6720 776f 726b 666c 6f77 2e0a 2020  ing workflow..  
+000e3ea0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+000e3eb0: 6e67 5f62 7563 6b65 745f 6e61 6d65 203d  ng_bucket_name =
+000e3ec0: 206d 6170 7069 6e67 5f62 7563 6b65 745f   mapping_bucket_
+000e3ed0: 6e61 6d65 0a20 2020 2020 2020 2023 2054  name.        # T
+000e3ee0: 6865 206e 616d 6520 6f66 2074 6865 2066  he name of the f
+000e3ef0: 6972 7374 2046 4153 5451 2066 696c 6520  irst FASTQ file 
+000e3f00: 6f66 2074 6865 206d 6170 7069 6e67 2077  of the mapping w
+000e3f10: 6f72 6b66 6c6f 772e 0a20 2020 2020 2020  orkflow..       
+000e3f20: 2073 656c 662e 6d61 7070 696e 675f 6661   self.mapping_fa
+000e3f30: 7374 715f 6669 7273 745f 6669 6c65 6e61  stq_first_filena
+000e3f40: 6d65 203d 206d 6170 7069 6e67 5f66 6173  me = mapping_fas
+000e3f50: 7471 5f66 6972 7374 5f66 696c 656e 616d  tq_first_filenam
+000e3f60: 650a 2020 2020 2020 2020 2320 5468 6520  e.        # The 
+000e3f70: 7061 7468 206f 6620 7468 6520 4641 5354  path of the FAST
+000e3f80: 5120 6669 6c65 7320 6f66 2074 6865 206d  Q files of the m
+000e3f90: 6170 7069 6e67 2077 6f72 6b66 6c6f 772e  apping workflow.
+000e3fa0: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+000e3fb0: 7070 696e 675f 6661 7374 715f 7061 7468  pping_fastq_path
+000e3fc0: 203d 206d 6170 7069 6e67 5f66 6173 7471   = mapping_fastq
+000e3fd0: 5f70 6174 680a 2020 2020 2020 2020 2320  _path.        # 
+000e3fe0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+000e3ff0: 7365 636f 6e64 2046 4153 5451 2066 696c  second FASTQ fil
+000e4000: 6520 6f66 2074 6865 206d 6170 7069 6e67  e of the mapping
+000e4010: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
+000e4020: 2020 2073 656c 662e 6d61 7070 696e 675f     self.mapping_
+000e4030: 6661 7374 715f 7365 636f 6e64 5f66 696c  fastq_second_fil
+000e4040: 656e 616d 6520 3d20 6d61 7070 696e 675f  ename = mapping_
+000e4050: 6661 7374 715f 7365 636f 6e64 5f66 696c  fastq_second_fil
+000e4060: 656e 616d 650a 2020 2020 2020 2020 2320  ename.        # 
+000e4070: 5370 6563 6966 6965 7320 7768 6574 6865  Specifies whethe
+000e4080: 7220 746f 206d 6172 6b20 6475 706c 6963  r to mark duplic
+000e4090: 6174 6520 7661 6c75 6573 2e0a 2020 2020  ate values..    
+000e40a0: 2020 2020 7365 6c66 2e6d 6170 7069 6e67      self.mapping
+000e40b0: 5f69 735f 6d61 726b 5f64 7570 203d 206d  _is_mark_dup = m
+000e40c0: 6170 7069 6e67 5f69 735f 6d61 726b 5f64  apping_is_mark_d
+000e40d0: 7570 0a20 2020 2020 2020 2023 2054 6865  up.        # The
+000e40e0: 2072 6567 696f 6e20 7768 6572 6520 7468   region where th
+000e40f0: 6520 4f62 6a65 6374 2053 746f 7261 6765  e Object Storage
+000e4100: 2053 6572 7669 6365 2028 4f53 5329 2062   Service (OSS) b
+000e4110: 7563 6b65 7420 7468 6174 2073 746f 7265  ucket that store
+000e4120: 7320 7468 6520 6461 7461 206f 6620 7468  s the data of th
+000e4130: 6520 6d61 7070 696e 6720 776f 726b 666c  e mapping workfl
+000e4140: 6f77 2069 7320 6465 706c 6f79 6564 2e0a  ow is deployed..
+000e4150: 2020 2020 2020 2020 7365 6c66 2e6d 6170          self.map
+000e4160: 7069 6e67 5f6f 7373 5f72 6567 696f 6e20  ping_oss_region 
+000e4170: 3d20 6d61 7070 696e 675f 6f73 735f 7265  = mapping_oss_re
+000e4180: 6769 6f6e 0a20 2020 2020 2020 2023 2054  gion.        # T
+000e4190: 6865 2070 6174 6820 6f66 2074 6865 2072  he path of the r
+000e41a0: 6566 6572 656e 6365 2066 696c 6573 206f  eference files o
+000e41b0: 6620 7468 6520 6d61 7070 696e 6720 776f  f the mapping wo
+000e41c0: 726b 666c 6f77 2e0a 2020 2020 2020 2020  rkflow..        
+000e41d0: 7365 6c66 2e6d 6170 7069 6e67 5f72 6566  self.mapping_ref
+000e41e0: 6572 656e 6365 5f70 6174 6820 3d20 6d61  erence_path = ma
+000e41f0: 7070 696e 675f 7265 6665 7265 6e63 655f  pping_reference_
+000e4200: 7061 7468 0a20 2020 2020 2020 2023 2054  path.        # T
+000e4210: 6865 2074 7970 6520 6f66 2073 6572 7669  he type of servi
+000e4220: 6365 2d6c 6576 656c 2061 6772 6565 6d65  ce-level agreeme
+000e4230: 6e74 2028 534c 4129 2e20 5661 6c69 6420  nt (SLA). Valid 
+000e4240: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+000e4250: 2320 0a20 2020 2020 2020 2023 202a 2020  # .        # *  
+000e4260: 2073 3a20 7468 6520 7369 6c76 6572 206c   s: the silver l
+000e4270: 6576 656c 2028 532d 6c65 7665 6c29 2e20  evel (S-level). 
+000e4280: 4974 2072 6571 7569 7265 7320 3120 6578  It requires 1 ex
+000e4290: 7472 6120 6d69 6e75 7465 2074 6f20 7072  tra minute to pr
+000e42a0: 6f63 6573 7320 6576 6572 7920 312e 3520  ocess every 1.5 
+000e42b0: 6269 6c6c 696f 6e20 6261 7365 2070 6169  billion base pai
+000e42c0: 7273 2062 6579 6f6e 6420 7468 6520 6c69  rs beyond the li
+000e42d0: 6d69 7420 6f66 2039 3020 6269 6c6c 696f  mit of 90 billio
+000e42e0: 6e20 6261 7365 2070 6169 7273 2e0a 2020  n base pairs..  
+000e42f0: 2020 2020 2020 2320 2a20 2020 673a 2074        # *   g: t
+000e4300: 6865 2067 6f6c 6420 6c65 7665 6c20 2847  he gold level (G
+000e4310: 2d6c 6576 656c 292e 2049 7420 7265 7175  -level). It requ
+000e4320: 6972 6573 2031 2065 7874 7261 206d 696e  ires 1 extra min
+000e4330: 7574 6520 746f 2070 726f 6365 7373 2065  ute to process e
+000e4340: 7665 7279 2032 2062 696c 6c69 6f6e 2062  very 2 billion b
+000e4350: 6173 6520 7061 6972 7320 6265 796f 6e64  ase pairs beyond
+000e4360: 2074 6865 206c 696d 6974 206f 6620 3930   the limit of 90
+000e4370: 2062 696c 6c69 6f6e 2062 6173 6520 7061   billion base pa
+000e4380: 6972 732e 0a20 2020 2020 2020 2023 202a  irs..        # *
+000e4390: 2020 2070 3a20 7468 6520 706c 6174 696e     p: the platin
+000e43a0: 756d 206c 6576 656c 2028 502d 6c65 7665  um level (P-leve
+000e43b0: 6c29 2e20 4974 2072 6571 7569 7265 7320  l). It requires 
+000e43c0: 3120 6578 7472 6120 6d69 6e75 7465 2074  1 extra minute t
+000e43d0: 6f20 7072 6f63 6573 7320 6576 6572 7920  o process every 
+000e43e0: 3320 6269 6c6c 696f 6e20 6261 7365 2070  3 billion base p
+000e43f0: 6169 7273 2062 6579 6f6e 6420 7468 6520  airs beyond the 
+000e4400: 6c69 6d69 7420 6f66 2039 3020 6269 6c6c  limit of 90 bill
+000e4410: 696f 6e20 6261 7365 2070 6169 7273 2e0a  ion base pairs..
+000e4420: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+000e4430: 7669 6365 203d 2073 6572 7669 6365 0a20  vice = service. 
+000e4440: 2020 2020 2020 2023 2054 6865 206e 616d         # The nam
+000e4450: 6520 6f66 2074 6865 204f 5353 2062 7563  e of the OSS buc
+000e4460: 6b65 7420 7468 6174 2073 746f 7265 7320  ket that stores 
+000e4470: 7468 6520 6461 7461 206f 6620 7468 6520  the data of the 
+000e4480: 5747 5320 776f 726b 666c 6f77 2e0a 2020  WGS workflow..  
+000e4490: 2020 2020 2020 7365 6c66 2e77 6773 5f62        self.wgs_b
+000e44a0: 7563 6b65 745f 6e61 6d65 203d 2077 6773  ucket_name = wgs
+000e44b0: 5f62 7563 6b65 745f 6e61 6d65 0a20 2020  _bucket_name.   
+000e44c0: 2020 2020 2023 2054 6865 206e 616d 6520       # The name 
+000e44d0: 6f66 2074 6865 2066 6972 7374 2046 4153  of the first FAS
+000e44e0: 5451 2066 696c 6520 6f66 2074 6865 2057  TQ file of the W
+000e44f0: 4753 2077 6f72 6b66 6c6f 772e 0a20 2020  GS workflow..   
+000e4500: 2020 2020 2073 656c 662e 7767 735f 6661       self.wgs_fa
+000e4510: 7374 715f 6669 7273 745f 6669 6c65 6e61  stq_first_filena
+000e4520: 6d65 203d 2077 6773 5f66 6173 7471 5f66  me = wgs_fastq_f
+000e4530: 6972 7374 5f66 696c 656e 616d 650a 2020  irst_filename.  
+000e4540: 2020 2020 2020 2320 5468 6520 7061 7468        # The path
+000e4550: 206f 6620 7468 6520 4641 5354 5120 6669   of the FASTQ fi
+000e4560: 6c65 7320 6f66 2074 6865 2057 4753 2077  les of the WGS w
+000e4570: 6f72 6b66 6c6f 772e 0a20 2020 2020 2020  orkflow..       
+000e4580: 2073 656c 662e 7767 735f 6661 7374 715f   self.wgs_fastq_
+000e4590: 7061 7468 203d 2077 6773 5f66 6173 7471  path = wgs_fastq
+000e45a0: 5f70 6174 680a 2020 2020 2020 2020 2320  _path.        # 
+000e45b0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+000e45c0: 7365 636f 6e64 2046 4153 5451 2066 696c  second FASTQ fil
+000e45d0: 6520 6f66 2074 6865 2057 4753 2077 6f72  e of the WGS wor
+000e45e0: 6b66 6c6f 772e 0a20 2020 2020 2020 2073  kflow..        s
+000e45f0: 656c 662e 7767 735f 6661 7374 715f 7365  elf.wgs_fastq_se
+000e4600: 636f 6e64 5f66 696c 656e 616d 6520 3d20  cond_filename = 
+000e4610: 7767 735f 6661 7374 715f 7365 636f 6e64  wgs_fastq_second
+000e4620: 5f66 696c 656e 616d 650a 2020 2020 2020  _filename.      
+000e4630: 2020 2320 5468 6520 7265 6769 6f6e 2077    # The region w
+000e4640: 6865 7265 2074 6865 204f 5353 2062 7563  here the OSS buc
+000e4650: 6b65 7420 7468 6174 2073 746f 7265 7320  ket that stores 
+000e4660: 7468 6520 6461 7461 206f 6620 7468 6520  the data of the 
+000e4670: 7768 6f6c 6520 6765 6e6f 6d65 2073 6571  whole genome seq
+000e4680: 7565 6e63 696e 6720 2857 4753 2920 776f  uencing (WGS) wo
+000e4690: 726b 666c 6f77 2069 7320 6465 706c 6f79  rkflow is deploy
+000e46a0: 6564 2e0a 2020 2020 2020 2020 7365 6c66  ed..        self
+000e46b0: 2e77 6773 5f6f 7373 5f72 6567 696f 6e20  .wgs_oss_region 
+000e46c0: 3d20 7767 735f 6f73 735f 7265 6769 6f6e  = wgs_oss_region
+000e46d0: 0a20 2020 2020 2020 2023 2054 6865 2070  .        # The p
+000e46e0: 6174 6820 6f66 2074 6865 2072 6566 6572  ath of the refer
+000e46f0: 656e 6365 2066 696c 6573 206f 6620 7468  ence files of th
+000e4700: 6520 5747 5320 776f 726b 666c 6f77 2e0a  e WGS workflow..
+000e4710: 2020 2020 2020 2020 7365 6c66 2e77 6773          self.wgs
+000e4720: 5f72 6566 6572 656e 6365 5f70 6174 6820  _reference_path 
+000e4730: 3d20 7767 735f 7265 6665 7265 6e63 655f  = wgs_reference_
+000e4740: 7061 7468 0a20 2020 2020 2020 2023 2054  path.        # T
+000e4750: 6865 206e 616d 6520 6f66 2074 6865 206f  he name of the o
+000e4760: 7574 7075 7420 5643 4620 6669 6c65 2e0a  utput VCF file..
+000e4770: 2020 2020 2020 2020 7365 6c66 2e77 6773          self.wgs
+000e4780: 5f76 6366 5f6f 7574 5f66 696c 656e 616d  _vcf_out_filenam
+000e4790: 6520 3d20 7767 735f 7663 665f 6f75 745f  e = wgs_vcf_out_
+000e47a0: 6669 6c65 6e61 6d65 0a20 2020 2020 2020  filename.       
+000e47b0: 2023 2054 6865 206f 7574 7075 7420 7061   # The output pa
+000e47c0: 7468 206f 6620 7468 6520 5661 7269 616e  th of the Varian
+000e47d0: 7420 4361 6c6c 2046 6f72 6d61 7420 2856  t Call Format (V
+000e47e0: 4346 2920 6669 6c65 2e0a 2020 2020 2020  CF) file..      
+000e47f0: 2020 7365 6c66 2e77 6773 5f76 6366 5f6f    self.wgs_vcf_o
+000e4800: 7574 5f70 6174 6820 3d20 7767 735f 7663  ut_path = wgs_vc
+000e4810: 665f 6f75 745f 7061 7468 0a20 2020 2020  f_out_path.     
+000e4820: 2020 2023 2054 6865 2074 7970 6520 6f66     # The type of
+000e4830: 2077 6f72 6b66 6c6f 772e 2056 616c 6964   workflow. Valid
+000e4840: 2076 616c 7565 733a 2077 6773 2061 6e64   values: wgs and
+000e4850: 206d 6170 7069 6e67 2e0a 2020 2020 2020   mapping..      
+000e4860: 2020 2320 0a20 2020 2020 2020 2023 2054    # .        # T
+000e4870: 6869 7320 7061 7261 6d65 7465 7220 6973  his parameter is
+000e4880: 2072 6571 7569 7265 642e 0a20 2020 2020   required..     
+000e4890: 2020 2073 656c 662e 776f 726b 666c 6f77     self.workflow
+000e48a0: 5f74 7970 6520 3d20 776f 726b 666c 6f77  _type = workflow
+000e48b0: 5f74 7970 650a 0a20 2020 2064 6566 2076  _type..    def v
+000e48c0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000e48d0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000e48e0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000e48f0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000e4900: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000e4910: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000e4920: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+000e4930: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000e4940: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+000e4950: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+000e4960: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000e4970: 2e6d 6170 7069 6e67 5f62 616d 5f6f 7574  .mapping_bam_out
+000e4980: 5f66 696c 656e 616d 6520 6973 206e 6f74  _filename is not
+000e4990: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e49a0: 2020 2072 6573 756c 745b 276d 6170 7069     result['mappi
+000e49b0: 6e67 5f62 616d 5f6f 7574 5f66 696c 656e  ng_bam_out_filen
+000e49c0: 616d 6527 5d20 3d20 7365 6c66 2e6d 6170  ame'] = self.map
+000e49d0: 7069 6e67 5f62 616d 5f6f 7574 5f66 696c  ping_bam_out_fil
+000e49e0: 656e 616d 650a 2020 2020 2020 2020 6966  ename.        if
+000e49f0: 2073 656c 662e 6d61 7070 696e 675f 6261   self.mapping_ba
+000e4a00: 6d5f 6f75 745f 7061 7468 2069 7320 6e6f  m_out_path is no
+000e4a10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e4a20: 2020 2020 7265 7375 6c74 5b27 6d61 7070      result['mapp
+000e4a30: 696e 675f 6261 6d5f 6f75 745f 7061 7468  ing_bam_out_path
+000e4a40: 275d 203d 2073 656c 662e 6d61 7070 696e  '] = self.mappin
+000e4a50: 675f 6261 6d5f 6f75 745f 7061 7468 0a20  g_bam_out_path. 
+000e4a60: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+000e4a70: 6170 7069 6e67 5f62 7563 6b65 745f 6e61  apping_bucket_na
+000e4a80: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+000e4a90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000e4aa0: 6c74 5b27 6d61 7070 696e 675f 6275 636b  lt['mapping_buck
+000e4ab0: 6574 5f6e 616d 6527 5d20 3d20 7365 6c66  et_name'] = self
+000e4ac0: 2e6d 6170 7069 6e67 5f62 7563 6b65 745f  .mapping_bucket_
+000e4ad0: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+000e4ae0: 7365 6c66 2e6d 6170 7069 6e67 5f66 6173  self.mapping_fas
+000e4af0: 7471 5f66 6972 7374 5f66 696c 656e 616d  tq_first_filenam
+000e4b00: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000e4b10: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000e4b20: 745b 276d 6170 7069 6e67 5f66 6173 7471  t['mapping_fastq
+000e4b30: 5f66 6972 7374 5f66 696c 656e 616d 6527  _first_filename'
+000e4b40: 5d20 3d20 7365 6c66 2e6d 6170 7069 6e67  ] = self.mapping
+000e4b50: 5f66 6173 7471 5f66 6972 7374 5f66 696c  _fastq_first_fil
+000e4b60: 656e 616d 650a 2020 2020 2020 2020 6966  ename.        if
+000e4b70: 2073 656c 662e 6d61 7070 696e 675f 6661   self.mapping_fa
+000e4b80: 7374 715f 7061 7468 2069 7320 6e6f 7420  stq_path is not 
+000e4b90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e4ba0: 2020 7265 7375 6c74 5b27 6d61 7070 696e    result['mappin
+000e4bb0: 675f 6661 7374 715f 7061 7468 275d 203d  g_fastq_path'] =
+000e4bc0: 2073 656c 662e 6d61 7070 696e 675f 6661   self.mapping_fa
+000e4bd0: 7374 715f 7061 7468 0a20 2020 2020 2020  stq_path.       
+000e4be0: 2069 6620 7365 6c66 2e6d 6170 7069 6e67   if self.mapping
+000e4bf0: 5f66 6173 7471 5f73 6563 6f6e 645f 6669  _fastq_second_fi
+000e4c00: 6c65 6e61 6d65 2069 7320 6e6f 7420 4e6f  lename is not No
+000e4c10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e4c20: 7265 7375 6c74 5b27 6d61 7070 696e 675f  result['mapping_
+000e4c30: 6661 7374 715f 7365 636f 6e64 5f66 696c  fastq_second_fil
+000e4c40: 656e 616d 6527 5d20 3d20 7365 6c66 2e6d  ename'] = self.m
+000e4c50: 6170 7069 6e67 5f66 6173 7471 5f73 6563  apping_fastq_sec
+000e4c60: 6f6e 645f 6669 6c65 6e61 6d65 0a20 2020  ond_filename.   
+000e4c70: 2020 2020 2069 6620 7365 6c66 2e6d 6170       if self.map
+000e4c80: 7069 6e67 5f69 735f 6d61 726b 5f64 7570  ping_is_mark_dup
+000e4c90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e4ca0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000e4cb0: 5b27 6d61 7070 696e 675f 6973 5f6d 6172  ['mapping_is_mar
+000e4cc0: 6b5f 6475 7027 5d20 3d20 7365 6c66 2e6d  k_dup'] = self.m
+000e4cd0: 6170 7069 6e67 5f69 735f 6d61 726b 5f64  apping_is_mark_d
+000e4ce0: 7570 0a20 2020 2020 2020 2069 6620 7365  up.        if se
+000e4cf0: 6c66 2e6d 6170 7069 6e67 5f6f 7373 5f72  lf.mapping_oss_r
+000e4d00: 6567 696f 6e20 6973 206e 6f74 204e 6f6e  egion is not Non
+000e4d10: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e4d20: 6573 756c 745b 276d 6170 7069 6e67 5f6f  esult['mapping_o
+000e4d30: 7373 5f72 6567 696f 6e27 5d20 3d20 7365  ss_region'] = se
+000e4d40: 6c66 2e6d 6170 7069 6e67 5f6f 7373 5f72  lf.mapping_oss_r
+000e4d50: 6567 696f 6e0a 2020 2020 2020 2020 6966  egion.        if
+000e4d60: 2073 656c 662e 6d61 7070 696e 675f 7265   self.mapping_re
+000e4d70: 6665 7265 6e63 655f 7061 7468 2069 7320  ference_path is 
+000e4d80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e4d90: 2020 2020 2020 7265 7375 6c74 5b27 6d61        result['ma
+000e4da0: 7070 696e 675f 7265 6665 7265 6e63 655f  pping_reference_
+000e4db0: 7061 7468 275d 203d 2073 656c 662e 6d61  path'] = self.ma
+000e4dc0: 7070 696e 675f 7265 6665 7265 6e63 655f  pping_reference_
+000e4dd0: 7061 7468 0a20 2020 2020 2020 2069 6620  path.        if 
+000e4de0: 7365 6c66 2e73 6572 7669 6365 2069 7320  self.service is 
+000e4df0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e4e00: 2020 2020 2020 7265 7375 6c74 5b27 7365        result['se
+000e4e10: 7276 6963 6527 5d20 3d20 7365 6c66 2e73  rvice'] = self.s
+000e4e20: 6572 7669 6365 0a20 2020 2020 2020 2069  ervice.        i
+000e4e30: 6620 7365 6c66 2e77 6773 5f62 7563 6b65  f self.wgs_bucke
+000e4e40: 745f 6e61 6d65 2069 7320 6e6f 7420 4e6f  t_name is not No
+000e4e50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e4e60: 7265 7375 6c74 5b27 7767 735f 6275 636b  result['wgs_buck
+000e4e70: 6574 5f6e 616d 6527 5d20 3d20 7365 6c66  et_name'] = self
+000e4e80: 2e77 6773 5f62 7563 6b65 745f 6e61 6d65  .wgs_bucket_name
+000e4e90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000e4ea0: 2e77 6773 5f66 6173 7471 5f66 6972 7374  .wgs_fastq_first
+000e4eb0: 5f66 696c 656e 616d 6520 6973 206e 6f74  _filename is not
+000e4ec0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e4ed0: 2020 2072 6573 756c 745b 2777 6773 5f66     result['wgs_f
+000e4ee0: 6173 7471 5f66 6972 7374 5f66 696c 656e  astq_first_filen
+000e4ef0: 616d 6527 5d20 3d20 7365 6c66 2e77 6773  ame'] = self.wgs
+000e4f00: 5f66 6173 7471 5f66 6972 7374 5f66 696c  _fastq_first_fil
+000e4f10: 656e 616d 650a 2020 2020 2020 2020 6966  ename.        if
+000e4f20: 2073 656c 662e 7767 735f 6661 7374 715f   self.wgs_fastq_
+000e4f30: 7061 7468 2069 7320 6e6f 7420 4e6f 6e65  path is not None
+000e4f40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000e4f50: 7375 6c74 5b27 7767 735f 6661 7374 715f  sult['wgs_fastq_
+000e4f60: 7061 7468 275d 203d 2073 656c 662e 7767  path'] = self.wg
+000e4f70: 735f 6661 7374 715f 7061 7468 0a20 2020  s_fastq_path.   
+000e4f80: 2020 2020 2069 6620 7365 6c66 2e77 6773       if self.wgs
+000e4f90: 5f66 6173 7471 5f73 6563 6f6e 645f 6669  _fastq_second_fi
+000e4fa0: 6c65 6e61 6d65 2069 7320 6e6f 7420 4e6f  lename is not No
+000e4fb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e4fc0: 7265 7375 6c74 5b27 7767 735f 6661 7374  result['wgs_fast
+000e4fd0: 715f 7365 636f 6e64 5f66 696c 656e 616d  q_second_filenam
+000e4fe0: 6527 5d20 3d20 7365 6c66 2e77 6773 5f66  e'] = self.wgs_f
+000e4ff0: 6173 7471 5f73 6563 6f6e 645f 6669 6c65  astq_second_file
+000e5000: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+000e5010: 7365 6c66 2e77 6773 5f6f 7373 5f72 6567  self.wgs_oss_reg
+000e5020: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+000e5030: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000e5040: 756c 745b 2777 6773 5f6f 7373 5f72 6567  ult['wgs_oss_reg
+000e5050: 696f 6e27 5d20 3d20 7365 6c66 2e77 6773  ion'] = self.wgs
+000e5060: 5f6f 7373 5f72 6567 696f 6e0a 2020 2020  _oss_region.    
+000e5070: 2020 2020 6966 2073 656c 662e 7767 735f      if self.wgs_
+000e5080: 7265 6665 7265 6e63 655f 7061 7468 2069  reference_path i
+000e5090: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e50a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e50b0: 7767 735f 7265 6665 7265 6e63 655f 7061  wgs_reference_pa
+000e50c0: 7468 275d 203d 2073 656c 662e 7767 735f  th'] = self.wgs_
+000e50d0: 7265 6665 7265 6e63 655f 7061 7468 0a20  reference_path. 
+000e50e0: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
+000e50f0: 6773 5f76 6366 5f6f 7574 5f66 696c 656e  gs_vcf_out_filen
+000e5100: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+000e5110: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000e5120: 756c 745b 2777 6773 5f76 6366 5f6f 7574  ult['wgs_vcf_out
+000e5130: 5f66 696c 656e 616d 6527 5d20 3d20 7365  _filename'] = se
+000e5140: 6c66 2e77 6773 5f76 6366 5f6f 7574 5f66  lf.wgs_vcf_out_f
+000e5150: 696c 656e 616d 650a 2020 2020 2020 2020  ilename.        
+000e5160: 6966 2073 656c 662e 7767 735f 7663 665f  if self.wgs_vcf_
+000e5170: 6f75 745f 7061 7468 2069 7320 6e6f 7420  out_path is not 
+000e5180: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e5190: 2020 7265 7375 6c74 5b27 7767 735f 7663    result['wgs_vc
+000e51a0: 665f 6f75 745f 7061 7468 275d 203d 2073  f_out_path'] = s
+000e51b0: 656c 662e 7767 735f 7663 665f 6f75 745f  elf.wgs_vcf_out_
+000e51c0: 7061 7468 0a20 2020 2020 2020 2069 6620  path.        if 
+000e51d0: 7365 6c66 2e77 6f72 6b66 6c6f 775f 7479  self.workflow_ty
+000e51e0: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
+000e51f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000e5200: 6c74 5b27 776f 726b 666c 6f77 5f74 7970  lt['workflow_typ
+000e5210: 6527 5d20 3d20 7365 6c66 2e77 6f72 6b66  e'] = self.workf
+000e5220: 6c6f 775f 7479 7065 0a20 2020 2020 2020  low_type.       
+000e5230: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000e5240: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000e5250: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+000e5260: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+000e5270: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+000e5280: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000e5290: 2827 6d61 7070 696e 675f 6261 6d5f 6f75  ('mapping_bam_ou
+000e52a0: 745f 6669 6c65 6e61 6d65 2729 2069 7320  t_filename') is 
+000e52b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e52c0: 2020 2020 2020 7365 6c66 2e6d 6170 7069        self.mappi
+000e52d0: 6e67 5f62 616d 5f6f 7574 5f66 696c 656e  ng_bam_out_filen
+000e52e0: 616d 6520 3d20 6d2e 6765 7428 276d 6170  ame = m.get('map
+000e52f0: 7069 6e67 5f62 616d 5f6f 7574 5f66 696c  ping_bam_out_fil
+000e5300: 656e 616d 6527 290a 2020 2020 2020 2020  ename').        
+000e5310: 6966 206d 2e67 6574 2827 6d61 7070 696e  if m.get('mappin
+000e5320: 675f 6261 6d5f 6f75 745f 7061 7468 2729  g_bam_out_path')
+000e5330: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e5340: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000e5350: 6170 7069 6e67 5f62 616d 5f6f 7574 5f70  apping_bam_out_p
+000e5360: 6174 6820 3d20 6d2e 6765 7428 276d 6170  ath = m.get('map
+000e5370: 7069 6e67 5f62 616d 5f6f 7574 5f70 6174  ping_bam_out_pat
+000e5380: 6827 290a 2020 2020 2020 2020 6966 206d  h').        if m
+000e5390: 2e67 6574 2827 6d61 7070 696e 675f 6275  .get('mapping_bu
+000e53a0: 636b 6574 5f6e 616d 6527 2920 6973 206e  cket_name') is n
+000e53b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e53c0: 2020 2020 2073 656c 662e 6d61 7070 696e       self.mappin
+000e53d0: 675f 6275 636b 6574 5f6e 616d 6520 3d20  g_bucket_name = 
+000e53e0: 6d2e 6765 7428 276d 6170 7069 6e67 5f62  m.get('mapping_b
+000e53f0: 7563 6b65 745f 6e61 6d65 2729 0a20 2020  ucket_name').   
+000e5400: 2020 2020 2069 6620 6d2e 6765 7428 276d       if m.get('m
+000e5410: 6170 7069 6e67 5f66 6173 7471 5f66 6972  apping_fastq_fir
+000e5420: 7374 5f66 696c 656e 616d 6527 2920 6973  st_filename') is
+000e5430: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e5440: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+000e5450: 696e 675f 6661 7374 715f 6669 7273 745f  ing_fastq_first_
+000e5460: 6669 6c65 6e61 6d65 203d 206d 2e67 6574  filename = m.get
+000e5470: 2827 6d61 7070 696e 675f 6661 7374 715f  ('mapping_fastq_
+000e5480: 6669 7273 745f 6669 6c65 6e61 6d65 2729  first_filename')
+000e5490: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000e54a0: 7428 276d 6170 7069 6e67 5f66 6173 7471  t('mapping_fastq
+000e54b0: 5f70 6174 6827 2920 6973 206e 6f74 204e  _path') is not N
+000e54c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e54d0: 2073 656c 662e 6d61 7070 696e 675f 6661   self.mapping_fa
+000e54e0: 7374 715f 7061 7468 203d 206d 2e67 6574  stq_path = m.get
+000e54f0: 2827 6d61 7070 696e 675f 6661 7374 715f  ('mapping_fastq_
+000e5500: 7061 7468 2729 0a20 2020 2020 2020 2069  path').        i
+000e5510: 6620 6d2e 6765 7428 276d 6170 7069 6e67  f m.get('mapping
+000e5520: 5f66 6173 7471 5f73 6563 6f6e 645f 6669  _fastq_second_fi
+000e5530: 6c65 6e61 6d65 2729 2069 7320 6e6f 7420  lename') is not 
+000e5540: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e5550: 2020 7365 6c66 2e6d 6170 7069 6e67 5f66    self.mapping_f
+000e5560: 6173 7471 5f73 6563 6f6e 645f 6669 6c65  astq_second_file
+000e5570: 6e61 6d65 203d 206d 2e67 6574 2827 6d61  name = m.get('ma
+000e5580: 7070 696e 675f 6661 7374 715f 7365 636f  pping_fastq_seco
+000e5590: 6e64 5f66 696c 656e 616d 6527 290a 2020  nd_filename').  
+000e55a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000e55b0: 6d61 7070 696e 675f 6973 5f6d 6172 6b5f  mapping_is_mark_
+000e55c0: 6475 7027 2920 6973 206e 6f74 204e 6f6e  dup') is not Non
+000e55d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000e55e0: 656c 662e 6d61 7070 696e 675f 6973 5f6d  elf.mapping_is_m
+000e55f0: 6172 6b5f 6475 7020 3d20 6d2e 6765 7428  ark_dup = m.get(
+000e5600: 276d 6170 7069 6e67 5f69 735f 6d61 726b  'mapping_is_mark
+000e5610: 5f64 7570 2729 0a20 2020 2020 2020 2069  _dup').        i
+000e5620: 6620 6d2e 6765 7428 276d 6170 7069 6e67  f m.get('mapping
+000e5630: 5f6f 7373 5f72 6567 696f 6e27 2920 6973  _oss_region') is
+000e5640: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e5650: 2020 2020 2020 2073 656c 662e 6d61 7070         self.mapp
+000e5660: 696e 675f 6f73 735f 7265 6769 6f6e 203d  ing_oss_region =
+000e5670: 206d 2e67 6574 2827 6d61 7070 696e 675f   m.get('mapping_
+000e5680: 6f73 735f 7265 6769 6f6e 2729 0a20 2020  oss_region').   
+000e5690: 2020 2020 2069 6620 6d2e 6765 7428 276d       if m.get('m
+000e56a0: 6170 7069 6e67 5f72 6566 6572 656e 6365  apping_reference
+000e56b0: 5f70 6174 6827 2920 6973 206e 6f74 204e  _path') is not N
+000e56c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e56d0: 2073 656c 662e 6d61 7070 696e 675f 7265   self.mapping_re
+000e56e0: 6665 7265 6e63 655f 7061 7468 203d 206d  ference_path = m
+000e56f0: 2e67 6574 2827 6d61 7070 696e 675f 7265  .get('mapping_re
+000e5700: 6665 7265 6e63 655f 7061 7468 2729 0a20  ference_path'). 
+000e5710: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000e5720: 2773 6572 7669 6365 2729 2069 7320 6e6f  'service') is no
+000e5730: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e5740: 2020 2020 7365 6c66 2e73 6572 7669 6365      self.service
+000e5750: 203d 206d 2e67 6574 2827 7365 7276 6963   = m.get('servic
+000e5760: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+000e5770: 2e67 6574 2827 7767 735f 6275 636b 6574  .get('wgs_bucket
+000e5780: 5f6e 616d 6527 2920 6973 206e 6f74 204e  _name') is not N
+000e5790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e57a0: 2073 656c 662e 7767 735f 6275 636b 6574   self.wgs_bucket
+000e57b0: 5f6e 616d 6520 3d20 6d2e 6765 7428 2777  _name = m.get('w
+000e57c0: 6773 5f62 7563 6b65 745f 6e61 6d65 2729  gs_bucket_name')
+000e57d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000e57e0: 7428 2777 6773 5f66 6173 7471 5f66 6972  t('wgs_fastq_fir
+000e57f0: 7374 5f66 696c 656e 616d 6527 2920 6973  st_filename') is
+000e5800: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e5810: 2020 2020 2020 2073 656c 662e 7767 735f         self.wgs_
+000e5820: 6661 7374 715f 6669 7273 745f 6669 6c65  fastq_first_file
+000e5830: 6e61 6d65 203d 206d 2e67 6574 2827 7767  name = m.get('wg
+000e5840: 735f 6661 7374 715f 6669 7273 745f 6669  s_fastq_first_fi
+000e5850: 6c65 6e61 6d65 2729 0a20 2020 2020 2020  lename').       
+000e5860: 2069 6620 6d2e 6765 7428 2777 6773 5f66   if m.get('wgs_f
+000e5870: 6173 7471 5f70 6174 6827 2920 6973 206e  astq_path') is n
+000e5880: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e5890: 2020 2020 2073 656c 662e 7767 735f 6661       self.wgs_fa
+000e58a0: 7374 715f 7061 7468 203d 206d 2e67 6574  stq_path = m.get
+000e58b0: 2827 7767 735f 6661 7374 715f 7061 7468  ('wgs_fastq_path
+000e58c0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000e58d0: 6765 7428 2777 6773 5f66 6173 7471 5f73  get('wgs_fastq_s
+000e58e0: 6563 6f6e 645f 6669 6c65 6e61 6d65 2729  econd_filename')
+000e58f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e5900: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+000e5910: 6773 5f66 6173 7471 5f73 6563 6f6e 645f  gs_fastq_second_
+000e5920: 6669 6c65 6e61 6d65 203d 206d 2e67 6574  filename = m.get
+000e5930: 2827 7767 735f 6661 7374 715f 7365 636f  ('wgs_fastq_seco
+000e5940: 6e64 5f66 696c 656e 616d 6527 290a 2020  nd_filename').  
+000e5950: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000e5960: 7767 735f 6f73 735f 7265 6769 6f6e 2729  wgs_oss_region')
+000e5970: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e5980: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+000e5990: 6773 5f6f 7373 5f72 6567 696f 6e20 3d20  gs_oss_region = 
+000e59a0: 6d2e 6765 7428 2777 6773 5f6f 7373 5f72  m.get('wgs_oss_r
+000e59b0: 6567 696f 6e27 290a 2020 2020 2020 2020  egion').        
+000e59c0: 6966 206d 2e67 6574 2827 7767 735f 7265  if m.get('wgs_re
+000e59d0: 6665 7265 6e63 655f 7061 7468 2729 2069  ference_path') i
+000e59e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e59f0: 2020 2020 2020 2020 7365 6c66 2e77 6773          self.wgs
+000e5a00: 5f72 6566 6572 656e 6365 5f70 6174 6820  _reference_path 
+000e5a10: 3d20 6d2e 6765 7428 2777 6773 5f72 6566  = m.get('wgs_ref
+000e5a20: 6572 656e 6365 5f70 6174 6827 290a 2020  erence_path').  
+000e5a30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000e5a40: 7767 735f 7663 665f 6f75 745f 6669 6c65  wgs_vcf_out_file
+000e5a50: 6e61 6d65 2729 2069 7320 6e6f 7420 4e6f  name') is not No
+000e5a60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e5a70: 7365 6c66 2e77 6773 5f76 6366 5f6f 7574  self.wgs_vcf_out
+000e5a80: 5f66 696c 656e 616d 6520 3d20 6d2e 6765  _filename = m.ge
+000e5a90: 7428 2777 6773 5f76 6366 5f6f 7574 5f66  t('wgs_vcf_out_f
+000e5aa0: 696c 656e 616d 6527 290a 2020 2020 2020  ilename').      
+000e5ab0: 2020 6966 206d 2e67 6574 2827 7767 735f    if m.get('wgs_
+000e5ac0: 7663 665f 6f75 745f 7061 7468 2729 2069  vcf_out_path') i
+000e5ad0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e5ae0: 2020 2020 2020 2020 7365 6c66 2e77 6773          self.wgs
+000e5af0: 5f76 6366 5f6f 7574 5f70 6174 6820 3d20  _vcf_out_path = 
+000e5b00: 6d2e 6765 7428 2777 6773 5f76 6366 5f6f  m.get('wgs_vcf_o
+000e5b10: 7574 5f70 6174 6827 290a 2020 2020 2020  ut_path').      
+000e5b20: 2020 6966 206d 2e67 6574 2827 776f 726b    if m.get('work
+000e5b30: 666c 6f77 5f74 7970 6527 2920 6973 206e  flow_type') is n
+000e5b40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e5b50: 2020 2020 2073 656c 662e 776f 726b 666c       self.workfl
+000e5b60: 6f77 5f74 7970 6520 3d20 6d2e 6765 7428  ow_type = m.get(
+000e5b70: 2777 6f72 6b66 6c6f 775f 7479 7065 2729  'workflow_type')
+000e5b80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000e5b90: 7365 6c66 0a0a 0a63 6c61 7373 2053 7461  self...class Sta
+000e5ba0: 7274 576f 726b 666c 6f77 5265 7370 6f6e  rtWorkflowRespon
+000e5bb0: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
+000e5bc0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000e5bd0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+000e5be0: 2c0a 2020 2020 2020 2020 6a6f 625f 6e61  ,.        job_na
+000e5bf0: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
+000e5c00: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
+000e5c10: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+000e5c20: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
+000e5c30: 2020 2073 656c 662e 6a6f 625f 6e61 6d65     self.job_name
+000e5c40: 203d 206a 6f62 5f6e 616d 650a 0a20 2020   = job_name..   
+000e5c50: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000e5c60: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000e5c70: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+000e5c80: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000e5c90: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+000e5ca0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000e5cb0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+000e5cc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e5cd0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+000e5ce0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000e5cf0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000e5d00: 6620 7365 6c66 2e6a 6f62 5f6e 616d 6520  f self.job_name 
+000e5d10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e5d20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000e5d30: 274a 6f62 4e61 6d65 275d 203d 2073 656c  'JobName'] = sel
+000e5d40: 662e 6a6f 625f 6e61 6d65 0a20 2020 2020  f.job_name.     
+000e5d50: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+000e5d60: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000e5d70: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+000e5d80: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+000e5d90: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000e5da0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000e5db0: 6574 2827 4a6f 624e 616d 6527 2920 6973  et('JobName') is
+000e5dc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e5dd0: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+000e5de0: 6e61 6d65 203d 206d 2e67 6574 2827 4a6f  name = m.get('Jo
+000e5df0: 624e 616d 6527 290a 2020 2020 2020 2020  bName').        
+000e5e00: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000e5e10: 6173 7320 5374 6172 7457 6f72 6b66 6c6f  ass StartWorkflo
+000e5e20: 7752 6573 706f 6e73 6528 5465 614d 6f64  wResponse(TeaMod
+000e5e30: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000e5e40: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000e5e50: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+000e5e60: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+000e5e70: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000e5e80: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+000e5e90: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+000e5ea0: 2020 2020 2020 626f 6479 3a20 5374 6172        body: Star
+000e5eb0: 7457 6f72 6b66 6c6f 7752 6573 706f 6e73  tWorkflowRespons
+000e5ec0: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+000e5ed0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+000e5ee0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+000e5ef0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+000e5f00: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000e5f10: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000e5f20: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+000e5f30: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+000e5f40: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000e5f50: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+000e5f60: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+000e5f70: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+000e5f80: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+000e5f90: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+000e5fa0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000e5fb0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+000e5fc0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+000e5fd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e5fe0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000e5ff0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000e6000: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000e6010: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+000e6020: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e6030: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000e6040: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+000e6050: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+000e6060: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+000e6070: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+000e6080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e6090: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+000e60a0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+000e60b0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+000e60c0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+000e60d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e60e0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+000e60f0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+000e6100: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000e6110: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000e6120: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000e6130: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000e6140: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+000e6150: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+000e6160: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000e6170: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+000e6180: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000e6190: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+000e61a0: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+000e61b0: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+000e61c0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000e61d0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+000e61e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000e61f0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000e6200: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000e6210: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+000e6220: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+000e6230: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e6240: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000e6250: 6c20 3d20 5374 6172 7457 6f72 6b66 6c6f  l = StartWorkflo
+000e6260: 7752 6573 706f 6e73 6542 6f64 7928 290a  wResponseBody().
+000e6270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000e6280: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+000e6290: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+000e62a0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+000e62b0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000e62c0: 7373 2053 746f 7041 6c65 7274 5265 7175  ss StopAlertRequ
+000e62d0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+000e62e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000e62f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000e6300: 2020 2020 2020 2061 6c65 7274 5f72 756c         alert_rul
+000e6310: 655f 6772 6f75 705f 6e61 6d65 3a20 7374  e_group_name: st
+000e6320: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000e6330: 2020 616c 6572 745f 7275 6c65 5f6e 616d    alert_rule_nam
+000e6340: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+000e6350: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
+000e6360: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
+000e6370: 616c 6572 7420 7275 6c65 2073 6574 2074  alert rule set t
+000e6380: 6f20 6265 2064 6973 6162 6c65 642e 0a20  o be disabled.. 
+000e6390: 2020 2020 2020 2073 656c 662e 616c 6572         self.aler
+000e63a0: 745f 7275 6c65 5f67 726f 7570 5f6e 616d  t_rule_group_nam
+000e63b0: 6520 3d20 616c 6572 745f 7275 6c65 5f67  e = alert_rule_g
+000e63c0: 726f 7570 5f6e 616d 650a 2020 2020 2020  roup_name.      
+000e63d0: 2020 2320 5468 6520 6e61 6d65 206f 6620    # The name of 
+000e63e0: 7468 6520 616c 6572 7420 7275 6c65 2074  the alert rule t
+000e63f0: 6f20 6265 2064 6973 6162 6c65 642e 2049  o be disabled. I
+000e6400: 6620 796f 7520 646f 206e 6f74 2073 7065  f you do not spe
+000e6410: 6369 6679 2061 6e20 616c 6572 7420 7275  cify an alert ru
+000e6420: 6c65 206e 616d 652c 2074 6865 2061 6c65  le name, the ale
+000e6430: 7274 2072 756c 6520 7365 7420 6973 2064  rt rule set is d
+000e6440: 6973 6162 6c65 642e 0a20 2020 2020 2020  isabled..       
+000e6450: 2073 656c 662e 616c 6572 745f 7275 6c65   self.alert_rule
+000e6460: 5f6e 616d 6520 3d20 616c 6572 745f 7275  _name = alert_ru
+000e6470: 6c65 5f6e 616d 650a 0a20 2020 2064 6566  le_name..    def
+000e6480: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+000e6490: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000e64a0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000e64b0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000e64c0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+000e64d0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+000e64e0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+000e64f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000e6500: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+000e6510: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+000e6520: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+000e6530: 6c66 2e61 6c65 7274 5f72 756c 655f 6772  lf.alert_rule_gr
+000e6540: 6f75 705f 6e61 6d65 2069 7320 6e6f 7420  oup_name is not 
+000e6550: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e6560: 2020 7265 7375 6c74 5b27 616c 6572 745f    result['alert_
+000e6570: 7275 6c65 5f67 726f 7570 5f6e 616d 6527  rule_group_name'
+000e6580: 5d20 3d20 7365 6c66 2e61 6c65 7274 5f72  ] = self.alert_r
+000e6590: 756c 655f 6772 6f75 705f 6e61 6d65 0a20  ule_group_name. 
+000e65a0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+000e65b0: 6c65 7274 5f72 756c 655f 6e61 6d65 2069  lert_rule_name i
+000e65c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e65d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e65e0: 616c 6572 745f 7275 6c65 5f6e 616d 6527  alert_rule_name'
+000e65f0: 5d20 3d20 7365 6c66 2e61 6c65 7274 5f72  ] = self.alert_r
+000e6600: 756c 655f 6e61 6d65 0a20 2020 2020 2020  ule_name.       
+000e6610: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000e6620: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000e6630: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+000e6640: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+000e6650: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+000e6660: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000e6670: 2827 616c 6572 745f 7275 6c65 5f67 726f  ('alert_rule_gro
+000e6680: 7570 5f6e 616d 6527 2920 6973 206e 6f74  up_name') is not
+000e6690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e66a0: 2020 2073 656c 662e 616c 6572 745f 7275     self.alert_ru
+000e66b0: 6c65 5f67 726f 7570 5f6e 616d 6520 3d20  le_group_name = 
+000e66c0: 6d2e 6765 7428 2761 6c65 7274 5f72 756c  m.get('alert_rul
+000e66d0: 655f 6772 6f75 705f 6e61 6d65 2729 0a20  e_group_name'). 
+000e66e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000e66f0: 2761 6c65 7274 5f72 756c 655f 6e61 6d65  'alert_rule_name
+000e6700: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000e6710: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000e6720: 2e61 6c65 7274 5f72 756c 655f 6e61 6d65  .alert_rule_name
+000e6730: 203d 206d 2e67 6574 2827 616c 6572 745f   = m.get('alert_
+000e6740: 7275 6c65 5f6e 616d 6527 290a 2020 2020  rule_name').    
+000e6750: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000e6760: 0a0a 636c 6173 7320 5374 6f70 416c 6572  ..class StopAler
+000e6770: 7452 6573 706f 6e73 6542 6f64 7928 5465  tResponseBody(Te
+000e6780: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+000e6790: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000e67a0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000e67b0: 206d 7367 3a20 7374 7220 3d20 4e6f 6e65   msg: str = None
+000e67c0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+000e67d0: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+000e67e0: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
+000e67f0: 5468 6520 6572 726f 7220 6d65 7373 6167  The error messag
+000e6800: 6520 7265 7475 726e 6564 2069 6620 7468  e returned if th
+000e6810: 6520 6361 6c6c 2066 6169 6c73 2e0a 2020  e call fails..  
+000e6820: 2020 2020 2020 7365 6c66 2e6d 7367 203d        self.msg =
+000e6830: 206d 7367 0a20 2020 2020 2020 2023 2054   msg.        # T
+000e6840: 6865 206f 7065 7261 7469 6f6e 2072 6573  he operation res
+000e6850: 756c 742e 2056 616c 6964 2076 616c 7565  ult. Valid value
+000e6860: 733a 0a20 2020 2020 2020 2023 200a 2020  s:.        # .  
+000e6870: 2020 2020 2020 2320 2a20 2020 5472 7565        # *   True
+000e6880: 3a20 5468 6520 6f70 6572 6174 696f 6e20  : The operation 
+000e6890: 6973 2073 7563 6365 7373 6675 6c2e 0a20  is successful.. 
+000e68a0: 2020 2020 2020 2023 202a 2020 2046 616c         # *   Fal
+000e68b0: 7365 3a20 5468 6520 6f70 6572 6174 696f  se: The operatio
+000e68c0: 6e20 6661 696c 6564 2e0a 2020 2020 2020  n failed..      
+000e68d0: 2020 7365 6c66 2e73 7461 7475 7320 3d20    self.status = 
+000e68e0: 7374 6174 7573 0a0a 2020 2020 6465 6620  status..    def 
+000e68f0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000e6900: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000e6910: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000e6920: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000e6930: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000e6940: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000e6950: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000e6960: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000e6970: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000e6980: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000e6990: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000e69a0: 662e 6d73 6720 6973 206e 6f74 204e 6f6e  f.msg is not Non
+000e69b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e69c0: 6573 756c 745b 276d 7367 275d 203d 2073  esult['msg'] = s
+000e69d0: 656c 662e 6d73 670a 2020 2020 2020 2020  elf.msg.        
+000e69e0: 6966 2073 656c 662e 7374 6174 7573 2069  if self.status i
+000e69f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e6a00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e6a10: 7374 6174 7573 275d 203d 2073 656c 662e  status'] = self.
+000e6a20: 7374 6174 7573 0a20 2020 2020 2020 2072  status.        r
+000e6a30: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+000e6a40: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+000e6a50: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+000e6a60: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+000e6a70: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+000e6a80: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000e6a90: 6d73 6727 2920 6973 206e 6f74 204e 6f6e  msg') is not Non
+000e6aa0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000e6ab0: 656c 662e 6d73 6720 3d20 6d2e 6765 7428  elf.msg = m.get(
+000e6ac0: 276d 7367 2729 0a20 2020 2020 2020 2069  'msg').        i
+000e6ad0: 6620 6d2e 6765 7428 2773 7461 7475 7327  f m.get('status'
+000e6ae0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000e6af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000e6b00: 7374 6174 7573 203d 206d 2e67 6574 2827  status = m.get('
+000e6b10: 7374 6174 7573 2729 0a20 2020 2020 2020  status').       
+000e6b20: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+000e6b30: 6c61 7373 2053 746f 7041 6c65 7274 5265  lass StopAlertRe
+000e6b40: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+000e6b50: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000e6b60: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+000e6b70: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+000e6b80: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+000e6b90: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+000e6ba0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+000e6bb0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+000e6bc0: 2020 2062 6f64 793a 2053 746f 7041 6c65     body: StopAle
+000e6bd0: 7274 5265 7370 6f6e 7365 426f 6479 203d  rtResponseBody =
+000e6be0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000e6bf0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+000e6c00: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+000e6c10: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000e6c20: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+000e6c30: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+000e6c40: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
+000e6c50: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000e6c60: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+000e6c70: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+000e6c80: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000e6c90: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+000e6ca0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000e6cb0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000e6cc0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000e6cd0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000e6ce0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000e6cf0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000e6d00: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000e6d10: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000e6d20: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000e6d30: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+000e6d40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e6d50: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+000e6d60: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+000e6d70: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+000e6d80: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+000e6d90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e6da0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000e6db0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+000e6dc0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000e6dd0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000e6de0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+000e6df0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e6e00: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+000e6e10: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+000e6e20: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+000e6e30: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000e6e40: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000e6e50: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+000e6e60: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000e6e70: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+000e6e80: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+000e6e90: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+000e6ea0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000e6eb0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000e6ec0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000e6ed0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000e6ee0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
 000e6ef0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e6f00: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
-000e6f10: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
-000e6f20: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
-000e6f30: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000e6f40: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
-000e6f50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000e6f60: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
-000e6f70: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
-000e6f80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000e6f90: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-000e6fa0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-000e6fb0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-000e6fc0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000e6fd0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000e6fe0: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-000e6ff0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-000e7000: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000e7010: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-000e7020: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-000e7030: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-000e7040: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-000e7050: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e7060: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000e7070: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-000e7080: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-000e7090: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-000e70a0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-000e70b0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-000e70c0: 6d70 5f6d 6f64 656c 203d 2053 796e 6343  mp_model = SyncC
-000e70d0: 6c75 7374 6572 4e6f 6465 506f 6f6c 5265  lusterNodePoolRe
-000e70e0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
-000e70f0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-000e7100: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-000e7110: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-000e7120: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-000e7130: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000e7140: 5461 6752 6573 6f75 7263 6573 5265 7175  TagResourcesRequ
-000e7150: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-000e7160: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000e7170: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000e7180: 2020 2020 2020 2072 6567 696f 6e5f 6964         region_id
-000e7190: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000e71a0: 2020 2020 2020 7265 736f 7572 6365 5f69        resource_i
-000e71b0: 6473 3a20 4c69 7374 5b73 7472 5d20 3d20  ds: List[str] = 
-000e71c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
-000e71d0: 736f 7572 6365 5f74 7970 653a 2073 7472  source_type: str
-000e71e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000e71f0: 2074 6167 733a 204c 6973 745b 5461 675d   tags: List[Tag]
-000e7200: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000e7210: 2020 2020 2020 2020 2320 5468 6520 7265          # The re
-000e7220: 6769 6f6e 2049 4420 6f66 2074 6865 2072  gion ID of the r
-000e7230: 6573 6f75 7263 652e 0a20 2020 2020 2020  esource..       
-000e7240: 2023 200a 2020 2020 2020 2020 2320 5468   # .        # Th
-000e7250: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
-000e7260: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
-000e7270: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
-000e7280: 203d 2072 6567 696f 6e5f 6964 0a20 2020   = region_id.   
-000e7290: 2020 2020 2023 2054 6865 206c 6973 7420       # The list 
-000e72a0: 6f66 2072 6573 6f75 7263 6520 4944 732e  of resource IDs.
-000e72b0: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
-000e72c0: 2020 2020 2320 5468 6973 2070 6172 616d      # This param
-000e72d0: 6574 6572 2069 7320 7265 7175 6972 6564  eter is required
-000e72e0: 2e0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-000e72f0: 6573 6f75 7263 655f 6964 7320 3d20 7265  esource_ids = re
-000e7300: 736f 7572 6365 5f69 6473 0a20 2020 2020  source_ids.     
-000e7310: 2020 2023 2054 6865 2074 7970 6520 6f66     # The type of
-000e7320: 2072 6573 6f75 7263 6520 7468 6174 2079   resource that y
-000e7330: 6f75 2077 616e 7420 746f 206c 6162 656c  ou want to label
-000e7340: 2e20 5365 7420 7468 6520 7661 6c75 6520  . Set the value 
-000e7350: 746f 2060 434c 5553 5445 5260 2e0a 2020  to `CLUSTER`..  
-000e7360: 2020 2020 2020 2320 0a20 2020 2020 2020        # .       
-000e7370: 2023 2054 6869 7320 7061 7261 6d65 7465   # This paramete
-000e7380: 7220 6973 2072 6571 7569 7265 642e 0a20  r is required.. 
-000e7390: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-000e73a0: 7572 6365 5f74 7970 6520 3d20 7265 736f  urce_type = reso
-000e73b0: 7572 6365 5f74 7970 650a 2020 2020 2020  urce_type.      
-000e73c0: 2020 2320 5468 6520 6c61 6265 6c73 2074    # The labels t
-000e73d0: 6861 7420 796f 7520 7761 6e74 2074 6f20  hat you want to 
-000e73e0: 6164 6420 746f 2074 6865 2072 6573 6f75  add to the resou
-000e73f0: 7263 6573 2069 6e20 6b65 792d 7661 6c75  rces in key-valu
-000e7400: 6520 7061 6972 732e 2059 6f75 2063 616e  e pairs. You can
-000e7410: 2061 6464 2075 7020 746f 2032 3020 6c61   add up to 20 la
-000e7420: 6265 6c73 2e20 5573 6167 6520 6e6f 7465  bels. Usage note
-000e7430: 733a 0a20 2020 2020 2020 2023 200a 2020  s:.        # .  
-000e7440: 2020 2020 2020 2320 2a20 2020 4c61 6265        # *   Labe
-000e7450: 6c20 7661 6c75 6573 206d 7573 7420 6e6f  l values must no
-000e7460: 7420 6265 2065 6d70 7479 2073 7472 696e  t be empty strin
-000e7470: 6773 2e20 4120 6c61 6265 6c20 7661 6c75  gs. A label valu
-000e7480: 6520 6d75 7374 2062 6520 3120 746f 2031  e must be 1 to 1
-000e7490: 3238 2063 6861 7261 6374 6572 7320 696e  28 characters in
-000e74a0: 206c 656e 6774 682e 0a20 2020 2020 2020   length..       
-000e74b0: 2023 202a 2020 2054 6865 206c 6162 656c   # *   The label
-000e74c0: 2076 616c 7565 206d 7573 7420 6e6f 7420   value must not 
-000e74d0: 7374 6172 7420 7769 7468 2060 616c 6979  start with `aliy
-000e74e0: 756e 6020 6f72 2060 6163 733a 602e 0a20  un` or `acs:`.. 
-000e74f0: 2020 2020 2020 2023 202a 2020 2054 6865         # *   The
-000e7500: 206c 6162 656c 2076 616c 7565 206d 7573   label value mus
-000e7510: 7420 6e6f 7420 636f 6e74 6169 6e20 6068  t not contain `h
-000e7520: 7474 703a 2f2f 6020 6f72 2060 6874 7470  ttp://` or `http
-000e7530: 733a 2f2f 602e 0a20 2020 2020 2020 2023  s://`..        #
-000e7540: 200a 2020 2020 2020 2020 2320 5468 6973   .        # This
-000e7550: 2070 6172 616d 6574 6572 2069 7320 7265   parameter is re
-000e7560: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-000e7570: 7365 6c66 2e74 6167 7320 3d20 7461 6773  self.tags = tags
-000e7580: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000e7590: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000e75a0: 2020 6966 2073 656c 662e 7461 6773 3a0a    if self.tags:.
-000e75b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000e75c0: 6b20 696e 2073 656c 662e 7461 6773 3a0a  k in self.tags:.
-000e75d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000e75e0: 6966 206b 3a0a 2020 2020 2020 2020 2020  if k:.          
-000e75f0: 2020 2020 2020 2020 2020 6b2e 7661 6c69            k.vali
-000e7600: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-000e7610: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-000e7620: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000e7630: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-000e7640: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-000e7650: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e7660: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000e7670: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000e7680: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000e7690: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
-000e76a0: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
-000e76b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e76c0: 6573 756c 745b 2772 6567 696f 6e5f 6964  esult['region_id
-000e76d0: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
-000e76e0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-000e76f0: 656c 662e 7265 736f 7572 6365 5f69 6473  elf.resource_ids
-000e7700: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e7710: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e7720: 5b27 7265 736f 7572 6365 5f69 6473 275d  ['resource_ids']
-000e7730: 203d 2073 656c 662e 7265 736f 7572 6365   = self.resource
-000e7740: 5f69 6473 0a20 2020 2020 2020 2069 6620  _ids.        if 
-000e7750: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
-000e7760: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-000e7770: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000e7780: 6c74 5b27 7265 736f 7572 6365 5f74 7970  lt['resource_typ
-000e7790: 6527 5d20 3d20 7365 6c66 2e72 6573 6f75  e'] = self.resou
-000e77a0: 7263 655f 7479 7065 0a20 2020 2020 2020  rce_type.       
-000e77b0: 2072 6573 756c 745b 2774 6167 7327 5d20   result['tags'] 
-000e77c0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-000e77d0: 7365 6c66 2e74 6167 7320 6973 206e 6f74  self.tags is not
-000e77e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e77f0: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
-000e7800: 2e74 6167 733a 0a20 2020 2020 2020 2020  .tags:.         
-000e7810: 2020 2020 2020 2072 6573 756c 745b 2774         result['t
-000e7820: 6167 7327 5d2e 6170 7065 6e64 286b 2e74  ags'].append(k.t
-000e7830: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
-000e7840: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
-000e7850: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000e7860: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000e7870: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-000e7880: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-000e7890: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000e78a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000e78b0: 2772 6567 696f 6e5f 6964 2729 2069 7320  'region_id') is 
-000e78c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e78d0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-000e78e0: 6e5f 6964 203d 206d 2e67 6574 2827 7265  n_id = m.get('re
-000e78f0: 6769 6f6e 5f69 6427 290a 2020 2020 2020  gion_id').      
-000e7900: 2020 6966 206d 2e67 6574 2827 7265 736f    if m.get('reso
-000e7910: 7572 6365 5f69 6473 2729 2069 7320 6e6f  urce_ids') is no
-000e7920: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e7930: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-000e7940: 655f 6964 7320 3d20 6d2e 6765 7428 2772  e_ids = m.get('r
-000e7950: 6573 6f75 7263 655f 6964 7327 290a 2020  esource_ids').  
-000e7960: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e7970: 7265 736f 7572 6365 5f74 7970 6527 2920  resource_type') 
-000e7980: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e7990: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000e79a0: 736f 7572 6365 5f74 7970 6520 3d20 6d2e  source_type = m.
-000e79b0: 6765 7428 2772 6573 6f75 7263 655f 7479  get('resource_ty
-000e79c0: 7065 2729 0a20 2020 2020 2020 2073 656c  pe').        sel
-000e79d0: 662e 7461 6773 203d 205b 5d0a 2020 2020  f.tags = [].    
-000e79e0: 2020 2020 6966 206d 2e67 6574 2827 7461      if m.get('ta
-000e79f0: 6773 2729 2069 7320 6e6f 7420 4e6f 6e65  gs') is not None
-000e7a00: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-000e7a10: 7220 6b20 696e 206d 2e67 6574 2827 7461  r k in m.get('ta
-000e7a20: 6773 2729 3a0a 2020 2020 2020 2020 2020  gs'):.          
-000e7a30: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-000e7a40: 203d 2054 6167 2829 0a20 2020 2020 2020   = Tag().       
-000e7a50: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-000e7a60: 6773 2e61 7070 656e 6428 7465 6d70 5f6d  gs.append(temp_m
-000e7a70: 6f64 656c 2e66 726f 6d5f 6d61 7028 6b29  odel.from_map(k)
-000e7a80: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000e7a90: 2073 656c 660a 0a0a 636c 6173 7320 5461   self...class Ta
-000e7aa0: 6752 6573 6f75 7263 6573 5265 7370 6f6e  gResourcesRespon
-000e7ab0: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-000e7ac0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000e7ad0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000e7ae0: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
-000e7af0: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
-000e7b00: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-000e7b10: 2023 2054 6865 2072 6571 7565 7374 2049   # The request I
-000e7b20: 442e 0a20 2020 2020 2020 2073 656c 662e  D..        self.
-000e7b30: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
-000e7b40: 7565 7374 5f69 640a 0a20 2020 2064 6566  uest_id..    def
-000e7b50: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000e7b60: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000e7b70: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-000e7b80: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-000e7b90: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-000e7ba0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-000e7bb0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-000e7bc0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e7bd0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-000e7be0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-000e7bf0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-000e7c00: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-000e7c10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e7c20: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-000e7c30: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-000e7c40: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-000e7c50: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000e7c60: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-000e7c70: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-000e7c80: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-000e7c90: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-000e7ca0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-000e7cb0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-000e7cc0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000e7cd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000e7ce0: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
-000e7cf0: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
-000e7d00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000e7d10: 656c 660a 0a0a 636c 6173 7320 5461 6752  elf...class TagR
-000e7d20: 6573 6f75 7263 6573 5265 7370 6f6e 7365  esourcesResponse
-000e7d30: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-000e7d40: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-000e7d50: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000e7d60: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
-000e7d70: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
-000e7d80: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-000e7d90: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
-000e7da0: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
-000e7db0: 793a 2054 6167 5265 736f 7572 6365 7352  y: TagResourcesR
-000e7dc0: 6573 706f 6e73 6542 6f64 7920 3d20 4e6f  esponseBody = No
-000e7dd0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-000e7de0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-000e7df0: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-000e7e00: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-000e7e10: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-000e7e20: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-000e7e30: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-000e7e40: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000e7e50: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-000e7e60: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
-000e7e70: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
-000e7e80: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-000e7e90: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000e7ea0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-000e7eb0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-000e7ec0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-000e7ed0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e7ee0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000e7ef0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-000e7f00: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-000e7f10: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-000e7f20: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-000e7f30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e7f40: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-000e7f50: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-000e7f60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e7f70: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-000e7f80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e7f90: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-000e7fa0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-000e7fb0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-000e7fc0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-000e7fd0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-000e7fe0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000e7ff0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-000e8000: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-000e8010: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000e8020: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-000e8030: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-000e8040: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-000e8050: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-000e8060: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000e8070: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-000e8080: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000e8090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e80a0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-000e80b0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-000e80c0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-000e80d0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-000e80e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e80f0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-000e8100: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-000e8110: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-000e8120: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
-000e8130: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-000e8140: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-000e8150: 705f 6d6f 6465 6c20 3d20 5461 6752 6573  p_model = TagRes
-000e8160: 6f75 7263 6573 5265 7370 6f6e 7365 426f  ourcesResponseBo
-000e8170: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
-000e8180: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-000e8190: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-000e81a0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-000e81b0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-000e81c0: 0a0a 636c 6173 7320 556e 496e 7374 616c  ..class UnInstal
-000e81d0: 6c43 6c75 7374 6572 4164 646f 6e73 5265  lClusterAddonsRe
-000e81e0: 7175 6573 7441 6464 6f6e 7328 5465 614d  questAddons(TeaM
-000e81f0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000e8200: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000e8210: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
-000e8220: 6c65 616e 7570 5f63 6c6f 7564 5f72 6573  leanup_cloud_res
-000e8230: 6f75 7263 6573 3a20 626f 6f6c 203d 204e  ources: bool = N
-000e8240: 6f6e 652c 0a20 2020 2020 2020 206e 616d  one,.        nam
-000e8250: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-000e8260: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000e8270: 5768 6574 6865 7220 746f 2063 6c65 616e  Whether to clean
-000e8280: 2075 7020 636c 6f75 6420 7265 736f 7572   up cloud resour
-000e8290: 6365 732e 0a20 2020 2020 2020 2073 656c  ces..        sel
-000e82a0: 662e 636c 6561 6e75 705f 636c 6f75 645f  f.cleanup_cloud_
-000e82b0: 7265 736f 7572 6365 7320 3d20 636c 6561  resources = clea
-000e82c0: 6e75 705f 636c 6f75 645f 7265 736f 7572  nup_cloud_resour
-000e82d0: 6365 730a 2020 2020 2020 2020 2320 5468  ces.        # Th
-000e82e0: 6520 636f 6d70 6f6e 656e 7420 6e61 6d65  e component name
-000e82f0: 2e0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-000e8300: 616d 6520 3d20 6e61 6d65 0a0a 2020 2020  ame = name..    
-000e8310: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-000e8320: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-000e8330: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000e8340: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e8350: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000e8360: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000e8370: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000e8380: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e8390: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000e83a0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000e83b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000e83c0: 2073 656c 662e 636c 6561 6e75 705f 636c   self.cleanup_cl
-000e83d0: 6f75 645f 7265 736f 7572 6365 7320 6973  oud_resources is
-000e83e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e83f0: 2020 2020 2020 2072 6573 756c 745b 2763         result['c
-000e8400: 6c65 616e 7570 5f63 6c6f 7564 5f72 6573  leanup_cloud_res
-000e8410: 6f75 7263 6573 275d 203d 2073 656c 662e  ources'] = self.
-000e8420: 636c 6561 6e75 705f 636c 6f75 645f 7265  cleanup_cloud_re
-000e8430: 736f 7572 6365 730a 2020 2020 2020 2020  sources.        
-000e8440: 6966 2073 656c 662e 6e61 6d65 2069 7320  if self.name is 
-000e8450: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000e8460: 2020 2020 2020 7265 7375 6c74 5b27 6e61        result['na
-000e8470: 6d65 275d 203d 2073 656c 662e 6e61 6d65  me'] = self.name
-000e8480: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000e8490: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-000e84a0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-000e84b0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-000e84c0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000e84d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000e84e0: 6966 206d 2e67 6574 2827 636c 6561 6e75  if m.get('cleanu
-000e84f0: 705f 636c 6f75 645f 7265 736f 7572 6365  p_cloud_resource
-000e8500: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-000e8510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000e8520: 662e 636c 6561 6e75 705f 636c 6f75 645f  f.cleanup_cloud_
-000e8530: 7265 736f 7572 6365 7320 3d20 6d2e 6765  resources = m.ge
-000e8540: 7428 2763 6c65 616e 7570 5f63 6c6f 7564  t('cleanup_cloud
-000e8550: 5f72 6573 6f75 7263 6573 2729 0a20 2020  _resources').   
-000e8560: 2020 2020 2069 6620 6d2e 6765 7428 276e       if m.get('n
-000e8570: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-000e8580: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000e8590: 656c 662e 6e61 6d65 203d 206d 2e67 6574  elf.name = m.get
-000e85a0: 2827 6e61 6d65 2729 0a20 2020 2020 2020  ('name').       
-000e85b0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000e85c0: 6c61 7373 2055 6e49 6e73 7461 6c6c 436c  lass UnInstallCl
-000e85d0: 7573 7465 7241 6464 6f6e 7352 6571 7565  usterAddonsReque
-000e85e0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-000e85f0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000e8600: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000e8610: 2020 2020 2020 6164 646f 6e73 3a20 4c69        addons: Li
-000e8620: 7374 5b55 6e49 6e73 7461 6c6c 436c 7573  st[UnInstallClus
-000e8630: 7465 7241 6464 6f6e 7352 6571 7565 7374  terAddonsRequest
-000e8640: 4164 646f 6e73 5d20 3d20 4e6f 6e65 2c0a  Addons] = None,.
-000e8650: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
-000e8660: 2054 6865 206c 6973 7420 6f66 2063 6f6d   The list of com
-000e8670: 706f 6e65 6e74 7320 7468 6174 2079 6f75  ponents that you
-000e8680: 2077 616e 7420 746f 2075 6e69 6e73 7461   want to uninsta
-000e8690: 6c6c 2e20 5468 6520 6c69 7374 2069 7320  ll. The list is 
-000e86a0: 616e 2061 7272 6179 2e0a 2020 2020 2020  an array..      
-000e86b0: 2020 7365 6c66 2e61 6464 6f6e 7320 3d20    self.addons = 
-000e86c0: 6164 646f 6e73 0a0a 2020 2020 6465 6620  addons..    def 
-000e86d0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000e86e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000e86f0: 6164 646f 6e73 3a0a 2020 2020 2020 2020  addons:.        
-000e8700: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
-000e8710: 662e 6164 646f 6e73 3a0a 2020 2020 2020  f.addons:.      
-000e8720: 2020 2020 2020 2020 2020 6966 206b 3a0a            if k:.
-000e8730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000e8740: 2020 2020 6b2e 7661 6c69 6461 7465 2829      k.validate()
-000e8750: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000e8760: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e8770: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000e8780: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000e8790: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000e87a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e87b0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000e87c0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000e87d0: 6963 7428 290a 2020 2020 2020 2020 7265  ict().        re
-000e87e0: 7375 6c74 5b27 6164 646f 6e73 275d 203d  sult['addons'] =
-000e87f0: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
-000e8800: 656c 662e 6164 646f 6e73 2069 7320 6e6f  elf.addons is no
-000e8810: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000e8820: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
-000e8830: 662e 6164 646f 6e73 3a0a 2020 2020 2020  f.addons:.      
-000e8840: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000e8850: 5b27 6164 646f 6e73 275d 2e61 7070 656e  ['addons'].appen
-000e8860: 6428 6b2e 746f 5f6d 6170 2829 2069 6620  d(k.to_map() if 
-000e8870: 6b20 656c 7365 204e 6f6e 6529 0a20 2020  k else None).   
-000e8880: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000e8890: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-000e88a0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-000e88b0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-000e88c0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-000e88d0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-000e88e0: 2e61 6464 6f6e 7320 3d20 5b5d 0a20 2020  .addons = [].   
-000e88f0: 2020 2020 2069 6620 6d2e 6765 7428 2761       if m.get('a
-000e8900: 6464 6f6e 7327 2920 6973 206e 6f74 204e  ddons') is not N
-000e8910: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e8920: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
-000e8930: 2761 6464 6f6e 7327 293a 0a20 2020 2020  'addons'):.     
-000e8940: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-000e8950: 6d6f 6465 6c20 3d20 556e 496e 7374 616c  model = UnInstal
-000e8960: 6c43 6c75 7374 6572 4164 646f 6e73 5265  lClusterAddonsRe
-000e8970: 7175 6573 7441 6464 6f6e 7328 290a 2020  questAddons().  
-000e8980: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000e8990: 6c66 2e61 6464 6f6e 732e 6170 7065 6e64  lf.addons.append
-000e89a0: 2874 656d 705f 6d6f 6465 6c2e 6672 6f6d  (temp_model.from
-000e89b0: 5f6d 6170 286b 2929 0a20 2020 2020 2020  _map(k)).       
-000e89c0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000e89d0: 6c61 7373 2055 6e49 6e73 7461 6c6c 436c  lass UnInstallCl
-000e89e0: 7573 7465 7241 6464 6f6e 7352 6573 706f  usterAddonsRespo
-000e89f0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-000e8a00: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000e8a10: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000e8a20: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-000e8a30: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-000e8a40: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-000e8a50: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
-000e8a60: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-000e8a70: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-000e8a80: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-000e8a90: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-000e8aa0: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-000e8ab0: 636f 6465 0a0a 2020 2020 6465 6620 7661  code..    def va
-000e8ac0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000e8ad0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000e8ae0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000e8af0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000e8b00: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-000e8b10: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-000e8b20: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000e8b30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000e8b40: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-000e8b50: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000e8b60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000e8b70: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
-000e8b80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e8b90: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
-000e8ba0: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
-000e8bb0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-000e8bc0: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
-000e8bd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e8be0: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
-000e8bf0: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
-000e8c00: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
-000e8c10: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000e8c20: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000e8c30: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000e8c40: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000e8c50: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000e8c60: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000e8c70: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-000e8c80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000e8c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000e8ca0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-000e8cb0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-000e8cc0: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-000e8cd0: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-000e8ce0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e8cf0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-000e8d00: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-000e8d10: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-000e8d20: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000e8d30: 636c 6173 7320 556e 7461 6752 6573 6f75  class UntagResou
-000e8d40: 7263 6573 5265 7175 6573 7428 5465 614d  rcesRequest(TeaM
-000e8d50: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000e8d60: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000e8d70: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
-000e8d80: 6c6c 3a20 626f 6f6c 203d 204e 6f6e 652c  ll: bool = None,
-000e8d90: 0a20 2020 2020 2020 2072 6567 696f 6e5f  .        region_
-000e8da0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-000e8db0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-000e8dc0: 5f69 6473 3a20 4c69 7374 5b73 7472 5d20  _ids: List[str] 
-000e8dd0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000e8de0: 7265 736f 7572 6365 5f74 7970 653a 2073  resource_type: s
-000e8df0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000e8e00: 2020 2074 6167 5f6b 6579 733a 204c 6973     tag_keys: Lis
-000e8e10: 745b 7374 725d 203d 204e 6f6e 652c 0a20  t[str] = None,. 
-000e8e20: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000e8e30: 5370 6563 6966 6965 7320 7768 6574 6865  Specifies whethe
-000e8e40: 7220 746f 2072 656d 6f76 6520 616c 6c20  r to remove all 
-000e8e50: 6375 7374 6f6d 206c 6162 656c 732e 2054  custom labels. T
-000e8e60: 6869 7320 7061 7261 6d65 7465 7220 7461  his parameter ta
-000e8e70: 6b65 7320 6566 6665 6374 206f 6e6c 7920  kes effect only 
-000e8e80: 7768 656e 2060 7461 675f 6b65 7973 6020  when `tag_keys` 
-000e8e90: 6973 206c 6566 7420 656d 7074 792e 2056  is left empty. V
-000e8ea0: 616c 6964 2076 616c 7565 733a 0a20 2020  alid values:.   
-000e8eb0: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
-000e8ec0: 2320 2a20 2020 6074 7275 6560 3a20 5265  # *   `true`: Re
-000e8ed0: 6d6f 7665 2061 6c6c 2063 7573 746f 6d20  move all custom 
-000e8ee0: 6c61 6265 6c73 2e0a 2020 2020 2020 2020  labels..        
-000e8ef0: 2320 2a20 2020 6066 616c 7365 603a 2044  # *   `false`: D
-000e8f00: 6f20 6e6f 7420 7265 6d6f 7665 2061 6c6c  o not remove all
-000e8f10: 2063 7573 746f 6d20 6c61 6265 6c73 2e0a   custom labels..
-000e8f20: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000e8f30: 203d 2061 6c6c 0a20 2020 2020 2020 2023   = all.        #
-000e8f40: 2054 6865 2072 6567 696f 6e20 4944 206f   The region ID o
-000e8f50: 6620 7468 6520 7265 736f 7572 6365 732e  f the resources.
-000e8f60: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
-000e8f70: 2020 2020 2320 5468 6973 2070 6172 616d      # This param
-000e8f80: 6574 6572 2069 7320 7265 7175 6972 6564  eter is required
-000e8f90: 2e0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-000e8fa0: 6567 696f 6e5f 6964 203d 2072 6567 696f  egion_id = regio
-000e8fb0: 6e5f 6964 0a20 2020 2020 2020 2023 2054  n_id.        # T
-000e8fc0: 6865 206c 6973 7420 6f66 2072 6573 6f75  he list of resou
-000e8fd0: 7263 6520 4944 732e 0a20 2020 2020 2020  rce IDs..       
-000e8fe0: 2023 200a 2020 2020 2020 2020 2320 5468   # .        # Th
-000e8ff0: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
-000e9000: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
-000e9010: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
-000e9020: 6964 7320 3d20 7265 736f 7572 6365 5f69  ids = resource_i
-000e9030: 6473 0a20 2020 2020 2020 2023 2054 6865  ds.        # The
-000e9040: 2074 7970 6520 6f66 2072 6573 6f75 7263   type of resourc
-000e9050: 652e 2053 6574 2074 6865 2076 616c 7565  e. Set the value
-000e9060: 2074 6f20 6043 4c55 5354 4552 602e 0a20   to `CLUSTER`.. 
-000e9070: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
-000e9080: 2020 2320 5468 6973 2070 6172 616d 6574    # This paramet
-000e9090: 6572 2069 7320 7265 7175 6972 6564 2e0a  er is required..
-000e90a0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-000e90b0: 6f75 7263 655f 7479 7065 203d 2072 6573  ource_type = res
-000e90c0: 6f75 7263 655f 7479 7065 0a20 2020 2020  ource_type.     
-000e90d0: 2020 2023 2054 6865 206c 6973 7420 6f66     # The list of
-000e90e0: 206b 6579 7320 6f66 2074 6865 206c 6162   keys of the lab
-000e90f0: 656c 7320 7468 6174 2079 6f75 2077 616e  els that you wan
-000e9100: 7420 746f 2072 656d 6f76 652e 0a20 2020  t to remove..   
-000e9110: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
-000e9120: 2320 5468 6973 2070 6172 616d 6574 6572  # This parameter
-000e9130: 2069 7320 7265 7175 6972 6564 2e0a 2020   is required..  
-000e9140: 2020 2020 2020 7365 6c66 2e74 6167 5f6b        self.tag_k
-000e9150: 6579 7320 3d20 7461 675f 6b65 7973 0a0a  eys = tag_keys..
-000e9160: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000e9170: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000e9180: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-000e9190: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-000e91a0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-000e91b0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-000e91c0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-000e91d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000e91e0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-000e91f0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000e9200: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000e9210: 2020 6966 2073 656c 662e 616c 6c20 6973    if self.all is
-000e9220: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e9230: 2020 2020 2020 2072 6573 756c 745b 2761         result['a
-000e9240: 6c6c 275d 203d 2073 656c 662e 616c 6c0a  ll'] = self.all.
-000e9250: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000e9260: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
-000e9270: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000e9280: 2020 2072 6573 756c 745b 2772 6567 696f     result['regio
-000e9290: 6e5f 6964 275d 203d 2073 656c 662e 7265  n_id'] = self.re
-000e92a0: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
-000e92b0: 6966 2073 656c 662e 7265 736f 7572 6365  if self.resource
-000e92c0: 5f69 6473 2069 7320 6e6f 7420 4e6f 6e65  _ids is not None
-000e92d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e92e0: 7375 6c74 5b27 7265 736f 7572 6365 5f69  sult['resource_i
-000e92f0: 6473 275d 203d 2073 656c 662e 7265 736f  ds'] = self.reso
-000e9300: 7572 6365 5f69 6473 0a20 2020 2020 2020  urce_ids.       
-000e9310: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
-000e9320: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
-000e9330: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e9340: 7265 7375 6c74 5b27 7265 736f 7572 6365  result['resource
-000e9350: 5f74 7970 6527 5d20 3d20 7365 6c66 2e72  _type'] = self.r
-000e9360: 6573 6f75 7263 655f 7479 7065 0a20 2020  esource_type.   
-000e9370: 2020 2020 2069 6620 7365 6c66 2e74 6167       if self.tag
-000e9380: 5f6b 6579 7320 6973 206e 6f74 204e 6f6e  _keys is not Non
-000e9390: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e93a0: 6573 756c 745b 2774 6167 5f6b 6579 7327  esult['tag_keys'
-000e93b0: 5d20 3d20 7365 6c66 2e74 6167 5f6b 6579  ] = self.tag_key
-000e93c0: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-000e93d0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-000e93e0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-000e93f0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-000e9400: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000e9410: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000e9420: 2069 6620 6d2e 6765 7428 2761 6c6c 2729   if m.get('all')
-000e9430: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000e9440: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000e9450: 6c6c 203d 206d 2e67 6574 2827 616c 6c27  ll = m.get('all'
-000e9460: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000e9470: 6574 2827 7265 6769 6f6e 5f69 6427 2920  et('region_id') 
-000e9480: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e9490: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000e94a0: 6769 6f6e 5f69 6420 3d20 6d2e 6765 7428  gion_id = m.get(
-000e94b0: 2772 6567 696f 6e5f 6964 2729 0a20 2020  'region_id').   
-000e94c0: 2020 2020 2069 6620 6d2e 6765 7428 2772       if m.get('r
-000e94d0: 6573 6f75 7263 655f 6964 7327 2920 6973  esource_ids') is
-000e94e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000e94f0: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-000e9500: 7572 6365 5f69 6473 203d 206d 2e67 6574  urce_ids = m.get
-000e9510: 2827 7265 736f 7572 6365 5f69 6473 2729  ('resource_ids')
-000e9520: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000e9530: 7428 2772 6573 6f75 7263 655f 7479 7065  t('resource_type
-000e9540: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000e9550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000e9560: 2e72 6573 6f75 7263 655f 7479 7065 203d  .resource_type =
-000e9570: 206d 2e67 6574 2827 7265 736f 7572 6365   m.get('resource
-000e9580: 5f74 7970 6527 290a 2020 2020 2020 2020  _type').        
-000e9590: 6966 206d 2e67 6574 2827 7461 675f 6b65  if m.get('tag_ke
-000e95a0: 7973 2729 2069 7320 6e6f 7420 4e6f 6e65  ys') is not None
-000e95b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000e95c0: 6c66 2e74 6167 5f6b 6579 7320 3d20 6d2e  lf.tag_keys = m.
-000e95d0: 6765 7428 2774 6167 5f6b 6579 7327 290a  get('tag_keys').
-000e95e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000e95f0: 656c 660a 0a0a 636c 6173 7320 556e 7461  elf...class Unta
-000e9600: 6752 6573 6f75 7263 6573 5368 7269 6e6b  gResourcesShrink
-000e9610: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-000e9620: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-000e9630: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000e9640: 662c 0a20 2020 2020 2020 2061 6c6c 3a20  f,.        all: 
-000e9650: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
-000e9660: 2020 2020 2072 6567 696f 6e5f 6964 3a20       region_id: 
-000e9670: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000e9680: 2020 2020 7265 736f 7572 6365 5f69 6473      resource_ids
-000e9690: 5f73 6872 696e 6b3a 2073 7472 203d 204e  _shrink: str = N
-000e96a0: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
-000e96b0: 6f75 7263 655f 7479 7065 3a20 7374 7220  ource_type: str 
-000e96c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000e96d0: 7461 675f 6b65 7973 5f73 6872 696e 6b3a  tag_keys_shrink:
-000e96e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000e96f0: 2029 3a0a 2020 2020 2020 2020 2320 5370   ):.        # Sp
-000e9700: 6563 6966 6965 7320 7768 6574 6865 7220  ecifies whether 
-000e9710: 746f 2072 656d 6f76 6520 616c 6c20 6375  to remove all cu
-000e9720: 7374 6f6d 206c 6162 656c 732e 2054 6869  stom labels. Thi
-000e9730: 7320 7061 7261 6d65 7465 7220 7461 6b65  s parameter take
-000e9740: 7320 6566 6665 6374 206f 6e6c 7920 7768  s effect only wh
-000e9750: 656e 2060 7461 675f 6b65 7973 6020 6973  en `tag_keys` is
-000e9760: 206c 6566 7420 656d 7074 792e 2056 616c   left empty. Val
-000e9770: 6964 2076 616c 7565 733a 0a20 2020 2020  id values:.     
-000e9780: 2020 2023 200a 2020 2020 2020 2020 2320     # .        # 
-000e9790: 2a20 2020 6074 7275 6560 3a20 5265 6d6f  *   `true`: Remo
-000e97a0: 7665 2061 6c6c 2063 7573 746f 6d20 6c61  ve all custom la
-000e97b0: 6265 6c73 2e0a 2020 2020 2020 2020 2320  bels..        # 
-000e97c0: 2a20 2020 6066 616c 7365 603a 2044 6f20  *   `false`: Do 
-000e97d0: 6e6f 7420 7265 6d6f 7665 2061 6c6c 2063  not remove all c
-000e97e0: 7573 746f 6d20 6c61 6265 6c73 2e0a 2020  ustom labels..  
-000e97f0: 2020 2020 2020 7365 6c66 2e61 6c6c 203d        self.all =
-000e9800: 2061 6c6c 0a20 2020 2020 2020 2023 2054   all.        # T
-000e9810: 6865 2072 6567 696f 6e20 4944 206f 6620  he region ID of 
-000e9820: 7468 6520 7265 736f 7572 6365 732e 0a20  the resources.. 
-000e9830: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
-000e9840: 2020 2320 5468 6973 2070 6172 616d 6574    # This paramet
-000e9850: 6572 2069 7320 7265 7175 6972 6564 2e0a  er is required..
-000e9860: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
-000e9870: 696f 6e5f 6964 203d 2072 6567 696f 6e5f  ion_id = region_
-000e9880: 6964 0a20 2020 2020 2020 2023 2054 6865  id.        # The
-000e9890: 206c 6973 7420 6f66 2072 6573 6f75 7263   list of resourc
-000e98a0: 6520 4944 732e 0a20 2020 2020 2020 2023  e IDs..        #
-000e98b0: 200a 2020 2020 2020 2020 2320 5468 6973   .        # This
-000e98c0: 2070 6172 616d 6574 6572 2069 7320 7265   parameter is re
-000e98d0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-000e98e0: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
-000e98f0: 735f 7368 7269 6e6b 203d 2072 6573 6f75  s_shrink = resou
-000e9900: 7263 655f 6964 735f 7368 7269 6e6b 0a20  rce_ids_shrink. 
-000e9910: 2020 2020 2020 2023 2054 6865 2074 7970         # The typ
-000e9920: 6520 6f66 2072 6573 6f75 7263 652e 2053  e of resource. S
-000e9930: 6574 2074 6865 2076 616c 7565 2074 6f20  et the value to 
-000e9940: 6043 4c55 5354 4552 602e 0a20 2020 2020  `CLUSTER`..     
-000e9950: 2020 2023 200a 2020 2020 2020 2020 2320     # .        # 
-000e9960: 5468 6973 2070 6172 616d 6574 6572 2069  This parameter i
-000e9970: 7320 7265 7175 6972 6564 2e0a 2020 2020  s required..    
-000e9980: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-000e9990: 655f 7479 7065 203d 2072 6573 6f75 7263  e_type = resourc
-000e99a0: 655f 7479 7065 0a20 2020 2020 2020 2023  e_type.        #
-000e99b0: 2054 6865 206c 6973 7420 6f66 206b 6579   The list of key
-000e99c0: 7320 6f66 2074 6865 206c 6162 656c 7320  s of the labels 
-000e99d0: 7468 6174 2079 6f75 2077 616e 7420 746f  that you want to
-000e99e0: 2072 656d 6f76 652e 0a20 2020 2020 2020   remove..       
-000e99f0: 2023 200a 2020 2020 2020 2020 2320 5468   # .        # Th
-000e9a00: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
-000e9a10: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
-000e9a20: 2020 7365 6c66 2e74 6167 5f6b 6579 735f    self.tag_keys_
-000e9a30: 7368 7269 6e6b 203d 2074 6167 5f6b 6579  shrink = tag_key
-000e9a40: 735f 7368 7269 6e6b 0a0a 2020 2020 6465  s_shrink..    de
-000e9a50: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000e9a60: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-000e9a70: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000e9a80: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000e9a90: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000e9aa0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000e9ab0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000e9ac0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e9ad0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000e9ae0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000e9af0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000e9b00: 656c 662e 616c 6c20 6973 206e 6f74 204e  elf.all is not N
-000e9b10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000e9b20: 2072 6573 756c 745b 2761 6c6c 275d 203d   result['all'] =
-000e9b30: 2073 656c 662e 616c 6c0a 2020 2020 2020   self.all.      
-000e9b40: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
-000e9b50: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-000e9b60: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000e9b70: 756c 745b 2772 6567 696f 6e5f 6964 275d  ult['region_id']
-000e9b80: 203d 2073 656c 662e 7265 6769 6f6e 5f69   = self.region_i
-000e9b90: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-000e9ba0: 662e 7265 736f 7572 6365 5f69 6473 5f73  f.resource_ids_s
-000e9bb0: 6872 696e 6b20 6973 206e 6f74 204e 6f6e  hrink is not Non
-000e9bc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000e9bd0: 6573 756c 745b 2772 6573 6f75 7263 655f  esult['resource_
-000e9be0: 6964 7327 5d20 3d20 7365 6c66 2e72 6573  ids'] = self.res
-000e9bf0: 6f75 7263 655f 6964 735f 7368 7269 6e6b  ource_ids_shrink
-000e9c00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000e9c10: 2e72 6573 6f75 7263 655f 7479 7065 2069  .resource_type i
-000e9c20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000e9c30: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000e9c40: 7265 736f 7572 6365 5f74 7970 6527 5d20  resource_type'] 
-000e9c50: 3d20 7365 6c66 2e72 6573 6f75 7263 655f  = self.resource_
-000e9c60: 7479 7065 0a20 2020 2020 2020 2069 6620  type.        if 
-000e9c70: 7365 6c66 2e74 6167 5f6b 6579 735f 7368  self.tag_keys_sh
-000e9c80: 7269 6e6b 2069 7320 6e6f 7420 4e6f 6e65  rink is not None
-000e9c90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000e9ca0: 7375 6c74 5b27 7461 675f 6b65 7973 275d  sult['tag_keys']
-000e9cb0: 203d 2073 656c 662e 7461 675f 6b65 7973   = self.tag_keys
-000e9cc0: 5f73 6872 696e 6b0a 2020 2020 2020 2020  _shrink.        
-000e9cd0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000e9ce0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000e9cf0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-000e9d00: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-000e9d10: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000e9d20: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000e9d30: 2761 6c6c 2729 2069 7320 6e6f 7420 4e6f  'all') is not No
-000e9d40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000e9d50: 7365 6c66 2e61 6c6c 203d 206d 2e67 6574  self.all = m.get
-000e9d60: 2827 616c 6c27 290a 2020 2020 2020 2020  ('all').        
-000e9d70: 6966 206d 2e67 6574 2827 7265 6769 6f6e  if m.get('region
-000e9d80: 5f69 6427 2920 6973 206e 6f74 204e 6f6e  _id') is not Non
-000e9d90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000e9da0: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
-000e9db0: 6d2e 6765 7428 2772 6567 696f 6e5f 6964  m.get('region_id
-000e9dc0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000e9dd0: 6765 7428 2772 6573 6f75 7263 655f 6964  get('resource_id
-000e9de0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-000e9df0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000e9e00: 662e 7265 736f 7572 6365 5f69 6473 5f73  f.resource_ids_s
-000e9e10: 6872 696e 6b20 3d20 6d2e 6765 7428 2772  hrink = m.get('r
-000e9e20: 6573 6f75 7263 655f 6964 7327 290a 2020  esource_ids').  
-000e9e30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000e9e40: 7265 736f 7572 6365 5f74 7970 6527 2920  resource_type') 
-000e9e50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000e9e60: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000e9e70: 736f 7572 6365 5f74 7970 6520 3d20 6d2e  source_type = m.
-000e9e80: 6765 7428 2772 6573 6f75 7263 655f 7479  get('resource_ty
-000e9e90: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-000e9ea0: 6d2e 6765 7428 2774 6167 5f6b 6579 7327  m.get('tag_keys'
-000e9eb0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000e9ec0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000e9ed0: 7461 675f 6b65 7973 5f73 6872 696e 6b20  tag_keys_shrink 
-000e9ee0: 3d20 6d2e 6765 7428 2774 6167 5f6b 6579  = m.get('tag_key
-000e9ef0: 7327 290a 2020 2020 2020 2020 7265 7475  s').        retu
-000e9f00: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000e9f10: 556e 7461 6752 6573 6f75 7263 6573 5265  UntagResourcesRe
-000e9f20: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
-000e9f30: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-000e9f40: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000e9f50: 7365 6c66 2c0a 2020 2020 2020 2020 7265  self,.        re
-000e9f60: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
-000e9f70: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000e9f80: 2020 2020 2023 2054 6865 2072 6571 7565       # The reque
-000e9f90: 7374 2049 442e 0a20 2020 2020 2020 2073  st ID..        s
-000e9fa0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-000e9fb0: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
-000e9fc0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000e9fd0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-000e9fe0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-000e9ff0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000ea000: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000ea010: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000ea020: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000ea030: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ea040: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000ea050: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000ea060: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000ea070: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
-000ea080: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000ea090: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000ea0a0: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
-000ea0b0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-000ea0c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000ea0d0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-000ea0e0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-000ea0f0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-000ea100: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000ea110: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000ea120: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
-000ea130: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
-000ea140: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000ea150: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-000ea160: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-000ea170: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
-000ea180: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000ea190: 556e 7461 6752 6573 6f75 7263 6573 5265  UntagResourcesRe
-000ea1a0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-000ea1b0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000ea1c0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000ea1d0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-000ea1e0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-000ea1f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000ea200: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-000ea210: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-000ea220: 2020 2062 6f64 793a 2055 6e74 6167 5265     body: UntagRe
-000ea230: 736f 7572 6365 7352 6573 706f 6e73 6542  sourcesResponseB
-000ea240: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
-000ea250: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000ea260: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-000ea270: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-000ea280: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-000ea290: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-000ea2a0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-000ea2b0: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-000ea2c0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000ea2d0: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-000ea2e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000ea2f0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-000ea300: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000ea310: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000ea320: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000ea330: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000ea340: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000ea350: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ea360: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000ea370: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000ea380: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000ea390: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-000ea3a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ea3b0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ea3c0: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-000ea3d0: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-000ea3e0: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-000ea3f0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-000ea400: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000ea410: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-000ea420: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-000ea430: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-000ea440: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-000ea450: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000ea460: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-000ea470: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-000ea480: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000ea490: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000ea4a0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000ea4b0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-000ea4c0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-000ea4d0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000ea4e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000ea4f0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-000ea500: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000ea510: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-000ea520: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-000ea530: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-000ea540: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-000ea550: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000ea560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000ea570: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-000ea580: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-000ea590: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000ea5a0: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-000ea5b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000ea5c0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-000ea5d0: 3d20 556e 7461 6752 6573 6f75 7263 6573  = UntagResources
-000ea5e0: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
-000ea5f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000ea600: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
-000ea610: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
-000ea620: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
-000ea630: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000ea640: 7320 5570 6461 7465 436f 6e74 6163 7447  s UpdateContactG
-000ea650: 726f 7570 466f 7241 6c65 7274 5265 7370  roupForAlertResp
-000ea660: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-000ea670: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000ea680: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000ea690: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-000ea6a0: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-000ea6b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000ea6c0: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-000ea6d0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000ea6e0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000ea6f0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-000ea700: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000ea710: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-000ea720: 5f63 6f64 650a 0a20 2020 2064 6566 2076  _code..    def v
-000ea730: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000ea740: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-000ea750: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-000ea760: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-000ea770: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-000ea780: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-000ea790: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-000ea7a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000ea7b0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-000ea7c0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-000ea7d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000ea7e0: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
-000ea7f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ea800: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
-000ea810: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
-000ea820: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
-000ea830: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
-000ea840: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ea850: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ea860: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
-000ea870: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
-000ea880: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000ea890: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-000ea8a0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-000ea8b0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-000ea8c0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-000ea8d0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000ea8e0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-000ea8f0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000ea900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000ea910: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-000ea920: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-000ea930: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-000ea940: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-000ea950: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000ea960: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-000ea970: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-000ea980: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-000ea990: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-000ea9a0: 0a63 6c61 7373 2055 7064 6174 6543 6f6e  .class UpdateCon
-000ea9b0: 7472 6f6c 506c 616e 654c 6f67 5265 7175  trolPlaneLogRequ
-000ea9c0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-000ea9d0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000ea9e0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000ea9f0: 2020 2020 2020 2061 6c69 7569 643a 2073         aliuid: s
-000eaa00: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000eaa10: 2020 2063 6f6d 706f 6e65 6e74 733a 204c     components: L
-000eaa20: 6973 745b 7374 725d 203d 204e 6f6e 652c  ist[str] = None,
-000eaa30: 0a20 2020 2020 2020 206c 6f67 5f70 726f  .        log_pro
-000eaa40: 6a65 6374 3a20 7374 7220 3d20 4e6f 6e65  ject: str = None
-000eaa50: 2c0a 2020 2020 2020 2020 6c6f 675f 7474  ,.        log_tt
-000eaa60: 6c3a 2073 7472 203d 204e 6f6e 652c 0a20  l: str = None,. 
-000eaa70: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000eaa80: 5468 6520 4944 206f 6620 7468 6520 416c  The ID of the Al
-000eaa90: 6962 6162 6120 436c 6f75 6420 6163 636f  ibaba Cloud acco
-000eaaa0: 756e 742e 0a20 2020 2020 2020 2073 656c  unt..        sel
-000eaab0: 662e 616c 6975 6964 203d 2061 6c69 7569  f.aliuid = aliui
-000eaac0: 640a 2020 2020 2020 2020 2320 5468 6520  d.        # The 
-000eaad0: 636f 6e74 726f 6c20 706c 616e 6520 636f  control plane co
-000eaae0: 6d70 6f6e 656e 7473 2066 6f72 2077 6869  mponents for whi
-000eaaf0: 6368 2079 6f75 2077 616e 7420 746f 2065  ch you want to e
-000eab00: 6e61 626c 6520 6c6f 6720 636f 6c6c 6563  nable log collec
-000eab10: 7469 6f6e 2e0a 2020 2020 2020 2020 7365  tion..        se
-000eab20: 6c66 2e63 6f6d 706f 6e65 6e74 7320 3d20  lf.components = 
-000eab30: 636f 6d70 6f6e 656e 7473 0a20 2020 2020  components.     
-000eab40: 2020 2023 2054 6865 206e 616d 6520 6f66     # The name of
-000eab50: 2074 6865 2053 696d 706c 6520 4c6f 6720   the Simple Log 
-000eab60: 5365 7276 6963 6520 7072 6f6a 6563 7420  Service project 
-000eab70: 7468 6174 2079 6f75 2077 616e 7420 746f  that you want to
-000eab80: 2075 7365 2074 6f20 7374 6f72 6520 7468   use to store th
-000eab90: 6520 6c6f 6773 206f 6620 636f 6e74 726f  e logs of contro
-000eaba0: 6c20 706c 616e 6520 636f 6d70 6f6e 656e  l plane componen
-000eabb0: 7473 2e0a 2020 2020 2020 2020 2320 0a20  ts..        # . 
-000eabc0: 2020 2020 2020 2023 2044 6566 6175 6c74         # Default
-000eabd0: 2076 616c 7565 3a20 6b38 732d 6c6f 672d   value: k8s-log-
-000eabe0: 2443 6c75 7374 6572 2049 442e 0a20 2020  $Cluster ID..   
-000eabf0: 2020 2020 2073 656c 662e 6c6f 675f 7072       self.log_pr
-000eac00: 6f6a 6563 7420 3d20 6c6f 675f 7072 6f6a  oject = log_proj
-000eac10: 6563 740a 2020 2020 2020 2020 2320 5468  ect.        # Th
-000eac20: 6520 7265 7465 6e74 696f 6e20 7065 7269  e retention peri
-000eac30: 6f64 206f 6620 7468 6520 6c6f 6720 6461  od of the log da
-000eac40: 7461 2073 746f 7265 6420 696e 2074 6865  ta stored in the
-000eac50: 204c 6f67 7374 6f72 652e 2056 616c 6964   Logstore. Valid
-000eac60: 2076 616c 7565 733a 2031 2074 6f20 3330   values: 1 to 30
-000eac70: 3030 2e20 556e 6974 3a20 6461 7973 2e0a  00. Unit: days..
-000eac80: 2020 2020 2020 2020 2320 0a20 2020 2020          # .     
-000eac90: 2020 2023 2044 6566 6175 6c74 2076 616c     # Default val
-000eaca0: 7565 3a20 3330 2e0a 2020 2020 2020 2020  ue: 30..        
-000eacb0: 7365 6c66 2e6c 6f67 5f74 746c 203d 206c  self.log_ttl = l
-000eacc0: 6f67 5f74 746c 0a0a 2020 2020 6465 6620  og_ttl..    def 
-000eacd0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000eace0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000eacf0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000ead00: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-000ead10: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-000ead20: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-000ead30: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-000ead40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000ead50: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-000ead60: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-000ead70: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000ead80: 662e 616c 6975 6964 2069 7320 6e6f 7420  f.aliuid is not 
-000ead90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000eada0: 2020 7265 7375 6c74 5b27 616c 6975 6964    result['aliuid
-000eadb0: 275d 203d 2073 656c 662e 616c 6975 6964  '] = self.aliuid
-000eadc0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000eadd0: 2e63 6f6d 706f 6e65 6e74 7320 6973 206e  .components is n
-000eade0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000eadf0: 2020 2020 2072 6573 756c 745b 2763 6f6d       result['com
-000eae00: 706f 6e65 6e74 7327 5d20 3d20 7365 6c66  ponents'] = self
-000eae10: 2e63 6f6d 706f 6e65 6e74 730a 2020 2020  .components.    
-000eae20: 2020 2020 6966 2073 656c 662e 6c6f 675f      if self.log_
-000eae30: 7072 6f6a 6563 7420 6973 206e 6f74 204e  project is not N
-000eae40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000eae50: 2072 6573 756c 745b 276c 6f67 5f70 726f   result['log_pro
-000eae60: 6a65 6374 275d 203d 2073 656c 662e 6c6f  ject'] = self.lo
-000eae70: 675f 7072 6f6a 6563 740a 2020 2020 2020  g_project.      
-000eae80: 2020 6966 2073 656c 662e 6c6f 675f 7474    if self.log_tt
-000eae90: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
-000eaea0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000eaeb0: 745b 276c 6f67 5f74 746c 275d 203d 2073  t['log_ttl'] = s
-000eaec0: 656c 662e 6c6f 675f 7474 6c0a 2020 2020  elf.log_ttl.    
-000eaed0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000eaee0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000eaef0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000eaf00: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000eaf10: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000eaf20: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000eaf30: 6765 7428 2761 6c69 7569 6427 2920 6973  get('aliuid') is
-000eaf40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000eaf50: 2020 2020 2020 2073 656c 662e 616c 6975         self.aliu
-000eaf60: 6964 203d 206d 2e67 6574 2827 616c 6975  id = m.get('aliu
-000eaf70: 6964 2729 0a20 2020 2020 2020 2069 6620  id').        if 
-000eaf80: 6d2e 6765 7428 2763 6f6d 706f 6e65 6e74  m.get('component
-000eaf90: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-000eafa0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000eafb0: 662e 636f 6d70 6f6e 656e 7473 203d 206d  f.components = m
-000eafc0: 2e67 6574 2827 636f 6d70 6f6e 656e 7473  .get('components
-000eafd0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000eafe0: 6765 7428 276c 6f67 5f70 726f 6a65 6374  get('log_project
-000eaff0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000eb000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000eb010: 2e6c 6f67 5f70 726f 6a65 6374 203d 206d  .log_project = m
-000eb020: 2e67 6574 2827 6c6f 675f 7072 6f6a 6563  .get('log_projec
-000eb030: 7427 290a 2020 2020 2020 2020 6966 206d  t').        if m
-000eb040: 2e67 6574 2827 6c6f 675f 7474 6c27 2920  .get('log_ttl') 
-000eb050: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000eb060: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-000eb070: 675f 7474 6c20 3d20 6d2e 6765 7428 276c  g_ttl = m.get('l
-000eb080: 6f67 5f74 746c 2729 0a20 2020 2020 2020  og_ttl').       
-000eb090: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000eb0a0: 6c61 7373 2055 7064 6174 6543 6f6e 7472  lass UpdateContr
-000eb0b0: 6f6c 506c 616e 654c 6f67 5265 7370 6f6e  olPlaneLogRespon
-000eb0c0: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-000eb0d0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000eb0e0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000eb0f0: 2c0a 2020 2020 2020 2020 636c 7573 7465  ,.        cluste
-000eb100: 725f 6964 3a20 7374 7220 3d20 4e6f 6e65  r_id: str = None
-000eb110: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
-000eb120: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
-000eb130: 2c0a 2020 2020 2020 2020 7461 736b 5f69  ,.        task_i
-000eb140: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-000eb150: 2020 2029 3a0a 2020 2020 2020 2020 2320     ):.        # 
-000eb160: 5468 6520 636c 7573 7465 7220 4944 2e0a  The cluster ID..
-000eb170: 2020 2020 2020 2020 7365 6c66 2e63 6c75          self.clu
-000eb180: 7374 6572 5f69 6420 3d20 636c 7573 7465  ster_id = cluste
-000eb190: 725f 6964 0a20 2020 2020 2020 2023 2054  r_id.        # T
-000eb1a0: 6865 2072 6571 7565 7374 2049 442e 0a20  he request ID.. 
-000eb1b0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-000eb1c0: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
-000eb1d0: 5f69 640a 2020 2020 2020 2020 2320 5468  _id.        # Th
-000eb1e0: 6520 7461 736b 2049 442e 0a20 2020 2020  e task ID..     
-000eb1f0: 2020 2073 656c 662e 7461 736b 5f69 6420     self.task_id 
-000eb200: 3d20 7461 736b 5f69 640a 0a20 2020 2064  = task_id..    d
-000eb210: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000eb220: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000eb230: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000eb240: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000eb250: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-000eb260: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000eb270: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000eb280: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000eb290: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000eb2a0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000eb2b0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000eb2c0: 7365 6c66 2e63 6c75 7374 6572 5f69 6420  self.cluster_id 
-000eb2d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000eb2e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000eb2f0: 2763 6c75 7374 6572 5f69 6427 5d20 3d20  'cluster_id'] = 
-000eb300: 7365 6c66 2e63 6c75 7374 6572 5f69 640a  self.cluster_id.
-000eb310: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000eb320: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
-000eb330: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000eb340: 2020 2020 7265 7375 6c74 5b27 7265 7175      result['requ
-000eb350: 6573 745f 6964 275d 203d 2073 656c 662e  est_id'] = self.
-000eb360: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
-000eb370: 2020 2069 6620 7365 6c66 2e74 6173 6b5f     if self.task_
-000eb380: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-000eb390: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000eb3a0: 6c74 5b27 7461 736b 5f69 6427 5d20 3d20  lt['task_id'] = 
-000eb3b0: 7365 6c66 2e74 6173 6b5f 6964 0a20 2020  self.task_id.   
-000eb3c0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000eb3d0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-000eb3e0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-000eb3f0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-000eb400: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-000eb410: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-000eb420: 2e67 6574 2827 636c 7573 7465 725f 6964  .get('cluster_id
-000eb430: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000eb440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000eb450: 2e63 6c75 7374 6572 5f69 6420 3d20 6d2e  .cluster_id = m.
-000eb460: 6765 7428 2763 6c75 7374 6572 5f69 6427  get('cluster_id'
-000eb470: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000eb480: 6574 2827 7265 7175 6573 745f 6964 2729  et('request_id')
-000eb490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000eb4a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000eb4b0: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-000eb4c0: 7428 2772 6571 7565 7374 5f69 6427 290a  t('request_id').
-000eb4d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000eb4e0: 2827 7461 736b 5f69 6427 2920 6973 206e  ('task_id') is n
-000eb4f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000eb500: 2020 2020 2073 656c 662e 7461 736b 5f69       self.task_i
-000eb510: 6420 3d20 6d2e 6765 7428 2774 6173 6b5f  d = m.get('task_
-000eb520: 6964 2729 0a20 2020 2020 2020 2072 6574  id').        ret
-000eb530: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-000eb540: 2055 7064 6174 6543 6f6e 7472 6f6c 506c   UpdateControlPl
-000eb550: 616e 654c 6f67 5265 7370 6f6e 7365 2854  aneLogResponse(T
-000eb560: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-000eb570: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-000eb580: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000eb590: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
-000eb5a0: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
-000eb5b0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
-000eb5c0: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
-000eb5d0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
-000eb5e0: 2055 7064 6174 6543 6f6e 7472 6f6c 506c   UpdateControlPl
-000eb5f0: 616e 654c 6f67 5265 7370 6f6e 7365 426f  aneLogResponseBo
-000eb600: 6479 203d 204e 6f6e 652c 0a20 2020 2029  dy = None,.    )
-000eb610: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-000eb620: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-000eb630: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-000eb640: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
-000eb650: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-000eb660: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
-000eb670: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000eb680: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000eb690: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-000eb6a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000eb6b0: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-000eb6c0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000eb6d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000eb6e0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000eb6f0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000eb700: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000eb710: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000eb720: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000eb730: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000eb740: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000eb750: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-000eb760: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000eb770: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-000eb780: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-000eb790: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-000eb7a0: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-000eb7b0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-000eb7c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000eb7d0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-000eb7e0: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-000eb7f0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-000eb800: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-000eb810: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000eb820: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-000eb830: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-000eb840: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-000eb850: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000eb860: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000eb870: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000eb880: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000eb890: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000eb8a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000eb8b0: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-000eb8c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000eb8d0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-000eb8e0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-000eb8f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000eb900: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-000eb910: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000eb920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000eb930: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-000eb940: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-000eb950: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000eb960: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-000eb970: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000eb980: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-000eb990: 2055 7064 6174 6543 6f6e 7472 6f6c 506c   UpdateControlPl
-000eb9a0: 616e 654c 6f67 5265 7370 6f6e 7365 426f  aneLogResponseBo
-000eb9b0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
-000eb9c0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-000eb9d0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-000eb9e0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-000eb9f0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-000eba00: 0a0a 636c 6173 7320 5570 6461 7465 4b38  ..class UpdateK8
-000eba10: 7343 6c75 7374 6572 5573 6572 436f 6e66  sClusterUserConf
-000eba20: 6967 4578 7069 7265 5265 7175 6573 7428  igExpireRequest(
-000eba30: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-000eba40: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000eba50: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000eba60: 2020 2065 7870 6972 655f 686f 7572 3a20     expire_hour: 
-000eba70: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
-000eba80: 2020 2020 7573 6572 3a20 7374 7220 3d20      user: str = 
-000eba90: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-000ebaa0: 2020 2020 2023 2054 6865 2076 616c 6964       # The valid
-000ebab0: 6974 7920 7065 7269 6f64 206f 6620 7468  ity period of th
-000ebac0: 6520 6b75 6265 636f 6e66 6967 2066 696c  e kubeconfig fil
-000ebad0: 652e 2055 6e69 743a 2068 6f75 7273 2e0a  e. Unit: hours..
-000ebae0: 2020 2020 2020 2020 2320 0a20 2020 2020          # .     
-000ebaf0: 2020 2023 203e 2054 6865 2076 616c 7565     # > The value
-000ebb00: 206f 6620 6578 7069 7265 5f68 6f75 7220   of expire_hour 
-000ebb10: 6d75 7374 2062 6520 6772 6561 7465 7220  must be greater 
-000ebb20: 7468 616e 2030 2061 6e64 2065 7175 616c  than 0 and equal
-000ebb30: 2074 6f20 6f72 2073 6d61 6c6c 6572 2074   to or smaller t
-000ebb40: 6861 6e20 3837 3630 3030 2028 3130 3020  han 876000 (100 
-000ebb50: 7965 6172 7329 2e0a 2020 2020 2020 2020  years)..        
-000ebb60: 2320 0a20 2020 2020 2020 2023 2054 6869  # .        # Thi
-000ebb70: 7320 7061 7261 6d65 7465 7220 6973 2072  s parameter is r
-000ebb80: 6571 7569 7265 642e 0a20 2020 2020 2020  equired..       
-000ebb90: 2073 656c 662e 6578 7069 7265 5f68 6f75   self.expire_hou
-000ebba0: 7220 3d20 6578 7069 7265 5f68 6f75 720a  r = expire_hour.
-000ebbb0: 2020 2020 2020 2020 2320 5468 6520 7573          # The us
-000ebbc0: 6572 2049 442e 0a20 2020 2020 2020 2023  er ID..        #
-000ebbd0: 200a 2020 2020 2020 2020 2320 5468 6973   .        # This
-000ebbe0: 2070 6172 616d 6574 6572 2069 7320 7265   parameter is re
-000ebbf0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-000ebc00: 7365 6c66 2e75 7365 7220 3d20 7573 6572  self.user = user
-000ebc10: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000ebc20: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000ebc30: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-000ebc40: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-000ebc50: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000ebc60: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-000ebc70: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-000ebc80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000ebc90: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-000ebca0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-000ebcb0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000ebcc0: 2020 2020 6966 2073 656c 662e 6578 7069      if self.expi
-000ebcd0: 7265 5f68 6f75 7220 6973 206e 6f74 204e  re_hour is not N
-000ebce0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000ebcf0: 2072 6573 756c 745b 2765 7870 6972 655f   result['expire_
-000ebd00: 686f 7572 275d 203d 2073 656c 662e 6578  hour'] = self.ex
-000ebd10: 7069 7265 5f68 6f75 720a 2020 2020 2020  pire_hour.      
-000ebd20: 2020 6966 2073 656c 662e 7573 6572 2069    if self.user i
-000ebd30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ebd40: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ebd50: 7573 6572 275d 203d 2073 656c 662e 7573  user'] = self.us
-000ebd60: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
-000ebd70: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000ebd80: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000ebd90: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000ebda0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000ebdb0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000ebdc0: 2020 6966 206d 2e67 6574 2827 6578 7069    if m.get('expi
-000ebdd0: 7265 5f68 6f75 7227 2920 6973 206e 6f74  re_hour') is not
-000ebde0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ebdf0: 2020 2073 656c 662e 6578 7069 7265 5f68     self.expire_h
-000ebe00: 6f75 7220 3d20 6d2e 6765 7428 2765 7870  our = m.get('exp
-000ebe10: 6972 655f 686f 7572 2729 0a20 2020 2020  ire_hour').     
-000ebe20: 2020 2069 6620 6d2e 6765 7428 2775 7365     if m.get('use
-000ebe30: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
-000ebe40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000ebe50: 662e 7573 6572 203d 206d 2e67 6574 2827  f.user = m.get('
-000ebe60: 7573 6572 2729 0a20 2020 2020 2020 2072  user').        r
-000ebe70: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-000ebe80: 7373 2055 7064 6174 654b 3873 436c 7573  ss UpdateK8sClus
-000ebe90: 7465 7255 7365 7243 6f6e 6669 6745 7870  terUserConfigExp
-000ebea0: 6972 6552 6573 706f 6e73 6528 5465 614d  ireResponse(TeaM
-000ebeb0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000ebec0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-000ebed0: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
-000ebee0: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
-000ebef0: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
-000ebf00: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
-000ebf10: 6465 3a20 696e 7420 3d20 4e6f 6e65 2c0a  de: int = None,.
-000ebf20: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-000ebf30: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-000ebf40: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-000ebf50: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-000ebf60: 2073 7461 7475 735f 636f 6465 0a0a 2020   status_code..  
-000ebf70: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-000ebf80: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000ebf90: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-000ebfa0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-000ebfb0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-000ebfc0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-000ebfd0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-000ebfe0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ebff0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-000ec000: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000ec010: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000ec020: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-000ec030: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000ec040: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000ec050: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-000ec060: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-000ec070: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-000ec080: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-000ec090: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000ec0a0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-000ec0b0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-000ec0c0: 735f 636f 6465 0a20 2020 2020 2020 2072  s_code.        r
-000ec0d0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000ec0e0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000ec0f0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000ec100: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000ec110: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000ec120: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000ec130: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-000ec140: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ec150: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-000ec160: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-000ec170: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000ec180: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-000ec190: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000ec1a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000ec1b0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-000ec1c0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-000ec1d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000ec1e0: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-000ec1f0: 6461 7465 5465 6d70 6c61 7465 5265 7175  dateTemplateRequ
-000ec200: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-000ec210: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000ec220: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000ec230: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000ec240: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
-000ec250: 2020 2020 2020 2020 6e61 6d65 3a20 7374          name: st
-000ec260: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-000ec270: 2020 7461 6773 3a20 7374 7220 3d20 4e6f    tags: str = No
-000ec280: 6e65 2c0a 2020 2020 2020 2020 7465 6d70  ne,.        temp
-000ec290: 6c61 7465 3a20 7374 7220 3d20 4e6f 6e65  late: str = None
-000ec2a0: 2c0a 2020 2020 2020 2020 7465 6d70 6c61  ,.        templa
-000ec2b0: 7465 5f74 7970 653a 2073 7472 203d 204e  te_type: str = N
-000ec2c0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000ec2d0: 2020 2020 2320 5468 6520 6465 7363 7269      # The descri
-000ec2e0: 7074 696f 6e20 6f66 2074 6865 2074 656d  ption of the tem
-000ec2f0: 706c 6174 652e 0a20 2020 2020 2020 2073  plate..        s
-000ec300: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
-000ec310: 3d20 6465 7363 7269 7074 696f 6e0a 2020  = description.  
-000ec320: 2020 2020 2020 2320 5468 6520 6e61 6d65        # The name
-000ec330: 206f 6620 7468 6520 7465 6d70 6c61 7465   of the template
-000ec340: 2e0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-000ec350: 616d 6520 3d20 6e61 6d65 0a20 2020 2020  ame = name.     
-000ec360: 2020 2023 2054 6865 206c 6162 656c 206f     # The label o
-000ec370: 6620 7468 6520 7465 6d70 6c61 7465 2e0a  f the template..
-000ec380: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
-000ec390: 7320 3d20 7461 6773 0a20 2020 2020 2020  s = tags.       
-000ec3a0: 2023 2054 6865 2059 414d 4c20 636f 6e74   # The YAML cont
-000ec3b0: 656e 7420 6f66 2074 6865 2074 656d 706c  ent of the templ
-000ec3c0: 6174 652e 0a20 2020 2020 2020 2073 656c  ate..        sel
-000ec3d0: 662e 7465 6d70 6c61 7465 203d 2074 656d  f.template = tem
-000ec3e0: 706c 6174 650a 2020 2020 2020 2020 2320  plate.        # 
-000ec3f0: 5468 6520 7479 7065 206f 6620 7465 6d70  The type of temp
-000ec400: 6c61 7465 2e20 5468 6973 2070 6172 616d  late. This param
-000ec410: 6574 6572 2063 616e 2062 6520 7365 7420  eter can be set 
-000ec420: 746f 2061 2063 7573 746f 6d20 7661 6c75  to a custom valu
-000ec430: 652e 0a20 2020 2020 2020 2023 200a 2020  e..        # .  
-000ec440: 2020 2020 2020 2320 2a20 2020 4966 2074        # *   If t
-000ec450: 6865 2070 6172 616d 6574 6572 2069 7320  he parameter is 
-000ec460: 7365 7420 746f 2060 6b75 6265 726e 6574  set to `kubernet
-000ec470: 6573 602c 2074 6865 2074 656d 706c 6174  es`, the templat
-000ec480: 6520 6973 2064 6973 706c 6179 6564 206f  e is displayed o
-000ec490: 6e20 7468 6520 5465 6d70 6c61 7465 7320  n the Templates 
-000ec4a0: 7061 6765 2069 6e20 7468 6520 636f 6e73  page in the cons
-000ec4b0: 6f6c 652e 0a20 2020 2020 2020 2023 202a  ole..        # *
-000ec4c0: 2020 2049 6620 7468 6520 7061 7261 6d65     If the parame
-000ec4d0: 7465 7220 6973 2073 6574 2074 6f20 6063  ter is set to `c
-000ec4e0: 6f6d 706f 7365 602c 2074 6865 2074 656d  ompose`, the tem
-000ec4f0: 706c 6174 6520 6973 2064 6973 706c 6179  plate is display
-000ec500: 6564 206f 6e20 7468 6520 436f 6e74 6169  ed on the Contai
-000ec510: 6e65 7220 5365 7276 6963 6520 2d20 5377  ner Service - Sw
-000ec520: 6172 6d20 7061 6765 2069 6e20 7468 6520  arm page in the 
-000ec530: 636f 6e73 6f6c 652e 2043 6f6e 7461 696e  console. Contain
-000ec540: 6572 2053 6572 7669 6365 2066 6f72 2053  er Service for S
-000ec550: 7761 726d 2069 7320 6465 7072 6563 6174  warm is deprecat
-000ec560: 6564 2e0a 2020 2020 2020 2020 7365 6c66  ed..        self
-000ec570: 2e74 656d 706c 6174 655f 7479 7065 203d  .template_type =
-000ec580: 2074 656d 706c 6174 655f 7479 7065 0a0a   template_type..
-000ec590: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000ec5a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000ec5b0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-000ec5c0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-000ec5d0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-000ec5e0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-000ec5f0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-000ec600: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000ec610: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-000ec620: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000ec630: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000ec640: 2020 6966 2073 656c 662e 6465 7363 7269    if self.descri
-000ec650: 7074 696f 6e20 6973 206e 6f74 204e 6f6e  ption is not Non
-000ec660: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000ec670: 6573 756c 745b 2764 6573 6372 6970 7469  esult['descripti
-000ec680: 6f6e 275d 203d 2073 656c 662e 6465 7363  on'] = self.desc
-000ec690: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
-000ec6a0: 6966 2073 656c 662e 6e61 6d65 2069 7320  if self.name is 
-000ec6b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ec6c0: 2020 2020 2020 7265 7375 6c74 5b27 6e61        result['na
-000ec6d0: 6d65 275d 203d 2073 656c 662e 6e61 6d65  me'] = self.name
-000ec6e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000ec6f0: 2e74 6167 7320 6973 206e 6f74 204e 6f6e  .tags is not Non
-000ec700: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000ec710: 6573 756c 745b 2774 6167 7327 5d20 3d20  esult['tags'] = 
-000ec720: 7365 6c66 2e74 6167 730a 2020 2020 2020  self.tags.      
-000ec730: 2020 6966 2073 656c 662e 7465 6d70 6c61    if self.templa
-000ec740: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  te is not None:.
-000ec750: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000ec760: 6c74 5b27 7465 6d70 6c61 7465 275d 203d  lt['template'] =
-000ec770: 2073 656c 662e 7465 6d70 6c61 7465 0a20   self.template. 
-000ec780: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-000ec790: 656d 706c 6174 655f 7479 7065 2069 7320  emplate_type is 
-000ec7a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ec7b0: 2020 2020 2020 7265 7375 6c74 5b27 7465        result['te
-000ec7c0: 6d70 6c61 7465 5f74 7970 6527 5d20 3d20  mplate_type'] = 
-000ec7d0: 7365 6c66 2e74 656d 706c 6174 655f 7479  self.template_ty
-000ec7e0: 7065 0a20 2020 2020 2020 2072 6574 7572  pe.        retur
-000ec7f0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000ec800: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000ec810: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000ec820: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000ec830: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000ec840: 2020 6966 206d 2e67 6574 2827 6465 7363    if m.get('desc
-000ec850: 7269 7074 696f 6e27 2920 6973 206e 6f74  ription') is not
-000ec860: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ec870: 2020 2073 656c 662e 6465 7363 7269 7074     self.descript
-000ec880: 696f 6e20 3d20 6d2e 6765 7428 2764 6573  ion = m.get('des
-000ec890: 6372 6970 7469 6f6e 2729 0a20 2020 2020  cription').     
-000ec8a0: 2020 2069 6620 6d2e 6765 7428 276e 616d     if m.get('nam
-000ec8b0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-000ec8c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000ec8d0: 662e 6e61 6d65 203d 206d 2e67 6574 2827  f.name = m.get('
-000ec8e0: 6e61 6d65 2729 0a20 2020 2020 2020 2069  name').        i
-000ec8f0: 6620 6d2e 6765 7428 2774 6167 7327 2920  f m.get('tags') 
-000ec900: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000ec910: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-000ec920: 6773 203d 206d 2e67 6574 2827 7461 6773  gs = m.get('tags
-000ec930: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000ec940: 6765 7428 2774 656d 706c 6174 6527 2920  get('template') 
-000ec950: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000ec960: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-000ec970: 6d70 6c61 7465 203d 206d 2e67 6574 2827  mplate = m.get('
-000ec980: 7465 6d70 6c61 7465 2729 0a20 2020 2020  template').     
-000ec990: 2020 2069 6620 6d2e 6765 7428 2774 656d     if m.get('tem
-000ec9a0: 706c 6174 655f 7479 7065 2729 2069 7320  plate_type') is 
-000ec9b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ec9c0: 2020 2020 2020 7365 6c66 2e74 656d 706c        self.templ
-000ec9d0: 6174 655f 7479 7065 203d 206d 2e67 6574  ate_type = m.get
-000ec9e0: 2827 7465 6d70 6c61 7465 5f74 7970 6527  ('template_type'
-000ec9f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000eca00: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-000eca10: 6461 7465 5465 6d70 6c61 7465 5265 7370  dateTemplateResp
-000eca20: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-000eca30: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000eca40: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000eca50: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-000eca60: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-000eca70: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000eca80: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-000eca90: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000ecaa0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000ecab0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-000ecac0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000ecad0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-000ecae0: 5f63 6f64 650a 0a20 2020 2064 6566 2076  _code..    def v
-000ecaf0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000ecb00: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-000ecb10: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-000ecb20: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-000ecb30: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-000ecb40: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-000ecb50: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-000ecb60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000ecb70: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-000ecb80: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-000ecb90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000ecba0: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
-000ecbb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ecbc0: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
-000ecbd0: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
-000ecbe0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
-000ecbf0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
-000ecc00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ecc10: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ecc20: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
-000ecc30: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
-000ecc40: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000ecc50: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-000ecc60: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-000ecc70: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-000ecc80: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-000ecc90: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000ecca0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-000eccb0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000eccc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000eccd0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-000ecce0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-000eccf0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-000ecd00: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-000ecd10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000ecd20: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-000ecd30: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-000ecd40: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-000ecd50: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-000ecd60: 0a63 6c61 7373 2055 7064 6174 6555 7365  .class UpdateUse
-000ecd70: 7250 6572 6d69 7373 696f 6e73 5265 7175  rPermissionsRequ
-000ecd80: 6573 7442 6f64 7928 5465 614d 6f64 656c  estBody(TeaModel
-000ecd90: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-000ecda0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000ecdb0: 662c 0a20 2020 2020 2020 2063 6c75 7374  f,.        clust
-000ecdc0: 6572 3a20 7374 7220 3d20 4e6f 6e65 2c0a  er: str = None,.
-000ecdd0: 2020 2020 2020 2020 6973 5f63 7573 746f          is_custo
-000ecde0: 6d3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  m: bool = None,.
-000ecdf0: 2020 2020 2020 2020 6973 5f72 616d 5f72          is_ram_r
-000ece00: 6f6c 653a 2062 6f6f 6c20 3d20 4e6f 6e65  ole: bool = None
-000ece10: 2c0a 2020 2020 2020 2020 6e61 6d65 7370  ,.        namesp
-000ece20: 6163 653a 2073 7472 203d 204e 6f6e 652c  ace: str = None,
-000ece30: 0a20 2020 2020 2020 2072 6f6c 655f 6e61  .        role_na
-000ece40: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-000ece50: 2020 2020 2020 2020 726f 6c65 5f74 7970          role_typ
-000ece60: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-000ece70: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-000ece80: 6c66 2e63 6c75 7374 6572 203d 2063 6c75  lf.cluster = clu
-000ece90: 7374 6572 0a20 2020 2020 2020 2073 656c  ster.        sel
-000ecea0: 662e 6973 5f63 7573 746f 6d20 3d20 6973  f.is_custom = is
-000eceb0: 5f63 7573 746f 6d0a 2020 2020 2020 2020  _custom.        
-000ecec0: 7365 6c66 2e69 735f 7261 6d5f 726f 6c65  self.is_ram_role
-000eced0: 203d 2069 735f 7261 6d5f 726f 6c65 0a20   = is_ram_role. 
-000ecee0: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
-000ecef0: 7370 6163 6520 3d20 6e61 6d65 7370 6163  space = namespac
-000ecf00: 650a 2020 2020 2020 2020 7365 6c66 2e72  e.        self.r
-000ecf10: 6f6c 655f 6e61 6d65 203d 2072 6f6c 655f  ole_name = role_
-000ecf20: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
-000ecf30: 662e 726f 6c65 5f74 7970 6520 3d20 726f  f.role_type = ro
-000ecf40: 6c65 5f74 7970 650a 0a20 2020 2064 6566  le_type..    def
-000ecf50: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000ecf60: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000ecf70: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-000ecf80: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-000ecf90: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-000ecfa0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-000ecfb0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-000ecfc0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000ecfd0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-000ecfe0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-000ecff0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-000ed000: 6c66 2e63 6c75 7374 6572 2069 7320 6e6f  lf.cluster is no
-000ed010: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000ed020: 2020 2020 7265 7375 6c74 5b27 636c 7573      result['clus
-000ed030: 7465 7227 5d20 3d20 7365 6c66 2e63 6c75  ter'] = self.clu
-000ed040: 7374 6572 0a20 2020 2020 2020 2069 6620  ster.        if 
-000ed050: 7365 6c66 2e69 735f 6375 7374 6f6d 2069  self.is_custom i
-000ed060: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ed070: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ed080: 6973 5f63 7573 746f 6d27 5d20 3d20 7365  is_custom'] = se
-000ed090: 6c66 2e69 735f 6375 7374 6f6d 0a20 2020  lf.is_custom.   
-000ed0a0: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
-000ed0b0: 7261 6d5f 726f 6c65 2069 7320 6e6f 7420  ram_role is not 
-000ed0c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ed0d0: 2020 7265 7375 6c74 5b27 6973 5f72 616d    result['is_ram
-000ed0e0: 5f72 6f6c 6527 5d20 3d20 7365 6c66 2e69  _role'] = self.i
-000ed0f0: 735f 7261 6d5f 726f 6c65 0a20 2020 2020  s_ram_role.     
-000ed100: 2020 2069 6620 7365 6c66 2e6e 616d 6573     if self.names
-000ed110: 7061 6365 2069 7320 6e6f 7420 4e6f 6e65  pace is not None
-000ed120: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000ed130: 7375 6c74 5b27 6e61 6d65 7370 6163 6527  sult['namespace'
-000ed140: 5d20 3d20 7365 6c66 2e6e 616d 6573 7061  ] = self.namespa
-000ed150: 6365 0a20 2020 2020 2020 2069 6620 7365  ce.        if se
-000ed160: 6c66 2e72 6f6c 655f 6e61 6d65 2069 7320  lf.role_name is 
-000ed170: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ed180: 2020 2020 2020 7265 7375 6c74 5b27 726f        result['ro
-000ed190: 6c65 5f6e 616d 6527 5d20 3d20 7365 6c66  le_name'] = self
-000ed1a0: 2e72 6f6c 655f 6e61 6d65 0a20 2020 2020  .role_name.     
-000ed1b0: 2020 2069 6620 7365 6c66 2e72 6f6c 655f     if self.role_
-000ed1c0: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-000ed1d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000ed1e0: 7375 6c74 5b27 726f 6c65 5f74 7970 6527  sult['role_type'
-000ed1f0: 5d20 3d20 7365 6c66 2e72 6f6c 655f 7479  ] = self.role_ty
-000ed200: 7065 0a20 2020 2020 2020 2072 6574 7572  pe.        retur
-000ed210: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000ed220: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000ed230: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000ed240: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000ed250: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000ed260: 2020 6966 206d 2e67 6574 2827 636c 7573    if m.get('clus
-000ed270: 7465 7227 2920 6973 206e 6f74 204e 6f6e  ter') is not Non
-000ed280: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000ed290: 656c 662e 636c 7573 7465 7220 3d20 6d2e  elf.cluster = m.
-000ed2a0: 6765 7428 2763 6c75 7374 6572 2729 0a20  get('cluster'). 
-000ed2b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000ed2c0: 2769 735f 6375 7374 6f6d 2729 2069 7320  'is_custom') is 
-000ed2d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ed2e0: 2020 2020 2020 7365 6c66 2e69 735f 6375        self.is_cu
-000ed2f0: 7374 6f6d 203d 206d 2e67 6574 2827 6973  stom = m.get('is
-000ed300: 5f63 7573 746f 6d27 290a 2020 2020 2020  _custom').      
-000ed310: 2020 6966 206d 2e67 6574 2827 6973 5f72    if m.get('is_r
-000ed320: 616d 5f72 6f6c 6527 2920 6973 206e 6f74  am_role') is not
-000ed330: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ed340: 2020 2073 656c 662e 6973 5f72 616d 5f72     self.is_ram_r
-000ed350: 6f6c 6520 3d20 6d2e 6765 7428 2769 735f  ole = m.get('is_
-000ed360: 7261 6d5f 726f 6c65 2729 0a20 2020 2020  ram_role').     
-000ed370: 2020 2069 6620 6d2e 6765 7428 276e 616d     if m.get('nam
-000ed380: 6573 7061 6365 2729 2069 7320 6e6f 7420  espace') is not 
-000ed390: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ed3a0: 2020 7365 6c66 2e6e 616d 6573 7061 6365    self.namespace
-000ed3b0: 203d 206d 2e67 6574 2827 6e61 6d65 7370   = m.get('namesp
-000ed3c0: 6163 6527 290a 2020 2020 2020 2020 6966  ace').        if
-000ed3d0: 206d 2e67 6574 2827 726f 6c65 5f6e 616d   m.get('role_nam
-000ed3e0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-000ed3f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000ed400: 662e 726f 6c65 5f6e 616d 6520 3d20 6d2e  f.role_name = m.
-000ed410: 6765 7428 2772 6f6c 655f 6e61 6d65 2729  get('role_name')
-000ed420: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000ed430: 7428 2772 6f6c 655f 7479 7065 2729 2069  t('role_type') i
-000ed440: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ed450: 2020 2020 2020 2020 7365 6c66 2e72 6f6c          self.rol
-000ed460: 655f 7479 7065 203d 206d 2e67 6574 2827  e_type = m.get('
-000ed470: 726f 6c65 5f74 7970 6527 290a 2020 2020  role_type').    
-000ed480: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-000ed490: 0a0a 636c 6173 7320 5570 6461 7465 5573  ..class UpdateUs
-000ed4a0: 6572 5065 726d 6973 7369 6f6e 7352 6571  erPermissionsReq
-000ed4b0: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
-000ed4c0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000ed4d0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000ed4e0: 2020 2020 2020 2020 626f 6479 3a20 4c69          body: Li
-000ed4f0: 7374 5b55 7064 6174 6555 7365 7250 6572  st[UpdateUserPer
-000ed500: 6d69 7373 696f 6e73 5265 7175 6573 7442  missionsRequestB
-000ed510: 6f64 795d 203d 204e 6f6e 652c 0a20 2020  ody] = None,.   
-000ed520: 2020 2020 206d 6f64 653a 2073 7472 203d       mode: str =
-000ed530: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-000ed540: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-000ed550: 3d20 626f 6479 0a20 2020 2020 2020 2073  = body.        s
-000ed560: 656c 662e 6d6f 6465 203d 206d 6f64 650a  elf.mode = mode.
-000ed570: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-000ed580: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000ed590: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-000ed5a0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-000ed5b0: 2069 6e20 7365 6c66 2e62 6f64 793a 0a20   in self.body:. 
-000ed5c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000ed5d0: 6620 6b3a 0a20 2020 2020 2020 2020 2020  f k:.           
-000ed5e0: 2020 2020 2020 2020 206b 2e76 616c 6964           k.valid
-000ed5f0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-000ed600: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-000ed610: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-000ed620: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-000ed630: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+000e6f00: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000e6f10: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+000e6f20: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+000e6f30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000e6f40: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+000e6f50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000e6f60: 7465 6d70 5f6d 6f64 656c 203d 2053 746f  temp_model = Sto
+000e6f70: 7041 6c65 7274 5265 7370 6f6e 7365 426f  pAlertResponseBo
+000e6f80: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+000e6f90: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+000e6fa0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+000e6fb0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+000e6fc0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000e6fd0: 0a0a 636c 6173 7320 5379 6e63 436c 7573  ..class SyncClus
+000e6fe0: 7465 724e 6f64 6550 6f6f 6c52 6573 706f  terNodePoolRespo
+000e6ff0: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+000e7000: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000e7010: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000e7020: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
+000e7030: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+000e7040: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000e7050: 2020 2320 5468 6520 7265 7175 6573 7420    # The request 
+000e7060: 4944 2e0a 2020 2020 2020 2020 7365 6c66  ID..        self
+000e7070: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+000e7080: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
+000e7090: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000e70a0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000e70b0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000e70c0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000e70d0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000e70e0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000e70f0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000e7100: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e7110: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000e7120: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000e7130: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000e7140: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
+000e7150: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e7160: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e7170: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
+000e7180: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
+000e7190: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000e71a0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000e71b0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+000e71c0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000e71d0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000e71e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000e71f0: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+000e7200: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000e7210: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000e7220: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
+000e7230: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+000e7240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000e7250: 7365 6c66 0a0a 0a63 6c61 7373 2053 796e  self...class Syn
+000e7260: 6343 6c75 7374 6572 4e6f 6465 506f 6f6c  cClusterNodePool
+000e7270: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+000e7280: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000e7290: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000e72a0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
+000e72b0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
+000e72c0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+000e72d0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
+000e72e0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+000e72f0: 2020 2020 2062 6f64 793a 2053 796e 6343       body: SyncC
+000e7300: 6c75 7374 6572 4e6f 6465 506f 6f6c 5265  lusterNodePoolRe
+000e7310: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
+000e7320: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000e7330: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+000e7340: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+000e7350: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000e7360: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
+000e7370: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000e7380: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
+000e7390: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000e73a0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+000e73b0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+000e73c0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+000e73d0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+000e73e0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000e73f0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000e7400: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000e7410: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000e7420: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e7430: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000e7440: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000e7450: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000e7460: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+000e7470: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+000e7480: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e7490: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+000e74a0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+000e74b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000e74c0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+000e74d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e74e0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+000e74f0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+000e7500: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+000e7510: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+000e7520: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+000e7530: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000e7540: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+000e7550: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+000e7560: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000e7570: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000e7580: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000e7590: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000e75a0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000e75b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000e75c0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+000e75d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000e75e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000e75f0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+000e7600: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+000e7610: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
+000e7620: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
+000e7630: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e7640: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000e7650: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
+000e7660: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
+000e7670: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+000e7680: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000e7690: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+000e76a0: 5f6d 6f64 656c 203d 2053 796e 6343 6c75  _model = SyncClu
+000e76b0: 7374 6572 4e6f 6465 506f 6f6c 5265 7370  sterNodePoolResp
+000e76c0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+000e76d0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000e76e0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+000e76f0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+000e7700: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000e7710: 2073 656c 660a 0a0a 636c 6173 7320 5461   self...class Ta
+000e7720: 6752 6573 6f75 7263 6573 5265 7175 6573  gResourcesReques
+000e7730: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+000e7740: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000e7750: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000e7760: 2020 2020 2072 6567 696f 6e5f 6964 3a20       region_id: 
+000e7770: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000e7780: 2020 2020 7265 736f 7572 6365 5f69 6473      resource_ids
+000e7790: 3a20 4c69 7374 5b73 7472 5d20 3d20 4e6f  : List[str] = No
+000e77a0: 6e65 2c0a 2020 2020 2020 2020 7265 736f  ne,.        reso
+000e77b0: 7572 6365 5f74 7970 653a 2073 7472 203d  urce_type: str =
+000e77c0: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+000e77d0: 6167 733a 204c 6973 745b 5461 675d 203d  ags: List[Tag] =
+000e77e0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000e77f0: 2020 2020 2020 2320 5468 6520 7265 6769        # The regi
+000e7800: 6f6e 2049 4420 6f66 2074 6865 2072 6573  on ID of the res
+000e7810: 6f75 7263 652e 0a20 2020 2020 2020 2023  ource..        #
+000e7820: 200a 2020 2020 2020 2020 2320 5468 6973   .        # This
+000e7830: 2070 6172 616d 6574 6572 2069 7320 7265   parameter is re
+000e7840: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+000e7850: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+000e7860: 2072 6567 696f 6e5f 6964 0a20 2020 2020   region_id.     
+000e7870: 2020 2023 2054 6865 206c 6973 7420 6f66     # The list of
+000e7880: 2072 6573 6f75 7263 6520 4944 732e 0a20   resource IDs.. 
+000e7890: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+000e78a0: 2020 2320 5468 6973 2070 6172 616d 6574    # This paramet
+000e78b0: 6572 2069 7320 7265 7175 6972 6564 2e0a  er is required..
+000e78c0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+000e78d0: 6f75 7263 655f 6964 7320 3d20 7265 736f  ource_ids = reso
+000e78e0: 7572 6365 5f69 6473 0a20 2020 2020 2020  urce_ids.       
+000e78f0: 2023 2054 6865 2074 7970 6520 6f66 2072   # The type of r
+000e7900: 6573 6f75 7263 6520 7468 6174 2079 6f75  esource that you
+000e7910: 2077 616e 7420 746f 206c 6162 656c 2e20   want to label. 
+000e7920: 5365 7420 7468 6520 7661 6c75 6520 746f  Set the value to
+000e7930: 2060 434c 5553 5445 5260 2e0a 2020 2020   `CLUSTER`..    
+000e7940: 2020 2020 2320 0a20 2020 2020 2020 2023      # .        #
+000e7950: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
+000e7960: 6973 2072 6571 7569 7265 642e 0a20 2020  is required..   
+000e7970: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+000e7980: 6365 5f74 7970 6520 3d20 7265 736f 7572  ce_type = resour
+000e7990: 6365 5f74 7970 650a 2020 2020 2020 2020  ce_type.        
+000e79a0: 2320 5468 6520 6c61 6265 6c73 2074 6861  # The labels tha
+000e79b0: 7420 796f 7520 7761 6e74 2074 6f20 6164  t you want to ad
+000e79c0: 6420 746f 2074 6865 2072 6573 6f75 7263  d to the resourc
+000e79d0: 6573 2069 6e20 6b65 792d 7661 6c75 6520  es in key-value 
+000e79e0: 7061 6972 732e 2059 6f75 2063 616e 2061  pairs. You can a
+000e79f0: 6464 2075 7020 746f 2032 3020 6c61 6265  dd up to 20 labe
+000e7a00: 6c73 2e20 5573 6167 6520 6e6f 7465 733a  ls. Usage notes:
+000e7a10: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
+000e7a20: 2020 2020 2320 2a20 2020 4c61 6265 6c20      # *   Label 
+000e7a30: 7661 6c75 6573 206d 7573 7420 6e6f 7420  values must not 
+000e7a40: 6265 2065 6d70 7479 2073 7472 696e 6773  be empty strings
+000e7a50: 2e20 4120 6c61 6265 6c20 7661 6c75 6520  . A label value 
+000e7a60: 6d75 7374 2062 6520 3120 746f 2031 3238  must be 1 to 128
+000e7a70: 2063 6861 7261 6374 6572 7320 696e 206c   characters in l
+000e7a80: 656e 6774 682e 0a20 2020 2020 2020 2023  ength..        #
+000e7a90: 202a 2020 2054 6865 206c 6162 656c 2076   *   The label v
+000e7aa0: 616c 7565 206d 7573 7420 6e6f 7420 7374  alue must not st
+000e7ab0: 6172 7420 7769 7468 2060 616c 6979 756e  art with `aliyun
+000e7ac0: 6020 6f72 2060 6163 733a 602e 0a20 2020  ` or `acs:`..   
+000e7ad0: 2020 2020 2023 202a 2020 2054 6865 206c       # *   The l
+000e7ae0: 6162 656c 2076 616c 7565 206d 7573 7420  abel value must 
+000e7af0: 6e6f 7420 636f 6e74 6169 6e20 6068 7474  not contain `htt
+000e7b00: 703a 2f2f 6020 6f72 2060 6874 7470 733a  p://` or `https:
+000e7b10: 2f2f 602e 0a20 2020 2020 2020 2023 200a  //`..        # .
+000e7b20: 2020 2020 2020 2020 2320 5468 6973 2070          # This p
+000e7b30: 6172 616d 6574 6572 2069 7320 7265 7175  arameter is requ
+000e7b40: 6972 6564 2e0a 2020 2020 2020 2020 7365  ired..        se
+000e7b50: 6c66 2e74 6167 7320 3d20 7461 6773 0a0a  lf.tags = tags..
+000e7b60: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000e7b70: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000e7b80: 6966 2073 656c 662e 7461 6773 3a0a 2020  if self.tags:.  
+000e7b90: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+000e7ba0: 696e 2073 656c 662e 7461 6773 3a0a 2020  in self.tags:.  
+000e7bb0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000e7bc0: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
+000e7bd0: 2020 2020 2020 2020 6b2e 7661 6c69 6461          k.valida
+000e7be0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+000e7bf0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000e7c00: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000e7c10: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+000e7c20: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000e7c30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e7c40: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000e7c50: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000e7c60: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000e7c70: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
+000e7c80: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+000e7c90: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000e7ca0: 756c 745b 2772 6567 696f 6e5f 6964 275d  ult['region_id']
+000e7cb0: 203d 2073 656c 662e 7265 6769 6f6e 5f69   = self.region_i
+000e7cc0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+000e7cd0: 662e 7265 736f 7572 6365 5f69 6473 2069  f.resource_ids i
+000e7ce0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e7cf0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e7d00: 7265 736f 7572 6365 5f69 6473 275d 203d  resource_ids'] =
+000e7d10: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+000e7d20: 6473 0a20 2020 2020 2020 2069 6620 7365  ds.        if se
+000e7d30: 6c66 2e72 6573 6f75 7263 655f 7479 7065  lf.resource_type
+000e7d40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e7d50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000e7d60: 5b27 7265 736f 7572 6365 5f74 7970 6527  ['resource_type'
+000e7d70: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
+000e7d80: 655f 7479 7065 0a20 2020 2020 2020 2072  e_type.        r
+000e7d90: 6573 756c 745b 2774 6167 7327 5d20 3d20  esult['tags'] = 
+000e7da0: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
+000e7db0: 6c66 2e74 6167 7320 6973 206e 6f74 204e  lf.tags is not N
+000e7dc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e7dd0: 2066 6f72 206b 2069 6e20 7365 6c66 2e74   for k in self.t
+000e7de0: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
+000e7df0: 2020 2020 2072 6573 756c 745b 2774 6167       result['tag
+000e7e00: 7327 5d2e 6170 7065 6e64 286b 2e74 6f5f  s'].append(k.to_
+000e7e10: 6d61 7028 2920 6966 206b 2065 6c73 6520  map() if k else 
+000e7e20: 4e6f 6e65 290a 2020 2020 2020 2020 7265  None).        re
+000e7e30: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000e7e40: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000e7e50: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000e7e60: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000e7e70: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000e7e80: 2020 2020 2069 6620 6d2e 6765 7428 2772       if m.get('r
+000e7e90: 6567 696f 6e5f 6964 2729 2069 7320 6e6f  egion_id') is no
+000e7ea0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e7eb0: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
+000e7ec0: 6964 203d 206d 2e67 6574 2827 7265 6769  id = m.get('regi
+000e7ed0: 6f6e 5f69 6427 290a 2020 2020 2020 2020  on_id').        
+000e7ee0: 6966 206d 2e67 6574 2827 7265 736f 7572  if m.get('resour
+000e7ef0: 6365 5f69 6473 2729 2069 7320 6e6f 7420  ce_ids') is not 
+000e7f00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e7f10: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+000e7f20: 6964 7320 3d20 6d2e 6765 7428 2772 6573  ids = m.get('res
+000e7f30: 6f75 7263 655f 6964 7327 290a 2020 2020  ource_ids').    
+000e7f40: 2020 2020 6966 206d 2e67 6574 2827 7265      if m.get('re
+000e7f50: 736f 7572 6365 5f74 7970 6527 2920 6973  source_type') is
+000e7f60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e7f70: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
+000e7f80: 7572 6365 5f74 7970 6520 3d20 6d2e 6765  urce_type = m.ge
+000e7f90: 7428 2772 6573 6f75 7263 655f 7479 7065  t('resource_type
+000e7fa0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+000e7fb0: 7461 6773 203d 205b 5d0a 2020 2020 2020  tags = [].      
+000e7fc0: 2020 6966 206d 2e67 6574 2827 7461 6773    if m.get('tags
+000e7fd0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000e7fe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000e7ff0: 6b20 696e 206d 2e67 6574 2827 7461 6773  k in m.get('tags
+000e8000: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+000e8010: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+000e8020: 2054 6167 2829 0a20 2020 2020 2020 2020   Tag().         
+000e8030: 2020 2020 2020 2073 656c 662e 7461 6773         self.tags
+000e8040: 2e61 7070 656e 6428 7465 6d70 5f6d 6f64  .append(temp_mod
+000e8050: 656c 2e66 726f 6d5f 6d61 7028 6b29 290a  el.from_map(k)).
+000e8060: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000e8070: 656c 660a 0a0a 636c 6173 7320 5461 6752  elf...class TagR
+000e8080: 6573 6f75 7263 6573 5265 7370 6f6e 7365  esourcesResponse
+000e8090: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
+000e80a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000e80b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000e80c0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+000e80d0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+000e80e0: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
+000e80f0: 2054 6865 2072 6571 7565 7374 2049 442e   The request ID.
+000e8100: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+000e8110: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+000e8120: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
+000e8130: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000e8140: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000e8150: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000e8160: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000e8170: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000e8180: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000e8190: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+000e81a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000e81b0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+000e81c0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+000e81d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000e81e0: 2e72 6571 7565 7374 5f69 6420 6973 206e  .request_id is n
+000e81f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e8200: 2020 2020 2072 6573 756c 745b 2752 6571       result['Req
+000e8210: 7565 7374 4964 275d 203d 2073 656c 662e  uestId'] = self.
+000e8220: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
+000e8230: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+000e8240: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000e8250: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+000e8260: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+000e8270: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000e8280: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000e8290: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+000e82a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e82b0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+000e82c0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+000e82d0: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+000e82e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000e82f0: 660a 0a0a 636c 6173 7320 5461 6752 6573  f...class TagRes
+000e8300: 6f75 7263 6573 5265 7370 6f6e 7365 2854  ourcesResponse(T
+000e8310: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000e8320: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000e8330: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000e8340: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+000e8350: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+000e8360: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+000e8370: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+000e8380: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+000e8390: 2054 6167 5265 736f 7572 6365 7352 6573   TagResourcesRes
+000e83a0: 706f 6e73 6542 6f64 7920 3d20 4e6f 6e65  ponseBody = None
+000e83b0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+000e83c0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000e83d0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+000e83e0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000e83f0: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
+000e8400: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000e8410: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
+000e8420: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+000e8430: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000e8440: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+000e8450: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+000e8460: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+000e8470: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000e8480: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000e8490: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000e84a0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000e84b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e84c0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000e84d0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000e84e0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000e84f0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+000e8500: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+000e8510: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000e8520: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+000e8530: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+000e8540: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000e8550: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+000e8560: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e8570: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+000e8580: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+000e8590: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+000e85a0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000e85b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e85c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000e85d0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+000e85e0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+000e85f0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000e8600: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000e8610: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+000e8620: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000e8630: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000e8640: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000e8650: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000e8660: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e8670: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+000e8680: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+000e8690: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000e86a0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+000e86b0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+000e86c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e86d0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+000e86e0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+000e86f0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+000e8700: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+000e8710: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000e8720: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+000e8730: 6d6f 6465 6c20 3d20 5461 6752 6573 6f75  model = TagResou
+000e8740: 7263 6573 5265 7370 6f6e 7365 426f 6479  rcesResponseBody
+000e8750: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+000e8760: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+000e8770: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+000e8780: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+000e8790: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+000e87a0: 636c 6173 7320 556e 496e 7374 616c 6c43  class UnInstallC
+000e87b0: 6c75 7374 6572 4164 646f 6e73 5265 7175  lusterAddonsRequ
+000e87c0: 6573 7441 6464 6f6e 7328 5465 614d 6f64  estAddons(TeaMod
+000e87d0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000e87e0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000e87f0: 656c 662c 0a20 2020 2020 2020 2063 6c65  elf,.        cle
+000e8800: 616e 7570 5f63 6c6f 7564 5f72 6573 6f75  anup_cloud_resou
+000e8810: 7263 6573 3a20 626f 6f6c 203d 204e 6f6e  rces: bool = Non
+000e8820: 652c 0a20 2020 2020 2020 206e 616d 653a  e,.        name:
+000e8830: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000e8840: 2029 3a0a 2020 2020 2020 2020 2320 5768   ):.        # Wh
+000e8850: 6574 6865 7220 746f 2063 6c65 616e 2075  ether to clean u
+000e8860: 7020 636c 6f75 6420 7265 736f 7572 6365  p cloud resource
+000e8870: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+000e8880: 636c 6561 6e75 705f 636c 6f75 645f 7265  cleanup_cloud_re
+000e8890: 736f 7572 6365 7320 3d20 636c 6561 6e75  sources = cleanu
+000e88a0: 705f 636c 6f75 645f 7265 736f 7572 6365  p_cloud_resource
+000e88b0: 730a 2020 2020 2020 2020 2320 5468 6520  s.        # The 
+000e88c0: 636f 6d70 6f6e 656e 7420 6e61 6d65 2e0a  component name..
+000e88d0: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
+000e88e0: 6520 3d20 6e61 6d65 0a0a 2020 2020 6465  e = name..    de
+000e88f0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000e8900: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000e8910: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000e8920: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000e8930: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000e8940: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000e8950: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000e8960: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e8970: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000e8980: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000e8990: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000e89a0: 656c 662e 636c 6561 6e75 705f 636c 6f75  elf.cleanup_clou
+000e89b0: 645f 7265 736f 7572 6365 7320 6973 206e  d_resources is n
+000e89c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e89d0: 2020 2020 2072 6573 756c 745b 2763 6c65       result['cle
+000e89e0: 616e 7570 5f63 6c6f 7564 5f72 6573 6f75  anup_cloud_resou
+000e89f0: 7263 6573 275d 203d 2073 656c 662e 636c  rces'] = self.cl
+000e8a00: 6561 6e75 705f 636c 6f75 645f 7265 736f  eanup_cloud_reso
+000e8a10: 7572 6365 730a 2020 2020 2020 2020 6966  urces.        if
+000e8a20: 2073 656c 662e 6e61 6d65 2069 7320 6e6f   self.name is no
+000e8a30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000e8a40: 2020 2020 7265 7375 6c74 5b27 6e61 6d65      result['name
+000e8a50: 275d 203d 2073 656c 662e 6e61 6d65 0a20  '] = self.name. 
+000e8a60: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000e8a70: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000e8a80: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000e8a90: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000e8aa0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000e8ab0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000e8ac0: 206d 2e67 6574 2827 636c 6561 6e75 705f   m.get('cleanup_
+000e8ad0: 636c 6f75 645f 7265 736f 7572 6365 7327  cloud_resources'
+000e8ae0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000e8af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000e8b00: 636c 6561 6e75 705f 636c 6f75 645f 7265  cleanup_cloud_re
+000e8b10: 736f 7572 6365 7320 3d20 6d2e 6765 7428  sources = m.get(
+000e8b20: 2763 6c65 616e 7570 5f63 6c6f 7564 5f72  'cleanup_cloud_r
+000e8b30: 6573 6f75 7263 6573 2729 0a20 2020 2020  esources').     
+000e8b40: 2020 2069 6620 6d2e 6765 7428 276e 616d     if m.get('nam
+000e8b50: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+000e8b60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000e8b70: 662e 6e61 6d65 203d 206d 2e67 6574 2827  f.name = m.get('
+000e8b80: 6e61 6d65 2729 0a20 2020 2020 2020 2072  name').        r
+000e8b90: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000e8ba0: 7373 2055 6e49 6e73 7461 6c6c 436c 7573  ss UnInstallClus
+000e8bb0: 7465 7241 6464 6f6e 7352 6571 7565 7374  terAddonsRequest
+000e8bc0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000e8bd0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000e8be0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000e8bf0: 2020 2020 6164 646f 6e73 3a20 4c69 7374      addons: List
+000e8c00: 5b55 6e49 6e73 7461 6c6c 436c 7573 7465  [UnInstallCluste
+000e8c10: 7241 6464 6f6e 7352 6571 7565 7374 4164  rAddonsRequestAd
+000e8c20: 646f 6e73 5d20 3d20 4e6f 6e65 2c0a 2020  dons] = None,.  
+000e8c30: 2020 293a 0a20 2020 2020 2020 2023 2054    ):.        # T
+000e8c40: 6865 206c 6973 7420 6f66 2063 6f6d 706f  he list of compo
+000e8c50: 6e65 6e74 7320 7468 6174 2079 6f75 2077  nents that you w
+000e8c60: 616e 7420 746f 2075 6e69 6e73 7461 6c6c  ant to uninstall
+000e8c70: 2e20 5468 6520 6c69 7374 2069 7320 616e  . The list is an
+000e8c80: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+000e8c90: 7365 6c66 2e61 6464 6f6e 7320 3d20 6164  self.addons = ad
+000e8ca0: 646f 6e73 0a0a 2020 2020 6465 6620 7661  dons..    def va
+000e8cb0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000e8cc0: 2020 2020 2020 6966 2073 656c 662e 6164        if self.ad
+000e8cd0: 646f 6e73 3a0a 2020 2020 2020 2020 2020  dons:.          
+000e8ce0: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
+000e8cf0: 6164 646f 6e73 3a0a 2020 2020 2020 2020  addons:.        
+000e8d00: 2020 2020 2020 2020 6966 206b 3a0a 2020          if k:.  
+000e8d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000e8d20: 2020 6b2e 7661 6c69 6461 7465 2829 0a0a    k.validate()..
+000e8d30: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000e8d40: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000e8d50: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000e8d60: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000e8d70: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000e8d80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e8d90: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000e8da0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000e8db0: 7428 290a 2020 2020 2020 2020 7265 7375  t().        resu
+000e8dc0: 6c74 5b27 6164 646f 6e73 275d 203d 205b  lt['addons'] = [
+000e8dd0: 5d0a 2020 2020 2020 2020 6966 2073 656c  ].        if sel
+000e8de0: 662e 6164 646f 6e73 2069 7320 6e6f 7420  f.addons is not 
+000e8df0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000e8e00: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
+000e8e10: 6164 646f 6e73 3a0a 2020 2020 2020 2020  addons:.        
+000e8e20: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000e8e30: 6164 646f 6e73 275d 2e61 7070 656e 6428  addons'].append(
+000e8e40: 6b2e 746f 5f6d 6170 2829 2069 6620 6b20  k.to_map() if k 
+000e8e50: 656c 7365 204e 6f6e 6529 0a20 2020 2020  else None).     
+000e8e60: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+000e8e70: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000e8e80: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+000e8e90: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+000e8ea0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000e8eb0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000e8ec0: 6464 6f6e 7320 3d20 5b5d 0a20 2020 2020  ddons = [].     
+000e8ed0: 2020 2069 6620 6d2e 6765 7428 2761 6464     if m.get('add
+000e8ee0: 6f6e 7327 2920 6973 206e 6f74 204e 6f6e  ons') is not Non
+000e8ef0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+000e8f00: 6f72 206b 2069 6e20 6d2e 6765 7428 2761  or k in m.get('a
+000e8f10: 6464 6f6e 7327 293a 0a20 2020 2020 2020  ddons'):.       
+000e8f20: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+000e8f30: 6465 6c20 3d20 556e 496e 7374 616c 6c43  del = UnInstallC
+000e8f40: 6c75 7374 6572 4164 646f 6e73 5265 7175  lusterAddonsRequ
+000e8f50: 6573 7441 6464 6f6e 7328 290a 2020 2020  estAddons().    
+000e8f60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000e8f70: 2e61 6464 6f6e 732e 6170 7065 6e64 2874  .addons.append(t
+000e8f80: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+000e8f90: 6170 286b 2929 0a20 2020 2020 2020 2072  ap(k)).        r
+000e8fa0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000e8fb0: 7373 2055 6e49 6e73 7461 6c6c 436c 7573  ss UnInstallClus
+000e8fc0: 7465 7241 6464 6f6e 7352 6573 706f 6e73  terAddonsRespons
+000e8fd0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+000e8fe0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000e8ff0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000e9000: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+000e9010: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+000e9020: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+000e9030: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+000e9040: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+000e9050: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+000e9060: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+000e9070: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+000e9080: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+000e9090: 6465 0a0a 2020 2020 6465 6620 7661 6c69  de..    def vali
+000e90a0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000e90b0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000e90c0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000e90d0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000e90e0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000e90f0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000e9100: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e9110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000e9120: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000e9130: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000e9140: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+000e9150: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+000e9160: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000e9170: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+000e9180: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+000e9190: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000e91a0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+000e91b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e91c0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+000e91d0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+000e91e0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+000e91f0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000e9200: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000e9210: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+000e9220: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+000e9230: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+000e9240: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+000e9250: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+000e9260: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000e9270: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000e9280: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+000e9290: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+000e92a0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+000e92b0: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+000e92c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e92d0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000e92e0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+000e92f0: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+000e9300: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000e9310: 6173 7320 556e 7461 6752 6573 6f75 7263  ass UntagResourc
+000e9320: 6573 5265 7175 6573 7428 5465 614d 6f64  esRequest(TeaMod
+000e9330: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000e9340: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000e9350: 656c 662c 0a20 2020 2020 2020 2061 6c6c  elf,.        all
+000e9360: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+000e9370: 2020 2020 2020 2072 6567 696f 6e5f 6964         region_id
+000e9380: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000e9390: 2020 2020 2020 7265 736f 7572 6365 5f69        resource_i
+000e93a0: 6473 3a20 4c69 7374 5b73 7472 5d20 3d20  ds: List[str] = 
+000e93b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
+000e93c0: 736f 7572 6365 5f74 7970 653a 2073 7472  source_type: str
+000e93d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000e93e0: 2074 6167 5f6b 6579 733a 204c 6973 745b   tag_keys: List[
+000e93f0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000e9400: 2029 3a0a 2020 2020 2020 2020 2320 5370   ):.        # Sp
+000e9410: 6563 6966 6965 7320 7768 6574 6865 7220  ecifies whether 
+000e9420: 746f 2072 656d 6f76 6520 616c 6c20 6375  to remove all cu
+000e9430: 7374 6f6d 206c 6162 656c 732e 2054 6869  stom labels. Thi
+000e9440: 7320 7061 7261 6d65 7465 7220 7461 6b65  s parameter take
+000e9450: 7320 6566 6665 6374 206f 6e6c 7920 7768  s effect only wh
+000e9460: 656e 2060 7461 675f 6b65 7973 6020 6973  en `tag_keys` is
+000e9470: 206c 6566 7420 656d 7074 792e 2056 616c   left empty. Val
+000e9480: 6964 2076 616c 7565 733a 0a20 2020 2020  id values:.     
+000e9490: 2020 2023 200a 2020 2020 2020 2020 2320     # .        # 
+000e94a0: 2a20 2020 6074 7275 6560 3a20 5265 6d6f  *   `true`: Remo
+000e94b0: 7665 2061 6c6c 2063 7573 746f 6d20 6c61  ve all custom la
+000e94c0: 6265 6c73 2e0a 2020 2020 2020 2020 2320  bels..        # 
+000e94d0: 2a20 2020 6066 616c 7365 603a 2044 6f20  *   `false`: Do 
+000e94e0: 6e6f 7420 7265 6d6f 7665 2061 6c6c 2063  not remove all c
+000e94f0: 7573 746f 6d20 6c61 6265 6c73 2e0a 2020  ustom labels..  
+000e9500: 2020 2020 2020 7365 6c66 2e61 6c6c 203d        self.all =
+000e9510: 2061 6c6c 0a20 2020 2020 2020 2023 2054   all.        # T
+000e9520: 6865 2072 6567 696f 6e20 4944 206f 6620  he region ID of 
+000e9530: 7468 6520 7265 736f 7572 6365 732e 0a20  the resources.. 
+000e9540: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+000e9550: 2020 2320 5468 6973 2070 6172 616d 6574    # This paramet
+000e9560: 6572 2069 7320 7265 7175 6972 6564 2e0a  er is required..
+000e9570: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+000e9580: 696f 6e5f 6964 203d 2072 6567 696f 6e5f  ion_id = region_
+000e9590: 6964 0a20 2020 2020 2020 2023 2054 6865  id.        # The
+000e95a0: 206c 6973 7420 6f66 2072 6573 6f75 7263   list of resourc
+000e95b0: 6520 4944 732e 0a20 2020 2020 2020 2023  e IDs..        #
+000e95c0: 200a 2020 2020 2020 2020 2320 5468 6973   .        # This
+000e95d0: 2070 6172 616d 6574 6572 2069 7320 7265   parameter is re
+000e95e0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+000e95f0: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
+000e9600: 7320 3d20 7265 736f 7572 6365 5f69 6473  s = resource_ids
+000e9610: 0a20 2020 2020 2020 2023 2054 6865 2074  .        # The t
+000e9620: 7970 6520 6f66 2072 6573 6f75 7263 652e  ype of resource.
+000e9630: 2053 6574 2074 6865 2076 616c 7565 2074   Set the value t
+000e9640: 6f20 6043 4c55 5354 4552 602e 0a20 2020  o `CLUSTER`..   
+000e9650: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+000e9660: 2320 5468 6973 2070 6172 616d 6574 6572  # This parameter
+000e9670: 2069 7320 7265 7175 6972 6564 2e0a 2020   is required..  
+000e9680: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+000e9690: 7263 655f 7479 7065 203d 2072 6573 6f75  rce_type = resou
+000e96a0: 7263 655f 7479 7065 0a20 2020 2020 2020  rce_type.       
+000e96b0: 2023 2054 6865 206c 6973 7420 6f66 206b   # The list of k
+000e96c0: 6579 7320 6f66 2074 6865 206c 6162 656c  eys of the label
+000e96d0: 7320 7468 6174 2079 6f75 2077 616e 7420  s that you want 
+000e96e0: 746f 2072 656d 6f76 652e 0a20 2020 2020  to remove..     
+000e96f0: 2020 2023 200a 2020 2020 2020 2020 2320     # .        # 
+000e9700: 5468 6973 2070 6172 616d 6574 6572 2069  This parameter i
+000e9710: 7320 7265 7175 6972 6564 2e0a 2020 2020  s required..    
+000e9720: 2020 2020 7365 6c66 2e74 6167 5f6b 6579      self.tag_key
+000e9730: 7320 3d20 7461 675f 6b65 7973 0a0a 2020  s = tag_keys..  
+000e9740: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000e9750: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+000e9760: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+000e9770: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+000e9780: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+000e9790: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000e97a0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+000e97b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000e97c0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000e97d0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000e97e0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000e97f0: 6966 2073 656c 662e 616c 6c20 6973 206e  if self.all is n
+000e9800: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e9810: 2020 2020 2072 6573 756c 745b 2761 6c6c       result['all
+000e9820: 275d 203d 2073 656c 662e 616c 6c0a 2020  '] = self.all.  
+000e9830: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+000e9840: 6769 6f6e 5f69 6420 6973 206e 6f74 204e  gion_id is not N
+000e9850: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000e9860: 2072 6573 756c 745b 2772 6567 696f 6e5f   result['region_
+000e9870: 6964 275d 203d 2073 656c 662e 7265 6769  id'] = self.regi
+000e9880: 6f6e 5f69 640a 2020 2020 2020 2020 6966  on_id.        if
+000e9890: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+000e98a0: 6473 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ds is not None:.
+000e98b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000e98c0: 6c74 5b27 7265 736f 7572 6365 5f69 6473  lt['resource_ids
+000e98d0: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+000e98e0: 6365 5f69 6473 0a20 2020 2020 2020 2069  ce_ids.        i
+000e98f0: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
+000e9900: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+000e9910: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000e9920: 7375 6c74 5b27 7265 736f 7572 6365 5f74  sult['resource_t
+000e9930: 7970 6527 5d20 3d20 7365 6c66 2e72 6573  ype'] = self.res
+000e9940: 6f75 7263 655f 7479 7065 0a20 2020 2020  ource_type.     
+000e9950: 2020 2069 6620 7365 6c66 2e74 6167 5f6b     if self.tag_k
+000e9960: 6579 7320 6973 206e 6f74 204e 6f6e 653a  eys is not None:
+000e9970: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000e9980: 756c 745b 2774 6167 5f6b 6579 7327 5d20  ult['tag_keys'] 
+000e9990: 3d20 7365 6c66 2e74 6167 5f6b 6579 730a  = self.tag_keys.
+000e99a0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000e99b0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+000e99c0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+000e99d0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+000e99e0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+000e99f0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000e9a00: 6620 6d2e 6765 7428 2761 6c6c 2729 2069  f m.get('all') i
+000e9a10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000e9a20: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+000e9a30: 203d 206d 2e67 6574 2827 616c 6c27 290a   = m.get('all').
+000e9a40: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000e9a50: 2827 7265 6769 6f6e 5f69 6427 2920 6973  ('region_id') is
+000e9a60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000e9a70: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+000e9a80: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2772  on_id = m.get('r
+000e9a90: 6567 696f 6e5f 6964 2729 0a20 2020 2020  egion_id').     
+000e9aa0: 2020 2069 6620 6d2e 6765 7428 2772 6573     if m.get('res
+000e9ab0: 6f75 7263 655f 6964 7327 2920 6973 206e  ource_ids') is n
+000e9ac0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000e9ad0: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+000e9ae0: 6365 5f69 6473 203d 206d 2e67 6574 2827  ce_ids = m.get('
+000e9af0: 7265 736f 7572 6365 5f69 6473 2729 0a20  resource_ids'). 
+000e9b00: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000e9b10: 2772 6573 6f75 7263 655f 7479 7065 2729  'resource_type')
+000e9b20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000e9b30: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000e9b40: 6573 6f75 7263 655f 7479 7065 203d 206d  esource_type = m
+000e9b50: 2e67 6574 2827 7265 736f 7572 6365 5f74  .get('resource_t
+000e9b60: 7970 6527 290a 2020 2020 2020 2020 6966  ype').        if
+000e9b70: 206d 2e67 6574 2827 7461 675f 6b65 7973   m.get('tag_keys
+000e9b80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000e9b90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000e9ba0: 2e74 6167 5f6b 6579 7320 3d20 6d2e 6765  .tag_keys = m.ge
+000e9bb0: 7428 2774 6167 5f6b 6579 7327 290a 2020  t('tag_keys').  
+000e9bc0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000e9bd0: 660a 0a0a 636c 6173 7320 556e 7461 6752  f...class UntagR
+000e9be0: 6573 6f75 7263 6573 5368 7269 6e6b 5265  esourcesShrinkRe
+000e9bf0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+000e9c00: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000e9c10: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+000e9c20: 0a20 2020 2020 2020 2061 6c6c 3a20 626f  .        all: bo
+000e9c30: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+000e9c40: 2020 2072 6567 696f 6e5f 6964 3a20 7374     region_id: st
+000e9c50: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000e9c60: 2020 7265 736f 7572 6365 5f69 6473 5f73    resource_ids_s
+000e9c70: 6872 696e 6b3a 2073 7472 203d 204e 6f6e  hrink: str = Non
+000e9c80: 652c 0a20 2020 2020 2020 2072 6573 6f75  e,.        resou
+000e9c90: 7263 655f 7479 7065 3a20 7374 7220 3d20  rce_type: str = 
+000e9ca0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7461  None,.        ta
+000e9cb0: 675f 6b65 7973 5f73 6872 696e 6b3a 2073  g_keys_shrink: s
+000e9cc0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+000e9cd0: 3a0a 2020 2020 2020 2020 2320 5370 6563  :.        # Spec
+000e9ce0: 6966 6965 7320 7768 6574 6865 7220 746f  ifies whether to
+000e9cf0: 2072 656d 6f76 6520 616c 6c20 6375 7374   remove all cust
+000e9d00: 6f6d 206c 6162 656c 732e 2054 6869 7320  om labels. This 
+000e9d10: 7061 7261 6d65 7465 7220 7461 6b65 7320  parameter takes 
+000e9d20: 6566 6665 6374 206f 6e6c 7920 7768 656e  effect only when
+000e9d30: 2060 7461 675f 6b65 7973 6020 6973 206c   `tag_keys` is l
+000e9d40: 6566 7420 656d 7074 792e 2056 616c 6964  eft empty. Valid
+000e9d50: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
+000e9d60: 2023 200a 2020 2020 2020 2020 2320 2a20   # .        # * 
+000e9d70: 2020 6074 7275 6560 3a20 5265 6d6f 7665    `true`: Remove
+000e9d80: 2061 6c6c 2063 7573 746f 6d20 6c61 6265   all custom labe
+000e9d90: 6c73 2e0a 2020 2020 2020 2020 2320 2a20  ls..        # * 
+000e9da0: 2020 6066 616c 7365 603a 2044 6f20 6e6f    `false`: Do no
+000e9db0: 7420 7265 6d6f 7665 2061 6c6c 2063 7573  t remove all cus
+000e9dc0: 746f 6d20 6c61 6265 6c73 2e0a 2020 2020  tom labels..    
+000e9dd0: 2020 2020 7365 6c66 2e61 6c6c 203d 2061      self.all = a
+000e9de0: 6c6c 0a20 2020 2020 2020 2023 2054 6865  ll.        # The
+000e9df0: 2072 6567 696f 6e20 4944 206f 6620 7468   region ID of th
+000e9e00: 6520 7265 736f 7572 6365 732e 0a20 2020  e resources..   
+000e9e10: 2020 2020 2023 200a 2020 2020 2020 2020       # .        
+000e9e20: 2320 5468 6973 2070 6172 616d 6574 6572  # This parameter
+000e9e30: 2069 7320 7265 7175 6972 6564 2e0a 2020   is required..  
+000e9e40: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+000e9e50: 6e5f 6964 203d 2072 6567 696f 6e5f 6964  n_id = region_id
+000e9e60: 0a20 2020 2020 2020 2023 2054 6865 206c  .        # The l
+000e9e70: 6973 7420 6f66 2072 6573 6f75 7263 6520  ist of resource 
+000e9e80: 4944 732e 0a20 2020 2020 2020 2023 200a  IDs..        # .
+000e9e90: 2020 2020 2020 2020 2320 5468 6973 2070          # This p
+000e9ea0: 6172 616d 6574 6572 2069 7320 7265 7175  arameter is requ
+000e9eb0: 6972 6564 2e0a 2020 2020 2020 2020 7365  ired..        se
+000e9ec0: 6c66 2e72 6573 6f75 7263 655f 6964 735f  lf.resource_ids_
+000e9ed0: 7368 7269 6e6b 203d 2072 6573 6f75 7263  shrink = resourc
+000e9ee0: 655f 6964 735f 7368 7269 6e6b 0a20 2020  e_ids_shrink.   
+000e9ef0: 2020 2020 2023 2054 6865 2074 7970 6520       # The type 
+000e9f00: 6f66 2072 6573 6f75 7263 652e 2053 6574  of resource. Set
+000e9f10: 2074 6865 2076 616c 7565 2074 6f20 6043   the value to `C
+000e9f20: 4c55 5354 4552 602e 0a20 2020 2020 2020  LUSTER`..       
+000e9f30: 2023 200a 2020 2020 2020 2020 2320 5468   # .        # Th
+000e9f40: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
+000e9f50: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
+000e9f60: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+000e9f70: 7479 7065 203d 2072 6573 6f75 7263 655f  type = resource_
+000e9f80: 7479 7065 0a20 2020 2020 2020 2023 2054  type.        # T
+000e9f90: 6865 206c 6973 7420 6f66 206b 6579 7320  he list of keys 
+000e9fa0: 6f66 2074 6865 206c 6162 656c 7320 7468  of the labels th
+000e9fb0: 6174 2079 6f75 2077 616e 7420 746f 2072  at you want to r
+000e9fc0: 656d 6f76 652e 0a20 2020 2020 2020 2023  emove..        #
+000e9fd0: 200a 2020 2020 2020 2020 2320 5468 6973   .        # This
+000e9fe0: 2070 6172 616d 6574 6572 2069 7320 7265   parameter is re
+000e9ff0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
+000ea000: 7365 6c66 2e74 6167 5f6b 6579 735f 7368  self.tag_keys_sh
+000ea010: 7269 6e6b 203d 2074 6167 5f6b 6579 735f  rink = tag_keys_
+000ea020: 7368 7269 6e6b 0a0a 2020 2020 6465 6620  shrink..    def 
+000ea030: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000ea040: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000ea050: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000ea060: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000ea070: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000ea080: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000ea090: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000ea0a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000ea0b0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000ea0c0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000ea0d0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000ea0e0: 662e 616c 6c20 6973 206e 6f74 204e 6f6e  f.all is not Non
+000ea0f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000ea100: 6573 756c 745b 2761 6c6c 275d 203d 2073  esult['all'] = s
+000ea110: 656c 662e 616c 6c0a 2020 2020 2020 2020  elf.all.        
+000ea120: 6966 2073 656c 662e 7265 6769 6f6e 5f69  if self.region_i
+000ea130: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+000ea140: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000ea150: 745b 2772 6567 696f 6e5f 6964 275d 203d  t['region_id'] =
+000ea160: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
+000ea170: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000ea180: 7265 736f 7572 6365 5f69 6473 5f73 6872  resource_ids_shr
+000ea190: 696e 6b20 6973 206e 6f74 204e 6f6e 653a  ink is not None:
+000ea1a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000ea1b0: 756c 745b 2772 6573 6f75 7263 655f 6964  ult['resource_id
+000ea1c0: 7327 5d20 3d20 7365 6c66 2e72 6573 6f75  s'] = self.resou
+000ea1d0: 7263 655f 6964 735f 7368 7269 6e6b 0a20  rce_ids_shrink. 
+000ea1e0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+000ea1f0: 6573 6f75 7263 655f 7479 7065 2069 7320  esource_type is 
+000ea200: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000ea210: 2020 2020 2020 7265 7375 6c74 5b27 7265        result['re
+000ea220: 736f 7572 6365 5f74 7970 6527 5d20 3d20  source_type'] = 
+000ea230: 7365 6c66 2e72 6573 6f75 7263 655f 7479  self.resource_ty
+000ea240: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
+000ea250: 6c66 2e74 6167 5f6b 6579 735f 7368 7269  lf.tag_keys_shri
+000ea260: 6e6b 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nk is not None:.
+000ea270: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000ea280: 6c74 5b27 7461 675f 6b65 7973 275d 203d  lt['tag_keys'] =
+000ea290: 2073 656c 662e 7461 675f 6b65 7973 5f73   self.tag_keys_s
+000ea2a0: 6872 696e 6b0a 2020 2020 2020 2020 7265  hrink.        re
+000ea2b0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000ea2c0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000ea2d0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000ea2e0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000ea2f0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000ea300: 2020 2020 2069 6620 6d2e 6765 7428 2761       if m.get('a
+000ea310: 6c6c 2729 2069 7320 6e6f 7420 4e6f 6e65  ll') is not None
+000ea320: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000ea330: 6c66 2e61 6c6c 203d 206d 2e67 6574 2827  lf.all = m.get('
+000ea340: 616c 6c27 290a 2020 2020 2020 2020 6966  all').        if
+000ea350: 206d 2e67 6574 2827 7265 6769 6f6e 5f69   m.get('region_i
+000ea360: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+000ea370: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000ea380: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
+000ea390: 6765 7428 2772 6567 696f 6e5f 6964 2729  get('region_id')
+000ea3a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000ea3b0: 7428 2772 6573 6f75 7263 655f 6964 7327  t('resource_ids'
+000ea3c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000ea3d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000ea3e0: 7265 736f 7572 6365 5f69 6473 5f73 6872  resource_ids_shr
+000ea3f0: 696e 6b20 3d20 6d2e 6765 7428 2772 6573  ink = m.get('res
+000ea400: 6f75 7263 655f 6964 7327 290a 2020 2020  ource_ids').    
+000ea410: 2020 2020 6966 206d 2e67 6574 2827 7265      if m.get('re
+000ea420: 736f 7572 6365 5f74 7970 6527 2920 6973  source_type') is
+000ea430: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000ea440: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
+000ea450: 7572 6365 5f74 7970 6520 3d20 6d2e 6765  urce_type = m.ge
+000ea460: 7428 2772 6573 6f75 7263 655f 7479 7065  t('resource_type
+000ea470: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000ea480: 6765 7428 2774 6167 5f6b 6579 7327 2920  get('tag_keys') 
+000ea490: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000ea4a0: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
+000ea4b0: 675f 6b65 7973 5f73 6872 696e 6b20 3d20  g_keys_shrink = 
+000ea4c0: 6d2e 6765 7428 2774 6167 5f6b 6579 7327  m.get('tag_keys'
+000ea4d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000ea4e0: 2073 656c 660a 0a0a 636c 6173 7320 556e   self...class Un
+000ea4f0: 7461 6752 6573 6f75 7263 6573 5265 7370  tagResourcesResp
+000ea500: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
+000ea510: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000ea520: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000ea530: 6c66 2c0a 2020 2020 2020 2020 7265 7175  lf,.        requ
+000ea540: 6573 745f 6964 3a20 7374 7220 3d20 4e6f  est_id: str = No
+000ea550: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000ea560: 2020 2023 2054 6865 2072 6571 7565 7374     # The request
+000ea570: 2049 442e 0a20 2020 2020 2020 2073 656c   ID..        sel
+000ea580: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+000ea590: 6571 7565 7374 5f69 640a 0a20 2020 2064  equest_id..    d
+000ea5a0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+000ea5b0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+000ea5c0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000ea5d0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000ea5e0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000ea5f0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000ea600: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000ea610: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ea620: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000ea630: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000ea640: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000ea650: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+000ea660: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000ea670: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000ea680: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+000ea690: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+000ea6a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000ea6b0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000ea6c0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000ea6d0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000ea6e0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000ea6f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000ea700: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+000ea710: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+000ea720: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000ea730: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
+000ea740: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+000ea750: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000ea760: 2073 656c 660a 0a0a 636c 6173 7320 556e   self...class Un
+000ea770: 7461 6752 6573 6f75 7263 6573 5265 7370  tagResourcesResp
+000ea780: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+000ea790: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000ea7a0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000ea7b0: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+000ea7c0: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
+000ea7d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000ea7e0: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
+000ea7f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000ea800: 2062 6f64 793a 2055 6e74 6167 5265 736f   body: UntagReso
+000ea810: 7572 6365 7352 6573 706f 6e73 6542 6f64  urcesResponseBod
+000ea820: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+000ea830: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000ea840: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+000ea850: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000ea860: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+000ea870: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+000ea880: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+000ea890: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000ea8a0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000ea8b0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+000ea8c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000ea8d0: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+000ea8e0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000ea8f0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000ea900: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000ea910: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000ea920: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000ea930: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ea940: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000ea950: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000ea960: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000ea970: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+000ea980: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000ea990: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+000ea9a0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+000ea9b0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+000ea9c0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+000ea9d0: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+000ea9e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000ea9f0: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+000eaa00: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+000eaa10: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+000eaa20: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+000eaa30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000eaa40: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+000eaa50: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+000eaa60: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+000eaa70: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000eaa80: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000eaa90: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000eaaa0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000eaab0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000eaac0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+000eaad0: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+000eaae0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000eaaf0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+000eab00: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+000eab10: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000eab20: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000eab30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000eab40: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000eab50: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+000eab60: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000eab70: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000eab80: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+000eab90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000eaba0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+000eabb0: 556e 7461 6752 6573 6f75 7263 6573 5265  UntagResourcesRe
+000eabc0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
+000eabd0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000eabe0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+000eabf0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+000eac00: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+000eac10: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000eac20: 5570 6461 7465 436f 6e74 6163 7447 726f  UpdateContactGro
+000eac30: 7570 466f 7241 6c65 7274 5265 7370 6f6e  upForAlertRespon
+000eac40: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+000eac50: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000eac60: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000eac70: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+000eac80: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+000eac90: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+000eaca0: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+000eacb0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000eacc0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+000eacd0: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+000eace0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000eacf0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+000ead00: 6f64 650a 0a20 2020 2064 6566 2076 616c  ode..    def val
+000ead10: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000ead20: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000ead30: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+000ead40: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000ead50: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+000ead60: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+000ead70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000ead80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000ead90: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+000eada0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+000eadb0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+000eadc0: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+000eadd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000eade0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+000eadf0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+000eae00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000eae10: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+000eae20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000eae30: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+000eae40: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+000eae50: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+000eae60: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000eae70: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000eae80: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+000eae90: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000eaea0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000eaeb0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000eaec0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000eaed0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000eaee0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+000eaef0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+000eaf00: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000eaf10: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+000eaf20: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+000eaf30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000eaf40: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+000eaf50: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+000eaf60: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+000eaf70: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+000eaf80: 6c61 7373 2055 7064 6174 6543 6f6e 7472  lass UpdateContr
+000eaf90: 6f6c 506c 616e 654c 6f67 5265 7175 6573  olPlaneLogReques
+000eafa0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+000eafb0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000eafc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000eafd0: 2020 2020 2061 6c69 7569 643a 2073 7472       aliuid: str
+000eafe0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000eaff0: 2063 6f6d 706f 6e65 6e74 733a 204c 6973   components: Lis
+000eb000: 745b 7374 725d 203d 204e 6f6e 652c 0a20  t[str] = None,. 
+000eb010: 2020 2020 2020 206c 6f67 5f70 726f 6a65         log_proje
+000eb020: 6374 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ct: str = None,.
+000eb030: 2020 2020 2020 2020 6c6f 675f 7474 6c3a          log_ttl:
+000eb040: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000eb050: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
+000eb060: 6520 4944 206f 6620 7468 6520 416c 6962  e ID of the Alib
+000eb070: 6162 6120 436c 6f75 6420 6163 636f 756e  aba Cloud accoun
+000eb080: 742e 0a20 2020 2020 2020 2073 656c 662e  t..        self.
+000eb090: 616c 6975 6964 203d 2061 6c69 7569 640a  aliuid = aliuid.
+000eb0a0: 2020 2020 2020 2020 2320 5468 6520 636f          # The co
+000eb0b0: 6e74 726f 6c20 706c 616e 6520 636f 6d70  ntrol plane comp
+000eb0c0: 6f6e 656e 7473 2066 6f72 2077 6869 6368  onents for which
+000eb0d0: 2079 6f75 2077 616e 7420 746f 2065 6e61   you want to ena
+000eb0e0: 626c 6520 6c6f 6720 636f 6c6c 6563 7469  ble log collecti
+000eb0f0: 6f6e 2e0a 2020 2020 2020 2020 7365 6c66  on..        self
+000eb100: 2e63 6f6d 706f 6e65 6e74 7320 3d20 636f  .components = co
+000eb110: 6d70 6f6e 656e 7473 0a20 2020 2020 2020  mponents.       
+000eb120: 2023 2054 6865 206e 616d 6520 6f66 2074   # The name of t
+000eb130: 6865 2053 696d 706c 6520 4c6f 6720 5365  he Simple Log Se
+000eb140: 7276 6963 6520 7072 6f6a 6563 7420 7468  rvice project th
+000eb150: 6174 2079 6f75 2077 616e 7420 746f 2075  at you want to u
+000eb160: 7365 2074 6f20 7374 6f72 6520 7468 6520  se to store the 
+000eb170: 6c6f 6773 206f 6620 636f 6e74 726f 6c20  logs of control 
+000eb180: 706c 616e 6520 636f 6d70 6f6e 656e 7473  plane components
+000eb190: 2e0a 2020 2020 2020 2020 2320 0a20 2020  ..        # .   
+000eb1a0: 2020 2020 2023 2044 6566 6175 6c74 2076       # Default v
+000eb1b0: 616c 7565 3a20 6b38 732d 6c6f 672d 2443  alue: k8s-log-$C
+000eb1c0: 6c75 7374 6572 2049 442e 0a20 2020 2020  luster ID..     
+000eb1d0: 2020 2073 656c 662e 6c6f 675f 7072 6f6a     self.log_proj
+000eb1e0: 6563 7420 3d20 6c6f 675f 7072 6f6a 6563  ect = log_projec
+000eb1f0: 740a 2020 2020 2020 2020 2320 5468 6520  t.        # The 
+000eb200: 7265 7465 6e74 696f 6e20 7065 7269 6f64  retention period
+000eb210: 206f 6620 7468 6520 6c6f 6720 6461 7461   of the log data
+000eb220: 2073 746f 7265 6420 696e 2074 6865 204c   stored in the L
+000eb230: 6f67 7374 6f72 652e 2056 616c 6964 2076  ogstore. Valid v
+000eb240: 616c 7565 733a 2031 2074 6f20 3330 3030  alues: 1 to 3000
+000eb250: 2e20 556e 6974 3a20 6461 7973 2e0a 2020  . Unit: days..  
+000eb260: 2020 2020 2020 2320 0a20 2020 2020 2020        # .       
+000eb270: 2023 2044 6566 6175 6c74 2076 616c 7565   # Default value
+000eb280: 3a20 3330 2e0a 2020 2020 2020 2020 7365  : 30..        se
+000eb290: 6c66 2e6c 6f67 5f74 746c 203d 206c 6f67  lf.log_ttl = log
+000eb2a0: 5f74 746c 0a0a 2020 2020 6465 6620 7661  _ttl..    def va
+000eb2b0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000eb2c0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000eb2d0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000eb2e0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000eb2f0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+000eb300: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000eb310: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000eb320: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000eb330: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000eb340: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000eb350: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000eb360: 616c 6975 6964 2069 7320 6e6f 7420 4e6f  aliuid is not No
+000eb370: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000eb380: 7265 7375 6c74 5b27 616c 6975 6964 275d  result['aliuid']
+000eb390: 203d 2073 656c 662e 616c 6975 6964 0a20   = self.aliuid. 
+000eb3a0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000eb3b0: 6f6d 706f 6e65 6e74 7320 6973 206e 6f74  omponents is not
+000eb3c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000eb3d0: 2020 2072 6573 756c 745b 2763 6f6d 706f     result['compo
+000eb3e0: 6e65 6e74 7327 5d20 3d20 7365 6c66 2e63  nents'] = self.c
+000eb3f0: 6f6d 706f 6e65 6e74 730a 2020 2020 2020  omponents.      
+000eb400: 2020 6966 2073 656c 662e 6c6f 675f 7072    if self.log_pr
+000eb410: 6f6a 6563 7420 6973 206e 6f74 204e 6f6e  oject is not Non
+000eb420: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000eb430: 6573 756c 745b 276c 6f67 5f70 726f 6a65  esult['log_proje
+000eb440: 6374 275d 203d 2073 656c 662e 6c6f 675f  ct'] = self.log_
+000eb450: 7072 6f6a 6563 740a 2020 2020 2020 2020  project.        
+000eb460: 6966 2073 656c 662e 6c6f 675f 7474 6c20  if self.log_ttl 
+000eb470: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000eb480: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000eb490: 276c 6f67 5f74 746c 275d 203d 2073 656c  'log_ttl'] = sel
+000eb4a0: 662e 6c6f 675f 7474 6c0a 2020 2020 2020  f.log_ttl.      
+000eb4b0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000eb4c0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000eb4d0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000eb4e0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+000eb4f0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+000eb500: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000eb510: 7428 2761 6c69 7569 6427 2920 6973 206e  t('aliuid') is n
+000eb520: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000eb530: 2020 2020 2073 656c 662e 616c 6975 6964       self.aliuid
+000eb540: 203d 206d 2e67 6574 2827 616c 6975 6964   = m.get('aliuid
+000eb550: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000eb560: 6765 7428 2763 6f6d 706f 6e65 6e74 7327  get('components'
+000eb570: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000eb580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000eb590: 636f 6d70 6f6e 656e 7473 203d 206d 2e67  components = m.g
+000eb5a0: 6574 2827 636f 6d70 6f6e 656e 7473 2729  et('components')
+000eb5b0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000eb5c0: 7428 276c 6f67 5f70 726f 6a65 6374 2729  t('log_project')
+000eb5d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000eb5e0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+000eb5f0: 6f67 5f70 726f 6a65 6374 203d 206d 2e67  og_project = m.g
+000eb600: 6574 2827 6c6f 675f 7072 6f6a 6563 7427  et('log_project'
+000eb610: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000eb620: 6574 2827 6c6f 675f 7474 6c27 2920 6973  et('log_ttl') is
+000eb630: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000eb640: 2020 2020 2020 2073 656c 662e 6c6f 675f         self.log_
+000eb650: 7474 6c20 3d20 6d2e 6765 7428 276c 6f67  ttl = m.get('log
+000eb660: 5f74 746c 2729 0a20 2020 2020 2020 2072  _ttl').        r
+000eb670: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000eb680: 7373 2055 7064 6174 6543 6f6e 7472 6f6c  ss UpdateControl
+000eb690: 506c 616e 654c 6f67 5265 7370 6f6e 7365  PlaneLogResponse
+000eb6a0: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
+000eb6b0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000eb6c0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000eb6d0: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+000eb6e0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+000eb6f0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+000eb700: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+000eb710: 2020 2020 2020 2020 7461 736b 5f69 643a          task_id:
+000eb720: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000eb730: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
+000eb740: 6520 636c 7573 7465 7220 4944 2e0a 2020  e cluster ID..  
+000eb750: 2020 2020 2020 7365 6c66 2e63 6c75 7374        self.clust
+000eb760: 6572 5f69 6420 3d20 636c 7573 7465 725f  er_id = cluster_
+000eb770: 6964 0a20 2020 2020 2020 2023 2054 6865  id.        # The
+000eb780: 2072 6571 7565 7374 2049 442e 0a20 2020   request ID..   
+000eb790: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+000eb7a0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+000eb7b0: 640a 2020 2020 2020 2020 2320 5468 6520  d.        # The 
+000eb7c0: 7461 736b 2049 442e 0a20 2020 2020 2020  task ID..       
+000eb7d0: 2073 656c 662e 7461 736b 5f69 6420 3d20   self.task_id = 
+000eb7e0: 7461 736b 5f69 640a 0a20 2020 2064 6566  task_id..    def
+000eb7f0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+000eb800: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000eb810: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000eb820: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000eb830: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+000eb840: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+000eb850: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+000eb860: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000eb870: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+000eb880: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+000eb890: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+000eb8a0: 6c66 2e63 6c75 7374 6572 5f69 6420 6973  lf.cluster_id is
+000eb8b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000eb8c0: 2020 2020 2020 2072 6573 756c 745b 2763         result['c
+000eb8d0: 6c75 7374 6572 5f69 6427 5d20 3d20 7365  luster_id'] = se
+000eb8e0: 6c66 2e63 6c75 7374 6572 5f69 640a 2020  lf.cluster_id.  
+000eb8f0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+000eb900: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
+000eb910: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000eb920: 2020 7265 7375 6c74 5b27 7265 7175 6573    result['reques
+000eb930: 745f 6964 275d 203d 2073 656c 662e 7265  t_id'] = self.re
+000eb940: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+000eb950: 2069 6620 7365 6c66 2e74 6173 6b5f 6964   if self.task_id
+000eb960: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000eb970: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000eb980: 5b27 7461 736b 5f69 6427 5d20 3d20 7365  ['task_id'] = se
+000eb990: 6c66 2e74 6173 6b5f 6964 0a20 2020 2020  lf.task_id.     
+000eb9a0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+000eb9b0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000eb9c0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+000eb9d0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+000eb9e0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000eb9f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000eba00: 6574 2827 636c 7573 7465 725f 6964 2729  et('cluster_id')
+000eba10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000eba20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000eba30: 6c75 7374 6572 5f69 6420 3d20 6d2e 6765  luster_id = m.ge
+000eba40: 7428 2763 6c75 7374 6572 5f69 6427 290a  t('cluster_id').
+000eba50: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000eba60: 2827 7265 7175 6573 745f 6964 2729 2069  ('request_id') i
+000eba70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000eba80: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+000eba90: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
+000ebaa0: 2772 6571 7565 7374 5f69 6427 290a 2020  'request_id').  
+000ebab0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000ebac0: 7461 736b 5f69 6427 2920 6973 206e 6f74  task_id') is not
+000ebad0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000ebae0: 2020 2073 656c 662e 7461 736b 5f69 6420     self.task_id 
+000ebaf0: 3d20 6d2e 6765 7428 2774 6173 6b5f 6964  = m.get('task_id
+000ebb00: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+000ebb10: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
+000ebb20: 7064 6174 6543 6f6e 7472 6f6c 506c 616e  pdateControlPlan
+000ebb30: 654c 6f67 5265 7370 6f6e 7365 2854 6561  eLogResponse(Tea
+000ebb40: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000ebb50: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000ebb60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000ebb70: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+000ebb80: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+000ebb90: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+000ebba0: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+000ebbb0: 0a20 2020 2020 2020 2062 6f64 793a 2055  .        body: U
+000ebbc0: 7064 6174 6543 6f6e 7472 6f6c 506c 616e  pdateControlPlan
+000ebbd0: 654c 6f67 5265 7370 6f6e 7365 426f 6479  eLogResponseBody
+000ebbe0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+000ebbf0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000ebc00: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+000ebc10: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000ebc20: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+000ebc30: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+000ebc40: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+000ebc50: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000ebc60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000ebc70: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+000ebc80: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000ebc90: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+000ebca0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000ebcb0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000ebcc0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000ebcd0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000ebce0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000ebcf0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000ebd00: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000ebd10: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000ebd20: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000ebd30: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+000ebd40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000ebd50: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+000ebd60: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+000ebd70: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000ebd80: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000ebd90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000ebda0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000ebdb0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000ebdc0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000ebdd0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+000ebde0: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+000ebdf0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ebe00: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+000ebe10: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+000ebe20: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+000ebe30: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000ebe40: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000ebe50: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000ebe60: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000ebe70: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000ebe80: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+000ebe90: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+000ebea0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ebeb0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000ebec0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000ebed0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000ebee0: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+000ebef0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000ebf00: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000ebf10: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+000ebf20: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000ebf30: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000ebf40: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+000ebf50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000ebf60: 2020 7465 6d70 5f6d 6f64 656c 203d 2055    temp_model = U
+000ebf70: 7064 6174 6543 6f6e 7472 6f6c 506c 616e  pdateControlPlan
+000ebf80: 654c 6f67 5265 7370 6f6e 7365 426f 6479  eLogResponseBody
+000ebf90: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+000ebfa0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+000ebfb0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+000ebfc0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+000ebfd0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+000ebfe0: 636c 6173 7320 5570 6461 7465 4b38 7343  class UpdateK8sC
+000ebff0: 6c75 7374 6572 5573 6572 436f 6e66 6967  lusterUserConfig
+000ec000: 4578 7069 7265 5265 7175 6573 7428 5465  ExpireRequest(Te
+000ec010: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+000ec020: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000ec030: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000ec040: 2065 7870 6972 655f 686f 7572 3a20 696e   expire_hour: in
+000ec050: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+000ec060: 2020 7573 6572 3a20 7374 7220 3d20 4e6f    user: str = No
+000ec070: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000ec080: 2020 2023 2054 6865 2076 616c 6964 6974     # The validit
+000ec090: 7920 7065 7269 6f64 206f 6620 7468 6520  y period of the 
+000ec0a0: 6b75 6265 636f 6e66 6967 2066 696c 652e  kubeconfig file.
+000ec0b0: 2055 6e69 743a 2068 6f75 7273 2e0a 2020   Unit: hours..  
+000ec0c0: 2020 2020 2020 2320 0a20 2020 2020 2020        # .       
+000ec0d0: 2023 203e 2054 6865 2076 616c 7565 206f   # > The value o
+000ec0e0: 6620 6578 7069 7265 5f68 6f75 7220 6d75  f expire_hour mu
+000ec0f0: 7374 2062 6520 6772 6561 7465 7220 7468  st be greater th
+000ec100: 616e 2030 2061 6e64 2065 7175 616c 2074  an 0 and equal t
+000ec110: 6f20 6f72 2073 6d61 6c6c 6572 2074 6861  o or smaller tha
+000ec120: 6e20 3837 3630 3030 2028 3130 3020 7965  n 876000 (100 ye
+000ec130: 6172 7329 2e0a 2020 2020 2020 2020 2320  ars)..        # 
+000ec140: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+000ec150: 7061 7261 6d65 7465 7220 6973 2072 6571  parameter is req
+000ec160: 7569 7265 642e 0a20 2020 2020 2020 2073  uired..        s
+000ec170: 656c 662e 6578 7069 7265 5f68 6f75 7220  elf.expire_hour 
+000ec180: 3d20 6578 7069 7265 5f68 6f75 720a 2020  = expire_hour.  
+000ec190: 2020 2020 2020 2320 5468 6520 7573 6572        # The user
+000ec1a0: 2049 442e 0a20 2020 2020 2020 2023 200a   ID..        # .
+000ec1b0: 2020 2020 2020 2020 2320 5468 6973 2070          # This p
+000ec1c0: 6172 616d 6574 6572 2069 7320 7265 7175  arameter is requ
+000ec1d0: 6972 6564 2e0a 2020 2020 2020 2020 7365  ired..        se
+000ec1e0: 6c66 2e75 7365 7220 3d20 7573 6572 0a0a  lf.user = user..
+000ec1f0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000ec200: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000ec210: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+000ec220: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000ec230: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000ec240: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+000ec250: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000ec260: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000ec270: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000ec280: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000ec290: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000ec2a0: 2020 6966 2073 656c 662e 6578 7069 7265    if self.expire
+000ec2b0: 5f68 6f75 7220 6973 206e 6f74 204e 6f6e  _hour is not Non
+000ec2c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000ec2d0: 6573 756c 745b 2765 7870 6972 655f 686f  esult['expire_ho
+000ec2e0: 7572 275d 203d 2073 656c 662e 6578 7069  ur'] = self.expi
+000ec2f0: 7265 5f68 6f75 720a 2020 2020 2020 2020  re_hour.        
+000ec300: 6966 2073 656c 662e 7573 6572 2069 7320  if self.user is 
+000ec310: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000ec320: 2020 2020 2020 7265 7375 6c74 5b27 7573        result['us
+000ec330: 6572 275d 203d 2073 656c 662e 7573 6572  er'] = self.user
+000ec340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000ec350: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000ec360: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000ec370: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000ec380: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000ec390: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000ec3a0: 6966 206d 2e67 6574 2827 6578 7069 7265  if m.get('expire
+000ec3b0: 5f68 6f75 7227 2920 6973 206e 6f74 204e  _hour') is not N
+000ec3c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ec3d0: 2073 656c 662e 6578 7069 7265 5f68 6f75   self.expire_hou
+000ec3e0: 7220 3d20 6d2e 6765 7428 2765 7870 6972  r = m.get('expir
+000ec3f0: 655f 686f 7572 2729 0a20 2020 2020 2020  e_hour').       
+000ec400: 2069 6620 6d2e 6765 7428 2775 7365 7227   if m.get('user'
+000ec410: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000ec420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000ec430: 7573 6572 203d 206d 2e67 6574 2827 7573  user = m.get('us
+000ec440: 6572 2729 0a20 2020 2020 2020 2072 6574  er').        ret
+000ec450: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+000ec460: 2055 7064 6174 654b 3873 436c 7573 7465   UpdateK8sCluste
+000ec470: 7255 7365 7243 6f6e 6669 6745 7870 6972  rUserConfigExpir
+000ec480: 6552 6573 706f 6e73 6528 5465 614d 6f64  eResponse(TeaMod
+000ec490: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000ec4a0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000ec4b0: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+000ec4c0: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+000ec4d0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+000ec4e0: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+000ec4f0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+000ec500: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+000ec510: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+000ec520: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+000ec530: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000ec540: 7461 7475 735f 636f 6465 0a0a 2020 2020  tatus_code..    
+000ec550: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+000ec560: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+000ec570: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000ec580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000ec590: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+000ec5a0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000ec5b0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000ec5c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ec5d0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+000ec5e0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+000ec5f0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000ec600: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+000ec610: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000ec620: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+000ec630: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+000ec640: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+000ec650: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+000ec660: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+000ec670: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000ec680: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+000ec690: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+000ec6a0: 636f 6465 0a20 2020 2020 2020 2072 6574  code.        ret
+000ec6b0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000ec6c0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000ec6d0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+000ec6e0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000ec6f0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000ec700: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+000ec710: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+000ec720: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ec730: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000ec740: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000ec750: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000ec760: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+000ec770: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000ec780: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000ec790: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+000ec7a0: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000ec7b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000ec7c0: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+000ec7d0: 7465 5465 6d70 6c61 7465 5265 7175 6573  teTemplateReques
+000ec7e0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+000ec7f0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000ec800: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000ec810: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000ec820: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000ec830: 2020 2020 2020 6e61 6d65 3a20 7374 7220        name: str 
+000ec840: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000ec850: 7461 6773 3a20 7374 7220 3d20 4e6f 6e65  tags: str = None
+000ec860: 2c0a 2020 2020 2020 2020 7465 6d70 6c61  ,.        templa
+000ec870: 7465 3a20 7374 7220 3d20 4e6f 6e65 2c0a  te: str = None,.
+000ec880: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
+000ec890: 5f74 7970 653a 2073 7472 203d 204e 6f6e  _type: str = Non
+000ec8a0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000ec8b0: 2020 2320 5468 6520 6465 7363 7269 7074    # The descript
+000ec8c0: 696f 6e20 6f66 2074 6865 2074 656d 706c  ion of the templ
+000ec8d0: 6174 652e 0a20 2020 2020 2020 2073 656c  ate..        sel
+000ec8e0: 662e 6465 7363 7269 7074 696f 6e20 3d20  f.description = 
+000ec8f0: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
+000ec900: 2020 2020 2320 5468 6520 6e61 6d65 206f      # The name o
+000ec910: 6620 7468 6520 7465 6d70 6c61 7465 2e0a  f the template..
+000ec920: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
+000ec930: 6520 3d20 6e61 6d65 0a20 2020 2020 2020  e = name.       
+000ec940: 2023 2054 6865 206c 6162 656c 206f 6620   # The label of 
+000ec950: 7468 6520 7465 6d70 6c61 7465 2e0a 2020  the template..  
+000ec960: 2020 2020 2020 7365 6c66 2e74 6167 7320        self.tags 
+000ec970: 3d20 7461 6773 0a20 2020 2020 2020 2023  = tags.        #
+000ec980: 2054 6865 2059 414d 4c20 636f 6e74 656e   The YAML conten
+000ec990: 7420 6f66 2074 6865 2074 656d 706c 6174  t of the templat
+000ec9a0: 652e 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+000ec9b0: 7465 6d70 6c61 7465 203d 2074 656d 706c  template = templ
+000ec9c0: 6174 650a 2020 2020 2020 2020 2320 5468  ate.        # Th
+000ec9d0: 6520 7479 7065 206f 6620 7465 6d70 6c61  e type of templa
+000ec9e0: 7465 2e20 5468 6973 2070 6172 616d 6574  te. This paramet
+000ec9f0: 6572 2063 616e 2062 6520 7365 7420 746f  er can be set to
+000eca00: 2061 2063 7573 746f 6d20 7661 6c75 652e   a custom value.
+000eca10: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
+000eca20: 2020 2020 2320 2a20 2020 4966 2074 6865      # *   If the
+000eca30: 2070 6172 616d 6574 6572 2069 7320 7365   parameter is se
+000eca40: 7420 746f 2060 6b75 6265 726e 6574 6573  t to `kubernetes
+000eca50: 602c 2074 6865 2074 656d 706c 6174 6520  `, the template 
+000eca60: 6973 2064 6973 706c 6179 6564 206f 6e20  is displayed on 
+000eca70: 7468 6520 5465 6d70 6c61 7465 7320 7061  the Templates pa
+000eca80: 6765 2069 6e20 7468 6520 636f 6e73 6f6c  ge in the consol
+000eca90: 652e 0a20 2020 2020 2020 2023 202a 2020  e..        # *  
+000ecaa0: 2049 6620 7468 6520 7061 7261 6d65 7465   If the paramete
+000ecab0: 7220 6973 2073 6574 2074 6f20 6063 6f6d  r is set to `com
+000ecac0: 706f 7365 602c 2074 6865 2074 656d 706c  pose`, the templ
+000ecad0: 6174 6520 6973 2064 6973 706c 6179 6564  ate is displayed
+000ecae0: 206f 6e20 7468 6520 436f 6e74 6169 6e65   on the Containe
+000ecaf0: 7220 5365 7276 6963 6520 2d20 5377 6172  r Service - Swar
+000ecb00: 6d20 7061 6765 2069 6e20 7468 6520 636f  m page in the co
+000ecb10: 6e73 6f6c 652e 2043 6f6e 7461 696e 6572  nsole. Container
+000ecb20: 2053 6572 7669 6365 2066 6f72 2053 7761   Service for Swa
+000ecb30: 726d 2069 7320 6465 7072 6563 6174 6564  rm is deprecated
+000ecb40: 2e0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+000ecb50: 656d 706c 6174 655f 7479 7065 203d 2074  emplate_type = t
+000ecb60: 656d 706c 6174 655f 7479 7065 0a0a 2020  emplate_type..  
+000ecb70: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+000ecb80: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+000ecb90: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+000ecba0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+000ecbb0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+000ecbc0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000ecbd0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+000ecbe0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000ecbf0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000ecc00: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000ecc10: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000ecc20: 6966 2073 656c 662e 6465 7363 7269 7074  if self.descript
+000ecc30: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
+000ecc40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000ecc50: 756c 745b 2764 6573 6372 6970 7469 6f6e  ult['description
+000ecc60: 275d 203d 2073 656c 662e 6465 7363 7269  '] = self.descri
+000ecc70: 7074 696f 6e0a 2020 2020 2020 2020 6966  ption.        if
+000ecc80: 2073 656c 662e 6e61 6d65 2069 7320 6e6f   self.name is no
+000ecc90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000ecca0: 2020 2020 7265 7375 6c74 5b27 6e61 6d65      result['name
+000eccb0: 275d 203d 2073 656c 662e 6e61 6d65 0a20  '] = self.name. 
+000eccc0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+000eccd0: 6167 7320 6973 206e 6f74 204e 6f6e 653a  ags is not None:
+000ecce0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000eccf0: 756c 745b 2774 6167 7327 5d20 3d20 7365  ult['tags'] = se
+000ecd00: 6c66 2e74 6167 730a 2020 2020 2020 2020  lf.tags.        
+000ecd10: 6966 2073 656c 662e 7465 6d70 6c61 7465  if self.template
+000ecd20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000ecd30: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000ecd40: 5b27 7465 6d70 6c61 7465 275d 203d 2073  ['template'] = s
+000ecd50: 656c 662e 7465 6d70 6c61 7465 0a20 2020  elf.template.   
+000ecd60: 2020 2020 2069 6620 7365 6c66 2e74 656d       if self.tem
+000ecd70: 706c 6174 655f 7479 7065 2069 7320 6e6f  plate_type is no
+000ecd80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000ecd90: 2020 2020 7265 7375 6c74 5b27 7465 6d70      result['temp
+000ecda0: 6c61 7465 5f74 7970 6527 5d20 3d20 7365  late_type'] = se
+000ecdb0: 6c66 2e74 656d 706c 6174 655f 7479 7065  lf.template_type
+000ecdc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000ecdd0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000ecde0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000ecdf0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000ece00: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000ece10: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000ece20: 6966 206d 2e67 6574 2827 6465 7363 7269  if m.get('descri
+000ece30: 7074 696f 6e27 2920 6973 206e 6f74 204e  ption') is not N
+000ece40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ece50: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+000ece60: 6e20 3d20 6d2e 6765 7428 2764 6573 6372  n = m.get('descr
+000ece70: 6970 7469 6f6e 2729 0a20 2020 2020 2020  iption').       
+000ece80: 2069 6620 6d2e 6765 7428 276e 616d 6527   if m.get('name'
+000ece90: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000ecea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000eceb0: 6e61 6d65 203d 206d 2e67 6574 2827 6e61  name = m.get('na
+000ecec0: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
+000eced0: 6d2e 6765 7428 2774 6167 7327 2920 6973  m.get('tags') is
+000ecee0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000ecef0: 2020 2020 2020 2073 656c 662e 7461 6773         self.tags
+000ecf00: 203d 206d 2e67 6574 2827 7461 6773 2729   = m.get('tags')
+000ecf10: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000ecf20: 7428 2774 656d 706c 6174 6527 2920 6973  t('template') is
+000ecf30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000ecf40: 2020 2020 2020 2073 656c 662e 7465 6d70         self.temp
+000ecf50: 6c61 7465 203d 206d 2e67 6574 2827 7465  late = m.get('te
+000ecf60: 6d70 6c61 7465 2729 0a20 2020 2020 2020  mplate').       
+000ecf70: 2069 6620 6d2e 6765 7428 2774 656d 706c   if m.get('templ
+000ecf80: 6174 655f 7479 7065 2729 2069 7320 6e6f  ate_type') is no
+000ecf90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000ecfa0: 2020 2020 7365 6c66 2e74 656d 706c 6174      self.templat
+000ecfb0: 655f 7479 7065 203d 206d 2e67 6574 2827  e_type = m.get('
+000ecfc0: 7465 6d70 6c61 7465 5f74 7970 6527 290a  template_type').
+000ecfd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000ecfe0: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+000ecff0: 7465 5465 6d70 6c61 7465 5265 7370 6f6e  teTemplateRespon
+000ed000: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+000ed010: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000ed020: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000ed030: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+000ed040: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+000ed050: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+000ed060: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+000ed070: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000ed080: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+000ed090: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+000ed0a0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000ed0b0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+000ed0c0: 6f64 650a 0a20 2020 2064 6566 2076 616c  ode..    def val
+000ed0d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000ed0e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000ed0f0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+000ed100: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000ed110: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+000ed120: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+000ed130: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000ed140: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000ed150: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+000ed160: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+000ed170: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+000ed180: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+000ed190: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ed1a0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+000ed1b0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+000ed1c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000ed1d0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+000ed1e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000ed1f0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+000ed200: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+000ed210: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+000ed220: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000ed230: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000ed240: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+000ed250: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000ed260: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000ed270: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000ed280: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000ed290: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000ed2a0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+000ed2b0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+000ed2c0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000ed2d0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+000ed2e0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+000ed2f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000ed300: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+000ed310: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+000ed320: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+000ed330: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+000ed340: 6c61 7373 2055 7064 6174 6555 7365 7250  lass UpdateUserP
+000ed350: 6572 6d69 7373 696f 6e73 5265 7175 6573  ermissionsReques
+000ed360: 7442 6f64 7928 5465 614d 6f64 656c 293a  tBody(TeaModel):
+000ed370: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000ed380: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+000ed390: 0a20 2020 2020 2020 2063 6c75 7374 6572  .        cluster
+000ed3a0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000ed3b0: 2020 2020 2020 6973 5f63 7573 746f 6d3a        is_custom:
+000ed3c0: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
+000ed3d0: 2020 2020 2020 6973 5f72 616d 5f72 6f6c        is_ram_rol
+000ed3e0: 653a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  e: bool = None,.
+000ed3f0: 2020 2020 2020 2020 6e61 6d65 7370 6163          namespac
+000ed400: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+000ed410: 2020 2020 2020 2072 6f6c 655f 6e61 6d65         role_name
+000ed420: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000ed430: 2020 2020 2020 726f 6c65 5f74 7970 653a        role_type:
+000ed440: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000ed450: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+000ed460: 2e63 6c75 7374 6572 203d 2063 6c75 7374  .cluster = clust
+000ed470: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+000ed480: 6973 5f63 7573 746f 6d20 3d20 6973 5f63  is_custom = is_c
+000ed490: 7573 746f 6d0a 2020 2020 2020 2020 7365  ustom.        se
+000ed4a0: 6c66 2e69 735f 7261 6d5f 726f 6c65 203d  lf.is_ram_role =
+000ed4b0: 2069 735f 7261 6d5f 726f 6c65 0a20 2020   is_ram_role.   
+000ed4c0: 2020 2020 2073 656c 662e 6e61 6d65 7370       self.namesp
+000ed4d0: 6163 6520 3d20 6e61 6d65 7370 6163 650a  ace = namespace.
+000ed4e0: 2020 2020 2020 2020 7365 6c66 2e72 6f6c          self.rol
+000ed4f0: 655f 6e61 6d65 203d 2072 6f6c 655f 6e61  e_name = role_na
+000ed500: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
+000ed510: 726f 6c65 5f74 7970 6520 3d20 726f 6c65  role_type = role
+000ed520: 5f74 7970 650a 0a20 2020 2064 6566 2076  _type..    def v
+000ed530: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000ed540: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000ed550: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000ed560: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000ed570: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000ed580: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000ed590: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+000ed5a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000ed5b0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+000ed5c0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+000ed5d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000ed5e0: 2e63 6c75 7374 6572 2069 7320 6e6f 7420  .cluster is not 
+000ed5f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000ed600: 2020 7265 7375 6c74 5b27 636c 7573 7465    result['cluste
+000ed610: 7227 5d20 3d20 7365 6c66 2e63 6c75 7374  r'] = self.clust
+000ed620: 6572 0a20 2020 2020 2020 2069 6620 7365  er.        if se
+000ed630: 6c66 2e69 735f 6375 7374 6f6d 2069 7320  lf.is_custom is 
 000ed640: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ed650: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000ed660: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000ed670: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000ed680: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-000ed690: 5d20 3d20 5b5d 0a20 2020 2020 2020 2069  ] = [].        i
-000ed6a0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-000ed6b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000ed6c0: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
-000ed6d0: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
-000ed6e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000ed6f0: 2762 6f64 7927 5d2e 6170 7065 6e64 286b  'body'].append(k
-000ed700: 2e74 6f5f 6d61 7028 2920 6966 206b 2065  .to_map() if k e
-000ed710: 6c73 6520 4e6f 6e65 290a 2020 2020 2020  lse None).      
-000ed720: 2020 6966 2073 656c 662e 6d6f 6465 2069    if self.mode i
-000ed730: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ed740: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ed750: 6d6f 6465 275d 203d 2073 656c 662e 6d6f  mode'] = self.mo
-000ed760: 6465 0a20 2020 2020 2020 2072 6574 7572  de.        retur
-000ed770: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000ed780: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000ed790: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000ed7a0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000ed7b0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000ed7c0: 2020 7365 6c66 2e62 6f64 7920 3d20 5b5d    self.body = []
-000ed7d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000ed7e0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-000ed7f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ed800: 2020 2066 6f72 206b 2069 6e20 6d2e 6765     for k in m.ge
-000ed810: 7428 2762 6f64 7927 293a 0a20 2020 2020  t('body'):.     
-000ed820: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-000ed830: 6d6f 6465 6c20 3d20 5570 6461 7465 5573  model = UpdateUs
-000ed840: 6572 5065 726d 6973 7369 6f6e 7352 6571  erPermissionsReq
-000ed850: 7565 7374 426f 6479 2829 0a20 2020 2020  uestBody().     
-000ed860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000ed870: 626f 6479 2e61 7070 656e 6428 7465 6d70  body.append(temp
-000ed880: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-000ed890: 6b29 290a 2020 2020 2020 2020 6966 206d  k)).        if m
-000ed8a0: 2e67 6574 2827 6d6f 6465 2729 2069 7320  .get('mode') is 
-000ed8b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ed8c0: 2020 2020 2020 7365 6c66 2e6d 6f64 6520        self.mode 
-000ed8d0: 3d20 6d2e 6765 7428 276d 6f64 6527 290a  = m.get('mode').
-000ed8e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000ed8f0: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
-000ed900: 7465 5573 6572 5065 726d 6973 7369 6f6e  teUserPermission
-000ed910: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
-000ed920: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000ed930: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000ed940: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
-000ed950: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
-000ed960: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-000ed970: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
-000ed980: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-000ed990: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-000ed9a0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-000ed9b0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-000ed9c0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-000ed9d0: 7461 7475 735f 636f 6465 0a0a 2020 2020  tatus_code..    
-000ed9e0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-000ed9f0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-000eda00: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000eda10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000eda20: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000eda30: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000eda40: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000eda50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000eda60: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000eda70: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000eda80: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000eda90: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-000edaa0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000edab0: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-000edac0: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-000edad0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-000edae0: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-000edaf0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-000edb00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000edb10: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-000edb20: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-000edb30: 636f 6465 0a20 2020 2020 2020 2072 6574  code.        ret
-000edb40: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000edb50: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000edb60: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000edb70: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000edb80: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000edb90: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-000edba0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-000edbb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000edbc0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-000edbd0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000edbe0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000edbf0: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-000edc00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000edc10: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000edc20: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-000edc30: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-000edc40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000edc50: 656c 660a 0a0a 636c 6173 7320 5570 6772  elf...class Upgr
-000edc60: 6164 6543 6c75 7374 6572 5265 7175 6573  adeClusterReques
-000edc70: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
-000edc80: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-000edc90: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000edca0: 2020 2020 2063 6f6d 706f 6e65 6e74 5f6e       component_n
-000edcb0: 616d 653a 2073 7472 203d 204e 6f6e 652c  ame: str = None,
-000edcc0: 0a20 2020 2020 2020 206d 6173 7465 725f  .        master_
-000edcd0: 6f6e 6c79 3a20 626f 6f6c 203d 204e 6f6e  only: bool = Non
-000edce0: 652c 0a20 2020 2020 2020 206e 6578 745f  e,.        next_
-000edcf0: 7665 7273 696f 6e3a 2073 7472 203d 204e  version: str = N
-000edd00: 6f6e 652c 0a20 2020 2020 2020 2076 6572  one,.        ver
-000edd10: 7369 6f6e 3a20 7374 7220 3d20 4e6f 6e65  sion: str = None
-000edd20: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-000edd30: 2023 2054 6865 206e 616d 6520 6f66 2074   # The name of t
-000edd40: 6865 2063 6f6d 706f 6e65 6e74 2e20 5365  he component. Se
-000edd50: 7420 7468 6520 7661 6c75 6520 746f 2060  t the value to `
-000edd60: 6b38 7360 2e0a 2020 2020 2020 2020 7365  k8s`..        se
-000edd70: 6c66 2e63 6f6d 706f 6e65 6e74 5f6e 616d  lf.component_nam
-000edd80: 6520 3d20 636f 6d70 6f6e 656e 745f 6e61  e = component_na
-000edd90: 6d65 0a20 2020 2020 2020 2023 2053 7065  me.        # Spe
-000edda0: 6369 6669 6573 2077 6865 7468 6572 2074  cifies whether t
-000eddb0: 6f20 7570 6461 7465 206f 6e6c 7920 6d61  o update only ma
-000eddc0: 7374 6572 206e 6f64 6573 2e20 5661 6c69  ster nodes. Vali
-000eddd0: 6420 7661 6c75 6573 3a0a 2020 2020 2020  d values:.      
-000edde0: 2020 2320 0a20 2020 2020 2020 2023 202a    # .        # *
-000eddf0: 2020 2074 7275 653a 2075 7064 6174 6520     true: update 
-000ede00: 6f6e 6c79 206d 6173 7465 7220 6e6f 6465  only master node
-000ede10: 732e 0a20 2020 2020 2020 2023 202a 2020  s..        # *  
-000ede20: 2066 616c 7365 3a20 7570 6461 7465 206d   false: update m
-000ede30: 6173 7465 7220 616e 6420 776f 726b 6572  aster and worker
-000ede40: 206e 6f64 6573 2e0a 2020 2020 2020 2020   nodes..        
-000ede50: 7365 6c66 2e6d 6173 7465 725f 6f6e 6c79  self.master_only
-000ede60: 203d 206d 6173 7465 725f 6f6e 6c79 0a20   = master_only. 
-000ede70: 2020 2020 2020 2023 2054 6865 204b 7562         # The Kub
-000ede80: 6572 6e65 7465 7320 7665 7273 696f 6e20  ernetes version 
-000ede90: 746f 2077 6869 6368 2074 6865 2063 6c75  to which the clu
-000edea0: 7374 6572 2063 616e 2062 6520 7570 6461  ster can be upda
-000edeb0: 7465 642e 0a20 2020 2020 2020 2073 656c  ted..        sel
-000edec0: 662e 6e65 7874 5f76 6572 7369 6f6e 203d  f.next_version =
-000eded0: 206e 6578 745f 7665 7273 696f 6e0a 2020   next_version.  
-000edee0: 2020 2020 2020 2320 5468 6520 6375 7272        # The curr
-000edef0: 656e 7420 4b75 6265 726e 6574 6573 2076  ent Kubernetes v
-000edf00: 6572 7369 6f6e 206f 6620 7468 6520 636c  ersion of the cl
-000edf10: 7573 7465 722e 2046 6f72 206d 6f72 6520  uster. For more 
-000edf20: 696e 666f 726d 6174 696f 6e2c 2073 6565  information, see
-000edf30: 205b 4b75 6265 726e 6574 6573 2076 6572   [Kubernetes ver
-000edf40: 7369 6f6e 735d 2868 7474 7073 3a2f 2f68  sions](https://h
-000edf50: 656c 702e 616c 6979 756e 2e63 6f6d 2f64  elp.aliyun.com/d
-000edf60: 6f63 756d 656e 745f 6465 7461 696c 2f31  ocument_detail/1
-000edf70: 3835 3236 392e 6874 6d6c 292e 0a20 2020  85269.html)..   
-000edf80: 2020 2020 2073 656c 662e 7665 7273 696f       self.versio
-000edf90: 6e20 3d20 7665 7273 696f 6e0a 0a20 2020  n = version..   
-000edfa0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000edfb0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-000edfc0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-000edfd0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000edfe0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000edff0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000ee000: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000ee010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ee020: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000ee030: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000ee040: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000ee050: 6620 7365 6c66 2e63 6f6d 706f 6e65 6e74  f self.component
-000ee060: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
-000ee070: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000ee080: 6573 756c 745b 2763 6f6d 706f 6e65 6e74  esult['component
-000ee090: 5f6e 616d 6527 5d20 3d20 7365 6c66 2e63  _name'] = self.c
-000ee0a0: 6f6d 706f 6e65 6e74 5f6e 616d 650a 2020  omponent_name.  
-000ee0b0: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
-000ee0c0: 7374 6572 5f6f 6e6c 7920 6973 206e 6f74  ster_only is not
-000ee0d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ee0e0: 2020 2072 6573 756c 745b 276d 6173 7465     result['maste
-000ee0f0: 725f 6f6e 6c79 275d 203d 2073 656c 662e  r_only'] = self.
-000ee100: 6d61 7374 6572 5f6f 6e6c 790a 2020 2020  master_only.    
-000ee110: 2020 2020 6966 2073 656c 662e 6e65 7874      if self.next
-000ee120: 5f76 6572 7369 6f6e 2069 7320 6e6f 7420  _version is not 
-000ee130: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ee140: 2020 7265 7375 6c74 5b27 6e65 7874 5f76    result['next_v
-000ee150: 6572 7369 6f6e 275d 203d 2073 656c 662e  ersion'] = self.
-000ee160: 6e65 7874 5f76 6572 7369 6f6e 0a20 2020  next_version.   
-000ee170: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
-000ee180: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-000ee190: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000ee1a0: 7375 6c74 5b27 7665 7273 696f 6e27 5d20  sult['version'] 
-000ee1b0: 3d20 7365 6c66 2e76 6572 7369 6f6e 0a20  = self.version. 
-000ee1c0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000ee1d0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000ee1e0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000ee1f0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000ee200: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000ee210: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000ee220: 206d 2e67 6574 2827 636f 6d70 6f6e 656e   m.get('componen
-000ee230: 745f 6e61 6d65 2729 2069 7320 6e6f 7420  t_name') is not 
-000ee240: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ee250: 2020 7365 6c66 2e63 6f6d 706f 6e65 6e74    self.component
-000ee260: 5f6e 616d 6520 3d20 6d2e 6765 7428 2763  _name = m.get('c
-000ee270: 6f6d 706f 6e65 6e74 5f6e 616d 6527 290a  omponent_name').
-000ee280: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000ee290: 2827 6d61 7374 6572 5f6f 6e6c 7927 2920  ('master_only') 
-000ee2a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000ee2b0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-000ee2c0: 7374 6572 5f6f 6e6c 7920 3d20 6d2e 6765  ster_only = m.ge
-000ee2d0: 7428 276d 6173 7465 725f 6f6e 6c79 2729  t('master_only')
-000ee2e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000ee2f0: 7428 276e 6578 745f 7665 7273 696f 6e27  t('next_version'
-000ee300: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000ee310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000ee320: 6e65 7874 5f76 6572 7369 6f6e 203d 206d  next_version = m
-000ee330: 2e67 6574 2827 6e65 7874 5f76 6572 7369  .get('next_versi
-000ee340: 6f6e 2729 0a20 2020 2020 2020 2069 6620  on').        if 
-000ee350: 6d2e 6765 7428 2776 6572 7369 6f6e 2729  m.get('version')
-000ee360: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000ee370: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-000ee380: 6572 7369 6f6e 203d 206d 2e67 6574 2827  ersion = m.get('
-000ee390: 7665 7273 696f 6e27 290a 2020 2020 2020  version').      
-000ee3a0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000ee3b0: 636c 6173 7320 5570 6772 6164 6543 6c75  class UpgradeClu
-000ee3c0: 7374 6572 5265 7370 6f6e 7365 426f 6479  sterResponseBody
-000ee3d0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-000ee3e0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-000ee3f0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-000ee400: 2020 2020 636c 7573 7465 725f 6964 3a20      cluster_id: 
-000ee410: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000ee420: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-000ee430: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000ee440: 2020 2020 7461 736b 5f69 643a 2073 7472      task_id: str
-000ee450: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000ee460: 2020 2020 2020 2020 7365 6c66 2e63 6c75          self.clu
-000ee470: 7374 6572 5f69 6420 3d20 636c 7573 7465  ster_id = cluste
-000ee480: 725f 6964 0a20 2020 2020 2020 2073 656c  r_id.        sel
-000ee490: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
-000ee4a0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
-000ee4b0: 2020 7365 6c66 2e74 6173 6b5f 6964 203d    self.task_id =
-000ee4c0: 2074 6173 6b5f 6964 0a0a 2020 2020 6465   task_id..    de
-000ee4d0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000ee4e0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-000ee4f0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000ee500: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000ee510: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000ee520: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000ee530: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000ee540: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000ee550: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000ee560: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000ee570: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000ee580: 656c 662e 636c 7573 7465 725f 6964 2069  elf.cluster_id i
-000ee590: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ee5a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ee5b0: 636c 7573 7465 725f 6964 275d 203d 2073  cluster_id'] = s
-000ee5c0: 656c 662e 636c 7573 7465 725f 6964 0a20  elf.cluster_id. 
-000ee5d0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-000ee5e0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-000ee5f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ee600: 2020 2072 6573 756c 745b 2772 6571 7565     result['reque
-000ee610: 7374 5f69 6427 5d20 3d20 7365 6c66 2e72  st_id'] = self.r
-000ee620: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
-000ee630: 2020 6966 2073 656c 662e 7461 736b 5f69    if self.task_i
-000ee640: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000ee650: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000ee660: 745b 2774 6173 6b5f 6964 275d 203d 2073  t['task_id'] = s
-000ee670: 656c 662e 7461 736b 5f69 640a 2020 2020  elf.task_id.    
-000ee680: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000ee690: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000ee6a0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000ee6b0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000ee6c0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000ee6d0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000ee6e0: 6765 7428 2763 6c75 7374 6572 5f69 6427  get('cluster_id'
-000ee6f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000ee700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000ee710: 636c 7573 7465 725f 6964 203d 206d 2e67  cluster_id = m.g
-000ee720: 6574 2827 636c 7573 7465 725f 6964 2729  et('cluster_id')
-000ee730: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000ee740: 7428 2772 6571 7565 7374 5f69 6427 2920  t('request_id') 
-000ee750: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000ee760: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000ee770: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-000ee780: 2827 7265 7175 6573 745f 6964 2729 0a20  ('request_id'). 
-000ee790: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000ee7a0: 2774 6173 6b5f 6964 2729 2069 7320 6e6f  'task_id') is no
-000ee7b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000ee7c0: 2020 2020 7365 6c66 2e74 6173 6b5f 6964      self.task_id
-000ee7d0: 203d 206d 2e67 6574 2827 7461 736b 5f69   = m.get('task_i
-000ee7e0: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
-000ee7f0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-000ee800: 5570 6772 6164 6543 6c75 7374 6572 5265  UpgradeClusterRe
-000ee810: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-000ee820: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000ee830: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000ee840: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-000ee850: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-000ee860: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000ee870: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-000ee880: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-000ee890: 2020 2062 6f64 793a 2055 7067 7261 6465     body: Upgrade
-000ee8a0: 436c 7573 7465 7252 6573 706f 6e73 6542  ClusterResponseB
-000ee8b0: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
-000ee8c0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000ee8d0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-000ee8e0: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-000ee8f0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-000ee900: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-000ee910: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-000ee920: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-000ee930: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000ee940: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-000ee950: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000ee960: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-000ee970: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000ee980: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000ee990: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000ee9a0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000ee9b0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000ee9c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000ee9d0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000ee9e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000ee9f0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000eea00: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-000eea10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000eea20: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000eea30: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-000eea40: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-000eea50: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-000eea60: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-000eea70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000eea80: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-000eea90: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-000eeaa0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-000eeab0: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-000eeac0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000eead0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-000eeae0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-000eeaf0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000eeb00: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000eeb10: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000eeb20: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-000eeb30: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-000eeb40: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000eeb50: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000eeb60: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-000eeb70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000eeb80: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-000eeb90: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-000eeba0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-000eebb0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-000eebc0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000eebd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000eebe0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-000eebf0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-000eec00: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000eec10: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-000eec20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000eec30: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-000eec40: 3d20 5570 6772 6164 6543 6c75 7374 6572  = UpgradeCluster
-000eec50: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
-000eec60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000eec70: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
-000eec80: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
-000eec90: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
-000eeca0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000eecb0: 7320 5570 6772 6164 6543 6c75 7374 6572  s UpgradeCluster
-000eecc0: 4164 646f 6e73 5265 7175 6573 7442 6f64  AddonsRequestBod
-000eecd0: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
-000eece0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-000eecf0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000eed00: 2020 2020 2063 6f6d 706f 6e65 6e74 5f6e       component_n
-000eed10: 616d 653a 2073 7472 203d 204e 6f6e 652c  ame: str = None,
-000eed20: 0a20 2020 2020 2020 2063 6f6e 6669 673a  .        config:
-000eed30: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000eed40: 2020 2020 206e 6578 745f 7665 7273 696f       next_versio
-000eed50: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
-000eed60: 2020 2020 2020 2070 6f6c 6963 793a 2073         policy: s
-000eed70: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000eed80: 2020 2076 6572 7369 6f6e 3a20 7374 7220     version: str 
-000eed90: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-000eeda0: 2020 2020 2020 2023 2054 6865 206e 616d         # The nam
-000eedb0: 6520 6f66 2074 6865 2063 6f6d 706f 6e65  e of the compone
-000eedc0: 6e74 2e0a 2020 2020 2020 2020 2320 0a20  nt..        # . 
-000eedd0: 2020 2020 2020 2023 2054 6869 7320 7061         # This pa
-000eede0: 7261 6d65 7465 7220 6973 2072 6571 7569  rameter is requi
-000eedf0: 7265 642e 0a20 2020 2020 2020 2073 656c  red..        sel
-000eee00: 662e 636f 6d70 6f6e 656e 745f 6e61 6d65  f.component_name
-000eee10: 203d 2063 6f6d 706f 6e65 6e74 5f6e 616d   = component_nam
-000eee20: 650a 2020 2020 2020 2020 2320 5468 6520  e.        # The 
-000eee30: 6375 7374 6f6d 2063 6f6d 706f 6e65 6e74  custom component
-000eee40: 2073 6574 7469 6e67 7320 7468 6174 2079   settings that y
-000eee50: 6f75 2077 616e 7420 746f 2075 7365 2e20  ou want to use. 
-000eee60: 5468 6520 7661 6c75 6520 6973 2061 204a  The value is a J
-000eee70: 534f 4e20 7374 7269 6e67 2e0a 2020 2020  SON string..    
-000eee80: 2020 2020 7365 6c66 2e63 6f6e 6669 6720      self.config 
-000eee90: 3d20 636f 6e66 6967 0a20 2020 2020 2020  = config.       
-000eeea0: 2023 2054 6865 2076 6572 7369 6f6e 2074   # The version t
-000eeeb0: 6f20 7768 6963 6820 7468 6520 636f 6d70  o which the comp
-000eeec0: 6f6e 656e 7420 6361 6e20 6265 2075 7064  onent can be upd
-000eeed0: 6174 6564 2e20 596f 7520 6361 6e20 6361  ated. You can ca
-000eeee0: 6c6c 2074 6865 2060 4465 7363 7269 6265  ll the `Describe
-000eeef0: 436c 7573 7465 7241 6464 6f6e 7356 6572  ClusterAddonsVer
-000eef00: 7369 6f6e 6020 6f70 6572 6174 696f 6e20  sion` operation 
-000eef10: 746f 2071 7565 7279 2074 6865 2076 6572  to query the ver
-000eef20: 7369 6f6e 2074 6f20 7768 6963 6820 7468  sion to which th
-000eef30: 6520 636f 6d70 6f6e 656e 7420 6361 6e20  e component can 
-000eef40: 6265 2075 7064 6174 6564 2e0a 2020 2020  be updated..    
-000eef50: 2020 2020 2320 0a20 2020 2020 2020 2023      # .        #
-000eef60: 2054 6869 7320 7061 7261 6d65 7465 7220   This parameter 
-000eef70: 6973 2072 6571 7569 7265 642e 0a20 2020  is required..   
-000eef80: 2020 2020 2073 656c 662e 6e65 7874 5f76       self.next_v
-000eef90: 6572 7369 6f6e 203d 206e 6578 745f 7665  ersion = next_ve
-000eefa0: 7273 696f 6e0a 2020 2020 2020 2020 2320  rsion.        # 
-000eefb0: 5468 6520 7570 6461 7465 2070 6f6c 6963  The update polic
-000eefc0: 792e 2056 616c 6964 2076 616c 7565 733a  y. Valid values:
-000eefd0: 0a20 2020 2020 2020 2023 200a 2020 2020  .        # .    
-000eefe0: 2020 2020 2320 2a20 2020 6f76 6572 7772      # *   overwr
-000eeff0: 6974 650a 2020 2020 2020 2020 2320 2a20  ite.        # * 
-000ef000: 2020 6361 6e61 7279 0a20 2020 2020 2020    canary.       
-000ef010: 2073 656c 662e 706f 6c69 6379 203d 2070   self.policy = p
-000ef020: 6f6c 6963 790a 2020 2020 2020 2020 2320  olicy.        # 
-000ef030: 5468 6520 6375 7272 656e 7420 7665 7273  The current vers
-000ef040: 696f 6e20 6f66 2074 6865 2063 6f6d 706f  ion of the compo
-000ef050: 6e65 6e74 2e0a 2020 2020 2020 2020 7365  nent..        se
-000ef060: 6c66 2e76 6572 7369 6f6e 203d 2076 6572  lf.version = ver
-000ef070: 7369 6f6e 0a0a 2020 2020 6465 6620 7661  sion..    def va
-000ef080: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-000ef090: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000ef0a0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-000ef0b0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-000ef0c0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-000ef0d0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-000ef0e0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-000ef0f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000ef100: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-000ef110: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000ef120: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000ef130: 636f 6d70 6f6e 656e 745f 6e61 6d65 2069  component_name i
-000ef140: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000ef150: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000ef160: 636f 6d70 6f6e 656e 745f 6e61 6d65 275d  component_name']
-000ef170: 203d 2073 656c 662e 636f 6d70 6f6e 656e   = self.componen
-000ef180: 745f 6e61 6d65 0a20 2020 2020 2020 2069  t_name.        i
-000ef190: 6620 7365 6c66 2e63 6f6e 6669 6720 6973  f self.config is
-000ef1a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000ef1b0: 2020 2020 2020 2072 6573 756c 745b 2763         result['c
-000ef1c0: 6f6e 6669 6727 5d20 3d20 7365 6c66 2e63  onfig'] = self.c
-000ef1d0: 6f6e 6669 670a 2020 2020 2020 2020 6966  onfig.        if
-000ef1e0: 2073 656c 662e 6e65 7874 5f76 6572 7369   self.next_versi
-000ef1f0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-000ef200: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000ef210: 6c74 5b27 6e65 7874 5f76 6572 7369 6f6e  lt['next_version
-000ef220: 275d 203d 2073 656c 662e 6e65 7874 5f76  '] = self.next_v
-000ef230: 6572 7369 6f6e 0a20 2020 2020 2020 2069  ersion.        i
-000ef240: 6620 7365 6c66 2e70 6f6c 6963 7920 6973  f self.policy is
-000ef250: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000ef260: 2020 2020 2020 2072 6573 756c 745b 2770         result['p
-000ef270: 6f6c 6963 7927 5d20 3d20 7365 6c66 2e70  olicy'] = self.p
-000ef280: 6f6c 6963 790a 2020 2020 2020 2020 6966  olicy.        if
-000ef290: 2073 656c 662e 7665 7273 696f 6e20 6973   self.version is
-000ef2a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000ef2b0: 2020 2020 2020 2072 6573 756c 745b 2776         result['v
-000ef2c0: 6572 7369 6f6e 275d 203d 2073 656c 662e  ersion'] = self.
-000ef2d0: 7665 7273 696f 6e0a 2020 2020 2020 2020  version.        
-000ef2e0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-000ef2f0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-000ef300: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-000ef310: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-000ef320: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-000ef330: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000ef340: 2763 6f6d 706f 6e65 6e74 5f6e 616d 6527  'component_name'
-000ef350: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000ef360: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000ef370: 636f 6d70 6f6e 656e 745f 6e61 6d65 203d  component_name =
-000ef380: 206d 2e67 6574 2827 636f 6d70 6f6e 656e   m.get('componen
-000ef390: 745f 6e61 6d65 2729 0a20 2020 2020 2020  t_name').       
-000ef3a0: 2069 6620 6d2e 6765 7428 2763 6f6e 6669   if m.get('confi
-000ef3b0: 6727 2920 6973 206e 6f74 204e 6f6e 653a  g') is not None:
-000ef3c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000ef3d0: 662e 636f 6e66 6967 203d 206d 2e67 6574  f.config = m.get
-000ef3e0: 2827 636f 6e66 6967 2729 0a20 2020 2020  ('config').     
-000ef3f0: 2020 2069 6620 6d2e 6765 7428 276e 6578     if m.get('nex
-000ef400: 745f 7665 7273 696f 6e27 2920 6973 206e  t_version') is n
-000ef410: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000ef420: 2020 2020 2073 656c 662e 6e65 7874 5f76       self.next_v
-000ef430: 6572 7369 6f6e 203d 206d 2e67 6574 2827  ersion = m.get('
-000ef440: 6e65 7874 5f76 6572 7369 6f6e 2729 0a20  next_version'). 
-000ef450: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000ef460: 2770 6f6c 6963 7927 2920 6973 206e 6f74  'policy') is not
-000ef470: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000ef480: 2020 2073 656c 662e 706f 6c69 6379 203d     self.policy =
-000ef490: 206d 2e67 6574 2827 706f 6c69 6379 2729   m.get('policy')
-000ef4a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000ef4b0: 7428 2776 6572 7369 6f6e 2729 2069 7320  t('version') is 
-000ef4c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000ef4d0: 2020 2020 2020 7365 6c66 2e76 6572 7369        self.versi
-000ef4e0: 6f6e 203d 206d 2e67 6574 2827 7665 7273  on = m.get('vers
-000ef4f0: 696f 6e27 290a 2020 2020 2020 2020 7265  ion').        re
-000ef500: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000ef510: 7320 5570 6772 6164 6543 6c75 7374 6572  s UpgradeCluster
-000ef520: 4164 646f 6e73 5265 7175 6573 7428 5465  AddonsRequest(Te
-000ef530: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-000ef540: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-000ef550: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000ef560: 2062 6f64 793a 204c 6973 745b 5570 6772   body: List[Upgr
-000ef570: 6164 6543 6c75 7374 6572 4164 646f 6e73  adeClusterAddons
-000ef580: 5265 7175 6573 7442 6f64 795d 203d 204e  RequestBody] = N
-000ef590: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000ef5a0: 2020 2020 2320 5468 6520 7265 7175 6573      # The reques
-000ef5b0: 7420 7061 7261 6d65 7465 7273 2e0a 2020  t parameters..  
-000ef5c0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-000ef5d0: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
-000ef5e0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000ef5f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000ef600: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-000ef610: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-000ef620: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-000ef630: 2020 2020 2020 6966 206b 3a0a 2020 2020        if k:.    
-000ef640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000ef650: 6b2e 7661 6c69 6461 7465 2829 0a0a 2020  k.validate()..  
-000ef660: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000ef670: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-000ef680: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-000ef690: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-000ef6a0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-000ef6b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000ef6c0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-000ef6d0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-000ef6e0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-000ef6f0: 5b27 626f 6479 275d 203d 205b 5d0a 2020  ['body'] = [].  
-000ef700: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-000ef710: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-000ef720: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000ef730: 6b20 696e 2073 656c 662e 626f 6479 3a0a  k in self.body:.
-000ef740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000ef750: 7265 7375 6c74 5b27 626f 6479 275d 2e61  result['body'].a
-000ef760: 7070 656e 6428 6b2e 746f 5f6d 6170 2829  ppend(k.to_map()
-000ef770: 2069 6620 6b20 656c 7365 204e 6f6e 6529   if k else None)
-000ef780: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000ef790: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-000ef7a0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-000ef7b0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-000ef7c0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000ef7d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000ef7e0: 7365 6c66 2e62 6f64 7920 3d20 5b5d 0a20  self.body = []. 
-000ef7f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000ef800: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-000ef810: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000ef820: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
-000ef830: 2762 6f64 7927 293a 0a20 2020 2020 2020  'body'):.       
-000ef840: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000ef850: 6465 6c20 3d20 5570 6772 6164 6543 6c75  del = UpgradeClu
-000ef860: 7374 6572 4164 646f 6e73 5265 7175 6573  sterAddonsReques
-000ef870: 7442 6f64 7928 290a 2020 2020 2020 2020  tBody().        
-000ef880: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-000ef890: 792e 6170 7065 6e64 2874 656d 705f 6d6f  y.append(temp_mo
-000ef8a0: 6465 6c2e 6672 6f6d 5f6d 6170 286b 2929  del.from_map(k))
-000ef8b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000ef8c0: 7365 6c66 0a0a 0a63 6c61 7373 2055 7067  self...class Upg
-000ef8d0: 7261 6465 436c 7573 7465 7241 6464 6f6e  radeClusterAddon
-000ef8e0: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
-000ef8f0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-000ef900: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000ef910: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
-000ef920: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
-000ef930: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-000ef940: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
-000ef950: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-000ef960: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-000ef970: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-000ef980: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-000ef990: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-000ef9a0: 7461 7475 735f 636f 6465 0a0a 2020 2020  tatus_code..    
-000ef9b0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-000ef9c0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-000ef9d0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000ef9e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000ef9f0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000efa00: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000efa10: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-000efa20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000efa30: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000efa40: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000efa50: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000efa60: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-000efa70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000efa80: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-000efa90: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-000efaa0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-000efab0: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-000efac0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-000efad0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000efae0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-000efaf0: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-000efb00: 636f 6465 0a20 2020 2020 2020 2072 6574  code.        ret
-000efb10: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000efb20: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000efb30: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000efb40: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000efb50: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000efb60: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-000efb70: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-000efb80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000efb90: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-000efba0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-000efbb0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000efbc0: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-000efbd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000efbe0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000efbf0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-000efc00: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-000efc10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000efc20: 656c 660a 0a0a 636c 6173 7320 5570 6772  elf...class Upgr
-000efc30: 6164 6543 6c75 7374 6572 4e6f 6465 706f  adeClusterNodepo
-000efc40: 6f6c 5265 7175 6573 7452 6f6c 6c69 6e67  olRequestRolling
-000efc50: 506f 6c69 6379 2854 6561 4d6f 6465 6c29  Policy(TeaModel)
-000efc60: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000efc70: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000efc80: 2c0a 2020 2020 2020 2020 6261 7463 685f  ,.        batch_
-000efc90: 696e 7465 7276 616c 3a20 696e 7420 3d20  interval: int = 
-000efca0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6d61  None,.        ma
-000efcb0: 785f 7061 7261 6c6c 656c 6973 6d3a 2069  x_parallelism: i
-000efcc0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-000efcd0: 2020 2070 6175 7365 5f70 6f6c 6963 793a     pause_policy:
-000efce0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000efcf0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-000efd00: 2e62 6174 6368 5f69 6e74 6572 7661 6c20  .batch_interval 
-000efd10: 3d20 6261 7463 685f 696e 7465 7276 616c  = batch_interval
-000efd20: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
-000efd30: 785f 7061 7261 6c6c 656c 6973 6d20 3d20  x_parallelism = 
-000efd40: 6d61 785f 7061 7261 6c6c 656c 6973 6d0a  max_parallelism.
-000efd50: 2020 2020 2020 2020 7365 6c66 2e70 6175          self.pau
-000efd60: 7365 5f70 6f6c 6963 7920 3d20 7061 7573  se_policy = paus
-000efd70: 655f 706f 6c69 6379 0a0a 2020 2020 6465  e_policy..    de
-000efd80: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000efd90: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-000efda0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000efdb0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000efdc0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000efdd0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000efde0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000efdf0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000efe00: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000efe10: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000efe20: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-000efe30: 656c 662e 6261 7463 685f 696e 7465 7276  elf.batch_interv
-000efe40: 616c 2069 7320 6e6f 7420 4e6f 6e65 3a0a  al is not None:.
-000efe50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000efe60: 6c74 5b27 6261 7463 685f 696e 7465 7276  lt['batch_interv
-000efe70: 616c 275d 203d 2073 656c 662e 6261 7463  al'] = self.batc
-000efe80: 685f 696e 7465 7276 616c 0a20 2020 2020  h_interval.     
-000efe90: 2020 2069 6620 7365 6c66 2e6d 6178 5f70     if self.max_p
-000efea0: 6172 616c 6c65 6c69 736d 2069 7320 6e6f  arallelism is no
-000efeb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000efec0: 2020 2020 7265 7375 6c74 5b27 6d61 785f      result['max_
-000efed0: 7061 7261 6c6c 656c 6973 6d27 5d20 3d20  parallelism'] = 
-000efee0: 7365 6c66 2e6d 6178 5f70 6172 616c 6c65  self.max_paralle
-000efef0: 6c69 736d 0a20 2020 2020 2020 2069 6620  lism.        if 
-000eff00: 7365 6c66 2e70 6175 7365 5f70 6f6c 6963  self.pause_polic
-000eff10: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-000eff20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000eff30: 745b 2770 6175 7365 5f70 6f6c 6963 7927  t['pause_policy'
-000eff40: 5d20 3d20 7365 6c66 2e70 6175 7365 5f70  ] = self.pause_p
-000eff50: 6f6c 6963 790a 2020 2020 2020 2020 7265  olicy.        re
-000eff60: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-000eff70: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-000eff80: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-000eff90: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-000effa0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-000effb0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-000effc0: 6174 6368 5f69 6e74 6572 7661 6c27 2920  atch_interval') 
-000effd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000effe0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
-000efff0: 7463 685f 696e 7465 7276 616c 203d 206d  tch_interval = m
-000f0000: 2e67 6574 2827 6261 7463 685f 696e 7465  .get('batch_inte
-000f0010: 7276 616c 2729 0a20 2020 2020 2020 2069  rval').        i
-000f0020: 6620 6d2e 6765 7428 276d 6178 5f70 6172  f m.get('max_par
-000f0030: 616c 6c65 6c69 736d 2729 2069 7320 6e6f  allelism') is no
-000f0040: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000f0050: 2020 2020 7365 6c66 2e6d 6178 5f70 6172      self.max_par
-000f0060: 616c 6c65 6c69 736d 203d 206d 2e67 6574  allelism = m.get
-000f0070: 2827 6d61 785f 7061 7261 6c6c 656c 6973  ('max_parallelis
-000f0080: 6d27 290a 2020 2020 2020 2020 6966 206d  m').        if m
-000f0090: 2e67 6574 2827 7061 7573 655f 706f 6c69  .get('pause_poli
-000f00a0: 6379 2729 2069 7320 6e6f 7420 4e6f 6e65  cy') is not None
-000f00b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000f00c0: 6c66 2e70 6175 7365 5f70 6f6c 6963 7920  lf.pause_policy 
-000f00d0: 3d20 6d2e 6765 7428 2770 6175 7365 5f70  = m.get('pause_p
-000f00e0: 6f6c 6963 7927 290a 2020 2020 2020 2020  olicy').        
-000f00f0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-000f0100: 6173 7320 5570 6772 6164 6543 6c75 7374  ass UpgradeClust
-000f0110: 6572 4e6f 6465 706f 6f6c 5265 7175 6573  erNodepoolReques
-000f0120: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
-000f0130: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-000f0140: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000f0150: 2020 2020 2069 6d61 6765 5f69 643a 2073       image_id: s
-000f0160: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000f0170: 2020 206b 7562 6572 6e65 7465 735f 7665     kubernetes_ve
-000f0180: 7273 696f 6e3a 2073 7472 203d 204e 6f6e  rsion: str = Non
-000f0190: 652c 0a20 2020 2020 2020 206e 6f64 655f  e,.        node_
-000f01a0: 6e61 6d65 733a 204c 6973 745b 7374 725d  names: List[str]
-000f01b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000f01c0: 2072 6f6c 6c69 6e67 5f70 6f6c 6963 793a   rolling_policy:
-000f01d0: 2055 7067 7261 6465 436c 7573 7465 724e   UpgradeClusterN
-000f01e0: 6f64 6570 6f6f 6c52 6571 7565 7374 526f  odepoolRequestRo
-000f01f0: 6c6c 696e 6750 6f6c 6963 7920 3d20 4e6f  llingPolicy = No
-000f0200: 6e65 2c0a 2020 2020 2020 2020 7275 6e74  ne,.        runt
-000f0210: 696d 655f 7479 7065 3a20 7374 7220 3d20  ime_type: str = 
-000f0220: 4e6f 6e65 2c0a 2020 2020 2020 2020 7275  None,.        ru
-000f0230: 6e74 696d 655f 7665 7273 696f 6e3a 2073  ntime_version: s
-000f0240: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000f0250: 2020 2075 7365 5f72 6570 6c61 6365 3a20     use_replace: 
-000f0260: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
-000f0270: 2029 3a0a 2020 2020 2020 2020 2320 5468   ):.        # Th
-000f0280: 6520 4944 206f 6620 7468 6520 4f53 2069  e ID of the OS i
-000f0290: 6d61 6765 2074 6861 7420 6973 2075 7365  mage that is use
-000f02a0: 6420 6279 2074 6865 206e 6f64 6573 2e0a  d by the nodes..
-000f02b0: 2020 2020 2020 2020 7365 6c66 2e69 6d61          self.ima
-000f02c0: 6765 5f69 6420 3d20 696d 6167 655f 6964  ge_id = image_id
-000f02d0: 0a20 2020 2020 2020 2023 2054 6865 204b  .        # The K
-000f02e0: 7562 6572 6e65 7465 7320 7665 7273 696f  ubernetes versio
-000f02f0: 6e20 7468 6174 2069 7320 7573 6564 2062  n that is used b
-000f0300: 7920 7468 6520 6e6f 6465 732e 0a20 2020  y the nodes..   
-000f0310: 2020 2020 2073 656c 662e 6b75 6265 726e       self.kubern
-000f0320: 6574 6573 5f76 6572 7369 6f6e 203d 206b  etes_version = k
-000f0330: 7562 6572 6e65 7465 735f 7665 7273 696f  ubernetes_versio
-000f0340: 6e0a 2020 2020 2020 2020 7365 6c66 2e6e  n.        self.n
-000f0350: 6f64 655f 6e61 6d65 7320 3d20 6e6f 6465  ode_names = node
-000f0360: 5f6e 616d 6573 0a20 2020 2020 2020 2073  _names.        s
-000f0370: 656c 662e 726f 6c6c 696e 675f 706f 6c69  elf.rolling_poli
-000f0380: 6379 203d 2072 6f6c 6c69 6e67 5f70 6f6c  cy = rolling_pol
-000f0390: 6963 790a 2020 2020 2020 2020 2320 5468  icy.        # Th
-000f03a0: 6520 7275 6e74 696d 6520 7479 7065 2e20  e runtime type. 
-000f03b0: 5661 6c69 6420 7661 6c75 6573 3a20 636f  Valid values: co
-000f03c0: 6e74 6169 6e65 7264 2061 6e64 2064 6f63  ntainerd and doc
-000f03d0: 6b65 722e 0a20 2020 2020 2020 2073 656c  ker..        sel
-000f03e0: 662e 7275 6e74 696d 655f 7479 7065 203d  f.runtime_type =
-000f03f0: 2072 756e 7469 6d65 5f74 7970 650a 2020   runtime_type.  
-000f0400: 2020 2020 2020 2320 5468 6520 7665 7273        # The vers
-000f0410: 696f 6e20 6f66 2074 6865 2063 6f6e 7461  ion of the conta
-000f0420: 696e 6572 2072 756e 7469 6d65 2074 6861  iner runtime tha
-000f0430: 7420 6973 2075 7365 6420 6279 2074 6865  t is used by the
-000f0440: 206e 6f64 6573 2e0a 2020 2020 2020 2020   nodes..        
-000f0450: 7365 6c66 2e72 756e 7469 6d65 5f76 6572  self.runtime_ver
-000f0460: 7369 6f6e 203d 2072 756e 7469 6d65 5f76  sion = runtime_v
-000f0470: 6572 7369 6f6e 0a20 2020 2020 2020 2073  ersion.        s
-000f0480: 656c 662e 7573 655f 7265 706c 6163 6520  elf.use_replace 
-000f0490: 3d20 7573 655f 7265 706c 6163 650a 0a20  = use_replace.. 
-000f04a0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-000f04b0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-000f04c0: 6620 7365 6c66 2e72 6f6c 6c69 6e67 5f70  f self.rolling_p
-000f04d0: 6f6c 6963 793a 0a20 2020 2020 2020 2020  olicy:.         
-000f04e0: 2020 2073 656c 662e 726f 6c6c 696e 675f     self.rolling_
-000f04f0: 706f 6c69 6379 2e76 616c 6964 6174 6528  policy.validate(
-000f0500: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000f0510: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000f0520: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000f0530: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000f0540: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000f0550: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000f0560: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000f0570: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000f0580: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000f0590: 6620 7365 6c66 2e69 6d61 6765 5f69 6420  f self.image_id 
-000f05a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000f05b0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000f05c0: 2769 6d61 6765 5f69 6427 5d20 3d20 7365  'image_id'] = se
-000f05d0: 6c66 2e69 6d61 6765 5f69 640a 2020 2020  lf.image_id.    
-000f05e0: 2020 2020 6966 2073 656c 662e 6b75 6265      if self.kube
-000f05f0: 726e 6574 6573 5f76 6572 7369 6f6e 2069  rnetes_version i
-000f0600: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000f0610: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000f0620: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
-000f0630: 6f6e 275d 203d 2073 656c 662e 6b75 6265  on'] = self.kube
-000f0640: 726e 6574 6573 5f76 6572 7369 6f6e 0a20  rnetes_version. 
-000f0650: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-000f0660: 6f64 655f 6e61 6d65 7320 6973 206e 6f74  ode_names is not
-000f0670: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000f0680: 2020 2072 6573 756c 745b 276e 6f64 655f     result['node_
-000f0690: 6e61 6d65 7327 5d20 3d20 7365 6c66 2e6e  names'] = self.n
-000f06a0: 6f64 655f 6e61 6d65 730a 2020 2020 2020  ode_names.      
-000f06b0: 2020 6966 2073 656c 662e 726f 6c6c 696e    if self.rollin
-000f06c0: 675f 706f 6c69 6379 2069 7320 6e6f 7420  g_policy is not 
-000f06d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000f06e0: 2020 7265 7375 6c74 5b27 726f 6c6c 696e    result['rollin
-000f06f0: 675f 706f 6c69 6379 275d 203d 2073 656c  g_policy'] = sel
-000f0700: 662e 726f 6c6c 696e 675f 706f 6c69 6379  f.rolling_policy
-000f0710: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-000f0720: 2020 6966 2073 656c 662e 7275 6e74 696d    if self.runtim
-000f0730: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
-000f0740: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000f0750: 7265 7375 6c74 5b27 7275 6e74 696d 655f  result['runtime_
-000f0760: 7479 7065 275d 203d 2073 656c 662e 7275  type'] = self.ru
-000f0770: 6e74 696d 655f 7479 7065 0a20 2020 2020  ntime_type.     
-000f0780: 2020 2069 6620 7365 6c66 2e72 756e 7469     if self.runti
-000f0790: 6d65 5f76 6572 7369 6f6e 2069 7320 6e6f  me_version is no
-000f07a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000f07b0: 2020 2020 7265 7375 6c74 5b27 7275 6e74      result['runt
-000f07c0: 696d 655f 7665 7273 696f 6e27 5d20 3d20  ime_version'] = 
-000f07d0: 7365 6c66 2e72 756e 7469 6d65 5f76 6572  self.runtime_ver
-000f07e0: 7369 6f6e 0a20 2020 2020 2020 2069 6620  sion.        if 
-000f07f0: 7365 6c66 2e75 7365 5f72 6570 6c61 6365  self.use_replace
-000f0800: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000f0810: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000f0820: 5b27 7573 655f 7265 706c 6163 6527 5d20  ['use_replace'] 
-000f0830: 3d20 7365 6c66 2e75 7365 5f72 6570 6c61  = self.use_repla
-000f0840: 6365 0a20 2020 2020 2020 2072 6574 7572  ce.        retur
-000f0850: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000f0860: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000f0870: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000f0880: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000f0890: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000f08a0: 2020 6966 206d 2e67 6574 2827 696d 6167    if m.get('imag
-000f08b0: 655f 6964 2729 2069 7320 6e6f 7420 4e6f  e_id') is not No
-000f08c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000f08d0: 7365 6c66 2e69 6d61 6765 5f69 6420 3d20  self.image_id = 
-000f08e0: 6d2e 6765 7428 2769 6d61 6765 5f69 6427  m.get('image_id'
-000f08f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000f0900: 6574 2827 6b75 6265 726e 6574 6573 5f76  et('kubernetes_v
-000f0910: 6572 7369 6f6e 2729 2069 7320 6e6f 7420  ersion') is not 
-000f0920: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000f0930: 2020 7365 6c66 2e6b 7562 6572 6e65 7465    self.kubernete
-000f0940: 735f 7665 7273 696f 6e20 3d20 6d2e 6765  s_version = m.ge
-000f0950: 7428 276b 7562 6572 6e65 7465 735f 7665  t('kubernetes_ve
-000f0960: 7273 696f 6e27 290a 2020 2020 2020 2020  rsion').        
-000f0970: 6966 206d 2e67 6574 2827 6e6f 6465 5f6e  if m.get('node_n
-000f0980: 616d 6573 2729 2069 7320 6e6f 7420 4e6f  ames') is not No
-000f0990: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000f09a0: 7365 6c66 2e6e 6f64 655f 6e61 6d65 7320  self.node_names 
-000f09b0: 3d20 6d2e 6765 7428 276e 6f64 655f 6e61  = m.get('node_na
-000f09c0: 6d65 7327 290a 2020 2020 2020 2020 6966  mes').        if
-000f09d0: 206d 2e67 6574 2827 726f 6c6c 696e 675f   m.get('rolling_
-000f09e0: 706f 6c69 6379 2729 2069 7320 6e6f 7420  policy') is not 
-000f09f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000f0a00: 2020 7465 6d70 5f6d 6f64 656c 203d 2055    temp_model = U
-000f0a10: 7067 7261 6465 436c 7573 7465 724e 6f64  pgradeClusterNod
-000f0a20: 6570 6f6f 6c52 6571 7565 7374 526f 6c6c  epoolRequestRoll
-000f0a30: 696e 6750 6f6c 6963 7928 290a 2020 2020  ingPolicy().    
-000f0a40: 2020 2020 2020 2020 7365 6c66 2e72 6f6c          self.rol
-000f0a50: 6c69 6e67 5f70 6f6c 6963 7920 3d20 7465  ling_policy = te
-000f0a60: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-000f0a70: 7028 6d5b 2772 6f6c 6c69 6e67 5f70 6f6c  p(m['rolling_pol
-000f0a80: 6963 7927 5d29 0a20 2020 2020 2020 2069  icy']).        i
-000f0a90: 6620 6d2e 6765 7428 2772 756e 7469 6d65  f m.get('runtime
-000f0aa0: 5f74 7970 6527 2920 6973 206e 6f74 204e  _type') is not N
-000f0ab0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000f0ac0: 2073 656c 662e 7275 6e74 696d 655f 7479   self.runtime_ty
-000f0ad0: 7065 203d 206d 2e67 6574 2827 7275 6e74  pe = m.get('runt
-000f0ae0: 696d 655f 7479 7065 2729 0a20 2020 2020  ime_type').     
-000f0af0: 2020 2069 6620 6d2e 6765 7428 2772 756e     if m.get('run
-000f0b00: 7469 6d65 5f76 6572 7369 6f6e 2729 2069  time_version') i
-000f0b10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000f0b20: 2020 2020 2020 2020 7365 6c66 2e72 756e          self.run
-000f0b30: 7469 6d65 5f76 6572 7369 6f6e 203d 206d  time_version = m
-000f0b40: 2e67 6574 2827 7275 6e74 696d 655f 7665  .get('runtime_ve
-000f0b50: 7273 696f 6e27 290a 2020 2020 2020 2020  rsion').        
-000f0b60: 6966 206d 2e67 6574 2827 7573 655f 7265  if m.get('use_re
-000f0b70: 706c 6163 6527 2920 6973 206e 6f74 204e  place') is not N
-000f0b80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000f0b90: 2073 656c 662e 7573 655f 7265 706c 6163   self.use_replac
-000f0ba0: 6520 3d20 6d2e 6765 7428 2775 7365 5f72  e = m.get('use_r
-000f0bb0: 6570 6c61 6365 2729 0a20 2020 2020 2020  eplace').       
-000f0bc0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-000f0bd0: 6c61 7373 2055 7067 7261 6465 436c 7573  lass UpgradeClus
-000f0be0: 7465 724e 6f64 6570 6f6f 6c52 6573 706f  terNodepoolRespo
-000f0bf0: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
-000f0c00: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-000f0c10: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000f0c20: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
-000f0c30: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
-000f0c40: 652c 0a20 2020 2020 2020 2074 6173 6b5f  e,.        task_
-000f0c50: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-000f0c60: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
-000f0c70: 2054 6865 2072 6571 7565 7374 2049 442e   The request ID.
-000f0c80: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000f0c90: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
-000f0ca0: 7374 5f69 640a 2020 2020 2020 2020 2320  st_id.        # 
-000f0cb0: 5468 6520 7461 736b 2049 442e 0a20 2020  The task ID..   
-000f0cc0: 2020 2020 2073 656c 662e 7461 736b 5f69       self.task_i
-000f0cd0: 6420 3d20 7461 736b 5f69 640a 0a20 2020  d = task_id..   
-000f0ce0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000f0cf0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-000f0d00: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-000f0d10: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000f0d20: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000f0d30: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000f0d40: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000f0d50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000f0d60: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000f0d70: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000f0d80: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000f0d90: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
-000f0da0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000f0db0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000f0dc0: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
-000f0dd0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-000f0de0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000f0df0: 2e74 6173 6b5f 6964 2069 7320 6e6f 7420  .task_id is not 
-000f0e00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000f0e10: 2020 7265 7375 6c74 5b27 7461 736b 5f69    result['task_i
-000f0e20: 6427 5d20 3d20 7365 6c66 2e74 6173 6b5f  d'] = self.task_
-000f0e30: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-000f0e40: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000f0e50: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000f0e60: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-000f0e70: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-000f0e80: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-000f0e90: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
-000f0ea0: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
-000f0eb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000f0ec0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-000f0ed0: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
-000f0ee0: 7449 6427 290a 2020 2020 2020 2020 6966  tId').        if
-000f0ef0: 206d 2e67 6574 2827 7461 736b 5f69 6427   m.get('task_id'
-000f0f00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000f0f10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000f0f20: 7461 736b 5f69 6420 3d20 6d2e 6765 7428  task_id = m.get(
-000f0f30: 2774 6173 6b5f 6964 2729 0a20 2020 2020  'task_id').     
-000f0f40: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-000f0f50: 0a63 6c61 7373 2055 7067 7261 6465 436c  .class UpgradeCl
-000f0f60: 7573 7465 724e 6f64 6570 6f6f 6c52 6573  usterNodepoolRes
-000f0f70: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-000f0f80: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000f0f90: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-000f0fa0: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-000f0fb0: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-000f0fc0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000f0fd0: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-000f0fe0: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-000f0ff0: 2020 626f 6479 3a20 5570 6772 6164 6543    body: UpgradeC
-000f1000: 6c75 7374 6572 4e6f 6465 706f 6f6c 5265  lusterNodepoolRe
-000f1010: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
-000f1020: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-000f1030: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-000f1040: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-000f1050: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000f1060: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-000f1070: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-000f1080: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-000f1090: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000f10a0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-000f10b0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-000f10c0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-000f10d0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-000f10e0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-000f10f0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-000f1100: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-000f1110: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-000f1120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000f1130: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000f1140: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-000f1150: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-000f1160: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-000f1170: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-000f1180: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000f1190: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-000f11a0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-000f11b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000f11c0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-000f11d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000f11e0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-000f11f0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-000f1200: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-000f1210: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-000f1220: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-000f1230: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000f1240: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-000f1250: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-000f1260: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000f1270: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000f1280: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000f1290: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000f12a0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000f12b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000f12c0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-000f12d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000f12e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000f12f0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-000f1300: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-000f1310: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-000f1320: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-000f1330: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000f1340: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-000f1350: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-000f1360: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-000f1370: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-000f1380: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000f1390: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000f13a0: 5f6d 6f64 656c 203d 2055 7067 7261 6465  _model = Upgrade
-000f13b0: 436c 7573 7465 724e 6f64 6570 6f6f 6c52  ClusterNodepoolR
-000f13c0: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
-000f13d0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000f13e0: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-000f13f0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-000f1400: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-000f1410: 7572 6e20 7365 6c66 0a0a 0a              urn self...
+000ed650: 2020 2020 2020 7265 7375 6c74 5b27 6973        result['is
+000ed660: 5f63 7573 746f 6d27 5d20 3d20 7365 6c66  _custom'] = self
+000ed670: 2e69 735f 6375 7374 6f6d 0a20 2020 2020  .is_custom.     
+000ed680: 2020 2069 6620 7365 6c66 2e69 735f 7261     if self.is_ra
+000ed690: 6d5f 726f 6c65 2069 7320 6e6f 7420 4e6f  m_role is not No
+000ed6a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ed6b0: 7265 7375 6c74 5b27 6973 5f72 616d 5f72  result['is_ram_r
+000ed6c0: 6f6c 6527 5d20 3d20 7365 6c66 2e69 735f  ole'] = self.is_
+000ed6d0: 7261 6d5f 726f 6c65 0a20 2020 2020 2020  ram_role.       
+000ed6e0: 2069 6620 7365 6c66 2e6e 616d 6573 7061   if self.namespa
+000ed6f0: 6365 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ce is not None:.
+000ed700: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000ed710: 6c74 5b27 6e61 6d65 7370 6163 6527 5d20  lt['namespace'] 
+000ed720: 3d20 7365 6c66 2e6e 616d 6573 7061 6365  = self.namespace
+000ed730: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000ed740: 2e72 6f6c 655f 6e61 6d65 2069 7320 6e6f  .role_name is no
+000ed750: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000ed760: 2020 2020 7265 7375 6c74 5b27 726f 6c65      result['role
+000ed770: 5f6e 616d 6527 5d20 3d20 7365 6c66 2e72  _name'] = self.r
+000ed780: 6f6c 655f 6e61 6d65 0a20 2020 2020 2020  ole_name.       
+000ed790: 2069 6620 7365 6c66 2e72 6f6c 655f 7479   if self.role_ty
+000ed7a0: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
+000ed7b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000ed7c0: 6c74 5b27 726f 6c65 5f74 7970 6527 5d20  lt['role_type'] 
+000ed7d0: 3d20 7365 6c66 2e72 6f6c 655f 7479 7065  = self.role_type
+000ed7e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000ed7f0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000ed800: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000ed810: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000ed820: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000ed830: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000ed840: 6966 206d 2e67 6574 2827 636c 7573 7465  if m.get('cluste
+000ed850: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
+000ed860: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000ed870: 662e 636c 7573 7465 7220 3d20 6d2e 6765  f.cluster = m.ge
+000ed880: 7428 2763 6c75 7374 6572 2729 0a20 2020  t('cluster').   
+000ed890: 2020 2020 2069 6620 6d2e 6765 7428 2769       if m.get('i
+000ed8a0: 735f 6375 7374 6f6d 2729 2069 7320 6e6f  s_custom') is no
+000ed8b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000ed8c0: 2020 2020 7365 6c66 2e69 735f 6375 7374      self.is_cust
+000ed8d0: 6f6d 203d 206d 2e67 6574 2827 6973 5f63  om = m.get('is_c
+000ed8e0: 7573 746f 6d27 290a 2020 2020 2020 2020  ustom').        
+000ed8f0: 6966 206d 2e67 6574 2827 6973 5f72 616d  if m.get('is_ram
+000ed900: 5f72 6f6c 6527 2920 6973 206e 6f74 204e  _role') is not N
+000ed910: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ed920: 2073 656c 662e 6973 5f72 616d 5f72 6f6c   self.is_ram_rol
+000ed930: 6520 3d20 6d2e 6765 7428 2769 735f 7261  e = m.get('is_ra
+000ed940: 6d5f 726f 6c65 2729 0a20 2020 2020 2020  m_role').       
+000ed950: 2069 6620 6d2e 6765 7428 276e 616d 6573   if m.get('names
+000ed960: 7061 6365 2729 2069 7320 6e6f 7420 4e6f  pace') is not No
+000ed970: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ed980: 7365 6c66 2e6e 616d 6573 7061 6365 203d  self.namespace =
+000ed990: 206d 2e67 6574 2827 6e61 6d65 7370 6163   m.get('namespac
+000ed9a0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+000ed9b0: 2e67 6574 2827 726f 6c65 5f6e 616d 6527  .get('role_name'
+000ed9c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000ed9d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000ed9e0: 726f 6c65 5f6e 616d 6520 3d20 6d2e 6765  role_name = m.ge
+000ed9f0: 7428 2772 6f6c 655f 6e61 6d65 2729 0a20  t('role_name'). 
+000eda00: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000eda10: 2772 6f6c 655f 7479 7065 2729 2069 7320  'role_type') is 
+000eda20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000eda30: 2020 2020 2020 7365 6c66 2e72 6f6c 655f        self.role_
+000eda40: 7479 7065 203d 206d 2e67 6574 2827 726f  type = m.get('ro
+000eda50: 6c65 5f74 7970 6527 290a 2020 2020 2020  le_type').      
+000eda60: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+000eda70: 636c 6173 7320 5570 6461 7465 5573 6572  class UpdateUser
+000eda80: 5065 726d 6973 7369 6f6e 7352 6571 7565  PermissionsReque
+000eda90: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+000edaa0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000edab0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000edac0: 2020 2020 2020 626f 6479 3a20 4c69 7374        body: List
+000edad0: 5b55 7064 6174 6555 7365 7250 6572 6d69  [UpdateUserPermi
+000edae0: 7373 696f 6e73 5265 7175 6573 7442 6f64  ssionsRequestBod
+000edaf0: 795d 203d 204e 6f6e 652c 0a20 2020 2020  y] = None,.     
+000edb00: 2020 206d 6f64 653a 2073 7472 203d 204e     mode: str = N
+000edb10: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+000edb20: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+000edb30: 626f 6479 0a20 2020 2020 2020 2073 656c  body.        sel
+000edb40: 662e 6d6f 6465 203d 206d 6f64 650a 0a20  f.mode = mode.. 
+000edb50: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+000edb60: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+000edb70: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+000edb80: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+000edb90: 6e20 7365 6c66 2e62 6f64 793a 0a20 2020  n self.body:.   
+000edba0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000edbb0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+000edbc0: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
+000edbd0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+000edbe0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+000edbf0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000edc00: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+000edc10: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+000edc20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000edc30: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000edc40: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000edc50: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000edc60: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+000edc70: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
+000edc80: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+000edc90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000edca0: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
+000edcb0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+000edcc0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+000edcd0: 6f64 7927 5d2e 6170 7065 6e64 286b 2e74  ody'].append(k.t
+000edce0: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
+000edcf0: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
+000edd00: 6966 2073 656c 662e 6d6f 6465 2069 7320  if self.mode is 
+000edd10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000edd20: 2020 2020 2020 7265 7375 6c74 5b27 6d6f        result['mo
+000edd30: 6465 275d 203d 2073 656c 662e 6d6f 6465  de'] = self.mode
+000edd40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000edd50: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000edd60: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000edd70: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000edd80: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000edd90: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000edda0: 7365 6c66 2e62 6f64 7920 3d20 5b5d 0a20  self.body = []. 
+000eddb0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000eddc0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+000eddd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000edde0: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
+000eddf0: 2762 6f64 7927 293a 0a20 2020 2020 2020  'body'):.       
+000ede00: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+000ede10: 6465 6c20 3d20 5570 6461 7465 5573 6572  del = UpdateUser
+000ede20: 5065 726d 6973 7369 6f6e 7352 6571 7565  PermissionsReque
+000ede30: 7374 426f 6479 2829 0a20 2020 2020 2020  stBody().       
+000ede40: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000ede50: 6479 2e61 7070 656e 6428 7465 6d70 5f6d  dy.append(temp_m
+000ede60: 6f64 656c 2e66 726f 6d5f 6d61 7028 6b29  odel.from_map(k)
+000ede70: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000ede80: 6574 2827 6d6f 6465 2729 2069 7320 6e6f  et('mode') is no
+000ede90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000edea0: 2020 2020 7365 6c66 2e6d 6f64 6520 3d20      self.mode = 
+000edeb0: 6d2e 6765 7428 276d 6f64 6527 290a 2020  m.get('mode').  
+000edec0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000eded0: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
+000edee0: 5573 6572 5065 726d 6973 7369 6f6e 7352  UserPermissionsR
+000edef0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+000edf00: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000edf10: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000edf20: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
+000edf30: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
+000edf40: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+000edf50: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
+000edf60: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+000edf70: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000edf80: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+000edf90: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+000edfa0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+000edfb0: 7475 735f 636f 6465 0a0a 2020 2020 6465  tus_code..    de
+000edfc0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000edfd0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000edfe0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000edff0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000ee000: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000ee010: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000ee020: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000ee030: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000ee040: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000ee050: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000ee060: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000ee070: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+000ee080: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000ee090: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+000ee0a0: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+000ee0b0: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000ee0c0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000ee0d0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000ee0e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000ee0f0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000ee100: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000ee110: 6465 0a20 2020 2020 2020 2072 6574 7572  de.        retur
+000ee120: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000ee130: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000ee140: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+000ee150: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000ee160: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+000ee170: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+000ee180: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+000ee190: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000ee1a0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000ee1b0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000ee1c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000ee1d0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+000ee1e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000ee1f0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000ee200: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+000ee210: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+000ee220: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000ee230: 660a 0a0a 636c 6173 7320 5570 6772 6164  f...class Upgrad
+000ee240: 6543 6c75 7374 6572 5265 7175 6573 7428  eClusterRequest(
+000ee250: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+000ee260: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000ee270: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000ee280: 2020 2063 6f6d 706f 6e65 6e74 5f6e 616d     component_nam
+000ee290: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+000ee2a0: 2020 2020 2020 206d 6173 7465 725f 6f6e         master_on
+000ee2b0: 6c79 3a20 626f 6f6c 203d 204e 6f6e 652c  ly: bool = None,
+000ee2c0: 0a20 2020 2020 2020 206e 6578 745f 7665  .        next_ve
+000ee2d0: 7273 696f 6e3a 2073 7472 203d 204e 6f6e  rsion: str = Non
+000ee2e0: 652c 0a20 2020 2020 2020 2076 6572 7369  e,.        versi
+000ee2f0: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+000ee300: 2020 2020 293a 0a20 2020 2020 2020 2023      ):.        #
+000ee310: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+000ee320: 2063 6f6d 706f 6e65 6e74 2e20 5365 7420   component. Set 
+000ee330: 7468 6520 7661 6c75 6520 746f 2060 6b38  the value to `k8
+000ee340: 7360 2e0a 2020 2020 2020 2020 7365 6c66  s`..        self
+000ee350: 2e63 6f6d 706f 6e65 6e74 5f6e 616d 6520  .component_name 
+000ee360: 3d20 636f 6d70 6f6e 656e 745f 6e61 6d65  = component_name
+000ee370: 0a20 2020 2020 2020 2023 2053 7065 6369  .        # Speci
+000ee380: 6669 6573 2077 6865 7468 6572 2074 6f20  fies whether to 
+000ee390: 7570 6461 7465 206f 6e6c 7920 6d61 7374  update only mast
+000ee3a0: 6572 206e 6f64 6573 2e20 5661 6c69 6420  er nodes. Valid 
+000ee3b0: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+000ee3c0: 2320 0a20 2020 2020 2020 2023 202a 2020  # .        # *  
+000ee3d0: 2074 7275 653a 2075 7064 6174 6520 6f6e   true: update on
+000ee3e0: 6c79 206d 6173 7465 7220 6e6f 6465 732e  ly master nodes.
+000ee3f0: 0a20 2020 2020 2020 2023 202a 2020 2066  .        # *   f
+000ee400: 616c 7365 3a20 7570 6461 7465 206d 6173  alse: update mas
+000ee410: 7465 7220 616e 6420 776f 726b 6572 206e  ter and worker n
+000ee420: 6f64 6573 2e0a 2020 2020 2020 2020 7365  odes..        se
+000ee430: 6c66 2e6d 6173 7465 725f 6f6e 6c79 203d  lf.master_only =
+000ee440: 206d 6173 7465 725f 6f6e 6c79 0a20 2020   master_only.   
+000ee450: 2020 2020 2023 2054 6865 204b 7562 6572       # The Kuber
+000ee460: 6e65 7465 7320 7665 7273 696f 6e20 746f  netes version to
+000ee470: 2077 6869 6368 2074 6865 2063 6c75 7374   which the clust
+000ee480: 6572 2063 616e 2062 6520 7570 6461 7465  er can be update
+000ee490: 642e 0a20 2020 2020 2020 2073 656c 662e  d..        self.
+000ee4a0: 6e65 7874 5f76 6572 7369 6f6e 203d 206e  next_version = n
+000ee4b0: 6578 745f 7665 7273 696f 6e0a 2020 2020  ext_version.    
+000ee4c0: 2020 2020 2320 5468 6520 6375 7272 656e      # The curren
+000ee4d0: 7420 4b75 6265 726e 6574 6573 2076 6572  t Kubernetes ver
+000ee4e0: 7369 6f6e 206f 6620 7468 6520 636c 7573  sion of the clus
+000ee4f0: 7465 722e 2046 6f72 206d 6f72 6520 696e  ter. For more in
+000ee500: 666f 726d 6174 696f 6e2c 2073 6565 205b  formation, see [
+000ee510: 4b75 6265 726e 6574 6573 2076 6572 7369  Kubernetes versi
+000ee520: 6f6e 735d 2868 7474 7073 3a2f 2f68 656c  ons](https://hel
+000ee530: 702e 616c 6979 756e 2e63 6f6d 2f64 6f63  p.aliyun.com/doc
+000ee540: 756d 656e 745f 6465 7461 696c 2f31 3835  ument_detail/185
+000ee550: 3236 392e 6874 6d6c 292e 0a20 2020 2020  269.html)..     
+000ee560: 2020 2073 656c 662e 7665 7273 696f 6e20     self.version 
+000ee570: 3d20 7665 7273 696f 6e0a 0a20 2020 2064  = version..    d
+000ee580: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+000ee590: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+000ee5a0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000ee5b0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000ee5c0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000ee5d0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000ee5e0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000ee5f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ee600: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000ee610: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000ee620: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000ee630: 7365 6c66 2e63 6f6d 706f 6e65 6e74 5f6e  self.component_n
+000ee640: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+000ee650: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000ee660: 756c 745b 2763 6f6d 706f 6e65 6e74 5f6e  ult['component_n
+000ee670: 616d 6527 5d20 3d20 7365 6c66 2e63 6f6d  ame'] = self.com
+000ee680: 706f 6e65 6e74 5f6e 616d 650a 2020 2020  ponent_name.    
+000ee690: 2020 2020 6966 2073 656c 662e 6d61 7374      if self.mast
+000ee6a0: 6572 5f6f 6e6c 7920 6973 206e 6f74 204e  er_only is not N
+000ee6b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000ee6c0: 2072 6573 756c 745b 276d 6173 7465 725f   result['master_
+000ee6d0: 6f6e 6c79 275d 203d 2073 656c 662e 6d61  only'] = self.ma
+000ee6e0: 7374 6572 5f6f 6e6c 790a 2020 2020 2020  ster_only.      
+000ee6f0: 2020 6966 2073 656c 662e 6e65 7874 5f76    if self.next_v
+000ee700: 6572 7369 6f6e 2069 7320 6e6f 7420 4e6f  ersion is not No
+000ee710: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ee720: 7265 7375 6c74 5b27 6e65 7874 5f76 6572  result['next_ver
+000ee730: 7369 6f6e 275d 203d 2073 656c 662e 6e65  sion'] = self.ne
+000ee740: 7874 5f76 6572 7369 6f6e 0a20 2020 2020  xt_version.     
+000ee750: 2020 2069 6620 7365 6c66 2e76 6572 7369     if self.versi
+000ee760: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+000ee770: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000ee780: 6c74 5b27 7665 7273 696f 6e27 5d20 3d20  lt['version'] = 
+000ee790: 7365 6c66 2e76 6572 7369 6f6e 0a20 2020  self.version.   
+000ee7a0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000ee7b0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000ee7c0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+000ee7d0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+000ee7e0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+000ee7f0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+000ee800: 2e67 6574 2827 636f 6d70 6f6e 656e 745f  .get('component_
+000ee810: 6e61 6d65 2729 2069 7320 6e6f 7420 4e6f  name') is not No
+000ee820: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000ee830: 7365 6c66 2e63 6f6d 706f 6e65 6e74 5f6e  self.component_n
+000ee840: 616d 6520 3d20 6d2e 6765 7428 2763 6f6d  ame = m.get('com
+000ee850: 706f 6e65 6e74 5f6e 616d 6527 290a 2020  ponent_name').  
+000ee860: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000ee870: 6d61 7374 6572 5f6f 6e6c 7927 2920 6973  master_only') is
+000ee880: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000ee890: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
+000ee8a0: 6572 5f6f 6e6c 7920 3d20 6d2e 6765 7428  er_only = m.get(
+000ee8b0: 276d 6173 7465 725f 6f6e 6c79 2729 0a20  'master_only'). 
+000ee8c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000ee8d0: 276e 6578 745f 7665 7273 696f 6e27 2920  'next_version') 
+000ee8e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000ee8f0: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
+000ee900: 7874 5f76 6572 7369 6f6e 203d 206d 2e67  xt_version = m.g
+000ee910: 6574 2827 6e65 7874 5f76 6572 7369 6f6e  et('next_version
+000ee920: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000ee930: 6765 7428 2776 6572 7369 6f6e 2729 2069  get('version') i
+000ee940: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000ee950: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+000ee960: 7369 6f6e 203d 206d 2e67 6574 2827 7665  sion = m.get('ve
+000ee970: 7273 696f 6e27 290a 2020 2020 2020 2020  rsion').        
+000ee980: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000ee990: 6173 7320 5570 6772 6164 6543 6c75 7374  ass UpgradeClust
+000ee9a0: 6572 5265 7370 6f6e 7365 426f 6479 2854  erResponseBody(T
+000ee9b0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000ee9c0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+000ee9d0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000ee9e0: 2020 636c 7573 7465 725f 6964 3a20 7374    cluster_id: st
+000ee9f0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000eea00: 2020 7265 7175 6573 745f 6964 3a20 7374    request_id: st
+000eea10: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000eea20: 2020 7461 736b 5f69 643a 2073 7472 203d    task_id: str =
+000eea30: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+000eea40: 2020 2020 2020 7365 6c66 2e63 6c75 7374        self.clust
+000eea50: 6572 5f69 6420 3d20 636c 7573 7465 725f  er_id = cluster_
+000eea60: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
+000eea70: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+000eea80: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
+000eea90: 7365 6c66 2e74 6173 6b5f 6964 203d 2074  self.task_id = t
+000eeaa0: 6173 6b5f 6964 0a0a 2020 2020 6465 6620  ask_id..    def 
+000eeab0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000eeac0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000eead0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000eeae0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000eeaf0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000eeb00: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000eeb10: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000eeb20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000eeb30: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000eeb40: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000eeb50: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000eeb60: 662e 636c 7573 7465 725f 6964 2069 7320  f.cluster_id is 
+000eeb70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000eeb80: 2020 2020 2020 7265 7375 6c74 5b27 636c        result['cl
+000eeb90: 7573 7465 725f 6964 275d 203d 2073 656c  uster_id'] = sel
+000eeba0: 662e 636c 7573 7465 725f 6964 0a20 2020  f.cluster_id.   
+000eebb0: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
+000eebc0: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
+000eebd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000eebe0: 2072 6573 756c 745b 2772 6571 7565 7374   result['request
+000eebf0: 5f69 6427 5d20 3d20 7365 6c66 2e72 6571  _id'] = self.req
+000eec00: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
+000eec10: 6966 2073 656c 662e 7461 736b 5f69 6420  if self.task_id 
+000eec20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000eec30: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000eec40: 2774 6173 6b5f 6964 275d 203d 2073 656c  'task_id'] = sel
+000eec50: 662e 7461 736b 5f69 640a 2020 2020 2020  f.task_id.      
+000eec60: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000eec70: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000eec80: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000eec90: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+000eeca0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+000eecb0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000eecc0: 7428 2763 6c75 7374 6572 5f69 6427 2920  t('cluster_id') 
+000eecd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000eece0: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+000eecf0: 7573 7465 725f 6964 203d 206d 2e67 6574  uster_id = m.get
+000eed00: 2827 636c 7573 7465 725f 6964 2729 0a20  ('cluster_id'). 
+000eed10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000eed20: 2772 6571 7565 7374 5f69 6427 2920 6973  'request_id') is
+000eed30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000eed40: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+000eed50: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+000eed60: 7265 7175 6573 745f 6964 2729 0a20 2020  request_id').   
+000eed70: 2020 2020 2069 6620 6d2e 6765 7428 2774       if m.get('t
+000eed80: 6173 6b5f 6964 2729 2069 7320 6e6f 7420  ask_id') is not 
+000eed90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000eeda0: 2020 7365 6c66 2e74 6173 6b5f 6964 203d    self.task_id =
+000eedb0: 206d 2e67 6574 2827 7461 736b 5f69 6427   m.get('task_id'
+000eedc0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000eedd0: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+000eede0: 6772 6164 6543 6c75 7374 6572 5265 7370  gradeClusterResp
+000eedf0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+000eee00: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000eee10: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000eee20: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+000eee30: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
+000eee40: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000eee50: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
+000eee60: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000eee70: 2062 6f64 793a 2055 7067 7261 6465 436c   body: UpgradeCl
+000eee80: 7573 7465 7252 6573 706f 6e73 6542 6f64  usterResponseBod
+000eee90: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+000eeea0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000eeeb0: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+000eeec0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000eeed0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+000eeee0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+000eeef0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+000eef00: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000eef10: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000eef20: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+000eef30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000eef40: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+000eef50: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000eef60: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000eef70: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000eef80: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000eef90: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000eefa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000eefb0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000eefc0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000eefd0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000eefe0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+000eeff0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000ef000: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+000ef010: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+000ef020: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+000ef030: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+000ef040: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+000ef050: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000ef060: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+000ef070: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+000ef080: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+000ef090: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+000ef0a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000ef0b0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+000ef0c0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+000ef0d0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+000ef0e0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000ef0f0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000ef100: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000ef110: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000ef120: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000ef130: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+000ef140: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+000ef150: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000ef160: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+000ef170: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+000ef180: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000ef190: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000ef1a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000ef1b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000ef1c0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+000ef1d0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+000ef1e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000ef1f0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+000ef200: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000ef210: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+000ef220: 5570 6772 6164 6543 6c75 7374 6572 5265  UpgradeClusterRe
+000ef230: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
+000ef240: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000ef250: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+000ef260: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+000ef270: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+000ef280: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000ef290: 5570 6772 6164 6543 6c75 7374 6572 4164  UpgradeClusterAd
+000ef2a0: 646f 6e73 5265 7175 6573 7442 6f64 7928  donsRequestBody(
+000ef2b0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+000ef2c0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000ef2d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000ef2e0: 2020 2063 6f6d 706f 6e65 6e74 5f6e 616d     component_nam
+000ef2f0: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+000ef300: 2020 2020 2020 2063 6f6e 6669 673a 2073         config: s
+000ef310: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000ef320: 2020 206e 6578 745f 7665 7273 696f 6e3a     next_version:
+000ef330: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000ef340: 2020 2020 2070 6f6c 6963 793a 2073 7472       policy: str
+000ef350: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000ef360: 2076 6572 7369 6f6e 3a20 7374 7220 3d20   version: str = 
+000ef370: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+000ef380: 2020 2020 2023 2054 6865 206e 616d 6520       # The name 
+000ef390: 6f66 2074 6865 2063 6f6d 706f 6e65 6e74  of the component
+000ef3a0: 2e0a 2020 2020 2020 2020 2320 0a20 2020  ..        # .   
+000ef3b0: 2020 2020 2023 2054 6869 7320 7061 7261       # This para
+000ef3c0: 6d65 7465 7220 6973 2072 6571 7569 7265  meter is require
+000ef3d0: 642e 0a20 2020 2020 2020 2073 656c 662e  d..        self.
+000ef3e0: 636f 6d70 6f6e 656e 745f 6e61 6d65 203d  component_name =
+000ef3f0: 2063 6f6d 706f 6e65 6e74 5f6e 616d 650a   component_name.
+000ef400: 2020 2020 2020 2020 2320 5468 6520 6375          # The cu
+000ef410: 7374 6f6d 2063 6f6d 706f 6e65 6e74 2073  stom component s
+000ef420: 6574 7469 6e67 7320 7468 6174 2079 6f75  ettings that you
+000ef430: 2077 616e 7420 746f 2075 7365 2e20 5468   want to use. Th
+000ef440: 6520 7661 6c75 6520 6973 2061 204a 534f  e value is a JSO
+000ef450: 4e20 7374 7269 6e67 2e0a 2020 2020 2020  N string..      
+000ef460: 2020 7365 6c66 2e63 6f6e 6669 6720 3d20    self.config = 
+000ef470: 636f 6e66 6967 0a20 2020 2020 2020 2023  config.        #
+000ef480: 2054 6865 2076 6572 7369 6f6e 2074 6f20   The version to 
+000ef490: 7768 6963 6820 7468 6520 636f 6d70 6f6e  which the compon
+000ef4a0: 656e 7420 6361 6e20 6265 2075 7064 6174  ent can be updat
+000ef4b0: 6564 2e20 596f 7520 6361 6e20 6361 6c6c  ed. You can call
+000ef4c0: 2074 6865 2060 4465 7363 7269 6265 436c   the `DescribeCl
+000ef4d0: 7573 7465 7241 6464 6f6e 7356 6572 7369  usterAddonsVersi
+000ef4e0: 6f6e 6020 6f70 6572 6174 696f 6e20 746f  on` operation to
+000ef4f0: 2071 7565 7279 2074 6865 2076 6572 7369   query the versi
+000ef500: 6f6e 2074 6f20 7768 6963 6820 7468 6520  on to which the 
+000ef510: 636f 6d70 6f6e 656e 7420 6361 6e20 6265  component can be
+000ef520: 2075 7064 6174 6564 2e0a 2020 2020 2020   updated..      
+000ef530: 2020 2320 0a20 2020 2020 2020 2023 2054    # .        # T
+000ef540: 6869 7320 7061 7261 6d65 7465 7220 6973  his parameter is
+000ef550: 2072 6571 7569 7265 642e 0a20 2020 2020   required..     
+000ef560: 2020 2073 656c 662e 6e65 7874 5f76 6572     self.next_ver
+000ef570: 7369 6f6e 203d 206e 6578 745f 7665 7273  sion = next_vers
+000ef580: 696f 6e0a 2020 2020 2020 2020 2320 5468  ion.        # Th
+000ef590: 6520 7570 6461 7465 2070 6f6c 6963 792e  e update policy.
+000ef5a0: 2056 616c 6964 2076 616c 7565 733a 0a20   Valid values:. 
+000ef5b0: 2020 2020 2020 2023 200a 2020 2020 2020         # .      
+000ef5c0: 2020 2320 2a20 2020 6f76 6572 7772 6974    # *   overwrit
+000ef5d0: 650a 2020 2020 2020 2020 2320 2a20 2020  e.        # *   
+000ef5e0: 6361 6e61 7279 0a20 2020 2020 2020 2073  canary.        s
+000ef5f0: 656c 662e 706f 6c69 6379 203d 2070 6f6c  elf.policy = pol
+000ef600: 6963 790a 2020 2020 2020 2020 2320 5468  icy.        # Th
+000ef610: 6520 6375 7272 656e 7420 7665 7273 696f  e current versio
+000ef620: 6e20 6f66 2074 6865 2063 6f6d 706f 6e65  n of the compone
+000ef630: 6e74 2e0a 2020 2020 2020 2020 7365 6c66  nt..        self
+000ef640: 2e76 6572 7369 6f6e 203d 2076 6572 7369  .version = versi
+000ef650: 6f6e 0a0a 2020 2020 6465 6620 7661 6c69  on..    def vali
+000ef660: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000ef670: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000ef680: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000ef690: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000ef6a0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+000ef6b0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000ef6c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000ef6d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000ef6e0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000ef6f0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000ef700: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+000ef710: 6d70 6f6e 656e 745f 6e61 6d65 2069 7320  mponent_name is 
+000ef720: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000ef730: 2020 2020 2020 7265 7375 6c74 5b27 636f        result['co
+000ef740: 6d70 6f6e 656e 745f 6e61 6d65 275d 203d  mponent_name'] =
+000ef750: 2073 656c 662e 636f 6d70 6f6e 656e 745f   self.component_
+000ef760: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+000ef770: 7365 6c66 2e63 6f6e 6669 6720 6973 206e  self.config is n
+000ef780: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000ef790: 2020 2020 2072 6573 756c 745b 2763 6f6e       result['con
+000ef7a0: 6669 6727 5d20 3d20 7365 6c66 2e63 6f6e  fig'] = self.con
+000ef7b0: 6669 670a 2020 2020 2020 2020 6966 2073  fig.        if s
+000ef7c0: 656c 662e 6e65 7874 5f76 6572 7369 6f6e  elf.next_version
+000ef7d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000ef7e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000ef7f0: 5b27 6e65 7874 5f76 6572 7369 6f6e 275d  ['next_version']
+000ef800: 203d 2073 656c 662e 6e65 7874 5f76 6572   = self.next_ver
+000ef810: 7369 6f6e 0a20 2020 2020 2020 2069 6620  sion.        if 
+000ef820: 7365 6c66 2e70 6f6c 6963 7920 6973 206e  self.policy is n
+000ef830: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000ef840: 2020 2020 2072 6573 756c 745b 2770 6f6c       result['pol
+000ef850: 6963 7927 5d20 3d20 7365 6c66 2e70 6f6c  icy'] = self.pol
+000ef860: 6963 790a 2020 2020 2020 2020 6966 2073  icy.        if s
+000ef870: 656c 662e 7665 7273 696f 6e20 6973 206e  elf.version is n
+000ef880: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000ef890: 2020 2020 2072 6573 756c 745b 2776 6572       result['ver
+000ef8a0: 7369 6f6e 275d 203d 2073 656c 662e 7665  sion'] = self.ve
+000ef8b0: 7273 696f 6e0a 2020 2020 2020 2020 7265  rsion.        re
+000ef8c0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000ef8d0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000ef8e0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000ef8f0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000ef900: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000ef910: 2020 2020 2069 6620 6d2e 6765 7428 2763       if m.get('c
+000ef920: 6f6d 706f 6e65 6e74 5f6e 616d 6527 2920  omponent_name') 
+000ef930: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000ef940: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+000ef950: 6d70 6f6e 656e 745f 6e61 6d65 203d 206d  mponent_name = m
+000ef960: 2e67 6574 2827 636f 6d70 6f6e 656e 745f  .get('component_
+000ef970: 6e61 6d65 2729 0a20 2020 2020 2020 2069  name').        i
+000ef980: 6620 6d2e 6765 7428 2763 6f6e 6669 6727  f m.get('config'
+000ef990: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000ef9a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000ef9b0: 636f 6e66 6967 203d 206d 2e67 6574 2827  config = m.get('
+000ef9c0: 636f 6e66 6967 2729 0a20 2020 2020 2020  config').       
+000ef9d0: 2069 6620 6d2e 6765 7428 276e 6578 745f   if m.get('next_
+000ef9e0: 7665 7273 696f 6e27 2920 6973 206e 6f74  version') is not
+000ef9f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000efa00: 2020 2073 656c 662e 6e65 7874 5f76 6572     self.next_ver
+000efa10: 7369 6f6e 203d 206d 2e67 6574 2827 6e65  sion = m.get('ne
+000efa20: 7874 5f76 6572 7369 6f6e 2729 0a20 2020  xt_version').   
+000efa30: 2020 2020 2069 6620 6d2e 6765 7428 2770       if m.get('p
+000efa40: 6f6c 6963 7927 2920 6973 206e 6f74 204e  olicy') is not N
+000efa50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000efa60: 2073 656c 662e 706f 6c69 6379 203d 206d   self.policy = m
+000efa70: 2e67 6574 2827 706f 6c69 6379 2729 0a20  .get('policy'). 
+000efa80: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000efa90: 2776 6572 7369 6f6e 2729 2069 7320 6e6f  'version') is no
+000efaa0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000efab0: 2020 2020 7365 6c66 2e76 6572 7369 6f6e      self.version
+000efac0: 203d 206d 2e67 6574 2827 7665 7273 696f   = m.get('versio
+000efad0: 6e27 290a 2020 2020 2020 2020 7265 7475  n').        retu
+000efae0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000efaf0: 5570 6772 6164 6543 6c75 7374 6572 4164  UpgradeClusterAd
+000efb00: 646f 6e73 5265 7175 6573 7428 5465 614d  donsRequest(TeaM
+000efb10: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+000efb20: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000efb30: 2073 656c 662c 0a20 2020 2020 2020 2062   self,.        b
+000efb40: 6f64 793a 204c 6973 745b 5570 6772 6164  ody: List[Upgrad
+000efb50: 6543 6c75 7374 6572 4164 646f 6e73 5265  eClusterAddonsRe
+000efb60: 7175 6573 7442 6f64 795d 203d 204e 6f6e  questBody] = Non
+000efb70: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000efb80: 2020 2320 5468 6520 7265 7175 6573 7420    # The request 
+000efb90: 7061 7261 6d65 7465 7273 2e0a 2020 2020  parameters..    
+000efba0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+000efbb0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
+000efbc0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000efbd0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+000efbe0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+000efbf0: 666f 7220 6b20 696e 2073 656c 662e 626f  for k in self.bo
+000efc00: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+000efc10: 2020 2020 6966 206b 3a0a 2020 2020 2020      if k:.      
+000efc20: 2020 2020 2020 2020 2020 2020 2020 6b2e                k.
+000efc30: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+000efc40: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000efc50: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000efc60: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+000efc70: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000efc80: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000efc90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000efca0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000efcb0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000efcc0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000efcd0: 626f 6479 275d 203d 205b 5d0a 2020 2020  body'] = [].    
+000efce0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000efcf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000efd00: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+000efd10: 696e 2073 656c 662e 626f 6479 3a0a 2020  in self.body:.  
+000efd20: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000efd30: 7375 6c74 5b27 626f 6479 275d 2e61 7070  sult['body'].app
+000efd40: 656e 6428 6b2e 746f 5f6d 6170 2829 2069  end(k.to_map() i
+000efd50: 6620 6b20 656c 7365 204e 6f6e 6529 0a20  f k else None). 
+000efd60: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000efd70: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000efd80: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000efd90: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000efda0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000efdb0: 6963 7428 290a 2020 2020 2020 2020 7365  ict().        se
+000efdc0: 6c66 2e62 6f64 7920 3d20 5b5d 0a20 2020  lf.body = [].   
+000efdd0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+000efde0: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+000efdf0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+000efe00: 6f72 206b 2069 6e20 6d2e 6765 7428 2762  or k in m.get('b
+000efe10: 6f64 7927 293a 0a20 2020 2020 2020 2020  ody'):.         
+000efe20: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+000efe30: 6c20 3d20 5570 6772 6164 6543 6c75 7374  l = UpgradeClust
+000efe40: 6572 4164 646f 6e73 5265 7175 6573 7442  erAddonsRequestB
+000efe50: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
+000efe60: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+000efe70: 6170 7065 6e64 2874 656d 705f 6d6f 6465  append(temp_mode
+000efe80: 6c2e 6672 6f6d 5f6d 6170 286b 2929 0a20  l.from_map(k)). 
+000efe90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000efea0: 6c66 0a0a 0a63 6c61 7373 2055 7067 7261  lf...class Upgra
+000efeb0: 6465 436c 7573 7465 7241 6464 6f6e 7352  deClusterAddonsR
+000efec0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+000efed0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000efee0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000efef0: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
+000eff00: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
+000eff10: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+000eff20: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
+000eff30: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+000eff40: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000eff50: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+000eff60: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+000eff70: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+000eff80: 7475 735f 636f 6465 0a0a 2020 2020 6465  tus_code..    de
+000eff90: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000effa0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000effb0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000effc0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000effd0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000effe0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000efff0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000f0000: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000f0010: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000f0020: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000f0030: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000f0040: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+000f0050: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000f0060: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+000f0070: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+000f0080: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+000f0090: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000f00a0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000f00b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000f00c0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000f00d0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000f00e0: 6465 0a20 2020 2020 2020 2072 6574 7572  de.        retur
+000f00f0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000f0100: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000f0110: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+000f0120: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000f0130: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+000f0140: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+000f0150: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+000f0160: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000f0170: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000f0180: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000f0190: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000f01a0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+000f01b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000f01c0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000f01d0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+000f01e0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+000f01f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000f0200: 660a 0a0a 636c 6173 7320 5570 6772 6164  f...class Upgrad
+000f0210: 6543 6c75 7374 6572 4e6f 6465 706f 6f6c  eClusterNodepool
+000f0220: 5265 7175 6573 7452 6f6c 6c69 6e67 506f  RequestRollingPo
+000f0230: 6c69 6379 2854 6561 4d6f 6465 6c29 3a0a  licy(TeaModel):.
+000f0240: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000f0250: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000f0260: 2020 2020 2020 2020 6261 7463 685f 696e          batch_in
+000f0270: 7465 7276 616c 3a20 696e 7420 3d20 4e6f  terval: int = No
+000f0280: 6e65 2c0a 2020 2020 2020 2020 6d61 785f  ne,.        max_
+000f0290: 7061 7261 6c6c 656c 6973 6d3a 2069 6e74  parallelism: int
+000f02a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000f02b0: 2070 6175 7365 5f70 6f6c 6963 793a 2073   pause_policy: s
+000f02c0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+000f02d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e62  :.        self.b
+000f02e0: 6174 6368 5f69 6e74 6572 7661 6c20 3d20  atch_interval = 
+000f02f0: 6261 7463 685f 696e 7465 7276 616c 0a20  batch_interval. 
+000f0300: 2020 2020 2020 2073 656c 662e 6d61 785f         self.max_
+000f0310: 7061 7261 6c6c 656c 6973 6d20 3d20 6d61  parallelism = ma
+000f0320: 785f 7061 7261 6c6c 656c 6973 6d0a 2020  x_parallelism.  
+000f0330: 2020 2020 2020 7365 6c66 2e70 6175 7365        self.pause
+000f0340: 5f70 6f6c 6963 7920 3d20 7061 7573 655f  _policy = pause_
+000f0350: 706f 6c69 6379 0a0a 2020 2020 6465 6620  policy..    def 
+000f0360: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000f0370: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000f0380: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000f0390: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000f03a0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+000f03b0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000f03c0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000f03d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000f03e0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000f03f0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000f0400: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000f0410: 662e 6261 7463 685f 696e 7465 7276 616c  f.batch_interval
+000f0420: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000f0430: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000f0440: 5b27 6261 7463 685f 696e 7465 7276 616c  ['batch_interval
+000f0450: 275d 203d 2073 656c 662e 6261 7463 685f  '] = self.batch_
+000f0460: 696e 7465 7276 616c 0a20 2020 2020 2020  interval.       
+000f0470: 2069 6620 7365 6c66 2e6d 6178 5f70 6172   if self.max_par
+000f0480: 616c 6c65 6c69 736d 2069 7320 6e6f 7420  allelism is not 
+000f0490: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000f04a0: 2020 7265 7375 6c74 5b27 6d61 785f 7061    result['max_pa
+000f04b0: 7261 6c6c 656c 6973 6d27 5d20 3d20 7365  rallelism'] = se
+000f04c0: 6c66 2e6d 6178 5f70 6172 616c 6c65 6c69  lf.max_paralleli
+000f04d0: 736d 0a20 2020 2020 2020 2069 6620 7365  sm.        if se
+000f04e0: 6c66 2e70 6175 7365 5f70 6f6c 6963 7920  lf.pause_policy 
+000f04f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000f0500: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000f0510: 2770 6175 7365 5f70 6f6c 6963 7927 5d20  'pause_policy'] 
+000f0520: 3d20 7365 6c66 2e70 6175 7365 5f70 6f6c  = self.pause_pol
+000f0530: 6963 790a 2020 2020 2020 2020 7265 7475  icy.        retu
+000f0540: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+000f0550: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+000f0560: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+000f0570: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+000f0580: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+000f0590: 2020 2069 6620 6d2e 6765 7428 2762 6174     if m.get('bat
+000f05a0: 6368 5f69 6e74 6572 7661 6c27 2920 6973  ch_interval') is
+000f05b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000f05c0: 2020 2020 2020 2073 656c 662e 6261 7463         self.batc
+000f05d0: 685f 696e 7465 7276 616c 203d 206d 2e67  h_interval = m.g
+000f05e0: 6574 2827 6261 7463 685f 696e 7465 7276  et('batch_interv
+000f05f0: 616c 2729 0a20 2020 2020 2020 2069 6620  al').        if 
+000f0600: 6d2e 6765 7428 276d 6178 5f70 6172 616c  m.get('max_paral
+000f0610: 6c65 6c69 736d 2729 2069 7320 6e6f 7420  lelism') is not 
+000f0620: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000f0630: 2020 7365 6c66 2e6d 6178 5f70 6172 616c    self.max_paral
+000f0640: 6c65 6c69 736d 203d 206d 2e67 6574 2827  lelism = m.get('
+000f0650: 6d61 785f 7061 7261 6c6c 656c 6973 6d27  max_parallelism'
+000f0660: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000f0670: 6574 2827 7061 7573 655f 706f 6c69 6379  et('pause_policy
+000f0680: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000f0690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000f06a0: 2e70 6175 7365 5f70 6f6c 6963 7920 3d20  .pause_policy = 
+000f06b0: 6d2e 6765 7428 2770 6175 7365 5f70 6f6c  m.get('pause_pol
+000f06c0: 6963 7927 290a 2020 2020 2020 2020 7265  icy').        re
+000f06d0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+000f06e0: 7320 5570 6772 6164 6543 6c75 7374 6572  s UpgradeCluster
+000f06f0: 4e6f 6465 706f 6f6c 5265 7175 6573 7428  NodepoolRequest(
+000f0700: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+000f0710: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000f0720: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000f0730: 2020 2069 6d61 6765 5f69 643a 2073 7472     image_id: str
+000f0740: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000f0750: 206b 7562 6572 6e65 7465 735f 7665 7273   kubernetes_vers
+000f0760: 696f 6e3a 2073 7472 203d 204e 6f6e 652c  ion: str = None,
+000f0770: 0a20 2020 2020 2020 206e 6f64 655f 6e61  .        node_na
+000f0780: 6d65 733a 204c 6973 745b 7374 725d 203d  mes: List[str] =
+000f0790: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
+000f07a0: 6f6c 6c69 6e67 5f70 6f6c 6963 793a 2055  olling_policy: U
+000f07b0: 7067 7261 6465 436c 7573 7465 724e 6f64  pgradeClusterNod
+000f07c0: 6570 6f6f 6c52 6571 7565 7374 526f 6c6c  epoolRequestRoll
+000f07d0: 696e 6750 6f6c 6963 7920 3d20 4e6f 6e65  ingPolicy = None
+000f07e0: 2c0a 2020 2020 2020 2020 7275 6e74 696d  ,.        runtim
+000f07f0: 655f 7479 7065 3a20 7374 7220 3d20 4e6f  e_type: str = No
+000f0800: 6e65 2c0a 2020 2020 2020 2020 7275 6e74  ne,.        runt
+000f0810: 696d 655f 7665 7273 696f 6e3a 2073 7472  ime_version: str
+000f0820: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000f0830: 2075 7365 5f72 6570 6c61 6365 3a20 626f   use_replace: bo
+000f0840: 6f6c 203d 204e 6f6e 652c 0a20 2020 2029  ol = None,.    )
+000f0850: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
+000f0860: 4944 206f 6620 7468 6520 4f53 2069 6d61  ID of the OS ima
+000f0870: 6765 2074 6861 7420 6973 2075 7365 6420  ge that is used 
+000f0880: 6279 2074 6865 206e 6f64 6573 2e0a 2020  by the nodes..  
+000f0890: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
+000f08a0: 5f69 6420 3d20 696d 6167 655f 6964 0a20  _id = image_id. 
+000f08b0: 2020 2020 2020 2023 2054 6865 204b 7562         # The Kub
+000f08c0: 6572 6e65 7465 7320 7665 7273 696f 6e20  ernetes version 
+000f08d0: 7468 6174 2069 7320 7573 6564 2062 7920  that is used by 
+000f08e0: 7468 6520 6e6f 6465 732e 0a20 2020 2020  the nodes..     
+000f08f0: 2020 2073 656c 662e 6b75 6265 726e 6574     self.kubernet
+000f0900: 6573 5f76 6572 7369 6f6e 203d 206b 7562  es_version = kub
+000f0910: 6572 6e65 7465 735f 7665 7273 696f 6e0a  ernetes_version.
+000f0920: 2020 2020 2020 2020 7365 6c66 2e6e 6f64          self.nod
+000f0930: 655f 6e61 6d65 7320 3d20 6e6f 6465 5f6e  e_names = node_n
+000f0940: 616d 6573 0a20 2020 2020 2020 2073 656c  ames.        sel
+000f0950: 662e 726f 6c6c 696e 675f 706f 6c69 6379  f.rolling_policy
+000f0960: 203d 2072 6f6c 6c69 6e67 5f70 6f6c 6963   = rolling_polic
+000f0970: 790a 2020 2020 2020 2020 2320 5468 6520  y.        # The 
+000f0980: 7275 6e74 696d 6520 7479 7065 2e20 5661  runtime type. Va
+000f0990: 6c69 6420 7661 6c75 6573 3a20 636f 6e74  lid values: cont
+000f09a0: 6169 6e65 7264 2061 6e64 2064 6f63 6b65  ainerd and docke
+000f09b0: 722e 0a20 2020 2020 2020 2073 656c 662e  r..        self.
+000f09c0: 7275 6e74 696d 655f 7479 7065 203d 2072  runtime_type = r
+000f09d0: 756e 7469 6d65 5f74 7970 650a 2020 2020  untime_type.    
+000f09e0: 2020 2020 2320 5468 6520 7665 7273 696f      # The versio
+000f09f0: 6e20 6f66 2074 6865 2063 6f6e 7461 696e  n of the contain
+000f0a00: 6572 2072 756e 7469 6d65 2074 6861 7420  er runtime that 
+000f0a10: 6973 2075 7365 6420 6279 2074 6865 206e  is used by the n
+000f0a20: 6f64 6573 2e0a 2020 2020 2020 2020 7365  odes..        se
+000f0a30: 6c66 2e72 756e 7469 6d65 5f76 6572 7369  lf.runtime_versi
+000f0a40: 6f6e 203d 2072 756e 7469 6d65 5f76 6572  on = runtime_ver
+000f0a50: 7369 6f6e 0a20 2020 2020 2020 2073 656c  sion.        sel
+000f0a60: 662e 7573 655f 7265 706c 6163 6520 3d20  f.use_replace = 
+000f0a70: 7573 655f 7265 706c 6163 650a 0a20 2020  use_replace..   
+000f0a80: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000f0a90: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+000f0aa0: 7365 6c66 2e72 6f6c 6c69 6e67 5f70 6f6c  self.rolling_pol
+000f0ab0: 6963 793a 0a20 2020 2020 2020 2020 2020  icy:.           
+000f0ac0: 2073 656c 662e 726f 6c6c 696e 675f 706f   self.rolling_po
+000f0ad0: 6c69 6379 2e76 616c 6964 6174 6528 290a  licy.validate().
+000f0ae0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000f0af0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000f0b00: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000f0b10: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000f0b20: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000f0b30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000f0b40: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000f0b50: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000f0b60: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000f0b70: 7365 6c66 2e69 6d61 6765 5f69 6420 6973  self.image_id is
+000f0b80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000f0b90: 2020 2020 2020 2072 6573 756c 745b 2769         result['i
+000f0ba0: 6d61 6765 5f69 6427 5d20 3d20 7365 6c66  mage_id'] = self
+000f0bb0: 2e69 6d61 6765 5f69 640a 2020 2020 2020  .image_id.      
+000f0bc0: 2020 6966 2073 656c 662e 6b75 6265 726e    if self.kubern
+000f0bd0: 6574 6573 5f76 6572 7369 6f6e 2069 7320  etes_version is 
+000f0be0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000f0bf0: 2020 2020 2020 7265 7375 6c74 5b27 6b75        result['ku
+000f0c00: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+000f0c10: 275d 203d 2073 656c 662e 6b75 6265 726e  '] = self.kubern
+000f0c20: 6574 6573 5f76 6572 7369 6f6e 0a20 2020  etes_version.   
+000f0c30: 2020 2020 2069 6620 7365 6c66 2e6e 6f64       if self.nod
+000f0c40: 655f 6e61 6d65 7320 6973 206e 6f74 204e  e_names is not N
+000f0c50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000f0c60: 2072 6573 756c 745b 276e 6f64 655f 6e61   result['node_na
+000f0c70: 6d65 7327 5d20 3d20 7365 6c66 2e6e 6f64  mes'] = self.nod
+000f0c80: 655f 6e61 6d65 730a 2020 2020 2020 2020  e_names.        
+000f0c90: 6966 2073 656c 662e 726f 6c6c 696e 675f  if self.rolling_
+000f0ca0: 706f 6c69 6379 2069 7320 6e6f 7420 4e6f  policy is not No
+000f0cb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000f0cc0: 7265 7375 6c74 5b27 726f 6c6c 696e 675f  result['rolling_
+000f0cd0: 706f 6c69 6379 275d 203d 2073 656c 662e  policy'] = self.
+000f0ce0: 726f 6c6c 696e 675f 706f 6c69 6379 2e74  rolling_policy.t
+000f0cf0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000f0d00: 6966 2073 656c 662e 7275 6e74 696d 655f  if self.runtime_
+000f0d10: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+000f0d20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000f0d30: 7375 6c74 5b27 7275 6e74 696d 655f 7479  sult['runtime_ty
+000f0d40: 7065 275d 203d 2073 656c 662e 7275 6e74  pe'] = self.runt
+000f0d50: 696d 655f 7479 7065 0a20 2020 2020 2020  ime_type.       
+000f0d60: 2069 6620 7365 6c66 2e72 756e 7469 6d65   if self.runtime
+000f0d70: 5f76 6572 7369 6f6e 2069 7320 6e6f 7420  _version is not 
+000f0d80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000f0d90: 2020 7265 7375 6c74 5b27 7275 6e74 696d    result['runtim
+000f0da0: 655f 7665 7273 696f 6e27 5d20 3d20 7365  e_version'] = se
+000f0db0: 6c66 2e72 756e 7469 6d65 5f76 6572 7369  lf.runtime_versi
+000f0dc0: 6f6e 0a20 2020 2020 2020 2069 6620 7365  on.        if se
+000f0dd0: 6c66 2e75 7365 5f72 6570 6c61 6365 2069  lf.use_replace i
+000f0de0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000f0df0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000f0e00: 7573 655f 7265 706c 6163 6527 5d20 3d20  use_replace'] = 
+000f0e10: 7365 6c66 2e75 7365 5f72 6570 6c61 6365  self.use_replace
+000f0e20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000f0e30: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000f0e40: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000f0e50: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000f0e60: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000f0e70: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000f0e80: 6966 206d 2e67 6574 2827 696d 6167 655f  if m.get('image_
+000f0e90: 6964 2729 2069 7320 6e6f 7420 4e6f 6e65  id') is not None
+000f0ea0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000f0eb0: 6c66 2e69 6d61 6765 5f69 6420 3d20 6d2e  lf.image_id = m.
+000f0ec0: 6765 7428 2769 6d61 6765 5f69 6427 290a  get('image_id').
+000f0ed0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000f0ee0: 2827 6b75 6265 726e 6574 6573 5f76 6572  ('kubernetes_ver
+000f0ef0: 7369 6f6e 2729 2069 7320 6e6f 7420 4e6f  sion') is not No
+000f0f00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000f0f10: 7365 6c66 2e6b 7562 6572 6e65 7465 735f  self.kubernetes_
+000f0f20: 7665 7273 696f 6e20 3d20 6d2e 6765 7428  version = m.get(
+000f0f30: 276b 7562 6572 6e65 7465 735f 7665 7273  'kubernetes_vers
+000f0f40: 696f 6e27 290a 2020 2020 2020 2020 6966  ion').        if
+000f0f50: 206d 2e67 6574 2827 6e6f 6465 5f6e 616d   m.get('node_nam
+000f0f60: 6573 2729 2069 7320 6e6f 7420 4e6f 6e65  es') is not None
+000f0f70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000f0f80: 6c66 2e6e 6f64 655f 6e61 6d65 7320 3d20  lf.node_names = 
+000f0f90: 6d2e 6765 7428 276e 6f64 655f 6e61 6d65  m.get('node_name
+000f0fa0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+000f0fb0: 2e67 6574 2827 726f 6c6c 696e 675f 706f  .get('rolling_po
+000f0fc0: 6c69 6379 2729 2069 7320 6e6f 7420 4e6f  licy') is not No
+000f0fd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000f0fe0: 7465 6d70 5f6d 6f64 656c 203d 2055 7067  temp_model = Upg
+000f0ff0: 7261 6465 436c 7573 7465 724e 6f64 6570  radeClusterNodep
+000f1000: 6f6f 6c52 6571 7565 7374 526f 6c6c 696e  oolRequestRollin
+000f1010: 6750 6f6c 6963 7928 290a 2020 2020 2020  gPolicy().      
+000f1020: 2020 2020 2020 7365 6c66 2e72 6f6c 6c69        self.rolli
+000f1030: 6e67 5f70 6f6c 6963 7920 3d20 7465 6d70  ng_policy = temp
+000f1040: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+000f1050: 6d5b 2772 6f6c 6c69 6e67 5f70 6f6c 6963  m['rolling_polic
+000f1060: 7927 5d29 0a20 2020 2020 2020 2069 6620  y']).        if 
+000f1070: 6d2e 6765 7428 2772 756e 7469 6d65 5f74  m.get('runtime_t
+000f1080: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+000f1090: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000f10a0: 656c 662e 7275 6e74 696d 655f 7479 7065  elf.runtime_type
+000f10b0: 203d 206d 2e67 6574 2827 7275 6e74 696d   = m.get('runtim
+000f10c0: 655f 7479 7065 2729 0a20 2020 2020 2020  e_type').       
+000f10d0: 2069 6620 6d2e 6765 7428 2772 756e 7469   if m.get('runti
+000f10e0: 6d65 5f76 6572 7369 6f6e 2729 2069 7320  me_version') is 
+000f10f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000f1100: 2020 2020 2020 7365 6c66 2e72 756e 7469        self.runti
+000f1110: 6d65 5f76 6572 7369 6f6e 203d 206d 2e67  me_version = m.g
+000f1120: 6574 2827 7275 6e74 696d 655f 7665 7273  et('runtime_vers
+000f1130: 696f 6e27 290a 2020 2020 2020 2020 6966  ion').        if
+000f1140: 206d 2e67 6574 2827 7573 655f 7265 706c   m.get('use_repl
+000f1150: 6163 6527 2920 6973 206e 6f74 204e 6f6e  ace') is not Non
+000f1160: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000f1170: 656c 662e 7573 655f 7265 706c 6163 6520  elf.use_replace 
+000f1180: 3d20 6d2e 6765 7428 2775 7365 5f72 6570  = m.get('use_rep
+000f1190: 6c61 6365 2729 0a20 2020 2020 2020 2072  lace').        r
+000f11a0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000f11b0: 7373 2055 7067 7261 6465 436c 7573 7465  ss UpgradeCluste
+000f11c0: 724e 6f64 6570 6f6f 6c52 6573 706f 6e73  rNodepoolRespons
+000f11d0: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+000f11e0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000f11f0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+000f1200: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+000f1210: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+000f1220: 0a20 2020 2020 2020 2074 6173 6b5f 6964  .        task_id
+000f1230: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000f1240: 2020 293a 0a20 2020 2020 2020 2023 2054    ):.        # T
+000f1250: 6865 2072 6571 7565 7374 2049 442e 0a20  he request ID.. 
+000f1260: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+000f1270: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
+000f1280: 5f69 640a 2020 2020 2020 2020 2320 5468  _id.        # Th
+000f1290: 6520 7461 736b 2049 442e 0a20 2020 2020  e task ID..     
+000f12a0: 2020 2073 656c 662e 7461 736b 5f69 6420     self.task_id 
+000f12b0: 3d20 7461 736b 5f69 640a 0a20 2020 2064  = task_id..    d
+000f12c0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+000f12d0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+000f12e0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000f12f0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+000f1300: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+000f1310: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000f1320: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000f1330: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000f1340: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000f1350: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000f1360: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000f1370: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+000f1380: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000f1390: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000f13a0: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+000f13b0: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+000f13c0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+000f13d0: 6173 6b5f 6964 2069 7320 6e6f 7420 4e6f  ask_id is not No
+000f13e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000f13f0: 7265 7375 6c74 5b27 7461 736b 5f69 6427  result['task_id'
+000f1400: 5d20 3d20 7365 6c66 2e74 6173 6b5f 6964  ] = self.task_id
+000f1410: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000f1420: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000f1430: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000f1440: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000f1450: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000f1460: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000f1470: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
+000f1480: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
+000f1490: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000f14a0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+000f14b0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+000f14c0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+000f14d0: 2e67 6574 2827 7461 736b 5f69 6427 2920  .get('task_id') 
+000f14e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000f14f0: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
+000f1500: 736b 5f69 6420 3d20 6d2e 6765 7428 2774  sk_id = m.get('t
+000f1510: 6173 6b5f 6964 2729 0a20 2020 2020 2020  ask_id').       
+000f1520: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+000f1530: 6c61 7373 2055 7067 7261 6465 436c 7573  lass UpgradeClus
+000f1540: 7465 724e 6f64 6570 6f6f 6c52 6573 706f  terNodepoolRespo
+000f1550: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+000f1560: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000f1570: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000f1580: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+000f1590: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+000f15a0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000f15b0: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
+000f15c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000f15d0: 626f 6479 3a20 5570 6772 6164 6543 6c75  body: UpgradeClu
+000f15e0: 7374 6572 4e6f 6465 706f 6f6c 5265 7370  sterNodepoolResp
+000f15f0: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
+000f1600: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000f1610: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+000f1620: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
+000f1630: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+000f1640: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
+000f1650: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+000f1660: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
+000f1670: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000f1680: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000f1690: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+000f16a0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+000f16b0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+000f16c0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+000f16d0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+000f16e0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+000f16f0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+000f1700: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000f1710: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+000f1720: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+000f1730: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+000f1740: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+000f1750: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+000f1760: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000f1770: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+000f1780: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+000f1790: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+000f17a0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+000f17b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000f17c0: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+000f17d0: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+000f17e0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000f17f0: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+000f1800: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000f1810: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000f1820: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+000f1830: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+000f1840: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000f1850: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000f1860: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+000f1870: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+000f1880: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+000f1890: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+000f18a0: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+000f18b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000f18c0: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000f18d0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+000f18e0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+000f18f0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+000f1900: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+000f1910: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000f1920: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000f1930: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+000f1940: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+000f1950: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+000f1960: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000f1970: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+000f1980: 6f64 656c 203d 2055 7067 7261 6465 436c  odel = UpgradeCl
+000f1990: 7573 7465 724e 6f64 6570 6f6f 6c52 6573  usterNodepoolRes
+000f19a0: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
+000f19b0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000f19c0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+000f19d0: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+000f19e0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+000f19f0: 6e20 7365 6c66 0a0a 0a                   n self...
```

### Comparing `alibabacloud_cs20151215-4.1.0/alibabacloud_cs20151215.egg-info/PKG-INFO` & `alibabacloud_cs20151215-4.1.1/alibabacloud_cs20151215.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cs20151215
-Version: 4.1.0
+Version: 4.1.1
 Summary: Alibaba Cloud CS (20151215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cs20151215-4.1.0/setup.py` & `alibabacloud_cs20151215-4.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cs20151215.
 
-Created on 24/05/2024
+Created on 27/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cs20151215"
 NAME = "alibabacloud_cs20151215" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CS (20151215) SDK Library for Python"
```

