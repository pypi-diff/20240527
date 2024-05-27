# Comparing `tmp/binarysearchfile-0.1.0.tar.gz` & `tmp/binarysearchfile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binarysearchfile-0.1.0.tar", last modified: Mon May 13 08:26:45 2024, max compression
+gzip compressed data, was "binarysearchfile-0.2.0.tar", last modified: Mon May 27 13:58:25 2024, max compression
```

## Comparing `binarysearchfile-0.1.0.tar` & `binarysearchfile-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-05-13 08:26:45.663169 binarysearchfile-0.1.0/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     3450 2024-05-13 08:26:45.655169 binarysearchfile-0.1.0/PKG-INFO
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     2904 2024-05-13 08:15:43.000000 binarysearchfile-0.1.0/README.md
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-05-13 08:26:45.639169 binarysearchfile-0.1.0/binarysearchfile.egg-info/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     3450 2024-05-13 08:26:45.000000 binarysearchfile-0.1.0/binarysearchfile.egg-info/PKG-INFO
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      230 2024-05-13 08:26:45.000000 binarysearchfile-0.1.0/binarysearchfile.egg-info/SOURCES.txt
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)        1 2024-05-13 08:26:45.000000 binarysearchfile-0.1.0/binarysearchfile.egg-info/dependency_links.txt
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)       40 2024-05-13 08:26:45.000000 binarysearchfile-0.1.0/binarysearchfile.egg-info/top_level.txt
--rw-rw-r--   0 gi48zar  (15276) bioinf3   (2904)    14936 2024-05-07 12:31:00.000000 binarysearchfile-0.1.0/binarysearchfile.py
--rw-rw-r--   0 gi48zar  (15276) bioinf3   (2904)     4898 2024-05-07 12:30:27.000000 binarysearchfile-0.1.0/binarysearchfile_tests.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      830 2024-05-13 08:08:07.000000 binarysearchfile-0.1.0/pyproject.toml
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)       38 2024-05-13 08:26:45.667169 binarysearchfile-0.1.0/setup.cfg
+drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-05-27 13:58:25.899082 binarysearchfile-0.2.0/
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     2961 2024-05-27 13:58:25.887082 binarysearchfile-0.2.0/PKG-INFO
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     3026 2024-05-27 13:55:23.000000 binarysearchfile-0.2.0/README.md
+drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-05-27 13:58:25.875082 binarysearchfile-0.2.0/binarysearchfile.egg-info/
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     2961 2024-05-27 13:58:25.000000 binarysearchfile-0.2.0/binarysearchfile.egg-info/PKG-INFO
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      239 2024-05-27 13:58:25.000000 binarysearchfile-0.2.0/binarysearchfile.egg-info/SOURCES.txt
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)        1 2024-05-27 13:58:25.000000 binarysearchfile-0.2.0/binarysearchfile.egg-info/dependency_links.txt
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)       40 2024-05-27 13:58:25.000000 binarysearchfile-0.2.0/binarysearchfile.egg-info/top_level.txt
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    15538 2024-05-27 13:55:23.000000 binarysearchfile-0.2.0/binarysearchfile.py
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     5016 2024-05-27 13:55:23.000000 binarysearchfile-0.2.0/binarysearchfile_tests.py
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      819 2024-05-13 09:14:49.000000 binarysearchfile-0.2.0/pyproject.toml
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)       38 2024-05-27 13:58:25.899082 binarysearchfile-0.2.0/setup.cfg
+-rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      366 2024-05-13 09:20:29.000000 binarysearchfile-0.2.0/setup.py
```

### Comparing `binarysearchfile-0.1.0/PKG-INFO` & `binarysearchfile-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 Metadata-Version: 2.1
 Name: binarysearchfile
-Version: 0.1.0
+Version: 0.2.0
 Summary: Binary search binary file for fast random access
 Author: Tom Eulenfeld
 License: MIT License
 Project-URL: Homepage, https://github.com/trichter/binarysearchfile
 Project-URL: Bug Tracker, https://github.com/trichter/binarysearchfile/issues
 Keywords: binary search,random access,direct access
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # binarysearchfile
-[![build status](https://github.com/trichter/binarysearchfile/workflows/tests/badge.svg)](https://github.com/trichter/binarysearchfile/actions)
-[![codecov](https://codecov.io/gh/trichter/binarysearchfile/branch/master/graph/badge.svg)](https://codecov.io/gh/trichter/binarysearchfile)
-[![pypi version](https://img.shields.io/pypi/v/binarysearchfile.svg)](https://pypi.python.org/pypi/binarysearchfile)
-[![python version](https://img.shields.io/pypi/pyversions/binarysearchfile.svg)](https://python.org)
-[![DOI](https://zenodo.org/badge/DOI/)](https://doi.org/)
 
 Binary search sorted binary file for fast random access
 
 ## Usage
 
 Define and use your own binary search file:
 
 ```py
 from binarysearchfile import BinarySearchFile
 
 class MyBinarySearchFile(BinarySearchFile):
     magic = b'\xfe\xff\x01\x01'  # magic string, you can change 2nd and 4th byte
     headerstart = b'MyBinarySearchFile'  # name of the file format
-    record = (10, 10)  # record structure, here two ints, first field can be searched binarily
+    record = (50, 50)  # record structure, here two ints, first field can be searched binarily
 
 bsf = MyBinarySearchFile('mybinarysearchfile')
 data = [(10, 42), (4, 10), (5, 5)]
 bsf.write(data)  # write sorted data
 print(len(bsf))  # number of records
 print(bsf.search(10))  # get index
 print(bsf.get(10))  # get record
@@ -53,23 +48,24 @@
 ```
 
 The example above defines records consisting of two integers.
 The first element ("key") in the record can be searched binarily.
 Currently, the following types can be used out of the box:
 
 ```
-0: ascii
-1: utf-8
-10: int
-11: signedint
+0: binary adding whitepace
+10: ascii adding whitespace
+20: utf-8 adding whitespace
+50: int
+51: signedint
 ```
 
 The file can be read by the original class:
 
-```
+```py
 bsf = BinarySearchFile('mybinarysearchfile')
 print(bsf.get(10))
 
 #Output:
 #(10, 42)
 
 ```
@@ -79,15 +75,15 @@
 ### Defining your own data types
 
 Use the following approach to define additional custom types with the DTypeDef class.
 Its init method takes arguments `name`, `len`, `encode` and `decode`.
 `len`, the byte length of an object, is usually a function of the object, but can be an integer for a fixed length.
 Register custom types only with keys greater than 99.
 
-```
+```py
 from binarysearchfile import BinarySearchFile, DTypeDef
 
 class MyBinarySearchFile(BinarySearchFile):
     DTYPE = BinarySearchFile.DTYPE.copy()
     DTYPE[100] = DTypeDef(
         'fixedlenint', 5,
         encode=lambda v, s: v.to_bytes(s),
@@ -96,14 +92,15 @@
     # definitions of other class properties follow
 ```
 
 ### Use binary sequential file
 
 We provide a `BinarySequentialFile` class that uses the same file layout and can be used for sequential reading and writing.
 
-```
+```py
 from binarysearchfile import BinarySequentialFile
 with BinarySequentialFile('mybinarysearchfile') as bseqf:
     print(bseqf[2])
+
 #Output:
 #(10, 42)
 ```
```

### Comparing `binarysearchfile-0.1.0/README.md` & `binarysearchfile-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # binarysearchfile
 [![build status](https://github.com/trichter/binarysearchfile/workflows/tests/badge.svg)](https://github.com/trichter/binarysearchfile/actions)
 [![codecov](https://codecov.io/gh/trichter/binarysearchfile/branch/master/graph/badge.svg)](https://codecov.io/gh/trichter/binarysearchfile)
 [![pypi version](https://img.shields.io/pypi/v/binarysearchfile.svg)](https://pypi.python.org/pypi/binarysearchfile)
 [![python version](https://img.shields.io/pypi/pyversions/binarysearchfile.svg)](https://python.org)
-[![DOI](https://zenodo.org/badge/DOI/)](https://doi.org/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11184031.svg)](https://doi.org/10.5281/zenodo.11184031)
 
 Binary search sorted binary file for fast random access
 
 ## Usage
 
 Define and use your own binary search file:
 
 ```py
 from binarysearchfile import BinarySearchFile
 
 class MyBinarySearchFile(BinarySearchFile):
     magic = b'\xfe\xff\x01\x01'  # magic string, you can change 2nd and 4th byte
     headerstart = b'MyBinarySearchFile'  # name of the file format
-    record = (10, 10)  # record structure, here two ints, first field can be searched binarily
+    record = (50, 50)  # record structure, here two ints, first field can be searched binarily
 
 bsf = MyBinarySearchFile('mybinarysearchfile')
 data = [(10, 42), (4, 10), (5, 5)]
 bsf.write(data)  # write sorted data
 print(len(bsf))  # number of records
 print(bsf.search(10))  # get index
 print(bsf.get(10))  # get record
@@ -39,23 +39,24 @@
 ```
 
 The example above defines records consisting of two integers.
 The first element ("key") in the record can be searched binarily.
 Currently, the following types can be used out of the box:
 
 ```
-0: ascii
-1: utf-8
-10: int
-11: signedint
+0: binary adding whitepace
+10: ascii adding whitespace
+20: utf-8 adding whitespace
+50: int
+51: signedint
 ```
 
 The file can be read by the original class:
 
-```
+```py
 bsf = BinarySearchFile('mybinarysearchfile')
 print(bsf.get(10))
 
 #Output:
 #(10, 42)
 
 ```
@@ -65,15 +66,15 @@
 ### Defining your own data types
 
 Use the following approach to define additional custom types with the DTypeDef class.
 Its init method takes arguments `name`, `len`, `encode` and `decode`.
 `len`, the byte length of an object, is usually a function of the object, but can be an integer for a fixed length.
 Register custom types only with keys greater than 99.
 
-```
+```py
 from binarysearchfile import BinarySearchFile, DTypeDef
 
 class MyBinarySearchFile(BinarySearchFile):
     DTYPE = BinarySearchFile.DTYPE.copy()
     DTYPE[100] = DTypeDef(
         'fixedlenint', 5,
         encode=lambda v, s: v.to_bytes(s),
@@ -82,14 +83,15 @@
     # definitions of other class properties follow
 ```
 
 ### Use binary sequential file
 
 We provide a `BinarySequentialFile` class that uses the same file layout and can be used for sequential reading and writing.
 
-```
+```py
 from binarysearchfile import BinarySequentialFile
 with BinarySequentialFile('mybinarysearchfile') as bseqf:
     print(bseqf[2])
+
 #Output:
 #(10, 42)
 ```
```

### Comparing `binarysearchfile-0.1.0/binarysearchfile.egg-info/PKG-INFO` & `binarysearchfile-0.2.0/binarysearchfile.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 Metadata-Version: 2.1
 Name: binarysearchfile
-Version: 0.1.0
+Version: 0.2.0
 Summary: Binary search binary file for fast random access
 Author: Tom Eulenfeld
 License: MIT License
 Project-URL: Homepage, https://github.com/trichter/binarysearchfile
 Project-URL: Bug Tracker, https://github.com/trichter/binarysearchfile/issues
 Keywords: binary search,random access,direct access
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # binarysearchfile
-[![build status](https://github.com/trichter/binarysearchfile/workflows/tests/badge.svg)](https://github.com/trichter/binarysearchfile/actions)
-[![codecov](https://codecov.io/gh/trichter/binarysearchfile/branch/master/graph/badge.svg)](https://codecov.io/gh/trichter/binarysearchfile)
-[![pypi version](https://img.shields.io/pypi/v/binarysearchfile.svg)](https://pypi.python.org/pypi/binarysearchfile)
-[![python version](https://img.shields.io/pypi/pyversions/binarysearchfile.svg)](https://python.org)
-[![DOI](https://zenodo.org/badge/DOI/)](https://doi.org/)
 
 Binary search sorted binary file for fast random access
 
 ## Usage
 
 Define and use your own binary search file:
 
 ```py
 from binarysearchfile import BinarySearchFile
 
 class MyBinarySearchFile(BinarySearchFile):
     magic = b'\xfe\xff\x01\x01'  # magic string, you can change 2nd and 4th byte
     headerstart = b'MyBinarySearchFile'  # name of the file format
-    record = (10, 10)  # record structure, here two ints, first field can be searched binarily
+    record = (50, 50)  # record structure, here two ints, first field can be searched binarily
 
 bsf = MyBinarySearchFile('mybinarysearchfile')
 data = [(10, 42), (4, 10), (5, 5)]
 bsf.write(data)  # write sorted data
 print(len(bsf))  # number of records
 print(bsf.search(10))  # get index
 print(bsf.get(10))  # get record
@@ -53,23 +48,24 @@
 ```
 
 The example above defines records consisting of two integers.
 The first element ("key") in the record can be searched binarily.
 Currently, the following types can be used out of the box:
 
 ```
-0: ascii
-1: utf-8
-10: int
-11: signedint
+0: binary adding whitepace
+10: ascii adding whitespace
+20: utf-8 adding whitespace
+50: int
+51: signedint
 ```
 
 The file can be read by the original class:
 
-```
+```py
 bsf = BinarySearchFile('mybinarysearchfile')
 print(bsf.get(10))
 
 #Output:
 #(10, 42)
 
 ```
@@ -79,15 +75,15 @@
 ### Defining your own data types
 
 Use the following approach to define additional custom types with the DTypeDef class.
 Its init method takes arguments `name`, `len`, `encode` and `decode`.
 `len`, the byte length of an object, is usually a function of the object, but can be an integer for a fixed length.
 Register custom types only with keys greater than 99.
 
-```
+```py
 from binarysearchfile import BinarySearchFile, DTypeDef
 
 class MyBinarySearchFile(BinarySearchFile):
     DTYPE = BinarySearchFile.DTYPE.copy()
     DTYPE[100] = DTypeDef(
         'fixedlenint', 5,
         encode=lambda v, s: v.to_bytes(s),
@@ -96,14 +92,15 @@
     # definitions of other class properties follow
 ```
 
 ### Use binary sequential file
 
 We provide a `BinarySequentialFile` class that uses the same file layout and can be used for sequential reading and writing.
 
-```
+```py
 from binarysearchfile import BinarySequentialFile
 with BinarySequentialFile('mybinarysearchfile') as bseqf:
     print(bseqf[2])
+
 #Output:
 #(10, 42)
 ```
```

### Comparing `binarysearchfile-0.1.0/binarysearchfile.py` & `binarysearchfile-0.2.0/binarysearchfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from collections import namedtuple
 from contextlib import contextmanager
 from dataclasses import dataclass
 import os.path
 from warnings import warn
 
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 
 
 def _rint(f, l):
     return int.from_bytes(f.read(l))
 
 
 def _humanb(size, p=2):
@@ -57,24 +57,27 @@
 
 def _byte_length(v):
     return (v.bit_length() + 7) // 8
 
 
 DTypeDef = namedtuple('DType', ['name', 'len', 'encode', 'decode'])
 DTYPE = {
-    0: DTypeDef('ascii', len,
+     0: DTypeDef('byte_ljust', len,
+                 encode=lambda v, s: v.ljust(s, b' '),
+                 decode=lambda v: v.rstrip(b' ')),
+    10: DTypeDef('ascii_ljust', len,
                 encode=lambda v, s: v.encode('latin1').ljust(s, b' '),
                 decode=lambda v: v.rstrip(b' ').decode('latin1')),
-    1: DTypeDef('utf-8', lambda v: len(v.encode('utf-8')),
+    20: DTypeDef('utf-8_ljust', lambda v: len(v.encode('utf-8')),
                 encode=lambda v, s: v.encode('utf-8').ljust(s, b' '),
                 decode=lambda v: v.rstrip(b' ').decode('utf-8')),
-    10: DTypeDef('int', _byte_length,
+    50: DTypeDef('int', _byte_length,
                  encode=lambda v, s: v.to_bytes(s),
                  decode=lambda v: int.from_bytes(v)),
-    11: DTypeDef('signedint', lambda v: _byte_length(2 * abs(v)),
+    51: DTypeDef('signedint', lambda v: _byte_length(2 * abs(v)),
                  encode=lambda v, s: v.to_bytes(s, signed=True),
                  decode=lambda v: int.from_bytes(v, signed=True))
 }
 
 
 @dataclass
 class _Attr:
@@ -102,15 +105,15 @@
     DTYPE = DTYPE
     # should be overriden
     magic = b'\xfe\xfe\x01\x01'
     # 4B follow
     #   2B offset to metadata
     #   2B offset to data
     headerstart = b'BinarySearchFile'
-    record = (0, 10)
+    record = (10, 50)
 
     def __init__(self, fname):
         self.f = None
         self.header = None
         self.size = None
         self.attr = _Attr(fname=fname)
 
@@ -179,17 +182,16 @@
         bytes_ = self.f.read(self.size[0])
         return self.DTYPE[self.record[0]].decode(bytes_)
 
     def _get_data(self, i=None):
         """Get record i or the next record"""
         if i is not None:
             self.f.seek(self.attr.dataoffset + i * self.attr.recsize)
-        data = tuple(self.DTYPE[record].decode(self.f.read(size))
+        return tuple(self.DTYPE[record].decode(self.f.read(size))
                      for record, size in zip(self.record, self.size))
-        return data
 
     def search(self, key, first=True):
         """Search for key and return the record number
 
         :param first: Wether too search for first or last occurence"""
         with self._open():
             self.read_header()
@@ -243,25 +245,36 @@
             f.write(self.magic)
             f.write(b'    ')  # reserve 4 bytes for metaoffset and dataoffset
             f.write(self.headerstart + header)
             metaoffset = f.tell()
 
             f.write(len(self.record).to_bytes(2))
             size = []
-            for i, d in enumerate(zip(*sorted(data))):
-                num = self.record[i]
-                len_ = self.DTYPE[num].len
-                if isinstance(len_, int):
-                    s = len_
-                else:
-                    s = max(len_(d1) for d1 in d)
-                size.append(s)
-                f.write(num.to_bytes(1))
-                f.write(s.to_bytes(2))
-
+            if len(data) == 0:
+                for i in range(len(self.record)):
+                    num = self.record[i]
+                    len_ = self.DTYPE[num].len
+                    if isinstance(len_, int):
+                        s = len_
+                    else:
+                        s = 0
+                    size.append(s)
+                    f.write(num.to_bytes(1))
+                    f.write(s.to_bytes(2))
+            else:
+                for i, d in enumerate(zip(*sorted(data))):
+                    num = self.record[i]
+                    len_ = self.DTYPE[num].len
+                    if isinstance(len_, int):
+                        s = len_
+                    else:
+                        s = max(len_(d1) for d1 in d)
+                    size.append(s)
+                    f.write(num.to_bytes(1))
+                    f.write(s.to_bytes(2))
             dataoffset = f.tell()
             f.seek(len(self.magic))
             f.write(metaoffset.to_bytes(2))
             f.write(dataoffset.to_bytes(2))
             f.seek(dataoffset)
 
             for d in sorted(data):
@@ -298,15 +311,15 @@
 
 
 class BinarySequentialFile():
     DTYPE = DTYPE
 
     magic = b'\xfe\xfe\x01\x01'
     headerstart = b'BinarySequentialFile'
-    record = (0, 10)
+    record = (10, 50)
     size = (20, 2)
 
     def __init__(self, fname, header=b''):
         self.f = None
         self.header = header
         self.attr = _Attr(fname=fname)
         self.open()
@@ -394,17 +407,16 @@
 
     def _sizecheck(self):
         return self.attr.dataoffset + self.attr.len * self.attr.recsize == self.attr.totalsize
 
     def _get_data(self, i=None):
         if i is not None:
             self.f.seek(self.attr.dataoffset + i * self.attr.recsize)
-        data = tuple(self.DTYPE[record].decode(self.f.read(size))
+        return tuple(self.DTYPE[record].decode(self.f.read(size))
                      for record, size in zip(self.record, self.size))
-        return data
 
     def __getitem__(self, item):
         return self.read(item)
 
     def __setitem__(self, item, data):
         return self.write(data, i=item)
```

### Comparing `binarysearchfile-0.1.0/binarysearchfile_tests.py` & `binarysearchfile-0.2.0/binarysearchfile_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,27 @@
             with self.assertWarnsRegex(UserWarning, 'Wrong magic'):
                 self.assertEqual(bsf['test3'], ('test3', 5))
 
     def test_inheritance(self):
         class MyBinarySearchFile(BinarySearchFile):
             magic = b'\xfe\xff\x01\x01'
             headerstart = b'MyBinarySearchFile'
-            record = (10, 10)
+            record = (50, 50)
         with TemporaryDirectory() as tmpdir:
             path = join(tmpdir, 'test.bsf')
             bsf = MyBinarySearchFile(path)
             bsf.write([(10, 10), (4, 10), (5, 5)])
             self.assertEqual(bsf.search(10), 2)
             self.assertIn('MyBinary', str(bsf))
             bsf = BinarySearchFile(path)
             self.assertEqual(bsf.search(10), 2)
 
     def test_inttypes(self):
         class MyBinarySearchFile(BinarySearchFile):
-            record = (10, 11, 10)
+            record = (50, 51, 50)
         data = list(zip(range(256), list(range(-127, 128)) + [127], [0] * 256))
         with TemporaryDirectory() as tmpdir:
             path = join(tmpdir, 'test.bsf')
             bsf = MyBinarySearchFile(path)
             bsf.write(data)
             self.assertEqual(bsf.read(), data)
             self.assertEqual(bsf.attr.recsize, 2)
@@ -74,14 +74,17 @@
             bsf = MyBinarySearchFile(path)
             bsf.write(data)
             self.assertTrue(MyBinarySearchFile.check_magic(path))
             self.assertTrue(BinarySearchFile.check_magic(path))
             self.assertEqual(bsf.read(), data)
             self.assertEqual(bsf.attr.recsize, 4)
             self.assertEqual(bsf.size, [2, 2, 0])
+            self.assertEqual(len(bsf), len(data))
+            bsf.write([])
+            self.assertEqual(len(bsf), 0)
 
     def test_newtypes(self):
         class MyBinarySearchFile(BinarySearchFile):
             DTYPE = BinarySearchFile.DTYPE.copy()
             DTYPE[100] = DTypeDef(
                 'fixedlenint', 5,
                 encode=lambda v, s: v.to_bytes(s),
```

### Comparing `binarysearchfile-0.1.0/pyproject.toml` & `binarysearchfile-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [project]
 name = "binarysearchfile"
-dynamic = ["version"]
+dynamic = ["readme", "version"]
 authors = [
     {name = "Tom Eulenfeld"},
 ]
 description = "Binary search binary file for fast random access"
-readme = "README.md"
 license = {text = "MIT License"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = [
```

