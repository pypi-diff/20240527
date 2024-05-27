# Comparing `tmp/qs_codec-0.2.2.tar.gz` & `tmp/qs_codec-1.0.0.tar.gz`

## Comparing `qs_codec-0.2.2.tar` & `qs_codec-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 qs_codec-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.2.2/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.2.2/requirements_dev.txt
--rw-r--r--   0        0        0    28807 2020-02-02 00:00:00.000000 qs_codec-0.2.2/docs/README.rst
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/__init__.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/decode.py
--rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/encode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/__init__.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/charset.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/duplicates.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/format.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/list_format.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/sentinel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/decode_options.py
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/encode_options.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/undefined.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/weak_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/decode_utils.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/encode_utils.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/str_utils.py
--rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/__init__.py
--rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/compare_outputs.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/package.json
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/qs.js
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/qs.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/test_cases.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/e2e/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/e2e/e2e_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/__init__.py
--rw-r--r--   0        0        0    30061 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/decode_test.py
--rw-r--r--   0        0        0    51290 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/encode_test.py
--rw-r--r--   0        0        0    22222 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/example_test.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/fixed_qs_issues_test.py
--rw-r--r--   0        0        0    14910 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/utils_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/weakref_test.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.2.2/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.2.2/LICENSE
--rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 qs_codec-0.2.2/README.rst
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 qs_codec-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 qs_codec-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 qs_codec-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-1.0.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-1.0.0/requirements_dev.txt
+-rw-r--r--   0        0        0    28805 2020-02-02 00:00:00.000000 qs_codec-1.0.0/docs/README.rst
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/__init__.py
+-rw-r--r--   0        0        0     6945 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/decode.py
+-rw-r--r--   0        0        0    10376 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/encode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/enums/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/enums/charset.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/enums/duplicates.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/enums/format.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/enums/list_format.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/enums/sentinel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/models/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/models/decode_options.py
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/models/encode_options.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/models/undefined.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/models/weak_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/utils/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/utils/decode_utils.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/utils/encode_utils.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/utils/str_utils.py
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 qs_codec-1.0.0/src/qs_codec/utils/utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/comparison/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/comparison/__init__.py
+-rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/comparison/compare_outputs.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/comparison/package.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/comparison/qs.js
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/comparison/qs.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/comparison/test_cases.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/e2e/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/e2e/e2e_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0    30061 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/unit/decode_test.py
+-rw-r--r--   0        0        0    51290 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/unit/encode_test.py
+-rw-r--r--   0        0        0    22222 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/unit/example_test.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/unit/fixed_qs_issues_test.py
+-rw-r--r--   0        0        0    14910 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/unit/utils_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-1.0.0/tests/unit/weakref_test.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-1.0.0/LICENSE
+-rw-r--r--   0        0        0    36419 2020-02-02 00:00:00.000000 qs_codec-1.0.0/README.rst
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 qs_codec-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    38038 2020-02-02 00:00:00.000000 qs_codec-1.0.0/PKG-INFO
```

### Comparing `qs_codec-0.2.2/CHANGELOG.md` & `qs_codec-1.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.0.0
+
+* [CHORE] first stable release
+
 ## 0.2.2
 
 * [FEAT] `decode` returns `dict[str, Any]` instead of `dict` ([#4](https://github.com/techouse/qs_codec/pull/4))
 * [FIX] fix decoding encoded square brackets in key names
 
 ## 0.2.1
```

### Comparing `qs_codec-0.2.2/CODE-OF-CONDUCT.md` & `qs_codec-1.0.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/docs/README.rst` & `qs_codec-1.0.0/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 ^^^^^^^^^^^^
 
 .. code:: python
 
    import qs_codec, typing as t
 
    def decode(
-       value: t.Optional[t.Union[str, t.Mapping]],
-       options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
+       value: t.Optional[t.Union[str, t.Dict[str, t.Any]]],
+       options: DecodeOptions = DecodeOptions(),
    ) -> t.Dict[str, t.Any]:
-       """Decodes a str or Mapping into a Dict. 
+       """Decodes a query string into a Dict[str, Any].
        
        Providing custom DecodeOptions will override the default behavior."""
        pass
 
 :py:attr:`decode <qs_codec.decode>` allows you to create nested ``dict``\ s within your query
 strings, by surrounding the name of sub-keys with square brackets
 ``[]``. For example, the string ``'foo[bar]=baz'`` converts to:
```

### Comparing `qs_codec-0.2.2/src/qs_codec/decode.py` & `qs_codec-1.0.0/src/qs_codec/decode.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from .enums.sentinel import Sentinel
 from .models.decode_options import DecodeOptions
 from .models.undefined import Undefined
 from .utils.utils import Utils
 
 
 def decode(
-    value: t.Optional[t.Union[str, t.Dict[str, t.Any]]], options: DecodeOptions = DecodeOptions()
+    value: t.Optional[t.Union[str, t.Dict[str, t.Any]]],
+    options: DecodeOptions = DecodeOptions(),
 ) -> t.Dict[str, t.Any]:
     """
-    Decodes a ``str`` or ``Mapping`` into a ``dict``.
+    Decodes a query string into a ``Dict[str, Any]``.
 
     Providing custom ``DecodeOptions`` will override the default behavior.
     """
     obj: t.Dict[str, t.Any] = {}
 
     if not value:
         return obj
```

### Comparing `qs_codec-0.2.2/src/qs_codec/encode.py` & `qs_codec-1.0.0/src/qs_codec/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .models.undefined import Undefined
 from .models.weak_wrapper import WeakWrapper
 from .utils.utils import Utils
 
 
 def encode(value: t.Any, options: EncodeOptions = EncodeOptions()) -> str:
     """
-    Encodes ``Any`` object into a query ``str`` ing.
+    Encodes an object into a query string.
 
     Providing custom ``EncodeOptions`` will override the default behavior.
     """
     if value is None:
         return ""
 
     obj: t.Mapping[str, t.Any]
```

### Comparing `qs_codec-0.2.2/src/qs_codec/enums/format.py` & `qs_codec-1.0.0/src/qs_codec/enums/format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/enums/list_format.py` & `qs_codec-1.0.0/src/qs_codec/enums/list_format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/enums/sentinel.py` & `qs_codec-1.0.0/src/qs_codec/enums/sentinel.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/models/decode_options.py` & `qs_codec-1.0.0/src/qs_codec/models/decode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/models/encode_options.py` & `qs_codec-1.0.0/src/qs_codec/models/encode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/models/weak_wrapper.py` & `qs_codec-1.0.0/src/qs_codec/models/weak_wrapper.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/utils/decode_utils.py` & `qs_codec-1.0.0/src/qs_codec/utils/decode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/utils/encode_utils.py` & `qs_codec-1.0.0/src/qs_codec/utils/encode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/utils/str_utils.py` & `qs_codec-1.0.0/src/qs_codec/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/src/qs_codec/utils/utils.py` & `qs_codec-1.0.0/src/qs_codec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/comparison/qs.py` & `qs_codec-1.0.0/tests/comparison/qs.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/comparison/test_cases.json` & `qs_codec-1.0.0/tests/comparison/test_cases.json`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/e2e/e2e_test.py` & `qs_codec-1.0.0/tests/e2e/e2e_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/unit/decode_test.py` & `qs_codec-1.0.0/tests/unit/decode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/unit/encode_test.py` & `qs_codec-1.0.0/tests/unit/encode_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/unit/example_test.py` & `qs_codec-1.0.0/tests/unit/example_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/unit/utils_test.py` & `qs_codec-1.0.0/tests/unit/utils_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/tests/unit/weakref_test.py` & `qs_codec-1.0.0/tests/unit/weakref_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/.gitignore` & `qs_codec-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/LICENSE` & `qs_codec-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.2/README.rst` & `qs_codec-1.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 ^^^^^^^^^^^^
 
 .. code:: python
 
    import qs_codec, typing as t
 
    def decode(
-       value: t.Optional[t.Union[str, t.Mapping]],
-       options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
+       value: t.Optional[t.Union[str, t.Dict[str, t.Any]]],
+       options: DecodeOptions = DecodeOptions(),
    ) -> t.Dict[str, t.Any]:
-       """Decodes a str or Mapping into a Dict. 
+       """Decodes a query string into a Dict[str, Any].
        
        Providing custom DecodeOptions will override the default behavior."""
        pass
 
 `decode <https://techouse.github.io/qs_codec/qs_codec.html#module-qs_codec.decode>`__ allows you to create nested ``dict``\ s within your query
 strings, by surrounding the name of sub-keys with square brackets
 ``[]``. For example, the string ``'foo[bar]=baz'`` converts to:
```

### Comparing `qs_codec-0.2.2/pyproject.toml` & `qs_codec-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "codec",
     "url",
     "query",
     "querystring",
     "query-string",
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `qs_codec-0.2.2/PKG-INFO` & `qs_codec-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: qs-codec
-Version: 0.2.2
+Version: 1.0.0
 Summary: A query string encoding and decoding library for Python. Ported from qs for JavaScript.
 Project-URL: Homepage, https://techouse.github.io/qs_codec/
 Project-URL: Documentation, https://techouse.github.io/qs_codec/
 Project-URL: Source, https://github.com/techouse/qs_codec
 Project-URL: Changelog, https://github.com/techouse/qs_codec/blob/master/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: BSD-3-Clause
 License-File: LICENSE
 Keywords: codec,qs,query,query-string,querystring,url
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -66,18 +66,18 @@
 ^^^^^^^^^^^^
 
 .. code:: python
 
    import qs_codec, typing as t
 
    def decode(
-       value: t.Optional[t.Union[str, t.Mapping]],
-       options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
+       value: t.Optional[t.Union[str, t.Dict[str, t.Any]]],
+       options: DecodeOptions = DecodeOptions(),
    ) -> t.Dict[str, t.Any]:
-       """Decodes a str or Mapping into a Dict. 
+       """Decodes a query string into a Dict[str, Any].
        
        Providing custom DecodeOptions will override the default behavior."""
        pass
 
 `decode <https://techouse.github.io/qs_codec/qs_codec.html#module-qs_codec.decode>`__ allows you to create nested ``dict``\ s within your query
 strings, by surrounding the name of sub-keys with square brackets
 ``[]``. For example, the string ``'foo[bar]=baz'`` converts to:
```

