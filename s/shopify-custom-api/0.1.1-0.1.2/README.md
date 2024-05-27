# Comparing `tmp/shopify_custom_api-0.1.1.tar.gz` & `tmp/shopify_custom_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopify_custom_api-0.1.1.tar", last modified: Fri May 24 03:52:19 2024, max compression
+gzip compressed data, was "shopify_custom_api-0.1.2.tar", last modified: Mon May 27 04:48:47 2024, max compression
```

## Comparing `shopify_custom_api-0.1.1.tar` & `shopify_custom_api-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:52:19.518408 shopify_custom_api-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-24 03:52:11.000000 shopify_custom_api-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-24 03:52:19.518408 shopify_custom_api-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-24 03:52:11.000000 shopify_custom_api-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:52:19.518408 shopify_custom_api-0.1.1/cshopify/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 03:52:11.000000 shopify_custom_api-0.1.1/cshopify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-24 03:52:11.000000 shopify_custom_api-0.1.1/cshopify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 03:52:19.518408 shopify_custom_api-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-24 03:52:11.000000 shopify_custom_api-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:52:19.518408 shopify_custom_api-0.1.1/shopify_custom_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-24 03:52:19.000000 shopify_custom_api-0.1.1/shopify_custom_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 03:52:19.000000 shopify_custom_api-0.1.1/shopify_custom_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:52:19.000000 shopify_custom_api-0.1.1/shopify_custom_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 03:52:19.000000 shopify_custom_api-0.1.1/shopify_custom_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 03:52:19.000000 shopify_custom_api-0.1.1/shopify_custom_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:48:47.313512 shopify_custom_api-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-27 04:48:39.000000 shopify_custom_api-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-27 04:48:47.313512 shopify_custom_api-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-27 04:48:39.000000 shopify_custom_api-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:48:47.313512 shopify_custom_api-0.1.2/cshopify/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 04:48:39.000000 shopify_custom_api-0.1.2/cshopify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-27 04:48:39.000000 shopify_custom_api-0.1.2/cshopify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:48:47.313512 shopify_custom_api-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-27 04:48:39.000000 shopify_custom_api-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:48:47.313512 shopify_custom_api-0.1.2/shopify_custom_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-27 04:48:47.000000 shopify_custom_api-0.1.2/shopify_custom_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-27 04:48:47.000000 shopify_custom_api-0.1.2/shopify_custom_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:48:47.000000 shopify_custom_api-0.1.2/shopify_custom_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 04:48:47.000000 shopify_custom_api-0.1.2/shopify_custom_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 04:48:47.000000 shopify_custom_api-0.1.2/shopify_custom_api.egg-info/top_level.txt
```

### Comparing `shopify_custom_api-0.1.1/LICENSE.txt` & `shopify_custom_api-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shopify_custom_api-0.1.1/PKG-INFO` & `shopify_custom_api-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopify_custom_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple library that helps call Shopify's API
 Home-page: https://github.com/bachnguyen2001/shopify_custom_api.git
 Author: Nguyen Ngoc Bach
 Author-email: bachnguyenfptu@gmail.com
 License: MIT
 Keywords: shopify rest api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shopify_custom_api-0.1.1/README.md` & `shopify_custom_api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shopify_custom_api-0.1.1/cshopify/api.py` & `shopify_custom_api-0.1.2/cshopify/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 class API:
     def __init__(self, store_name, access_token, api_version):
         self.store_name = store_name
         self.access_token = access_token
         self.version = api_version
 
+    # Check if input data is in right format
     def validateJSON(self, data):
         return isinstance(data, dict)
 
     def __request(self, method, endpoint, data=None, params=None, **kwargs):
         url = f"https://{self.store_name}.myshopify.com/admin/api/{self.version}/{endpoint}.json"
 
         headers = {"X-Shopify-Access-Token": self.access_token}
```

### Comparing `shopify_custom_api-0.1.1/setup.py` & `shopify_custom_api-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Verify packages found
 packages = find_packages()
 print("Packages found:", packages)
 
 setup(
     name="shopify_custom_api",
-    version="0.1.1",
+    version="0.1.2",
     description="A simple library that helps call Shopify's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bachnguyen2001/shopify_custom_api.git",
     author="Nguyen Ngoc Bach",
     author_email="bachnguyenfptu@gmail.com",
     license="MIT",
```

### Comparing `shopify_custom_api-0.1.1/shopify_custom_api.egg-info/PKG-INFO` & `shopify_custom_api-0.1.2/shopify_custom_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopify_custom_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple library that helps call Shopify's API
 Home-page: https://github.com/bachnguyen2001/shopify_custom_api.git
 Author: Nguyen Ngoc Bach
 Author-email: bachnguyenfptu@gmail.com
 License: MIT
 Keywords: shopify rest api
 Classifier: Programming Language :: Python :: 3
```

