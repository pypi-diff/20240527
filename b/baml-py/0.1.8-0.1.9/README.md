# Comparing `tmp/baml_py-0.1.8-cp38-abi3-win_amd64.whl.zip` & `tmp/baml_py-0.1.9-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 3314034 bytes, number of entries: 9
--rw-r--r--  4.6 unx      336 b- defN 24-May-03 22:07 baml_py-0.1.8.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-03 22:07 baml_py-0.1.8.dist-info/WHEEL
--rw-r--r--  4.6 unx    11556 b- defN 24-May-03 22:07 baml_py-0.1.8.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11556 b- defN 24-May-03 22:07 baml_py-0.1.8.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      111 b- defN 24-May-03 22:07 baml_py/__init__.py
--rw-r--r--  4.6 unx     1342 b- defN 24-May-03 22:07 baml_py/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-May-03 22:07 baml_py/py.typed
--rwxr-xr-x  4.6 unx  8790016 b- defN 24-May-03 22:07 baml_py/baml_py.pyd
--rw-r--r--  4.6 unx      712 b- defN 24-May-03 22:07 baml_py-0.1.8.dist-info/RECORD
-9 files, 8815723 bytes uncompressed, 3312818 bytes compressed:  62.4%
+Zip file size: 4286269 bytes, number of entries: 12
+-rw-r--r--  4.6 unx      336 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/WHEEL
+-rw-r--r--  4.6 unx       54 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     3272 b- defN 24-May-26 23:13 baml_py/async_context_vars.py
+-rw-r--r--  4.6 unx     2641 b- defN 24-May-26 23:13 baml_py/baml_py.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-26 23:13 baml_py/py.typed
+-rw-r--r--  4.6 unx     2275 b- defN 24-May-26 23:13 baml_py/stream.py
+-rw-r--r--  4.6 unx      518 b- defN 24-May-26 23:13 baml_py/__init__.py
+-rwxr-xr-x  4.6 unx 11260928 b- defN 24-May-26 23:13 baml_py/baml_py.pyd
+-rw-r--r--  4.6 unx      967 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/RECORD
+12 files, 11294197 bytes uncompressed, 4284655 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -1,28 +1,37 @@
-Filename: baml_py-0.1.8.dist-info/METADATA
+Filename: baml_py-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: baml_py-0.1.8.dist-info/WHEEL
+Filename: baml_py-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: baml_py-0.1.8.dist-info/license_files/LICENSE
+Filename: baml_py-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: baml_py-0.1.8.dist-info/license_files/LICENSE
+Filename: baml_py-0.1.9.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: baml_py/__init__.py
+Filename: baml_py-0.1.9.dist-info/license_files/LICENSE
+Comment: 
+
+Filename: baml_py/async_context_vars.py
 Comment: 
 
-Filename: baml_py/__init__.pyi
+Filename: baml_py/baml_py.pyi
 Comment: 
 
 Filename: baml_py/py.typed
 Comment: 
 
+Filename: baml_py/stream.py
+Comment: 
+
+Filename: baml_py/__init__.py
+Comment: 
+
 Filename: baml_py/baml_py.pyd
 Comment: 
 
-Filename: baml_py-0.1.8.dist-info/RECORD
+Filename: baml_py-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## baml_py/__init__.py

```diff
@@ -1,5 +1,22 @@
-from .baml_py import *
-
-__doc__ = baml_py.__doc__
-if hasattr(baml_py, "__all__"):
-    __all__ = baml_py.__all__
+# BAML Python API: provides the Python API for the BAML runtime.
+
+# Re-export the pyo3 API
+from .baml_py import (
+    BamlRuntimePy,
+    FunctionResultPy,
+    FunctionResultStreamPy,
+    BamlImagePy as Image,
+    invoke_runtime_cli,
+)
+from .stream import BamlStream
+from .async_context_vars import CtxManager as BamlCtxManager
+
+__all__ = [
+    "BamlRuntimePy",
+    "BamlStream",
+    "BamlCtxManager",
+    "FunctionResultPy",
+    "FunctionResultStreamPy",
+    "Image",
+    "invoke_runtime_cli",
+]
```

## Comparing `baml_py-0.1.8.dist-info/license_files/LICENSE` & `baml_py-0.1.9.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `baml_py/__init__.pyi` & `baml_py/baml_py.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Any, Dict, Optional
+from typing import Any, Callable, Dict, Optional
 
-class FunctionResult:
+class FunctionResultPy:
     """The result of a BAML function call.
 
     Represents any of:
 
         - a successful LLM call, with a successful type parse
         - a successful LLM call, with a failed type parse
         - a failed LLM call, due to a provider outage or other network error
@@ -13,38 +13,68 @@
 
     We only expose the parsed result to Python right now.
     """
 
     def __str__(self) -> str: ...
     def parsed(self) -> Any: ...
 
-class Image:
+class FunctionResultStreamPy:
+    """The result of a BAML function stream.
+
+    Provides a callback interface to receive events from a BAML result stream.
+
+    Use `on_event` to set the callback, and `done` to drive the stream to completion.
+    """
+
+    def __str__(self) -> str: ...
+    def on_event(
+        self, on_event: Callable[[FunctionResultPy], None]
+    ) -> FunctionResultStreamPy: ...
+    async def done(self, ctx: RuntimeContextManagerPy) -> FunctionResultPy: ...
+
+class BamlImagePy:
     def __init__(
         self, url: Optional[str] = None, base64: Optional[str] = None
     ) -> None: ...
-
     @property
     def url(self) -> Optional[str]: ...
-
     @url.setter
     def url(self, value: Optional[str]) -> None: ...
-
     @property
     def base64(self) -> Optional[str]: ...
-
     @base64.setter
     def base64(self, value: Optional[str]) -> None: ...
 
+class RuntimeContextManagerPy:
+    def upsert_tags(self, tags: Dict[str, Any]) -> None: ...
+    def deep_clone(self) -> RuntimeContextManagerPy: ...
 
-class BamlRuntimeFfi:
+class BamlRuntimePy:
     @staticmethod
-    def from_directory(directory: str) -> BamlRuntimeFfi: ...
-
-    @staticmethod
-    def from_encoded(encoded: str) -> BamlRuntimeFfi: ...
-
+    def from_directory(directory: str, env_vars: Dict[str, str]) -> BamlRuntimePy: ...
     async def call_function(
         self,
         function_name: str,
         args: Dict[str, Any],
-        ctx: Dict[str, Any],
-    ) -> FunctionResult: ...
+        ctx: RuntimeContextManagerPy,
+    ) -> FunctionResultPy: ...
+    def stream_function(
+        self,
+        function_name: str,
+        args: Dict[str, Any],
+        on_event: Optional[Callable[[FunctionResultPy], None]],
+        ctx: RuntimeContextManagerPy,
+    ) -> FunctionResultStreamPy: ...
+    def create_context_manager(self) -> RuntimeContextManagerPy: ...
+    def flush(self) -> None: ...
+
+class BamlSpanPy:
+    @staticmethod
+    def new(
+        runtime: BamlRuntimePy,
+        function_name: str,
+        args: Dict[str, Any],
+        ctx: RuntimeContextManagerPy,
+    ) -> BamlSpanPy: ...
+    async def finish(self, result: Any, ctx: RuntimeContextManagerPy) -> str | None: ...
+
+def invoke_runtime_cli() -> None: ...
```

