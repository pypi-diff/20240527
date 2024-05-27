# Comparing `tmp/fastapi-openid-connect-0.1.0a0.tar.gz` & `tmp/fastapi-openid-connect-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-openid-connect-0.1.0a0.tar", last modified: Sat May 18 05:05:01 2024, max compression
+gzip compressed data, was "fastapi-openid-connect-0.1.0a1.tar", last modified: Mon May 27 16:06:40 2024, max compression
```

## Comparing `fastapi-openid-connect-0.1.0a0.tar` & `fastapi-openid-connect-0.1.0a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:05:01.088166 fastapi-openid-connect-0.1.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:05:01.084166 fastapi-openid-connect-0.1.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:05:01.084166 fastapi-openid-connect-0.1.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-18 05:05:01.088166 fastapi-openid-connect-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:05:01.088166 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:05:01.088166 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-18 05:05:01.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-18 05:05:01.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 05:05:01.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-18 05:05:01.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 05:05:01.000000 fastapi-openid-connect-0.1.0a0/fastapi_openid_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 05:05:01.088166 fastapi-openid-connect-0.1.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 05:04:41.000000 fastapi-openid-connect-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:40.930169 fastapi-openid-connect-0.1.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:40.930169 fastapi-openid-connect-0.1.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:40.930169 fastapi-openid-connect-0.1.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 16:06:40.930169 fastapi-openid-connect-0.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:40.930169 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:40.930169 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 16:06:40.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-27 16:06:40.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:06:40.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-27 16:06:40.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 16:06:40.000000 fastapi-openid-connect-0.1.0a1/fastapi_openid_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:06:40.930169 fastapi-openid-connect-0.1.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:06:26.000000 fastapi-openid-connect-0.1.0a1/setup.py
```

### Comparing `fastapi-openid-connect-0.1.0a0/.github/workflows/publish.yaml` & `fastapi-openid-connect-0.1.0a1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-openid-connect-0.1.0a0/.gitignore` & `fastapi-openid-connect-0.1.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi-openid-connect-0.1.0a0/LICENSE` & `fastapi-openid-connect-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-openid-connect-0.1.0a0/PKG-INFO` & `fastapi-openid-connect-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-openid-connect
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Models and Types for implementing and integrating with Open ID Connect 1.0 providers in FastAPI
 Author-email: "ApeWorX LTD." <admin@apeworx.io>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fastapi-openid-connect-0.1.0a0/demo.py` & `fastapi-openid-connect-0.1.0a1/demo.py`

 * *Files identical despite different names*

### Comparing `fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/models.py` & `fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/provider.py` & `fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     """
     OpenID Connect 1.0 authentication class. An instance of it would be used as a
     dependency to parse token.
 
     Example::
 
         >>> example_oidc = OpenIdConnect(baseUrl="https://example.com")
-        >>> @app.post("/auth")
-        ... def auth_with_example(token: dict = Depends(example_oidc)):
-        ...     user = db.add(User, id=token["sub"])
+        >>> @app.get("/auth")
+        ... def auth_callback_example(auth: AuthData = Depends(example_oidc)):
+        ...     user = db.add(User, id=auth.id_token["sub"])
     """
 
     def __init__(
         self,
         *,
         baseUrl: Annotated[
             Optional[str],
```

### Comparing `fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/types.py` & `fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/types.py`

 * *Files identical despite different names*

### Comparing `fastapi-openid-connect-0.1.0a0/fastapi_openid_connect/validators.py` & `fastapi-openid-connect-0.1.0a1/fastapi_openid_connect/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi-openid-connect-0.1.0a0/fastapi_openid_connect.egg-info/PKG-INFO` & `fastapi-openid-connect-0.1.0a1/fastapi_openid_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-openid-connect
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Models and Types for implementing and integrating with Open ID Connect 1.0 providers in FastAPI
 Author-email: "ApeWorX LTD." <admin@apeworx.io>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fastapi-openid-connect-0.1.0a0/pyproject.toml` & `fastapi-openid-connect-0.1.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 # NOTE: Hard pin all prod deps
 dependencies = [
-    "fastapi>=0.110",
-    "httpx",  # Peer of fastapi[all]
-    "python-jose",
-    "pydantic",  # Peer of fastapi
+    "fastapi>=0.100",  # added pydantic v2
+    "httpx>=0.23",  # Peer of fastapi[all]
+    "python-jose[cryptography]>=3.3",
+    "pydantic>=2.1",  # Peer of fastapi
 ]
 
 [project.optional-dependencies]
 lint = [
-    "ruff>=0.4.2",
+    "ruff",
 ]
 test = [
     "fastapi[all]",
     "pytest",
 ]
 release = [
   "setuptools_scm",
```

