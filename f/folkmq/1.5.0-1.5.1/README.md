# Comparing `tmp/folkmq-1.5.0.tar.gz` & `tmp/folkmq-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folkmq-1.5.0.tar", last modified: Fri May 24 13:24:40 2024, max compression
+gzip compressed data, was "folkmq-1.5.1.tar", last modified: Mon May 27 07:37:39 2024, max compression
```

## Comparing `folkmq-1.5.0.tar` & `folkmq-1.5.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.489270 folkmq-1.5.0/
--rw-r--r--   0 noear      (501) staff       (20)      587 2024-05-24 13:24:40.488533 folkmq-1.5.0/PKG-INFO
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.470216 folkmq-1.5.0/folkmq/
--rw-r--r--   0 noear      (501) staff       (20)      624 2024-05-24 01:20:55.000000 folkmq-1.5.0/folkmq/FolkMQ.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.478751 folkmq-1.5.0/folkmq/client/
--rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/client/MqAlarm.py
--rw-r--r--   0 noear      (501) staff       (20)     4021 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqClient.py
--rw-r--r--   0 noear      (501) staff       (20)    15624 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqClientDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     5657 2024-05-22 11:46:21.000000 folkmq-1.5.0/folkmq/client/MqClientListener.py
--rw-r--r--   0 noear      (501) staff       (20)     4180 2024-05-22 11:43:44.000000 folkmq-1.5.0/folkmq/client/MqMessage.py
--rw-r--r--   0 noear      (501) staff       (20)     3589 2024-05-22 11:46:21.000000 folkmq-1.5.0/folkmq/client/MqMessageReceived.py
--rw-r--r--   0 noear      (501) staff       (20)     1094 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqRouter.py
--rw-r--r--   0 noear      (501) staff       (20)      890 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqSubscription.py
--rw-r--r--   0 noear      (501) staff       (20)     1073 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/client/MqTransaction.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.485794 folkmq-1.5.0/folkmq/common/
--rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/MqApis.py
--rw-r--r--   0 noear      (501) staff       (20)     1079 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/common/MqAssert.py
--rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/MqConstants.py
--rw-r--r--   0 noear      (501) staff       (20)     2636 2024-05-22 11:39:58.000000 folkmq-1.5.0/folkmq/common/MqMetasResolver.py
--rw-r--r--   0 noear      (501) staff       (20)     5015 2024-05-22 11:48:43.000000 folkmq-1.5.0/folkmq/common/MqMetasResolverV1.py
--rw-r--r--   0 noear      (501) staff       (20)     5231 2024-05-22 11:48:43.000000 folkmq-1.5.0/folkmq/common/MqMetasResolverV2.py
--rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/MqMetasV1.py
--rw-r--r--   0 noear      (501) staff       (20)     1078 2024-05-22 11:38:28.000000 folkmq-1.5.0/folkmq/common/MqMetasV2.py
--rw-r--r--   0 noear      (501) staff       (20)      422 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/common/MqTopicHelper.py
--rw-r--r--   0 noear      (501) staff       (20)     1184 2024-05-16 09:27:43.000000 folkmq-1.5.0/folkmq/common/MqUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/common/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.486954 folkmq-1.5.0/folkmq/exception/
--rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/exception/FolkmqException.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.0/folkmq/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-24 13:24:40.487548 folkmq-1.5.0/folkmq.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      587 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)      896 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       47 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)        7 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-24 13:24:40.000000 folkmq-1.5.0/folkmq.egg-info/zip-safe
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-05-24 13:24:40.489428 folkmq-1.5.0/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      910 2024-05-24 11:16:43.000000 folkmq-1.5.0/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-27 07:37:39.175964 folkmq-1.5.1/
+-rw-r--r--   0 noear      (501) staff       (20)      587 2024-05-27 07:37:39.175086 folkmq-1.5.1/PKG-INFO
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-27 07:37:39.152666 folkmq-1.5.1/folkmq/
+-rw-r--r--   0 noear      (501) staff       (20)      624 2024-05-27 07:20:12.000000 folkmq-1.5.1/folkmq/FolkMQ.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-27 07:37:39.167508 folkmq-1.5.1/folkmq/client/
+-rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/client/MqAlarm.py
+-rw-r--r--   0 noear      (501) staff       (20)     4021 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/client/MqClient.py
+-rw-r--r--   0 noear      (501) staff       (20)    15624 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/client/MqClientDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     5657 2024-05-24 13:27:30.000000 folkmq-1.5.1/folkmq/client/MqClientListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     4180 2024-05-24 13:27:30.000000 folkmq-1.5.1/folkmq/client/MqMessage.py
+-rw-r--r--   0 noear      (501) staff       (20)     3589 2024-05-24 13:27:30.000000 folkmq-1.5.1/folkmq/client/MqMessageReceived.py
+-rw-r--r--   0 noear      (501) staff       (20)     1094 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/client/MqRouter.py
+-rw-r--r--   0 noear      (501) staff       (20)      890 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/client/MqSubscription.py
+-rw-r--r--   0 noear      (501) staff       (20)     1073 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/client/MqTransaction.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-27 07:37:39.173389 folkmq-1.5.1/folkmq/common/
+-rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/common/MqApis.py
+-rw-r--r--   0 noear      (501) staff       (20)     1079 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/common/MqAssert.py
+-rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/common/MqConstants.py
+-rw-r--r--   0 noear      (501) staff       (20)     2636 2024-05-24 13:27:30.000000 folkmq-1.5.1/folkmq/common/MqMetasResolver.py
+-rw-r--r--   0 noear      (501) staff       (20)     5015 2024-05-24 13:27:30.000000 folkmq-1.5.1/folkmq/common/MqMetasResolverV1.py
+-rw-r--r--   0 noear      (501) staff       (20)     5231 2024-05-24 13:27:30.000000 folkmq-1.5.1/folkmq/common/MqMetasResolverV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/common/MqMetasV1.py
+-rw-r--r--   0 noear      (501) staff       (20)     1078 2024-05-24 13:27:30.000000 folkmq-1.5.1/folkmq/common/MqMetasV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      422 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/common/MqTopicHelper.py
+-rw-r--r--   0 noear      (501) staff       (20)     1184 2024-05-16 09:27:43.000000 folkmq-1.5.1/folkmq/common/MqUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/common/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-27 07:37:39.174074 folkmq-1.5.1/folkmq/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/exception/FolkmqException.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-30 10:37:05.000000 folkmq-1.5.1/folkmq/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-05-27 07:37:39.174517 folkmq-1.5.1/folkmq.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      587 2024-05-27 07:37:39.000000 folkmq-1.5.1/folkmq.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)      896 2024-05-27 07:37:39.000000 folkmq-1.5.1/folkmq.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-27 07:37:39.000000 folkmq-1.5.1/folkmq.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       47 2024-05-27 07:37:39.000000 folkmq-1.5.1/folkmq.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)        7 2024-05-27 07:37:39.000000 folkmq-1.5.1/folkmq.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-05-27 07:37:39.000000 folkmq-1.5.1/folkmq.egg-info/zip-safe
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-05-27 07:37:39.176184 folkmq-1.5.1/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      910 2024-05-27 07:20:13.000000 folkmq-1.5.1/setup.py
```

### Comparing `folkmq-1.5.0/PKG-INFO` & `folkmq-1.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.5.0
+Version: 1.5.1
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `folkmq-1.5.0/folkmq/client/MqClient.py` & `folkmq-1.5.1/folkmq/client/MqClient.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/client/MqClientDefault.py` & `folkmq-1.5.1/folkmq/client/MqClientDefault.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/client/MqClientListener.py` & `folkmq-1.5.1/folkmq/client/MqClientListener.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/client/MqMessage.py` & `folkmq-1.5.1/folkmq/client/MqMessage.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/client/MqMessageReceived.py` & `folkmq-1.5.1/folkmq/client/MqMessageReceived.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/client/MqRouter.py` & `folkmq-1.5.1/folkmq/client/MqRouter.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/client/MqSubscription.py` & `folkmq-1.5.1/folkmq/client/MqSubscription.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/client/MqTransaction.py` & `folkmq-1.5.1/folkmq/client/MqTransaction.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqAssert.py` & `folkmq-1.5.1/folkmq/common/MqAssert.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqConstants.py` & `folkmq-1.5.1/folkmq/common/MqConstants.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqMetasResolver.py` & `folkmq-1.5.1/folkmq/common/MqMetasResolver.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqMetasResolverV1.py` & `folkmq-1.5.1/folkmq/common/MqMetasResolverV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqMetasResolverV2.py` & `folkmq-1.5.1/folkmq/common/MqMetasResolverV2.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqMetasV1.py` & `folkmq-1.5.1/folkmq/common/MqMetasV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqMetasV2.py` & `folkmq-1.5.1/folkmq/common/MqMetasV2.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq/common/MqUtils.py` & `folkmq-1.5.1/folkmq/common/MqUtils.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/folkmq.egg-info/PKG-INFO` & `folkmq-1.5.1/folkmq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.5.0
+Version: 1.5.1
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `folkmq-1.5.0/folkmq.egg-info/SOURCES.txt` & `folkmq-1.5.1/folkmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `folkmq-1.5.0/setup.py` & `folkmq-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='folkmq',
-    version='1.5.0',
+    version='1.5.1',
     description='@noear/folkmq python project',
     author='noear',
     url='https://folkmq.noear.org/',
     packages=find_packages(exclude=['*folkmq-test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru>=0.7.2',
         'websockets>=12.0',
```

