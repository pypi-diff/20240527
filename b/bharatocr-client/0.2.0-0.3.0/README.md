# Comparing `tmp/bharatocr_client-0.2.0.tar.gz` & `tmp/bharatocr_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bharatocr_client-0.2.0.tar", last modified: Tue Apr 30 10:11:27 2024, max compression
+gzip compressed data, was "bharatocr_client-0.3.0.tar", last modified: Mon May 27 07:26:48 2024, max compression
```

## Comparing `bharatocr_client-0.2.0.tar` & `bharatocr_client-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:11:27.993221 bharatocr_client-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-30 10:11:27.989221 bharatocr_client-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:11:27.989221 bharatocr_client-0.2.0/bharatocr_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-30 10:11:27.000000 bharatocr_client-0.2.0/bharatocr_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-30 10:11:27.000000 bharatocr_client-0.2.0/bharatocr_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:11:27.000000 bharatocr_client-0.2.0/bharatocr_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:11:27.000000 bharatocr_client-0.2.0/bharatocr_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 10:11:27.000000 bharatocr_client-0.2.0/bharatocr_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:11:27.989221 bharatocr_client-0.2.0/bharatocrclient/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:11:27.989221 bharatocr_client-0.2.0/bharatocrclient/clients/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/aadhaar.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/driving_licence.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/pan.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/passport.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/bharatocrclient/clients/voter_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 10:11:27.993221 bharatocr_client-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-30 10:11:23.000000 bharatocr_client-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:26:48.234236 bharatocr_client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-27 07:26:48.234236 bharatocr_client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:26:48.234236 bharatocr_client-0.3.0/bharatocr_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-27 07:26:48.000000 bharatocr_client-0.3.0/bharatocr_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-27 07:26:48.000000 bharatocr_client-0.3.0/bharatocr_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:26:48.000000 bharatocr_client-0.3.0/bharatocr_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:26:48.000000 bharatocr_client-0.3.0/bharatocr_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 07:26:48.000000 bharatocr_client-0.3.0/bharatocr_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:26:48.230235 bharatocr_client-0.3.0/bharatocrclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:26:48.234236 bharatocr_client-0.3.0/bharatocrclient/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/aadhaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/driving_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/pan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/passport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/vehicle_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/voter_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/bharatocrclient/clients/water_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 07:26:48.234236 bharatocr_client-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-27 07:26:41.000000 bharatocr_client-0.3.0/setup.py
```

### Comparing `bharatocr_client-0.2.0/LICENSE` & `bharatocr_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bharatocr_client-0.2.0/PKG-INFO` & `bharatocr_client-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bharatocr-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: bharatocr-client is an opensource python library to access BharatOcrAPIs 
 Home-page: https://github.com/essentiasoftserv/bharatocrclient
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `bharatocr_client-0.2.0/README.md` & `bharatocr_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bharatocr_client-0.2.0/bharatocr_client.egg-info/PKG-INFO` & `bharatocr_client-0.3.0/bharatocr_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bharatocr-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: bharatocr-client is an opensource python library to access BharatOcrAPIs 
 Home-page: https://github.com/essentiasoftserv/bharatocrclient
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `bharatocr_client-0.2.0/bharatocr_client.egg-info/SOURCES.txt` & `bharatocr_client-0.3.0/bharatocr_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 bharatocrclient/clients/api.py
 bharatocrclient/clients/auth.py
 bharatocrclient/clients/common.py
 bharatocrclient/clients/driving_licence.py
 bharatocrclient/clients/exceptions.py
 bharatocrclient/clients/pan.py
 bharatocrclient/clients/passport.py
-bharatocrclient/clients/voter_id.py
+bharatocrclient/clients/vehicle_registration.py
+bharatocrclient/clients/voter_id.py
+bharatocrclient/clients/water_bill.py
```

### Comparing `bharatocr_client-0.2.0/bharatocrclient/clients/aadhaar.py` & `bharatocr_client-0.3.0/bharatocrclient/clients/aadhaar.py`

 * *Files identical despite different names*

### Comparing `bharatocr_client-0.2.0/bharatocrclient/clients/auth.py` & `bharatocr_client-0.3.0/bharatocrclient/clients/auth.py`

 * *Files identical despite different names*

### Comparing `bharatocr_client-0.2.0/bharatocrclient/clients/voter_id.py` & `bharatocr_client-0.3.0/bharatocrclient/clients/voter_id.py`

 * *Files identical despite different names*

### Comparing `bharatocr_client-0.2.0/setup.py` & `bharatocr_client-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="bharatocr-client",
-    version="0.2.0",
+    version="0.3.0",
     description="bharatocr-client is an opensource python library to access BharatOcrAPIs ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/essentiasoftserv/bharatocrclient",
     author="essentiasoftserv",
     python_requires=">=3.6",
     install_requires=install_requires,
```

