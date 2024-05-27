# Comparing `tmp/librds-1.3.8.tar.gz` & `tmp/librds-1.381.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librds-1.3.8.tar", last modified: Mon May 27 17:39:38 2024, max compression
+gzip compressed data, was "librds-1.381.tar", last modified: Mon May 27 17:47:22 2024, max compression
```

## Comparing `librds-1.3.8.tar` & `librds-1.381.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:39:38.695175 librds-1.3.8/
--rw-rw-rw-   0 root         (0) root         (0)    35187 2024-05-27 16:08:02.000000 librds-1.3.8/LICENCE
--rw-r--r--   0 root         (0) root         (0)     1834 2024-05-27 17:39:38.695175 librds-1.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-27 16:08:02.000000 librds-1.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:39:38.687174 librds-1.3.8/librds/
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-27 17:38:47.000000 librds-1.3.8/librds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-27 16:08:02.000000 librds-1.3.8/librds/af.py
--rw-rw-rw-   0 root         (0) root         (0)    17334 2024-05-27 16:08:02.000000 librds-1.3.8/librds/charset.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-27 16:08:02.000000 librds-1.3.8/librds/comfort.py
--rw-rw-rw-   0 root         (0) root         (0)     4713 2024-05-27 16:08:02.000000 librds-1.3.8/librds/decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     5820 2024-05-27 16:08:02.000000 librds-1.3.8/librds/generator.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-27 16:08:02.000000 librds-1.3.8/librds/group.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-27 17:38:47.000000 librds-1.3.8/librds/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:39:38.691174 librds-1.3.8/librds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1834 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      288 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-27 17:39:38.000000 librds-1.3.8/librds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 17:39:38.695175 librds-1.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-27 17:38:47.000000 librds-1.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:47:22.757978 librds-1.381/
+-rw-rw-rw-   0 root         (0) root         (0)    35187 2024-05-27 16:08:02.000000 librds-1.381/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-05-27 17:47:22.757978 librds-1.381/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-05-27 16:08:02.000000 librds-1.381/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:47:22.753978 librds-1.381/librds/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-27 17:45:26.000000 librds-1.381/librds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-27 16:08:02.000000 librds-1.381/librds/af.py
+-rw-rw-rw-   0 root         (0) root         (0)    17334 2024-05-27 16:08:02.000000 librds-1.381/librds/charset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2024-05-27 16:08:02.000000 librds-1.381/librds/comfort.py
+-rw-rw-rw-   0 root         (0) root         (0)     4713 2024-05-27 16:08:02.000000 librds-1.381/librds/decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     5820 2024-05-27 16:08:02.000000 librds-1.381/librds/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-27 16:08:02.000000 librds-1.381/librds/group.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2024-05-27 17:45:26.000000 librds-1.381/librds/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:47:22.757978 librds-1.381/librds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-05-27 17:47:22.000000 librds-1.381/librds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      288 2024-05-27 17:47:22.000000 librds-1.381/librds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 17:47:22.000000 librds-1.381/librds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-27 17:47:22.000000 librds-1.381/librds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 17:47:22.757978 librds-1.381/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-27 17:46:32.000000 librds-1.381/setup.py
```

### Comparing `librds-1.3.8/LICENCE` & `librds-1.381/LICENCE`

 * *Files identical despite different names*

### Comparing `librds-1.3.8/PKG-INFO` & `librds-1.381/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.3.8
+Version: 1.381
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `librds-1.3.8/README.md` & `librds-1.381/README.md`

 * *Files identical despite different names*

### Comparing `librds-1.3.8/librds/af.py` & `librds-1.381/librds/af.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.8/librds/charset.py` & `librds-1.381/librds/charset.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.8/librds/comfort.py` & `librds-1.381/librds/comfort.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.8/librds/decoder.py` & `librds-1.381/librds/decoder.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.8/librds/generator.py` & `librds-1.381/librds/generator.py`

 * *Files identical despite different names*

### Comparing `librds-1.3.8/librds/interface.py` & `librds-1.381/librds/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         else: text += "\r" # http://www.interactive-radio-system.com/docs/EN50067_RDS_Standard.pdf page 26
         if not full:
             while len(text) % 4: # if we don't have text to equally spread across 4 charcter parts then we add padding
                 text = text + " "
             segments = 0
             for _ in range(len(text)):
                 segments = segments + 0.25 # 1/4 = 0.25 | 0.25*4 = 1
-            if not segments.is_integer(): raise Exception("Segment error (segment is not int)")
+            if not float(segments).is_integer(): raise Exception("Segment error (segment is not int)")
             if int(segments) > 15: return None, None
             return text, int(segments)
         else:
             return text.ljust(64), 16
     def getPTYN(text: str):
         if len(text) > 8: text = text[8:]
         return text.ljust(8), 2
```

### Comparing `librds-1.3.8/librds.egg-info/PKG-INFO` & `librds-1.381/librds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.3.8
+Version: 1.381
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `librds-1.3.8/setup.py` & `librds-1.381/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
         name="librds", 
-        version="1.3.8",
+        version="1.381",
         author="kuba201",
         description='RDS Group Generator',
         long_description=readme,
         long_description_content_type='text/markdown',
         packages=find_packages(),
         url="https://flerken.zapto.org:1115/kuba/librds",
         install_requires=[],
```

