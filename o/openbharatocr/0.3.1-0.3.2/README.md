# Comparing `tmp/openbharatocr-0.3.1.tar.gz` & `tmp/openbharatocr-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbharatocr-0.3.1.tar", last modified: Mon May 27 05:57:55 2024, max compression
+gzip compressed data, was "openbharatocr-0.3.2.tar", last modified: Mon May 27 14:10:38 2024, max compression
```

## Comparing `openbharatocr-0.3.1.tar` & `openbharatocr-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.174043 openbharatocr-0.3.1/openbharatocr/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.174043 openbharatocr-0.3.1/openbharatocr/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/aadhaar.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/driving_licence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/pan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/passport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/vehicle_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/voter_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/water_bill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.174043 openbharatocr-0.3.1/openbharatocr/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/unit_tests/test_pan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/openbharatocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:10:38.944525 openbharatocr-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 14:10:38.944525 openbharatocr-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:10:38.940525 openbharatocr-0.3.2/openbharatocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:10:38.944525 openbharatocr-0.3.2/openbharatocr/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/aadhaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/driving_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/pan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/passport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/vehicle_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/voter_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/ocr/water_bill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:10:38.944525 openbharatocr-0.3.2/openbharatocr/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/unit_tests/test_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/openbharatocr/unit_tests/test_pan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:10:38.944525 openbharatocr-0.3.2/openbharatocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 14:10:38.000000 openbharatocr-0.3.2/openbharatocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-27 14:10:38.000000 openbharatocr-0.3.2/openbharatocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:10:38.000000 openbharatocr-0.3.2/openbharatocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:10:38.000000 openbharatocr-0.3.2/openbharatocr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 14:10:38.000000 openbharatocr-0.3.2/openbharatocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 14:10:38.000000 openbharatocr-0.3.2/openbharatocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 14:10:38.944525 openbharatocr-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-27 14:10:30.000000 openbharatocr-0.3.2/setup.py
```

### Comparing `openbharatocr-0.3.1/LICENSE` & `openbharatocr-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/PKG-INFO` & `openbharatocr-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.3.1
+Version: 0.3.2
 Summary: openbharatocr is an opensource python library for ocr Indian government documents
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openbharatocr-0.3.1/README.md` & `openbharatocr-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/ocr/aadhaar.py` & `openbharatocr-0.3.2/openbharatocr/ocr/aadhaar.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/ocr/driving_licence.py` & `openbharatocr-0.3.2/openbharatocr/ocr/driving_licence.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/ocr/pan.py` & `openbharatocr-0.3.2/openbharatocr/ocr/pan.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/ocr/passport.py` & `openbharatocr-0.3.2/openbharatocr/ocr/passport.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/ocr/vehicle_registration.py` & `openbharatocr-0.3.2/openbharatocr/ocr/vehicle_registration.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/ocr/voter_id.py` & `openbharatocr-0.3.2/openbharatocr/ocr/voter_id.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/ocr/water_bill.py` & `openbharatocr-0.3.2/openbharatocr/ocr/water_bill.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr/unit_tests/test_pan.py` & `openbharatocr-0.3.2/openbharatocr/unit_tests/test_pan.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.1/openbharatocr.egg-info/PKG-INFO` & `openbharatocr-0.3.2/openbharatocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.3.1
+Version: 0.3.2
 Summary: openbharatocr is an opensource python library for ocr Indian government documents
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openbharatocr-0.3.1/openbharatocr.egg-info/SOURCES.txt` & `openbharatocr-0.3.2/openbharatocr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 openbharatocr/ocr/driving_licence.py
 openbharatocr/ocr/pan.py
 openbharatocr/ocr/passport.py
 openbharatocr/ocr/vehicle_registration.py
 openbharatocr/ocr/voter_id.py
 openbharatocr/ocr/water_bill.py
 openbharatocr/unit_tests/__init__.py
+openbharatocr/unit_tests/test_licence.py
 openbharatocr/unit_tests/test_pan.py
```

### Comparing `openbharatocr-0.3.1/setup.py` & `openbharatocr-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="openbharatocr",
-    version="0.3.1",
+    version="0.3.2",
     description="openbharatocr is an opensource python library for ocr Indian government documents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/essentiasoftserv/openbharatocr",
     author="essentiasoftserv",
     python_requires=">=3.6",
     install_requires=install_requires,
```

