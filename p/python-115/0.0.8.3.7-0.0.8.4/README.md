# Comparing `tmp/python_115-0.0.8.3.7.tar.gz` & `tmp/python_115-0.0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.3.7.tar", max compression
+gzip compressed data, was "python_115-0.0.8.4.tar", max compression
```

## Comparing `python_115-0.0.8.3.7.tar` & `python_115-0.0.8.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.7/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.7/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.7/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.7/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.7/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.7/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.7/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.7/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8669 2024-05-25 05:50:21.865251 python_115-0.0.8.3.7/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.7/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.7/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.7/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.7/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.7/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.7/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.7/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.7/p115/component/cipher.py
--rwxr-xr-x   0        0        0   246414 2024-05-25 12:36:05.460976 python_115-0.0.8.3.7/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.7/p115/component/exception.py
--rwxr-xr-x   0        0        0    60836 2024-05-25 12:32:04.821744 python_115-0.0.8.3.7/p115/component/fs.py
--rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.3.7/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.7/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.7/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.3.7/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.3.7/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.3.7/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.3.7/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.7/p115/py.typed
--rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.3.7/p115/tool/__init__.py
--rw-r--r--   0        0        0     1665 2024-05-25 12:36:24.214636 python_115-0.0.8.3.7/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.7/readme.md
--rw-r--r--   0        0        0    36371 1970-01-01 00:00:00.000000 python_115-0.0.8.3.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.4/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.4/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.4/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.4/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.4/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8669 2024-05-25 05:50:21.865251 python_115-0.0.8.4/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.4/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.4/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.4/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.4/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.4/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   242824 2024-05-27 16:36:52.623847 python_115-0.0.8.4/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.4/p115/component/exception.py
+-rwxr-xr-x   0        0        0    65840 2024-05-27 16:29:09.478683 python_115-0.0.8.4/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.4/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.4/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.4/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.4/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.4/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.4/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.4/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.4/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.4/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1679 2024-05-27 16:45:21.674629 python_115-0.0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.4/readme.md
+-rw-r--r--   0        0        0    36397 1970-01-01 00:00:00.000000 python_115-0.0.8.4/PKG-INFO
```

### Comparing `python_115-0.0.8.3.7/LICENSE` & `python_115-0.0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/cmd/iterdir.py` & `python_115-0.0.8.4/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/cmd/qrcode.py` & `python_115-0.0.8.4/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/component/__init__.py` & `python_115-0.0.8.4/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/component/cipher.py` & `python_115-0.0.8.4/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/component/client.py` & `python_115-0.0.8.4/p115/component/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from urllib.parse import quote, urlencode, urlsplit
 from uuid import uuid4
 from xml.etree.ElementTree import fromstring
 
 from asynctools import as_thread, ensure_aiter, ensure_async
 from cookietools import cookies_str_to_dict, create_cookie
 from filewrap import (
-    SupportsRead, 
+    Buffer, SupportsRead, 
     bio_chunk_iter, bio_chunk_async_iter, 
     bio_skip_iter, bio_skip_async_iter, 
     bytes_iter_skip, bytes_async_iter_skip, 
     bytes_to_chunk_iter, bytes_to_chunk_async_iter, 
     bytes_ensure_part_iter, bytes_ensure_part_async_iter, 
 )
 from hashtools import file_digest, file_digest_async
@@ -67,15 +67,15 @@
 
 RequestVarT = TypeVar("RequestVarT", dict, Callable)
 RSA_ENCODER: Final = P115RSACipher()
 ECDH_ENCODER: Final = P115ECDHCipher()
 CRE_SHARE_LINK_search = re_compile(r"/s/(?P<share_code>\w+)(\?password=(?P<receive_code>\w+))?").search
 APP_VERSION: Final = "99.99.99.99"
 
-request = partial(httpx_request, parse=lambda _, content: loads(content))
+request = partial(httpx_request, parse=lambda _, content: loads(content), timeout=60)
 
 
 def to_base64(s: bytes | str, /) -> str:
     if isinstance(s, str):
         s = bytes(s, "utf-8")
     return str(b64encode(s), "ascii")
 
@@ -3825,18 +3825,15 @@
             **request_kwargs, 
         )
 
     @overload
     def _oss_multipart_upload_part(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         url: str, 
         token: dict, 
         upload_id: str, 
         part_number: int, 
         part_size: int, 
@@ -3844,36 +3841,30 @@
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def _oss_multipart_upload_part(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         url: str, 
         token: dict, 
         upload_id: str, 
         part_number: int, 
         part_size: int, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def _oss_multipart_upload_part(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         url: str, 
         token: dict, 
         upload_id: str, 
         part_number: int, 
         part_size: int = 10 * 1 << 20, # default to: 10 MB
@@ -3898,15 +3889,20 @@
                 "ETag": headers["ETag"], 
                 "HashCrc64ecma": int(headers["x-oss-hash-crc64ecma"]), 
                 "Size": count_in_bytes, 
             }
         request_kwargs["parse"] = parse
         request_kwargs["params"] = {"partNumber": part_number, "uploadId": upload_id}
         request_kwargs["headers"] = {"x-oss-security-token": token["SecurityToken"]}
-        if isinstance(file, (bytes, bytearray, memoryview)):
+        if hasattr(file, "getbuffer"):
+            try:
+                file = getattr(self, "getbuffer")()
+            except TypeError:
+                pass
+        if isinstance(file, Buffer):
             count_in_bytes = len(file)
             if async_:
                 async def make_iter():
                     yield file
                 dataiter = make_iter()
             else:
                 dataiter = iter((file,))
@@ -4061,18 +4057,15 @@
             **request_kwargs, 
         )
 
     @overload
     def _oss_multipart_upload_part_iter(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         url: str, 
         token: dict, 
         upload_id: str, 
         part_number_start, 
         part_size: int, 
@@ -4080,49 +4073,48 @@
         **request_kwargs, 
     ) -> Iterator[dict]:
         ...
     @overload
     def _oss_multipart_upload_part_iter(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         url: str, 
         token: dict, 
         upload_id: str, 
         part_number_start: int, 
         part_size: int, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> AsyncIterator[dict]:
         ...
     def _oss_multipart_upload_part_iter(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         url: str, 
         token: dict, 
         upload_id: str, 
         part_number_start: int = 1, 
         part_size: int = 10 * 1 << 20, # default to: 10 MB
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> Iterator[dict] | AsyncIterator[dict]:
         """帮助函数：迭代器，迭代一次上传一个分片
         """
-        if isinstance(file, (bytes, bytearray, memoryview)):
+        if hasattr(file, "getbuffer"):
+            try:
+                file = getattr(self, "getbuffer")()
+            except TypeError:
+                pass
+        if isinstance(file, Buffer):
             if async_:
                 file = bytes_to_chunk_async_iter(file, part_size)
             else:
                 file = bytes_to_chunk_iter(file, part_size)
         elif isinstance(file, SupportsRead):
             if not async_ and iscoroutinefunction(file.read):
                 raise TypeError(f"{file!r} with async read in non-async mode")
@@ -4255,60 +4247,56 @@
                     params["part-number-marker"] = etree.find("NextPartNumberMarker").text
             return request()
 
     @overload
     def _oss_upload(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         callback: dict, 
         token: None | dict, 
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def _oss_upload(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         callback: dict, 
         token: None | dict, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def _oss_upload(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         callback: dict, 
         token: None | dict = None, 
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """帮助函数：上传文件到阿里云 OSS，一次上传全部（即不进行分片）
         """
         url = self.upload_endpoint_url(bucket, object)
-        if isinstance(file, (bytes, bytearray, memoryview)):
+        if hasattr(file, "getbuffer"):
+            try:
+                file = getattr(self, "getbuffer")()
+            except TypeError:
+                pass
+        if isinstance(file, Buffer):
             if async_:
                 async def make_iter(file):
                     yield file
                 dataiter = make_iter(file)
             else:
                 dataiter = iter((file,))
         elif isinstance(file, SupportsRead):
@@ -4370,64 +4358,60 @@
     # TODO: 支持断点续传，但只支持 buffer、路径、url、可 seek 的 reader，否则报错
     def _oss_multipart_upload_ctx(self): ...
 
     @overload
     def _oss_multipart_upload(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         callback: dict, 
         token: None | dict, 
         upload_id: None | str, 
         part_size: int, 
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def _oss_multipart_upload(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         callback: dict, 
         token: None | dict, 
         upload_id: None | str, 
         part_size: int, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def _oss_multipart_upload(
         self, 
         /, 
-        file: ( bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+        file: Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer], 
         bucket: str, 
         object: str, 
         callback: dict, 
         token: None | dict = None, 
         upload_id: None | str = None, 
         part_size: int = 10 * 1 << 20, # default to: 10 MB
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         url = self.upload_endpoint_url(bucket, object)
         parts: list[dict] = []
+        if hasattr(file, "getbuffer"):
+            try:
+                file = getattr(self, "getbuffer")()
+            except TypeError:
+                pass
         if async_:
             async def async_request():
                 nonlocal async_, file, token, upload_id
                 async_ = cast(Literal[True], async_)
                 if not token:
                     token = await self.upload_token(async_=async_)
                 if upload_id:
@@ -4435,15 +4419,15 @@
                         bucket, object, url, token, upload_id, async_=async_, **request_kwargs, 
                     ):
                         if part["Size"] != part_size:
                             break
                         parts.append(part)
                     skipsize = sum(part["Size"] for part in parts)
                     if skipsize:
-                        if isinstance(file, (bytes, bytearray, memoryview)):
+                        if isinstance(file, Buffer):
                             file = memoryview(file)[skipsize:]
                         elif isinstance(file, SupportsRead):
                             try:
                                 file_seek = ensure_async(getattr(file, "seek"))
                                 await file_seek(skipsize, 1)
                             except (AttributeError, TypeError, OSError):
                                 await async_through(bio_skip_async_iter(file, skipsize))
@@ -4484,15 +4468,15 @@
                 parts.extend(takewhile(
                     lambda p: p["Size"] == part_size, 
                     self._oss_multipart_part_iter(
                         bucket, object, url, token, upload_id, async_=async_, **request_kwargs)
                 ))
                 skipsize = sum(part["Size"] for part in parts)
                 if skipsize:
-                    if isinstance(file, (bytes, bytearray, memoryview)):
+                    if isinstance(file, Buffer):
                         file = memoryview(file)[skipsize:]
                     elif isinstance(file, SupportsRead):
                         if iscoroutinefunction(file.read):
                             raise TypeError(f"{file!r} with async read in non-async mode")
                         try:
                             file_seek = getattr(file, "seek")
                             file_seek(skipsize, 1)
@@ -4632,56 +4616,52 @@
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     @overload
     def upload_file_sample(
         self, 
         /, 
         file: ( str | PathLike | URL | SupportsGeturl | 
-                bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer] ), 
         filename: None | str = None, 
         pid: int = 0, 
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def upload_file_sample(
         self, 
         /, 
         file: ( str | PathLike | URL | SupportsGeturl | 
-                bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer] ), 
         filename: None | str, 
         pid: int, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def upload_file_sample(
         self, 
         /, 
         file: ( str | PathLike | URL | SupportsGeturl | 
-                bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer] ), 
         filename: None | str = None, 
         pid: int = 0, 
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """网页端的上传接口，注意：不支持秒传，但也不需要文件大小和 sha1
         """
         file_will_open: None | tuple[str, Any] = None
-        if isinstance(file, (bytes, bytearray, memoryview)):
+        if hasattr(file, "getbuffer"):
+            try:
+                file = getattr(self, "getbuffer")()
+            except TypeError:
+                pass
+        if isinstance(file, Buffer):
             pass
         elif isinstance(file, (str, PathLike)):
             path = fsdecode(file)
             if not filename:
                 filename = ospath.basename(path)
             if async_:
                 file_will_open = ("path", path)
@@ -4712,18 +4692,18 @@
             elif isinstance(file, AsyncIterable):
                 raise TypeError(f"async iterable {file!r} in non-async mode")
         if async_:
             async def do_request(file, filename):
                 nonlocal async_
                 async_ = cast(Literal[True], async_)
 
-                file = cast(bytes | bytearray | memoryview | 
-                    SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                    Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                    AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview], file)
+                file = cast(Buffer | 
+                    SupportsRead[Buffer] | 
+                    Iterable[Buffer] | 
+                    AsyncIterable[Buffer], file)
                 if not filename:
                     filename = str(uuid4())
                 resp = await self.upload_file_sample_init(filename, pid, async_=async_, **request_kwargs)
                 api = resp["host"]
                 data = {
                     "name": filename, 
                     "key": resp["object"], 
@@ -4760,17 +4740,17 @@
                             async with request("GET", url) as resp:
                                 return await do_request(resp.content, filename or get_filename(resp))
                     else:
                         raise ValueError
                 return await do_request(file, filename)
             return async_request()
         else:
-            file = cast(bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview], file)
+            file = cast(Buffer | 
+                SupportsRead[Buffer] | 
+                Iterable[Buffer], file)
             if not filename:
                 filename = str(uuid4())
             resp = self.upload_file_sample_init(filename, pid, async_=async_, **request_kwargs)
             api = resp["host"]
             data = {
                 "name": filename, 
                 "key": resp["object"], 
@@ -4899,40 +4879,40 @@
     @overload
     def upload_file_init(
         self, 
         /, 
         filename: str, 
         filesize: int, 
         file_sha1: str, 
-        read_range_bytes_or_hash: None | Callable[[str], str | bytes | bytearray | memoryview], 
+        read_range_bytes_or_hash: None | Callable[[str], str | Buffer], 
         pid: int,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def upload_file_init(
         self, 
         /, 
         filename: str, 
         filesize: int, 
         file_sha1: str, 
-        read_range_bytes_or_hash: None | Callable[[str], str | bytes | bytearray | memoryview], 
+        read_range_bytes_or_hash: None | Callable[[str], str | Buffer], 
         pid: int,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def upload_file_init(
         self, 
         /, 
         filename: str, 
         filesize: int, 
         file_sha1: str, 
-        read_range_bytes_or_hash: None | Callable[[str], str | bytes | bytearray | memoryview] = None, 
+        read_range_bytes_or_hash: None | Callable[[str], str | Buffer] = None, 
         pid: int = 0, 
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """秒传接口，此接口是对 `upload_init` 的封装。
         NOTE: 
             - 文件大小 和 sha1 是必需的，只有 sha1 是没用的。
@@ -4951,18 +4931,18 @@
                     filesize, 
                     file_sha1, 
                     target, 
                     async_=async_, 
                     **request_kwargs, 
                 )
                 if resp["status"] == 7 and resp["statuscode"] == 701:
-                    read_range_bytes_or_hash = cast(Callable[[str], str | bytes | bytearray | memoryview], read_range_bytes_or_hash)
+                    read_range_bytes_or_hash = cast(Callable[[str], str | Buffer], read_range_bytes_or_hash)
                     sign_key = resp["sign_key"]
                     sign_check = resp["sign_check"]
-                    data: str | bytes | bytearray | memoryview = await ensure_async(read_range_bytes_or_hash)(sign_check) # type: ignore
+                    data: str | Buffer = await ensure_async(read_range_bytes_or_hash)(sign_check) # type: ignore
                     if isinstance(data, str):
                         sign_val = data.upper()
                     else:
                         sign_val = sha1(data).hexdigest().upper()
                     resp = await self._upload_file_init(
                         filename, 
                         filesize, 
@@ -4993,15 +4973,15 @@
                 target, 
                 async_=async_, 
                 **request_kwargs, 
             )
             # NOTE: 当文件大于等于 1 MB (1048576 B)，需要 2 次检验 1 个范围哈希，它会给出此文件的 1 个范围区间
             #       ，你读取对应的数据计算 sha1 后上传，以供 2 次检验
             if resp["status"] == 7 and resp["statuscode"] == 701:
-                read_range_bytes_or_hash = cast(Callable[[str], str | bytes | bytearray | memoryview], read_range_bytes_or_hash)
+                read_range_bytes_or_hash = cast(Callable[[str], str | Buffer], read_range_bytes_or_hash)
                 sign_key = resp["sign_key"]
                 sign_check = resp["sign_check"]
                 data = read_range_bytes_or_hash(sign_check)
                 if isinstance(data, str):
                     sign_val = data.upper()
                 else:
                     sign_val = sha1(data).hexdigest().upper()
@@ -5030,18 +5010,15 @@
     #           @classmethod
     #           def from_cache(cls, /, bucket, object, upload_id, callback, file): ...
     @overload
     def upload_file(
         self, 
         /, 
         file: ( str | PathLike | URL | SupportsGeturl | 
-                bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer] ), 
         filename: None | str = None, 
         pid: int = 0, 
         filesize: int = -1, 
         file_sha1: None | str = None, 
         part_size: int = 0, 
         upload_directly: bool = False, 
         async_: Literal[False] = False, 
@@ -5049,51 +5026,48 @@
     ) -> dict:
         ...
     @overload
     def upload_file(
         self, 
         /, 
         file: ( str | PathLike | URL | SupportsGeturl | 
-                bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer] ), 
         filename: None | str, 
         pid: int, 
         filesize: int, 
         file_sha1: None | str, 
         part_size: int, 
         upload_directly: bool, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def upload_file(
         self, 
         /, 
         file: ( str | PathLike | URL | SupportsGeturl | 
-                # TODO: 当升级到 0.1 版本时，将强制要求 python 3.12，这 bytes | bytearray | memoryview 用 collections.abc.Buffer 
-                bytes | bytearray | memoryview | 
-                SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer] ), 
         filename: None | str = None, 
         pid: int = 0, 
         filesize: int = -1, 
         file_sha1: None | str = None, 
         part_size: int = 0, 
         upload_directly: bool = False, 
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """文件上传接口，这是高层封装，推荐使用
         """
         if upload_directly:
             return self.upload_file_sample(file, filename, pid, async_=async_, **request_kwargs)
-
+        if hasattr(file, "getbuffer"):
+            try:
+                file = getattr(self, "getbuffer")()
+            except TypeError:
+                pass
         if async_:
             async def async_request():
                 nonlocal async_, file, filename, filesize, file_sha1
                 async_ = cast(Literal[True], async_)
 
                 async def do_upload(file):
                     nonlocal async_
@@ -5134,15 +5108,15 @@
                             callback, 
                             part_size=part_size, 
                             async_=async_, 
                             **request_kwargs, 
                         )
 
                 read_range_bytes_or_hash = None
-                if isinstance(file, (bytes, bytearray, memoryview)):
+                if isinstance(file, Buffer):
                     if filesize < 0:
                         filesize = len(file)
                     if not file_sha1:
                         file_sha1 = sha1(file).hexdigest()
                     if filesize >= 1 << 20:
                         mmv = memoryview(file)
                         def read_range_bytes_or_hash(sign_check: str):
@@ -5322,15 +5296,15 @@
                         callback, 
                         part_size=part_size, 
                         async_=async_, 
                         **request_kwargs, 
                     )
 
             read_range_bytes_or_hash: None | Callable = None
-            if isinstance(file, (bytes, bytearray, memoryview)):
+            if isinstance(file, Buffer):
                 if filesize < 0:
                     filesize = len(file)
                 if not file_sha1:
                     file_sha1 = sha1(file).hexdigest()
                 if filesize >= 1 << 20:
                     mmv = memoryview(file)
                     def read_range_bytes_or_hash(sign_check: str):
@@ -5543,29 +5517,33 @@
         /,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def extract_info(
         self, 
-        payload: dict, 
+        payload: str | dict, 
         /,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """获取压缩文件的文件列表，推荐直接用封装函数 `extract_list`
         GET https://webapi.115.com/files/extract_info
         payload:
             - pick_code: str
-            - file_name: str
-            - paths: str
-            - next_marker: str
-            - page_count: int | str # NOTE: 介于 1-999
+            - file_name: str = ""
+            - next_marker: str = ""
+            - page_count: int | str = 999 # NOTE: 介于 1-999
+            - paths: str = "文件"
         """
         api = "https://webapi.115.com/files/extract_info"
+        if isinstance(payload, str):
+            payload = {"paths": "文件", "page_count": 999, "next_marker": "", "file_name": "", "pick_code": payload}
+        else:
+            payload = {"paths": "文件", "page_count": 999, "next_marker": "", "file_name": "", **payload}
         request_kwargs.pop("parse", None)
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     @overload
     def extract_list(
         self, 
         /,
```

### Comparing `python_115-0.0.8.3.7/p115/component/fs.py` & `python_115-0.0.8.4/p115/component/fs.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,36 +10,40 @@
 
 from collections import deque, ChainMap
 from collections.abc import (
     Callable, Iterable, Iterator, Mapping, MutableMapping, Sequence, 
 )
 from datetime import datetime
 from io import BytesIO, TextIOWrapper
+from itertools import islice
+from json import JSONDecodeError
 from os import (
     path as ospath, fsdecode, fspath, makedirs, remove, rmdir, scandir, stat_result, PathLike
 )
 from pathlib import Path
 from posixpath import join as joinpath, splitext
 from shutil import SameFileError
 from stat import S_IFDIR, S_IFREG
 from typing import cast, Literal, Optional, Self
 from uuid import uuid4
+from yarl import URL
 
-from filewrap import SupportsRead
+from filewrap import Buffer, SupportsRead
+from http_request import SupportsGeturl
 from posixpatht import basename, commonpath, dirname, escape, joins, normpath, splits, unescape
 
 from .client import check_response, P115Client
 from .fs_base import AttrDict, IDOrPathType, P115PathBase, P115FileSystemBase
 
 
 def normalize_info(
     info: Mapping, 
     keep_raw: bool = False, 
     **extra_data, 
-) -> dict:
+) -> AttrDict:
     if "fid" in info:
         fid = info["fid"]
         parent_id = info["cid"]
         is_dir = False
     else:
         fid = info["cid"]
         parent_id = info["pid"]
@@ -93,137 +97,134 @@
         info2.update(extra_data)
     return info2
 
 
 class P115Path(P115PathBase):
     fs: P115FileSystem
 
+    @property
+    def length(self, /):
+        if self.is_dir():
+            return self.fs.dirlen(self.id)
+        return self["size"]
+
+    @property
+    def desc(self, /):
+        return self.fs.desc(self)
+
+    @desc.setter
+    def desc(self, /, desc: str = ""):
+        return self.fs.desc(self, desc=desc)
+
+    @property
+    def score(self, /) -> bool:
+        return self["score"]
+
+    @score.setter
+    def score(self, /, score: bool = True):
+        self.fs.score(self, score=score)
+
+    @property
+    def star(self, /) -> bool:
+        return self["star"]
+
+    @star.setter
+    def star(self, /, star: bool = True):
+        self.fs.star(self, star=star)
+
     def copy(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
-        overwrite_or_ignore: Optional[bool] = None, 
-    ) -> Optional[Self]:
+        overwrite: bool = False, 
+        onerror: bool | Callable[[OSError], bool] = True, 
+    ) -> None | Self:
         attr = self.fs.copy(
             self, 
             dst_path, 
             pid=pid, 
-            overwrite_or_ignore=overwrite_or_ignore, 
+            overwrite=overwrite, 
+            onerror=onerror, 
             recursive=True, 
         )
         if attr is None:
             return None
         return type(self)(attr)
 
-    @property
-    def desc(self, /):
-        return self.fs.desc(self)
-
-    @desc.setter
-    def desc(self, /, desc: str = ""):
-        return self.fs.desc(self, desc=desc)
-
-    @property
-    def length(self, /):
-        if self.is_dir():
-            return self.fs.dirlen(self.id)
-        return self["size"]
-
     def mkdir(self, /, exist_ok: bool = True) -> Self:
         self.__dict__.update(self.fs.makedirs(self, exist_ok=exist_ok))
         return self
 
     def move(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
     ) -> Self:
-        attr = self.fs.move(self, dst_path, pid)
-        if attr:
-            self.__dict__.update(attr)
+        self.__dict__.update(self.fs.move(self, dst_path, pid))
         return self
 
-    def remove(self, /, recursive: bool = True) -> dict:
+    def remove(self, /, recursive: bool = True) -> AttrDict:
         return self.fs.remove(self, recursive=recursive)
 
     def rename(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
     ) -> Self:
-        attr = self.fs.rename(self, dst_path, pid)
-        if attr:
-            self.__dict__.update(attr)
+        self.__dict__.update(self.fs.rename(self, dst_path, pid))
         return self
 
     def renames(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
     ) -> Self:
-        attr = self.fs.renames(self, dst_path, pid)
-        if attr:
-            self.__dict__.update(attr)
+        self.__dict__.update(self.fs.renames(self, dst_path, pid))
         return self
 
     def replace(
         self, 
         /, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
     ) -> Self:
-        attr = self.fs.replace(self, dst_path, pid)
-        if attr:
-            self.__dict__.update(attr)
+        self.__dict__.update(self.fs.replace(self, dst_path, pid))
         return self
 
-    def rmdir(self, /) -> dict:
+    def rmdir(self, /) -> AttrDict:
         return self.fs.rmdir(self)
 
-    @property
-    def score(self, /) -> bool:
-        return self["score"]
-
-    @score.setter
-    def score(self, /, score: bool = True):
-        self.fs.score(self, score=score)
-
-    @property
-    def star(self, /) -> bool:
-        return self["star"]
-
-    @star.setter
-    def star(self, /, star: bool = True):
-        self.fs.star(self, star=star)
+    def search(self, /, **payload) -> Iterator[P115Path]:
+        return self.fs.search(self, **payload)
 
     def touch(self, /) -> Self:
         self.__dict__.update(self.fs.touch(self))
         return self
 
     unlink = remove
 
     def write_bytes(
         self, 
         /, 
-        data: bytes | bytearray | memoryview | SupportsRead[bytes] = b"", 
+        data: Buffer | SupportsRead[Buffer] = b"", 
     ) -> Self:
         self.__dict__.update(self.fs.write_bytes(self, data))
         return self
 
     def write_text(
         self, 
         /, 
         text: str = "", 
-        encoding: Optional[str] = None, 
-        errors: Optional[str] = None, 
-        newline: Optional[str] = None, 
+        encoding: None | str = None, 
+        errors: None | str = None, 
+        newline: None | str = None, 
     ) -> Self:
         self.__dict__.update(self.fs.write_text(
             self, 
             text, 
             encoding=encoding, 
             errors=errors, 
             newline=newline, 
@@ -269,15 +270,16 @@
 
     def __len__(self, /) -> int:
         return self.dirlen(self.id)
 
     def __setitem__(
         self, 
         id_or_path: IDOrPathType, 
-        file: None | str | bytes | bytearray | memoryview | PathLike = None, 
+        file: ( None | str | PathLike | URL | SupportsGeturl | 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] ), 
         /, 
     ):
         if file is None:
             return self.touch(id_or_path)
         elif isinstance(file, PathLike):
             if ospath.isdir(file):
                 return list(self.upload_tree(file, id_or_path, no_root=True, overwrite=True))
@@ -304,129 +306,121 @@
         return self.__dict__["password"]
 
     @password.setter
     def password(self, /, password: str = ""):
         self.__dict__["password"] = password
 
     @check_response
-    def fs_mkdir(self, name: str, /, pid: int = 0) -> dict:
+    def fs_mkdir(self, name: str, /, pid: int = 0) -> AttrDict:
         return self.client.fs_mkdir({"cname": name, "pid": pid})
 
     @check_response
-    def fs_copy(self, id: int, /, pid: int = 0) -> dict:
+    def fs_copy(self, id: int, /, pid: int = 0) -> AttrDict:
         return self.client.fs_copy(id, pid)
 
     @check_response
-    def fs_delete(self, id: int, /) -> dict:
+    def fs_delete(self, id: int, /) -> AttrDict:
         return self.client.fs_delete(id)
 
     @check_response
-    def fs_move(self, id: int, /, pid: int = 0) -> dict:
+    def fs_move(self, id: int, /, pid: int = 0) -> AttrDict:
         return self.client.fs_move(id, pid)
 
     @check_response
-    def fs_rename(self, id: int, name: str, /) -> dict:
+    def fs_rename(self, id: int, name: str, /) -> AttrDict:
         return self.client.fs_rename(id, name)
 
     @check_response
     def fs_batch_copy(
         self, 
         payload: dict | Iterable[int | str], 
         /, 
         pid: int = 0, 
-    ) -> dict:
+    ) -> AttrDict:
         return self.client.fs_batch_copy(payload, pid)
 
     @check_response
     def fs_batch_delete(
         self, 
         payload: dict | Iterable[int | str], 
         /, 
-    ) -> dict:
+    ) -> AttrDict:
         return self.client.fs_batch_delete(payload)
 
     @check_response
     def fs_batch_move(
         self, 
         payload: dict | Iterable[int | str], 
         /, 
         pid: int = 0, 
-    ) -> dict:
+    ) -> AttrDict:
         return self.client.fs_batch_move(payload, pid)
 
     @check_response
     def fs_batch_rename(
         self, 
         payload: dict | Iterable[tuple[int | str, str]], 
         /, 
-    ) -> dict:
+    ) -> AttrDict:
         return self.client.fs_batch_rename(payload)
 
-    def fs_info(self, id: int, /) -> dict:
+    def fs_info(self, id: int, /) -> AttrDict:
         result = self.client.fs_info({"file_id": id})
         if result["state"]:
             return result
         match result["code"]:
             # {'state': False, 'code': 20018, 'message': '文件不存在或已删除。'}
             case 20018:
                 raise FileNotFoundError(result)
             # {'state': False, 'code': 990002, 'message': '参数错误。'}
             case 990002:
                 raise OSError(errno.EINVAL, result)
             case _:
                 raise OSError(errno.EIO, result)
 
-    def fs_files(
-        self, 
-        /, 
-        id: int = 0, 
-        limit: int = 32, 
-        offset: int = 0, 
-    ) -> dict:
-        resp = check_response(self.client.fs_files({
-            "cid": id, 
-            "limit": limit, 
-            "offset": offset, 
-            "show_dir": 1, 
-        }))
-        if id and int(resp["path"][-1]["cid"]) != id:
-            raise NotADirectoryError(errno.ENOTDIR, f"{id} is not a directory")
+    def fs_files(self, /, payload: dict) -> AttrDict:
+        id = int(payload["id"])
+        resp = check_response(self.client.fs_files(payload))
+        if int(resp["path"][-1]["cid"]) != id:
+            raise NotADirectoryError(errno.ENOTDIR, f"{id!r} is not a directory")
         return resp
 
     @check_response
-    def fs_search(self, payload: str | dict, /) -> dict:
+    def fs_search(self, payload: str | dict, /) -> AttrDict:
         return self.client.fs_search(payload)
 
     @check_response
-    def space_summury(self, /) -> dict:
+    def space_summury(self, /) -> AttrDict:
         return self.client.fs_space_summury()
 
-    def _upload(self, file, name, pid: Optional[int] = None) -> dict:
+    def _upload(
+        self, 
+        /, 
+        file: ( str | PathLike | URL | SupportsGeturl | 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] ), 
+        name: str, 
+        pid: None | int = None, 
+    ) -> AttrDict:
         if pid is None:
             pid = self.id
-        if not hasattr(file, "getbuffer") or len(file.getbuffer()) > 0:
+        data = check_response(self.client.upload_file(file, name, pid))["data"]
+        if "file_id" in data:
+            file_id = int(data["file_id"])
             try:
-                file.seek(0, 1)
-            except:
-                pass
-            else:
-                resp = self.client.upload_file(file, name, pid)
-                name = resp["data"]["file_name"]
-                try:
-                    return self._attr_path([name], pid)
-                except FileNotFoundError:
-                    self.fs_files(pid, 1)
-                    return self._attr_path([name], pid)
-        resp = check_response(self.client.upload_file_sample)(file, name, pid)
-        id = int(resp["data"]["file_id"])
-        try:
-            return self._attr(id)
-        except FileNotFoundError:
-            self.fs_files(pid, 1)
-            return self._attr(id)
+                return self._attr(file_id)
+            except FileNotFoundError:
+                self.fs_files({"cid": pid, "limit": 1})
+                return self._attr(file_id)
+        else:
+            name = data["file_name"]
+            try:
+                return self._attr_path([name], pid)
+            except FileNotFoundError:
+                self.fs_files({"cid": pid, "limit": 1})
+                return self._attr_path([name], pid)
 
     def _clear_cache(self, attr: dict, /):
         attr_cache = self.attr_cache
         if attr_cache is None:
             return
         id = attr["id"]
         pid = attr["parent_id"]
@@ -524,104 +518,14 @@
                                 path_to_id[new_subpath] = subid
                         if subattr["is_directory"]:
                             put(subid)
             if path_to_id is not None and pop_path is not None:
                 for k in tuple(k for k in path_to_id if startswith(k, old_path)):
                     pop_path(k)
 
-    def iterdir(
-        self, 
-        id_or_path: IDOrPathType = "", 
-        /, 
-        pid: None | int = None, 
-        refresh: bool = False, 
-        **kwargs, 
-    ) -> Iterator[AttrDict]:
-        path_to_id = self.path_to_id
-        attr_cache = self.attr_cache
-        get_version = self.get_version
-        version = None
-        if attr_cache is None and isinstance(id_or_path, int):
-            id = id_or_path
-        else:
-            attr = None
-            if not refresh:
-                path_class = type(self).path_class
-                if isinstance(id_or_path, dict):
-                    attr = id_or_path
-                elif isinstance(id_or_path, path_class):
-                    attr = id_or_path.__dict__
-            if attr is None:
-                attr = self.attr(id_or_path, pid)
-            if not attr["is_directory"]:
-                raise NotADirectoryError(
-                    errno.ENOTDIR, 
-                    f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
-                )
-            id = attr["id"]
-            if get_version is not None:
-                version = get_version(attr)
-        if attr_cache is None:
-            pid_attrs = None
-        else:
-            pid_attrs = attr_cache.get(id)
-        if (
-            refresh or 
-            pid_attrs is None or 
-            "version" not in pid_attrs or
-            version != pid_attrs["version"]
-        ):
-            pagesize = 1 << 10
-            def normalize_attr(attr, dirname, /, **extra):
-                attr = normalize_info(attr, **extra)
-                path = attr["path"] = joinpath(dirname, escape(attr["name"]))
-                if path_to_id is not None:
-                    path_to_id[path] = attr["id"]
-                if attr_cache is not None:
-                    try:
-                        id_attrs = attr_cache[attr["id"]]
-                    except LookupError:
-                        attr_cache[attr["id"]] = {"attr": attr}
-                    else:
-                        try:
-                            old_attr = id_attrs["attr"]
-                        except LookupError:
-                            id_attrs["attr"] = attr
-                        else:
-                            if path != old_attr["path"] and path_to_id is not None:
-                                try:
-                                    del path_to_id[old_attr["path"]]
-                                except LookupError:
-                                    pass
-                            old_attr.update(attr)
-                return attr
-            def iterdir():
-                get_files = self.fs_files
-                kwargs["limit"] = pagesize
-                resp = get_files(id, **kwargs)
-                dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
-                if path_to_id is not None:
-                    path_to_id[dirname] = id
-                count = resp["count"]
-                for attr in resp["data"]:
-                    yield normalize_attr(attr, dirname, fs=self)
-                for offset in range(pagesize, count, 1 << 10):
-                    kwargs["offset"] = offset
-                    resp = get_files(id, **kwargs)
-                    if resp["count"] != count:
-                        raise RuntimeError(f"{id} detected count changes during iteration")
-                    for attr in resp["data"]:
-                        yield normalize_attr(attr, dirname, fs=self)
-            children = {a["id"]: a for a in iterdir()}
-            if attr_cache is not None:
-                attrs = attr_cache[id] = {"version": version, "attr": attr, "children": children}
-        else:
-            children = pid_attrs["children"]
-        return iter(children.values())
-
     def _attr(self, id: int, /)  -> AttrDict:
         if id == 0:
             last_update = datetime.now()
             return {
                 "id": 0, 
                 "parent_id": 0, 
                 "name": "", 
@@ -730,282 +634,441 @@
                 if attr["name"] == name:
                     pid = cast(int, attr["id"])
                     break
             else:
                 raise FileNotFoundError(errno.ENOENT, f"no such file {name!r} (in {pid!r})")
         return attr
 
+    def _dir_get_ancestors(self, id: int, /) -> list[dict]:
+        ls = [{"name": "", "id": 0, "parent_id": 0, "is_directory": True}]
+        if id:
+            ls.extend(
+                {"name": p["name"], "id": int(p["cid"]), "parent_id": int(p["pid"]), "is_directory": True} 
+                for p in self.fs_files({"cid": id, "limit": 1})["path"][1:]
+            )
+        return ls
+
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     )  -> AttrDict:
+        "获取属性"
         if isinstance(id_or_path, P115Path):
             return id_or_path.__dict__
         elif isinstance(id_or_path, dict):
             return id_or_path
         elif isinstance(id_or_path, int):
             return self._attr(id_or_path)
         else:
             return self._attr_path(id_or_path, pid)
 
+    def iterdir(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: None | int = None, 
+        refresh: bool = False, 
+        page_size: int = 1_000, 
+        **payload, 
+    ) -> Iterator[AttrDict]:
+        """迭代获取目录内直属的文件或目录的信息
+        payload:
+            - asc: 0 | 1 = 1     # 是否升序排列
+            - code: int | str = <default>
+            - count_folders: 0 | 1 = 1
+            - custom_order: int | str = <default>
+            - fc_mix: 0 | 1 = <default> # 是否文件夹置顶，0 为置顶
+            - format: str = "json"
+            - is_q: 0 | 1 = <default>
+            - is_share: 0 | 1 = <default>
+            - natsort: 0 | 1 = <default>
+            - o: str = "file_name"
+                # 用某字段排序：
+                # - 文件名："file_name"
+                # - 文件大小："file_size"
+                # - 文件种类："file_type"
+                # - 修改时间："user_utime"
+                # - 创建时间："user_ptime"
+                # - 上次打开时间："user_otime"
+            - offset: int = 0    # 索引偏移，索引从 0 开始计算
+            - record_open_time: 0 | 1 = 1
+            - scid: int | str = <default>
+            - show_dir: 0 | 1 = 1
+            - snap: 0 | 1 = <default>
+            - source: str = <default>
+            - star: 0 | 1 = <default> # 是否星标文件
+            - suffix: str = <default> # 后缀名
+            - type: int | str = <default>
+                # 文件类型：
+                # - 所有: 0
+                # - 文档: 1
+                # - 图片: 2
+                # - 音频: 3
+                # - 视频: 4
+                # - 压缩包: 5
+                # - 应用: 6
+                # - 书籍: 7
+        """
+        if page_size <= 0:
+            page_size = 1_000
+        path_to_id = self.path_to_id
+        attr_cache = self.attr_cache
+        get_version = self.get_version
+        version = None
+        if attr_cache is None and isinstance(id_or_path, int):
+            id = id_or_path
+        else:
+            attr = None
+            if not refresh:
+                path_class = type(self).path_class
+                if isinstance(id_or_path, dict):
+                    attr = id_or_path
+                elif isinstance(id_or_path, path_class):
+                    attr = id_or_path.__dict__
+            if attr is None:
+                attr = self.attr(id_or_path, pid)
+            if not attr["is_directory"]:
+                raise NotADirectoryError(
+                    errno.ENOTDIR, 
+                    f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
+                )
+            id = attr["id"]
+            if get_version is not None:
+                version = get_version(attr)
+        payload["cid"] = id
+        payload["limit"] = page_size
+        offset = int(payload.setdefault("offset", 0))
+        if offset < 0:
+            offset = payload["offset"] = 0
+        if attr_cache is None:
+            pid_attrs = None
+        else:
+            pid_attrs = attr_cache.get(id)
+        if (
+            refresh or 
+            pid_attrs is None or 
+            "version" not in pid_attrs or
+            version != pid_attrs["version"]
+        ):
+            def normalize_attr(attr, dirname, /, **extra):
+                attr = normalize_info(attr, **extra)
+                path = attr["path"] = joinpath(dirname, escape(attr["name"]))
+                if path_to_id is not None:
+                    path_to_id[path] = attr["id"]
+                if attr_cache is not None:
+                    try:
+                        id_attrs = attr_cache[attr["id"]]
+                    except LookupError:
+                        attr_cache[attr["id"]] = {"attr": attr}
+                    else:
+                        try:
+                            old_attr = id_attrs["attr"]
+                        except LookupError:
+                            id_attrs["attr"] = attr
+                        else:
+                            if path != old_attr["path"] and path_to_id is not None:
+                                try:
+                                    del path_to_id[old_attr["path"]]
+                                except LookupError:
+                                    pass
+                            old_attr.update(attr)
+                return attr
+            def iterdir():
+                get_files = self.fs_files
+                resp = get_files(payload)
+                dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
+                if path_to_id is not None:
+                    path_to_id[dirname] = id
+                count = resp["count"]
+                for attr in resp["data"]:
+                    yield normalize_attr(attr, dirname, fs=self)
+                for offset in range(page_size, count, 1 << 10):
+                    payload["offset"] = offset
+                    resp = get_files(payload)
+                    if resp["count"] != count:
+                        raise RuntimeError(f"{id} detected count changes during iteration")
+                    for attr in resp["data"]:
+                        yield normalize_attr(attr, dirname, fs=self)
+            if attr_cache is None:
+                return iterdir()
+            else:
+                payload["offset"] = 0
+                children = {a["id"]: a for a in iterdir()}
+                attrs = attr_cache[id] = {"version": version, "attr": attr, "children": children}
+        else:
+            children = pid_attrs["children"]
+        return islice(children.values(), offset, None)
+
     def copy(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
-        overwrite_or_ignore: Optional[bool] = None, 
+        overwrite: bool = False, 
+        onerror: bool | Callable[[OSError], bool] = True, 
         recursive: bool = False, 
-    ) -> Optional[dict]:
-        src_patht = self.get_patht(src_path, pid)
-        dst_patht = self.get_patht(dst_path, pid)
-        src_fullpath = joins(src_patht)
-        dst_fullpath = joins(dst_patht)
-        src_attr = self.attr(src_path, pid)
-        if src_attr["is_directory"]:
-            if recursive:
-                return self.copytree(
-                    src_attr["id"], 
-                    dst_path, 
-                    pid, 
-                    overwrite_or_ignore=overwrite_or_ignore, 
-                )
-            if overwrite_or_ignore == False:
-                return None
-            raise IsADirectoryError(
-                errno.EISDIR, f"source is a directory: {src_fullpath!r} -> {dst_fullpath!r}")
-        if src_patht == dst_patht:
-            if overwrite_or_ignore is None:
-                raise SameFileError(src_fullpath)
-            return None
-        elif dst_patht == src_patht[:len(dst_patht)]:
-            if overwrite_or_ignore == False:
-                return None
-            raise PermissionError(
-                errno.EPERM, 
-                f"copy a path as its ancestor is not allowed: {src_fullpath!r} -> {dst_fullpath!r}", 
-            )
-        elif src_patht == dst_patht[:len(src_patht)]:
-            if overwrite_or_ignore == False:
-                return None
-            raise PermissionError(
-                errno.EPERM, 
-                f"copy a path as its descendant is not allowed: {src_fullpath!r} -> {dst_fullpath!r}", 
-            )
-        *src_dirt, src_name = src_patht
-        *dst_dirt, dst_name = dst_patht
+    ) -> None | AttrDict:
+        "复制文件"
         try:
-            dst_attr = self.attr(dst_path, pid)
-        except FileNotFoundError:
-            if src_dirt == dst_dirt:
-                dst_pid = src_attr["parent_id"]
-            else:
-                destdir_attr = self.attr(dst_dirt)
-                if not destdir_attr["is_directory"]:
-                    raise NotADirectoryError(
-                        errno.ENOTDIR, 
-                        f"parent path {joins(dst_dirt)!r} is not directory: {src_fullpath!r} -> {dst_fullpath!r}", 
+            src_attr = self.attr(src_path, pid)
+            src_path = cast(str, src_attr["path"])
+            if src_attr["is_directory"]:
+                if recursive:
+                    return self.copytree(
+                        src_attr, 
+                        dst_path, 
+                        pid=pid, 
+                        overwrite=overwrite, 
+                        onerror=onerror, 
                     )
-                dst_pid = destdir_attr["id"]
-        else:
-            if dst_attr["is_directory"]:
-                if overwrite_or_ignore == False:
-                    return None
-                raise IsADirectoryError(
-                    errno.EISDIR, 
-                    f"destination is a directory: {src_fullpath!r} -> {dst_fullpath!r}", 
-                )
-            elif overwrite_or_ignore is None:
-                raise FileExistsError(
-                    errno.EEXIST, 
-                    f"destination already exists: {src_fullpath!r} -> {dst_fullpath!r}", 
-                )
-            elif not overwrite_or_ignore:
-                return None
-            self.fs_delete(dst_attr["id"])
-            dst_pid = dst_attr["parent_id"]
-        src_id = src_attr["id"]
-        if splitext(src_name)[1] != splitext(dst_name)[1]:
-            dst_name = check_response(self.client.upload_file_init)(
-                dst_name, 
-                filesize=src_attr["size"], 
-                file_sha1=src_attr["sha1"], 
-                read_range_bytes_or_hash=lambda rng: self.read_bytes_range(src_id, rng), 
-                pid=dst_pid, 
-            )["data"]["file_name"]
-            return self.attr([dst_name], dst_pid)
-        elif src_name == dst_name:
-            self.fs_copy(src_id, dst_pid)
-            return self.attr([src_name], dst_pid)
-        else:
-            tempdir_id = int(self.fs_mkdir(str(uuid4()))["id"])
+                raise IsADirectoryError(errno.EISDIR, f"source path is a directory: {src_path!r}")
+
+            src_patht = self.get_patht(src_path)
+            *src_dirt, src_name = src_patht
+            src_id = src_attr["id"]
             try:
-                self.fs_copy(src_id, tempdir_id)
-                dst_id = self.attr([src_name], tempdir_id)["id"]
-                resp = self.fs_rename(dst_id, dst_name)
-                if resp["data"]:
-                    dst_name = resp["data"][str(dst_id)]
-                self.fs_move(dst_id, dst_pid)
-            finally:
-                self.fs_delete(tempdir_id)
-            return self.attr(dst_id)
+                dst_attr = self.attr(dst_path, pid)
+            except FileNotFoundError:
+                if isinstance(dst_path, int):
+                    raise
+
+                dst_patht = self.get_patht(dst_path, pid)
+                *dst_dirt, dst_name = dst_patht
+                dst_path = joins(dst_patht)
+                if dst_patht == src_patht[:len(dst_patht)]:
+                    raise PermissionError(
+                        errno.EPERM, 
+                        f"copy a file to its ancestor path is not allowed: {src_path!r} -> {dst_path!r}", 
+                    )
+                elif src_patht == dst_patht[:len(src_patht)]:
+                    raise PermissionError(
+                        errno.EPERM, 
+                        f"copy a file to its descendant path is not allowed: {src_path!r} -> {dst_path!r}", 
+                    )
+
+                if src_dirt == dst_dirt:
+                    dst_pid = src_attr["parent_id"]
+                else:
+                    dst_pattr = self.makedirs(dst_patht[:-1])
+                    dst_pid = dst_pattr["id"]
+            else:
+                if src_id == dst_attr["id"]:
+                    raise SameFileError(src_path)
+                elif dst_attr["is_directory"]:
+                    raise IsADirectoryError(
+                        errno.EISDIR, 
+                        f"destination is a directory: {src_path!r} -> {dst_path!r}", 
+                    )
+                elif overwrite:
+                    self.remove(dst_attr)
+                else:
+                    raise FileExistsError(
+                        errno.EEXIST, 
+                        f"destination already exists: {src_path!r} -> {dst_path!r}", 
+                    )
+                dst_pid = dst_attr["parent_id"]
 
-    # TODO: 去除 overwrite_or_ignore 参数，拆分为 overwrite 和 onerror
-    # TODO: 支持多线程操作
+            if splitext(src_name)[1] != splitext(dst_name)[1]:
+                dst_name = check_response(self.client.upload_file_init)(
+                    filename=dst_name, 
+                    filesize=src_attr["size"], 
+                    file_sha1=src_attr["sha1"], 
+                    read_range_bytes_or_hash=lambda rng: self.read_bytes_range(src_id, rng), 
+                    pid=dst_pid, 
+                )["data"]["file_name"]
+                return self.attr([dst_name], dst_pid)
+            elif src_name == dst_name:
+                self.fs_copy(src_id, dst_pid)
+                return self.attr([dst_name], dst_pid)
+            else:
+                tempdir_id = int(self.fs_mkdir(str(uuid4()))["id"])
+                try:
+                    self.fs_copy(src_id, tempdir_id)
+                    dst_id = self.attr([src_name], tempdir_id)["id"]
+                    resp = self.fs_rename(dst_id, dst_name)
+                    if resp["data"]:
+                        dst_name = resp["data"][str(dst_id)]
+                    self.fs_move(dst_id, dst_pid)
+                finally:
+                    self.fs_delete(tempdir_id)
+                return self.attr(dst_id)
+        except OSError as e:
+            if onerror is True:
+                raise
+            elif onerror is False:
+                pass
+            else:
+                onerror(e)
+            return None
+
+    # TODO: 使用 fs_batch_* 方法，尽量加快执行速度，但是如果任务数过大（大于 5 万）而报错，则尝试对任务进行拆分
+    # TODO: 删除、还原、复制、移动等操作均遵此例，也就是尽量用 batch 方法
     def copytree(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType = "", 
         pid: None | int = None, 
-        overwrite_or_ignore: Optional[bool] = None, 
-        **kwargs, 
-    ) -> Optional[dict]:
-        src_attr = self.attr(src_path, pid)
-        src_id = src_attr["id"]
-        if not src_attr["is_directory"]:
-            return self.copy(
-                src_id, 
-                dst_path, 
-                pid, 
-                overwrite_or_ignore=overwrite_or_ignore, 
-            )
-        src_name = src_attr["name"]
-        src_fullpath = src_attr["path"]
+        overwrite: bool = False, 
+        onerror: bool | Callable[[OSError], bool] = True, 
+    ) -> None | AttrDict:
+        "复制路径"
         try:
-            dst_attr = self.attr(dst_path, pid)
-        except FileNotFoundError:
-            if isinstance(dst_path, int):
-                if overwrite_or_ignore == False:
-                    return None
-                raise
-            dst_patht = self.get_patht(dst_path, pid)
-            if len(dst_patht) == 1:
-                dst_attr = self.attr(0)
-                dst_id = 0
+            src_attr = self.attr(src_path, pid)
+            if not src_attr["is_directory"]:
+                return self.copy(
+                    src_attr, 
+                    dst_path, 
+                    pid=pid, 
+                    overwrite=overwrite, 
+                    onerror=onerror, 
+                )
+
+            src_id = src_attr["id"]
+            src_path = src_attr["path"]
+            src_name = src_attr["name"]
+            try:
+                dst_attr = self.attr(dst_path, pid)
+            except FileNotFoundError:
+                if isinstance(dst_path, int):
+                    raise
+                dst_patht = self.get_patht(dst_path, pid)
+                if len(dst_patht) == 1:
+                    dst_id = 0
+                    dst_name = src_name
+                else:
+                    dst_pattr = self.makedirs(dst_patht[:-1], exist_ok=True)
+                    dst_id = dst_pattr["id"]
+                    dst_name = dst_patht[-1]
+                try:
+                    if src_name == dst_name:
+                        self.fs_copy(src_id, dst_id)
+                        return self.attr([dst_name], dst_id)
+                except (OSError, JSONDecodeError):
+                    pass
+                dst_attr = self.makedirs([dst_name], pid=dst_id, exist_ok=True)
+                dst_id = dst_pattr["id"]
+                dst_attrs_map = {}
             else:
-                dst_attr = self.makedirs(dst_patht[:-1], exist_ok=True)
-                dst_id = dst_attr["id"]
-                if src_name == dst_patht[-1]:
-                    self.fs_copy(src_id, dst_id)
-                    return self.attr([src_name], dst_id)
-                dst_attr = self.makedirs([src_name], dst_id, exist_ok=True)
+                dst_path = dst_attr["path"]
+                if not dst_attr["is_directory"]:
+                    raise NotADirectoryError(
+                        errno.ENOTDIR, 
+                        f"destination path {dst_path!r} is not directory", 
+                    )
                 dst_id = dst_attr["id"]
-        else:
-            dst_id = dst_attr["id"]
-            dst_fullpath = dst_attr["path"]
-            if src_fullpath == dst_fullpath:
-                if overwrite_or_ignore is None:
-                    raise SameFileError(dst_fullpath)
-                return None
-            elif any(a["id"] == src_id for a in self.get_ancestors(dst_id)):
-                if overwrite_or_ignore == False:
-                    return None
-                raise PermissionError(
-                    errno.EPERM, 
-                    f"copy a directory as its descendant is not allowed: {src_fullpath!r} -> {dst_fullpath!r}", 
-                )
-            elif not dst_attr["is_directory"]:
-                if overwrite_or_ignore == False:
-                    return None
-                raise NotADirectoryError(
-                    errno.ENOTDIR, 
-                    f"destination is not directory: {src_fullpath!r} -> {dst_fullpath!r}", 
-                )
-            elif overwrite_or_ignore is None:
-                raise FileExistsError(
-                    errno.EEXIST, 
-                    f"destination already exists: {src_fullpath!r} -> {dst_fullpath!r}", 
-                )
-        for attr in self.iterdir(src_id, **kwargs):
-            if attr["is_directory"]:
-                self.copytree(
-                    attr["id"], 
-                    [attr["name"]], 
-                    dst_id, 
-                    overwrite_or_ignore=overwrite_or_ignore, 
-                )
+                if src_id == dst_id:
+                    raise SameFileError(src_path)
+                elif any(a["id"] == src_id for a in self.get_ancestors(dst_id)):
+                    raise PermissionError(
+                        errno.EPERM, 
+                        f"copy a directory as its descendant is not allowed: {src_path!r} -> {dst_path!r}", 
+                    )
+                dst_attrs_map = {a["name"]: a for a in self.listdir_attr(dst_id)}
+
+            src_attrs = self.listdir_attr(src_id)
+        except OSError as e:
+            if onerror is True:
+                raise
+            elif onerror is False:
+                pass
             else:
-                self.copy(
-                    attr["id"], 
-                    [attr["name"]], 
-                    dst_id, 
-                    overwrite_or_ignore=overwrite_or_ignore, 
-                )
-        return self.attr(dst_attr["id"])
+                onerror(e)
+            return None
 
-    def _dir_get_ancestors(self, id: int, /) -> list[dict]:
-        ls = [{"name": "", "id": 0, "parent_id": 0, "is_directory": True}]
-        if id:
-            ls.extend(
-                {"name": p["name"], "id": int(p["cid"]), "parent_id": int(p["pid"]), "is_directory": True} 
-                for p in self.fs_files(id, limit=1)["path"][1:]
-            )
-        return ls
+        src_files: list[int] = []
+        payload: dict = dict(pid=dst_id, overwrite=overwrite, onerror=onerror)
+        for attr in src_attrs:
+            payload["src_path"] = attr
+            if attr["name"] in dst_attrs_map:
+                payload["dst_path"] = dst_attrs_map[attr["name"]]
+                if attr["is_directory"]:
+                    self.copytree(**payload)
+                else:
+                    self.copy(**payload)
+            elif attr["is_directory"]:
+                payload["dst_path"] = [attr["name"]]
+                self.copytree(**payload)
+            else:
+                src_files.append(attr["id"])
+        if src_files:
+            for i in range(0, len(src_files), 50_000):
+                self.fs_batch_copy(src_files[i:i+50_000], dst_id)
+        return dst_attr
 
     def desc(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
         desc: None | str = None, 
     ) -> str:
+        """目录的描述文本（支持 HTML）
+        :param desc: 如果为 None，返回描述文本；否则，设置文本
+        """
         fid = self.get_id(id_or_path, pid)
         if fid == 0:
             return ""
         if desc is None:
             return check_response(self.client.fs_desc_get(fid))["desc"]
         else:
             return check_response(self.client.fs_desc(fid, desc))["file_description"]
 
     def get_ancestors(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> list[dict]:
+        "获取各个上级目录的少量信息（从根目录到当前目录）"
         attr = self.attr(id_or_path, pid)
         ls = self._dir_get_ancestors(attr["parent_id"])
         ls.append({"name": attr["name"], "id": attr["id"], "parent_id": attr["parent_id"], "is_directory": attr["is_directory"]})
         return ls
 
     def dirlen(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
     ) -> int:
-        return self.fs_files(self.get_id(id_or_path, pid), limit=1)["count"]
+        "文件夹中的项目数（直属的文件和目录计数）"
+        return self.fs_files({"cid": self.get_id(id_or_path, pid), "limit": 1})["count"]
 
     def get_id_from_pickcode(self, /, pickcode: str = "") -> int:
+        "由 pickcode 获取 id"
         if not pickcode:
             return 0
         return self.get_info_from_pickcode(pickcode)["id"]
 
-    def get_info_from_pickcode(self, /, pickcode: str) -> dict:
+    def get_info_from_pickcode(self, /, pickcode: str) -> AttrDict:
+        "由 pickcode 获取一些目录信息"
         return self.client.download_url(pickcode, strict=False, detail=True).__dict__
 
     def get_pickcode(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
     ) -> str:
+        "获取 pickcode"
         return self.attr(id_or_path, pid).get("pickcode", "")
 
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
     ) -> str:
+        "获取下载链接"
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
         return self.client.download_url(
             attr["pickcode"], 
             use_web_api=attr.get("violated", False) and attr["size"] < 1024 * 1024 * 115, 
             detail=detail, 
@@ -1015,57 +1078,63 @@
     def get_url_from_pickcode(
         self, 
         /, 
         pickcode: str, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
     ) -> str:
+        "由 pickcode 获取下载链接"
         return self.client.download_url(
             pickcode, 
             detail=detail, 
             headers=headers, 
         )
 
+    # TODO: 如果超过 5 万个文件，则需要分批进入隐藏模式
     def hide(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
         show: None | bool = None, 
     ) -> bool:
+        "把路径隐藏或显示（如果隐藏，只能在隐藏模式中看到）"
         if show is None:
             return self.attr(id_or_path, pid)["hidden"]
         else:
             fid = self.get_id(id_or_path, pid)
             if fid == 0:
                 return False
             hidden = not show
             check_response(self.client.fs_files_hidden({"hidden": int(hidden), "fid[0]": fid}))
             return hidden
 
     @property
     def hidden_mode(self, /) -> bool:
+        "是否进入隐藏模式"
         return self.client.user_setting()["data"]["show"] == "1"
 
     def hidden_switch(
         self, 
         /, 
         show: None | bool = None, 
         password: str = "", 
     ):
+        "切换隐藏模式，如果需要进入隐藏模式，需要提供密码"
         if show is None:
             show = not self.hidden_mode
         check_response(self.client.fs_hidden_switch({"show": int(show), "safe_pwd": password or self.password}))
 
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> bool:
+        "路径是否为空文件或空目录"
         attr: dict | P115Path
         if isinstance(id_or_path, P115Path):
             attr = id_or_path
         else:
             try:
                 attr = self.attr(id_or_path, pid)
             except FileNotFoundError:
@@ -1076,15 +1145,16 @@
 
     def iter_repeat(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
         page_size: int = 1150, 
-    ) -> Iterator[dict]:
+    ) -> Iterator[AttrDict]:
+        "获取重复文件（不含当前这个）"
         if page_size <= 0:
             page_size = 1150
         payload = {
             "file_id": self.get_id(id_or_path, pid), 
             "offset": 0, 
             "limit": page_size, 
             "format": "json", 
@@ -1098,23 +1168,25 @@
 
     def labels(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> list[dict]:
+        "获取路径的标签"
         return self.attr(id_or_path, pid)["labels"]
 
     def makedirs(
         self, 
         path: str | PathLike[str] | Sequence[str] | AttrDict, 
         /, 
         pid: None | int = None, 
         exist_ok: bool = False, 
-    ) -> dict:
+    ) -> AttrDict:
+        "创建目录，如果上级目录不存在，则会进行创建"
         if isinstance(path, dict):
             patht, parents = splits(path["path"])
         elif isinstance(path, (str, PathLike)):
             patht, parents = splits(fspath(path))
         else:
             patht = [p for p in path if p]
             parents = 0
@@ -1137,27 +1209,33 @@
                 exists = False
                 resp = self.fs_mkdir(name, pid)
                 pid = int(resp["cid"])
                 attr = get_attr(pid)
             else:
                 exists = True
                 if not attr["is_directory"]:
-                    raise NotADirectoryError(errno.ENOTDIR, f"{path!r} (in {pid!r}): there is a superior non-directory")
+                    raise NotADirectoryError(
+                        errno.ENOTDIR, 
+                        f"{path!r} (in {pid!r}): there is a superior non-directory", 
+                    )
                 pid = attr["id"]
         if not exist_ok and exists:
             raise FileExistsError(errno.EEXIST, f"{path!r} (in {pid!r}) exists")
         return attr
 
     def mkdir(
         self, 
-        path: str | PathLike[str] | Sequence[str], 
+        path: IDOrPathType, 
         /, 
         pid: None | int = None, 
-    ) -> dict:
-        if isinstance(path, (str, PathLike)):
+    ) -> AttrDict:
+        "创建目录"
+        if isinstance(path, (int, dict)):
+            return self.attr(path)
+        elif isinstance(path, (str, PathLike)):
             patht, parents = splits(fspath(path))
         else:
             patht = [p for p in path if p]
             parents = 0
         if not patht or patht == [""]:
             raise OSError(errno.EINVAL, f"invalid path: {path!r}")
         if pid is None:
@@ -1170,290 +1248,340 @@
         for i, name in enumerate(patht, 1):
             try:
                 attr = get_attr([name], pid)
             except FileNotFoundError:
                 break
             else:
                 if not attr["is_directory"]:
-                    raise NotADirectoryError(errno.ENOTDIR, f"{attr['id']!r} ({name!r} in {pid!r}) not a directory")
+                    raise NotADirectoryError(
+                        errno.ENOTDIR, 
+                        f"{attr['id']!r} ({name!r} in {pid!r}) not a directory", 
+                    )
                 pid = attr["id"]
         else:
-            raise FileExistsError(errno.EEXIST, f"{path!r} (in {pid!r}) already exists")
+            raise FileExistsError(
+                errno.EEXIST, f"{path!r} (in {pid!r}) already exists")
         if i < len(patht):
-            raise FileNotFoundError(errno.ENOENT, f"{path!r} (in {pid!r}) missing superior directory")
+            raise FileNotFoundError(
+                errno.ENOENT, 
+                f"{path!r} (in {pid!r}) missing superior directory", 
+            )
         resp = self.fs_mkdir(name, pid)
         return self.attr(int(resp["cid"]))
 
     def move(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
-    ) -> Optional[dict]:
+    ) -> AttrDict:
+        "重命名路径，如果目标路径是目录，则移动到其中"
         try:
             dst_attr = self.attr(dst_path, pid)
         except FileNotFoundError:
             return self.rename(src_path, dst_path, pid)
         src_attr = self.attr(src_path, pid)
         src_id = src_attr["id"]
         dst_id = dst_attr["id"]
         if src_id == dst_id or src_attr["parent_id"] == dst_id:
-            return None
+            return src_attr
+        src_path = src_attr["path"]
+        dst_path = dst_attr["path"]
         if any(a["id"] == src_id for a in self.get_ancestors(dst_id)):
-            raise PermissionError(errno.EPERM, f"move a path to its subordinate path is not allowed: {src_id!r} -> {dst_id!r}")
+            raise PermissionError(
+                errno.EPERM, 
+                f"move a path to its subordinate path is not allowed: {src_path!r} -> {dst_path!r}"
+            )
         if dst_attr["is_directory"]:
-            name = src_attr["name"]
-            if self.exists([name], dst_id):
-                raise FileExistsError(errno.EEXIST, f"destination {name!r} (in {dst_id!r}) already exists")
-            self.fs_move(src_id, dst_id)
-            new_attr = self.attr(src_id)
-            self._update_cache_path(src_attr, new_attr)
-            return new_attr
-        raise FileExistsError(errno.EEXIST, f"destination {dst_id!r} already exists")
+            return self.rename(src_attr, [src_attr["name"]], pid=dst_attr["id"])
+        raise FileExistsError(
+            errno.EEXIST, 
+            f"destination already exists: {src_path!r} -> {dst_path!r}", 
+        )
 
-    # TODO: 由于 115 网盘不支持删除里面有超过 5 万个文件等文件夹，因此需要增加参数，支持在失败后，拆分任务，返回一个 Future 对象，可以获取已完成和未完成，并且可以随时取消
+    # TODO: 由于 115 网盘不支持删除里面有超过 5 万个文件等目录，因此执行失败时需要拆分任务
+    # TODO: 就算删除和还原执行返回成功，后台可能依然在执行，需要等待前一批完成再执行下一批
     def remove(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
         recursive: bool = False, 
-    ) -> dict:
+    ) -> AttrDict:
+        "删除文件"
         attr = self.attr(id_or_path, pid)
         id = attr["id"]
-        clear_cache = self._clear_cache
         if attr["is_directory"]:
             if not recursive:
-                raise IsADirectoryError(errno.EISDIR, f"{id_or_path!r} (in {pid!r}) is a directory")
+                raise IsADirectoryError(
+                    errno.EISDIR, 
+                    f"{attr['path']!r} (id={id!r}) is a directory", 
+                )
             if id == 0:
                 for subattr in self.iterdir(0):
-                    id = subattr["id"]
-                    self.fs_delete(id)
-                    clear_cache(subattr)
+                    self.remove(subattr, recursive=True)
                 return attr
         self.fs_delete(id)
-        clear_cache(attr)
+        self._clear_cache(attr)
         return attr
 
     def removedirs(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
-    ) -> Optional[dict]:
-        try:
-            attr = self.attr(id_or_path, pid)
-        except FileNotFoundError:
-            return None
+    ) -> AttrDict:
+        "逐级往上尝试删除空目录"
+        attr = self.attr(id_or_path, pid)
+        id = attr["id"]
         if not attr["is_directory"]:
-            raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
+            raise NotADirectoryError(
+                errno.ENOTDIR, 
+                f"{attr['path']!r} (id={id!r}) is not a directory", 
+            )
         delid = 0
-        pid = attr["id"]
         pattr = attr
         get_files = self.fs_files
-        while pid:
-            files = get_files(pid, limit=1)
+        while id:
+            files = get_files({"id": id, "limit": 1})
             if files["count"] > 1:
                 break
-            delid = pid
-            pid = int(files["path"][-1]["pid"])
+            delid = id
+            id = int(files["path"][-1]["pid"])
             pattr = {
                 "id": delid, 
-                "parent_id": pid, 
+                "parent_id": id, 
                 "is_directory": True, 
                 "path": "/" + joins([p["name"] for p in files["path"][1:]]), 
             }
-        if delid == 0:
-            return None
-        self.fs_delete(delid)
-        self._clear_cache(pattr)
+        if delid:
+            self.fs_delete(delid)
+            self._clear_cache(pattr)
         return attr
 
-    # TODO: 支持 dst_path 从 src_path 开始的相对路径
     def rename(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
         replace: bool = False, 
-    ) -> Optional[dict]:
-        src_patht = self.get_patht(src_path, pid)
-        dst_patht = self.get_patht(dst_path, pid)
-        src_fullpath = joins(src_patht)
-        dst_fullpath = joins(dst_patht)
-        if src_patht == dst_patht:
-            return None
-        elif dst_patht == src_patht[:len(dst_patht)]:
-            raise PermissionError(errno.EPERM, f"rename a path as its ancestor is not allowed: {src_fullpath!r} -> {dst_fullpath!r}")
-        elif src_patht == dst_patht[:len(src_patht)]:
-            raise PermissionError(errno.EPERM, f"rename a path as its descendant is not allowed: {src_fullpath!r} -> {dst_fullpath!r}")
-        *src_dirt, src_name = src_patht
-        *dst_dirt, dst_name = dst_patht
+    ) -> AttrDict:
+        "重命名路径"
         src_attr = self.attr(src_path, pid)
         src_id = src_attr["id"]
-        src_id_str = str(src_id)
-        src_ext = splitext(src_name)[1]
-        dst_ext = splitext(dst_name)[1]
-        def get_result(resp):
-            if resp["data"]:
-                new_attr = self._attr(src_id)
-                self._update_cache_path(src_attr, new_attr)
-                return new_attr
-            return None
+        src_path = src_attr["path"]
+        src_patht = self.get_patht(src_path)
         try:
             dst_attr = self.attr(dst_path, pid)
         except FileNotFoundError:
-            if src_dirt == dst_dirt and (src_attr["is_directory"] or src_ext == dst_ext):
-                return get_result(self.fs_rename(src_id, dst_name))
-            destdir_attr = self.attr(dst_dirt)
-            if not destdir_attr["is_directory"]:
-                raise NotADirectoryError(errno.ENOTDIR, f"parent path {joins(dst_dirt)!r} is not directory: {src_fullpath!r} -> {dst_fullpath!r}")
-            dst_pid = destdir_attr["id"]
+            dst_patht = self.get_patht(dst_path, pid)
+            dst_path = joins(dst_patht)
+            if dst_patht == src_patht[:len(dst_patht)]:
+                raise PermissionError(
+                    errno.EPERM, 
+                    f"rename a path to its ancestor is not allowed: {src_path!r} -> {dst_path!r}", 
+                )
+            elif src_patht == dst_patht[:len(src_patht)]:
+                raise PermissionError(
+                    errno.EPERM, 
+                    f"rename a path to its descendant is not allowed: {src_path!r} -> {dst_path!r}", 
+                )
+            dst_pattr = self.makedirs(dst_patht[:-1], exist_ok=True)
+            dst_pid = dst_pattr["id"]
         else:
+            dst_id = dst_attr["id"]
+            if src_id == dst_id:
+                return dst_attr
             if replace:
                 if src_attr["is_directory"]:
                     if dst_attr["is_directory"]:
                         if self.dirlen(dst_attr["id"]):
-                            raise OSError(errno.ENOTEMPTY, f"source is directory, but destination is non-empty directory: {src_fullpath!r} -> {dst_fullpath!r}")
+                            raise OSError(
+                                errno.ENOTEMPTY, 
+                                f"source is directory, but destination is non-empty directory: {src_path!r} -> {dst_path!r}", 
+                            )
                     else:
-                        raise NotADirectoryError(errno.ENOTDIR, f"source is directory, but destination is not a directory: {src_fullpath!r} -> {dst_fullpath!r}")
+                        raise NotADirectoryError(
+                            errno.ENOTDIR, 
+                            f"source is directory, but destination is not a directory: {src_path!r} -> {dst_path!r}", 
+                        )
                 elif dst_attr["is_directory"]:
-                    raise IsADirectoryError(errno.EISDIR, f"source is file, but destination is directory: {src_fullpath!r} -> {dst_fullpath!r}")
-                self.fs_delete(dst_attr["id"])
+                    raise IsADirectoryError(
+                        errno.EISDIR, 
+                        f"source is file, but destination is directory: {src_path!r} -> {dst_path!r}", 
+                    )
+                self.fs_delete(dst_id)
             else:
-                raise FileExistsError(errno.EEXIST, f"destination already exists: {src_fullpath!r} -> {dst_fullpath!r}")
+                raise FileExistsError(
+                    errno.EEXIST, 
+                    f"destination already exists: {src_path!r} -> {dst_path!r}", 
+                )
             dst_pid = dst_attr["parent_id"]
-        if not (src_attr["is_directory"] or src_ext == dst_ext):
-            name = check_response(self.client.upload_file_init)(
+            dst_path = dst_attr["path"]
+            dst_patht = self.get_patht(dst_path)
+
+        *src_dirt, src_name = src_patht
+        *dst_dirt, dst_name = dst_patht
+        src_ext = splitext(src_name)[1]
+        dst_ext = splitext(dst_name)[1]
+
+        if src_dirt == dst_dirt and (src_attr["is_directory"] or src_ext == dst_ext):
+            self.fs_rename(src_id, dst_name)
+        elif src_name == dst_name:
+            self.fs_move(src_id, dst_pid)
+        elif not src_attr["is_directory"] and src_ext != dst_ext:
+            dst_name = check_response(self.client.upload_file_init)(
                 dst_name, 
                 filesize=src_attr["size"], 
                 file_sha1=src_attr["sha1"], 
                 read_range_bytes_or_hash=lambda rng: self.read_bytes_range(src_id, rng), 
                 pid=dst_pid, 
             )["data"]["file_name"]
             self.fs_delete(src_id)
-            new_attr = self._attr_path([name], dst_pid)
-            self._update_cache_path(src_attr, new_attr)
-            return new_attr
-        if src_name == dst_name:
-            self.fs_move(src_id, dst_pid)
-            new_attr = self._attr(src_id)
-            self._update_cache_path(src_attr, new_attr)
-            return new_attr
-        elif src_dirt == dst_dirt:
-            return get_result(self.fs_rename(src_id, dst_name))
+            return self.attr([dst_name], dst_pid)
         else:
             self.fs_rename(src_id, str(uuid4()))
             try:
                 self.fs_move(src_id, dst_pid)
                 try:
-                    return get_result(self.fs_rename(src_id, dst_name))
+                    self.fs_rename(src_id, dst_name)
                 except:
                     self.fs_move(src_id, src_attr["parent_id"])
                     raise
             except:
                 self.fs_rename(src_id, src_name)
                 raise
+        return self.attr(src_id)
 
     def renames(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
-    ) -> Optional[dict]:
-        result = self.rename(src_path, dst_path, pid=pid)
-        if result:
-            self.removedirs(result["parent_id"])
-            return result
-        return None
+    ) -> AttrDict:
+        "重命名路径，如果文件被移动到其它目录中，则尝试从原来的上级目录逐级往上删除空目录"
+        attr = self.attr(src_path, pid)
+        parent_id = attr["parent_id"]
+        attr = self.rename(attr, dst_path, pid=pid)
+        if parent_id != attr["parent_id"]:
+            self.removedirs(parent_id)
+        return attr
 
     def replace(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: None | int = None, 
-    ) -> Optional[dict]:
+    ) -> AttrDict:
+        "替换路径"
         return self.rename(src_path, dst_path, pid=pid, replace=True)
 
     def rmdir(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
-    ) -> dict:
+    ) -> AttrDict:
+        "删除空目录"
         attr = self.attr(id_or_path, pid)
         id = attr["id"]
         if id == 0:
             raise PermissionError(errno.EPERM, "remove the root directory is not allowed")
         elif not attr["is_directory"]:
             raise NotADirectoryError(errno.ENOTDIR, f"{id_or_path!r} (in {pid!r}) is not a directory")
-        elif self.fs_files(id, limit=1)["count"]:
+        elif self.fs_files({"id": id, "limit": 1})["count"]:
             raise OSError(errno.ENOTEMPTY, f"directory is not empty: {id_or_path!r} (in {pid!r})")
         self.fs_delete(id)
         self._clear_cache(attr) 
         return attr
 
     def rmtree(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
-    ) -> dict:
+    ) -> AttrDict:
+        "删除路径"
         return self.remove(id_or_path, pid, recursive=True)
 
     def score(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
         score: None | int = None, 
     ) -> int:
+        """路径的分数
+        :param star: 如果为 None，返回分数；否则，设置分数
+        """
         if score is None:
             return self.attr(id_or_path, pid).get("score", 0)
         else:
             fid = self.get_id(id_or_path, pid)
             if fid == 0:
                 return 0
             self.client.fs_score(fid, score)
             return score
 
     def search(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
-        search_value: str = "", 
         page_size: int = 1_000, 
-        offset: int = 0, 
-        **kwargs, 
+        **payload, 
     ) -> Iterator[P115Path]:
-        assert page_size > 0
+        """搜索目录
+        :param payload:
+            - asc: 0 | 1 = <default> # 是否升序排列
+            - count_folders: 0 | 1 = <default>
+            - date: str = <default> # 筛选日期
+            - fc_mix: 0 | 1 = <default> # 是否目录置顶，0 为置顶
+            - file_label: int | str = <default> # 标签 id
+            - format: str = "json" # 输出格式（不用管）
+            - o: str = <default>
+                # 用某字段排序：
+                # - 文件名："file_name"
+                # - 文件大小："file_size"
+                # - 文件种类："file_type"
+                # - 修改时间："user_utime"
+                # - 创建时间："user_ptime"
+                # - 上次打开时间："user_otime"
+            - offset: int = 0  # 索引偏移，索引从 0 开始计算
+            - pick_code: str = <default>
+            - search_value: str = <default>
+            - show_dir: 0 | 1 = 1
+            - source: str = <default>
+            - star: 0 | 1 = <default>
+            - suffix: str = <default>
+            - type: int | str = <default>
+                # 文件类型：
+                # - 所有: 0
+                # - 文档: 1
+                # - 图片: 2
+                # - 音频: 3
+                # - 视频: 4
+                # - 压缩包: 5
+                # - 应用: 6
+                # - 书籍: 7
+        """
+        if page_size <= 0:
+            page_size = 1_000
         attr = self.attr(id_or_path, pid)
-        if attr["is_directory"]:
-            if not search_value:
-                return
-            id = attr["id"]
-        else:
-            if not search_value:
-                search_value = attr["sha1"]
-            id = 0
-        payload = {
-            "cid": id, 
-            "search_value": search_value, 
-            "limit": page_size, 
-            "offset": offset, 
-            **kwargs, 
-        }
-        def wrap(attr):
-            attr = normalize_info(attr, fs=self)
-            return P115Path(attr)
+        payload["cid"] = attr["id"]
+        payload["limit"] = page_size
+        offset = int(payload.setdefault("offset", 0))
+        if offset < 0:
+            payload["offset"] = 0
+        if not attr["is_directory"]:
+            payload.setdefault("search_value", attr["sha1"])
         search = self.fs_search
         while True:
             resp = search(payload)
             if resp["offset"] != offset:
                 break
             data = resp["data"]
             if not data:
@@ -1468,14 +1596,17 @@
     def star(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
         star: None | bool = None, 
     ) -> bool:
+        """路径的星标
+        :param star: 如果为 None，返回星标是否已设置；如果为 True，设置星标；如果为 False，取消星标
+        """
         if star is None:
             return self.attr(id_or_path, pid).get("star", False)
         else:
             fid = self.get_id(id_or_path, pid)
             if fid == 0:
                 return False
             check_response(self.client.fs_star(fid, star))
@@ -1483,14 +1614,15 @@
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> stat_result:
+        "检查路径的属性，就像 `os.stat`"
         attr = self.attr(id_or_path, pid)
         is_dir = attr["is_directory"]
         return stat_result((
             (S_IFDIR if is_dir else S_IFREG) | 0o777, # mode
             cast(int, attr["id"]), # ino
             cast(int, attr["parent_id"]), # dev
             1, # nlink
@@ -1503,32 +1635,41 @@
         ))
 
     def touch(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
-    ) -> dict:
+        is_dir: bool = False, 
+    ) -> AttrDict:
+        """检查路径是否存在，当不存在时，如果 is_dir 是 False 时，则创建空文件，否则创建空目录
+        """
         try:
             return self.attr(id_or_path, pid)
         except FileNotFoundError:
             if isinstance(id_or_path, int):
                 raise ValueError(f"no such id: {id_or_path!r}")
-            return self.upload(BytesIO(), id_or_path, pid=pid)
+            elif is_dir:
+                return self.mkdir(id_or_path, pid)
+            else:
+                return self.upload(b"", id_or_path, pid=pid)
 
     # TODO: 增加功能，返回一个 Task 对象，可以获取上传进度，可随时取消
+    # TODO: 参数 file 支持更多类型
     def upload(
         self, 
         /, 
-        file: bytes | str | PathLike | SupportsRead[bytes], 
+        file: ( str | PathLike | URL | SupportsGeturl | 
+                Buffer | SupportsRead[Buffer] | Iterable[Buffer] ), 
         path: IDOrPathType = "", 
         pid: None | int = None, 
         overwrite: bool = False, 
-        remove_success: bool = False, 
-    ) -> dict:
+        remove_done: bool = False, 
+    ) -> AttrDict:
+        "上传文件"
         name: str = ""
         if not path:
             pid = self.id if pid is None else self.get_id(pid)
         else:
             attr: Mapping
             if isinstance(path, int):
                 attr = self.attr(path)
@@ -1559,54 +1700,38 @@
                 elif overwrite:
                     self.remove(attr)
                     name = attr["name"]
                     pid = attr["parent_id"]
                 else:
                     raise FileExistsError(errno.EEXIST, f"remote path {attr['path']!r} already exists")
 
-        fio: SupportsRead[bytes]
-        if isinstance(file, SupportsRead):
-            fio = file
-            if not name:
-                try:
-                    name = ospath.basename(getattr(file, "name"))
-                except:
-                    pass
-        elif isinstance(file, (str, PathLike)):
-            file = fsdecode(file)
-            fio = open(file, "rb")
-            if not name:
-                name = ospath.basename(file)
-        else:
-            fio = BytesIO(file)
-
-        resp = self._upload(fio, name, pid)
-        if remove_success and isinstance(file, (str, PathLike)):
+        resp = self._upload(file, name, pid)
+        if remove_done and isinstance(file, (str, PathLike)):
             try:
                 remove(file)
             except OSError:
                 pass
         return resp
 
-    # TODO: 为了提升速度，之后会支持多线程上传，以及直接上传不做检查
+    # TODO: 上传和下载都要支持多线程
     # TODO: 返回上传任务的迭代器，包含进度相关信息，以及最终的响应信息
-    # TODO: 增加参数，predicate
     # TODO: 增加参数，submit，可以把任务提交给线程池
     def upload_tree(
         self, 
         /, 
         local_path: str | PathLike[str] = ".", 
         path: IDOrPathType = "", 
         pid: None | int = None, 
         no_root: bool = False, 
         overwrite: bool = False, 
-        remove_success: bool = False, 
+        remove_done: bool = False, 
         predicate: None | Callable[[Path], bool] = None, 
-        onerror: bool | Callable[[OSError], bool] = False, 
-    ) -> Iterator[dict]:
+        onerror: bool | Callable[[OSError], bool] = True, 
+    ) -> Iterator[AttrDict]:
+        "上传到路径"
         remote_path_attr_map: None | dict[str, dict] = None
         try:
             attr = self.attr(path, pid)
         except FileNotFoundError:
             if isinstance(path, int):
                 raise ValueError(f"no such id: {path!r}")
             attr = self.makedirs(path, pid=pid, exist_ok=True)
@@ -1631,15 +1756,15 @@
             except NotADirectoryError:
                 try:
                     yield self.upload(
                         local_path, 
                         [ospath.basename(local_path)], 
                         pid=pid, 
                         overwrite=overwrite, 
-                        remove_success=remove_success, 
+                        remove_done=remove_done, 
                     )
                 except OSError as e:
                     if onerror is True:
                         raise e
                     elif onerror is False:
                         pass
                     else:
@@ -1686,87 +1811,86 @@
                 if remote_path_attr is None:
                     yield from self.upload_tree(
                         entry, 
                         [name], 
                         pid=pid, 
                         no_root=True, 
                         overwrite=overwrite, 
-                        remove_success=remove_success, 
+                        remove_done=remove_done, 
                         onerror=onerror, 
                     )
                 else:
                     yield from self.upload_tree(
                         entry, 
                         remote_path_attr, 
                         no_root=True, 
                         overwrite=overwrite, 
-                        remove_success=remove_success, 
+                        remove_done=remove_done, 
                         onerror=onerror, 
                     )
-                if remove_success:
+                if remove_done:
                     try:
                         rmdir(entry)
                     except OSError:
                         pass
             else:
                 try:
                     if remote_path_attr is None:
                         yield self.upload(
                             entry, 
                             [name], 
                             pid=pid, 
                             overwrite=overwrite, 
-                            remove_success=remove_success, 
+                            remove_done=remove_done, 
                         )
                     else:
                         yield self.upload(
                             entry, 
                             remote_path_attr, 
                             overwrite=overwrite, 
-                            remove_success=remove_success, 
+                            remove_done=remove_done, 
                         )
                 except OSError as e:
                     if onerror is True:
                         raise e
                     elif onerror is False:
                         pass
                     else:
                         onerror(e)
-                    return
 
     unlink = remove
 
     def write_bytes(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        data: bytes | bytearray | memoryview | SupportsRead[bytes] = b"", 
+        data: Buffer | SupportsRead[Buffer] = b"", 
         pid: None | int = None, 
-    ) -> dict:
-        if isinstance(data, (bytes, bytearray, memoryview)):
-            data = BytesIO(data)
+    ) -> AttrDict:
+        "向文件写入二进制数据，如果文件已存在则替换"
         return self.upload(data, id_or_path, pid=pid, overwrite=True)
 
     def write_text(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         text: str = "", 
         pid: None | int = None, 
-        encoding: Optional[str] = None, 
-        errors: Optional[str] = None, 
-        newline: Optional[str] = None, 
-    ) -> dict:
+        encoding: None | str = None, 
+        errors: None | str = None, 
+        newline: None | str = None, 
+    ) -> AttrDict:
+        "向文件写入文本数据，如果文件已存在则替换"
         bio = BytesIO()
         if text:
             if encoding is None:
                 encoding = "utf-8"
             tio = TextIOWrapper(bio, encoding=encoding, errors=errors, newline=newline)
             tio.write(text)
             tio.flush()
             bio.seek(0)
-        return self.write_bytes(id_or_path, bio, pid=pid)
+        return self.write_bytes(id_or_path, data=bio, pid=pid)
 
     cp = copy
     mv = move
     rm = remove
```

### Comparing `python_115-0.0.8.3.7/p115/component/fs_base.py` & `python_115-0.0.8.4/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/component/fs_share.py` & `python_115-0.0.8.4/p115/component/fs_share.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from collections import deque
 from collections.abc import (
     Iterable, Iterator, Mapping, MutableMapping, Sequence
 )
 from datetime import datetime
 from functools import cached_property
+from itertools import islice
 from os import fspath, stat_result, PathLike
 from posixpath import join as joinpath
 from re import compile as re_compile
 from stat import S_IFDIR, S_IFREG
 from time import time
 from typing import cast, Never, Optional, Self
 
@@ -74,22 +75,26 @@
     fs: P115ShareFileSystem
 
 
 class P115ShareFileSystem(P115FileSystemBase[P115SharePath]):
     share_link: str
     share_code: str
     receive_code: str
-    user_id: int
     path_to_id: MutableMapping[str, int]
     id_to_attr: MutableMapping[int, AttrDict]
     attr_cache: MutableMapping[int, tuple[AttrDict]]
     full_loaded: bool
     path_class = P115SharePath
 
-    def __init__(self, /, client: str | P115Client, share_link: str):
+    def __init__(
+        self, 
+        /, 
+        client: str | P115Client, 
+        share_link: str, 
+    ):
         m = CRE_SHARE_LINK_search(share_link)
         if m is None:
             raise ValueError("not a valid 115 share link")
         if isinstance(client, str):
             client = P115Client(client)
         self.__dict__.update(
             client=client, 
@@ -99,83 +104,93 @@
             share_code=m["share_code"], 
             receive_code= m["receive_code"] or "", 
             path_to_id={"/": 0}, 
             id_to_attr={}, 
             attr_cache={}, 
             full_loaded=False, 
         )
-        self.__dict__["user_id"] = int(self.sharedata["userinfo"]["user_id"])
 
     def __repr__(self, /) -> str:
         cls = type(self)
         module = cls.__module__
         name = cls.__qualname__
         if module != "__main__":
             name = module + "." + name
         return f"<{name}(client={self.client!r}, share_link={self.share_link!r}, id={self.id!r}, path={self.path!r}) at {hex(id(self))}>"
 
+    def __setattr__(self, attr, val, /) -> Never:
+        raise TypeError("can't set attributes")
+
     @classmethod
     def login(
         cls, 
         /, 
         share_link: str, 
         cookie = None, 
         app: str = "web", 
+        **kwargs, 
     ) -> Self:
-        return cls(P115Client(cookie, app=app), share_link)
+        return cls(P115Client(cookie, app=app), share_link, **kwargs)
 
     @check_response
-    def fs_files(
-        self, 
-        /, 
-        id: int = 0, 
-        **kwargs, 
-    ) -> dict:
+    def fs_files(self, /, payload: dict) -> dict:
         """获取分享链接的某个文件夹中的文件和子文件夹的列表（包含详细信息）
-        params:
+        :param payload:
             - id: int | str = 0
             - limit: int = 32
             - offset: int = 0
             - asc: 0 | 1 = <default> # 是否升序排列
             - o: str = <default>
                 # 用某字段排序：
                 # - 文件名："file_name"
                 # - 文件大小："file_size"
                 # - 文件种类："file_type"
                 # - 修改时间："user_utime"
                 # - 创建时间："user_ptime"
                 # - 上次打开时间："user_otime"
         """
         return self.client.share_snap({
-            **kwargs, 
+            **payload, 
             "share_code": self.share_code, 
             "receive_code": self.receive_code, 
-            "cid": id, 
         })
 
     @check_response
     def downlist(self, /, id: int = 0) -> dict:
         """获取分享链接的某个文件夹中可下载的文件的列表（只含文件，不含文件夹，任意深度，简略信息）
         """
         return self.client.share_downlist({
             "share_code": self.share_code, 
             "receive_code": self.receive_code, 
             "cid": id, 
         })
 
     @cached_property
     def create_time(self, /) -> datetime:
+        "分享的创建时间"
         return datetime.fromtimestamp(int(self.shareinfo["create_time"]))
 
+    @cached_property
+    def snap_id(self, /) -> int:
+        "获取这个分享的 id"
+        return int(self.shareinfo["snap_id"])
+
+    @cached_property
+    def user_id(self, /) -> int:
+        "获取分享者的用户 id"
+        return int(self.sharedata["userinfo"]["user_id"])
+
     @property
     def sharedata(self, /) -> dict:
-        return self.fs_files(limit=1)["data"]
+        "获取分享的首页数据"
+        return self.fs_files({"limit": 1})["data"]
 
     @property
     def shareinfo(self, /) -> dict:
+        "获取分享信息"
         return self.sharedata["shareinfo"]
 
     def _attr(self, id: int = 0, /) -> AttrDict:
         try:
             return self.id_to_attr[id]
         except KeyError:
             pass
@@ -238,14 +253,15 @@
 
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> AttrDict:
+        "获取属性"
         path_class = type(self).path_class
         if isinstance(id_or_path, path_class):
             return self._attr(id_or_path["id"])
         elif isinstance(id_or_path, dict):
             attr = id_or_path
             if "id" in attr:
                 return self._attr(attr["id"])
@@ -258,14 +274,15 @@
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
         headers: Optional[Mapping] = None, 
     ) -> str:
+        "获取下载链接"
         path_class = type(self).path_class
         if isinstance(id_or_path, (int, path_class)):
             id = id_or_path if isinstance(id_or_path, int) else id_or_path.id
             if id in self.id_to_attr:
                 attr = self.id_to_attr[id]
                 if attr["is_directory"]:
                     raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
@@ -281,16 +298,33 @@
         }, headers=headers)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
-        **kwargs, 
+        page_size: int = 1_000, 
+        **payload, 
     ) -> Iterator[AttrDict]:
+        """迭代获取目录内直属的文件或目录的信息
+        :param payload:
+            - limit: int = 32
+            - offset: int = 0
+            - asc: 0 | 1 = <default> # 是否升序排列
+            - o: str = <default>
+                # 用某字段排序：
+                # - 文件名："file_name"
+                # - 文件大小："file_size"
+                # - 文件种类："file_type"
+                # - 修改时间："user_utime"
+                # - 创建时间："user_ptime"
+                # - 上次打开时间："user_otime"
+        """
+        if page_size <= 0:
+            page_size = 1_000
         path_class = type(self).path_class
         if isinstance(id_or_path, int):
             attr = self.attr(id_or_path)
         elif isinstance(id_or_path, dict):
             attr = id_or_path
         elif isinstance(id_or_path, path_class):
             attr = id_or_path.__dict__
@@ -298,61 +332,77 @@
             attr = self.attr(id_or_path, pid)
         if not attr["is_directory"]:
             raise NotADirectoryError(
                 errno.ENOTDIR, 
                 f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
             )
         id = attr["id"]
+        payload["cid"] = id
+        payload["limit"] = page_size
+        offset = int(payload.setdefault("offset", 0))
+        if offset < 0:
+            offset = payload["offset"] = 0
+        else:
+            payload["offset"] = 0
         try:
-            return iter(self.attr_cache[id])
+            return islice(self.attr_cache[id], offset, None)
         except KeyError:
             dirname = attr["path"]
             def iterdir():
-                page_size = kwargs.setdefault("limit", 1 << 10)
                 get_files = self.fs_files
                 path_to_id = self.path_to_id
-                data = get_files(id, **kwargs)["data"]
+                data = get_files(payload)["data"]
                 for attr in map(normalize_info, data["list"]):
                     attr["fs"] = self
                     path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                     path_to_id[path] = attr["id"]
                     yield attr
                 for offset in range(page_size, data["count"], page_size):
-                    kwargs["offset"] = offset
-                    data = get_files(id, **kwargs)["data"]
+                    payload["offset"] = offset
+                    data = get_files(payload)["data"]
                     for attr in map(normalize_info, data["list"]):
                         attr["fs"] = self
                         path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                         path_to_id[path] = attr["id"]
                         yield attr
             t = self.attr_cache[id] = tuple(iterdir())
             self.id_to_attr.update((attr["id"], attr) for attr in t)
             return iter(t)
 
-    def receive(self, ids: int | str | Iterable[int | str], /, cid: int = 0):
+    def receive(
+        self, 
+        ids: int | str | Iterable[int | str], 
+        /, 
+        to_pid: int = 0, 
+    ) -> dict:
+        """接收分享文件到网盘
+        :param ids: 要转存到文件 id（这些 id 归属分享链接）
+        :param to_pid: 你的网盘的一个目录 id（这个 id 归属你的网盘）
+        """
         if isinstance(ids, int):
             ids = str(ids)
         elif isinstance(ids, Iterable):
             ids = ",".join(map(str, ids))
         if not ids:
             raise ValueError("no id (to file) to receive")
         payload = {
             "share_code": self.share_code, 
             "receive_code": self.receive_code, 
             "file_id": ids, 
-            "cid": cid, 
+            "cid": to_pid, 
         }
         return check_response(self.client.share_receive)(payload)
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> stat_result:
+        "检查路径的属性，就像 `os.stat`"
         attr = self.attr(id_or_path, pid)
         is_dir = attr["is_directory"]
         timestamp: float = attr["timestamp"]
         return stat_result((
             (S_IFDIR if is_dir else S_IFREG) | 0o444, 
             cast(int, attr["id"]), 
             cast(int, attr["parent_id"]),
```

### Comparing `python_115-0.0.8.3.7/p115/component/fs_zip.py` & `python_115-0.0.8.4/p115/component/fs_zip.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import errno
 
 from collections import deque
 from collections.abc import Iterator, Mapping, MutableMapping, Sequence
 from datetime import datetime
 from functools import cached_property
-from itertools import count
+from itertools import count, islice
 from os import fspath, stat_result, PathLike
 from posixpath import join as joinpath
 from stat import S_IFDIR, S_IFREG
 from typing import cast, Never, Self
 
 from posixpatht import escape, joins
 
@@ -44,54 +44,53 @@
 class P115ZipPath(P115PathBase):
     fs: P115ZipFileSystem
 
 
 # TODO: 参考 zipfile 模块的接口设计 namelist、filelist 等属性，以及其它的和 zipfile 兼容的接口
 # TODO: 当文件特别多时，可以用 zipfile 等模块来读取文件列表
 class P115ZipFileSystem(P115FileSystemBase[P115ZipPath]):
-    file_id: None | int
+    file_id: int
     pickcode: str
     path_to_id: MutableMapping[str, int]
     id_to_attr: MutableMapping[int, AttrDict]
     attr_cache: MutableMapping[int, tuple[AttrDict]]
     full_loaded: bool
     path_class = P115ZipPath
 
     def __init__(
         self, 
         /, 
         client: str | P115Client, 
         id_or_pickcode: int | str, 
     ):
-        file_id: None | int
         if isinstance(client, str):
             client = P115Client(client)
         if isinstance(id_or_pickcode, int):
             file_id = id_or_pickcode
-            pickcode = client.fs.attr(file_id)["pickcode"]
+            attr = client.fs.attr(file_id)
+            pickcode = attr["pickcode"]
+            self.__dict__["create_time"] = attr["ptime"]
         else:
-            file_id = None
             pickcode = id_or_pickcode
+            file_id = client.fs.get_id_from_pickcode(pickcode)
         resp = check_response(client.extract_push_progress(pickcode))
         if resp["data"]["extract_status"]["unzip_status"] != 4:
             raise OSError(errno.EIO, "file was not decompressed")
         self.__dict__.update(
             client=client, 
             id=0, 
             path="/", 
-            pickcode=pickcode, 
             file_id=file_id, 
+            pickcode=pickcode, 
             path_to_id={"/": 0}, 
             id_to_attr={}, 
             attr_cache={}, 
             full_loaded=False, 
             _nextid=count(1).__next__, 
         )
-        if file_id is None:
-            self.__dict__["create_time"] = datetime.fromtimestamp(0)
 
     def __setattr__(self, attr, val, /) -> Never:
         raise TypeError("can't set attributes")
 
     @classmethod
     def login(
         cls, 
@@ -115,16 +114,15 @@
             path=path, 
             next_marker=next_marker, 
             page_count=page_count, 
         )
 
     @cached_property
     def create_time(self, /) -> datetime:
-        if self.file_id is None:
-            return datetime.fromtimestamp(0)
+        "创建时间"
         return self.client.fs.attr(self.file_id)["ptime"]
 
     def _attr(self, id: int = 0, /) -> AttrDict:
         try:
             return self.id_to_attr[id]
         except KeyError:
             pass
@@ -190,14 +188,15 @@
 
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> AttrDict:
+        "获取属性"
         path_class = type(self).path_class
         if isinstance(id_or_path, path_class):
             return self._attr(id_or_path["id"])
         elif isinstance(id_or_path, dict):
             attr = id_or_path
             if "id" in attr:
                 return self._attr(attr["id"])
@@ -210,35 +209,42 @@
     def extract(
         self, 
         /, 
         paths: str | Sequence[str] = "", 
         dirname: str = "", 
         to_pid: int | str = 0, 
     ) -> ExtractProgress:
+        "解压缩到网盘"
         return self.client.extract_file_future(self.pickcode, paths, dirname, to_pid)
 
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: None | int = None, 
         headers: None | Mapping = None, 
     ) -> str:
+        "获取下载链接"
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
         return self.client.extract_download_url(self.pickcode, attr["path"], headers=headers)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
+        page_size: int = 999, 
         **kwargs, 
     ) -> Iterator[AttrDict]:
+        """迭代获取目录内直属的文件或目录的信息
+        """
+        if page_size <= 0 or page_size > 999:
+            page_size = 999
         attr = self.attr(id_or_path, pid)
         if not attr["is_directory"]:
             raise NotADirectoryError(
                 errno.ENOTDIR, 
                 f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
             )
         id = attr["id"]
@@ -246,24 +252,24 @@
             return iter(self.attr_cache[id])
         except KeyError:
             nextid = self.__dict__["_nextid"]
             dirname = attr["path"]
             def iterdir():
                 get_files = self.fs_files
                 path_to_id = self.path_to_id
-                data = get_files(dirname, **kwargs)["data"]
+                data = get_files(path=dirname, page_count=page_size)["data"]
                 for info in data["list"]:
                     attr = normalize_info(info, fs=self)
                     path = joinpath(dirname, escape(attr["name"]))
                     attr.update(id=nextid(), parent_id=id, path=path)
                     path_to_id[path] = attr["id"]
                     yield attr
                 next_marker = data["next_marker"]
                 while next_marker:
-                    data = get_files(dirname, next_marker, **kwargs)["data"]
+                    data = get_files(path=dirname, next_marker=next_marker, page_count=page_size)["data"]
                     for info in data["list"]:
                         attr = normalize_info(info, fs=self)
                         path = joinpath(dirname, escape(attr["name"]))
                         attr.update(id=nextid(), parent_id=id, path=path)
                         path_to_id[path] = attr["id"]
                         yield attr
                     next_marker = data["next_marker"]
@@ -273,14 +279,15 @@
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: None | int = None, 
     ) -> stat_result:
+        "检查路径的属性，就像 `os.stat`"
         attr = self.attr(id_or_path, pid)
         is_dir = attr["is_directory"]
         timestamp: float = attr["timestamp"]
         return stat_result((
             (S_IFDIR if is_dir else S_IFREG) | 0o444, 
             cast(int, attr["id"]), 
             cast(int, attr["parent_id"]),
```

### Comparing `python_115-0.0.8.3.7/p115/component/labellist.py` & `python_115-0.0.8.4/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/component/offline.py` & `python_115-0.0.8.4/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/component/recyclebin.py` & `python_115-0.0.8.4/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/component/sharing.py` & `python_115-0.0.8.4/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/p115/tool/__init__.py` & `python_115-0.0.8.4/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/pyproject.toml` & `python_115-0.0.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.3.7"
+version = "0.0.8.4"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
@@ -38,20 +38,20 @@
 multidict = "*"
 posixpatht = "*"
 pycryptodome = "*"
 python-asynctools = "*"
 python-concurrenttools = "*"
 python-cookietools = "*"
 python-download = "*"
-python-filewrap = "*"
+python-filewrap = ">=0.1"
 python-hashtools = "*"
 python-httpfile = "*"
-python-http_request = "*"
+python-http_request = ">=0.0.5"
 python-iterutils = "*"
-python-startfile = "*"
+python-startfile = ">=0.0.2"
 python-urlopen = "*"
 qrcode = "*"
 yarl = "*"
 
 [tool.poetry.scripts]
 python-115 = "p115.__main__:main"
 p115 = "p115.__main__:main"
```

### Comparing `python_115-0.0.8.3.7/readme.md` & `python_115-0.0.8.4/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.7/PKG-INFO` & `python_115-0.0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.3.7
+Version: 0.0.8.4
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -31,20 +31,20 @@
 Requires-Dist: multidict
 Requires-Dist: posixpatht
 Requires-Dist: pycryptodome
 Requires-Dist: python-asynctools
 Requires-Dist: python-concurrenttools
 Requires-Dist: python-cookietools
 Requires-Dist: python-download
-Requires-Dist: python-filewrap
+Requires-Dist: python-filewrap (>=0.1)
 Requires-Dist: python-hashtools
-Requires-Dist: python-http_request
+Requires-Dist: python-http_request (>=0.0.5)
 Requires-Dist: python-httpfile
 Requires-Dist: python-iterutils
-Requires-Dist: python-startfile
+Requires-Dist: python-startfile (>=0.0.2)
 Requires-Dist: python-urlopen
 Requires-Dist: qrcode
 Requires-Dist: yarl
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 Description-Content-Type: text/markdown
 
 # 115 网盘 Web API 的 Python 封装
```

