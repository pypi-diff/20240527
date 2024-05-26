# Comparing `tmp/repro-apk-0.2.6.tar.gz` & `tmp/repro-apk-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repro-apk-0.2.6.tar", last modified: Thu May 16 18:31:58 2024, max compression
+gzip compressed data, was "repro-apk-0.2.7.tar", last modified: Sun May 26 23:49:28 2024, max compression
```

## Comparing `repro-apk-0.2.6.tar` & `repro-apk-0.2.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwx------   0 fay       (1000) fay       (1000)        0 2024-05-16 18:31:58.977356 repro-apk-0.2.6/
--rw-------   0 fay       (1000) fay       (1000)       23 2024-05-16 18:21:27.000000 repro-apk-0.2.6/.flake8
--rw-------   0 fay       (1000) fay       (1000)       73 2024-05-16 18:21:27.000000 repro-apk-0.2.6/.gitignore
--rw-------   0 fay       (1000) fay       (1000)      140 2024-05-16 18:21:27.000000 repro-apk-0.2.6/.pylintrc
--rw-------   0 fay       (1000) fay       (1000)    35149 2024-05-16 18:21:27.000000 repro-apk-0.2.6/LICENSE.GPLv3
--rw-------   0 fay       (1000) fay       (1000)      139 2024-05-16 18:21:27.000000 repro-apk-0.2.6/MANIFEST.in
--rw-------   0 fay       (1000) fay       (1000)    10395 2024-05-16 18:21:27.000000 repro-apk-0.2.6/Makefile
--rw-------   0 fay       (1000) fay       (1000)    34272 2024-05-16 18:31:58.977356 repro-apk-0.2.6/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)    32842 2024-05-16 18:21:27.000000 repro-apk-0.2.6/README.md
--rw-------   0 fay       (1000) fay       (1000)     1346 2024-05-16 18:21:27.000000 repro-apk-0.2.6/changelog.txt
-drwx------   0 fay       (1000) fay       (1000)        0 2024-05-16 18:31:58.973356 repro-apk-0.2.6/repro_apk/
--rw-------   0 fay       (1000) fay       (1000)    16728 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/__init__.py
--rwx------   0 fay       (1000) fay       (1000)    77054 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/binres.py
--rwx------   0 fay       (1000) fay       (1000)    14505 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/diff_zip_meta.py
--rwx------   0 fay       (1000) fay       (1000)     5546 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/dump_arsc.py
--rwx------   0 fay       (1000) fay       (1000)     5536 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/dump_axml.py
--rwx------   0 fay       (1000) fay       (1000)    11653 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/dump_baseline.py
--rwx------   0 fay       (1000) fay       (1000)     6047 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/fix_compresslevel.py
--rwx------   0 fay       (1000) fay       (1000)     6506 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/fix_files.py
--rwx------   0 fay       (1000) fay       (1000)     6900 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/fix_newlines.py
--rwx------   0 fay       (1000) fay       (1000)     9707 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/fix_pg_map_id.py
--rwx------   0 fay       (1000) fay       (1000)     7324 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/inplace_fix.py
--rwx------   0 fay       (1000) fay       (1000)     3478 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/list_compresslevel.py
--rw-------   0 fay       (1000) fay       (1000)        0 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/py.typed
--rwx------   0 fay       (1000) fay       (1000)     5524 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/rm_files.py
--rwx------   0 fay       (1000) fay       (1000)     5511 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/sort_apk.py
--rwx------   0 fay       (1000) fay       (1000)     7208 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/sort_baseline.py
--rwx------   0 fay       (1000) fay       (1000)     7276 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/zipalign.py
--rwx------   0 fay       (1000) fay       (1000)    11965 2024-05-16 18:21:27.000000 repro-apk-0.2.6/repro_apk/zipinfo.py
-drwx------   0 fay       (1000) fay       (1000)        0 2024-05-16 18:31:58.977356 repro-apk-0.2.6/repro_apk.egg-info/
--rw-------   0 fay       (1000) fay       (1000)    34272 2024-05-16 18:31:58.000000 repro-apk-0.2.6/repro_apk.egg-info/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)      735 2024-05-16 18:31:58.000000 repro-apk-0.2.6/repro_apk.egg-info/SOURCES.txt
--rw-------   0 fay       (1000) fay       (1000)        1 2024-05-16 18:31:58.000000 repro-apk-0.2.6/repro_apk.egg-info/dependency_links.txt
--rw-------   0 fay       (1000) fay       (1000)       96 2024-05-16 18:31:58.000000 repro-apk-0.2.6/repro_apk.egg-info/entry_points.txt
--rw-------   0 fay       (1000) fay       (1000)       11 2024-05-16 18:31:58.000000 repro-apk-0.2.6/repro_apk.egg-info/requires.txt
--rw-------   0 fay       (1000) fay       (1000)       10 2024-05-16 18:31:58.000000 repro-apk-0.2.6/repro_apk.egg-info/top_level.txt
--rw-------   0 fay       (1000) fay       (1000)       38 2024-05-16 18:31:58.977356 repro-apk-0.2.6/setup.cfg
--rw-------   0 fay       (1000) fay       (1000)     1973 2024-05-16 18:21:27.000000 repro-apk-0.2.6/setup.py
+drwx------   0 fay       (1000) fay       (1000)        0 2024-05-26 23:49:28.414961 repro-apk-0.2.7/
+-rw-------   0 fay       (1000) fay       (1000)       23 2024-05-26 23:40:17.000000 repro-apk-0.2.7/.flake8
+-rw-------   0 fay       (1000) fay       (1000)       73 2024-05-26 23:40:17.000000 repro-apk-0.2.7/.gitignore
+-rw-------   0 fay       (1000) fay       (1000)      126 2024-05-26 23:40:17.000000 repro-apk-0.2.7/.pylintrc
+-rw-------   0 fay       (1000) fay       (1000)    35149 2024-05-26 23:40:17.000000 repro-apk-0.2.7/LICENSE.GPLv3
+-rw-------   0 fay       (1000) fay       (1000)      139 2024-05-26 23:40:17.000000 repro-apk-0.2.7/MANIFEST.in
+-rw-------   0 fay       (1000) fay       (1000)    10395 2024-05-26 23:40:17.000000 repro-apk-0.2.7/Makefile
+-rw-------   0 fay       (1000) fay       (1000)    34272 2024-05-26 23:49:28.414961 repro-apk-0.2.7/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)    32842 2024-05-26 23:40:17.000000 repro-apk-0.2.7/README.md
+-rw-------   0 fay       (1000) fay       (1000)     1554 2024-05-26 23:40:17.000000 repro-apk-0.2.7/changelog.txt
+drwx------   0 fay       (1000) fay       (1000)        0 2024-05-26 23:49:28.414961 repro-apk-0.2.7/repro_apk/
+-rw-------   0 fay       (1000) fay       (1000)    16728 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/__init__.py
+-rwx------   0 fay       (1000) fay       (1000)    86306 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/binres.py
+-rwx------   0 fay       (1000) fay       (1000)    14505 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/diff_zip_meta.py
+-rwx------   0 fay       (1000) fay       (1000)     5546 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/dump_arsc.py
+-rwx------   0 fay       (1000) fay       (1000)     5536 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/dump_axml.py
+-rwx------   0 fay       (1000) fay       (1000)    11653 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/dump_baseline.py
+-rwx------   0 fay       (1000) fay       (1000)     6047 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/fix_compresslevel.py
+-rwx------   0 fay       (1000) fay       (1000)     6506 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/fix_files.py
+-rwx------   0 fay       (1000) fay       (1000)     6900 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/fix_newlines.py
+-rwx------   0 fay       (1000) fay       (1000)     9707 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/fix_pg_map_id.py
+-rwx------   0 fay       (1000) fay       (1000)     7358 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/inplace_fix.py
+-rwx------   0 fay       (1000) fay       (1000)     3478 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/list_compresslevel.py
+-rw-------   0 fay       (1000) fay       (1000)        0 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/py.typed
+-rwx------   0 fay       (1000) fay       (1000)     5524 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/rm_files.py
+-rwx------   0 fay       (1000) fay       (1000)     5511 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/sort_apk.py
+-rwx------   0 fay       (1000) fay       (1000)     7174 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/sort_baseline.py
+-rwx------   0 fay       (1000) fay       (1000)     7276 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/zipalign.py
+-rwx------   0 fay       (1000) fay       (1000)    11965 2024-05-26 23:40:17.000000 repro-apk-0.2.7/repro_apk/zipinfo.py
+drwx------   0 fay       (1000) fay       (1000)        0 2024-05-26 23:49:28.414961 repro-apk-0.2.7/repro_apk.egg-info/
+-rw-------   0 fay       (1000) fay       (1000)    34272 2024-05-26 23:49:28.000000 repro-apk-0.2.7/repro_apk.egg-info/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)      735 2024-05-26 23:49:28.000000 repro-apk-0.2.7/repro_apk.egg-info/SOURCES.txt
+-rw-------   0 fay       (1000) fay       (1000)        1 2024-05-26 23:49:28.000000 repro-apk-0.2.7/repro_apk.egg-info/dependency_links.txt
+-rw-------   0 fay       (1000) fay       (1000)       96 2024-05-26 23:49:28.000000 repro-apk-0.2.7/repro_apk.egg-info/entry_points.txt
+-rw-------   0 fay       (1000) fay       (1000)       11 2024-05-26 23:49:28.000000 repro-apk-0.2.7/repro_apk.egg-info/requires.txt
+-rw-------   0 fay       (1000) fay       (1000)       10 2024-05-26 23:49:28.000000 repro-apk-0.2.7/repro_apk.egg-info/top_level.txt
+-rw-------   0 fay       (1000) fay       (1000)       38 2024-05-26 23:49:28.414961 repro-apk-0.2.7/setup.cfg
+-rw-------   0 fay       (1000) fay       (1000)     1973 2024-05-26 23:40:17.000000 repro-apk-0.2.7/setup.py
```

### Comparing `repro-apk-0.2.6/LICENSE.GPLv3` & `repro-apk-0.2.7/LICENSE.GPLv3`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/Makefile` & `repro-apk-0.2.7/Makefile`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/PKG-INFO` & `repro-apk-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repro-apk
-Version: 0.2.6
+Version: 0.2.7
 Summary: scripts to make android apks reproducible
 Home-page: https://github.com/obfusk/reproducible-apk-tools
 Author: FC (Fay) Stegerman
 Author-email: flx@obfusk.net
 License: GPLv3+
 Keywords: android apk reproducible
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repro-apk Version: 0.2.6 Summary: scripts to make
+Metadata-Version: 2.1 Name: repro-apk Version: 0.2.7 Summary: scripts to make
 android apks reproducible Home-page: https://github.com/obfusk/reproducible-
 apk-tools Author: FC (Fay) Stegerman Author-email: flx@obfusk.net License:
 GPLv3+ Keywords: android apk reproducible Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Intended Audience ::
 Telecommunications Industry Classifier: License :: OSI Approved :: GNU General
```

### Comparing `repro-apk-0.2.6/README.md` & `repro-apk-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/changelog.txt` & `repro-apk-0.2.7/changelog.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v0.2.7
+
+• binres.py: add get_manifest_info(), load_and_list_apk(); refactoring.
+• binres.py: fix offset for null-terminated UTF-8 check.
+• inplace-fix.py: cleanup/refactor variables in zipalign_cmd().
+
 v0.2.6
 
 • add binres.py.
 • fix compatibility w/ python 3.13 ZipInfo .compress_level changes.
 
 v0.2.5
```

### Comparing `repro-apk-0.2.6/repro_apk/__init__.py` & `repro-apk-0.2.7/repro_apk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from . import sort_apk as _sort_apk
 from . import sort_baseline as _sort_baseline
 from . import zipalign as _zipalign
 from . import zipinfo as _zipinfo
 
 import click
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 NAME = "repro-apk"
 
 ERRORS = (
     _binres.Error,
     _diff_zip_meta.Error,
     _dump_arsc.Error,
     _dump_axml.Error,
```

### Comparing `repro-apk-0.2.6/repro_apk/binres.py` & `repro-apk-0.2.7/repro_apk/binres.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,16 +135,16 @@
 import zlib
 
 from collections import namedtuple
 from dataclasses import dataclass, field
 from enum import Enum
 from fnmatch import fnmatch
 from functools import cached_property, lru_cache
-from typing import (cast, Any, BinaryIO, Callable, ClassVar, Dict, Iterable,
-                    Iterator, List, Optional, TextIO, Tuple, Union, TYPE_CHECKING)
+from typing import (cast, Any, BinaryIO, Callable, ClassVar, Dict, Iterable, Iterator,
+                    List, Optional, Set, TextIO, Tuple, Union, TYPE_CHECKING)
 
 # https://android.googlesource.com/platform/tools/base
 #   apkparser/binary-resources/src/main/java/com/google/devrel/gmscore/tools/apk/arsc/*.java
 # https://android.googlesource.com/platform/frameworks/base
 #   libs/androidfw/include/androidfw/ResourceTypes.h
 #   tools/aapt2/ResourceValues.cpp
 
@@ -481,18 +481,56 @@
         chunk = cls(**d, namespace_idx=_noref(ns_idx), name_idx=name_idx,
                     id_idx=_noref(id_idx - 1), class_idx=_noref(class_idx - 1),
                     style_idx=_noref(style_idx - 1), attributes=())
         attrs = tuple(_read_attrs(data, weakref.ref(chunk), attr_start - 20, n_attrs))
         object.__setattr__(chunk, "attributes", attrs)
         return chunk
 
-    @property
+    def attr_as_bool(self, name: str, **kwargs: Any) -> Optional[bool]:
+        """Get bool attr."""
+        value = self._attr_as(bool, name, **kwargs)
+        assert value is None or isinstance(value, bool)
+        return value
+
+    def attr_as_int(self, name: str, **kwargs: Any) -> Optional[int]:
+        """Get int attr."""
+        value = self._attr_as(int, name, **kwargs)
+        assert value is None or isinstance(value, int)
+        return value
+
+    def attr_as_str(self, name: str, **kwargs: Any) -> Optional[str]:
+        """Get str attr."""
+        value = self._attr_as(str, name, **kwargs)
+        assert value is None or isinstance(value, str)
+        return value
+
+    def _attr_as(self, typ: type, name: str, *, android: bool = False,
+                 optional: bool = False) -> Any:
+        brv_type = py_type_to_brv_type(typ)
+        if android:
+            name = f"{{{SCHEMA_ANDROID}}}{name}"
+        if name not in self.attrs_as_dict:
+            if optional:
+                return None
+            raise ParseError(f"No such attribute: {name!r}")
+        attr = self.attrs_as_dict[name]
+        if attr.typed_value.type is not brv_type:
+            raise ParseError(f"Wrong type for attribute {name!r}: "
+                             f"expected {brv_type.name}, got {attr.typed_value.type.name}")
+        return brv_to_py(attr.typed_value, attr.raw_value)[2]
+
+    @cached_property
     def attrs_as_dict(self) -> Dict[str, XMLAttr]:
         """XML attributes as dict."""
-        return {a.name_with_ns: a for a in self.attributes}
+        d = {}
+        for a in self.attributes:
+            if (n := a.name_with_ns) in d:
+                raise ParseError(f"Duplicate attribute name: {n!r}")
+            d[n] = a
+        return d
 
     @property
     def namespace(self) -> str:
         """Get namespace string."""
         return self.string(self.namespace_idx)
 
     @property
@@ -1140,14 +1178,42 @@
         return self.string(self.raw_value_idx)
 
     @classmethod
     def fields(cls) -> Tuple[Tuple[str, str, int, Optional[str]], ...]:
         return _fields(cls)     # type: ignore[arg-type]
 
 
+@dataclass(frozen=True)
+class UsesFeature:
+    """AndroidManifest.xml uses-feature."""
+    name: str
+    required: bool
+
+
+@dataclass(frozen=True)
+class UsesPermission:
+    """AndroidManifest.xml uses-permission(-sdk-23)."""
+    name: str
+    min_sdk_version: Optional[int]
+    max_sdk_version: Optional[int]
+
+
+@dataclass(frozen=True)
+class ManifestInfo:
+    """AndroidManifest.xml data."""
+    appid: str
+    version_code: int
+    version_name: str
+    min_sdk: int
+    target_sdk: int
+    features: List[UsesFeature]
+    permissions: List[UsesPermission]
+    abis: Optional[List[str]]
+
+
 if TYPE_CHECKING:
     ChunkRef = weakref.ReferenceType[Chunk]
     StringPoolChunkRef = weakref.ReferenceType[StringPoolChunk]
     XMLNodeChunkRef = weakref.ReferenceType[XMLNodeChunk]
     TypeChunkRef = weakref.ReferenceType[TypeChunk]
 else:
     ChunkRef = weakref.ReferenceType
@@ -1577,38 +1643,48 @@
         return f"#{i:08x}"
 
     t, T = brv.type, BinResVal.Type
     if t is T.NULL:
         if brv.size == 0 and raw_value:
             return repr, str, raw_value
         return null2s, null2s, brv.data
-    elif t is T.REFERENCE:
+    if t is T.REFERENCE:
         return ref2s, ref2s, brv.data
-    elif t is T.ATTRIBUTE:
+    if t is T.ATTRIBUTE:
         return attr2s, attr2s, brv.data
-    elif t is T.STRING:
+    if t is T.STRING:
         return repr, str, raw_value
-    elif t is T.FLOAT:
+    if t is T.FLOAT:
         return f2s, f2s, struct.unpack("<f", struct.pack("<I", brv.data))[0]
-    elif t is T.DIMENSION:
+    if t is T.DIMENSION:
         return c2s, c2s, BinResVal.complex2pair(brv.data, fraction=False)
-    elif t is T.FRACTION:
+    if t is T.FRACTION:
         return c2s, c2s, BinResVal.complex2pair(brv.data, fraction=True)
-    elif t in (T.DYNAMIC_REFERENCE, T.DYNAMIC_ATTRIBUTE):
+    if t in (T.DYNAMIC_REFERENCE, T.DYNAMIC_ATTRIBUTE):
         raise NotImplementedError("Dynamic reference/attribute not (yet) supported")
-    elif t is T.INT_DEC:
+    if t is T.INT_DEC:
         return str, str, brv.data
-    elif t is T.INT_HEX:
+    if t is T.INT_HEX:
         return i2h, i2h, brv.data
-    elif t is T.INT_BOOLEAN:
+    if t is T.INT_BOOLEAN:
         return b2s, b2s, (False if brv.data == 0 else True)
-    elif t in (T.INT_COLOR_ARGB8, T.INT_COLOR_RGB8, T.INT_COLOR_ARGB4, T.INT_COLOR_RGB4):
+    if t in (T.INT_COLOR_ARGB8, T.INT_COLOR_RGB8, T.INT_COLOR_ARGB4, T.INT_COLOR_RGB4):
         return clr2s, clr2s, brv.data
-    else:
-        raise ValueError(f"Unsupported value type {t.name}")
+    raise ValueError(f"Unsupported value type {t.name}")
+
+
+def py_type_to_brv_type(typ: type) -> BinResVal.Type:
+    """Python type to BinResVal.Type (must be bool, int, str)."""
+    if typ is bool:
+        return BinResVal.Type.INT_BOOLEAN
+    if typ is int:
+        return BinResVal.Type.INT_DEC
+    if typ is str:
+        return BinResVal.Type.STRING
+    raise ValueError(f"Unsupported type {typ.__name__}")
 
 
 def parse(data: bytes) -> Tuple[Chunk, ...]:
     """Parse raw data to AXML/ARSC chunks."""
     return tuple(read_chunks(data))
 
 
@@ -1748,15 +1824,15 @@
         j, n = _decode_strlen(data, off + i, codec)
         a, b = off + i + j, off + i + j + n
         if data[b] != 0:
             if j != 2:
                 raise ParseError("UTF-8 string not null-terminated")
             b = data.index(b"\x00", b)
             x = b - a
-            if data[off:off + 2] != bytes([(x & 0x7F00) >> 8 | 0x80, x & 0xFF]):
+            if data[off + i:off + i + 2] != bytes([(x & 0x7F00) >> 8 | 0x80, x & 0xFF]):
                 raise ParseError("UTF-8 string not null-terminated")
             log = logging.getLogger(__name__)
             log.warning(f"UTF-8 string null-terminator/length mismatch: expected {n}, got {x}")
         try:
             s = data[a:b].decode(codec)
             k = len(s)
         except UnicodeDecodeError:
@@ -1856,70 +1932,180 @@
 
 def _safe(x: Any) -> str:
     if not isinstance(x, str):
         return repr(x)
     return "".join(c if c.isprintable() and c != '\\' else repr(c)[1:-1] for c in x)
 
 
+def quick_get_idver_perms(apk: str) \
+        -> Tuple[Tuple[str, int, str], Iterator[Tuple[str, Tuple[Tuple[str, str], ...]]]]:
+    chunk = read_chunk(quick_load(apk, MANIFEST))[0]
+    if not isinstance(chunk, XMLChunk):
+        raise ParseError("Expected XMLChunk")
+    return quick_get_idver(apk, chunk=chunk), quick_get_perms(apk, chunk=chunk)
+
+
 # FIXME
 def quick_get_idver(apk: str, *, chunk: Optional[XMLChunk] = None) -> Tuple[str, int, str]:
     """Quickly get appid & version code/name from APK."""
-    manifest = quick_get_manifest(apk, chunk=chunk)
-    appid = vercode = vername = None
-    for a in manifest.attributes:
-        if a.name == "package" and not a.namespace:
-            appid = a.raw_value
-        elif a.name == "versionCode" and a.namespace == SCHEMA_ANDROID:
-            vercode = a.typed_value.data
-        elif a.name == "versionName" and a.namespace == SCHEMA_ANDROID:
-            vername = a.raw_value
-        if appid is not None and vercode is not None and vername is not None:
-            break
-    else:
-        raise ParseError("Could not find required attribute(s)")
-    return appid, vercode, vername
+    return _manifest_idver(quick_get_manifest(apk, chunk=chunk))
 
 
 # FIXME
 def quick_get_perms(apk: str, *, chunk: Optional[XMLChunk] = None) \
         -> Iterator[Tuple[str, Tuple[Tuple[str, str], ...]]]:
     """Quickly get permissions from APK."""
     if chunk is None:
         first = read_chunk(quick_load(apk, MANIFEST))[0]
         if not isinstance(first, XMLChunk):
-            raise Error("Expected XMLChunk")
+            raise ParseError("Expected XMLChunk")
         chunk = first
-    perm_tags = ("uses-permission", "uses-permission-sdk-23", "permission")
-    in_manifest = False
     for c in chunk.children:
-        if isinstance(c, XMLElemStartChunk):
-            if c.level == 2:
-                in_manifest = c.name == "manifest"
-            elif in_manifest and c.level == 3 and c.name in perm_tags:
-                perm, attrs = None, []
-                if c.name == "uses-permission-sdk-23":
-                    attrs.append(("minSdkVersion", "23"))
-                elif c.name == "permission":
-                    attrs.append(("declaration", "true"))
-                for a in c.attributes:
-                    if a.name == "name" and a.namespace == SCHEMA_ANDROID:
-                        perm = a.raw_value
-                    else:
-                        attrs.append((a.name, brv_str(a.typed_value, a.raw_value)))
-                if perm is None:
-                    raise ParseError("Could not find required attribute 'name'")
-                yield perm, tuple(attrs)
+        if isinstance(c, XMLElemStartChunk) and c.level == 3 and _is_perm_tag(c):
+            yield _perm_from_tag(c)
 
 
-def quick_get_idver_perms(apk: str) \
-        -> Tuple[Tuple[str, int, str], Iterator[Tuple[str, Tuple[Tuple[str, str], ...]]]]:
-    chunk = read_chunk(quick_load(apk, MANIFEST))[0]
+# FIXME
+def get_manifest_info(axml: bytes, files: Optional[Set[str]] = None) -> ManifestInfo:
+    r"""
+    Get ManifestInfo from AXML (and optionally list of APK files for abis).
+
+    >>> import dataclasses
+    >>> with open("test/data/AndroidManifest-catima.xml", "rb") as fh:
+    ...     axml = fh.read()
+    >>> man = get_manifest_info(axml)
+    >>> for field in dataclasses.fields(man):
+    ...     x = getattr(man, field.name)
+    ...     if isinstance(x, list):
+    ...         print(f"{field.name}:")
+    ...         for y in x:
+    ...             print(f"  {y!r}")
+    ...     else:
+    ...         print(f"{field.name}={x!r}")
+    appid='me.hackerchick.catima'
+    version_code=134
+    version_name='2.29.0'
+    min_sdk=21
+    target_sdk=34
+    features:
+      UsesFeature(name='android.hardware.camera', required=True)
+      UsesFeature(name='android.hardware.camera.autofocus', required=False)
+      UsesFeature(name='android.hardware.camera.front', required=False)
+      UsesFeature(name='android.hardware.camera.flash', required=False)
+      UsesFeature(name='android.hardware.screen.landscape', required=False)
+      UsesFeature(name='android.hardware.wifi', required=False)
+    permissions:
+      UsesPermission(name='android.permission.CAMERA', min_sdk_version=None, max_sdk_version=None)
+      UsesPermission(name='android.permission.READ_EXTERNAL_STORAGE', min_sdk_version=None, max_sdk_version=23)
+      UsesPermission(name='me.hackerchick.catima.DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION', min_sdk_version=None, max_sdk_version=None)
+    abis=None
+
+    """
+    chunk = read_chunk(axml)[0]
     if not isinstance(chunk, XMLChunk):
-        raise Error("Expected XMLChunk")
-    return quick_get_idver(apk, chunk=chunk), quick_get_perms(apk, chunk=chunk)
+        raise ParseError("Expected XMLChunk")
+    return _get_manifest_info(chunk, files)
+
+
+# FIXME
+# FIXME: minSdkVersion/targetSdkVersion="Q"
+def _get_manifest_info(chunk: XMLChunk, files: Optional[Set[str]] = None) -> ManifestInfo:
+    namespace = manifest = uses_sdk = abis = None
+    min_sdk = target_sdk = 1
+    features: List[UsesFeature] = []
+    permissions: List[UsesPermission] = []
+    if files:
+        abis = sorted(set(f.split("/")[1] for f in files
+                          if f.startswith("lib/") and f.endswith(".so")))
+    for c in chunk.children:
+        if isinstance(c, XMLNSStartChunk):
+            if c.level == 1:
+                if c.prefix == "android" and c.uri == SCHEMA_ANDROID:
+                    if namespace:
+                        raise ParseError("Expected only one android namespace")
+                    namespace = c
+                else:
+                    raise ParseError("Expected android namespace")
+        elif isinstance(c, XMLElemStartChunk):
+            if c.level == 2:
+                if namespace and c.name == "manifest" and not c.namespace:
+                    if manifest:
+                        raise ParseError("Expected only one manifest element")
+                    manifest = c
+                else:
+                    raise ParseError("Expected manifest element")
+            elif not (manifest and c.level == 3 and not c.namespace):
+                continue
+            if c.name == "uses-sdk":
+                if uses_sdk:
+                    raise ParseError("Expected only one uses-sdk element")
+                uses_sdk = c
+                msv = c.attr_as_int("minSdkVersion", android=True, optional=True)
+                tsv = c.attr_as_int("targetSdkVersion", android=True, optional=True)
+                min_sdk = msv if msv is not None else 1
+                target_sdk = tsv if tsv is not None else min_sdk
+            elif c.name == "uses-feature":
+                name = c.attr_as_str("name", android=True)
+                assert name is not None
+                req = c.attr_as_bool("required", android=True, optional=True)
+                required = req if req is not None else True
+                features.append(UsesFeature(name=name, required=required))
+            elif c.name in ("uses-permission", "uses-permission-sdk-23"):
+                name = c.attr_as_str("name", android=True)
+                assert name is not None
+                min_sdk_version = 23 if c.name.endswith("-sdk-23") else None
+                max_sdk_version = c.attr_as_int("maxSdkVersion", android=True, optional=True)
+                permissions.append(UsesPermission(name=name, min_sdk_version=min_sdk_version,
+                                                  max_sdk_version=max_sdk_version))
+    if not manifest:
+        raise ParseError("No manifest element")
+    appid, vercode, vername = _manifest_idver(manifest)
+    return ManifestInfo(
+        appid=appid, version_code=vercode, version_name=vername, min_sdk=min_sdk,
+        target_sdk=target_sdk, features=features, permissions=permissions, abis=abis)
+
+
+def get_manifest_info_apk(apk: str) -> ManifestInfo:
+    r"""
+    Get ManifestInfo from APK.
+
+    >>> get_manifest_info_apk("test/data/golden-aligned-in.apk")
+    ManifestInfo(appid='android.appsecurity.cts.tinyapp', version_code=10, version_name='1.0', min_sdk=23, target_sdk=23, features=[], permissions=[], abis=['armeabi'])
+
+    """
+    file_data, files = load_and_list_apk(apk, MANIFEST)
+    return get_manifest_info(file_data[MANIFEST], files)
+
+
+# NB: includes declarations
+def _is_perm_tag(chunk: XMLElemStartChunk) -> bool:
+    return not chunk.namespace and chunk.name in (
+        "uses-permission", "uses-permission-sdk-23", "permission")
+
+
+# FIXME
+def _perm_from_tag(chunk: XMLElemStartChunk) -> Tuple[str, Tuple[Tuple[str, str], ...]]:
+    perm = chunk.attr_as_str("name", android=True)
+    assert perm is not None
+    attrs = {a.name: brv_str(a.typed_value, a.raw_value)
+             for a in chunk.attrs_as_dict.values()
+             if a.name_with_ns != f"{{{SCHEMA_ANDROID}}}name"}
+    if chunk.name == "uses-permission-sdk-23":
+        attrs["minSdkVersion"] = "23"
+    elif chunk.name == "permission":
+        attrs["declaration"] = "true"
+    return perm, tuple(attrs.items())
+
+
+def _manifest_idver(manifest: XMLElemStartChunk) -> Tuple[str, int, str]:
+    appid = manifest.attr_as_str("package")
+    vercode = manifest.attr_as_int("versionCode", android=True)
+    vername = manifest.attr_as_str("versionName", android=True)
+    assert appid is not None and vercode is not None and vername is not None
+    return appid, vercode, vername
 
 
 # FIXME
 def quick_get_manifest(apk: str, *, chunk: Optional[XMLChunk] = None) -> XMLElemStartChunk:
     """Quickly get manifest XMLElemStartChunk (w/o children) from APK."""
     if chunk is None:
         tid, d, _ = _read_chunk(quick_load(apk, MANIFEST))
@@ -1943,57 +2129,106 @@
     else:
         for c in chunk.children:
             if isinstance(c, XMLElemStartChunk):
                 start = c
                 break
         else:
             raise ParseError("Expected XMLElemStartChunk")
-    if start.name != "manifest":
+    if not (start.name == "manifest" and not start.namespace):
         raise ParseError("Expected manifest element")
     return start
 
 
 def quick_load(apk: str, filename: str) -> bytes:
     """Quickly load one file from APK."""
-    def _read_cdh(fh: BinaryIO) -> Tuple[bytes, int, int, int]:
-        hdr = fh.read(46)
-        if hdr[:4] != b"\x50\x4b\x01\x02":
-            raise ZipError("Expected central directory file header signature")
-        n, m, k = struct.unpack("<HHH", hdr[28:34])
-        hdr += fh.read(n + m + k)
-        ctype = int.from_bytes(hdr[10:12], "little")
-        csize = int.from_bytes(hdr[20:24], "little")
-        offset = int.from_bytes(hdr[42:46], "little")
-        return hdr[46:46 + n], offset, ctype, csize
-
-    def _read_data(fh: BinaryIO, offset: int, ctype: int, csize: int) -> bytes:
-        fh.seek(offset)
-        hdr = fh.read(30)
-        if hdr[:4] != b"\x50\x4b\x03\x04":
-            raise ZipError("Expected local file header signature")
-        n, m = struct.unpack("<HH", hdr[26:30])
-        hdr += fh.read(n + m)
-        if ctype == 0:
-            return fh.read(csize)
-        elif ctype == 8:
-            return zlib.decompress(fh.read(csize), -15)
-        else:
-            raise ZipError(f"Unsupported compress_type {ctype}")
-
     filename_b = filename.encode()
     zdata = zip_data(apk)
     with open(apk, "rb") as fh:
         fh.seek(zdata.cd_offset)
         while fh.tell() < zdata.eocd_offset:
-            name, offset, ctype, csize = _read_cdh(fh)
+            name, offset, ctype, csize = _zip_read_cdh(fh)
             if name == filename_b:
-                return _read_data(fh, offset, ctype, csize)
+                return _zip_read_data(fh, offset, ctype, csize)
     raise Error(f"Entry not found: {filename!r}")
 
 
+# FIXME
+def load_and_list_apk(apk: str, *filenames: str,
+                      expand: bool = False) -> Tuple[Dict[str, bytes], Set[str]]:
+    r"""
+    Load files from APK and list all files.
+
+    >>> fd, fs = load_and_list_apk("test/data/golden-aligned-in.apk", "AndroidManifest.xml")
+    >>> sorted(fs)
+    ['AndroidManifest.xml', 'META-INF/', 'META-INF/MANIFEST.MF', 'classes.dex', 'lib/armeabi/fake.so', 'resources.arsc', 'temp.txt', 'temp2.txt']
+    >>> sorted(fd.keys())
+    ['AndroidManifest.xml']
+    >>> fd, fs = load_and_list_apk("test/data/golden-aligned-in.apk", "*.xml", "*.dex",
+    ...                            "*.arsc", "*.so", expand=True)
+    >>> sorted(fs)
+    ['AndroidManifest.xml', 'META-INF/', 'META-INF/MANIFEST.MF', 'classes.dex', 'lib/armeabi/fake.so', 'resources.arsc', 'temp.txt', 'temp2.txt']
+    >>> sorted(fd.keys())
+    ['AndroidManifest.xml', 'classes.dex', 'lib/armeabi/fake.so', 'resources.arsc']
+    >>> fd["lib/armeabi/fake.so"]
+    b'Hello\n'
+    >>> fd["AndroidManifest.xml"][:4] == AXML_MAGIC
+    True
+
+    """
+    if not expand:
+        find = set(filenames)
+    read = {}
+    files = set()
+    zdata = zip_data(apk)
+    with open(apk, "rb") as fh:
+        fh.seek(zdata.cd_offset)
+        while fh.tell() < zdata.eocd_offset:
+            name, offset, ctype, csize = _zip_read_cdh(fh)
+            filename = name.decode()
+            if filename in files:
+                raise ZipError(f"Duplicate entry: {filename!r}")
+            files.add(filename)
+            if not expand and filename not in find:
+                continue
+            if expand and not fnmatches_with_negation(filename, *filenames):
+                continue
+            read[filename] = (offset, ctype, csize)
+        if not expand and len(find) != len(read):
+            raise Error(f"Entries not found: {sorted(find - set(read))}")
+        file_data = {k: _zip_read_data(fh, o, t, s) for k, (o, t, s) in read.items()}
+    return file_data, files
+
+
+def _zip_read_cdh(fh: BinaryIO) -> Tuple[bytes, int, int, int]:
+    hdr = fh.read(46)
+    if hdr[:4] != b"\x50\x4b\x01\x02":
+        raise ZipError("Expected central directory file header signature")
+    n, m, k = struct.unpack("<HHH", hdr[28:34])
+    hdr += fh.read(n + m + k)
+    ctype = int.from_bytes(hdr[10:12], "little")
+    csize = int.from_bytes(hdr[20:24], "little")
+    offset = int.from_bytes(hdr[42:46], "little")
+    return hdr[46:46 + n], offset, ctype, csize
+
+
+def _zip_read_data(fh: BinaryIO, offset: int, ctype: int, csize: int) -> bytes:
+    fh.seek(offset)
+    hdr = fh.read(30)
+    if hdr[:4] != b"\x50\x4b\x03\x04":
+        raise ZipError("Expected local file header signature")
+    n, m = struct.unpack("<HH", hdr[26:30])
+    hdr += fh.read(n + m)
+    if ctype == 0:
+        return fh.read(csize)
+    elif ctype == 8:
+        return zlib.decompress(fh.read(csize), -15)
+    else:
+        raise ZipError(f"Unsupported compress_type {ctype}")
+
+
 def fnmatches_with_negation(filename: str, *patterns: str) -> bool:
     r"""
     Filename matching with shell patterns and negation.
 
     Checks whether filename matches any of the fnmatch patterns.
 
     An optional prefix "!" negates the pattern, invalidating a successful match
```

### Comparing `repro-apk-0.2.6/repro_apk/diff_zip_meta.py` & `repro-apk-0.2.7/repro_apk/diff_zip_meta.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/dump_arsc.py` & `repro-apk-0.2.7/repro_apk/dump_arsc.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/dump_axml.py` & `repro-apk-0.2.7/repro_apk/dump_axml.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/dump_baseline.py` & `repro-apk-0.2.7/repro_apk/dump_baseline.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/fix_compresslevel.py` & `repro-apk-0.2.7/repro_apk/fix_compresslevel.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/fix_files.py` & `repro-apk-0.2.7/repro_apk/fix_files.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/fix_newlines.py` & `repro-apk-0.2.7/repro_apk/fix_newlines.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/fix_pg_map_id.py` & `repro-apk-0.2.7/repro_apk/fix_pg_map_id.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/inplace_fix.py` & `repro-apk-0.2.7/repro_apk/inplace_fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,27 +102,27 @@
 
     """
     cmd, *args = _zipalign_cmd(page_align, page_size)
     if not internal:
         if shutil.which(cmd):
             return (cmd, *args)
         for k in SDK_ENV:
-            if v := os.environ.get(k):
-                t = os.path.join(v, "build-tools")
-                if os.path.exists(t):
-                    for v in sorted(os.listdir(t), key=_vsn, reverse=True):
-                        if page_size and _vsn(v) < _vsn(BUILD_TOOLS_WITH_PAGE_SIZE_FROM):
-                            print(f"[SKIP TOO OLD] {v}")
+            if home := os.environ.get(k):
+                tools = os.path.join(home, "build-tools")
+                if os.path.exists(tools):
+                    for vsn in sorted(os.listdir(tools), key=_vsn, reverse=True):
+                        if page_size and _vsn(vsn) < _vsn(BUILD_TOOLS_WITH_PAGE_SIZE_FROM):
+                            print(f"[SKIP TOO OLD] {vsn}")
                             continue
                         for s in BUILD_TOOLS_WITH_BROKEN_ZIPALIGN:
-                            if v.startswith(s):
-                                print(f"[SKIP BROKEN] {v}")
+                            if vsn.startswith(s):
+                                print(f"[SKIP BROKEN] {vsn}")
                                 break
                         else:
-                            c = os.path.join(t, v, cmd)
+                            c = os.path.join(tools, vsn, cmd)
                             if shutil.which(c):
                                 print(f"[FOUND] {c}")
                                 return (c, *args)
     return (*_script_cmd(cmd), *args)
 
 
 def _vsn(v: str) -> Tuple[int, ...]:
```

### Comparing `repro-apk-0.2.6/repro_apk/list_compresslevel.py` & `repro-apk-0.2.7/repro_apk/list_compresslevel.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/rm_files.py` & `repro-apk-0.2.7/repro_apk/rm_files.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/sort_apk.py` & `repro-apk-0.2.7/repro_apk/sort_apk.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/sort_baseline.py` & `repro-apk-0.2.7/repro_apk/sort_baseline.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,21 +122,19 @@
 # Supported .profm: 002
 # Unsupported .profm: 001 N
 def _sort_baseline(data: bytes) -> bytes:
     magic, data = _split(data, 4)
     version, data = _split(data, 4)
     if magic == PROF_MAGIC:
         raise Error(f"Unsupported prof version {version!r}")
-    elif magic == PROFM_MAGIC:
+    if magic == PROFM_MAGIC:
         if version == PROFM_002:
             return PROFM_MAGIC + PROFM_002 + sort_profm_002(data)
-        else:
-            raise Error(f"Unsupported profm version {version!r}")
-    else:
-        raise Error(f"Unsupported magic {magic!r}")
+        raise Error(f"Unsupported profm version {version!r}")
+    raise Error(f"Unsupported magic {magic!r}")
 
 
 def sort_profm_002(data: bytes) -> bytes:
     num_dex_files, uncompressed_data_size, compressed_data_size, data = _unpack("<HII", data)
     profiles = []
     if len(data) != compressed_data_size:
         raise Error("Compressed data size does not match")
```

### Comparing `repro-apk-0.2.6/repro_apk/zipalign.py` & `repro-apk-0.2.7/repro_apk/zipalign.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk/zipinfo.py` & `repro-apk-0.2.7/repro_apk/zipinfo.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/repro_apk.egg-info/PKG-INFO` & `repro-apk-0.2.7/repro_apk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repro-apk
-Version: 0.2.6
+Version: 0.2.7
 Summary: scripts to make android apks reproducible
 Home-page: https://github.com/obfusk/reproducible-apk-tools
 Author: FC (Fay) Stegerman
 Author-email: flx@obfusk.net
 License: GPLv3+
 Keywords: android apk reproducible
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repro-apk Version: 0.2.6 Summary: scripts to make
+Metadata-Version: 2.1 Name: repro-apk Version: 0.2.7 Summary: scripts to make
 android apks reproducible Home-page: https://github.com/obfusk/reproducible-
 apk-tools Author: FC (Fay) Stegerman Author-email: flx@obfusk.net License:
 GPLv3+ Keywords: android apk reproducible Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Intended Audience ::
 Telecommunications Industry Classifier: License :: OSI Approved :: GNU General
```

### Comparing `repro-apk-0.2.6/repro_apk.egg-info/SOURCES.txt` & `repro-apk-0.2.7/repro_apk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.6/setup.py` & `repro-apk-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 import setuptools
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 info = Path(__file__).with_name("README.md").read_text(encoding="utf8")
 
 setuptools.setup(
     name="repro-apk",
     url="https://github.com/obfusk/reproducible-apk-tools",
     description="scripts to make android apks reproducible",
```

