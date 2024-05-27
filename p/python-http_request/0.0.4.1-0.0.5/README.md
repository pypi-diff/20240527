# Comparing `tmp/python_http_request-0.0.4.1.tar.gz` & `tmp/python_http_request-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_http_request-0.0.4.1.tar", max compression
+gzip compressed data, was "python_http_request-0.0.5.tar", max compression
```

## Comparing `python_http_request-0.0.4.1.tar` & `python_http_request-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.4.1/LICENSE
--rwxr-xr-x   0        0        0     6169 2024-05-23 06:21:05.290392 python_http_request-0.0.4.1/http_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.4.1/http_request/py.typed
--rw-r--r--   0        0        0     1259 2024-05-24 17:03:37.634863 python_http_request-0.0.4.1/pyproject.toml
--rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.4.1/readme.md
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 python_http_request-0.0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     5566 2024-05-27 13:36:55.658258 python_http_request-0.0.5/http_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.5/http_request/py.typed
+-rw-r--r--   0        0        0     1261 2024-05-27 13:38:22.109733 python_http_request-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.5/readme.md
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 python_http_request-0.0.5/PKG-INFO
```

### Comparing `python_http_request-0.0.4.1/LICENSE` & `python_http_request-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_http_request-0.0.4.1/http_request/__init__.py` & `python_http_request-0.0.5/http_request/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 4)
+__version__ = (0, 0, 5)
 __all__ = [
     "SupportsGeturl", "url_origin", "complete_url", "cookies_str_to_dict", "headers_str_to_dict", 
     "encode_multipart_data", "encode_multipart_data_async", 
 ]
 
 from itertools import chain
 from collections.abc import AsyncIterable, AsyncIterator, ItemsView, Iterable, Iterator, Mapping
 from re import compile as re_compile, Pattern
 from typing import runtime_checkable, Any, Final, Protocol, TypeVar
 from urllib.parse import quote, urlsplit, urlunsplit
 from uuid import uuid4
 
 from asynctools import ensure_aiter, async_chain
-from filewrap import bio_chunk_iter, bio_chunk_async_iter, SupportsRead
+from filewrap import bio_chunk_iter, bio_chunk_async_iter, Buffer, SupportsRead
 from integer_tool import int_to_bytes
 from texttools import text_to_dict
 
 
 AnyStr = TypeVar("AnyStr", bytes, str, covariant=True)
 
 CRE_URL_SCHEME: Final = re_compile(r"^(?i:[a-z][a-z0-9.+-]*)://")
@@ -69,48 +69,46 @@
     /, 
     kv_sep: str | Pattern[str] = re_compile(r":\s+"), 
     entry_sep: str | Pattern[str] = re_compile("\n+"), 
 ) -> dict[str, str]:
     return text_to_dict(headers.strip(), kv_sep, entry_sep)
 
 
-def ensure_bytes(s, /) -> bytes | bytearray | memoryview:
-    if isinstance(s, (bytes, bytearray, memoryview)):
+def ensure_bytes(s, /) -> Buffer:
+    if isinstance(s, Buffer):
         return s
     if isinstance(s, int):
         return int_to_bytes(s)
     elif isinstance(s, str):
         return bytes(s, "utf-8")
     try:
         return bytes(s)
     except TypeError:
         return bytes(str(s), "utf-8")
 
 
 def encode_multipart_data(
     data: Mapping[str, Any], 
-    files: Mapping[str, bytes | bytearray | memoryview | 
-                        SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                        Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview]], 
+    files: Mapping[str, Buffer | SupportsRead[Buffer] | Iterable[Buffer]], 
     boundary: None | str = None, 
-) -> tuple[dict, Iterator[bytes | bytearray | memoryview]]:
+) -> tuple[dict, Iterator[Buffer]]:
     if not boundary:
         boundary = uuid4().bytes.hex()
     headers = {"Content-Type": f"multipart/form-data; boundary={boundary}"}
 
-    def encode_data(data) -> Iterator[bytes | bytearray | memoryview]:
+    def encode_data(data) -> Iterator[Buffer]:
         if isinstance(data, Mapping):
             data = ItemsView(data)
         for name, value in data:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\n\r\n' % bytes(quote(name), "ascii")
             yield ensure_bytes(value)
             yield b"\r\n"
 
-    def encode_files(files) -> Iterator[bytes | bytearray | memoryview]:
+    def encode_files(files) -> Iterator[Buffer]:
         if isinstance(files, Mapping):
             files = ItemsView(files)
         for name, file in files:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\nContent-Type: application/octet-stream\r\n\r\n' % bytes(quote(name), "ascii")
             if isinstance(file, (bytes, bytearray, memoryview)):
                 yield file
@@ -122,34 +120,31 @@
 
     boundary_line = b"--%s\r\n" % boundary.encode("utf-8")
     return headers, chain(encode_data(data), encode_files(files), (b'--%s--\r\n' % boundary.encode("ascii"),))
 
 
 def encode_multipart_data_async(
     data: Mapping[str, Any], 
-    files: Mapping[str, bytes | bytearray | memoryview | 
-                        SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
-                        Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
-                        AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview]], 
+    files: Mapping[str, Buffer | SupportsRead[Buffer] | Iterable[Buffer] | AsyncIterable[Buffer]], 
     boundary: None | str = None, 
-) -> tuple[dict, AsyncIterator[bytes | bytearray | memoryview]]:
+) -> tuple[dict, AsyncIterator[Buffer]]:
     if not boundary:
         boundary = uuid4().bytes.hex()
     headers = {"Content-Type": f"multipart/form-data; boundary={boundary}"}
 
-    async def encode_data(data) -> AsyncIterator[bytes | bytearray | memoryview]:
+    async def encode_data(data) -> AsyncIterator[Buffer]:
         if isinstance(data, Mapping):
             data = ItemsView(data)
         for name, value in data:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\n\r\n' % bytes(quote(name), "ascii")
             yield ensure_bytes(value)
             yield b"\r\n"
 
-    async def encode_files(files) -> AsyncIterator[bytes | bytearray | memoryview]:
+    async def encode_files(files) -> AsyncIterator[Buffer]:
         if isinstance(files, Mapping):
             files = ItemsView(files)
         for name, file in files:
             yield boundary_line
             yield b'Content-Disposition: form-data; name="%s"\r\nContent-Type: application/octet-stream\r\n\r\n' % bytes(quote(name), "ascii")
             if isinstance(file, (bytes, bytearray, memoryview)):
                 yield file
```

### Comparing `python_http_request-0.0.4.1/pyproject.toml` & `python_http_request-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-http_request"
-version = "0.0.4.1"
+version = "0.0.5"
 description = "Python http response utils."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 keywords = ["http", "request"]
@@ -24,15 +24,15 @@
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-asynctools = "*"
-python-filewrap = "*"
+python-filewrap = ">=0.1"
 python-texttools = "*"
 integer_tool = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_http_request-0.0.4.1/PKG-INFO` & `python_http_request-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-http_request
-Version: 0.0.4.1
+Version: 0.0.5
 Summary: Python http response utils.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request
 License: MIT
 Keywords: http,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: integer_tool
 Requires-Dist: python-asynctools
-Requires-Dist: python-filewrap
+Requires-Dist: python-filewrap (>=0.1)
 Requires-Dist: python-texttools
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request
 Description-Content-Type: text/markdown
 
 # Python http response utils.
 
 ## Installation
```

