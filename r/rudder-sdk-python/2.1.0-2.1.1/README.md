# Comparing `tmp/rudder-sdk-python-2.1.0.tar.gz` & `tmp/rudder-sdk-python-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudder-sdk-python-2.1.0.tar", last modified: Wed Mar 20 11:52:26 2024, max compression
+gzip compressed data, was "rudder-sdk-python-2.1.1.tar", last modified: Mon May 27 05:07:31 2024, max compression
```

## Comparing `rudder-sdk-python-2.1.0.tar` & `rudder-sdk-python-2.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-20 11:52:26.557073 rudder-sdk-python-2.1.0/
--rw-r--r--   0 root         (0) staff       (20)     2372 2024-03-20 05:51:32.000000 rudder-sdk-python-2.1.0/LICENSE.md
--rw-r--r--   0 root         (0) staff       (20)     1205 2024-03-20 11:52:26.557223 rudder-sdk-python-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2100 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-20 11:52:26.545992 rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1205 2024-03-20 11:52:26.000000 rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      769 2024-03-20 11:52:26.000000 rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-03-20 11:52:26.000000 rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      187 2024-03-20 11:52:26.000000 rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       12 2024-03-20 11:52:26.000000 rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-20 11:52:26.540785 rudder-sdk-python-2.1.0/rudderstack/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-20 11:52:26.551589 rudder-sdk-python-2.1.0/rudderstack/analytics/
--rw-r--r--   0 root         (0) staff       (20)     3103 2023-03-06 05:33:57.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    11597 2024-01-08 09:37:13.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/client.py
--rw-r--r--   0 root         (0) staff       (20)     4460 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/consumer.py
--rw-r--r--   0 root         (0) staff       (20)      157 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/get_env.py
--rw-r--r--   0 root         (0) staff       (20)     2417 2023-03-01 10:14:07.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/request.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-20 11:52:26.556614 rudder-sdk-python-2.1.0/rudderstack/analytics/test/
--rw-r--r--   0 root         (0) staff       (20)     2695 2023-12-15 12:28:36.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/test/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    13478 2023-05-04 18:33:52.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_client.py
--rw-r--r--   0 root         (0) staff       (20)       31 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_constants.py
--rw-r--r--   0 root         (0) staff       (20)     7953 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_consumer.py
--rw-r--r--   0 root         (0) staff       (20)     1234 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_module.py
--rw-r--r--   0 root         (0) staff       (20)     2750 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_request.py
--rw-r--r--   0 root         (0) staff       (20)     2197 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_utils.py
--rw-r--r--   0 root         (0) staff       (20)     2472 2023-02-13 11:55:42.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/utils.py
--rw-r--r--   0 root         (0) staff       (20)       17 2024-03-20 11:48:12.000000 rudder-sdk-python-2.1.0/rudderstack/analytics/version.py
--rw-r--r--   0 root         (0) staff       (20)      108 2024-03-20 11:52:26.557821 rudder-sdk-python-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     2136 2024-01-08 09:37:13.000000 rudder-sdk-python-2.1.0/setup.py
+drwxr-xr-x   0 debanjanchatterjee   (501) staff       (20)        0 2024-05-27 05:07:31.935680 rudder-sdk-python-2.1.1/
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2147 2024-05-27 05:04:33.000000 rudder-sdk-python-2.1.1/LICENSE.md
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     1205 2024-05-27 05:07:31.935746 rudder-sdk-python-2.1.1/PKG-INFO
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2100 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/README.md
+drwxr-xr-x   0 debanjanchatterjee   (501) staff       (20)        0 2024-05-27 05:07:31.931452 rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     1205 2024-05-27 05:07:31.000000 rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)      769 2024-05-27 05:07:31.000000 rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)        1 2024-05-27 05:07:31.000000 rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)      186 2024-05-27 05:07:31.000000 rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)       12 2024-05-27 05:07:31.000000 rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 debanjanchatterjee   (501) staff       (20)        0 2024-05-27 05:07:31.929950 rudder-sdk-python-2.1.1/rudderstack/
+drwxr-xr-x   0 debanjanchatterjee   (501) staff       (20)        0 2024-05-27 05:07:31.933534 rudder-sdk-python-2.1.1/rudderstack/analytics/
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     3103 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/__init__.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)    11597 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/client.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     4498 2024-04-02 07:26:15.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/consumer.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)      157 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/get_env.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2442 2024-04-02 07:27:08.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/request.py
+drwxr-xr-x   0 debanjanchatterjee   (501) staff       (20)        0 2024-05-27 05:07:31.935114 rudder-sdk-python-2.1.1/rudderstack/analytics/test/
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2695 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/test/__init__.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)    13478 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_client.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)       31 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_constants.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     7953 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_consumer.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     1234 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_module.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2750 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_request.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2197 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_utils.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2472 2024-04-01 13:23:49.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/utils.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)       18 2024-05-17 11:10:47.000000 rudder-sdk-python-2.1.1/rudderstack/analytics/version.py
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)      108 2024-05-27 05:07:31.935959 rudder-sdk-python-2.1.1/setup.cfg
+-rw-r--r--   0 debanjanchatterjee   (501) staff       (20)     2135 2024-05-17 11:10:47.000000 rudder-sdk-python-2.1.1/setup.py
```

### Comparing `rudder-sdk-python-2.1.0/PKG-INFO` & `rudder-sdk-python-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudder-sdk-python
-Version: 2.1.0
+Version: 2.1.1
 Summary: RudderStack is an open-source Segment alternative written in Go, built for the enterprise.
 Home-page: https://github.com/rudderlabs/rudder-sdk-python
 Author: Rudderstack
 Author-email: sdk@rudderstack.com
 Maintainer: Rudderstack
 Maintainer-email: sdk@rudderstack.com
 License: MIT License
```

### Comparing `rudder-sdk-python-2.1.0/README.md` & `rudder-sdk-python-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/PKG-INFO` & `rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudder-sdk-python
-Version: 2.1.0
+Version: 2.1.1
 Summary: RudderStack is an open-source Segment alternative written in Go, built for the enterprise.
 Home-page: https://github.com/rudderlabs/rudder-sdk-python
 Author: Rudderstack
 Author-email: sdk@rudderstack.com
 Maintainer: Rudderstack
 Maintainer-email: sdk@rudderstack.com
 License: MIT License
```

### Comparing `rudder-sdk-python-2.1.0/rudder_sdk_python.egg-info/SOURCES.txt` & `rudder-sdk-python-2.1.1/rudder_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/__init__.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/client.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/client.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/consumer.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             if isinstance(exc, APIError):
                 # retry on server errors and client errors
                 # with 429 status code (rate limited),
                 # don't retry on other client errors
                 return (400 <= exc.status < 500) and exc.status != 429
             else:
                 # retry on all other errors (eg. network)
+                print("error: ", exc)
                 return False
 
         @backoff.on_exception(
             backoff.expo,
             Exception,
             max_tries=self.retries + 1,
             giveup=fatal_exception)
```

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/request.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     if proxies:
         kwargs['proxies'] = proxies
 
     res = _session.post(url, data=data, auth=auth,
                         headers=headers, timeout=timeout)
 
     if res.status_code == 200:
+        print("success")
         log.debug('data uploaded successfully')
         return res
 
     try:
         payload = res.json()
         log.debug('received response: %s', payload)
         raise APIError(res.status_code, payload['code'], payload['message'])
```

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/test/__init__.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/test/__init__.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_client.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_client.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_consumer.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_consumer.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_module.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_module.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_request.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_request.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/test/test_utils.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/rudderstack/analytics/utils.py` & `rudder-sdk-python-2.1.1/rudderstack/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `rudder-sdk-python-2.1.0/setup.py` & `rudder-sdk-python-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 '''
 
 install_requires = [
     "requests>=2.8,<3.0",
     "monotonic>=1.5,<2.0",
     "backoff>=2.1,<3.0",
     "python-dateutil>=2.2,<3.0",
-    "python-dotenv>=0.21.0,<0.22.0",
+    "python-dotenv>=0.21.0,<2.0.0",
     "deprecation>=2.0.6,<3.0.0",
 ]
 
 tests_require = [
     "mock==2.0.0",
     "pylint==2.8.0",
     "flake8==3.7.9",
```

