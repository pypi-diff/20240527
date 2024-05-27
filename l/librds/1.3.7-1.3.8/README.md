# Comparing `tmp/librds-1.3.7.tar.gz` & `tmp/librds-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librds-1.3.7.tar", last modified: Mon May 27 15:29:27 2024, max compression
+gzip compressed data, was "librds-1.3.8.tar", last modified: Mon May 27 17:39:38 2024, max compression
```

## Comparing `librds-1.3.7.tar` & `librds-1.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-27 15:29:27.523499 librds-1.3.7/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    35187 2024-05-26 15:33:12.000000 librds-1.3.7/LICENCE
--rw-r--r--   0 kuba      (1000) kuba      (1000)     1681 2024-05-27 15:29:27.523499 librds-1.3.7/PKG-INFO
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1022 2024-05-26 17:05:21.000000 librds-1.3.7/README.md
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-27 15:29:27.523499 librds-1.3.7/librds/
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      264 2024-05-27 15:29:04.000000 librds-1.3.7/librds/__init__.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     3279 2024-05-27 15:21:34.000000 librds-1.3.7/librds/af.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)    17334 2024-05-27 15:20:37.000000 librds-1.3.7/librds/charset.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1011 2024-05-25 10:25:25.000000 librds-1.3.7/librds/comfort.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     4713 2024-05-26 16:49:35.000000 librds-1.3.7/librds/decoder.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     5820 2024-05-27 15:19:18.000000 librds-1.3.7/librds/generator.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      417 2024-05-27 15:18:56.000000 librds-1.3.7/librds/group.py
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      872 2024-05-27 15:18:17.000000 librds-1.3.7/librds/interface.py
-drwxrwxr-x   0 kuba      (1000) kuba      (1000)        0 2024-05-27 15:29:27.523499 librds-1.3.7/librds.egg-info/
--rw-r--r--   0 kuba      (1000) kuba      (1000)     1681 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/PKG-INFO
--rw-rw-r--   0 kuba      (1000) kuba      (1000)      288 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/SOURCES.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)        1 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/dependency_links.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)        7 2024-05-27 15:29:27.000000 librds-1.3.7/librds.egg-info/top_level.txt
--rw-rw-r--   0 kuba      (1000) kuba      (1000)       38 2024-05-27 15:29:27.523499 librds-1.3.7/setup.cfg
--rw-rw-r--   0 kuba      (1000) kuba      (1000)     1001 2024-05-27 15:28:18.000000 librds-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:39:38.695175 librds-1.3.8/
+-rw-rw-rw-   0 root         (0) root         (0)    35187 2024-05-27 16:08:02.000000 librds-1.3.8/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-05-27 17:39:38.695175 librds-1.3.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-27 16:08:02.000000 librds-1.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:39:38.687174 librds-1.3.8/librds/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-27 17:38:47.000000 librds-1.3.8/librds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-27 16:08:02.000000 librds-1.3.8/librds/af.py
+-rw-rw-rw-   0 root         (0) root         (0)    17334 2024-05-27 16:08:02.000000 librds-1.3.8/librds/charset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-27 16:08:02.000000 librds-1.3.8/librds/comfort.py
+-rw-rw-rw-   0 root         (0) root         (0)     4713 2024-05-27 16:08:02.000000 librds-1.3.8/librds/decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5820 2024-05-27 16:08:02.000000 librds-1.3.8/librds/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-27 16:08:02.000000 librds-1.3.8/librds/group.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-27 17:38:47.000000 librds-1.3.8/librds/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:39:38.691174 librds-1.3.8/librds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      288 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 17:39:38.695175 librds-1.3.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-27 17:38:47.000000 librds-1.3.8/setup.py
```

### Comparing `librds-1.3.7/LICENCE` & `librds-1.3.8/LICENCE`

 * *Files identical despite different names*

### Comparing `librds-1.3.7/PKG-INFO` & `librds-1.3.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.3.7
+Version: 1.3.8
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # LibRDS
+[![pipeline status](https://flerken.zapto.org:1115/kuba/librds/badges/main/pipeline.svg)](https://flerken.zapto.org:1115/kuba/librds/-/commits/main)<br>
 LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library
 
 Example code:
 ```python
 import librds
 
 basic = librds.GroupGenerator.basic(0x3000)
```

### Comparing `librds-1.3.7/librds/af.py` & `librds-1.3.8/librds/af.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.7/librds/charset.py` & `librds-1.3.8/librds/charset.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.7/librds/comfort.py` & `librds-1.3.8/librds/comfort.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.7/librds/decoder.py` & `librds-1.3.8/librds/decoder.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.7/librds/generator.py` & `librds-1.3.8/librds/generator.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.7/librds/interface.py` & `librds-1.3.8/librds/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 class GroupInterface:
     def getPS(text: str):
         return text[8:].ljust(8), 4
     def getRT(text: str,full:bool=False):
-        if len(text) > 64: text = text[64:]
+        if len(text) >= 64: text = text[64:]
         else: text += "\r" # http://www.interactive-radio-system.com/docs/EN50067_RDS_Standard.pdf page 26
         if not full:
             while len(text) % 4: # if we don't have text to equally spread across 4 charcter parts then we add padding
                 text = text + " "
             segments = 0
             for _ in range(len(text)):
                 segments = segments + 0.25 # 1/4 = 0.25 | 0.25*4 = 1
             if not segments.is_integer(): raise Exception("Segment error (segment is not int)")
+            if int(segments) > 15: return None, None
             return text, int(segments)
         else:
             return text.ljust(64), 16
     def getPTYN(text: str):
         if len(text) > 8: text = text[8:]
         return text.ljust(8), 2
```

### Comparing `librds-1.3.7/librds.egg-info/PKG-INFO` & `librds-1.3.8/librds.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.3.7
+Version: 1.3.8
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # LibRDS
+[![pipeline status](https://flerken.zapto.org:1115/kuba/librds/badges/main/pipeline.svg)](https://flerken.zapto.org:1115/kuba/librds/-/commits/main)<br>
 LibRDS is a simple library that you can use to generate the RDS groups, just the groups, so something like `3000 2000 7575 7575` the origins of development of this started on 12 May, later creating the [rdPy](https://github.com/KubaPro010/rdPy) repository, here it is mostly similiar code but improved and packaged as a library
 
 Example code:
 ```python
 import librds
 
 basic = librds.GroupGenerator.basic(0x3000)
```

### Comparing `librds-1.3.7/setup.py` & `librds-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
         name="librds", 
-        version="1.3.7",
+        version="1.3.8",
         author="kuba201",
         description='RDS Group Generator',
         long_description=readme,
         long_description_content_type='text/markdown',
         packages=find_packages(),
         url="https://flerken.zapto.org:1115/kuba/librds",
         install_requires=[],
```

