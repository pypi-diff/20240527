# Comparing `tmp/gongsf-0.1.0.tar.gz` & `tmp/gongsf-0.1.1.tar.gz`

## Comparing `gongsf-0.1.0.tar` & `gongsf-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 gongsf-0.1.0/gongsf/__init__.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 gongsf-0.1.0/gongsf/codec.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 gongsf-0.1.0/gongsf/context.py
--rw-r--r--   0        0        0    21347 2020-02-02 00:00:00.000000 gongsf-0.1.0/gongsf/data.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 gongsf-0.1.0/gongsf/lib.py
--rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 gongsf-0.1.0/gongsf/types.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gongsf-0.1.0/.gitignore
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 gongsf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gongsf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 gongsf-0.1.1/gongsf/__init__.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 gongsf-0.1.1/gongsf/codec.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 gongsf-0.1.1/gongsf/context.py
+-rw-r--r--   0        0        0    21326 2020-02-02 00:00:00.000000 gongsf-0.1.1/gongsf/data.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 gongsf-0.1.1/gongsf/lib.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 gongsf-0.1.1/gongsf/types.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gongsf-0.1.1/.gitignore
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 gongsf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 gongsf-0.1.1/PKG-INFO
```

### Comparing `gongsf-0.1.0/gongsf/codec.py` & `gongsf-0.1.1/gongsf/codec.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ]
 
 def read_schema_txt(
         string: str, *,
         save_comments=False, no_comments=False,
 ) -> tuple[Descriptor, Schema]:
     descriptor = Descriptor(gsf.create_descriptor(), own=True)
-    schema = Schema(gsf.create_schema(), own=True)
+    schema = Schema(gsf.create_schema(), own=True, descriptor=descriptor)
     reader = GsfCodecStruct()
     reader.format = 0
     reader.flags = _parse_flags('TXT_READ', {
         'SAVE_COMMENTS': save_comments,
         'NO_COMMENTS': no_comments,
     })
     cstr = c_str(string)
@@ -45,15 +45,15 @@
     reader = GsfCodecStruct()
     reader.format = 0
     reader.flags = _parse_flags('TXT_READ', {
         'SAVE_COMMENTS': save_comments,
         'NO_COMMENTS': no_comments,
     })
     cstr = c_str(string)
-    gsf.reader_create_buf(ct.pointer(reader), cstr, ct.c_size_t(len(string) + 1))
+    gsf.reader_create_buf(ct.pointer(reader), cstr, ct.c_size_t(len(cstr) + 1))
     gsf.read_article(ct.pointer(reader), article.handle, schema.handle)
     gsf.reader_delete_buf(ct.pointer(reader))
     return article
 
 
 def write_schema_txt(
         schema: Schema, max_size: int = 2048, *,
@@ -72,27 +72,29 @@
     gsf.writer_create_buf(ct.pointer(writer), string, ct.c_size_t(max_size))
     gsf.write_article(ct.pointer(writer), schema.handle)
     gsf.writer_delete_buf(ct.pointer(writer))
     return py_str(string.value)
 
 
 def write_article_txt(
-        article: Article, max_size: int = 2048, *,
+        article: Article, max_size_deprecated: int = 0, *,
         signature=False, comments=False, no_header_newline=False,
         no_descriptor=False, strong_all=False, strong_root=False, strong_types=False,
 ) -> str:
     writer = GsfCodecStruct()
     writer.format = 0
     writer.flags = _parse_flags('TXT_WRITE', {
         'SIGNATURE': signature,
         'COMMENTS': comments,
         'NO_HEADER_NEWLINE': no_header_newline,
         'ARTICLE_NO_DESCRIPTOR': no_descriptor,
         'ARTICLE_STRONG_TYPES_ALL': strong_all,
         'ARTICLE_STRING_ROOT': strong_root,
         'ARTICLE_STRING_TYPES': strong_types,
+        'LEADING_ZERO': True,
     })
-    string = ct.create_string_buffer(max_size)
-    gsf.writer_create_buf(ct.pointer(writer), string, ct.c_size_t(max_size))
+    buf = ct.c_char_p()
+    gsf.writer_create_growing_buf(ct.pointer(writer), ct.pointer(buf), ct.c_size_t(0))
     gsf.write_article(ct.pointer(writer), article.handle)
-    gsf.writer_delete_buf(ct.pointer(writer))
-    return py_str(string.value)
+    result = py_str(buf.value)
+    gsf.writer_delete_growing_buf(ct.pointer(writer))
+    return result
```

### Comparing `gongsf-0.1.0/gongsf/context.py` & `gongsf-0.1.1/gongsf/context.py`

 * *Files identical despite different names*

### Comparing `gongsf-0.1.0/gongsf/data.py` & `gongsf-0.1.1/gongsf/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,24 +50,25 @@
 
     @version.setter
     def version(self, value: str) -> None:
         self.edit(None, None, value)
 
 
 class Schema:
-    def __init__(self, handle, const: bool = True, own: bool = False) -> None:
+    def __init__(self, handle, const: bool = True, own: bool = False, descriptor: Descriptor | None = None) -> None:
         self.handle = ct.c_void_p(handle)
         self._const = const and not own
         self._own = own
+        self._descriptor = descriptor
 
     @classmethod
     def new(cls, descriptor: Descriptor, root: Typing | str, class_count: int) -> Schema:
         return Schema(
             gsf.schema_new(descriptor.handle, c_str_or(root, lambda t: t.handle), ct.c_size_t(class_count)),
-            own=True
+            False, True, descriptor
         )
 
     def __del__(self) -> None:
         if self._own:
             gsf.delete_schema[None](self.handle)
 
     @property
@@ -87,18 +88,15 @@
 
     @property
     def context(self) -> Context:
         return Context(gsf.schema_get_context(self.handle))
 
     @property
     def root(self) -> Typing:
-        if not self._const:
-            return Typing(gsf.schema_get_root(self.handle))
-        else:
-            return Typing(gsf.schema_get_root_const(self.handle))
+        return Typing(gsf.schema_get_root(self.handle))
 
     @root.setter
     def root(self, value: Typing) -> None:
         gsf.schema_set_root(self.handle, value.handle)
 
     @property
     def class_count(self) -> int:
```

### Comparing `gongsf-0.1.0/gongsf/lib.py` & `gongsf-0.1.1/gongsf/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 
 # TODO const check before mutable methods
 
 
 class GsfException(Exception):
     pass
 
+def gsf_raise() -> None:
+    error = ct.create_string_buffer(2048)
+    gsf.errno_string(error, no_except=True)
+    err = py_str(error.value)
+    if err == 'no error':
+        return
+    raise GsfException(err)
+
 
 class GsfSymbol:
     def __init__(self, symbol, name: str):
         symbol.restype = ct.c_void_p
         self._symbol = symbol
         self._bool = False
         self._name = name
@@ -23,20 +31,16 @@
     def __call__(self, *args, **kwargs) -> Any:
         error_val = kwargs.get('error', None)
         no_except = kwargs.get('no_except', False) or self._symbol.restype is None
         ret = self._symbol(*args, **kwargs)
         if self._bool:
             return ret is not None
         if not no_except and ret == error_val:
-            error = ct.create_string_buffer(2048)
-            gsf.errno_string(error, no_except=True)
-            err = py_str(error.value)
-            if err == 'no error':
-                return ret
-            raise GsfException(err)
+            gsf_raise()
+            return ret
         return ret
 
     def __getitem__(self, item: type | None) -> GsfSymbol:
         if item != ct.c_bool:
             self._symbol.restype = item
         else:
             self._bool = True
```

### Comparing `gongsf-0.1.0/pyproject.toml` & `gongsf-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gongsf"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
 	{ name = "BeetMacol", website = "https://beetmacol.com" },
 ]
 description = "Python bindings for the GSF Libary using ctypes"
 requires-python = ">=3.10"
 license = {text = "BSD-3-Clause"}
 classifiers = [
```

