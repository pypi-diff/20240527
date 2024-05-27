# Comparing `tmp/appmesh-1.1.6-py3-none-any.whl.zip` & `tmp/appmesh-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16443 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-26 04:46 appmesh/__init__.py
--rw-r--r--  2.0 unx    59591 b- defN 24-May-26 04:46 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10832 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/RECORD
-6 files, 70989 bytes uncompressed, 15621 bytes compressed:  78.0%
+Zip file size: 16442 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-27 11:16 appmesh/__init__.py
+-rw-r--r--  2.0 unx    59591 b- defN 24-May-27 11:16 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10832 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-27 11:16 appmesh-1.1.7.dist-info/RECORD
+6 files, 70989 bytes uncompressed, 15620 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.1.6.dist-info/METADATA
+Filename: appmesh-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.1.6.dist-info/WHEEL
+Filename: appmesh-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.1.6.dist-info/top_level.txt
+Filename: appmesh-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.1.6.dist-info/RECORD
+Filename: appmesh-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -349,16 +349,16 @@
                 "Authorization": "Basic " + base64.b64encode((user_name + ":" + user_pwd).encode()).decode(),
                 "Expire-Seconds": self._parse_duration(timeout_seconds),
             },
         )
         if resp.status_code == HTTPStatus.OK:
             if "Access-Token" in resp.json():
                 self.jwt_token = resp.json()["Access-Token"]
-        elif resp.status_code == HTTPStatus.UNAUTHORIZED and "totp_challenge" in resp.json():
-            challenge = resp.json()["totp_challenge"]
+        elif resp.status_code == HTTPStatus.UNAUTHORIZED and "Totp-Challenge" in resp.json():
+            challenge = resp.json()["Totp-Challenge"]
             resp = self._request_http(
                 AppMeshClient.Method.POST,
                 path="/appmesh/totp/validate",
                 header={
                     "Username": base64.b64encode(user_name.encode()).decode(),
                     "Totp-Challenge": base64.b64encode(challenge.encode()).decode(),
                     "Totp": totp_code,
```

## Comparing `appmesh-1.1.6.dist-info/METADATA` & `appmesh-1.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.1.6
+Version: 1.1.7
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 1.1.6 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.1.7 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

