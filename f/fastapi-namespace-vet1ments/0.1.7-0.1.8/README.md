# Comparing `tmp/fastapi_namespace_vet1ments-0.1.7.tar.gz` & `tmp/fastapi_namespace_vet1ments-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_namespace_vet1ments-0.1.7.tar", last modified: Mon May 27 20:22:18 2024, max compression
+gzip compressed data, was "fastapi_namespace_vet1ments-0.1.8.tar", last modified: Mon May 27 20:59:20 2024, max compression
```

## Comparing `fastapi_namespace_vet1ments-0.1.7.tar` & `fastapi_namespace_vet1ments-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/mixinBase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/jwtTokenMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/opaqueTokenMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/tokenBaseMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.424211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 20:22:08.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:22:18.000000 fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:22:18.428211 fastapi_namespace_vet1ments-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-27 20:22:16.000000 fastapi_namespace_vet1ments-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.393896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/mixinBase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/jwtTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/opaqueTokenMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/tokenBaseMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 20:59:13.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:59:20.000000 fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:59:20.397896 fastapi_namespace_vet1ments-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-27 20:59:19.000000 fastapi_namespace_vet1ments-0.1.8/setup.py
```

### Comparing `fastapi_namespace_vet1ments-0.1.7/LICENSE` & `fastapi_namespace_vet1ments-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_namespace_vet1ments
-Version: 0.1.7
+Version: 0.1.8
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.7/README.md` & `fastapi_namespace_vet1ments-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/mixinBase.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/mixinBase.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/opaqueTokenMixin.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/opaqueTokenMixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,11 +15,11 @@
             token_info_validator=validate_opaque_token_info
         )
 
     def create_token(self) -> RawToken:
         return token_urlsafe(48)
 
     def _make_token(self, token: Token) -> OpaqueTokenInfo:
-        OpaqueTokenInfo(
+        return OpaqueTokenInfo(
             **token,
             idf=uuid4().hex
         )
```

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/tokenBaseMixin.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/tokenBaseMixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         이미 지워진 토큰 들을 user token list 에서 삭제함
         """
 
         async def wrap(pipe: AsyncPipeline, key: UserTokenKey):
             if len((tokens := await pipe.smembers(key))) == 0:
                 return
             await pipe.watch(*tokens)
-            tokens_for_delete = [i async for i in (await pipe.exists(i) for i in tokens) if i == 0]
+            tokens_for_delete = [i[0] async for i in ((i, await pipe.exists(i)) for i in tokens) if i[1] == 0]
             if len(tokens_for_delete) == 0:
                 return
             pipe.multi()
             _: AsyncPipeline = pipe.srem(key, *tokens_for_delete)
 
         await rd.transaction(
             partial(wrap, key=key),
@@ -394,18 +394,18 @@
             if len(tokens) == 0:
                 return []
 
             await pipe.watch(*tokens)
 
             return [self._TokenInfo(
                 token=i.split('/')[1],
-                expires_in=await pipe.ttl(i),
+                expires_in=ttl,
                 **token
             )
-            for i in tokens if self._token_validator((token := self._Token(**loads(await pipe.get(i)))))]
+            for i in tokens if self._token_validator((token := self._Token(**loads(await pipe.get(i))))) and (ttl := await pipe.ttl(i)) > 5]
 
         await self._manage_user_token(rd=rd, key=key)
         res: list[TI] = await rd.transaction(
             partial(transaction, key=key),
             key,
             value_from_callable=True
         )
```

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/typings.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/typings.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,22 @@
     Generic
 )
 from typing_extensions import (
     TypedDict,
     NotRequired
 )
 
-MethodType = Literal["get", "post", "put", "delete", "patch", "head", "options", "trace"]
 
-TokenType = Literal["ACCESS", "REFRESH"]
 TokenKey = NewType('TokenKey', str)
 UserTokenKey = NewType('UserTokenKey', str)
-# RawToken = NewType("RawToken", str)
 
+MethodType = Literal["get", "post", "put", "delete", "patch", "head", "options", "trace"]
+TokenType = Literal["ACCESS", "REFRESH"]
+# RawToken = NewType("RawToken", str)
 RawToken = str
-
 # TokenLimit = NewType("TokenLimit", int)
 TokenLimit = int
 # TokenExpire = NewType("TokenExpire", int)
 TokenExpire = int
 # TokenIdentify = NewType("TokenIdentify", int)
 TokenIdentify = str
 # TokenPayload = NewType("TokenPayload", dict[str, Any])
```

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/mixins/token/utils.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/mixins/token/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/namespace.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/namespace.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/resource.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/tests/test.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/tests/test.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/types.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace/typings.py` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace/typings.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-namespace-vet1ments
-Version: 0.1.7
+Version: 0.1.8
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.7/fastapi_namespace_vet1ments.egg-info/SOURCES.txt` & `fastapi_namespace_vet1ments-0.1.8/fastapi_namespace_vet1ments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.7/setup.py` & `fastapi_namespace_vet1ments-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fastapi_namespace_vet1ments',
     description="For FastAPI Routing Class",
-    version='0.1.7',
+    version='0.1.8',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
@@ -19,10 +19,11 @@
     },
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "fastapi>=0.108.0"
     ],
     tests_require=[
-        "uvicorn>=0.9.0"
+        "uvicorn>=0.9.0",
+        "fastapi-redis-vet1ments>=0.2.6"
     ],
 )
```

