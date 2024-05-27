# Comparing `tmp/fastapi_namespace_vet1ments-0.1.6.tar.gz` & `tmp/fastapi_namespace_vet1ments-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_namespace_vet1ments-0.1.6.tar", last modified: Mon May 27 19:47:19 2024, max compression
+gzip compressed data, was "fastapi_namespace_vet1ments-0.1.7.tar", last modified: Mon May 27 20:22:18 2024, max compression
```

## Comparing `fastapi_namespace_vet1ments-0.1.6.tar` & `fastapi_namespace_vet1ments-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/mixinBase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/jwtTokenMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/opaqueTokenMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/tokenBaseMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.481398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 19:47:11.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 19:47:19.000000 fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:47:19.485398 fastapi_namespace_vet1ments-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-27 19:47:18.000000 fastapi_namespace_vet1ments-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/mixinBase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/jwtTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/opaqueTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/tokenBaseMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-27 20:22:16.000000 fastapi_namespace_vet1ments-0.1.7/setup.py
```

### Comparing `fastapi_namespace_vet1ments-0.1.6/LICENSE` & `fastapi_namespace_vet1ments-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_namespace_vet1ments
-Version: 0.1.6
+Version: 0.1.7
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.6/README.md` & `fastapi_namespace_vet1ments-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/mixinBase.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/mixinBase.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/opaqueTokenMixin.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/opaqueTokenMixin.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/tokenBaseMixin.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/tokenBaseMixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Callable,
     Union,
     ParamSpec,
     TypeAlias,
     Generic,
     TypeVar,
     Iterable,
+    Coroutine
 )
 from functools import partial
 from orjson import dumps, loads
 
 P = ParamSpec("P")
 _TokenInfos = Union[OpaqueTokenInfo, JWTTokenInfo]
 _Tokens = Union[OpaqueToken, JWTToken]
@@ -478,15 +479,15 @@
             identify: UserIdentify,
             user_tokens: RawToken | Iterable[RawToken] | None = None
     ) -> None:
         default = partial(self._abort_user_type_token, rd=rd, identify=identify, type="ACCESS")
         if user_tokens is None:
             await default()
         elif isinstance(user_tokens, Iterable):
-            await default(user_tokens=user_tokens)
+            await default(user_tokens=[i for i in user_tokens])
         elif isinstance(user_tokens, str):
             await default(user_token=[user_tokens])
         else:
             raise ValueError('user Token error')
 
     async def abort_user_refresh_token(
             self,
@@ -494,15 +495,15 @@
             identify: UserIdentify,
             user_tokens: RawToken | Iterable[RawToken] | None = None
     ) -> None:
         default = partial(self._abort_user_type_token, rd=rd, identify=identify, type="REFRESH")
         if user_tokens is None:
             await default()
         elif isinstance(user_tokens, Iterable):
-            await default(user_tokens=user_tokens)
+            await default(user_tokens=[i for i in user_tokens])
         elif isinstance(user_tokens, str):
             await default(user_token=[user_tokens])
         else:
             raise ValueError('user Token error')
 
     async def abort_token(
             self,
```

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/typings.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/typings.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,26 @@
 )
 
 MethodType = Literal["get", "post", "put", "delete", "patch", "head", "options", "trace"]
 
 TokenType = Literal["ACCESS", "REFRESH"]
 TokenKey = NewType('TokenKey', str)
 UserTokenKey = NewType('UserTokenKey', str)
-RawToken = NewType("RawToken", str)
+# RawToken = NewType("RawToken", str)
 
-TokenLimit = NewType("TokenLimit", int)
-TokenExpire = NewType("TokenExpire", int)
-TokenIdentify = NewType("TokenIdentify", int)
-TokenPayload = NewType("TokenPayload", int)
+RawToken = str
+
+# TokenLimit = NewType("TokenLimit", int)
+TokenLimit = int
+# TokenExpire = NewType("TokenExpire", int)
+TokenExpire = int
+# TokenIdentify = NewType("TokenIdentify", int)
+TokenIdentify = str
+# TokenPayload = NewType("TokenPayload", dict[str, Any])
+TokenPayload = dict[str, Any]
 UserIdentify = Union[int, str]
 
 class Token(TypedDict):
     payload: TokenPayload
     uid: UserIdentify
 
 class TokenInfo(TypedDict):
```

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/mixins/token/utils.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/namespace.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/namespace.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/resource.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/tests/test.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 
 def depend_get(get: str) -> bool:
     print(get)
 
 def depend_post(post: str) -> bool:
     print(post)
 
+from fastapi import Security
+
 @namespace.route('/{asd}')
 class Root(OpaqueTokenMixin):
 
     global_dependencies = [Depends(depend_test), Depends(depend_test2)]
     get_dependencies = [Depends(depend_get)]
     post_dependencies = [Depends(depend_post)]
     def get(self) -> ItemResponse:
```

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/types.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace/typings.py` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/typings.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-namespace-vet1ments
-Version: 0.1.6
+Version: 0.1.7
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.6/fastapi_namespace_vet1ments.egg-info/SOURCES.txt` & `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.6/setup.py` & `fastapi_namespace_vet1ments-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fastapi_namespace_vet1ments',
     description="For FastAPI Routing Class",
-    version='0.1.6',
+    version='0.1.7',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

