# Comparing `tmp/pdfnaut-0.2.0.tar.gz` & `tmp/pdfnaut-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfnaut-0.2.0.tar", last modified: Sun May  5 16:54:09 2024, max compression
+gzip compressed data, was "pdfnaut-0.3.0.tar", last modified: Sun May 26 22:42:08 2024, max compression
```

## Comparing `pdfnaut-0.2.0.tar` & `pdfnaut-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.803774 pdfnaut-0.2.0/
--rw-rw-rw-   0        0        0    10315 2024-01-02 18:49:05.000000 pdfnaut-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    14726 2024-05-05 16:54:09.803774 pdfnaut-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1880 2024-04-03 04:18:41.000000 pdfnaut-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.507081 pdfnaut-0.2.0/pdfnaut/
--rw-rw-rw-   0        0        0      320 2024-05-05 02:30:46.000000 pdfnaut-0.2.0/pdfnaut/__init__.py
--rw-rw-rw-   0        0        0      329 2024-04-23 00:33:36.000000 pdfnaut-0.2.0/pdfnaut/exceptions.py
--rw-rw-rw-   0        0        0    11422 2024-04-25 03:11:59.000000 pdfnaut-0.2.0/pdfnaut/filters.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.625120 pdfnaut-0.2.0/pdfnaut/objects/
--rw-rw-rw-   0        0        0      551 2024-03-29 21:44:31.000000 pdfnaut-0.2.0/pdfnaut/objects/__init__.py
--rw-rw-rw-   0        0        0     1632 2024-03-30 00:16:33.000000 pdfnaut-0.2.0/pdfnaut/objects/base.py
--rw-rw-rw-   0        0        0     1638 2024-03-30 00:18:21.000000 pdfnaut-0.2.0/pdfnaut/objects/stream.py
--rw-rw-rw-   0        0        0     1471 2024-03-30 00:48:56.000000 pdfnaut-0.2.0/pdfnaut/objects/xref.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.680202 pdfnaut-0.2.0/pdfnaut/parsers/
--rw-rw-rw-   0        0        0      105 2024-03-29 21:48:59.000000 pdfnaut-0.2.0/pdfnaut/parsers/__init__.py
--rw-rw-rw-   0        0        0    21582 2024-05-05 04:21:54.000000 pdfnaut-0.2.0/pdfnaut/parsers/pdf.py
--rw-rw-rw-   0        0        0    12503 2024-04-12 02:41:06.000000 pdfnaut-0.2.0/pdfnaut/parsers/simple.py
--rw-rw-rw-   0        0        0        0 2023-12-28 16:38:46.000000 pdfnaut-0.2.0/pdfnaut/py.typed
--rw-rw-rw-   0        0        0    13542 2024-05-05 04:00:09.000000 pdfnaut-0.2.0/pdfnaut/security_handler.py
--rw-rw-rw-   0        0        0     9684 2024-03-30 15:58:40.000000 pdfnaut-0.2.0/pdfnaut/serializer.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.794336 pdfnaut-0.2.0/pdfnaut.egg-info/
--rw-rw-rw-   0        0        0    14726 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1275 2024-05-05 02:30:26.000000 pdfnaut-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 16:54:09.803774 pdfnaut-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.784201 pdfnaut-0.2.0/tests/
--rw-rw-rw-   0        0        0     2864 2024-05-05 15:19:17.000000 pdfnaut-0.2.0/tests/test_encryption.py
--rw-rw-rw-   0        0        0      936 2024-05-05 16:43:43.000000 pdfnaut-0.2.0/tests/test_filters.py
--rw-rw-rw-   0        0        0     3726 2024-04-12 02:42:40.000000 pdfnaut-0.2.0/tests/test_object_parsing.py
--rw-rw-rw-   0        0        0     2673 2024-04-11 22:31:30.000000 pdfnaut-0.2.0/tests/test_parsing_files.py
--rw-rw-rw-   0        0        0     3719 2024-03-27 21:43:26.000000 pdfnaut-0.2.0/tests/test_serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.961742 pdfnaut-0.3.0/
+-rw-rw-rw-   0        0        0    10315 2024-01-02 18:49:05.000000 pdfnaut-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    15186 2024-05-26 22:42:08.958106 pdfnaut-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2273 2024-05-09 04:01:03.000000 pdfnaut-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1264 2024-05-08 03:10:17.000000 pdfnaut-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 22:42:08.961742 pdfnaut-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.725639 pdfnaut-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.787928 pdfnaut-0.3.0/src/pdfnaut/
+-rw-rw-rw-   0        0        0      400 2024-05-26 21:23:05.000000 pdfnaut-0.3.0/src/pdfnaut/__init__.py
+-rw-rw-rw-   0        0        0     6334 2024-05-25 17:03:32.000000 pdfnaut-0.3.0/src/pdfnaut/document.py
+-rw-rw-rw-   0        0        0      329 2024-04-23 00:33:36.000000 pdfnaut-0.3.0/src/pdfnaut/exceptions.py
+-rw-rw-rw-   0        0        0    11705 2024-05-08 02:17:46.000000 pdfnaut-0.3.0/src/pdfnaut/filters.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.889200 pdfnaut-0.3.0/src/pdfnaut/objects/
+-rw-rw-rw-   0        0        0      551 2024-03-29 21:44:31.000000 pdfnaut-0.3.0/src/pdfnaut/objects/__init__.py
+-rw-rw-rw-   0        0        0     1884 2024-05-22 23:49:01.000000 pdfnaut-0.3.0/src/pdfnaut/objects/base.py
+-rw-rw-rw-   0        0        0     1722 2024-05-08 02:28:18.000000 pdfnaut-0.3.0/src/pdfnaut/objects/stream.py
+-rw-rw-rw-   0        0        0     1471 2024-05-26 21:48:10.000000 pdfnaut-0.3.0/src/pdfnaut/objects/xref.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.906339 pdfnaut-0.3.0/src/pdfnaut/parsers/
+-rw-rw-rw-   0        0        0      105 2024-03-29 21:48:59.000000 pdfnaut-0.3.0/src/pdfnaut/parsers/__init__.py
+-rw-rw-rw-   0        0        0    24471 2024-05-26 00:25:57.000000 pdfnaut-0.3.0/src/pdfnaut/parsers/pdf.py
+-rw-rw-rw-   0        0        0    12529 2024-05-17 01:42:00.000000 pdfnaut-0.3.0/src/pdfnaut/parsers/simple.py
+-rw-rw-rw-   0        0        0        0 2023-12-28 16:38:46.000000 pdfnaut-0.3.0/src/pdfnaut/py.typed
+-rw-rw-rw-   0        0        0    13693 2024-05-08 02:48:29.000000 pdfnaut-0.3.0/src/pdfnaut/security_handler.py
+-rw-rw-rw-   0        0        0     9747 2024-05-10 17:51:53.000000 pdfnaut-0.3.0/src/pdfnaut/serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.924051 pdfnaut-0.3.0/src/pdfnaut/typings/
+-rw-rw-rw-   0        0        0    12346 2024-05-17 01:53:52.000000 pdfnaut-0.3.0/src/pdfnaut/typings/document.py
+-rw-rw-rw-   0        0        0     3281 2024-05-17 01:40:07.000000 pdfnaut-0.3.0/src/pdfnaut/typings/encryption.py
+-rw-rw-rw-   0        0        0     1173 2024-05-17 01:40:28.000000 pdfnaut-0.3.0/src/pdfnaut/typings/filters.py
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.952105 pdfnaut-0.3.0/src/pdfnaut.egg-info/
+-rw-rw-rw-   0        0        0    15186 2024-05-26 22:42:08.000000 pdfnaut-0.3.0/src/pdfnaut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      815 2024-05-26 22:42:08.000000 pdfnaut-0.3.0/src/pdfnaut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 22:42:08.000000 pdfnaut-0.3.0/src/pdfnaut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-05-26 22:42:08.000000 pdfnaut-0.3.0/src/pdfnaut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 22:42:08.000000 pdfnaut-0.3.0/src/pdfnaut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 22:42:08.944082 pdfnaut-0.3.0/tests/
+-rw-rw-rw-   0        0        0     2905 2024-05-23 00:34:20.000000 pdfnaut-0.3.0/tests/test_encryption.py
+-rw-rw-rw-   0        0        0      936 2024-05-05 16:43:43.000000 pdfnaut-0.3.0/tests/test_filters.py
+-rw-rw-rw-   0        0        0     3726 2024-04-12 02:42:40.000000 pdfnaut-0.3.0/tests/test_object_parsing.py
+-rw-rw-rw-   0        0        0     3276 2024-05-26 03:11:12.000000 pdfnaut-0.3.0/tests/test_parsing_files.py
+-rw-rw-rw-   0        0        0     3719 2024-03-27 21:43:26.000000 pdfnaut-0.3.0/tests/test_serializer.py
```

### Comparing `pdfnaut-0.2.0/LICENSE` & `pdfnaut-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.2.0/PKG-INFO` & `pdfnaut-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfnaut
-Version: 0.2.0
+Version: 0.3.0
 Summary: Explore PDFs with ease
 Author: Angel Carias
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -189,14 +189,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.11.0; python_version < "3.11"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
@@ -212,14 +213,30 @@
 > [!Warning]
 > pdfnaut is currently in an early stage of development and has only been tested with a small set of compliant documents. Expect bugs or issues.
 
 pdfnaut is a Python library for parsing PDF 1.7 files.
 
 pdfnaut provides a low-level interface for reading and writing PDF objects as defined in the [PDF 1.7 specification](https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf). pdfnaut currently does not attempt to deviate from the specification. There's no guarantee that valid documents not fully conforming to the standard will be processed correctly.
 
+## Examples
+
+The newer high-level API
+
+```py
+from pdfnaut import PdfDocument
+
+pdf = PdfDocument.from_filename("tests/docs/sample.pdf")
+first_page = list(pdf.flattened_pages)[0]
+if "Contents" in first_page:
+    first_page_stream = pdf.resolve_reference(first_page["Contents"])
+    print(first_page_stream.decompress())
+```
+
+The more mature low-level API
+
 ```py
 from pdfnaut import PdfParser
 
 with open("tests/docs/sample.pdf", "rb") as doc:
     pdf = PdfParser(doc.read())
     pdf.parse()
 
@@ -233,11 +250,11 @@
     print(first_page_stream.decompress())
 ```
 
 ## Coverage
 
 The following tracks coverage of certain portions of the PDF standard.
 
-- Compression filters: **Supported** (only FlateDecode, ASCII85Decode, and ASCIIHexDecode for now)
+- Compression filters: **Supported** -- FlateDecode, ASCII85, ASCIIHex, Crypt (decode only), and RunLength (decode only).
 - Reading from encrypted PDFs: **Supported** (ARC4 and AES; requires a user-supplied implementation or availability of a compatible module -- `pycryptodome` for now)
 - XRef streams: **Supported**
 - File specifications: **Not supported**
```

### Comparing `pdfnaut-0.2.0/README.md` & `pdfnaut-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,30 @@
 > [!Warning]
 > pdfnaut is currently in an early stage of development and has only been tested with a small set of compliant documents. Expect bugs or issues.
 
 pdfnaut is a Python library for parsing PDF 1.7 files.
 
 pdfnaut provides a low-level interface for reading and writing PDF objects as defined in the [PDF 1.7 specification](https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf). pdfnaut currently does not attempt to deviate from the specification. There's no guarantee that valid documents not fully conforming to the standard will be processed correctly.
 
+## Examples
+
+The newer high-level API
+
+```py
+from pdfnaut import PdfDocument
+
+pdf = PdfDocument.from_filename("tests/docs/sample.pdf")
+first_page = list(pdf.flattened_pages)[0]
+if "Contents" in first_page:
+    first_page_stream = pdf.resolve_reference(first_page["Contents"])
+    print(first_page_stream.decompress())
+```
+
+The more mature low-level API
+
 ```py
 from pdfnaut import PdfParser
 
 with open("tests/docs/sample.pdf", "rb") as doc:
     pdf = PdfParser(doc.read())
     pdf.parse()
 
@@ -29,11 +45,11 @@
     print(first_page_stream.decompress())
 ```
 
 ## Coverage
 
 The following tracks coverage of certain portions of the PDF standard.
 
-- Compression filters: **Supported** (only FlateDecode, ASCII85Decode, and ASCIIHexDecode for now)
+- Compression filters: **Supported** -- FlateDecode, ASCII85, ASCIIHex, Crypt (decode only), and RunLength (decode only).
 - Reading from encrypted PDFs: **Supported** (ARC4 and AES; requires a user-supplied implementation or availability of a compatible module -- `pycryptodome` for now)
 - XRef streams: **Supported**
 - File specifications: **Not supported**
```

### Comparing `pdfnaut-0.2.0/pdfnaut/filters.py` & `pdfnaut-0.3.0/src/pdfnaut/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 from __future__ import annotations
 
 import zlib
-from typing import Any, Protocol, cast
+from typing import Any, Mapping, Protocol
 from math import floor, ceil
 from base64 import b16decode, b16encode, a85decode, a85encode
 
+from .typings.filters import CryptFilterParams, LZWFlateParams
 from .parsers.simple import WHITESPACE
 from .exceptions import PdfFilterError
 from .objects.base import PdfName
 
 
 class PdfFilter(Protocol):
-    def decode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def decode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:
         ...
 
-    def encode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def encode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:
         ...
 
 
 class ASCIIHexFilter(PdfFilter):
     """Filter for hexadecimal strings (``§ 7.4.2 ASCIIHexDecode Filter``). EOD is ``>``.
     
     This filter does not take any parameters. ``params`` will be ignored.
     """
-    def decode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def decode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:
         if contents[-1:] != b">":
             raise PdfFilterError("ASCIIHex: EOD not at end of stream.")
 
         hexdata = bytearray(ch for ch in contents[:-1] if ch not in WHITESPACE)
         return b16decode(hexdata, casefold=True)
 
-    def encode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def encode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:
         return b16encode(contents) + b">"
 
 
 class ASCII85Filter(PdfFilter):
     """Filter for Adobe's ASCII85 implementation (``§ 7.4.3 ASCII85Decode Filter``).
     EOD is ``~>``.
     
     This filter does not take any parameters. ``params`` will be ignored.
     """
-    def decode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def decode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:
         return a85decode(contents, ignorechars=WHITESPACE, adobe=True)
 
-    def encode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def encode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:
         # the PDF spec does not need the starting delimiter
         return a85encode(contents, adobe=True)[2:]
 
 
 class RunLengthFilter(PdfFilter):
     """Filter for a form of Run-Length Encoding or RLE (``§ 7.4.5 RunLengthDecode Filter``)
     
@@ -58,15 +59,15 @@
         bytes shall be copied exactly.
     - If the length byte is in the range 129 to 255, the following byte shall be copied \
         ``257 - length`` bytes.
     - A length byte of 128 means EOD.
 
     This filter does not take any parameters. ``params`` will be ignored.
     """
-    def decode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:    
+    def decode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:    
         idx = 0
         output = bytes()
         
         while idx < len(contents):
             lenbyte = contents[idx]
             idx += 1
 
@@ -77,15 +78,15 @@
                 output += bytes(contents[idx] for _ in range(257 - lenbyte))
                 idx += 1
             elif lenbyte == 128:
                 break
         
         return output
     
-    def encode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def encode(self, contents: bytes, *, params: Mapping[str, Any] | None = None) -> bytes:
         raise NotImplementedError("RunLengthDecode: Encoding not implemented.")
 
 
 class FlateFilter(PdfFilter):
     """Filter for zlib/deflate compression (``§ 7.4.4 LZWDecode and FlateDecode Filters``).
     
     This filter supports predictors which can increase predictability of data and hence
@@ -100,15 +101,16 @@
     - **Columns**: Amount of samples per row. Any value greater than 1 (default=1).
 
     Given these values, the length of a sample in bytes is obtained by 
         ``Length(Sample) = ceil((Colors * BitsPerComponent) / 8)`` 
     and the length of a row is obtained by 
         ``Length(Row) = Length(Sample) * Columns``
     """
-    def decode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+
+    def decode(self, contents: bytes, *, params: LZWFlateParams | None = None) -> bytes: # pyright: ignore[reportIncompatibleMethodOverride]
         if params is None:
             params = {}
 
         uncomp = zlib.decompress(contents, 0)
 
         # No predictor applied, return uncompressed.
         if (predictor := params.get("Predictor", 1)) == 1:
@@ -121,15 +123,15 @@
         if predictor == 2:
             raise PdfFilterError("FlateDecode: TIFF Predictor 2 not supported.")
         elif 10 <= predictor <= 15:
             return bytes(self._undo_png_prediction(bytearray(uncomp), cols, colors, bpc))
         else:
             raise PdfFilterError(f"FlateDecode: Predictor {predictor} not supported.")
 
-    def encode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def encode(self, contents: bytes, *, params: LZWFlateParams | None = None) -> bytes: # pyright: ignore[reportIncompatibleMethodOverride]
         if params is None:
             params = {}
         
         if (predictor := params.get("Predictor", 1)) == 1:
             return zlib.compress(contents)
 
         cols = params.get("Columns", 1)
@@ -235,35 +237,33 @@
     This filter takes two optional parameters: ``Type``, which defines the decode parameters
     as being for this filter; and ``Name``, which defines what filter should be used to 
     decrypt the stream.
 
     This filter requires 3 additional parameters. These parameters are for use exclusively
     within the PDF processor and shall not be written to the document.
     
-    - **Handler**: An instance of the security handler.
-    - **EncryptionKey**: The encryption key generated from the security handler.
-    - **IndirectRef**: The indirect reference of the object to decrypt.
+    - **_Handler**: An instance of the security handler.
+    - **_EncryptionKey**: The encryption key generated from the security handler.
+    - **_IndirectRef**: The indirect reference of the object to decrypt.
     """
-    def encode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def encode(self, contents: bytes, *, params: CryptFilterParams | None = None) -> bytes: # pyright: ignore[reportIncompatibleMethodOverride]
         raise NotImplementedError("Crypt: Encrypting streams not implemented.")
 
-    def decode(self, contents: bytes, *, params: dict[str, Any] | None = None) -> bytes:
+    def decode(self, contents: bytes, *, params: CryptFilterParams | None = None) -> bytes: # pyright: ignore[reportIncompatibleMethodOverride]
         if params is None:
-            params = {}
+            raise ValueError("Crypt: This filter requires parameters.")
         
-        cf_name = cast("PdfName | None", params.get("Name"))
-        if cf_name is None or cf_name.value == b"Identity":
+        cf_name = params.get("Name", PdfName(b"Identity"))
+        if cf_name.value == b"Identity":
             return contents
+        
+        crypt_filter = params["_Handler"].encryption.get("CF", {}).get(cf_name.value.decode())
 
-        crypt_filter = params["Handler"].encryption.get("CF", {}).get(
-            cf_name.value.decode(), params["Handler"].encryption.get("StmF")
-        )
-
-        return params["Handler"].decrypt_object(params["EncryptionKey"],
-            contents, params["IndirectRef"], crypt_filter=crypt_filter)
+        return params["_Handler"].decrypt_object(params["_EncryptionKey"],
+            contents, params["_IndirectRef"], crypt_filter=crypt_filter)
 
 
 SUPPORTED_FILTERS: dict[bytes, type[PdfFilter]] = {
     b"FlateDecode": FlateFilter,
     b"ASCII85Decode": ASCII85Filter,
     b"ASCIIHexDecode": ASCIIHexFilter,
     b"RunLengthDecode": RunLengthFilter,
```

### Comparing `pdfnaut-0.2.0/pdfnaut/objects/__init__.py` & `pdfnaut-0.3.0/src/pdfnaut/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.2.0/pdfnaut/objects/base.py` & `pdfnaut-0.3.0/src/pdfnaut/objects/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from binascii import unhexlify, hexlify
-from typing import Union, List, Dict, Any
+from typing import Mapping, Union, List, TypeVar, Generic, TYPE_CHECKING, Any
 
 
 class PdfNull:
     """A PDF null object (``§ 7.3.9 Null Object``)."""
     pass
 
+
 @dataclass
 class PdfComment:
     """A PDF comment (``§ 7.2.3 Comments``). Comments have no syntactical meaning and shall 
     be interpreted as whitespace."""
     value: bytes
 
 
+if TYPE_CHECKING:
+    from typing_extensions import TypeVar
+
+    T = TypeVar("T", default=bytes)
+else:
+    T = TypeVar("T") # pytest complains if this is not here
+
+
 @dataclass
-class PdfName:
+class PdfName(Generic[T]):
     """A PDF name object (``§ 7.3.5 Name Objects``)."""
-    value: bytes
+    value: T
 
 
 @dataclass
 class PdfHexString:
     """A PDF hexadecimal string which can be used to include arbitrary binary data in a PDF
     (``§ 7.3.4.3 Hexadecimal Strings``)."""
     
@@ -42,26 +51,27 @@
 
     @property
     def value(self) -> bytes:
         """The decoded value of the hex string"""
         return unhexlify(self.raw)
 
 
+T = TypeVar("T")
 @dataclass
-class PdfIndirectRef:
+class PdfIndirectRef(Generic[T]):
     """A reference to a PDF indirect object."""
     object_number: int
     generation: int
 
 
 @dataclass
 class PdfOperator:
     """A PDF operator within a content stream."""
     value: bytes
 
 
 PdfObject = Union[
     bool, int, float, bytes, 
-    List[Any], Dict[str, Any], 
+    List[Any], Mapping[str, Any], 
     PdfHexString, PdfName, 
     PdfIndirectRef, PdfNull
 ]
```

### Comparing `pdfnaut-0.2.0/pdfnaut/objects/stream.py` & `pdfnaut-0.3.0/src/pdfnaut/objects/stream.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 from typing import Any
 from dataclasses import dataclass, field
 
+
 from .base import PdfName, PdfNull
 from ..filters import SUPPORTED_FILTERS
 from ..exceptions import PdfFilterError
 
 
 @dataclass
 class PdfStream:
     """A stream object in a PDF"""
+    # we don't yet use a type here given details can have a lot of other things
     details: dict[str, Any]
     raw: bytes = field(repr=False)
     _sec_handler: dict[str, Any] = field(default_factory=dict, repr=False)
 
     def decompress(self) -> bytes:
         """Returns the contents of the stream decompressed.
         
@@ -39,13 +41,13 @@
         for filt, params in zip(filters, params):
             if filt.value not in SUPPORTED_FILTERS:
                 raise PdfFilterError(f"{filt.value.decode()}: Filter is unsupported.")
             
             if isinstance(params, PdfNull) or params is None:
                 params = {}
             
-            if filt.value == b"Crypt" and self._sec_handler.get("Handler"):
+            if filt.value == b"Crypt" and self._sec_handler.get("_Handler"):
                 params.update(self._sec_handler)
             
             output = SUPPORTED_FILTERS[filt.value]().decode(self.raw, params=params)
 
         return output
```

### Comparing `pdfnaut-0.2.0/pdfnaut/objects/xref.py` & `pdfnaut-0.3.0/src/pdfnaut/objects/xref.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.2.0/pdfnaut/parsers/pdf.py` & `pdfnaut-0.3.0/src/pdfnaut/parsers/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import re
-from typing import Any, cast, TypeVar
+from typing import Any, cast, TypeVar, overload
 from enum import IntEnum
 from io import BytesIO
 
 from ..objects.base import PdfNull, PdfIndirectRef, PdfObject, PdfName, PdfHexString
 from ..objects.stream import PdfStream
-from ..objects.xref import (
-    PdfXRefEntry, PdfXRefSubsection, PdfXRefTable, 
-    FreeXRefEntry, InUseXRefEntry, CompressedXRefEntry
-)
+from ..objects.xref import (PdfXRefEntry, PdfXRefSubsection, PdfXRefTable, 
+                            FreeXRefEntry, InUseXRefEntry, CompressedXRefEntry)
 from ..exceptions import PdfParseError
 from ..security_handler import StandardSecurityHandler
 from .simple import PdfTokenizer
+from ..typings.document import Trailer, XRefStream
+from ..typings.encryption import StandardEncrypt
 
 
 class PermsAcquired(IntEnum):
     NONE = 0
     """No permissions acquired, document is still encrypted."""
     USER = 1
     """User permissions within the limits specified by the security handler"""
@@ -26,24 +26,36 @@
 
 
 class PdfParser:
     """A parser that can completely parse a PDF document.
     
     It consumes the PDF's cross-reference tables and trailers. It merges the tables
     into a single one and provides an interface to individually parse each indirect 
-    object using :class:`~pdfnaut.parsers.simple.PdfTokenizer`."""
+    object using :class:`~pdfnaut.parsers.simple.PdfTokenizer`.
+    
+    Arguments:
+        data (bytes):
+            The document to be processed.
+
+    Keyword Arguments:
+        strict (bool, optional):
+            Whether to warn or fail at issues caused by non-spec-compliance.
+            Defaults to False.
+    """
 
-    def __init__(self, data: bytes) -> None:
+    def __init__(self, data: bytes, *, strict: bool = False) -> None:
+        self.strict = strict
         self._tokenizer = PdfTokenizer(data)
 
-        self.updates: list[tuple[PdfXRefTable, dict[str, Any]]] = []
+        self.updates: list[tuple[PdfXRefTable, Trailer | XRefStream]] = []
         """A list of all incremental updates present in the document. The items are two-element 
         tuples: first, the XRef table; second, the trailer. (most recent/last update first)"""
 
-        self.trailer: dict[str, Any] = {}
+        # placeholder to make the type checker happy
+        self.trailer: Trailer | XRefStream = { "Size": 0, "Root": PdfIndirectRef(0, 0) }
         """The most recent trailer in the PDF document.
         
         For details on the contents of the trailer, see ``§ 7.5.5 File Trailer`` in the PDF spec.
         """
 
         self.xref: dict[tuple[int, int], PdfXRefEntry] = {}
         """A cross-reference mapping combining the entries of all XRef tables present 
@@ -66,14 +78,21 @@
 
         This field being set indicates that a supported security handler was used for
         encryption. If not set, the parser will not attempt to decrypt this document.
         """
 
         self._encryption_key = None
 
+    T = TypeVar("T")
+    def _ensure_resolved(self, obj: PdfIndirectRef[T] | T) -> T:
+        return self.resolve_reference(obj) if isinstance(obj, PdfIndirectRef) else obj
+
+    def _get_closest(self, values: list[int], target: int) -> int:
+        return min(values, key=lambda offset: abs(offset - target))
+
     def parse(self, start_xref: int | None = None) -> None:
         """Parses the entire document.
         
         It begins by parsing the most recent XRef table and trailer. If this trailer 
         points to a previous XRef, this function is called again with a ``start_xref``
         offset until no more XRefs are found.
 
@@ -102,19 +121,20 @@
         else:
             # That's it. Merge them together.
             self.xref = self.get_merged_xrefs()
             self.trailer = self.updates[0][1]
 
         # Is the document encrypted with a standard security handler?
         if "Encrypt" in self.trailer:
-            encryption = cast("dict[str, Any]", 
-                self.resolve_reference(_E) if isinstance((_E := self.trailer["Encrypt"]), PdfIndirectRef) else _E)
-            
+            assert "ID" in self.trailer
+            encryption = self._ensure_resolved(self.trailer["Encrypt"])
+
             if encryption["Filter"].value == b"Standard":
-                self.security_handler = StandardSecurityHandler(encryption, self.trailer["ID"])
+                self.security_handler = StandardSecurityHandler(
+                    cast(StandardEncrypt, encryption), self.trailer["ID"])
 
     def parse_header(self) -> str:
         """Parses the %PDF-n.m header that is expected to be at the start of a PDF file."""
         header = self._tokenizer.parse_comment()
         mat = re.match(rb"PDF-(?P<major>\d+).(?P<minor>\d+)", header.value)
         if mat:
             return f"{mat.group('major').decode()}.{mat.group('minor').decode()}"
@@ -168,41 +188,72 @@
         
         # advance to the startxref offset, we know it's there.
         self._tokenizer.advance(9)
         self._tokenizer.advance_whitespace()
 
         return int(self._tokenizer.parse_numeric()) # startxref
 
-    def parse_xref_and_trailer(self) -> tuple[PdfXRefTable, dict[str, Any]]:
+    def parse_xref_and_trailer(self) -> tuple[PdfXRefTable, Trailer | XRefStream]:
         """Parses both the cross-reference table and the PDF trailer.
         
         PDFs may include a typical uncompressed XRef table (and hence separate XRefs and
         trailers) or an XRef stream that combines both.
         """
         if self._tokenizer.current + self._tokenizer.peek(3) == b"xref":
             xref = self.parse_simple_xref()
             self._tokenizer.advance_whitespace()
             trailer = self.parse_simple_trailer()
             return xref, trailer
         elif re.match(rb"(?P<num>\d+)\s+(?P<gen>\d+)\s+obj", self._tokenizer.current_to_eol):
             return self.parse_compressed_xref()
+        elif not self.strict:
+            # let's attempt to locate a nearby xref table
+            target = self._tokenizer.position
+            table_offsets = self._find_xref_offsets()
+
+            # get the xref table nearest to our offset
+            self._tokenizer.position = self._get_closest(table_offsets, target)
+            xref, trailer = self.parse_xref_and_trailer()
+            # make sure the user can see our corrections
+            if "Prev" in trailer:
+                trailer["Prev"] = self._get_closest(table_offsets, trailer["Prev"])
+            return xref, trailer
         else:
             raise PdfParseError("XRef offset does not point to XRef table.")
+
+    def _find_xref_offsets(self) -> list[int]:
+        table_offsets = []
+        # looks for the start of a xref table
+        for mat in re.finditer(rb"(?<!start)xref(\W*)(\d+) (\d+)", self._tokenizer.data):
+            table_offsets.append(mat.start())
+
+        # looks for indirect objects, then checks if they are xref streams
+        for mat in re.finditer(rb"(?P<num>\d+)\s+(?P<gen>\d+)\s+obj", self._tokenizer.data):
+            self._tokenizer.position = mat.start()
+            self._tokenizer.advance(mat.end() - mat.start())
+            self._tokenizer.advance_whitespace()
+            
+            if self._tokenizer.current + self._tokenizer.peek() == b"<<":
+                mapping = self._tokenizer.parse_dictionary()
+                if isinstance(typ := mapping.get("Type"), PdfName) and typ.value == b"XRef":
+                    table_offsets.append(mat.start())
+        
+        return sorted(table_offsets)
         
-    def parse_simple_trailer(self) -> dict[str, Any]:
+    def parse_simple_trailer(self) -> Trailer:
         """Parses the PDF's standard trailer which is used to quickly locate other 
         cross reference tables and special objects.
         
         The trailer is separate if the XRef table is standard (uncompressed).
         Otherwise it is part of the XRef object."""
         self._tokenizer.advance(7) # past the 'trailer' keyword
         self._tokenizer.advance_whitespace()
         
         # next token is a dictionary
-        trailer = self._tokenizer.parse_dictionary()
+        trailer = cast(Trailer, self._tokenizer.parse_dictionary()) 
         return trailer
 
     def parse_simple_xref(self) -> PdfXRefTable:
         """Parses a standard, uncompressed XRef table of the format described in 
         ``§ 7.5.4 Cross-Reference Table`` in the PDF spec.
 
         If ``startxref`` points to an XRef object, :meth:`.parse_compressed_xref`
@@ -234,25 +285,28 @@
                 generation = int(entry.group("gen"))
 
                 if entry.group("status") == b"n":
                     entries.append(InUseXRefEntry(offset, generation))
                 else:
                     entries.append(FreeXRefEntry(offset, generation))
 
-                self._tokenizer.advance(20)
+                # some files do not respect the 20-byte length req. for entries
+                # hence this is here for tolerance
+                self._tokenizer.advance(entry.end())
+                self._tokenizer.advance_whitespace()
             
             table.sections.append(PdfXRefSubsection(
                 int(subsection.group("first_obj")),
                 int(subsection.group("count")),
                 entries
             ))
             
         return table
 
-    def parse_compressed_xref(self) -> tuple[PdfXRefTable, dict[str, Any]]:
+    def parse_compressed_xref(self) -> tuple[PdfXRefTable, XRefStream]:
         """Parses a compressed cross-reference stream which includes both the XRef table 
         and information from the PDF trailer. 
         
         Described in ``§ 7.5.4 Cross-Reference Streams``."""
         xref_stream = self.parse_indirect_object(
             InUseXRefEntry(self._tokenizer.position, 0))
         assert isinstance(xref_stream, PdfStream)
@@ -281,26 +335,25 @@
                     section.entries.append(InUseXRefEntry(offset=second, generation=third))
                 elif field_type == 2:
                     section.entries.append(CompressedXRefEntry(objstm_number=second, 
                                                                index_within=third))
 
             table.sections.append(section)
 
-        return table, xref_stream.details
+        return table, cast(XRefStream, xref_stream.details)
 
     def parse_indirect_object(self, xref_entry: InUseXRefEntry) -> PdfObject | PdfStream:
         """Parses an indirect object not within an object stream, or basically, an object 
         that is directly referred to by an ``xref_entry``"""
         self._tokenizer.position = xref_entry.offset
         self._tokenizer.advance_whitespace()
         mat = re.match(rb"(?P<num>\d+)\s+(?P<gen>\d+)\s+obj", 
                        self._tokenizer.current_to_eol)
         if not mat:
             raise PdfParseError("XRef entry does not point to indirect object.")
-        
         self._tokenizer.advance(mat.end())
         self._tokenizer.advance_whitespace()
 
         tok = self._tokenizer.next_token()
         self._tokenizer.advance_whitespace()
 
         try:
@@ -344,17 +397,17 @@
                     use_stmf = False
                 elif isinstance(filter_, list):
                     use_stmf = not any(isinstance(filt, PdfName) and filt.value == b"Crypt" 
                                         for filt in filter_)
             
             # Give the stream an instance of the security handler
             pdf_object._sec_handler = {
-                "Handler": self.security_handler,
-                "EncryptionKey": self._encryption_key,
-                "IndirectRef": reference
+                "_Handler": self.security_handler,
+                "_EncryptionKey": self._encryption_key,
+                "_IndirectRef": reference
             }
 
             if use_stmf:
                 pdf_object.raw = self.security_handler.decrypt_object(
                     self._encryption_key, pdf_object, reference)
 
             return pdf_object
@@ -369,15 +422,15 @@
                 self._encryption_key, pdf_object, reference
             )
         elif isinstance(pdf_object, list):
             return [self._get_decrypted(obj, reference) for obj in pdf_object]
         elif isinstance(pdf_object, dict):
             # make a special exception if the dictionary is the Encrypt key in the trailer
             # we do not need to decrypt them
-            if reference == self.trailer["Encrypt"]:
+            if reference == self.trailer.get("Encrypt", {}):
                 return pdf_object
             return {name: self._get_decrypted(value, reference) for name, value in pdf_object.items()}         
 
         # Why would a number be encrypted?
         return pdf_object
 
     def parse_stream(self, xref_entry: InUseXRefEntry, extent: int) -> bytes:
@@ -420,15 +473,24 @@
         self._tokenizer.advance_whitespace()
         # Have we not reached the end?
         if not self._tokenizer.advance_if_next(b"endstream"):
             raise PdfParseError("\\Length key in stream extent does not match end of stream.")
         
         return contents
 
-    def resolve_reference(self, reference: PdfIndirectRef | tuple[int, int]) -> PdfObject | PdfStream | PdfNull:
+    T = TypeVar("T")
+    @overload
+    def resolve_reference(self, reference: PdfIndirectRef[T]) -> T:
+        ...
+    
+    @overload
+    def resolve_reference(self, reference: tuple[int, int]) -> PdfObject | PdfStream | PdfNull:
+        ...
+    
+    def resolve_reference(self, reference: PdfIndirectRef | tuple[int, int]) -> PdfObject | PdfStream | PdfNull | Any:
         """Resolves a reference into the indirect object it points to.
         
         Arguments:
             reference (:class:`.PdfIndirectRef` | tuple[int, int]): 
                 An indirect reference object or a tuple of two integers representing, 
                 in order, the object number and the generation number.
```

### Comparing `pdfnaut-0.2.0/pdfnaut/parsers/simple.py` & `pdfnaut-0.3.0/src/pdfnaut/parsers/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,18 +127,18 @@
         while not self.at_end():
             if self.advance_if_next(b"true"):
                 return True
             elif self.advance_if_next(b"false"):
                 return False
             elif self.advance_if_next(b"null"):
                 return PdfNull()
-            elif (mat := re.match(rb"(?P<num>\d+)\s+(?P<gen>\d+)\s+R", self.current_to_eol)):
+            elif self.current.isdigit() and (mat := re.match(rb"(?P<num>\d+)\s+(?P<gen>\d+)\s+R", self.current_to_eol)):
                 return self.parse_indirect_reference(mat)
             elif self.current.isdigit() or self.current in b"+-":
-                return self.parse_numeric() 
+                return self.parse_numeric()
             elif self.current == b"[":
                 return self.parse_array()
             elif self.current == b"/":
                 return self.parse_name()
             elif self.current + self.peek() == b"<<":
                 return self.parse_dictionary()
             elif self.current == b"<":
```

### Comparing `pdfnaut-0.2.0/pdfnaut/security_handler.py` & `pdfnaut-0.3.0/src/pdfnaut/security_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from hashlib import md5
-from typing import Any, Union, Protocol, Literal, cast
+from typing import Union, Protocol, Literal
 
+from .typings.encryption import EncrCryptFilter, StandardEncrypt
 from .objects import PdfHexString, PdfIndirectRef, PdfName, PdfStream
 
 
 class CryptProvider(Protocol):
     key: bytes
 
     def __init__(self, key: bytes) -> None:
@@ -43,46 +44,50 @@
             # last byte of decrypted indicates amount of trailing padding
             return decrypted[:-decrypted[-1]]
         
         def encrypt(self, contents: bytes) -> bytes:
             padded = Padding.pad(contents, 16, style="pkcs7")
 
             encryptor = AES.new(self.key, AES.MODE_CBC)
-            return encryptor.iv + encryptor.encrypt(padded)
-        
+            return bytes(encryptor.iv) + encryptor.encrypt(padded)
+    
+
     CRYPT_PROVIDERS = { "ARC4": _DomeARC4Provider, "AESV2": _DomeAES128Provider, 
                         "Identity": _IdentityProvider }
 except ImportError:
     CRYPT_PROVIDERS = { "ARC4": None, "AESV2": None, "Identity": _IdentityProvider }
 
 
 PASSWORD_PADDING = b'(\xbfN^Nu\x8aAd\x00NV\xff\xfa\x01\x08..\x00\xb6\xd0h>\x80/\x0c\xa9\xfedSiz'
 
 def pad_password(password: bytes) -> bytes:
     return password[:32] + PASSWORD_PADDING[:32 - len(password)]
 
+def get_value_from_bytes(contents: PdfHexString | bytes) -> bytes:
+    return contents.value if isinstance(contents, PdfHexString) else contents
+
 
 class StandardSecurityHandler:
-    def __init__(self, encryption: dict[str, Any], ids: list[PdfHexString]) -> None:
+    def __init__(self, encryption: StandardEncrypt, ids: list[PdfHexString | bytes]) -> None:
         self.encryption = encryption
         self.ids = ids
 
     @property
     def key_length(self) -> int:
         return self.encryption.get("Length", 40) // 8
 
     def compute_encryption_key(self, password: bytes) -> bytes:  
         """Computes an encryption key as defined in ``§ 7.6.3.3 Encryption Key Algorithm > 
         Algorithm 2: Computing an encryption key`` in the PDF spec."""      
         padded_password = pad_password(password)
 
         psw_hash = md5(padded_password)
-        psw_hash.update(_O.value if isinstance(_O := self.encryption["O"], PdfHexString) else _O)
+        psw_hash.update(get_value_from_bytes(self.encryption["O"]))
         psw_hash.update(self.encryption["P"].to_bytes(4, "little", signed=True))
-        psw_hash.update(self.ids[0].value)
+        psw_hash.update(get_value_from_bytes(self.ids[0]))
 
         if self.encryption.get("V", 0) >= 4 and not self.encryption.get("EncryptMetadata", True):
             psw_hash.update(b"\xff\xff\xff\xff")
 
         if self.encryption["R"] >= 3:
             for _ in range(50):
                 psw_hash = md5(psw_hash.digest()[:self.key_length])
@@ -117,15 +122,15 @@
 
         encr_key = self.compute_encryption_key(password)
         arc4 = self._get_provider("ARC4")
         if self.encryption["R"] == 2:
             padding_crypt = arc4(encr_key).encrypt(PASSWORD_PADDING)
             return padding_crypt
         else: # rev 3
-            padded_id_hash = md5(PASSWORD_PADDING + self.ids[0].value)
+            padded_id_hash = md5(PASSWORD_PADDING + get_value_from_bytes(self.ids[0]))
             user_cipher = arc4(encr_key).encrypt(padded_id_hash.digest())
 
             for i in range(1, 20):
                 user_cipher = arc4(bytearray(b ^ i for b in encr_key)).encrypt(user_cipher)
 
             return pad_password(user_cipher)
          
@@ -133,64 +138,65 @@
         """Authenticates the provided user ``password`` according to Algorithm 4, 5, and 6 in 
         ``§ 7.6.3.4 Password Algorithms`` of the PDF spec.
         
         Returns:
             If the password was correct, a tuple of two values: the encryption key that should 
             decrypt the document and True. Otherwise, ``(b"", False)`` is returned."""
         encryption_key = self.compute_encryption_key(password)
-        stored_password = _U.value if isinstance(_U := self.encryption["U"], PdfHexString) else _U
+        stored_password = get_value_from_bytes(self.encryption["U"])
         
         make_provider = self._get_provider("ARC4")
 
         # Algorithm 4
         if self.encryption["R"] == 2:
             user_cipher = make_provider(encryption_key).encrypt(PASSWORD_PADDING)
         
             return (encryption_key, True) if stored_password == user_cipher else (b"", False)
         # Algorithm 5
         else:
-            padded_id_hash = md5(PASSWORD_PADDING + self.ids[0].value)
+            padded_id_hash = md5(PASSWORD_PADDING + get_value_from_bytes(self.ids[0]))
             user_cipher = make_provider(encryption_key).encrypt(padded_id_hash.digest())
 
             for i in range(1, 20):
                 user_cipher = make_provider(bytearray(b ^ i for b in encryption_key)).encrypt(user_cipher)
 
             return (encryption_key, True) if stored_password[:16] == user_cipher[:16] else (b"", False)
 
     def authenticate_owner_password(self, password: bytes) -> tuple[bytes, bool]:
         """Authenticates the provided owner ``password`` (or user password if none) 
         according to Algorithms 3 and 7 in ``§ 7.6.3.4 Password Algorithms`` of the PDF spec.
         
         Returns:
             If the password was correct, a tuple of two values: the encryption key that should 
-            decrypt the document and True. Otherwise, ``(b"", False)`` is returned."""
+            decrypt the document and True. Otherwise, ``(b"", False)`` is returned.
+        """
         # (a) to (d) in Algorithm 3
         padded_password = pad_password(password)
         digest = md5(padded_password).digest()
         if self.encryption["R"] >= 3:
             for _ in range(50):
                 digest = md5(digest).digest()
 
         cipher_key = digest[:self.key_length]
-        user_cipher = _O.value if isinstance(_O := self.encryption["O"], PdfHexString) else _O
-
+        user_cipher = get_value_from_bytes(self.encryption["O"])
+        
         make_provider = self._get_provider("ARC4")
         # Algorithm 7
         if self.encryption["R"] == 2:
             user_cipher = make_provider(user_cipher).decrypt(user_cipher)
         else:
             for i in range(19, -1, -1):
                 user_cipher = make_provider(bytearray(b ^ i for b in cipher_key)).encrypt(user_cipher)
 
         return self.authenticate_user_password(user_cipher)
 
     _Encryptable = Union[PdfStream, PdfHexString, bytes]
     def compute_object_crypt(self, encryption_key: bytes, contents: _Encryptable, 
                              reference: PdfIndirectRef, *, 
-                             crypt_filter: dict[str, Any] | None = None) -> tuple[CryptMethod, bytes, bytes]:
+                             crypt_filter: EncrCryptFilter | None = None) -> tuple[CryptMethod, bytes, bytes]:
         """Computes all needed parameters to encrypt or decrypt ``contents`` according to 
         Algorithm 1 in ``§ 7.6.2 General Encryption Algorithm``
         
         Arguments:
             encryption_key (bytes):
                 An encryption key generated by :meth:`.compute_encryption_key`
 
@@ -231,29 +237,29 @@
         else:
             raise TypeError("contents arg not a stream or string object")
 
         return (method, crypt_key, data)
 
     def encrypt_object(self, encryption_key: bytes, contents: _Encryptable, 
                        reference: PdfIndirectRef, *, 
-                       crypt_filter: dict[str, Any] | None = None) -> bytes:
+                       crypt_filter: EncrCryptFilter | None = None) -> bytes:
         """Encrypts the specified ``contents`` according to Algorithm 1 in 
         ``§ 7.6.2 General Encryption Algorithm``.
         
         For details on arguments, please see :meth:`.compute_object_crypt`"""
         
         crypt_method, key, decrypted = self.compute_object_crypt(encryption_key, 
                                                                  contents, reference, 
                                                                  crypt_filter=crypt_filter)
 
         return self._get_provider(crypt_method)(key).encrypt(decrypted)
 
     def decrypt_object(self, encryption_key: bytes, contents: _Encryptable, 
                        reference: PdfIndirectRef, *, 
-                       crypt_filter: dict[str, Any] | None = None) -> bytes:
+                       crypt_filter: EncrCryptFilter | None = None) -> bytes:
         """Decrypts the specified ``contents`` according to Algorithm 1 in 
         ``§ 7.6.2 General Encryption Algorithm``.
         
         For details on arguments, please see :meth:`.compute_object_crypt`"""
         
         crypt_method, key, encrypted = self.compute_object_crypt(encryption_key, 
                                                                  contents, reference,
@@ -265,35 +271,35 @@
         provider = CRYPT_PROVIDERS.get(name)
         if provider is None:
             raise NotImplementedError(f"Missing crypt provider for {name}. Register in CRYPT_PROVIDERS or install a compatible module.")
         return provider
 
     CryptMethod = Literal["Identity", "ARC4", "AESV2"]
     def _get_crypt_method(self, contents: _Encryptable) -> CryptMethod:
-        if self.encryption["V"] != 4:
+        if self.encryption.get("V", 0) != 4:
             # ARC4 is assumed given that can only be specified if V = 4. It is definitely
             # not Identity because the document wouldn't be encrypted in that case.
             return "ARC4"            
 
         if isinstance(contents, PdfStream):
-            cf_name = cast(PdfName, self.encryption.get("StmF", PdfName(b"Identity")))
+            cf_name = self.encryption.get("StmF", PdfName(b"Identity"))
         elif isinstance(contents, (bytes, PdfHexString)):
-            cf_name = cast(PdfName, self.encryption.get("StrF", PdfName(b"Identity")))
+            cf_name = self.encryption.get("StrF", PdfName(b"Identity"))
         else:
             raise TypeError("contents arg not a stream or string object")
 
         if cf_name.value == b"Identity":
             return "Identity" # No processing needed
         
-        crypt_filters = cast("dict[str, Any]", self.encryption.get("CF", {}))
+        crypt_filters = self.encryption.get("CF", {})
         crypter = crypt_filters.get(cf_name.value.decode(), {})
         
         return self._get_cfm_method(crypter)
 
-    def _get_cfm_method(self, crypt_filter: dict[str, Any]) -> CryptMethod:
+    def _get_cfm_method(self, crypt_filter: EncrCryptFilter) -> CryptMethod:
         cf_name = crypt_filter.get("CFM", PdfName(b"Identity"))
         if cf_name.value == b"Identity":
             return "Identity"
         elif cf_name.value == b"AESV2":
             return "AESV2"
         elif cf_name.value == b"V2":
             return "ARC4"
```

### Comparing `pdfnaut-0.2.0/pdfnaut/serializer.py` & `pdfnaut-0.3.0/src/pdfnaut/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-from typing import Literal, Any
+from typing import Any, Literal, Mapping
 from collections import defaultdict
 
+from .typings.document import Trailer
 from .objects.stream import PdfStream
 from .objects.xref import PdfXRefSubsection, PdfXRefTable, FreeXRefEntry, InUseXRefEntry
 from .objects.base import (PdfComment, PdfIndirectRef, PdfObject, PdfNull, PdfName,
                            PdfHexString)
 from .parsers.simple import STRING_ESCAPE
 from .exceptions import PdfWriteError
 
@@ -53,15 +54,15 @@
     unbalanced.extend(paren_stack)
     for pos in unbalanced:
         output.insert(pos, ord("\\"))
 
     return b"(" + output + b")"
 
 
-def serialize_name(name: PdfName) -> bytes:
+def serialize_name(name: PdfName[bytes]) -> bytes:
     output = b"/"
 
     for char in name.value:
         char = char.to_bytes(1)
         if char.isalnum():
             output += char
         else:
@@ -82,15 +83,15 @@
     return str(number).encode()
 
 
 def serialize_array(array: list[Any]) -> bytes:
     return b"[" + b" ".join(serialize(item) for item in array) + b"]"
 
 
-def serialize_dictionary(mapping: dict[str, Any]) -> bytes:
+def serialize_dictionary(mapping: Mapping[str, Any]) -> bytes:
     items = []
     for k, v in mapping.items():
         items.append(serialize(PdfName(k.encode())))
         items.append(serialize(v))
 
     return b"<<" + b" ".join(items) + b">>"
 
@@ -168,15 +169,15 @@
             self.content += serialize_comment(marker) + self.eol
 
     def write_object(self, reference: PdfIndirectRef | tuple[int, int],
                      contents: PdfObject | PdfStream) -> int:
         """Writes an indirect object to the stream.
 
         Arguments:
-            reference (:class:`PdfIndirectRef` | tuple[int, int]):
+            reference (:class:`PdfIndirectRef` | :class:`tuple[int, int]`):
                 The object number and generation to which the object should be assigned.
 
             contents (:class:`PdfObject` | :class:`PdfStream`):
                 The contents to associate with the reference.
 
         Returns:
             The offset where the indirect object starts.
@@ -250,17 +251,17 @@
                     self.content += f"{entry.next_free_object:0>10} {entry.gen_if_used_again:0>5} f".encode()
                 else:
                     raise PdfWriteError("Cannot write compressed XRef entry within standard table")
                 self.content += self.eol
 
         return startxref
 
-    def write_trailer(self, details: dict[str, Any], startxref: int) -> None:
-        """Writes the trailer of the PDF (``details``) and the ``startxref`` offset."""
+    def write_trailer(self, trailer: Trailer, startxref: int) -> None:
+        """Writes a standard ``trailer`` to the PDF alongisde the ``startxref`` offset."""
         self.content += b"trailer" + self.eol
-        self.content += serialize_dictionary(details) + self.eol
+        self.content += serialize_dictionary(trailer) + self.eol
         self.content += b"startxref" + self.eol
         self.content += str(startxref).encode() + self.eol
 
     def write_eof(self) -> None:
         """Writes the End-Of-File marker."""
         self.content += b"%%EOF" + self.eol
```

### Comparing `pdfnaut-0.2.0/pdfnaut.egg-info/PKG-INFO` & `pdfnaut-0.3.0/src/pdfnaut.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfnaut
-Version: 0.2.0
+Version: 0.3.0
 Summary: Explore PDFs with ease
 Author: Angel Carias
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -189,14 +189,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.11.0; python_version < "3.11"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
@@ -212,14 +213,30 @@
 > [!Warning]
 > pdfnaut is currently in an early stage of development and has only been tested with a small set of compliant documents. Expect bugs or issues.
 
 pdfnaut is a Python library for parsing PDF 1.7 files.
 
 pdfnaut provides a low-level interface for reading and writing PDF objects as defined in the [PDF 1.7 specification](https://opensource.adobe.com/dc-acrobat-sdk-docs/pdfstandards/PDF32000_2008.pdf). pdfnaut currently does not attempt to deviate from the specification. There's no guarantee that valid documents not fully conforming to the standard will be processed correctly.
 
+## Examples
+
+The newer high-level API
+
+```py
+from pdfnaut import PdfDocument
+
+pdf = PdfDocument.from_filename("tests/docs/sample.pdf")
+first_page = list(pdf.flattened_pages)[0]
+if "Contents" in first_page:
+    first_page_stream = pdf.resolve_reference(first_page["Contents"])
+    print(first_page_stream.decompress())
+```
+
+The more mature low-level API
+
 ```py
 from pdfnaut import PdfParser
 
 with open("tests/docs/sample.pdf", "rb") as doc:
     pdf = PdfParser(doc.read())
     pdf.parse()
 
@@ -233,11 +250,11 @@
     print(first_page_stream.decompress())
 ```
 
 ## Coverage
 
 The following tracks coverage of certain portions of the PDF standard.
 
-- Compression filters: **Supported** (only FlateDecode, ASCII85Decode, and ASCIIHexDecode for now)
+- Compression filters: **Supported** -- FlateDecode, ASCII85, ASCIIHex, Crypt (decode only), and RunLength (decode only).
 - Reading from encrypted PDFs: **Supported** (ARC4 and AES; requires a user-supplied implementation or availability of a compatible module -- `pycryptodome` for now)
 - XRef streams: **Supported**
 - File specifications: **Not supported**
```

### Comparing `pdfnaut-0.2.0/pyproject.toml` & `pdfnaut-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,30 +17,28 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11", 
     "Programming Language :: Python :: 3.12"    
 ]
 dynamic = ["version"]
-dependencies = []
+dependencies = [
+    "typing-extensions >= 4.11.0 ; python_version < '3.11'"
+]
 
 [project.urls]
 homepage = "https://github.com/aescarias/pdfnaut"
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-cov"]
 docs = ["sphinx", "sphinx-copybutton", "sphinx-design", "furo"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 pythonpath = ["."]
 
-[tool.setuptools.packages.find]
-where = ["."]
-include = ["pdfnaut*"]
-
 [tool.setuptools.dynamic]
 version = { attr = "pdfnaut.__version__" }
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pdfnaut-0.2.0/tests/test_encryption.py` & `pdfnaut-0.3.0/tests/test_encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     # TODO: A stream check wouldn't hurt?
     # TODO: Some files have different StmF and StrF filters
     with open("tests/docs/encrypted-arc4.pdf", "rb") as fp:
         parser = PdfParser(fp.read())
         parser.parse()
 
         parser.decrypt("null")
+        assert "Info" in parser.trailer
         metadata = cast("dict[str, Any]", parser.resolve_reference(parser.trailer["Info"]))
         assert metadata["Producer"].value == b"pypdf"
 
     with open("tests/docs/encrypted-aes128.pdf", "rb") as fp:
         parser = PdfParser(fp.read())
         parser.parse()
```

### Comparing `pdfnaut-0.2.0/tests/test_filters.py` & `pdfnaut-0.3.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.2.0/tests/test_object_parsing.py` & `pdfnaut-0.3.0/tests/test_object_parsing.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.2.0/tests/test_parsing_files.py` & `pdfnaut-0.3.0/tests/test_parsing_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,7 +59,22 @@
 
         catalog = parser.resolve_reference(parser.trailer["Root"])
         pages = parser.resolve_reference(catalog["Pages"])
         first_page = parser.resolve_reference(pages["Kids"][0])
         stream = parser.resolve_reference(first_page["Contents"]).decompress()
 
         assert stream.startswith(b"q\n0.000008871 0 595.32 841.92 re\n") 
+
+
+def test_pdf_with_strict_mode() -> None:
+    """Tests a PDF document with a wrong XRef offset. Asserts that it will not open with strict=True."""
+    with pytest.raises(PdfParseError):
+        with open("tests/docs/random-annots.pdf", "rb") as data:
+            parser = PdfParser(data.read(), strict=True)
+            parser.parse()
+
+    with open("tests/docs/random-annots.pdf", "rb") as data:
+        parser = PdfParser(data.read(), strict=False)
+        parser.parse()
+
+        root = parser.resolve_reference(parser.trailer["Root"])
+        assert root["Type"].value == b"Catalog"
```

### Comparing `pdfnaut-0.2.0/tests/test_serializer.py` & `pdfnaut-0.3.0/tests/test_serializer.py`

 * *Files identical despite different names*

