# Comparing `tmp/python_filewrap-0.0.8.tar.gz` & `tmp/python_filewrap-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.8.tar", max compression
+gzip compressed data, was "python_filewrap-0.1.tar", max compression
```

## Comparing `python_filewrap-0.0.8.tar` & `python_filewrap-0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.8/LICENSE
--rwxr-xr-x   0        0        0    18778 2024-05-23 09:38:37.272775 python_filewrap-0.0.8/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.8/filewrap/py.typed
--rw-r--r--   0        0        0     1171 2024-05-23 09:38:46.018483 python_filewrap-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.8/readme.md
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.1/LICENSE
+-rwxr-xr-x   0        0        0    19814 2024-05-27 13:32:43.338203 python_filewrap-0.1/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.1/filewrap/py.typed
+-rw-r--r--   0        0        0     1169 2024-05-27 13:33:43.361286 python_filewrap-0.1/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.1/readme.md
+-rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 python_filewrap-0.1/PKG-INFO
```

### Comparing `python_filewrap-0.0.8/LICENSE` & `python_filewrap-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.8/filewrap/__init__.py` & `python_filewrap-0.1/filewrap/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 8)
+__version__ = (0, 1)
 __all__ = [
-    "SupportsRead", "SupportsWrite", "SupportsSeek", 
+    "Buffer", "SupportsRead", "SupportsReadinto", 
+    "SupportsWrite", "SupportsSeek", 
     "bio_chunk_iter", "bio_chunk_async_iter", 
     "bio_skip_iter", "bio_skip_async_iter", 
     "bytes_iter_skip", "bytes_async_iter_skip", 
     "bytes_iter_to_reader", "bytes_iter_to_async_reader", 
     "bytes_to_chunk_iter", "bytes_to_chunk_async_iter", 
     "bytes_ensure_part_iter", "bytes_ensure_part_async_iter", 
 ]
@@ -21,29 +22,66 @@
 from shutil import COPY_BUFSIZE # type: ignore
 from threading import Lock
 from typing import runtime_checkable, Any, Protocol, TypeVar
 
 try:
     from collections.abc import Buffer # type: ignore
 except ImportError:
-    Buffer = Any
+    from abc import ABC, abstractmethod
+    from array import array
+
+    def _check_methods(C, *methods):
+        mro = C.__mro__
+        for method in methods:
+            for B in mro:
+                if method in B.__dict__:
+                    if B.__dict__[method] is None:
+                        return NotImplemented
+                    break
+            else:
+                return NotImplemented
+        return True
+
+    class Buffer(ABC): # type: ignore
+        __slots__ = ()
+
+        @abstractmethod
+        def __buffer__(self, flags: int, /) -> memoryview:
+            raise NotImplementedError
+
+        @classmethod
+        def __subclasshook__(cls, C):
+            if cls is Buffer:
+                return _check_methods(C, "__buffer__")
+            return NotImplemented
+
+    Buffer.register(bytes)
+    Buffer.register(bytearray)
+    Buffer.register(memoryview)
+    Buffer.register(array)
+
 
 from asynctools import async_chain, ensure_async, ensure_aiter
 
 
 _T_co = TypeVar("_T_co", covariant=True)
 _T_contra = TypeVar("_T_contra", contravariant=True)
 
 
 @runtime_checkable
 class SupportsRead(Protocol[_T_co]):
     def read(self, /, __length: int = ...) -> _T_co: ...
 
 
 @runtime_checkable
+class SupportsReadinto(Protocol):
+    def readinto(self, /, buf: Buffer = ...) -> int: ...
+
+
+@runtime_checkable
 class SupportsWrite(Protocol[_T_contra]):
     def write(self, /, __s: _T_contra) -> object: ...
 
 
 @runtime_checkable
 class SupportsSeek(Protocol):
     def seek(self, /, __offset: int, __whence: int = 0) -> int: ...
```

### Comparing `python_filewrap-0.0.8/pyproject.toml` & `python_filewrap-0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.8"
+version = "0.1"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.8/PKG-INFO` & `python_filewrap-0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.8
+Version: 0.1
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

