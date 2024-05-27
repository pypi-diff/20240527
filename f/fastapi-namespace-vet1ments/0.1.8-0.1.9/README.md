# Comparing `tmp/fastapi_namespace_vet1ments-0.1.8.tar.gz` & `tmp/fastapi_namespace_vet1ments-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_namespace_vet1ments-0.1.8.tar", last modified: Mon May 27 20:59:20 2024, max compression
+gzip compressed data, was "fastapi_namespace_vet1ments-0.1.9.tar", last modified: Mon May 27 21:19:32 2024, max compression
```

## Comparing `fastapi_namespace_vet1ments-0.1.8.tar` & `fastapi_namespace_vet1ments-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.393896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/mixinBase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/jwtTokenMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/opaqueTokenMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/tokenBaseMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 20:59:19.000000 fastapi_namespace_vet1ments-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:19:32.745882 fastapi_namespace_vet1ments-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 21:19:32.745882 fastapi_namespace_vet1ments-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:19:32.741882 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:19:32.741882 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/mixinBase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:19:32.745882 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/jwtTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/opaqueTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/tokenBaseMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:19:32.745882 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/tests/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 21:19:24.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:19:32.745882 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 21:19:32.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 21:19:32.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:19:32.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 21:19:32.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 21:19:32.000000 fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 21:19:32.745882 fastapi_namespace_vet1ments-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 21:19:31.000000 fastapi_namespace_vet1ments-0.1.9/setup.py
```

### Comparing `fastapi_namespace_vet1ments-0.1.8/LICENSE` & `fastapi_namespace_vet1ments-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fastapi_namespace_vet1ments
-Version: 0.1.8
+Name: fastapi-namespace-vet1ments
+Version: 0.1.9
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.8/README.md` & `fastapi_namespace_vet1ments-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/mixinBase.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/mixinBase.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/opaqueTokenMixin.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/opaqueTokenMixin.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/tokenBaseMixin.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/tokenBaseMixin.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/typings.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/mixins/token/typings.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/namespace.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/namespace.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/resource.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/test.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/tests/test.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/test2.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/tests/test2.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/types.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/typings.py` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace/typings.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fastapi-namespace-vet1ments
-Version: 0.1.8
+Name: fastapi_namespace_vet1ments
+Version: 0.1.9
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/SOURCES.txt` & `fastapi_namespace_vet1ments-0.1.9/fastapi_namespace_vet1ments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.8/setup.py` & `fastapi_namespace_vet1ments-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fastapi_namespace_vet1ments',
     description="For FastAPI Routing Class",
-    version='0.1.8',
+    version='0.1.9',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

