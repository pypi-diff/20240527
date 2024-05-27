# Comparing `tmp/alibabacloud_green20220302-2.2.5.tar.gz` & `tmp/alibabacloud_green20220302-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-2.2.5.tar", last modified: Sat May 11 06:09:58 2024, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-2.2.6.tar", last modified: Mon May 27 08:14:21 2024, max compression
```

## Comparing `alibabacloud_green20220302-2.2.5.tar` & `alibabacloud_green20220302-2.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/
--rw-r--r--   0 root         (0) root         (0)     1372 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63849 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)   124740 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2621 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63849 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)   125248 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-05-27 08:14:21.000000 alibabacloud_green20220302-2.2.6/setup.py
```

### Comparing `alibabacloud_green20220302-2.2.5/ChangeLog.md` & `alibabacloud_green20220302-2.2.6/ChangeLog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-05-11 Version: 2.2.5
+- Update API ImageModeration: update response param.
+
+
 2024-04-19 Version: 2.2.4
 - Update API ImageModeration: update response param.
 
 
 2024-04-11 Version: 2.2.3
 - Update API DescribeImageResultExt: update response param.
```

### Comparing `alibabacloud_green20220302-2.2.5/LICENSE` & `alibabacloud_green20220302-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.5/PKG-INFO` & `alibabacloud_green20220302-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 2.2.5
+Version: 2.2.6
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.5/README-CN.md` & `alibabacloud_green20220302-2.2.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.5/README.md` & `alibabacloud_green20220302-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/client.py` & `alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-2.2.6/alibabacloud_green20220302/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2250,34 +2250,46 @@
         return self
 
 
 class TextModerationPlusResponseBodyDataAdvice(TeaModel):
     def __init__(
         self,
         answer: str = None,
+        hit_label: str = None,
+        hit_lib_name: str = None,
     ):
         self.answer = answer
+        self.hit_label = hit_label
+        self.hit_lib_name = hit_lib_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.answer is not None:
             result['Answer'] = self.answer
+        if self.hit_label is not None:
+            result['HitLabel'] = self.hit_label
+        if self.hit_lib_name is not None:
+            result['HitLibName'] = self.hit_lib_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Answer') is not None:
             self.answer = m.get('Answer')
+        if m.get('HitLabel') is not None:
+            self.hit_label = m.get('HitLabel')
+        if m.get('HitLibName') is not None:
+            self.hit_lib_name = m.get('HitLibName')
         return self
 
 
 class TextModerationPlusResponseBodyDataResultCustomizedHit(TeaModel):
     def __init__(
         self,
         key_words: str = None,
```

### Comparing `alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-2.2.6/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 2.2.5
+Version: 2.2.6
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.5/setup.py` & `alibabacloud_green20220302-2.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 11/05/2024
+Created on 27/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
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

