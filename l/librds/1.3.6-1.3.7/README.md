# Comparing `tmp/librds-1.3.6.tar.gz` & `tmp/librds-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librds-1.3.6.tar", last modified: Sun May 26 17:04:17 2024, max compression
+gzip compressed data, was "librds-1.3.7.tar", last modified: Mon May 27 15:29:27 2024, max compression
```

## Comparing `librds-1.3.6.tar` & `librds-1.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 17:04:17.705911 librds-1.3.6/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    35187 2024-05-26 15:33:12.000000 librds-1.3.6/LICENCE
--rw-r--r--   0 kuba      (1000) kuba      (1000)     1619 2024-05-26 17:04:17.705911 librds-1.3.6/PKG-INFO
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1078 2024-05-26 16:55:12.000000 librds-1.3.6/README.md
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 17:04:17.705911 librds-1.3.6/librds/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      255 2024-05-26 17:03:39.000000 librds-1.3.6/librds/__init__.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     3275 2024-05-26 16:50:31.000000 librds-1.3.6/librds/af.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    17372 2024-05-26 16:47:04.000000 librds-1.3.6/librds/charset.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1011 2024-05-25 10:25:25.000000 librds-1.3.6/librds/comfort.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     4713 2024-05-26 16:49:35.000000 librds-1.3.6/librds/decoder.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     5811 2024-05-26 16:56:09.000000 librds-1.3.6/librds/generator.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      601 2024-05-26 16:49:45.000000 librds-1.3.6/librds/group.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1178 2024-05-26 11:07:23.000000 librds-1.3.6/librds/interface.py
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-26 17:04:17.705911 librds-1.3.6/librds.egg-info/
--rw-r--r--   0 kuba      (1000) kuba      (1000)     1619 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/PKG-INFO
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      288 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/SOURCES.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)        1 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/dependency_links.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)        7 2024-05-26 17:04:17.000000 librds-1.3.6/librds.egg-info/top_level.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       38 2024-05-26 17:04:17.705911 librds-1.3.6/setup.cfg
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      851 2024-05-26 17:04:09.000000 librds-1.3.6/setup.py
+drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-27 15:29:27.523499 librds-1.3.7/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)    35187 2024-05-26 15:33:12.000000 librds-1.3.7/LICENCE
+-rw-r--r--   0 kuba      (1000) kuba      (1000)     1681 2024-05-27 15:29:27.523499 librds-1.3.7/PKG-INFO
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1022 2024-05-26 17:05:21.000000 librds-1.3.7/README.md
+drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-27 15:29:27.523499 librds-1.3.7/librds/
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      264 2024-05-27 15:29:04.000000 librds-1.3.7/librds/__init__.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     3279 2024-05-27 15:21:34.000000 librds-1.3.7/librds/af.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)    17334 2024-05-27 15:20:37.000000 librds-1.3.7/librds/charset.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1011 2024-05-25 10:25:25.000000 librds-1.3.7/librds/comfort.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     4713 2024-05-26 16:49:35.000000 librds-1.3.7/librds/decoder.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     5820 2024-05-27 15:19:18.000000 librds-1.3.7/librds/generator.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      417 2024-05-27 15:18:56.000000 librds-1.3.7/librds/group.py
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      872 2024-05-27 15:18:17.000000 librds-1.3.7/librds/interface.py
+drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-27 15:29:27.523499 librds-1.3.7/librds.egg-info/
+-rw-r--r--   0 kuba      (1000) kuba      (1000)     1681 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/PKG-INFO
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)      288 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/SOURCES.txt
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)        1 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/dependency_links.txt
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)        7 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/top_level.txt
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)       38 2024-05-27 15:29:27.523499 librds-1.3.7/setup.cfg
+-rw-rw-r--   0 kuba      (1000) kuba      (1000)     1001 2024-05-27 15:28:18.000000 librds-1.3.7/setup.py
```

### Comparing `librds-1.3.6/LICENCE` & `librds-1.3.7/LICENCE`

 * *Files identical despite different names*

### Comparing `librds-1.3.6/PKG-INFO` & `librds-1.3.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.3.6
+Version: 1.3.7
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
-Keywords: radiodatasystem,rds
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
+Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # LibRDS
-LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library. It is also on [PyPI](https://pypi.org/project/librds/)
+LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library
 
 Example code:
 ```python
 import librds
 
 basic = librds.GroupGenerator.basic(0x3000)
 print(basic)
```

### Comparing `librds-1.3.6/README.md` & `librds-1.3.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # LibRDS
-LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library. It is also on [PyPI](https://pypi.org/project/librds/)
+LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library
 
 Example code:
 ```python
 import librds
 
 basic = librds.GroupGenerator.basic(0x3000)
 print(basic)
```

### Comparing `librds-1.3.6/librds/af.py` & `librds-1.3.7/librds/af.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum, IntEnum
 
 class AF_Codes(Enum):
-    Filler = 205
-    NoAF = 224
-    NumAFSBase = 224 #same as no af
-    LfMf_Follows = 250
+    Filler = 0xCD
+    NoAF = 0xE0
+    NumAFSBase = 0xE0 #same as no af
+    LfMf_Follows = 0xFA
 class AF_Bands(Enum):
     FM = 0
     LF = 1
     MF = 2
     MF_RBDS = 3
 class AlternativeFrequencyEntry:
     """This is a AF Entry which will be used by the AF Class"""
```

### Comparing `librds-1.3.6/librds/charset.py` & `librds-1.3.7/librds/charset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 class RDSCharsetError(Exception): pass
-class RDSCharset: #From version 1.1, don't initilize it
+class RDSCharset:
     def translate(character:str):
         if not type(character) == str: raise RDSCharsetError("Input is not a string")
         elif len(character) != 1: raise RDSCharsetError("This accepts only 1 character.")
         out = 0
         match ord(character):
             case 0xa1: out = 0x8e #INVERTED EXCLAMATION MARK
             case 0xa3: out = 0xaa #POUND SIGN
```

### Comparing `librds-1.3.6/librds/comfort.py` & `librds-1.3.7/librds/comfort.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.6/librds/decoder.py` & `librds-1.3.7/librds/decoder.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.6/librds/generator.py` & `librds-1.3.7/librds/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .group import Group
 from .comfort import get_from_list
 from .af import AlternativeFrequency
-from .charset import *
+from .charset import RDSCharset
 
 class GroupGenerator:
     def basic(pi:int, tp: bool=False, pty: int=0):
         """This function will generate a basic block structure which includes the PI, TP and PTY, this shouldn't be sent by itself to a decoder"""
         return Group(
             pi & 0xFFFF, #A
             (int(tp) << 10 | pty << 5) & 0xFFFF, #B
```

### Comparing `librds-1.3.6/librds.egg-info/PKG-INFO` & `librds-1.3.7/librds.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.3.6
+Version: 1.3.7
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
-Keywords: radiodatasystem,rds
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
+Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # LibRDS
-LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library. It is also on [PyPI](https://pypi.org/project/librds/)
+LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library
 
 Example code:
 ```python
 import librds
 
 basic = librds.GroupGenerator.basic(0x3000)
 print(basic)
```

### Comparing `librds-1.3.6/setup.py` & `librds-1.3.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
         name="librds", 
-        version="1.3.6",
+        version="1.3.7",
         author="kuba201",
         description='RDS Group Generator',
         long_description=readme,
         long_description_content_type='text/markdown',
         packages=find_packages(),
         url="https://flerken.zapto.org:1115/kuba/librds",
         install_requires=[],
-        
-        keywords=['radiodatasystem','rds'],
+        project_urls={
+            'Source': 'https://flerken.zapto.org:1115/kuba/librds',
+        },
+        keywords=['radiodatasystem','rds','broadcast_fm'],
         classifiers= [
-            "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Intended Audience :: Telecommunications Industry",
             "Programming Language :: Python :: 3 :: Only",
             "Programming Language :: Python :: 3.10",
-            "Development Status :: 4 - Beta"
+            "Development Status :: 5 - Production/Stable",
+            "License :: OSI Approved :: GNU General Public License (GPL)",
         ]
 )
```

