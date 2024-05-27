# Comparing `tmp/dvs_printf-1.3.tar.gz` & `tmp/dvs_printf-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvs_printf-1.3.tar", last modified: Mon May 27 05:49:37 2024, max compression
+gzip compressed data, was "dvs_printf-2.0.tar", last modified: Mon May 27 05:34:52 2024, max compression
```

## Comparing `dvs_printf-1.3.tar` & `dvs_printf-2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:49:37.991038 dvs_printf-1.3/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1070 2024-04-04 03:31:22.000000 dvs_printf-1.3/LICENSE
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       73 2024-05-27 04:55:17.000000 dvs_printf-1.3/MANIFEST.in
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4617 2024-05-27 05:49:37.990821 dvs_printf-1.3/PKG-INFO
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3818 2024-05-26 15:52:22.000000 dvs_printf-1.3/README.md
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:49:37.986244 dvs_printf-1.3/dvs_printf/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     6148 2024-05-25 15:56:41.000000 dvs_printf-1.3/dvs_printf/.DS_Store
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3066 2024-04-07 04:48:27.000000 dvs_printf-1.3/dvs_printf/__Loding__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4377 2024-05-09 03:52:50.000000 dvs_printf-1.3/dvs_printf/__init.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1242 2024-05-27 04:40:02.000000 dvs_printf-1.3/dvs_printf/__init__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10693 2024-05-27 04:39:53.000000 dvs_printf-1.3/dvs_printf/__printf__.py
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:49:37.988880 dvs_printf-1.3/dvs_printf/__pycache__/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     2977 2024-04-07 12:04:37.000000 dvs_printf-1.3/dvs_printf/__pycache__/Loding.cpython-310.pyc
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     2981 2024-05-25 03:20:22.000000 dvs_printf-1.3/dvs_printf/__pycache__/__Loding__.cpython-310.pyc
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4959 2024-05-09 03:53:25.000000 dvs_printf-1.3/dvs_printf/__pycache__/__init.cpython-310.pyc
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1439 2024-05-25 03:20:22.000000 dvs_printf-1.3/dvs_printf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     8046 2024-05-25 06:45:57.000000 dvs_printf-1.3/dvs_printf/__pycache__/__printf__.cpython-310.pyc
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     8286 2024-05-25 04:28:46.000000 dvs_printf-1.3/dvs_printf/__pycache__/oth_styles.cpython-310.pyc
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10813 2024-05-25 04:28:33.000000 dvs_printf-1.3/dvs_printf/oth_styles.py
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:49:37.990572 dvs_printf-1.3/dvs_printf.egg-info/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4617 2024-05-27 05:49:37.000000 dvs_printf-1.3/dvs_printf.egg-info/PKG-INFO
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      803 2024-05-27 05:49:37.000000 dvs_printf-1.3/dvs_printf.egg-info/SOURCES.txt
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-05-27 05:49:37.000000 dvs_printf-1.3/dvs_printf.egg-info/dependency_links.txt
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       11 2024-05-27 05:49:37.000000 dvs_printf-1.3/dvs_printf.egg-info/top_level.txt
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      104 2024-05-27 04:55:17.000000 dvs_printf-1.3/pyproject.toml
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)       38 2024-05-27 05:49:37.991082 dvs_printf-1.3/setup.cfg
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1022 2024-05-27 05:45:19.000000 dvs_printf-1.3/setup.py
-drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:49:37.990363 dvs_printf-1.3/tests/
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      880 2024-05-25 04:32:10.000000 dvs_printf-1.3/tests/test_Numpy.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      968 2024-04-04 03:31:22.000000 dvs_printf-1.3/tests/test_Pandas.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      962 2024-04-04 03:31:22.000000 dvs_printf-1.3/tests/test_PyTorch.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1223 2024-05-25 03:57:35.000000 dvs_printf-1.3/tests/test_Tensorflow.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      885 2024-05-20 04:30:21.000000 dvs_printf-1.3/tests/test__init__.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      372 2024-04-04 03:31:22.000000 dvs_printf-1.3/tests/test_arrayToList.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1543 2024-05-20 03:51:25.000000 dvs_printf-1.3/tests/test_listfunction.py
--rw-r--r--   0 vyasdhruvan   (501) staff       (20)      210 2024-04-04 03:31:22.000000 dvs_printf-1.3/tests/test_loding.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:34:52.288030 dvs_printf-2.0/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1070 2024-04-04 03:31:22.000000 dvs_printf-2.0/LICENSE
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       73 2024-05-27 04:55:17.000000 dvs_printf-2.0/MANIFEST.in
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4617 2024-05-27 05:34:52.287825 dvs_printf-2.0/PKG-INFO
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3818 2024-05-26 15:52:22.000000 dvs_printf-2.0/README.md
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:34:52.283435 dvs_printf-2.0/dvs_printf/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     6148 2024-05-25 15:56:41.000000 dvs_printf-2.0/dvs_printf/.DS_Store
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     3066 2024-04-07 04:48:27.000000 dvs_printf-2.0/dvs_printf/__Loding__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4377 2024-05-09 03:52:50.000000 dvs_printf-2.0/dvs_printf/__init.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1242 2024-05-27 04:40:02.000000 dvs_printf-2.0/dvs_printf/__init__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10693 2024-05-27 04:39:53.000000 dvs_printf-2.0/dvs_printf/__printf__.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:34:52.286012 dvs_printf-2.0/dvs_printf/__pycache__/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     2977 2024-04-07 12:04:37.000000 dvs_printf-2.0/dvs_printf/__pycache__/Loding.cpython-310.pyc
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     2981 2024-05-25 03:20:22.000000 dvs_printf-2.0/dvs_printf/__pycache__/__Loding__.cpython-310.pyc
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4959 2024-05-09 03:53:25.000000 dvs_printf-2.0/dvs_printf/__pycache__/__init.cpython-310.pyc
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1439 2024-05-25 03:20:22.000000 dvs_printf-2.0/dvs_printf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     8046 2024-05-25 06:45:57.000000 dvs_printf-2.0/dvs_printf/__pycache__/__printf__.cpython-310.pyc
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     8286 2024-05-25 04:28:46.000000 dvs_printf-2.0/dvs_printf/__pycache__/oth_styles.cpython-310.pyc
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)    10813 2024-05-25 04:28:33.000000 dvs_printf-2.0/dvs_printf/oth_styles.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:34:52.287603 dvs_printf-2.0/dvs_printf.egg-info/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     4617 2024-05-27 05:34:52.000000 dvs_printf-2.0/dvs_printf.egg-info/PKG-INFO
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      803 2024-05-27 05:34:52.000000 dvs_printf-2.0/dvs_printf.egg-info/SOURCES.txt
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)        1 2024-05-27 05:34:52.000000 dvs_printf-2.0/dvs_printf.egg-info/dependency_links.txt
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       11 2024-05-27 05:34:52.000000 dvs_printf-2.0/dvs_printf.egg-info/top_level.txt
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      104 2024-05-27 04:55:17.000000 dvs_printf-2.0/pyproject.toml
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)       38 2024-05-27 05:34:52.288079 dvs_printf-2.0/setup.cfg
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1099 2024-05-27 05:31:49.000000 dvs_printf-2.0/setup.py
+drwxr-xr-x   0 vyasdhruvan   (501) staff       (20)        0 2024-05-27 05:34:52.287410 dvs_printf-2.0/tests/
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      880 2024-05-25 04:32:10.000000 dvs_printf-2.0/tests/test_Numpy.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      968 2024-04-04 03:31:22.000000 dvs_printf-2.0/tests/test_Pandas.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      962 2024-04-04 03:31:22.000000 dvs_printf-2.0/tests/test_PyTorch.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1223 2024-05-25 03:57:35.000000 dvs_printf-2.0/tests/test_Tensorflow.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      885 2024-05-20 04:30:21.000000 dvs_printf-2.0/tests/test__init__.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      372 2024-04-04 03:31:22.000000 dvs_printf-2.0/tests/test_arrayToList.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)     1543 2024-05-20 03:51:25.000000 dvs_printf-2.0/tests/test_listfunction.py
+-rw-r--r--   0 vyasdhruvan   (501) staff       (20)      210 2024-04-04 03:31:22.000000 dvs_printf-2.0/tests/test_loding.py
```

### Comparing `dvs_printf-1.3/LICENSE` & `dvs_printf-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/PKG-INFO` & `dvs_printf-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvs_printf
-Version: 1.3
+Version: 2.0
 Summary: Animated Visual appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf
 Author: dhruvan_vyas
 License: MIT License
 Project-URL: Documentation, https://github.com/dhruvan-vyas/dvs_printf/blob/main/README.md
 Project-URL: hii, https://pypi.org/project/dvs-printf
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvs_printf Version: 1.3 Summary: Animated Visual
+Metadata-Version: 2.1 Name: dvs_printf Version: 2.0 Summary: Animated Visual
 appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf Author: dhruvan_vyas
 License: MIT License Project-URL: Documentation, https://github.com/dhruvan-
 vyas/dvs_printf/blob/main/README.md Project-URL: hii, https://pypi.org/project/
 dvs-printf Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `dvs_printf-1.3/README.md` & `dvs_printf-2.0/README.md`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/.DS_Store` & `dvs_printf-2.0/dvs_printf/.DS_Store`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__Loding__.py` & `dvs_printf-2.0/dvs_printf/__Loding__.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__init.py` & `dvs_printf-2.0/dvs_printf/__init.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__init__.py` & `dvs_printf-2.0/dvs_printf/__init__.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__printf__.py` & `dvs_printf-2.0/dvs_printf/__printf__.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__pycache__/Loding.cpython-310.pyc` & `dvs_printf-2.0/dvs_printf/__pycache__/Loding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__pycache__/__Loding__.cpython-310.pyc` & `dvs_printf-2.0/dvs_printf/__pycache__/__Loding__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__pycache__/__init.cpython-310.pyc` & `dvs_printf-2.0/dvs_printf/__pycache__/__init.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__pycache__/__init__.cpython-310.pyc` & `dvs_printf-2.0/dvs_printf/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__pycache__/__printf__.cpython-310.pyc` & `dvs_printf-2.0/dvs_printf/__pycache__/__printf__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/__pycache__/oth_styles.cpython-310.pyc` & `dvs_printf-2.0/dvs_printf/__pycache__/oth_styles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf/oth_styles.py` & `dvs_printf-2.0/dvs_printf/oth_styles.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/dvs_printf.egg-info/PKG-INFO` & `dvs_printf-2.0/dvs_printf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvs_printf
-Version: 1.3
+Version: 2.0
 Summary: Animated Visual appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf
 Author: dhruvan_vyas
 License: MIT License
 Project-URL: Documentation, https://github.com/dhruvan-vyas/dvs_printf/blob/main/README.md
 Project-URL: hii, https://pypi.org/project/dvs-printf
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvs_printf Version: 1.3 Summary: Animated Visual
+Metadata-Version: 2.1 Name: dvs_printf Version: 2.0 Summary: Animated Visual
 appearance for console-based applications, with different animation styles
 Home-page: https://github.com/dhruvan-vyas/dvs_printf Author: dhruvan_vyas
 License: MIT License Project-URL: Documentation, https://github.com/dhruvan-
 vyas/dvs_printf/blob/main/README.md Project-URL: hii, https://pypi.org/project/
 dvs-printf Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python ::
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `dvs_printf-1.3/dvs_printf.egg-info/SOURCES.txt` & `dvs_printf-2.0/dvs_printf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/setup.py` & `dvs_printf-2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import pathlib, setuptools
 
 setuptools.setup(
     name="dvs_printf",
-    version="1.3",
+
+
+    version="2.0", #===========XXXIJAjjjrojqwgjqrojjqriojerjjfjeqrjfslkdjfalsj>>>>>>>>++++
+
+
+
     description=
 "Animated Visual appearance for console-based applications, with different animation styles",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/dhruvan-vyas/dvs_printf",
     author="dhruvan_vyas",
     license="MIT License",
```

### Comparing `dvs_printf-1.3/tests/test_Numpy.py` & `dvs_printf-2.0/tests/test_Numpy.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/tests/test_Pandas.py` & `dvs_printf-2.0/tests/test_Pandas.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/tests/test_PyTorch.py` & `dvs_printf-2.0/tests/test_PyTorch.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/tests/test_Tensorflow.py` & `dvs_printf-2.0/tests/test_Tensorflow.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/tests/test__init__.py` & `dvs_printf-2.0/tests/test__init__.py`

 * *Files identical despite different names*

### Comparing `dvs_printf-1.3/tests/test_listfunction.py` & `dvs_printf-2.0/tests/test_listfunction.py`

 * *Files identical despite different names*

