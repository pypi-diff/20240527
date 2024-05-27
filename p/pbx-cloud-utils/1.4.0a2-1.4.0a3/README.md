# Comparing `tmp/pbx_cloud_utils-1.4.0a2-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.4.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7601 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 24-May-24 14:27 cloud_utils/__init__.py
+Zip file size: 7600 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-May-27 13:24 cloud_utils/__init__.py
 -rw-r--r--  2.0 unx    12094 b- defN 24-May-23 08:46 cloud_utils/aio_storage.py
 -rw-r--r--  2.0 unx       57 b- defN 24-May-23 08:46 cloud_utils/const.py
 -rw-r--r--  2.0 unx      284 b- defN 24-May-23 08:46 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx    10471 b- defN 24-May-24 14:25 cloud_utils/storage.py
+-rw-r--r--  2.0 unx    10384 b- defN 24-May-27 13:19 cloud_utils/storage.py
 -rw-r--r--  2.0 unx     1365 b- defN 24-May-23 08:46 cloud_utils/types.py
 -rw-r--r--  2.0 unx      346 b- defN 24-May-23 08:46 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-May-24 14:27 pbx_cloud_utils-1.4.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:27 pbx_cloud_utils-1.4.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-24 14:27 pbx_cloud_utils-1.4.0a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      887 b- defN 24-May-24 14:27 pbx_cloud_utils-1.4.0a2.dist-info/RECORD
-11 files, 25932 bytes uncompressed, 6095 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx      324 b- defN 24-May-27 13:25 pbx_cloud_utils-1.4.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 13:25 pbx_cloud_utils-1.4.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-27 13:25 pbx_cloud_utils-1.4.0a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      887 b- defN 24-May-27 13:25 pbx_cloud_utils-1.4.0a3.dist-info/RECORD
+11 files, 25845 bytes uncompressed, 6094 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a2.dist-info/METADATA
+Filename: pbx_cloud_utils-1.4.0a3.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a2.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.4.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a2.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.4.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.4.0a2.dist-info/RECORD
+Filename: pbx_cloud_utils-1.4.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/storage.py

```diff
@@ -222,26 +222,23 @@
 
 class HybridGoogleCloudStorageObject(AmazonS3Object):
     provider_storage_class_map: dict[str, str] = gcs_storage_class_map
 
     def __init__(self, client, gcs_client: gcs_storage.Bucket) -> None:
         super().__init__(client)
         self.gcs_client = gcs_client
-
-    def set_storage_class(self, storage_class: str) -> None:
-        destination_storage_class = self.provider_storage_class_map[storage_class]
-        try:
-            self.client.put(StorageClass=destination_storage_class)
-        except BotoError as e:
-            raise exceptions.StorageError() from e
+        self.blob = self.gcs_client.get_blob(self.path)
 
     @property
     def _provider_storage_class(self) -> str:
-        blob = self.gcs_client.get_blob(self.path)
-        return blob.storage_class
+        return self.blob.storage_class
+
+    def set_storage_class(self, storage_class: str) -> None:
+        destination_storage_class = self.provider_storage_class_map[storage_class]
+        self.blob.update_storage_class(destination_storage_class)
 
 
 class Storage(ABC):
     object_class: type[StorageObject]
 
     def get_object(self, path: str) -> StorageObject:
         object_client = self.object_client_class(path)
```

## Comparing `pbx_cloud_utils-1.4.0a2.dist-info/RECORD` & `pbx_cloud_utils-1.4.0a3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cloud_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cloud_utils/aio_storage.py,sha256=hTMYwaK2Bx64vQVUj1PFKXg_649-sOIy3PQnSRpuifE,12094
 cloud_utils/const.py,sha256=I0vJw5LuVCMJZK3ajhM1v2O85cpxnnirDG-scWyxeRE,57
 cloud_utils/exceptions.py,sha256=4TFl0EqL8X2vEgs4xpNgev93bDMcawfVc9DAty7SAqw,284
-cloud_utils/storage.py,sha256=uq4fMAEAVuK1a57HTYkKjFe-d9PEitm8Ua9t5bicRZs,10471
+cloud_utils/storage.py,sha256=GDttP3oICvkayIo8GLxwEw1JIhPvAhvAIKOITMQp1hM,10384
 cloud_utils/types.py,sha256=o98xCZ9mwhjvvm2-CmGkgcEVbdj8wbZxwIgKICr2E08,1365
 cloud_utils/utils.py,sha256=gi__PPdP5YKxehoe9Az5lhAgN11sFxk3YLmHM0cxm1I,346
-pbx_cloud_utils-1.4.0a2.dist-info/METADATA,sha256=r2bIJ_jgxuROgWYW0VZRg1BxIp-pSt2ZSWN_xGlmiMs,324
-pbx_cloud_utils-1.4.0a2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pbx_cloud_utils-1.4.0a2.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
-pbx_cloud_utils-1.4.0a2.dist-info/RECORD,,
+pbx_cloud_utils-1.4.0a3.dist-info/METADATA,sha256=nJevZEVPCiT2Hb_UWVGNIAgil9UuXwMCJl1RR4Lmnrc,324
+pbx_cloud_utils-1.4.0a3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pbx_cloud_utils-1.4.0a3.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
+pbx_cloud_utils-1.4.0a3.dist-info/RECORD,,
```

