# Comparing `tmp/lions-1.4.1.tar.gz` & `tmp/lions-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lions-1.4.1.tar", last modified: Mon May 27 13:17:36 2024, max compression
+gzip compressed data, was "lions-1.4.2.tar", last modified: Mon May 27 13:38:24 2024, max compression
```

## Comparing `lions-1.4.1.tar` & `lions-1.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:17:36.946478 lions-1.4.1/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.4.1/LICENSE
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8474 2024-05-27 13:17:36.946164 lions-1.4.1/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)     7621 2024-05-27 09:43:31.000000 lions-1.4.1/README.md
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:17:36.943066 lions-1.4.1/lions/
--rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.4.1/lions/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3446 2024-05-27 09:43:31.000000 lions-1.4.1/lions/errors.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     5223 2024-05-23 13:46:06.000000 lions-1.4.1/lions/lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     3288 2024-05-27 09:43:31.000000 lions-1.4.1/lions/main.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.4.1/lions/yaml_parser.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:17:36.944267 lions-1.4.1/lions.egg-info/
--rw-r--r--   0 diogoferreira   (501) staff       (20)     8474 2024-05-27 13:17:36.000000 lions-1.4.1/lions.egg-info/PKG-INFO
--rw-r--r--   0 diogoferreira   (501) staff       (20)      452 2024-05-27 13:17:36.000000 lions-1.4.1/lions.egg-info/SOURCES.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-27 13:17:36.000000 lions-1.4.1/lions.egg-info/dependency_links.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-27 13:17:36.000000 lions-1.4.1/lions.egg-info/entry_points.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-27 13:17:36.000000 lions-1.4.1/lions.egg-info/requires.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-27 13:17:36.000000 lions-1.4.1/lions.egg-info/top_level.txt
--rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-27 13:17:36.946676 lions-1.4.1/setup.cfg
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-27 13:16:03.000000 lions-1.4.1/setup.py
-drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:17:36.945611 lions-1.4.1/tests/
--rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.4.1/tests/__init__.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1621 2024-05-27 09:43:31.000000 lions-1.4.1/tests/test_cpp_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1563 2024-05-27 09:43:31.000000 lions-1.4.1/tests/test_js_gen copy.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.4.1/tests/test_lmsg.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1588 2024-05-27 10:00:50.000000 lions-1.4.1/tests/test_python_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     1563 2024-05-27 09:43:31.000000 lions-1.4.1/tests/test_ts_gen.py
--rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.4.1/tests/test_yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:38:24.920873 lions-1.4.2/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1071 2024-04-30 12:52:47.000000 lions-1.4.2/LICENSE
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8474 2024-05-27 13:38:24.920682 lions-1.4.2/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     7621 2024-05-27 09:43:31.000000 lions-1.4.2/README.md
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:38:24.917566 lions-1.4.2/lions/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       23 2024-05-13 08:58:00.000000 lions-1.4.2/lions/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3446 2024-05-27 09:43:31.000000 lions-1.4.2/lions/errors.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     5223 2024-05-23 13:46:06.000000 lions-1.4.2/lions/lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     3288 2024-05-27 09:43:31.000000 lions-1.4.2/lions/main.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     6813 2024-05-10 09:08:10.000000 lions-1.4.2/lions/yaml_parser.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:38:24.918530 lions-1.4.2/lions.egg-info/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     8474 2024-05-27 13:38:24.000000 lions-1.4.2/lions.egg-info/PKG-INFO
+-rw-r--r--   0 diogoferreira   (501) staff       (20)      452 2024-05-27 13:38:24.000000 lions-1.4.2/lions.egg-info/SOURCES.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        1 2024-05-27 13:38:24.000000 lions-1.4.2/lions.egg-info/dependency_links.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       42 2024-05-27 13:38:24.000000 lions-1.4.2/lions.egg-info/entry_points.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       59 2024-05-27 13:38:24.000000 lions-1.4.2/lions.egg-info/requires.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       12 2024-05-27 13:38:24.000000 lions-1.4.2/lions.egg-info/top_level.txt
+-rw-r--r--   0 diogoferreira   (501) staff       (20)       79 2024-05-27 13:38:24.921083 lions-1.4.2/setup.cfg
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1226 2024-05-27 13:37:06.000000 lions-1.4.2/setup.py
+drwxr-xr-x   0 diogoferreira   (501) staff       (20)        0 2024-05-27 13:38:24.920121 lions-1.4.2/tests/
+-rw-r--r--   0 diogoferreira   (501) staff       (20)        0 2024-05-06 14:13:19.000000 lions-1.4.2/tests/__init__.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1621 2024-05-27 09:43:31.000000 lions-1.4.2/tests/test_cpp_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1563 2024-05-27 09:43:31.000000 lions-1.4.2/tests/test_js_gen copy.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     2844 2024-05-23 08:42:03.000000 lions-1.4.2/tests/test_lmsg.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1588 2024-05-27 10:00:50.000000 lions-1.4.2/tests/test_python_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     1563 2024-05-27 09:43:31.000000 lions-1.4.2/tests/test_ts_gen.py
+-rw-r--r--   0 diogoferreira   (501) staff       (20)     4716 2024-05-23 08:42:03.000000 lions-1.4.2/tests/test_yaml_parser.py
```

### Comparing `lions-1.4.1/LICENSE` & `lions-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/PKG-INFO` & `lions-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.4.1
+Version: 1.4.2
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.4.1/README.md` & `lions-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/lions/errors.py` & `lions-1.4.2/lions/errors.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/lions/lmsg.py` & `lions-1.4.2/lions/lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/lions/main.py` & `lions-1.4.2/lions/main.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/lions/yaml_parser.py` & `lions-1.4.2/lions/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/lions.egg-info/PKG-INFO` & `lions-1.4.2/lions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lions
-Version: 1.4.1
+Version: 1.4.2
 Summary: LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.
 Home-page: https://github.com/ItsNotSoftware/lions
 Author: Diogo Ferreira
 Author-email: itsnotsoftware@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lions-1.4.1/setup.py` & `lions-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lions",
-    version="1.4.1",
+    version="1.4.2",
     author="Diogo Ferreira",
     author_email="itsnotsoftware@gmail.com",
     description="LIONS (Lightweight IoT Network Specification) is a communication protocol designed for IoT mesh/ad hoc networks. It facilitates seamless communication between devices and includes code generation based on message files (yaml), streamlining development and implementation processes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"lions": ["cpp_gen/templates/*.jinja"]},
     url="https://github.com/ItsNotSoftware/lions",
```

### Comparing `lions-1.4.1/tests/test_cpp_gen.py` & `lions-1.4.2/tests/test_cpp_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/tests/test_js_gen copy.py` & `lions-1.4.2/tests/test_js_gen copy.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/tests/test_lmsg.py` & `lions-1.4.2/tests/test_lmsg.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/tests/test_python_gen.py` & `lions-1.4.2/tests/test_python_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/tests/test_ts_gen.py` & `lions-1.4.2/tests/test_ts_gen.py`

 * *Files identical despite different names*

### Comparing `lions-1.4.1/tests/test_yaml_parser.py` & `lions-1.4.2/tests/test_yaml_parser.py`

 * *Files identical despite different names*

